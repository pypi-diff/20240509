# Comparing `tmp/firebird_qa-0.19.3.tar.gz` & `tmp/firebird_qa-0.20.0.tar.gz`

## Comparing `firebird_qa-0.19.3.tar` & `firebird_qa-0.20.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 firebird_qa-0.19.3/src/firebird/qa/__about__.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 firebird_qa-0.19.3/src/firebird/qa/__init__.py
--rw-r--r--   0        0        0    19703 2020-02-02 00:00:00.000000 firebird_qa-0.19.3/src/firebird/qa/fbtconv.py
--rw-r--r--   0        0        0   121896 2020-02-02 00:00:00.000000 firebird_qa-0.19.3/src/firebird/qa/plugin.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 firebird_qa-0.19.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 firebird_qa-0.19.3/LICENSE
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 firebird_qa-0.19.3/PLUGIN-README.md
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 firebird_qa-0.19.3/pyproject.toml
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 firebird_qa-0.19.3/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 firebird_qa-0.20.0/src/firebird/qa/__about__.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 firebird_qa-0.20.0/src/firebird/qa/__init__.py
+-rw-r--r--   0        0        0    19703 2020-02-02 00:00:00.000000 firebird_qa-0.20.0/src/firebird/qa/fbtconv.py
+-rw-r--r--   0        0        0   123738 2020-02-02 00:00:00.000000 firebird_qa-0.20.0/src/firebird/qa/plugin.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 firebird_qa-0.20.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 firebird_qa-0.20.0/LICENSE
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 firebird_qa-0.20.0/PLUGIN-README.md
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 firebird_qa-0.20.0/pyproject.toml
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 firebird_qa-0.20.0/PKG-INFO
```

### Comparing `firebird_qa-0.19.3/src/firebird/qa/__init__.py` & `firebird_qa-0.20.0/src/firebird/qa/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 """firebird-qa - Firebird QA module
 
 
 """
 
 from .plugin import db_factory, Database, user_factory, User, isql_act, python_act, Action, \
      temp_file, temp_files, role_factory, Role, envar_factory, Envar, Mapping, mapping_factory, \
-     ServerKeeper, ExecutionError, QA_GLOBALS
+     ServerKeeper, ExecutionError, QA_GLOBALS, existing_db_factory
```

### Comparing `firebird_qa-0.19.3/src/firebird/qa/fbtconv.py` & `firebird_qa-0.20.0/src/firebird/qa/fbtconv.py`

 * *Files identical despite different names*

### Comparing `firebird_qa-0.19.3/src/firebird/qa/plugin.py` & `firebird_qa-0.20.0/src/firebird/qa/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,14 +508,16 @@
                 selected.append(item)
             else:
                 if skip in [SKIP_VERSION, SKIP_ANY]:
                     selected.append(item)
                     item.add_marker(version_skip)
                 else:
                     deselected.append(item)
+        elif platform_ok:
+            selected.append(item)
     items[:] = selected
     config.hook.pytest_deselected(items=deselected)
     # Add OUR OWN test metadata to Item
     for item in items:
         item._qa_id_ = item.nodeid
         item._qa_issue_ = None
         item._qa_jira_ = None
@@ -882,14 +884,46 @@
             srv.database.set_write_mode(database=self.db_path, mode=DbWriteMode.ASYNC)
     def set_sync_write(self) -> None:
         "Set the database to `sync write` mode."
         __tracebackhide__ = True
         with connect_server(_vars_['server']) as srv:
             srv.database.set_write_mode(database=self.db_path, mode=DbWriteMode.SYNC)
 
+def existing_db_factory(*, filename: str='test.fdb', charset: Optional[str]=None,
+                        user: Optional[str]=None, password: Optional[str]=None,
+                        config_name: str='pytest', utf8filename: bool=False):
+    """Factory function that returns :doc:`fixture <pytest:explanation/fixtures>` providing
+    the `Database` instance to existing database.
+
+    Arguments:
+        filename: Test database filename. It's also possible to specify database alias using
+            '#' as prefix, for example `#employee` means alias `employee`.
+            The database with this alias must be defined in `databases.conf`.
+        charset: Default charset for connections.
+        user: User name used to connect the test database. Default is taken from server configuration.
+        password: User password used to connect the test database. Default
+            is taken from server configuration.
+        config_name: Name for database configuration.
+        utf8filename: Use utf8filename DPB flag.
+
+    .. note::
+
+       The returned instance must be assigned to module-level variable. Name of this variable
+       is important, as it's used to reference the fixture in other fixture-factory functions
+       that use the database, and the test function itself.
+    """
+
+    @pytest.fixture
+    def existing_database_fixture(request: pytest.FixtureRequest) -> Database:
+        db = Database(_vars_['databases'], filename, user, password, charset, debug=str(request.module),
+                      config_name=config_name, utf8filename=utf8filename)
+        yield db
+
+    return existing_database_fixture
+
 def db_factory(*, filename: str='test.fdb', init: Optional[str]=None,
                from_backup: Optional[str]=None, copy_of: Optional[str]=None,
                page_size: Optional[int]=None, sql_dialect: Optional[int]=None,
                charset: Optional[str]=None, user: Optional[str]=None,
                password: Optional[str]=None, do_not_create: bool=False,
                do_not_drop: bool=False, async_write: bool=True,
                config_name: str='pytest', utf8filename: bool=False):
@@ -1775,15 +1809,15 @@
             params.extend(['-user', self.db.user, '-password', self.db.password, str(self.db.dsn)])
         if combine_output:
             result: CompletedProcess = run(params, input=substitute_macros(self.script, self.db.subs),
                                            encoding=io_enc, stdout=PIPE, stderr=STDOUT)
         else:
             result: CompletedProcess = run(params, input=self.script,
                                            encoding=io_enc, capture_output=True)
-        if result.returncode and not bool(self.expected_stderr) and not combine_output:
+        if (result.returncode or result.stderr) and not bool(self.expected_stderr) and not combine_output:
             self._node.add_report_section('call', 'ISQL stdout', result.stdout)
             self._node.add_report_section('call', 'ISQL stderr', result.stderr)
             raise ExecutionError("Test script execution failed")
 
         self.return_code: int = result.returncode
         self.stdout: str = result.stdout
         self.stderr: str = result.stderr
@@ -1889,15 +1923,15 @@
         params = [_vars_['gstat']]
         if credentials:
             params.extend(['-user', self.db.user, '-password', self.db.password])
         params.extend(switches)
         if connect_db:
             params.append(str(self.db.dsn))
         result: CompletedProcess = run(params, encoding=io_enc, capture_output=True)
-        if result.returncode and not bool(self.expected_stderr):
+        if (result.returncode or result.stderr) and not bool(self.expected_stderr):
             self._node.add_report_section('call', 'gstat stdout', result.stdout)
             self._node.add_report_section('call', 'gstat stderr', result.stderr)
             raise ExecutionError("gstat execution failed")
         self.return_code: int = result.returncode
         self.stdout: str = result.stdout
         self.stderr: str = result.stderr
         # Store output
@@ -1953,15 +1987,15 @@
         params = [_vars_['gsec']]
         if switches is not None:
             params.extend(switches)
         if credentials:
             params.extend(['-user', self.db.user, '-password', self.db.password])
         result: CompletedProcess = run(params, input=input,
                                        encoding=io_enc, capture_output=True)
-        if result.returncode and not bool(self.expected_stderr):
+        if (result.returncode or result.stderr) and not bool(self.expected_stderr):
             self._node.add_report_section('call', 'gsec stdout', result.stdout)
             self._node.add_report_section('call', 'gsec stderr', result.stderr)
             raise ExecutionError("gsec execution failed")
         self.return_code: int = result.returncode
         self.stdout: str = result.stdout
         self.stderr: str = result.stderr
         # Store output
@@ -2017,15 +2051,15 @@
             params.extend(['-user', self.db.user, '-password', self.db.password])
         if switches is not None:
             params.extend(switches)
         if combine_output:
             result: CompletedProcess = run(params, encoding=io_enc, stdout=PIPE, stderr=STDOUT)
         else:
             result: CompletedProcess = run(params, encoding=io_enc, capture_output=True)
-        if result.returncode and not (bool(self.expected_stderr) or combine_output):
+        if (result.returncode or result.stderr) and not (bool(self.expected_stderr) or combine_output):
             self._node.add_report_section('call', 'gbak stdout', result.stdout)
             self._node.add_report_section('call', 'gbak stderr', result.stderr)
             raise ExecutionError("gbak execution failed")
         self.return_code: int = result.returncode
         self.stdout: str = result.stdout
         self.stderr: str = result.stderr
         # Store output
@@ -2080,15 +2114,15 @@
         params.extend(switches)
         if credentials:
             params.extend(['-user', self.db.user, '-password', self.db.password])
         if combine_output:
             result: CompletedProcess = run(params, encoding=io_enc, stdout=PIPE, stderr=STDOUT)
         else:
             result: CompletedProcess = run(params, encoding=io_enc, capture_output=True)
-        if result.returncode and not (bool(self.expected_stderr) or combine_output):
+        if (result.returncode or result.stderr) and not (bool(self.expected_stderr) or combine_output):
             self._node.add_report_section('call', 'nbackup stdout', result.stdout)
             self._node.add_report_section('call', 'nbackup stderr', result.stderr)
             raise ExecutionError("nbackup execution failed")
         self.return_code: int = result.returncode
         self.stdout: str = result.stdout
         self.stderr: str = result.stderr
         # Store output
@@ -2144,15 +2178,15 @@
             params.extend(switches)
         if credentials:
             params.extend(['-user', self.db.user, '-password', self.db.password])
         if combine_output:
             result: CompletedProcess = run(params, encoding=io_enc, stdout=PIPE, stderr=STDOUT)
         else:
             result: CompletedProcess = run(params, encoding=io_enc, capture_output=True)
-        if result.returncode and not (bool(self.expected_stderr) or combine_output):
+        if (result.returncode or result.stderr) and not (bool(self.expected_stderr) or combine_output):
             self._node.add_report_section('call', 'gfix stdout', result.stdout)
             self._node.add_report_section('call', 'gfix stderr', result.stderr)
             raise ExecutionError("gfix execution failed")
         self.return_code: int = result.returncode
         self.stdout: str = result.stdout
         self.stderr: str = result.stderr
         # Store output
@@ -2222,15 +2256,15 @@
             params.append(str(db.dsn))
         if combine_output:
             result: CompletedProcess = run(params, input=input,
                                            encoding=io_enc, stdout=PIPE, stderr=STDOUT)
         else:
             result: CompletedProcess = run(params, input=input,
                                            encoding=io_enc, capture_output=True)
-        if result.returncode and not (bool(self.expected_stderr) or combine_output):
+        if (result.returncode or result.stderr) and not (bool(self.expected_stderr) or combine_output):
             self._node.add_report_section('call', 'ISQL stdout', result.stdout)
             self._node.add_report_section('call', 'ISQL stderr', result.stderr)
             raise ExecutionError("ISQL execution failed")
         self.return_code: int = result.returncode
         self.stdout: str = result.stdout
         self.stderr: str = result.stderr
         # Store output
@@ -2285,15 +2319,15 @@
         params = [_vars_['fbsvcmgr']]
         if connect_mngr:
             params.extend([f"{_vars_['host']}:service_mgr" if _vars_['host'] else 'service_mgr',
                            'user', self.db.user, 'password', self.db.password])
         if switches is not None:
             params.extend(switches)
         result: CompletedProcess = run(params, encoding=io_enc, capture_output=True)
-        if result.returncode and not bool(self.expected_stderr):
+        if (result.returncode or result.stderr) and not bool(self.expected_stderr):
             self._node.add_report_section('call', 'fbsvcmgr stdout', result.stdout)
             self._node.add_report_section('call', 'fbsvcmgr stderr', result.stderr)
             raise ExecutionError("fbsvcmgr execution failed")
         self.return_code: int = result.returncode
         self.stdout: str = result.stdout
         self.stderr: str = result.stderr
         # Store output
```

### Comparing `firebird_qa-0.19.3/.gitignore` & `firebird_qa-0.20.0/.gitignore`

 * *Files identical despite different names*

### Comparing `firebird_qa-0.19.3/LICENSE` & `firebird_qa-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firebird_qa-0.19.3/PLUGIN-README.md` & `firebird_qa-0.20.0/PLUGIN-README.md`

 * *Files identical despite different names*

### Comparing `firebird_qa-0.19.3/pyproject.toml` & `firebird_qa-0.20.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Topic :: Database :: Database Engines/Servers",
     "Topic :: Software Development :: Testing",
     "Framework :: Pytest",
     ]
 dependencies = [
-    "firebird-base>=1.7.2",
+    "firebird-base>=1.8.0",
     "firebird-driver~=1.10",
     "pytest>=7.4",
     "psutil~=5.9",
     ]
 
 [project.urls]
 Home = "https://github.com/FirebirdSQL/firebird-qa"
@@ -85,15 +85,15 @@
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.doc]
 detached = false
 platforms = ["linux"]
 dependencies = [
-  "Sphinx>=7.2.6",
+  "Sphinx==7.2.6",
   "sphinx-bootstrap-theme>=0.8.1",
   "sphinx-autodoc-typehints>=1.24.0",
   "doc2dash>=3.0.0"
 ]
 [tool.hatch.envs.doc.scripts]
 build = "cd docs ; make html"
 docset = [
```

### Comparing `firebird_qa-0.19.3/PKG-INFO` & `firebird_qa-0.20.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firebird-qa
-Version: 0.19.3
+Version: 0.20.0
 Summary: pytest plugin for Firebird QA
 Project-URL: Home, https://github.com/FirebirdSQL/firebird-qa
 Project-URL: Documentation, https://firebird-qa.rtfd.io
 Project-URL: Issues, https://github.com/FirebirdSQL/firebird-qa/issues
 Project-URL: Funding, https://github.com/sponsors/pcisar
 Project-URL: Source, https://github.com/FirebirdSQL/firebird-qa
 Author-email: Pavel Cisar <pcisar@users.sourceforge.net>
@@ -43,15 +43,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: <4,>=3.8
-Requires-Dist: firebird-base>=1.7.2
+Requires-Dist: firebird-base>=1.8.0
 Requires-Dist: firebird-driver~=1.10
 Requires-Dist: psutil~=5.9
 Requires-Dist: pytest>=7.4
 Description-Content-Type: text/markdown
 
 # pytest plugin for Firebird QA
```


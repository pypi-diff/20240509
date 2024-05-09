# Comparing `tmp/prometa-2024.3.tar.gz` & `tmp/prometa-2024.4.tar.gz`

## Comparing `prometa-2024.3.tar` & `prometa-2024.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 prometa-2024.3/CITATION.cff
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.3/TODO.md
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 prometa-2024.3/codemeta.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.3/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.3/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.3/doc/requirements.txt
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.3/doc/source/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.3/doc/source/readme.md
--rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.3/scripts/publish_documentation.sh
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/__init__.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/citation.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/codemeta.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/common.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/config.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/file.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/insert.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/main.py
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/project.py
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/readme.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/version.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/gitlab/__init__.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/gitlab/ci.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/gitlab/repo.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/id/__init__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/id/hal.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/id/orcid.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/id/swh.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/python/__init__.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/python/common.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/python/venv.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 prometa-2024.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.3/LICENSE.txt
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 prometa-2024.3/README.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 prometa-2024.3/pyproject.toml
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 prometa-2024.3/PKG-INFO
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 prometa-2024.4/CITATION.cff
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.4/TODO.md
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 prometa-2024.4/codemeta.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.4/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.4/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.4/doc/requirements.txt
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.4/doc/source/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.4/doc/source/readme.md
+-rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.4/scripts/publish_documentation.sh
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/__init__.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/citation.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/codemeta.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/common.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/config.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/file.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/insert.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/main.py
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/project.py
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/readme.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/version.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/gitlab/__init__.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/gitlab/ci.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/gitlab/repo.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/id/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/id/hal.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/id/orcid.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/id/swh.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/python/__init__.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/python/common.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/python/venv.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 prometa-2024.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.4/LICENSE.txt
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 prometa-2024.4/README.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 prometa-2024.4/pyproject.toml
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 prometa-2024.4/PKG-INFO
```

### Comparing `prometa-2024.3/.gitlab-ci.yml` & `prometa-2024.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/codemeta.json` & `prometa-2024.4/codemeta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'2024.4'"}*

```diff
@@ -97,9 +97,9 @@
         "@type": "CommandLineApplication",
         "description": "Update project metadata.",
         "executableName": "prometa",
         "name": "prometa",
         "runtimePlatform": "Python 3"
     },
     "url": "https://gitlab.inria.fr/jrye/prometa",
-    "version": "2024.3"
+    "version": "2024.4"
 }
```

### Comparing `prometa-2024.3/doc/Makefile` & `prometa-2024.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/doc/make.bat` & `prometa-2024.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/doc/source/conf.py` & `prometa-2024.4/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/scripts/publish_documentation.sh` & `prometa-2024.4/scripts/publish_documentation.sh`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/citation.py` & `prometa-2024.4/src/prometa/citation.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/codemeta.py` & `prometa-2024.4/src/prometa/codemeta.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/config.py` & `prometa-2024.4/src/prometa/config.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/file.py` & `prometa-2024.4/src/prometa/file.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/insert.py` & `prometa-2024.4/src/prometa/insert.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/main.py` & `prometa-2024.4/src/prometa/main.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/project.py` & `prometa-2024.4/src/prometa/project.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/readme.py` & `prometa-2024.4/src/prometa/readme.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/gitlab/ci.py` & `prometa-2024.4/src/prometa/gitlab/ci.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/gitlab/repo.py` & `prometa-2024.4/src/prometa/gitlab/repo.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/id/hal.py` & `prometa-2024.4/src/prometa/id/hal.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/id/swh.py` & `prometa-2024.4/src/prometa/id/swh.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/src/prometa/python/common.py` & `prometa-2024.4/src/prometa/python/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -73,32 +73,55 @@
         LOGGER.warning(
             'Failed to map SPDX license ID %s to a Python trove classifier.',
             spdx_id
         )
     return closest
 
 
+def _join_names(given_names, family_names):
+    '''
+    Join given and family names to a single string.
+
+    Args:
+        given_names:
+            The given names.
+
+        family_names:
+            The family names.
+
+    Returns:
+        A string with the joined names.
+    '''
+    if given_names and family_names:
+        return f'{given_names} {family_names}'
+    if given_names:
+        return str(given_names)
+    if family_names:
+        return str(family_names)
+    return None
+
+
 def update_pyproject_toml(project):
     '''
     Update the URLs in a pyproject.toml file.
 
     Args:
         project:
             The Project instance.
     '''
     path = project.pyproject_toml_path
     data = tomllib.loads(path.read_text(encoding='utf-8'))
 
     urls = data['project']['urls']
-    urls.clear()
+    #  urls.clear()
     urls.update(project.urls)
 
     data['project']['authors'] = [
         {
-            'name': f'{author["given-names"]} {author["family-names"]}',
+            'name': _join_names(author["given-names"], author["family-names"]),
             'email': author['email']
         }
         for author in project.config.config['authors']
     ]
 
     classifiers = set(
         classifier
```

### Comparing `prometa-2024.3/src/prometa/python/venv.py` & `prometa-2024.4/src/prometa/python/venv.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/LICENSE.txt` & `prometa-2024.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/README.md` & `prometa-2024.4/README.md`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/pyproject.toml` & `prometa-2024.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prometa-2024.3/PKG-INFO` & `prometa-2024.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Prometa
-Version: 2024.3
+Version: 2024.4
 Summary: Manage project metadata.
 Project-URL: Homepage, https://gitlab.inria.fr/jrye/prometa
 Project-URL: Source, https://gitlab.inria.fr/jrye/prometa.git
 Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/prometa
 Project-URL: Issues, https://gitlab.inria.fr/jrye/prometa/-/issues
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
 License: MIT License
```


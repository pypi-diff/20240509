# Comparing `tmp/pytest-servers-0.5.1.tar.gz` & `tmp/pytest_servers-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-servers-0.5.1.tar", last modified: Tue Mar 19 22:41:53 2024, max compression
+gzip compressed data, was "pytest_servers-0.5.2.tar", last modified: Thu May  9 06:22:08 2024, max compression
```

## Comparing `pytest-servers-0.5.1.tar` & `pytest_servers-0.5.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:41:53.664010 pytest-servers-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:41:53.656010 pytest-servers-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:41:53.656010 pytest-servers-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-03-19 22:41:53.664010 pytest-servers-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/renovate.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 22:41:53.664010 pytest-servers-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:41:53.656010 pytest-servers-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:41:53.660010 pytest-servers-0.5.1/src/pytest_servers/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/local.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/src/pytest_servers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:41:53.660010 pytest-servers-0.5.1/src/pytest_servers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-03-19 22:41:53.000000 pytest-servers-0.5.1/src/pytest_servers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-03-19 22:41:53.000000 pytest-servers-0.5.1/src/pytest_servers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 22:41:53.000000 pytest-servers-0.5.1/src/pytest_servers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-19 22:41:53.000000 pytest-servers-0.5.1/src/pytest_servers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-03-19 22:41:53.000000 pytest-servers-0.5.1/src/pytest_servers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-19 22:41:53.000000 pytest-servers-0.5.1/src/pytest_servers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 22:41:53.660010 pytest-servers-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/tests/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-19 22:41:37.000000 pytest-servers-0.5.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:22:08.060172 pytest_servers-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:22:08.052172 pytest_servers-0.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:22:08.052172 pytest_servers-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-09 06:22:08.060172 pytest_servers-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:22:08.060172 pytest_servers-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:22:08.048172 pytest_servers-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:22:08.056172 pytest_servers-0.5.2/src/pytest_servers/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/src/pytest_servers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:22:08.056172 pytest_servers-0.5.2/src/pytest_servers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-09 06:22:08.000000 pytest_servers-0.5.2/src/pytest_servers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-09 06:22:08.000000 pytest_servers-0.5.2/src/pytest_servers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:22:08.000000 pytest_servers-0.5.2/src/pytest_servers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 06:22:08.000000 pytest_servers-0.5.2/src/pytest_servers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 06:22:08.000000 pytest_servers-0.5.2/src/pytest_servers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 06:22:08.000000 pytest_servers-0.5.2/src/pytest_servers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:22:08.056172 pytest_servers-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/tests/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-09 06:21:53.000000 pytest_servers-0.5.2/tests/test_utils.py
```

### Comparing `pytest-servers-0.5.1/.cruft.json` & `pytest_servers-0.5.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/.github/workflows/release.yml` & `pytest_servers-0.5.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/.github/workflows/tests.yml` & `pytest_servers-0.5.2/.github/workflows/tests.yml`

 * *Files 21% similar despite different names*

```diff
@@ -43,30 +43,39 @@
           python -m pip install --upgrade pip nox
           pip --version
           nox --version
 
       - name: Lint code and check dependencies
         run: nox -s lint safety
 
+      # https://github.com/iterative/pytest-servers/pull/122
       # https://github.com/abiosoft/colima/issues/468
+      # https://github.com/abiosoft/colima/blob/main/docs/FAQ.md#cannot-connect-to-the-docker-daemon-at-unixvarrundockersock-is-the-docker-daemon-running
+      # colima v0.5.6 seems to run more stable than the latest - that has occasional network failures (ports are not open)
+      # see: https://github.com/abiosoft/colima/issues/962
       - name: Use colima as default docker host on MacOS
         if: matrix.os == 'macos-latest'
         run: |
-          brew install docker
+          brew install docker lima || true # avoid non-zero exit code if brew link fails
+          sudo curl -L -o /usr/local/bin/colima https://github.com/abiosoft/colima/releases/download/v0.5.6/colima-Darwin-x86_64
+          sudo chmod +x /usr/local/bin/colima
           colima start
-          ls -la $HOME/.colima/default/docker.sock
-          sudo ln -sf $HOME/.colima/default/docker.sock /var/run/docker.sock
-          ls -la /var/run/docker.sock
+          sudo ln -vsf "${HOME}"/.colima/default/docker.sock /var/run/docker.sock
+        env:
+          HOMEBREW_NO_AUTO_UPDATE: true
+          HOMEBREW_NO_INSTALL_CLEANUP: true
+          HOMEBREW_NO_INSTALLED_DEPENDENTS_CHECK: true
+          HOMEBREW_NO_INSTALL_UPGRADE: true
 
       - name: Run tests
         id: tests
         run: nox -s tests-${{ matrix.pyv }}
         continue-on-error: ${{ matrix.os == 'macos-latest' }}
         env:
           COVERAGE_XML: true
 
       - name: Upload coverage report
         if: steps.tests.outcome  == 'success'
-        uses: codecov/codecov-action@v4.0.1
+        uses: codecov/codecov-action@v4.1.0
 
       - name: Build package
         run: nox -s build
```

### Comparing `pytest-servers-0.5.1/.gitignore` & `pytest_servers-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/.pre-commit-config.yaml` & `pytest_servers-0.5.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 default_language_version:
   python: python3
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-json
       - id: check-merge-conflict
@@ -15,24 +15,24 @@
       - id: check-yaml
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ['--fix=lf']
       - id: sort-simple-yaml
       - id: trailing-whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.3.3'
+    rev: 'v0.4.1'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
         additional_dependencies: ["tomli"]
   - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-    rev: v2.12.0
+    rev: v2.13.0
     hooks:
       - id: pretty-format-toml
         args: [--autofix, --no-sort]
       - id: pretty-format-yaml
         args: [--autofix, --indent, '2', '--offset', '2', --preserve-quotes]
```

### Comparing `pytest-servers-0.5.1/CODE_OF_CONDUCT.rst` & `pytest_servers-0.5.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/CONTRIBUTING.rst` & `pytest_servers-0.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/LICENSE` & `pytest_servers-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/PKG-INFO` & `pytest_servers-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-servers
-Version: 0.5.1
+Version: 0.5.2
 Summary: pytest servers
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/pytest-servers/issues
 Project-URL: Source, https://github.com/iterative/pytest-servers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytest-servers-0.5.1/README.rst` & `pytest_servers-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/noxfile.py` & `pytest_servers-0.5.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/pyproject.toml` & `pytest_servers-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/src/pytest_servers/azure.py` & `pytest_servers-0.5.2/src/pytest_servers/azure.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     azurite_lock = root_tmp_dir / "azurite.lock"
 
     with FileLock(azurite_lock):
         try:
             container: Container = docker_client.containers.get(container_name)
         except NotFound:
             container = docker_client.containers.run(
-                "mcr.microsoft.com/azure-storage/azurite:3.29.0",  # renovate
+                "mcr.microsoft.com/azure-storage/azurite:3.30.0",  # renovate
                 command="azurite-blob --loose --blobHost 0.0.0.0",
                 name=container_name,
                 stdout=True,
                 stderr=True,
                 detach=True,
                 remove=True,
                 ports={f"{AZURITE_PORT}/tcp": None},  # assign a random port
```

### Comparing `pytest-servers-0.5.1/src/pytest_servers/exceptions.py` & `pytest_servers-0.5.2/src/pytest_servers/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/src/pytest_servers/factory.py` & `pytest_servers-0.5.2/src/pytest_servers/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,24 +49,19 @@
         self._gcs_endpoint_url = gcs_endpoint_url
         self._s3_client_kwargs = s3_client_kwargs
 
     @classmethod
     def from_request(
         cls: type[TempUPathFactory],
         request: pytest.FixtureRequest,
-        tmp_path_factory: pytest.TempPathFactory | None = None,
+        tmp_path_factory: pytest.TempPathFactory,
         *args,
         **kwargs,
     ) -> TempUPathFactory:
         """Create a factory according to pytest configuration."""
-        if tmp_path_factory is None:
-            tmp_path_factory = pytest.TempPathFactory.from_config(
-                request.config,
-                _ispytest=True,
-            )
         tmp_upath_factory = cls(*args, **kwargs)
         tmp_upath_factory._local_path_factory = tmp_path_factory  # noqa: SLF001
         tmp_upath_factory._request = request  # noqa: SLF001
 
         return tmp_upath_factory
 
     def _mock_remote_setup(self, fs: str) -> None:
```

### Comparing `pytest-servers-0.5.1/src/pytest_servers/fixtures.py` & `pytest_servers-0.5.2/src/pytest_servers/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/src/pytest_servers/gcs.py` & `pytest_servers-0.5.2/src/pytest_servers/gcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             port = get_free_port()
             url = f"http://localhost:{port}"
             command = (
                 "-backend memory -scheme http "
                 f"-public-host {url} -external-url {url} "
             )
             container = docker_client.containers.run(
-                "fsouza/fake-gcs-server:1.47.8",  # renovate
+                "fsouza/fake-gcs-server:1.49.0",  # renovate
                 name=container_name,
                 command=command,
                 stdout=True,
                 stderr=True,
                 detach=True,
                 remove=True,
                 ports={f"{GCS_DEFAULT_PORT}/tcp": port},
```

### Comparing `pytest-servers-0.5.1/src/pytest_servers/s3.py` & `pytest_servers-0.5.2/src/pytest_servers/s3.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/src/pytest_servers/utils.py` & `pytest_servers-0.5.2/src/pytest_servers/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/src/pytest_servers.egg-info/PKG-INFO` & `pytest_servers-0.5.2/src/pytest_servers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-servers
-Version: 0.5.1
+Version: 0.5.2
 Summary: pytest servers
 Author-email: Iterative <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/pytest-servers/issues
 Project-URL: Source, https://github.com/iterative/pytest-servers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pytest-servers-0.5.1/src/pytest_servers.egg-info/SOURCES.txt` & `pytest_servers-0.5.2/src/pytest_servers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/tests/test_factory.py` & `pytest_servers-0.5.2/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `pytest-servers-0.5.1/tests/test_fixtures.py` & `pytest_servers-0.5.2/tests/test_fixtures.py`

 * *Files identical despite different names*


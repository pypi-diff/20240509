# Comparing `tmp/exponent_run-0.0.2.tar.gz` & `tmp/exponent_run-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponent_run-0.0.2.tar", max compression
+gzip compressed data, was "exponent_run-0.0.3.tar", max compression
```

## Comparing `exponent_run-0.0.2.tar` & `exponent_run-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       57 2024-05-03 23:47:20.021413 exponent_run-0.0.2/exponent/__init__.py
--rw-r--r--   0        0        0     3099 2024-05-04 21:27:55.629978 exponent_run-0.0.2/exponent/cli.py
--rw-r--r--   0        0        0      501 2024-05-04 21:27:55.630193 exponent_run-0.0.2/exponent/core/config.py
--rw-r--r--   0        0        0     2435 2024-05-04 21:27:55.630339 exponent_run-0.0.2/exponent/core/remote_execution/client.py
--rw-r--r--   0        0        0      747 2024-05-04 21:27:55.630473 exponent_run-0.0.2/exponent/core/remote_execution/types.py
--rw-r--r--   0        0        0        0 2024-05-03 23:47:19.960349 exponent_run-0.0.2/exponent/tests/__init__.py
--rw-r--r--   0        0        0      718 2024-05-04 21:27:55.630751 exponent_run-0.0.2/exponent/tests/conftest.py
--rw-r--r--   0        0        0      464 2024-05-04 21:27:55.630962 exponent_run-0.0.2/exponent/tests/test_cli.py
--rw-r--r--   0        0        0     1420 2024-05-06 21:37:07.087406 exponent_run-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 exponent_run-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       57 2024-05-03 23:47:20.021413 exponent_run-0.0.3/exponent/__init__.py
+-rw-r--r--   0        0        0     5040 2024-05-09 19:22:41.007830 exponent_run-0.0.3/exponent/cli.py
+-rw-r--r--   0        0        0     1403 2024-05-07 07:10:08.943140 exponent_run-0.0.3/exponent/core/config.py
+-rw-r--r--   0        0        0     7194 2024-05-09 03:32:46.489461 exponent_run-0.0.3/exponent/core/remote_execution/client.py
+-rw-r--r--   0        0        0     1994 2024-05-09 00:30:27.349939 exponent_run-0.0.3/exponent/core/remote_execution/kernel.py
+-rw-r--r--   0        0        0     5414 2024-05-09 00:30:27.350382 exponent_run-0.0.3/exponent/core/remote_execution/types.py
+-rw-r--r--   0        0        0        0 2024-05-03 23:47:19.960349 exponent_run-0.0.3/exponent/tests/__init__.py
+-rw-r--r--   0        0        0     1309 2024-05-09 03:32:46.489873 exponent_run-0.0.3/exponent/tests/conftest.py
+-rw-r--r--   0        0        0     7764 2024-05-09 03:32:46.490229 exponent_run-0.0.3/exponent/tests/test_cli.py
+-rw-r--r--   0        0        0     1518 2024-05-09 19:22:57.019385 exponent_run-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 exponent_run-0.0.3/PKG-INFO
```

### Comparing `exponent_run-0.0.2/exponent/tests/conftest.py` & `exponent_run-0.0.3/exponent/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import asyncio
+import os
+import tempfile
 from collections.abc import Generator
 
 import pytest
 from click.testing import CliRunner
 
 
 @pytest.fixture(scope="session")
@@ -20,7 +22,24 @@
 
 @pytest.fixture(scope="session", autouse=True)
 async def fixture_setup_env() -> None:
     session_mpatch = pytest.MonkeyPatch()
     session_mpatch.setenv("EXPONENT_API_KEY", "123456")
     session_mpatch.setenv("EXPONENT_BASE_URL", "https://exponent.run")
     session_mpatch.setenv("EXPONENT_API_BASE_URL", "https://api.exponent.run")
+
+
+@pytest.fixture(scope="function")
+def temporary_directory() -> Generator[str, None, None]:
+    with tempfile.TemporaryDirectory() as test_directory:
+        yield test_directory
+
+
+@pytest.fixture(scope="function")
+def default_temporary_directory(temporary_directory: str) -> Generator[str, None, None]:
+    with open(os.path.join(temporary_directory, "test1.py"), "w") as f:
+        f.write("print('Hello, world!')")
+
+    with open(os.path.join(temporary_directory, "test2.py"), "w") as f:
+        f.write("print('Hello, world!')")
+
+    yield temporary_directory
```

### Comparing `exponent_run-0.0.2/pyproject.toml` & `exponent_run-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [tool.poetry]
 authors = ["Sashank Thupukari <sashank@exponent.run>"]
 description = "Exponent is an AI Pair Programmer"
 name = "exponent-run"
-version = "0.0.2"
+version = "0.0.3"
 packages = [{ include = "exponent" }]
 
 [tool.poetry.scripts]
 exponent = "exponent.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 
 pydantic = { extras = ["dotenv", "email"], version = "^2.6.4" }
 pydantic-settings = "^2.2.1"
 pytest-env = "^1.1.3"
 click = "^8.1.7"
 httpx = "^0.27.0"
+rapidfuzz = "^3.9.0"
+gitignore-parser = "^0.1.11"
+jupyter-client = "^8.6.1"
+ipykernel = "^6.29.4"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.4.4"
 freezegun = "^1.4.0"
 gevent = "^24.2.1"
 mypy = "^1.9.0"
 pre-commit = "^3.7.0"
```


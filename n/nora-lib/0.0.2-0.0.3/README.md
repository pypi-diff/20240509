# Comparing `tmp/nora_lib-0.0.2.tar.gz` & `tmp/nora_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nora_lib-0.0.2.tar", last modified: Wed Feb 21 01:25:38 2024, max compression
+gzip compressed data, was "nora_lib-0.0.3.tar", last modified: Thu May  9 17:33:47 2024, max compression
```

## Comparing `nora_lib-0.0.2.tar` & `nora_lib-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,32 @@
-drwxr-xr-x   0 miked     (2379) users      (100)        0 2024-02-21 01:25:38.037303 nora_lib-0.0.2/
--rw-r--r--   0 miked     (2379) users      (100)      337 2024-02-21 01:25:38.033303 nora_lib-0.0.2/PKG-INFO
--rw-r--r--   0 miked     (2379) users      (100)       58 2024-02-16 23:08:27.000000 nora_lib-0.0.2/README.md
-drwxr-xr-x   0 miked     (2379) users      (100)        0 2024-02-21 01:25:37.961307 nora_lib-0.0.2/nora_lib/
--rw-r--r--   0 miked     (2379) users      (100)        0 2024-02-16 23:08:27.000000 nora_lib-0.0.2/nora_lib/__init__.py
--rw-r--r--   0 miked     (2379) users      (100)        0 2024-02-16 23:08:27.000000 nora_lib-0.0.2/nora_lib/py.typed
-drwxr-xr-x   0 miked     (2379) users      (100)        0 2024-02-21 01:25:37.993305 nora_lib-0.0.2/nora_lib/tasks/
--rw-r--r--   0 miked     (2379) users      (100)        0 2024-02-16 23:08:27.000000 nora_lib-0.0.2/nora_lib/tasks/__init__.py
--rw-r--r--   0 miked     (2379) users      (100)      925 2024-02-16 23:08:27.000000 nora_lib-0.0.2/nora_lib/tasks/models.py
--rw-r--r--   0 miked     (2379) users      (100)     1793 2024-02-21 01:25:28.000000 nora_lib-0.0.2/nora_lib/tasks/state.py
-drwxr-xr-x   0 miked     (2379) users      (100)        0 2024-02-21 01:25:38.026304 nora_lib-0.0.2/nora_lib.egg-info/
--rw-r--r--   0 miked     (2379) users      (100)      337 2024-02-21 01:25:37.000000 nora_lib-0.0.2/nora_lib.egg-info/PKG-INFO
--rw-r--r--   0 miked     (2379) users      (100)      383 2024-02-21 01:25:37.000000 nora_lib-0.0.2/nora_lib.egg-info/SOURCES.txt
--rw-r--r--   0 miked     (2379) users      (100)        1 2024-02-21 01:25:37.000000 nora_lib-0.0.2/nora_lib.egg-info/dependency_links.txt
--rw-r--r--   0 miked     (2379) users      (100)       40 2024-02-21 01:25:37.000000 nora_lib-0.0.2/nora_lib.egg-info/requires.txt
--rw-r--r--   0 miked     (2379) users      (100)       15 2024-02-21 01:25:37.000000 nora_lib-0.0.2/nora_lib.egg-info/top_level.txt
--rw-r--r--   0 miked     (2379) users      (100)       90 2024-02-16 23:08:27.000000 nora_lib-0.0.2/pyproject.toml
--rw-r--r--   0 miked     (2379) users      (100)       38 2024-02-21 01:25:38.038303 nora_lib-0.0.2/setup.cfg
--rw-r--r--   0 miked     (2379) users      (100)      570 2024-02-21 01:25:28.000000 nora_lib-0.0.2/setup.py
-drwxr-xr-x   0 miked     (2379) users      (100)        0 2024-02-21 01:25:37.996305 nora_lib-0.0.2/tests/
-drwxr-xr-x   0 miked     (2379) users      (100)        0 2024-02-21 01:25:38.008305 nora_lib-0.0.2/tests/tasks/
--rw-r--r--   0 miked     (2379) users      (100)        0 2024-02-16 23:08:27.000000 nora_lib-0.0.2/tests/tasks/__init__.py
--rw-r--r--   0 miked     (2379) users      (100)     2670 2024-02-21 01:25:28.000000 nora_lib-0.0.2/tests/tasks/test_state.py
--rw-r--r--   0 miked     (2379) users      (100)      123 2024-02-16 23:08:27.000000 nora_lib-0.0.2/tests/test_placeholder.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.362088 nora_lib-0.0.3/
+-rw-r--r--   0 reganh     (502) staff       (20)      407 2024-05-09 17:33:47.361834 nora_lib-0.0.3/PKG-INFO
+-rw-r--r--   0 reganh     (502) staff       (20)      887 2024-05-09 17:31:43.000000 nora_lib-0.0.3/README.md
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.356611 nora_lib-0.0.3/nora_lib/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/__init__.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.358215 nora_lib-0.0.3/nora_lib/context/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/context/__init__.py
+-rw-r--r--   0 reganh     (502) staff       (20)     3130 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/context/context_service.py
+-rw-r--r--   0 reganh     (502) staff       (20)      757 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/context/models.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.358715 nora_lib-0.0.3/nora_lib/interactions/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/interactions/__init__.py
+-rw-r--r--   0 reganh     (502) staff       (20)     4163 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/interactions/interactions_service.py
+-rw-r--r--   0 reganh     (502) staff       (20)     3377 2024-05-09 17:26:38.000000 nora_lib-0.0.3/nora_lib/interactions/models.py
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/py.typed
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.359171 nora_lib-0.0.3/nora_lib/tasks/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/tasks/__init__.py
+-rw-r--r--   0 reganh     (502) staff       (20)      925 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/tasks/models.py
+-rw-r--r--   0 reganh     (502) staff       (20)     1793 2024-05-03 17:18:14.000000 nora_lib-0.0.3/nora_lib/tasks/state.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.361256 nora_lib-0.0.3/nora_lib.egg-info/
+-rw-r--r--   0 reganh     (502) staff       (20)      407 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/PKG-INFO
+-rw-r--r--   0 reganh     (502) staff       (20)      587 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 reganh     (502) staff       (20)        1 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 reganh     (502) staff       (20)       64 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/requires.txt
+-rw-r--r--   0 reganh     (502) staff       (20)       15 2024-05-09 17:33:47.000000 nora_lib-0.0.3/nora_lib.egg-info/top_level.txt
+-rw-r--r--   0 reganh     (502) staff       (20)       90 2024-05-03 17:18:14.000000 nora_lib-0.0.3/pyproject.toml
+-rw-r--r--   0 reganh     (502) staff       (20)       38 2024-05-09 17:33:47.362140 nora_lib-0.0.3/setup.cfg
+-rw-r--r--   0 reganh     (502) staff       (20)      600 2024-05-09 17:29:40.000000 nora_lib-0.0.3/setup.py
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.359344 nora_lib-0.0.3/tests/
+drwxr-xr-x   0 reganh     (502) staff       (20)        0 2024-05-09 17:33:47.359876 nora_lib-0.0.3/tests/tasks/
+-rw-r--r--   0 reganh     (502) staff       (20)        0 2024-05-03 17:18:14.000000 nora_lib-0.0.3/tests/tasks/__init__.py
+-rw-r--r--   0 reganh     (502) staff       (20)     2670 2024-05-03 17:18:14.000000 nora_lib-0.0.3/tests/tasks/test_state.py
+-rw-r--r--   0 reganh     (502) staff       (20)      123 2024-05-03 17:18:14.000000 nora_lib-0.0.3/tests/test_placeholder.py
```

### Comparing `nora_lib-0.0.2/nora_lib/tasks/models.py` & `nora_lib-0.0.3/nora_lib/tasks/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.2/nora_lib/tasks/state.py` & `nora_lib-0.0.3/nora_lib/tasks/state.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.2/setup.py` & `nora_lib-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
-runtime_requirements = ["pydantic>=2,<3"]
+runtime_requirements = ["pydantic>=2,<3", "requests"]
 
 # For running tests, linting, etc
-dev_requirements = ["mypy", "pytest", "black"]
+dev_requirements = ["mypy", "pytest", "black", "types-requests"]
 
 setuptools.setup(
     name="nora_lib",
-    version="0.0.2",
+    version="0.0.3",
     description="For making and coordinating agents and tools",
     url="https://github.com/allenai/nora_lib",
     packages=setuptools.find_packages(exclude=(["tests"])),
     install_requires=runtime_requirements,
     package_data={
         "nora_lib": ["py.typed"],
     },
```

### Comparing `nora_lib-0.0.2/tests/tasks/test_state.py` & `nora_lib-0.0.3/tests/tasks/test_state.py`

 * *Files identical despite different names*


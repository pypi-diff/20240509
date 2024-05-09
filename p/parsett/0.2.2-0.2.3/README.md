# Comparing `tmp/parsett-0.2.2.tar.gz` & `tmp/parsett-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsett-0.2.2.tar", max compression
+gzip compressed data, was "parsett-0.2.3.tar", max compression
```

## Comparing `parsett-0.2.2.tar` & `parsett-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2024-05-06 19:33:45.939820 parsett-0.2.2/LICENSE
--rw-r--r--   0        0        0      108 2024-05-06 19:33:45.948819 parsett-0.2.2/PTT/__init__.py
--rw-r--r--   0        0        0    44237 2024-05-06 19:33:48.912965 parsett-0.2.2/PTT/handlers.py
--rw-r--r--   0        0        0     8689 2024-05-06 19:33:48.917963 parsett-0.2.2/PTT/parse.py
--rw-r--r--   0        0        0     3880 2024-05-06 19:33:48.926971 parsett-0.2.2/PTT/transformers.py
--rw-r--r--   0        0        0     2499 2024-05-06 19:38:32.994091 parsett-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 parsett-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-06 19:33:45.939820 parsett-0.2.3/LICENSE
+-rw-r--r--   0        0        0      108 2024-05-06 19:33:45.948819 parsett-0.2.3/PTT/__init__.py
+-rw-r--r--   0        0        0    44237 2024-05-06 19:33:48.912965 parsett-0.2.3/PTT/handlers.py
+-rw-r--r--   0        0        0     8689 2024-05-09 02:49:32.440767 parsett-0.2.3/PTT/parse.py
+-rw-r--r--   0        0        0     3880 2024-05-06 19:33:48.926971 parsett-0.2.3/PTT/transformers.py
+-rw-r--r--   0        0        0     2499 2024-05-09 02:52:50.069785 parsett-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 parsett-0.2.3/PKG-INFO
```

### Comparing `parsett-0.2.2/LICENSE` & `parsett-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `parsett-0.2.2/PTT/handlers.py` & `parsett-0.2.3/PTT/handlers.py`

 * *Files identical despite different names*

### Comparing `parsett-0.2.2/PTT/parse.py` & `parsett-0.2.3/PTT/parse.py`

 * *Files identical despite different names*

### Comparing `parsett-0.2.2/PTT/transformers.py` & `parsett-0.2.3/PTT/transformers.py`

 * *Files identical despite different names*

### Comparing `parsett-0.2.2/pyproject.toml` & `parsett-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parsett"
-version = "0.2.2"
+version = "0.2.3"
 description = "PTT"
 authors = ["Dreu LaVelle <dreu.lavelle@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 regex = "^2023.12.25"
```


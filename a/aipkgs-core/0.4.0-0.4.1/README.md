# Comparing `tmp/aipkgs_core-0.4.0.tar.gz` & `tmp/aipkgs_core-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aipkgs_core-0.4.0.tar", max compression
+gzip compressed data, was "aipkgs_core-0.4.1.tar", max compression
```

## Comparing `aipkgs_core-0.4.0.tar` & `aipkgs_core-0.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.926815 aipkgs_core-0.4.0/LICENSE.md
--rw-r--r--   0        0        0        0 2022-03-08 13:06:48.926754 aipkgs_core-0.4.0/README.rst
--rw-r--r--   0        0        0      519 2022-09-03 21:38:40.961067 aipkgs_core-0.4.0/aipkgs_core/__init__.py
--rw-r--r--   0        0        0      620 2022-04-01 17:46:38.417317 aipkgs_core-0.4.0/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc
--rw-r--r--   0        0        0      621 2022-09-03 21:08:25.855962 aipkgs_core-0.4.0/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc
--rw-r--r--   0        0        0     1070 2022-03-08 13:06:48.926158 aipkgs_core-0.4.0/aipkgs_core/encryption/encryption.py
--rw-r--r--   0        0        0      408 2023-10-29 22:52:51.609411 aipkgs_core-0.4.0/aipkgs_core/logger/helpers.py
--rw-r--r--   0        0        0     2124 2022-04-01 17:46:38.433739 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     2161 2022-09-03 21:08:25.861529 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc
--rw-r--r--   0        0        0     1655 2022-04-01 17:46:33.794476 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1654 2022-09-03 21:01:09.128303 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      496 2022-04-01 17:46:33.832091 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/email.cpython-38.pyc
--rw-r--r--   0        0        0      495 2022-09-03 21:01:09.190830 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/email.cpython-39.pyc
--rw-r--r--   0        0        0     1298 2022-04-01 17:46:33.756440 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1311 2022-09-03 21:01:09.121203 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      930 2022-04-01 17:46:38.432909 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/json.cpython-38.pyc
--rw-r--r--   0        0        0      931 2022-09-03 21:08:25.860844 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0      571 2022-04-01 17:46:38.302196 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc
--rw-r--r--   0        0        0      572 2022-09-03 21:01:09.369200 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc
--rw-r--r--   0        0        0     1412 2022-04-01 17:46:38.363966 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc
--rw-r--r--   0        0        0     1414 2022-09-03 21:08:25.846360 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc
--rw-r--r--   0        0        0      166 2022-04-01 17:46:38.413690 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0      167 2022-09-03 21:08:25.855049 aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0        0        0     2196 2022-04-01 17:48:43.916256 aipkgs_core-0.4.0/aipkgs_core/utils/date_helpers.py
--rw-r--r--   0        0        0     1315 2022-03-11 08:48:14.567742 aipkgs_core-0.4.0/aipkgs_core/utils/dir_helpers.py
--rw-r--r--   0        0        0      246 2022-03-08 13:06:48.925758 aipkgs_core-0.4.0/aipkgs_core/utils/email.py
--rw-r--r--   0        0        0      700 2022-03-08 13:06:48.925633 aipkgs_core-0.4.0/aipkgs_core/utils/file_helpers.py
--rw-r--r--   0        0        0      827 2022-03-08 13:06:48.925703 aipkgs_core-0.4.0/aipkgs_core/utils/json.py
--rw-r--r--   0        0        0      304 2022-03-08 13:06:48.926210 aipkgs_core-0.4.0/aipkgs_core/utils/phone_number.py
--rw-r--r--   0        0        0     1542 2022-08-20 15:51:07.521999 aipkgs_core-0.4.0/aipkgs_core/utils/singleton.py
--rw-r--r--   0        0        0     1105 2022-09-03 21:08:23.013667 aipkgs_core-0.4.0/aipkgs_core/utils/string_helpers.py
--rw-r--r--   0        0        0        0 2022-03-08 13:06:48.925998 aipkgs_core-0.4.0/aipkgs_core/utils/utils.py
--rw-r--r--   0        0        0      934 2024-05-08 14:01:46.841879 aipkgs_core-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 aipkgs_core-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-03-08 13:06:48.926815 aipkgs_core-0.4.1/LICENSE.md
+-rw-r--r--   0        0        0        0 2022-03-08 13:06:48.926754 aipkgs_core-0.4.1/README.rst
+-rw-r--r--   0        0        0      519 2022-09-03 21:38:40.961067 aipkgs_core-0.4.1/aipkgs_core/__init__.py
+-rw-r--r--   0        0        0      620 2022-04-01 17:46:38.417317 aipkgs_core-0.4.1/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc
+-rw-r--r--   0        0        0      621 2022-09-03 21:08:25.855962 aipkgs_core-0.4.1/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc
+-rw-r--r--   0        0        0     1070 2022-03-08 13:06:48.926158 aipkgs_core-0.4.1/aipkgs_core/encryption/encryption.py
+-rw-r--r--   0        0        0      408 2023-10-29 22:52:51.609411 aipkgs_core-0.4.1/aipkgs_core/logger/helpers.py
+-rw-r--r--   0        0        0     2124 2022-04-01 17:46:38.433739 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     2161 2022-09-03 21:08:25.861529 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0     1655 2022-04-01 17:46:33.794476 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1654 2022-09-03 21:01:09.128303 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2022-04-01 17:46:33.832091 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/email.cpython-38.pyc
+-rw-r--r--   0        0        0      495 2022-09-03 21:01:09.190830 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/email.cpython-39.pyc
+-rw-r--r--   0        0        0     1298 2022-04-01 17:46:33.756440 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1311 2022-09-03 21:01:09.121203 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      930 2022-04-01 17:46:38.432909 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/json.cpython-38.pyc
+-rw-r--r--   0        0        0      931 2022-09-03 21:08:25.860844 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0      571 2022-04-01 17:46:38.302196 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc
+-rw-r--r--   0        0        0      572 2022-09-03 21:01:09.369200 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc
+-rw-r--r--   0        0        0     1412 2022-04-01 17:46:38.363966 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc
+-rw-r--r--   0        0        0     1414 2022-09-03 21:08:25.846360 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc
+-rw-r--r--   0        0        0      166 2022-04-01 17:46:38.413690 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0        0        0      167 2022-09-03 21:08:25.855049 aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0     2196 2022-04-01 17:48:43.916256 aipkgs_core-0.4.1/aipkgs_core/utils/date_helpers.py
+-rw-r--r--   0        0        0     1315 2022-03-11 08:48:14.567742 aipkgs_core-0.4.1/aipkgs_core/utils/dir_helpers.py
+-rw-r--r--   0        0        0      246 2022-03-08 13:06:48.925758 aipkgs_core-0.4.1/aipkgs_core/utils/email.py
+-rw-r--r--   0        0        0      700 2022-03-08 13:06:48.925633 aipkgs_core-0.4.1/aipkgs_core/utils/file_helpers.py
+-rw-r--r--   0        0        0      827 2022-03-08 13:06:48.925703 aipkgs_core-0.4.1/aipkgs_core/utils/json.py
+-rw-r--r--   0        0        0      304 2022-03-08 13:06:48.926210 aipkgs_core-0.4.1/aipkgs_core/utils/phone_number.py
+-rw-r--r--   0        0        0     1542 2022-08-20 15:51:07.521999 aipkgs_core-0.4.1/aipkgs_core/utils/singleton.py
+-rw-r--r--   0        0        0     1105 2022-09-03 21:08:23.013667 aipkgs_core-0.4.1/aipkgs_core/utils/string_helpers.py
+-rw-r--r--   0        0        0      665 2024-05-09 14:43:31.886429 aipkgs_core-0.4.1/aipkgs_core/utils/utils.py
+-rw-r--r--   0        0        0      983 2024-05-09 14:44:41.510274 aipkgs_core-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      773 1970-01-01 00:00:00.000000 aipkgs_core-0.4.1/PKG-INFO
```

### Comparing `aipkgs_core-0.4.0/LICENSE.md` & `aipkgs_core-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/__init__.py` & `aipkgs_core-0.4.1/aipkgs_core/__init__.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc` & `aipkgs_core-0.4.1/aipkgs_core/encryption/__pycache__/encryption.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc` & `aipkgs_core-0.4.1/aipkgs_core/encryption/__pycache__/encryption.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/encryption/encryption.py` & `aipkgs_core-0.4.1/aipkgs_core/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/date_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/date_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/dir_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/dir_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/file_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/file_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/json.cpython-38.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/json.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/json.cpython-39.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/phone_number.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/phone_number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/string_helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc` & `aipkgs_core-0.4.1/aipkgs_core/utils/__pycache__/string_helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/date_helpers.py` & `aipkgs_core-0.4.1/aipkgs_core/utils/date_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/dir_helpers.py` & `aipkgs_core-0.4.1/aipkgs_core/utils/dir_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/file_helpers.py` & `aipkgs_core-0.4.1/aipkgs_core/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/json.py` & `aipkgs_core-0.4.1/aipkgs_core/utils/json.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/singleton.py` & `aipkgs_core-0.4.1/aipkgs_core/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/aipkgs_core/utils/string_helpers.py` & `aipkgs_core-0.4.1/aipkgs_core/utils/string_helpers.py`

 * *Files identical despite different names*

### Comparing `aipkgs_core-0.4.0/pyproject.toml` & `aipkgs_core-0.4.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aipkgs-core"
-version = "0.4.0"
-description = ""
+version = "0.4.1"
+description = "Core package for aipy packages."
 authors = ["Alexy <alexy.ib@outlook.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://gitlab.com/aipy/public/packages.git"
 repository = "https://gitlab.com/aipy/public/packages.git"
 keywords = ["ai"]
 include = [
@@ -32,14 +32,15 @@
 [tool.poetry.dependencies]
 python = "^3.11.3"
 requests = "^2.28.1"
 pendulum = "^3.0.0"
 email-validator = "^2.1.1"
 emoji = "^2.11.1"
 phonenumbers = "^8.13.36"
+bcrypt = "^4.1.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.1"
```

### Comparing `aipkgs_core-0.4.0/PKG-INFO` & `aipkgs_core-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: aipkgs-core
-Version: 0.4.0
-Summary: 
+Version: 0.4.1
+Summary: Core package for aipy packages.
 Home-page: https://gitlab.com/aipy/public/packages.git
 License: MIT
 Keywords: ai
 Author: Alexy
 Author-email: alexy.ib@outlook.com
 Requires-Python: >=3.11.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bcrypt (>=4.1.3,<5.0.0)
 Requires-Dist: email-validator (>=2.1.1,<3.0.0)
 Requires-Dist: emoji (>=2.11.1,<3.0.0)
 Requires-Dist: pendulum (>=3.0.0,<4.0.0)
 Requires-Dist: phonenumbers (>=8.13.36,<9.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://gitlab.com/aipy/public/packages.git
 Description-Content-Type: text/x-rst
```


# Comparing `tmp/pyscopedstorage-0.0.2.tar.gz` & `tmp/pyscopedstorage-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscopedstorage-0.0.2.tar", max compression
+gzip compressed data, was "pyscopedstorage-0.0.3.tar", max compression
```

## Comparing `pyscopedstorage-0.0.2.tar` & `pyscopedstorage-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.2/LICENSE
--rw-r--r--   0        0        0     3200 2024-05-07 15:43:20.841694 pyscopedstorage-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       59 2024-05-08 00:56:10.748860 pyscopedstorage-0.0.2/src/PyScopedStorage/__init__.py
--rw-r--r--   0        0        0      496 2024-05-07 16:10:47.864603 pyscopedstorage-0.0.2/src/PyScopedStorage/android_objects.py
--rw-r--r--   0        0        0     2870 2024-04-29 16:44:18.965900 pyscopedstorage-0.0.2/src/PyScopedStorage/filechooser.py
--rw-r--r--   0        0        0      266 2024-04-13 10:37:21.713902 pyscopedstorage-0.0.2/src/PyScopedStorage/io.py
--rw-r--r--   0        0        0     2617 2024-05-07 23:46:46.622090 pyscopedstorage-0.0.2/src/PyScopedStorage/tools.py
--rw-r--r--   0        0        0     3436 2024-05-08 01:13:30.867802 pyscopedstorage-0.0.2/src/PyScopedStorage/utils.py
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-29 16:56:36.604859 pyscopedstorage-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3200 2024-05-08 01:25:11.149763 pyscopedstorage-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-05-08 00:56:10.748860 pyscopedstorage-0.0.3/src/PyScopedStorage/__init__.py
+-rw-r--r--   0        0        0      496 2024-05-07 16:10:47.864603 pyscopedstorage-0.0.3/src/PyScopedStorage/android_objects.py
+-rw-r--r--   0        0        0     2870 2024-04-29 16:44:18.965900 pyscopedstorage-0.0.3/src/PyScopedStorage/filechooser.py
+-rw-r--r--   0        0        0      266 2024-04-13 10:37:21.713902 pyscopedstorage-0.0.3/src/PyScopedStorage/io.py
+-rw-r--r--   0        0        0     2617 2024-05-07 23:46:46.622090 pyscopedstorage-0.0.3/src/PyScopedStorage/tools.py
+-rw-r--r--   0        0        0     3567 2024-05-10 01:31:20.716536 pyscopedstorage-0.0.3/src/PyScopedStorage/utils.py
+-rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 pyscopedstorage-0.0.3/PKG-INFO
```

### Comparing `pyscopedstorage-0.0.2/LICENSE` & `pyscopedstorage-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.2/pyproject.toml` & `pyscopedstorage-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyScopedStorage"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python library to simplify storage interaction in Android apps."
 # readme = "README.md"  # TODO..
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
 license = "Apache 2.0"
 
 classifiers = [
 	"Development Status :: 5 - Production/Stable",
```

### Comparing `pyscopedstorage-0.0.2/src/PyScopedStorage/filechooser.py` & `pyscopedstorage-0.0.3/src/PyScopedStorage/filechooser.py`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.2/src/PyScopedStorage/tools.py` & `pyscopedstorage-0.0.3/src/PyScopedStorage/tools.py`

 * *Files identical despite different names*

### Comparing `pyscopedstorage-0.0.2/src/PyScopedStorage/utils.py` & `pyscopedstorage-0.0.3/src/PyScopedStorage/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,27 +45,34 @@
 	'r': 'r',
 	'rb': 'r',
 
 	# TODO: Optionally skip truncate..
 	# java "w" -> "wt"
 	'w': 'wt',
 	'wb': 'wt',
+	'w+': 'wt',
+	'wb+': 'wt',
 
 	'x': 'wt',  # existent check is inside sfopen_{sync/async}
+	'xb': 'wt',
 
 	'a': 'wa',
 	'ab': 'wa',
 
+	'a+': 'rwa',
+	'ab+': 'rwa',
+
 	# no truncate, because
 	# usually in stdlib `io.open` if file will just read, it's doesn't be overwritten
 	'r+': 'rw',
 	'rb+': 'rw',
 }
 
 
+# TODO: Handle access errors..
 def get_fd_from_android_uri(
 	content_uri: 'android.net.Uri',
 	mode: str = 'r',
 ) -> int:
 	"""Open and detach android java file descriptor for	directly access in python.
 
 	Note for open modes:
@@ -115,14 +122,15 @@
 # 	ret = DocumentsContract.buildDocumentUriUsingTree(access_uri, doc_file)
 
 # 	del py_uri, doc_file
 
 # 	return ret
 
 
+# TODO: Handle parse errors..
 def generate_file_uri_from_access_uri(access_uri: 'android.net.Uri', name: str) -> 'android.net.Uri':
 	dir_name: str = DocumentsContract.getTreeDocumentId(access_uri)
 	doc_file: str = f'{dir_name}/{name}'
 	del dir_name
 
 	ret = DocumentsContract.buildDocumentUriUsingTree(access_uri, doc_file)
```

### Comparing `pyscopedstorage-0.0.2/PKG-INFO` & `pyscopedstorage-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyScopedStorage
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library to simplify storage interaction in Android apps.
 License: Apache 2.0
 Author: BlackCatDevel0per
 Author-email: bcdev@mail.ru
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```


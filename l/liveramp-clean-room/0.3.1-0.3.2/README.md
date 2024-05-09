# Comparing `tmp/liveramp_clean_room-0.3.1.tar.gz` & `tmp/liveramp_clean_room-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_clean_room-0.3.1.tar", max compression
+gzip compressed data, was "liveramp_clean_room-0.3.2.tar", max compression
```

## Comparing `liveramp_clean_room-0.3.1.tar` & `liveramp_clean_room-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2557 2024-03-26 03:41:06.365945 liveramp_clean_room-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-03-26 03:41:06.365945 liveramp_clean_room-0.3.1/liveramp_clean_room/__init__.py
--rw-r--r--   0        0        0      558 2024-03-26 03:41:06.365945 liveramp_clean_room-0.3.1/liveramp_clean_room/config/api_config.toml
--rw-r--r--   0        0        0       27 2024-03-26 03:41:06.365945 liveramp_clean_room-0.3.1/liveramp_clean_room/datahub/__init__.py
--rw-r--r--   0        0        0    18837 2024-03-26 03:41:06.365945 liveramp_clean_room-0.3.1/liveramp_clean_room/datahub/client.py
--rw-r--r--   0        0        0     1052 2024-03-26 03:41:06.365945 liveramp_clean_room-0.3.1/liveramp_clean_room/datahub/credentials.py
--rw-r--r--   0        0        0      984 2024-03-26 03:41:06.365945 liveramp_clean_room-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3501 1970-01-01 00:00:00.000000 liveramp_clean_room-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2557 2024-05-09 06:31:30.798762 liveramp_clean_room-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 06:31:30.798762 liveramp_clean_room-0.3.2/liveramp_clean_room/__init__.py
+-rw-r--r--   0        0        0      558 2024-05-09 06:31:30.798762 liveramp_clean_room-0.3.2/liveramp_clean_room/config/api_config.toml
+-rw-r--r--   0        0        0       27 2024-05-09 06:31:30.798762 liveramp_clean_room-0.3.2/liveramp_clean_room/datahub/__init__.py
+-rw-r--r--   0        0        0    18959 2024-05-09 06:31:30.798762 liveramp_clean_room-0.3.2/liveramp_clean_room/datahub/client.py
+-rw-r--r--   0        0        0     1052 2024-05-09 06:31:30.798762 liveramp_clean_room-0.3.2/liveramp_clean_room/datahub/credentials.py
+-rw-r--r--   0        0        0      984 2024-05-09 06:31:30.798762 liveramp_clean_room-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3501 1970-01-01 00:00:00.000000 liveramp_clean_room-0.3.2/PKG-INFO
```

### Comparing `liveramp_clean_room-0.3.1/README.md` & `liveramp_clean_room-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_clean_room-0.3.1/liveramp_clean_room/config/api_config.toml` & `liveramp_clean_room-0.3.2/liveramp_clean_room/config/api_config.toml`

 * *Files identical despite different names*

### Comparing `liveramp_clean_room-0.3.1/liveramp_clean_room/datahub/client.py` & `liveramp_clean_room-0.3.2/liveramp_clean_room/datahub/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,19 @@
     def _required_headers(self):
         return {
             "Authorization": f"Bearer {self.get_token()}",
             "LR-Org-ID": self.org_id,
             "Content-Type": "application/json",
         }
 
+    @backoff.on_exception(
+        backoff.expo,
+        requests.exceptions.RequestException,
+        max_tries=5,
+    )
     def process_request(self, method, endpoint, data=None, params=None):
         """
         Direct call to clean room API
         """
         # Set header
         headers = self._required_headers()
         full_endpoint = f"{self.base_url}{self.config['api']['version']}{endpoint}"
```

### Comparing `liveramp_clean_room-0.3.1/liveramp_clean_room/datahub/credentials.py` & `liveramp_clean_room-0.3.2/liveramp_clean_room/datahub/credentials.py`

 * *Files identical despite different names*

### Comparing `liveramp_clean_room-0.3.1/pyproject.toml` & `liveramp_clean_room-0.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liveramp_clean_room"
-version = "0.3.1"
+version = "0.3.2"
 description = "This is a python client that provides high level functions for interacting with liveramp's clean room."
 authors = ["Datahub Eng <datahub_ops@liveramp.com>"]
 readme = "README.md"
 packages = [{include = "liveramp_clean_room"}]
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
```

### Comparing `liveramp_clean_room-0.3.1/PKG-INFO` & `liveramp_clean_room-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-clean-room
-Version: 0.3.1
+Version: 0.3.2
 Summary: This is a python client that provides high level functions for interacting with liveramp's clean room.
 Author: Datahub Eng
 Author-email: datahub_ops@liveramp.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/metafold-0.1.1.tar.gz` & `tmp/metafold-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metafold-0.1.1.tar", last modified: Mon Feb 12 15:15:17 2024, max compression
+gzip compressed data, was "metafold-0.1.2.tar", last modified: Thu May  9 13:26:46 2024, max compression
```

## Comparing `metafold-0.1.1.tar` & `metafold-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 15:15:17.521082 metafold-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-12 15:15:07.000000 metafold-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-02-12 15:15:17.521082 metafold-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-12 15:15:07.000000 metafold-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 15:15:17.517082 metafold-0.1.1/metafold/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-12 15:15:07.000000 metafold-0.1.1/metafold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-02-12 15:15:07.000000 metafold-0.1.1/metafold/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-02-12 15:15:07.000000 metafold-0.1.1/metafold/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-02-12 15:15:07.000000 metafold-0.1.1/metafold/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-12 15:15:07.000000 metafold-0.1.1/metafold/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-02-12 15:15:07.000000 metafold-0.1.1/metafold/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 15:15:17.521082 metafold-0.1.1/metafold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-02-12 15:15:17.000000 metafold-0.1.1/metafold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-12 15:15:17.000000 metafold-0.1.1/metafold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 15:15:17.000000 metafold-0.1.1/metafold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-12 15:15:17.000000 metafold-0.1.1/metafold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-12 15:15:17.000000 metafold-0.1.1/metafold.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-12 15:15:07.000000 metafold-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 15:15:17.521082 metafold-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 15:15:17.521082 metafold-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-02-12 15:15:07.000000 metafold-0.1.1/tests/test_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-02-12 15:15:07.000000 metafold-0.1.1/tests/test_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:46.770036 metafold-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-09 13:26:43.000000 metafold-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-09 13:26:46.770036 metafold-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-09 13:26:43.000000 metafold-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:46.766036 metafold-0.1.2/metafold/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-09 13:26:43.000000 metafold-0.1.2/metafold/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:46.766036 metafold-0.1.2/metafold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:26:46.000000 metafold-0.1.2/metafold.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-09 13:26:43.000000 metafold-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:26:46.770036 metafold-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:46.766036 metafold-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-09 13:26:43.000000 metafold-0.1.2/tests/test_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-09 13:26:43.000000 metafold-0.1.2/tests/test_jobs.py
```

### Comparing `metafold-0.1.1/LICENSE` & `metafold-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `metafold-0.1.1/PKG-INFO` & `metafold-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metafold
-Version: 0.1.1
+Version: 0.1.2
 Summary: Metafold SDK for Python
 Author-email: Metafold 3D <info@metafold3d.com>
 License: Copyright 2024 Metafold 3D
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -17,19 +17,20 @@
 Project-URL: Issues, https://github.com/Metafold3d/metafold-python/issues
 Keywords: metafold,api,sdk,implicit geometry
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs>=23.2
 Requires-Dist: requests>=2.31
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.2; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0; extra == "docs"
```

### Comparing `metafold-0.1.1/README.md` & `metafold-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `metafold-0.1.1/metafold/__init__.py` & `metafold-0.1.2/metafold/__init__.py`

 * *Files identical despite different names*

### Comparing `metafold-0.1.1/metafold/api.py` & `metafold-0.1.2/metafold/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timezone
-from typing import Any
+from typing import Any, Union
 
 
-def asdatetime(s: str | datetime) -> datetime:
+def asdatetime(s: Union[str, datetime]) -> datetime:
     """Parse Metafold API datetime.
 
     Note datetime strings returned by the Metafold API are RFC 1123 formatted,
     times are always in GMT.
 
     Returns:
         UTC datetime.
```

### Comparing `metafold-0.1.1/metafold/assets.py` & `metafold-0.1.2/metafold/assets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from attrs import field, frozen
 from datetime import datetime
 from metafold.api import asdatetime, asdict
 from metafold.client import Client
 from os import PathLike
 from requests import Response
-from typing import IO, Optional
+from typing import IO, Optional, Union
 import requests
 
 
 @frozen(kw_only=True)
 class Asset:
     """Asset resource.
 
@@ -61,29 +61,29 @@
         Returns:
             Asset resource.
         """
         url = f"/projects/{self._client.project_id}/assets/{id}"
         r: Response = self._client.get(url)
         return Asset(**r.json())
 
-    def download_file(self, id: str, path: str | PathLike):
+    def download_file(self, id: str, path: Union[str, PathLike]):
         """Download an asset.
 
         Args:
             id: ID of asset to download.
             path: Path to downloaded file.
         """
         url = f"/projects/{self._client.project_id}/assets/{id}"
         r: Response = self._client.get(url, params={"download": "true"})
         r = requests.get(r.json()["link"], stream=True)
         with open(path, "wb") as f:
             for chunk in r.iter_content(chunk_size=65536):  # 64 KiB
                 f.write(chunk)
 
-    def create(self, f: str | bytes | PathLike | IO[bytes]) -> Asset:
+    def create(self, f: Union[str, bytes, PathLike, IO[bytes]]) -> Asset:
         """Upload an asset.
 
         Args:
             f: File-like object (opened in binary mode) or path to file on disk.
 
         Returns:
             Asset resource.
@@ -92,15 +92,15 @@
         try:
             url = f"/projects/{self._client.project_id}/assets"
             r: Response = self._client.post(url, files={"file": fp})
         finally:
             fp.close()
         return Asset(**r.json())
 
-    def update(self, id: str, f: str | bytes | PathLike | IO[bytes]) -> Asset:
+    def update(self, id: str, f: Union[str, bytes, PathLike, IO[bytes]]) -> Asset:
         """Update an asset.
 
         Args:
             id: ID of asset to update.
             f: File-like object (opened in binary mode) or path to file on disk.
 
         Returns:
@@ -120,11 +120,11 @@
         Args:
             id: ID of asset to delete.
         """
         url = f"/projects/{self._client.project_id}/assets/{id}"
         self._client.delete(url)
 
 
-def _open_file(f: str | bytes | PathLike | IO[bytes]) -> IO[bytes]:
-    if isinstance(f, str | bytes | PathLike):
+def _open_file(f: Union[str, bytes, PathLike, IO[bytes]]) -> IO[bytes]:
+    if isinstance(f, (str, bytes, PathLike)):
         return open(f, "rb")
     return f
```

### Comparing `metafold-0.1.1/metafold/client.py` & `metafold-0.1.2/metafold/client.py`

 * *Files identical despite different names*

### Comparing `metafold-0.1.1/metafold/jobs.py` & `metafold-0.1.2/metafold/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from attrs import field, frozen
 from datetime import datetime
 from metafold.api import asdatetime, asdict
 from metafold.assets import Asset
 from metafold.client import Client
 from metafold.exceptions import PollTimeout
 from requests import Response
-from typing import Any, Optional
+from typing import Any, Optional, Union
 import time
 
 
-def _assets(v: list[dict[str, Any] | Asset]) -> list[Asset]:
+def _assets(v: list[Union[dict[str, Any], Asset]]) -> list[Asset]:
     return [a if isinstance(a, Asset) else Asset(**a) for a in v]
 
 
 @frozen(kw_only=True)
 class Job:
     """Job resource.
 
@@ -72,15 +72,15 @@
         url = f"/projects/{self._client.project_id}/jobs/{id}"
         r: Response = self._client.get(url)
         return Job(**r.json())
 
     def run(
         self, type: str, params: dict[str, Any],
         name: Optional[str] = None,
-        timeout: int | float = 120,
+        timeout: Union[int, float] = 120,
     ) -> Job:
         """Dispatch a new job and wait for a result.
 
         See Metafold API docs for the full list of jobs.
 
         Args:
             type: Job type.
@@ -107,15 +107,15 @@
             Updated job resource.
         """
         url = f"/projects/{self._client.project_id}/jobs/{id}"
         payload = asdict(name=name)
         r: Response = self._client.patch(url, data=payload)
         return Job(**r.json())
 
-    def _poll(self, url: str, timeout: int | float) -> Response:
+    def _poll(self, url: str, timeout: Union[int, float]) -> Response:
         t0 = time.monotonic()
         r = self._client.get(url)
         while r.status_code == 202:
             elapsed = time.monotonic() - t0
             if elapsed >= timeout:
                 raise PollTimeout("Job timed out")
             time.sleep(1)
```

### Comparing `metafold-0.1.1/metafold.egg-info/PKG-INFO` & `metafold-0.1.2/metafold.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metafold
-Version: 0.1.1
+Version: 0.1.2
 Summary: Metafold SDK for Python
 Author-email: Metafold 3D <info@metafold3d.com>
 License: Copyright 2024 Metafold 3D
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -17,19 +17,20 @@
 Project-URL: Issues, https://github.com/Metafold3d/metafold-python/issues
 Keywords: metafold,api,sdk,implicit geometry
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs>=23.2
 Requires-Dist: requests>=2.31
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.2; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=2.0; extra == "docs"
```

### Comparing `metafold-0.1.1/pyproject.toml` & `metafold-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metafold"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Metafold 3D", email = "info@metafold3d.com"},
 ]
 dependencies = [
     "attrs>=23.2",
     "requests>=2.31",
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 description = "Metafold SDK for Python"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 keywords = ["metafold", "api", "sdk", "implicit geometry"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [project.urls]
```

### Comparing `metafold-0.1.1/tests/test_assets.py` & `metafold-0.1.2/tests/test_assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,70 +53,66 @@
 }
 
 
 class MockRequestHandler(BaseHTTPRequestHandler):
     def do_GET(self):
         u = urlparse(self.path)
         params = parse_qs(u.query)
-        match u.path:
-            case "/projects/1/assets":
-                self.send_response(HTTPStatus.OK)
-                self.send_header("Content-Type", "application/json")
-                self.end_headers()
-                payload = asset_list
-                if params.get("sort") == ["id:1"]:
-                    payload = sorted(asset_list, key=lambda p: p["id"])
-                elif params.get("q") == ["filename:f763df409e79eb1c.bin"]:
-                    payload = [p for p in asset_list if p["filename"] == "f763df409e79eb1c.bin"]
-                self.wfile.write(json.dumps(payload).encode())
-            case "/projects/1/assets/1":
-                self.send_response(HTTPStatus.OK)
-                self.send_header("Content-Type", "application/json")
-                self.end_headers()
-                payload = deepcopy(asset_list[-1])
-                if params.get("download") == ["true"]:
-                    payload["link"] = "http://localhost:8000/download?filename=f763df409e79eb1c.bin"
-                self.wfile.write(json.dumps(payload).encode())
-            case "/download":
-                self.send_response(HTTPStatus.OK)
-                self.end_headers()
-                with open(test_file, "rb") as f:
-                    self.wfile.write(f.read())
-            case _:
-                self.send_error(HTTPStatus.NOT_FOUND)
+        if u.path == "/projects/1/assets":
+            self.send_response(HTTPStatus.OK)
+            self.send_header("Content-Type", "application/json")
+            self.end_headers()
+            payload = asset_list
+            if params.get("sort") == ["id:1"]:
+                payload = sorted(asset_list, key=lambda p: p["id"])
+            elif params.get("q") == ["filename:f763df409e79eb1c.bin"]:
+                payload = [p for p in asset_list if p["filename"] == "f763df409e79eb1c.bin"]
+            self.wfile.write(json.dumps(payload).encode())
+        elif u.path == "/projects/1/assets/1":
+            self.send_response(HTTPStatus.OK)
+            self.send_header("Content-Type", "application/json")
+            self.end_headers()
+            payload = deepcopy(asset_list[-1])
+            if params.get("download") == ["true"]:
+                payload["link"] = "http://localhost:8000/download?filename=f763df409e79eb1c.bin"
+            self.wfile.write(json.dumps(payload).encode())
+        elif u.path == "/download":
+            self.send_response(HTTPStatus.OK)
+            self.end_headers()
+            with open(test_file, "rb") as f:
+                self.wfile.write(f.read())
+        else:
+            self.send_error(HTTPStatus.NOT_FOUND)
 
     def do_POST(self):
-        match self.path:
-            case "/projects/1/assets":
-                self.send_response(HTTPStatus.ACCEPTED)
-                self.send_header("Content-Type", "application/json")
-                self.end_headers()
-                self._assert_file()
-                self.wfile.write(json.dumps(new_asset).encode())
-            case _:
-                self.send_error(HTTPStatus.NOT_FOUND)
+        if self.path == "/projects/1/assets":
+            self.send_response(HTTPStatus.CREATED)
+            self.send_header("Content-Type", "application/json")
+            self.end_headers()
+            self._assert_file()
+            self.wfile.write(json.dumps(new_asset).encode())
+        else:
+            self.send_error(HTTPStatus.NOT_FOUND)
 
     def do_PATCH(self):
-        match self.path:
-            case "/projects/1/assets/1":
-                self.send_response(HTTPStatus.OK)
-                self.send_header("Content-Type", "application/json")
-                self.end_headers()
-                self._assert_file()
-                self.wfile.write(json.dumps(new_asset).encode())
-            case _:
-                self.send_error(HTTPStatus.NOT_FOUND)
+        if self.path == "/projects/1/assets/1":
+            self.send_response(HTTPStatus.OK)
+            self.send_header("Content-Type", "application/json")
+            self.end_headers()
+            self._assert_file()
+            self.wfile.write(json.dumps(new_asset).encode())
+        else:
+            self.send_error(HTTPStatus.NOT_FOUND)
 
     def do_DELETE(self):
-        match self.path:
-            case "/projects/1/assets/1":
-                self.send_response(HTTPStatus.OK)
-                self.end_headers()
-            case _:
-                self.send_error(HTTPStatus.NOT_FOUND)
+        if self.path == "/projects/1/assets/1":
+            self.send_response(HTTPStatus.OK)
+            self.end_headers()
+        else:
+            self.send_error(HTTPStatus.NOT_FOUND)
 
     def _assert_file(self):
         length = self.headers.get("Content-Length")
         content_type = self.headers.get("Content-Type")
         content = self.rfile.read(int(length))
         decoder = MultipartDecoder(content, content_type)
         file = decoder.parts[0].content
```

### Comparing `metafold-0.1.1/tests/test_jobs.py` & `metafold-0.1.2/tests/test_jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,77 +85,74 @@
 poll_count: int = 0
 
 
 class MockRequestHandler(BaseHTTPRequestHandler):
     def do_GET(self):
         u = urlparse(self.path)
         params = parse_qs(u.query)
-        match u.path:
-            case "/projects/1/jobs":
-                self.send_response(HTTPStatus.OK)
-                self.send_header("Content-Type", "application/json")
-                self.end_headers()
-                payload = job_list
-                if params.get("sort") == ["id:1"]:
-                    payload = sorted(job_list, key=lambda p: p["id"])
-                elif params.get("q") == ["name:foo"]:
-                    payload = [p for p in job_list if p["name"] == "foo"]
-                self.wfile.write(json.dumps(payload).encode())
-            case "/projects/1/jobs/1":
-                self.send_response(HTTPStatus.OK)
-                self.send_header("Content-Type", "application/json")
-                self.end_headers()
-                payload = job_list[-1]
-                self.wfile.write(json.dumps(payload).encode())
-            case "/projects/1/jobs/1/status":
-                global poll_count
-                poll_count += 1
-                if poll_count < 3:
-                    self.send_response(HTTPStatus.ACCEPTED)
-                    payload = deepcopy(new_job)
-                    payload["state"] = "started"
-                else:
-                    self.send_response(HTTPStatus.OK)
-                    payload = deepcopy(new_job)
-                    payload.update({
-                        "state": "success",
-                        "assets": [asset_json],
-                    })
-                self.send_header("Content-Type", "application/json")
-                self.end_headers()
-                self.wfile.write(json.dumps(payload).encode())
-            case _:
-                self.send_error(HTTPStatus.NOT_FOUND)
-
-    def do_POST(self):
-        match self.path:
-            case "/projects/1/jobs":
+        if u.path == "/projects/1/jobs":
+            self.send_response(HTTPStatus.OK)
+            self.send_header("Content-Type", "application/json")
+            self.end_headers()
+            payload = job_list
+            if params.get("sort") == ["id:1"]:
+                payload = sorted(job_list, key=lambda p: p["id"])
+            elif params.get("q") == ["name:foo"]:
+                payload = [p for p in job_list if p["name"] == "foo"]
+            self.wfile.write(json.dumps(payload).encode())
+        elif u.path == "/projects/1/jobs/1":
+            self.send_response(HTTPStatus.OK)
+            self.send_header("Content-Type", "application/json")
+            self.end_headers()
+            payload = job_list[-1]
+            self.wfile.write(json.dumps(payload).encode())
+        elif u.path == "/projects/1/jobs/1/status":
+            global poll_count
+            poll_count += 1
+            if poll_count < 3:
                 self.send_response(HTTPStatus.ACCEPTED)
-                self.send_header("Content-Type", "application/json")
-                self.end_headers()
+                payload = deepcopy(new_job)
+                payload["state"] = "started"
+            else:
+                self.send_response(HTTPStatus.CREATED)
                 payload = deepcopy(new_job)
                 payload.update({
-                    "state": "pending",
-                    "link": "http://localhost:8000/projects/1/jobs/1/status",
+                    "state": "success",
+                    "assets": [asset_json],
                 })
-                self.wfile.write(json.dumps(payload).encode())
-            case _:
-                self.send_error(HTTPStatus.NOT_FOUND)
+            self.send_header("Content-Type", "application/json")
+            self.end_headers()
+            self.wfile.write(json.dumps(payload).encode())
+        else:
+            self.send_error(HTTPStatus.NOT_FOUND)
+
+    def do_POST(self):
+        if self.path == "/projects/1/jobs":
+            self.send_response(HTTPStatus.ACCEPTED)
+            self.send_header("Content-Type", "application/json")
+            self.end_headers()
+            payload = deepcopy(new_job)
+            payload.update({
+                "state": "pending",
+                "link": "http://localhost:8000/projects/1/jobs/1/status",
+            })
+            self.wfile.write(json.dumps(payload).encode())
+        else:
+            self.send_error(HTTPStatus.NOT_FOUND)
 
     def do_PATCH(self):
-        match self.path:
-            case "/projects/1/jobs/1":
-                self.send_response(HTTPStatus.OK)
-                self.send_header("Content-Type", "application/json")
-                self.end_headers()
-                payload = deepcopy(job_list[-1])
-                payload["name"] = "baz"
-                self.wfile.write(json.dumps(payload).encode())
-            case _:
-                self.send_error(HTTPStatus.NOT_FOUND)
+        if self.path == "/projects/1/jobs/1":
+            self.send_response(HTTPStatus.OK)
+            self.send_header("Content-Type", "application/json")
+            self.end_headers()
+            payload = deepcopy(job_list[-1])
+            payload["name"] = "baz"
+            self.wfile.write(json.dumps(payload).encode())
+        else:
+            self.send_error(HTTPStatus.NOT_FOUND)
 
 
 @pytest.fixture(scope="module")
 def request_handler():
     return MockRequestHandler
```


# Comparing `tmp/ai_models-0.5.5.tar.gz` & `tmp/ai_models-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_models-0.5.5.tar", last modified: Tue May  7 09:20:16 2024, max compression
+gzip compressed data, was "ai_models-0.5.6.tar", last modified: Thu May  9 13:04:04 2024, max compression
```

## Comparing `ai_models-0.5.5.tar` & `ai_models-0.5.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.043257 ai_models-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.035256 ai_models-0.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-07 09:20:05.000000 ai_models-0.5.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-07 09:20:05.000000 ai_models-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-07 09:20:05.000000 ai_models-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 09:20:05.000000 ai_models-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-07 09:20:16.043257 ai_models-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-07 09:20:05.000000 ai_models-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-07 09:20:05.000000 ai_models-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:20:16.043257 ai_models-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.035256 ai_models-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 09:20:15.000000 ai_models-0.5.5/src/ai_models/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models/inputs/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/outputs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models/remote/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/remote/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/remote/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/remote/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-07 09:20:05.000000 ai_models-0.5.5/src/ai_models/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/src/ai_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 09:20:16.000000 ai_models-0.5.5/src/ai_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:20:16.039256 ai_models-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 09:20:05.000000 ai_models-0.5.5/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 09:20:05.000000 ai_models-0.5.5/tests/test_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.568602 ai_models-0.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.560602 ai_models-0.5.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.564602 ai_models-0.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-09 13:03:54.000000 ai_models-0.5.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-09 13:03:54.000000 ai_models-0.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-09 13:03:54.000000 ai_models-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 13:03:54.000000 ai_models-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-09 13:04:04.564602 ai_models-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-05-09 13:03:54.000000 ai_models-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-09 13:03:54.000000 ai_models-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:04:04.568602 ai_models-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.560602 ai_models-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.564602 ai_models-0.5.6/src/ai_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 13:04:04.000000 ai_models-0.5.6/src/ai_models/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.564602 ai_models-0.5.6/src/ai_models/inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.564602 ai_models-0.5.6/src/ai_models/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/outputs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.564602 ai_models-0.5.6/src/ai_models/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/remote/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/remote/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/remote/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-09 13:03:54.000000 ai_models-0.5.6/src/ai_models/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.564602 ai_models-0.5.6/src/ai_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-09 13:04:04.000000 ai_models-0.5.6/src/ai_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 13:04:04.000000 ai_models-0.5.6/src/ai_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:04:04.000000 ai_models-0.5.6/src/ai_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-09 13:04:04.000000 ai_models-0.5.6/src/ai_models.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 13:04:04.000000 ai_models-0.5.6/src/ai_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 13:04:04.000000 ai_models-0.5.6/src/ai_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:04:04.564602 ai_models-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 13:03:54.000000 ai_models-0.5.6/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 13:03:54.000000 ai_models-0.5.6/tests/test_code.py
```

### Comparing `ai_models-0.5.5/.github/workflows/python-publish.yml` & `ai_models-0.5.6/.github/workflows/python-publish.yml`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
     - uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install
       run: |
+        python -m pip install --upgrade pip
         pip install pytest
         pip install -e .
         pip install -r tests/requirements.txt
         pip freeze
 
     - name: Tests
       run: pytest
```

### Comparing `ai_models-0.5.5/.gitignore` & `ai_models-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/.pre-commit-config.yaml` & `ai_models-0.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/LICENSE` & `ai_models-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/PKG-INFO` & `ai_models-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.5.5
+Version: 0.5.6
 Summary: A package to run AI weather models.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ai_models-0.5.5/README.md` & `ai_models-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/pyproject.toml` & `ai_models-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/src/ai_models/__main__.py` & `ai_models-0.5.6/src/ai_models/__main__.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/src/ai_models/checkpoint.py` & `ai_models-0.5.6/src/ai_models/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/src/ai_models/inputs/__init__.py` & `ai_models-0.5.6/src/ai_models/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/src/ai_models/model.py` & `ai_models-0.5.6/src/ai_models/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,19 +129,40 @@
                 handle = handle.clone()
 
             self.archiving[path].add(handle.as_mars())
 
     def finalise(self):
         if self.archive_requests:
             with open(self.archive_requests, "w") as f:
+                json_requests = []
+
                 for path, archive in self.archiving.items():
                     request = dict(source=f'"{path}"', expect=archive.expect)
                     request.update(archive.request)
                     request.update(self._requests_extra)
-                    self._print_request("archive", request, file=f)
+
+                    if self.json:
+                        json_requests.append(request)
+                    else:
+                        self._print_request("archive", request, file=f)
+
+                if json_requests:
+
+                    def json_default(obj):
+                        if isinstance(obj, set):
+                            if len(obj) > 1:
+                                return list(obj)
+                            else:
+                                return obj.pop()
+                        return obj
+
+                    print(
+                        json.dumps(json_requests, separators=(",", ":"), default=json_default),
+                        file=f,
+                    )
 
     def download_assets(self, **kwargs):
         for file in self.download_files:
             asset = os.path.realpath(os.path.join(self.assets, file))
             if not os.path.exists(asset):
                 os.makedirs(os.path.dirname(asset), exist_ok=True)
                 LOG.info("Downloading %s", asset)
```

### Comparing `ai_models-0.5.5/src/ai_models/outputs/__init__.py` & `ai_models-0.5.6/src/ai_models/outputs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,20 +74,20 @@
 
                 assert str(handle.get(key)) == str(value), (key, handle.get(key), value)
 
         return handle, path
 
 
 class HindcastReLabel:
-    def __init__(self, owner, output, hindcast_reference_year, hind_cast_reference_date, **kwargs):
+    def __init__(self, owner, output, hindcast_reference_year=None, hindcast_reference_date=None, **kwargs):
         self.owner = owner
         self.output = output
         self.hindcast_reference_year = int(hindcast_reference_year) if hindcast_reference_year else None
-        self.hind_cast_reference_date = int(hind_cast_reference_date) if hind_cast_reference_date else None
-        assert self.hindcast_reference_year is not None or self.hind_cast_reference_date is not None
+        self.hindcast_reference_date = int(hindcast_reference_date) if hindcast_reference_date else None
+        assert self.hindcast_reference_year is not None or self.hindcast_reference_date is not None
 
     def write(self, *args, **kwargs):
         if "hdate" in kwargs:
             warnings.warn(f"Ignoring hdate='{kwargs['hdate']}' in HindcastReLabel", stacklevel=3)
             kwargs.pop("hdate")
 
         if "date" in kwargs:
@@ -96,30 +96,30 @@
 
         date = kwargs["template"]["date"]
         hdate = kwargs["template"]["hdate"]
 
         if hdate is not None:
             # Input was a hindcast
             referenceDate = (
-                self.hind_cast_reference_date
-                if self.hind_cast_reference_date is not None
+                self.hindcast_reference_date
+                if self.hindcast_reference_date is not None
                 else self.hindcast_reference_year * 10000 + date % 10000
             )
             assert date == referenceDate, (
                 date,
                 referenceDate,
                 hdate,
                 kwargs["template"],
             )
             kwargs["referenceDate"] = referenceDate
             kwargs["hdate"] = hdate
         else:
             referenceDate = (
-                self.hind_cast_reference_date
-                if self.hind_cast_reference_date is not None
+                self.hindcast_reference_date
+                if self.hindcast_reference_date is not None
                 else self.hindcast_reference_year * 10000 + date % 10000
             )
             kwargs["referenceDate"] = referenceDate
             kwargs["hdate"] = date
 
         kwargs.setdefault("check", True)
```

### Comparing `ai_models-0.5.5/src/ai_models/remote/api.py` & `ai_models-0.5.6/src/ai_models/remote/api.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/src/ai_models/remote/config.py` & `ai_models-0.5.6/src/ai_models/remote/config.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/src/ai_models/remote/model.py` & `ai_models-0.5.6/src/ai_models/remote/model.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/src/ai_models/stepper.py` & `ai_models-0.5.6/src/ai_models/stepper.py`

 * *Files identical despite different names*

### Comparing `ai_models-0.5.5/src/ai_models.egg-info/PKG-INFO` & `ai_models-0.5.6/src/ai_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-models
-Version: 0.5.5
+Version: 0.5.6
 Summary: A package to run AI weather models.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ai_models-0.5.5/src/ai_models.egg-info/SOURCES.txt` & `ai_models-0.5.6/src/ai_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*


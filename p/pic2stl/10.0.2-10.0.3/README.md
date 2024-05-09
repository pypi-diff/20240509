# Comparing `tmp/pic2stl-10.0.2.tar.gz` & `tmp/pic2stl-10.0.3.tar.gz`

## Comparing `pic2stl-10.0.2.tar` & `pic2stl-10.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pic2stl-10.0.2/requirements.txt
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 pic2stl-10.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pic2stl-10.0.2/src/pic2stl/__init__.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 pic2stl-10.0.2/src/pic2stl/pic2stl.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pic2stl-10.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pic2stl-10.0.2/LICENSE
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 pic2stl-10.0.2/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pic2stl-10.0.2/pyproject.toml
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pic2stl-10.0.2/PKG-INFO
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pic2stl-10.0.3/requirements.txt
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 pic2stl-10.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pic2stl-10.0.3/src/pic2stl/__init__.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 pic2stl-10.0.3/src/pic2stl/pic2stl.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pic2stl-10.0.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pic2stl-10.0.3/LICENSE
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 pic2stl-10.0.3/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pic2stl-10.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 pic2stl-10.0.3/PKG-INFO
```

### Comparing `pic2stl-10.0.2/.github/workflows/python-package.yml` & `pic2stl-10.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pic2stl-10.0.2/src/pic2stl/pic2stl.py` & `pic2stl-10.0.3/src/pic2stl/pic2stl.py`

 * *Files identical despite different names*

### Comparing `pic2stl-10.0.2/.gitignore` & `pic2stl-10.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pic2stl-10.0.2/LICENSE` & `pic2stl-10.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pic2stl-10.0.2/README.md` & `pic2stl-10.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pic2stl-10.0.2/pyproject.toml` & `pic2stl-10.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pic2stl"
-version = "10.0.2"
+version = "10.0.3"
 authors = [
   { name="niljub", email="dickergamer@tutanota.com" },
 ]
 description = "img2stl is a Python package that converts images to 3D STL models."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pic2stl-10.0.2/PKG-INFO` & `pic2stl-10.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pic2stl
-Version: 10.0.2
+Version: 10.0.3
 Summary: img2stl is a Python package that converts images to 3D STL models.
 Project-URL: Homepage, https://github.com/niljub/pic2stl/
 Project-URL: Issues, https://github.com/niljub/pic2stl/issues
 Author-email: niljub <dickergamer@tutanota.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


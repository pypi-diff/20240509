# Comparing `tmp/pic2stl-0.0.1.tar.gz` & `tmp/pic2stl-1.0.1.tar.gz`

## Comparing `pic2stl-0.0.1.tar` & `pic2stl-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pic2stl-0.0.1/requirements.txt
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 pic2stl-0.0.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pic2stl-0.0.1/src/pic2stl/__init__.py
--rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 pic2stl-0.0.1/src/pic2stl/pic2stl.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pic2stl-0.0.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pic2stl-0.0.1/LICENSE
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 pic2stl-0.0.1/README.md
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pic2stl-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pic2stl-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pic2stl-1.0.1/requirements.txt
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 pic2stl-1.0.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pic2stl-1.0.1/src/pic2stl/__init__.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 pic2stl-1.0.1/src/pic2stl/pic2stl.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pic2stl-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pic2stl-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 pic2stl-1.0.1/README.md
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pic2stl-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 pic2stl-1.0.1/PKG-INFO
```

### Comparing `pic2stl-0.0.1/.github/workflows/python-package.yml` & `pic2stl-1.0.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pic2stl-0.0.1/src/pic2stl/pic2stl.py` & `pic2stl-1.0.1/src/pic2stl/pic2stl.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,11 +82,8 @@
     for i, f in enumerate(faces):
         for j in range(3):
             output_mesh.vectors[i][j] = vertices[f[j]]
     
     # Write to file
     output_mesh.save(output_path)
 
-# Example usage
-image_to_stl('transparent.webp', 'output.stl', extrusion_height=3, add_base=False, base_thickness=1)
-
```

### Comparing `pic2stl-0.0.1/.gitignore` & `pic2stl-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pic2stl-0.0.1/LICENSE` & `pic2stl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pic2stl-0.0.1/README.md` & `pic2stl-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pic2stl-0.0.1/pyproject.toml` & `pic2stl-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pic2stl"
-version = "0.0.1"
+version = "1.0.1"
 authors = [
   { name="niljub", email="dickergamer@tutanota.com" },
 ]
 description = "img2stl is a Python package that converts images to 3D STL models."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pic2stl-0.0.1/PKG-INFO` & `pic2stl-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pic2stl
-Version: 0.0.1
+Version: 1.0.1
 Summary: img2stl is a Python package that converts images to 3D STL models.
 Project-URL: Homepage, https://github.com/niljub/pic2stl/
 Project-URL: Issues, https://github.com/niljub/pic2stl/issues
 Author-email: niljub <dickergamer@tutanota.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


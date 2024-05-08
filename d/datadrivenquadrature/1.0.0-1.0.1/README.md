# Comparing `tmp/datadrivenquadrature-1.0.0.tar.gz` & `tmp/datadrivenquadrature-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadrivenquadrature-1.0.0.tar", last modified: Wed Apr 24 03:11:08 2024, max compression
+gzip compressed data, was "datadrivenquadrature-1.0.1.tar", last modified: Wed May  8 22:11:45 2024, max compression
```

## Comparing `datadrivenquadrature-1.0.0.tar` & `datadrivenquadrature-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 03:11:08.084270 datadrivenquadrature-1.0.0/
--rw-rw-rw-   0        0        0     1147 2024-03-06 17:12:06.000000 datadrivenquadrature-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     7251 2024-04-24 03:11:08.083214 datadrivenquadrature-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6963 2024-04-24 03:06:05.000000 datadrivenquadrature-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 03:11:08.058621 datadrivenquadrature-1.0.0/datadrivenquadrature/
--rw-rw-rw-   0        0        0       99 2024-04-19 19:28:15.000000 datadrivenquadrature-1.0.0/datadrivenquadrature/__init__.py
--rw-rw-rw-   0        0        0    17168 2024-04-24 03:06:30.000000 datadrivenquadrature-1.0.0/datadrivenquadrature/main.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:11:08.083214 datadrivenquadrature-1.0.0/datadrivenquadrature.egg-info/
--rw-rw-rw-   0        0        0     7251 2024-04-24 03:11:07.000000 datadrivenquadrature-1.0.0/datadrivenquadrature.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-04-24 03:11:08.000000 datadrivenquadrature-1.0.0/datadrivenquadrature.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 03:11:07.000000 datadrivenquadrature-1.0.0/datadrivenquadrature.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-24 03:11:07.000000 datadrivenquadrature-1.0.0/datadrivenquadrature.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-24 03:11:07.000000 datadrivenquadrature-1.0.0/datadrivenquadrature.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 03:11:08.084270 datadrivenquadrature-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      591 2024-04-24 03:11:02.000000 datadrivenquadrature-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:11:45.860428 datadrivenquadrature-1.0.1/
+-rw-rw-rw-   0        0        0     1147 2024-03-06 17:12:06.000000 datadrivenquadrature-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7251 2024-05-08 22:11:45.859359 datadrivenquadrature-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6963 2024-04-24 03:06:05.000000 datadrivenquadrature-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 22:11:45.838180 datadrivenquadrature-1.0.1/datadrivenquadrature/
+-rw-rw-rw-   0        0        0       99 2024-04-19 19:28:15.000000 datadrivenquadrature-1.0.1/datadrivenquadrature/__init__.py
+-rw-rw-rw-   0        0        0    17223 2024-05-08 22:07:25.000000 datadrivenquadrature-1.0.1/datadrivenquadrature/main.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:11:45.858354 datadrivenquadrature-1.0.1/datadrivenquadrature.egg-info/
+-rw-rw-rw-   0        0        0     7251 2024-05-08 22:11:45.000000 datadrivenquadrature-1.0.1/datadrivenquadrature.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-08 22:11:45.000000 datadrivenquadrature-1.0.1/datadrivenquadrature.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 22:11:45.000000 datadrivenquadrature-1.0.1/datadrivenquadrature.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-08 22:11:45.000000 datadrivenquadrature-1.0.1/datadrivenquadrature.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-08 22:11:45.000000 datadrivenquadrature-1.0.1/datadrivenquadrature.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 22:11:45.860428 datadrivenquadrature-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      591 2024-05-08 22:11:13.000000 datadrivenquadrature-1.0.1/setup.py
```

### Comparing `datadrivenquadrature-1.0.0/LICENSE` & `datadrivenquadrature-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datadrivenquadrature-1.0.0/PKG-INFO` & `datadrivenquadrature-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadrivenquadrature
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/LDEO-CREW/data-driven-quadrature
 Author: Neal Ma
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: cvxpy
```

### Comparing `datadrivenquadrature-1.0.0/README.md` & `datadrivenquadrature-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `datadrivenquadrature-1.0.0/datadrivenquadrature/main.py` & `datadrivenquadrature-1.0.1/datadrivenquadrature/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     :param sized_integration_axes_list: list of tuples representing the integration axis name and length of integration axis
     :returns: list representing a point with the order of indices matching the given order of integration axes
     """
     point = []
     # TODO: Add user-defined limit selection
     for axis, size in sized_integration_axes_list:
         point.append(random.randrange(size))
-    return point
+    return point if len(sized_integration_axes_list) != 1 else point[0]
 
 def neighbor(point_set, sized_integration_axes_list):
     """"Returns a neighbor state of a given point set (one point changed)
     
     :param point_set: a list of points, each matching the defined integration axes list
     :param sized_integration_axes_list: list of tuples representing the integration axis name and length of integration axis
     :returns: a new object containing a point set that is a neighbor of the input point set
```

### Comparing `datadrivenquadrature-1.0.0/datadrivenquadrature.egg-info/PKG-INFO` & `datadrivenquadrature-1.0.1/datadrivenquadrature.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadrivenquadrature
-Version: 1.0.0
+Version: 1.0.1
 Home-page: https://github.com/LDEO-CREW/data-driven-quadrature
 Author: Neal Ma
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: cvxpy
```

### Comparing `datadrivenquadrature-1.0.0/setup.py` & `datadrivenquadrature-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     description_text = f.read()
 
 # sample setup.py: https://github.com/pypa/sampleproject/blob/db5806e0a3204034c51b1c00dde7d5eb3fa2532e/setup.py
 setup(
     name='datadrivenquadrature',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'xarray',
         'cvxpy'
     ],
     url="https://github.com/LDEO-CREW/data-driven-quadrature",
```


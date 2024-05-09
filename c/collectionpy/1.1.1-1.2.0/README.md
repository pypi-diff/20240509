# Comparing `tmp/collectionpy-1.1.1.tar.gz` & `tmp/collectionpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collectionpy-1.1.1.tar", last modified: Mon Feb  5 18:08:36 2024, max compression
+gzip compressed data, was "collectionpy-1.2.0.tar", last modified: Thu May  9 12:04:54 2024, max compression
```

## Comparing `collectionpy-1.1.1.tar` & `collectionpy-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-02-05 18:08:36.988407 collectionpy-1.1.1/
--rw-rw-rw-   0        0        0     1421 2024-02-05 18:08:36.987410 collectionpy-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1094 2024-01-25 14:31:55.000000 collectionpy-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-05 18:08:36.975332 collectionpy-1.1.1/collectionpy/
--rw-rw-rw-   0        0        0        0 2024-01-25 09:58:22.000000 collectionpy-1.1.1/collectionpy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-05 18:08:36.980428 collectionpy-1.1.1/collectionpy/chart/
--rw-rw-rw-   0        0        0        0 2024-01-25 09:58:22.000000 collectionpy-1.1.1/collectionpy/chart/__init__.py
--rw-rw-rw-   0        0        0     5692 2024-01-25 15:33:16.000000 collectionpy-1.1.1/collectionpy/chart/apexcharts.py
--rw-rw-rw-   0        0        0     3527 2024-02-05 18:07:31.000000 collectionpy-1.1.1/collectionpy/chart/googlecharts.py
-drwxrwxrwx   0        0        0        0 2024-02-05 18:08:36.983420 collectionpy-1.1.1/collectionpy/date/
--rw-rw-rw-   0        0        0     2083 2024-01-26 13:06:56.000000 collectionpy-1.1.1/collectionpy/date/__init__.py
--rw-rw-rw-   0        0        0     1100 2024-01-25 20:01:33.000000 collectionpy-1.1.1/collectionpy/date/dtget.py
--rw-rw-rw-   0        0        0     1713 2024-01-25 09:58:22.000000 collectionpy-1.1.1/collectionpy/date/dtmath.py
-drwxrwxrwx   0        0        0        0 2024-02-05 18:08:36.984417 collectionpy-1.1.1/collectionpy/math/
--rw-rw-rw-   0        0        0        0 2024-01-25 09:58:22.000000 collectionpy-1.1.1/collectionpy/math/__init__.py
--rw-rw-rw-   0        0        0     1144 2024-01-25 09:58:22.000000 collectionpy-1.1.1/collectionpy/math/statistic.py
-drwxrwxrwx   0        0        0        0 2024-02-05 18:08:36.986412 collectionpy-1.1.1/collectionpy/text/
--rw-rw-rw-   0        0        0        0 2024-01-25 09:58:22.000000 collectionpy-1.1.1/collectionpy/text/__init__.py
--rw-rw-rw-   0        0        0      424 2024-01-25 09:58:22.000000 collectionpy-1.1.1/collectionpy/text/number.py
-drwxrwxrwx   0        0        0        0 2024-02-05 18:08:36.979430 collectionpy-1.1.1/collectionpy.egg-info/
--rw-rw-rw-   0        0        0     1421 2024-02-05 18:08:36.000000 collectionpy-1.1.1/collectionpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2024-02-05 18:08:36.000000 collectionpy-1.1.1/collectionpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-05 18:08:36.000000 collectionpy-1.1.1/collectionpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-02-05 18:08:36.000000 collectionpy-1.1.1/collectionpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-05 18:08:36.988407 collectionpy-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      705 2024-02-05 18:07:20.000000 collectionpy-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:04:54.172477 collectionpy-1.2.0/
+-rw-rw-rw-   0        0        0     1421 2024-05-09 12:04:54.172477 collectionpy-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1094 2024-05-09 11:28:52.000000 collectionpy-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 12:04:54.139951 collectionpy-1.2.0/collectionpy/
+-rw-rw-rw-   0        0        0        0 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:04:54.166491 collectionpy-1.2.0/collectionpy/chart/
+-rw-rw-rw-   0        0        0        0 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/chart/__init__.py
+-rw-rw-rw-   0        0        0     5692 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/chart/apexcharts.py
+-rw-rw-rw-   0        0        0     3527 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/chart/googlecharts.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:04:54.168486 collectionpy-1.2.0/collectionpy/date/
+-rw-rw-rw-   0        0        0     2083 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/date/__init__.py
+-rw-rw-rw-   0        0        0     1100 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/date/dtget.py
+-rw-rw-rw-   0        0        0     1713 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/date/dtmath.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:04:54.169483 collectionpy-1.2.0/collectionpy/math/
+-rw-rw-rw-   0        0        0        0 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/math/__init__.py
+-rw-rw-rw-   0        0        0     1902 2024-05-09 12:03:12.000000 collectionpy-1.2.0/collectionpy/math/statistic.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:04:54.171479 collectionpy-1.2.0/collectionpy/text/
+-rw-rw-rw-   0        0        0        0 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/text/__init__.py
+-rw-rw-rw-   0        0        0      424 2024-05-09 11:28:52.000000 collectionpy-1.2.0/collectionpy/text/number.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:04:54.164182 collectionpy-1.2.0/collectionpy.egg-info/
+-rw-rw-rw-   0        0        0     1421 2024-05-09 12:04:53.000000 collectionpy-1.2.0/collectionpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-05-09 12:04:54.000000 collectionpy-1.2.0/collectionpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:04:53.000000 collectionpy-1.2.0/collectionpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-09 12:04:53.000000 collectionpy-1.2.0/collectionpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-09 12:04:53.000000 collectionpy-1.2.0/collectionpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 12:04:54.172477 collectionpy-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      712 2024-05-09 12:04:33.000000 collectionpy-1.2.0/setup.py
```

### Comparing `collectionpy-1.1.1/PKG-INFO` & `collectionpy-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collectionpy
-Version: 1.1.1
+Version: 1.2.0
 Summary: "collectionpy" is more than just a library; it is a comprehensive tool that provides efficient solutions for various areas, ranging from date manipulation and text formatting to the creation of impressive graphics.
 Description-Content-Type: text/markdown
 
 <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
 
 ## COLLECTIONPY
```

### Comparing `collectionpy-1.1.1/README.md` & `collectionpy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `collectionpy-1.1.1/collectionpy/chart/apexcharts.py` & `collectionpy-1.2.0/collectionpy/chart/apexcharts.py`

 * *Files identical despite different names*

### Comparing `collectionpy-1.1.1/collectionpy/chart/googlecharts.py` & `collectionpy-1.2.0/collectionpy/chart/googlecharts.py`

 * *Files identical despite different names*

### Comparing `collectionpy-1.1.1/collectionpy/date/__init__.py` & `collectionpy-1.2.0/collectionpy/date/__init__.py`

 * *Files identical despite different names*

### Comparing `collectionpy-1.1.1/collectionpy/date/dtget.py` & `collectionpy-1.2.0/collectionpy/date/dtget.py`

 * *Files identical despite different names*

### Comparing `collectionpy-1.1.1/collectionpy/date/dtmath.py` & `collectionpy-1.2.0/collectionpy/date/dtmath.py`

 * *Files identical despite different names*

### Comparing `collectionpy-1.1.1/collectionpy.egg-info/PKG-INFO` & `collectionpy-1.2.0/collectionpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collectionpy
-Version: 1.1.1
+Version: 1.2.0
 Summary: "collectionpy" is more than just a library; it is a comprehensive tool that provides efficient solutions for various areas, ranging from date manipulation and text formatting to the creation of impressive graphics.
 Description-Content-Type: text/markdown
 
 <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css">
 
 ## COLLECTIONPY
```

### Comparing `collectionpy-1.1.1/setup.py` & `collectionpy-1.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 
 # Carregar o conteúdo do arquivo README.md
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='collectionpy',
-    version='1.1.1',
+    version='1.2.0',
     description='"collectionpy" is more than just a library; it is a comprehensive tool that provides efficient solutions for various areas, ranging from date manipulation and text formatting to the creation of impressive graphics.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['collectionpy', 'collectionpy.chart', 'collectionpy.date', 'collectionpy.math', 'collectionpy.text'],
-    install_requires=[],
+    install_requires=['numpy'],
 )
```


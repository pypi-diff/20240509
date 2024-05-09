# Comparing `tmp/first_glance-1.0.0.tar.gz` & `tmp/first_glance-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "first_glance-1.0.0.tar", last modified: Thu May  9 18:45:49 2024, max compression
+gzip compressed data, was "first_glance-1.0.1.tar", last modified: Thu May  9 18:11:46 2024, max compression
```

## Comparing `first_glance-1.0.0.tar` & `first_glance-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jordankanius   (501) staff       (20)        0 2024-05-09 18:45:49.760676 first_glance-1.0.0/
--rw-r--r--   0 jordankanius   (501) staff       (20)      707 2024-05-09 18:45:49.760470 first_glance-1.0.0/PKG-INFO
--rw-r--r--   0 jordankanius   (501) staff       (20)     1977 2024-05-09 17:36:07.000000 first_glance-1.0.0/README.md
-drwxr-xr-x   0 jordankanius   (501) staff       (20)        0 2024-05-09 18:45:49.759306 first_glance-1.0.0/first_glance/
--rw-r--r--   0 jordankanius   (501) staff       (20)        0 2024-05-08 15:32:57.000000 first_glance-1.0.0/first_glance/__init__.py
--rw-r--r--   0 jordankanius   (501) staff       (20)     6039 2024-05-09 18:16:37.000000 first_glance-1.0.0/first_glance/report.py
-drwxr-xr-x   0 jordankanius   (501) staff       (20)        0 2024-05-09 18:45:49.760158 first_glance-1.0.0/first_glance.egg-info/
--rw-r--r--   0 jordankanius   (501) staff       (20)      707 2024-05-09 18:45:49.000000 first_glance-1.0.0/first_glance.egg-info/PKG-INFO
--rw-r--r--   0 jordankanius   (501) staff       (20)      245 2024-05-09 18:45:49.000000 first_glance-1.0.0/first_glance.egg-info/SOURCES.txt
--rw-r--r--   0 jordankanius   (501) staff       (20)        1 2024-05-09 18:45:49.000000 first_glance-1.0.0/first_glance.egg-info/dependency_links.txt
--rw-r--r--   0 jordankanius   (501) staff       (20)       15 2024-05-09 18:45:49.000000 first_glance-1.0.0/first_glance.egg-info/requires.txt
--rw-r--r--   0 jordankanius   (501) staff       (20)       13 2024-05-09 18:45:49.000000 first_glance-1.0.0/first_glance.egg-info/top_level.txt
--rw-r--r--   0 jordankanius   (501) staff       (20)       38 2024-05-09 18:45:49.760713 first_glance-1.0.0/setup.cfg
--rw-r--r--   0 jordankanius   (501) staff       (20)      860 2024-05-09 18:19:42.000000 first_glance-1.0.0/setup.py
+drwxr-xr-x   0 jordankanius   (501) staff       (20)        0 2024-05-09 18:11:46.659210 first_glance-1.0.1/
+-rw-r--r--   0 jordankanius   (501) staff       (20)      673 2024-05-09 18:11:46.658981 first_glance-1.0.1/PKG-INFO
+-rw-r--r--   0 jordankanius   (501) staff       (20)     1977 2024-05-09 17:36:07.000000 first_glance-1.0.1/README.md
+drwxr-xr-x   0 jordankanius   (501) staff       (20)        0 2024-05-09 18:11:46.657795 first_glance-1.0.1/first_glance/
+-rw-r--r--   0 jordankanius   (501) staff       (20)        0 2024-05-08 15:32:57.000000 first_glance-1.0.1/first_glance/__init__.py
+-rw-r--r--   0 jordankanius   (501) staff       (20)     6063 2024-05-09 17:58:32.000000 first_glance-1.0.1/first_glance/report.py
+drwxr-xr-x   0 jordankanius   (501) staff       (20)        0 2024-05-09 18:11:46.658662 first_glance-1.0.1/first_glance.egg-info/
+-rw-r--r--   0 jordankanius   (501) staff       (20)      673 2024-05-09 18:11:46.000000 first_glance-1.0.1/first_glance.egg-info/PKG-INFO
+-rw-r--r--   0 jordankanius   (501) staff       (20)      245 2024-05-09 18:11:46.000000 first_glance-1.0.1/first_glance.egg-info/SOURCES.txt
+-rw-r--r--   0 jordankanius   (501) staff       (20)        1 2024-05-09 18:11:46.000000 first_glance-1.0.1/first_glance.egg-info/dependency_links.txt
+-rw-r--r--   0 jordankanius   (501) staff       (20)       15 2024-05-09 18:11:46.000000 first_glance-1.0.1/first_glance.egg-info/requires.txt
+-rw-r--r--   0 jordankanius   (501) staff       (20)       13 2024-05-09 18:11:46.000000 first_glance-1.0.1/first_glance.egg-info/top_level.txt
+-rw-r--r--   0 jordankanius   (501) staff       (20)       38 2024-05-09 18:11:46.659247 first_glance-1.0.1/setup.cfg
+-rw-r--r--   0 jordankanius   (501) staff       (20)      826 2024-05-09 18:11:21.000000 first_glance-1.0.1/setup.py
```

### Comparing `first_glance-1.0.0/PKG-INFO` & `first_glance-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: first_glance
-Version: 1.0.0
+Version: 1.0.1
 Summary: Quick plotting and examination for early analysis of data
 Home-page: https://github.com/Kanustu/analysis_reporting
 Author: Jordan Kanius
 Author-email: Kaniusjordan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: seaborn
 
-Python package used for early inital analysis with the ability to return plots(boxplots, histograms and heatmap)    and also return dataframe with a count of nulls, column datatype, and descriptive stats for each column within the data
+Python package used for early inital analysis with the ability to return plots(boxplots, histograms and heatmap)    and a count of nulls, datatype, and descriptive stats for each column within the data
```

### Comparing `first_glance-1.0.0/README.md` & `first_glance-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `first_glance-1.0.0/first_glance/report.py` & `first_glance-1.0.1/first_glance/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                        if data[column].dtypes == 'int64' or data[column].dtypes == 'float64']
     num_plots = len(numeric_columns)
     if num_plots == 0:
         print("No numeric columns found in the DataFrame.")
         return
     
     # Determine the number of rows and columns for subplots
-    num_cols = min(2, num_plots)
+    num_cols = min(2, num_plots)  # Maximum of 3 columns
     num_rows = (num_plots + num_cols - 1) // num_cols
     
     # Create subplots
     if num_cols <= 1:
         raise ValueError('There must be more than one numeric column in the dataframe')
     elif num_cols == 2:
         fig, axes = plt.subplots(num_plots, 1, figsize=(8, num_plots * 5))
```

### Comparing `first_glance-1.0.0/first_glance.egg-info/PKG-INFO` & `first_glance-1.0.1/first_glance.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: first-glance
-Version: 1.0.0
+Version: 1.0.1
 Summary: Quick plotting and examination for early analysis of data
 Home-page: https://github.com/Kanustu/analysis_reporting
 Author: Jordan Kanius
 Author-email: Kaniusjordan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: seaborn
 
-Python package used for early inital analysis with the ability to return plots(boxplots, histograms and heatmap)    and also return dataframe with a count of nulls, column datatype, and descriptive stats for each column within the data
+Python package used for early inital analysis with the ability to return plots(boxplots, histograms and heatmap)    and a count of nulls, datatype, and descriptive stats for each column within the data
```

### Comparing `first_glance-1.0.0/setup.py` & `first_glance-1.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='first_glance',
-    version='1.0.0',
+    version='1.0.1',
     author='Jordan Kanius',
     author_email='Kaniusjordan@gmail.com',
     description='Quick plotting and examination for early analysis of data',
     long_description='Python package used for early inital analysis with the ability to return plots(boxplots, histograms and heatmap)\
-    and also return dataframe with a count of nulls, column datatype, and descriptive stats for each column within the data',
+    and a count of nulls, datatype, and descriptive stats for each column within the data',
     long_description_content_type='text/markdown',
     url='https://github.com/Kanustu/analysis_reporting',
     packages=find_packages(),
     install_requires=['pandas', 'seaborn'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```


# Comparing `tmp/village-data-analysis-1.2.tar.gz` & `tmp/village-data-analysis-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "village-data-analysis-1.2.tar", last modified: Thu Apr 25 12:42:03 2024, max compression
+gzip compressed data, was "village-data-analysis-1.3.tar", last modified: Thu May  9 09:40:40 2024, max compression
```

## Comparing `village-data-analysis-1.2.tar` & `village-data-analysis-1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-04-25 12:42:03.050438 village-data-analysis-1.2/
--rw-r--r--   0 istvan    (1000) istvan    (1000)     1036 2024-04-25 12:42:03.050438 village-data-analysis-1.2/PKG-INFO
--rw-r--r--   0 istvan    (1000) istvan    (1000)      753 2024-04-24 12:43:39.000000 village-data-analysis-1.2/README.md
--rw-r--r--   0 istvan    (1000) istvan    (1000)       38 2024-04-25 12:42:03.050438 village-data-analysis-1.2/setup.cfg
--rw-r--r--   0 istvan    (1000) istvan    (1000)      648 2024-04-25 12:41:52.000000 village-data-analysis-1.2/setup.py
-drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-04-25 12:42:03.050438 village-data-analysis-1.2/village_data_analysis/
--rw-r--r--   0 istvan    (1000) istvan    (1000)        0 2024-04-22 12:22:55.000000 village-data-analysis-1.2/village_data_analysis/__init__.py
--rw-r--r--   0 istvan    (1000) istvan    (1000)    14800 2024-04-22 12:22:55.000000 village-data-analysis-1.2/village_data_analysis/analyzer.py
--rw-r--r--   0 istvan    (1000) istvan    (1000)     1107 2024-04-22 12:22:55.000000 village-data-analysis-1.2/village_data_analysis/coord_converter.py
--rw-r--r--   0 istvan    (1000) istvan    (1000)     4294 2024-04-22 12:22:55.000000 village-data-analysis-1.2/village_data_analysis/data_create.py
--rw-r--r--   0 istvan    (1000) istvan    (1000)      708 2024-04-22 12:22:55.000000 village-data-analysis-1.2/village_data_analysis/helpers.py
-drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-04-25 12:42:03.050438 village-data-analysis-1.2/village_data_analysis.egg-info/
--rw-r--r--   0 istvan    (1000) istvan    (1000)     1036 2024-04-25 12:42:03.000000 village-data-analysis-1.2/village_data_analysis.egg-info/PKG-INFO
--rw-r--r--   0 istvan    (1000) istvan    (1000)      421 2024-04-25 12:42:03.000000 village-data-analysis-1.2/village_data_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 istvan    (1000) istvan    (1000)        1 2024-04-25 12:42:03.000000 village-data-analysis-1.2/village_data_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 istvan    (1000) istvan    (1000)       52 2024-04-25 12:42:03.000000 village-data-analysis-1.2/village_data_analysis.egg-info/requires.txt
--rw-r--r--   0 istvan    (1000) istvan    (1000)       22 2024-04-25 12:42:03.000000 village-data-analysis-1.2/village_data_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-05-09 09:40:40.240174 village-data-analysis-1.3/
+-rw-r--r--   0 istvan    (1000) istvan    (1000)     1036 2024-05-09 09:40:40.240174 village-data-analysis-1.3/PKG-INFO
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      753 2024-04-24 12:43:39.000000 village-data-analysis-1.3/README.md
+-rw-r--r--   0 istvan    (1000) istvan    (1000)       38 2024-05-09 09:40:40.240174 village-data-analysis-1.3/setup.cfg
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      648 2024-05-09 09:39:52.000000 village-data-analysis-1.3/setup.py
+drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-05-09 09:40:40.240174 village-data-analysis-1.3/village_data_analysis/
+-rw-r--r--   0 istvan    (1000) istvan    (1000)        0 2024-04-22 12:22:55.000000 village-data-analysis-1.3/village_data_analysis/__init__.py
+-rw-r--r--   0 istvan    (1000) istvan    (1000)    14815 2024-05-09 09:39:07.000000 village-data-analysis-1.3/village_data_analysis/analyzer.py
+-rw-r--r--   0 istvan    (1000) istvan    (1000)     1107 2024-04-22 12:22:55.000000 village-data-analysis-1.3/village_data_analysis/coord_converter.py
+-rw-r--r--   0 istvan    (1000) istvan    (1000)     4294 2024-04-22 12:22:55.000000 village-data-analysis-1.3/village_data_analysis/data_create.py
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      708 2024-04-22 12:22:55.000000 village-data-analysis-1.3/village_data_analysis/helpers.py
+drwxr-xr-x   0 istvan    (1000) istvan    (1000)        0 2024-05-09 09:40:40.240174 village-data-analysis-1.3/village_data_analysis.egg-info/
+-rw-r--r--   0 istvan    (1000) istvan    (1000)     1036 2024-05-09 09:40:40.000000 village-data-analysis-1.3/village_data_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 istvan    (1000) istvan    (1000)      421 2024-05-09 09:40:40.000000 village-data-analysis-1.3/village_data_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 istvan    (1000) istvan    (1000)        1 2024-05-09 09:40:40.000000 village-data-analysis-1.3/village_data_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 istvan    (1000) istvan    (1000)       52 2024-05-09 09:40:40.000000 village-data-analysis-1.3/village_data_analysis.egg-info/requires.txt
+-rw-r--r--   0 istvan    (1000) istvan    (1000)       22 2024-05-09 09:40:40.000000 village-data-analysis-1.3/village_data_analysis.egg-info/top_level.txt
```

### Comparing `village-data-analysis-1.2/PKG-INFO` & `village-data-analysis-1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: village-data-analysis
-Version: 1.2
+Version: 1.3
 Summary: Generates report in xlsx and csv format about the inputed geometric shape file within the provided time range.
 Author: Istvan Gallo
 Author-email: istvan.gallo@lexunit.hu
 Description-Content-Type: text/markdown
 
 # Village data analysis package
```

### Comparing `village-data-analysis-1.2/README.md` & `village-data-analysis-1.3/README.md`

 * *Files identical despite different names*

### Comparing `village-data-analysis-1.2/setup.py` & `village-data-analysis-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='village-data-analysis',
-    version='1.2',
+    version='1.3',
     packages=find_packages(),
     author='Istvan Gallo',
     author_email='istvan.gallo@lexunit.hu',
     description='Generates report in xlsx and csv format about the inputed geometric shape file within the provided time range.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
```

### Comparing `village-data-analysis-1.2/village_data_analysis/analyzer.py` & `village-data-analysis-1.3/village_data_analysis/analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     global tif
     previous_year_map = dict()
     grid_dict = dict()
     first_year_village_count = 0
     for i, p in enumerate(tqdm(shapefile_paths, "Preparing shapefiles: ", len(shapefile_paths))):
         gdf = gpd.read_file(p[1])
         # This is specific for JT's data
-        for ID_variant in [f"ID{p[0]}_d", f"ID{p[0]}", "iddesa", "IDDESA"]:
+        for ID_variant in [f"ID{p[0]}_d", f"ID{p[0]}", "iddesa", "IDDESA", f"IPUM{p[0]}"]:
             if ID_variant in gdf.columns:
                 break
         gdf = gdf[[ID_variant, 'geometry']]
         gdf.rename(columns={ID_variant: 'village_id'}, inplace=True)
 
         gdf = gdf.groupby("village_id").agg({'geometry': merge_polygons})
         if i == 0:
```

### Comparing `village-data-analysis-1.2/village_data_analysis/coord_converter.py` & `village-data-analysis-1.3/village_data_analysis/coord_converter.py`

 * *Files identical despite different names*

### Comparing `village-data-analysis-1.2/village_data_analysis/data_create.py` & `village-data-analysis-1.3/village_data_analysis/data_create.py`

 * *Files identical despite different names*

### Comparing `village-data-analysis-1.2/village_data_analysis/helpers.py` & `village-data-analysis-1.3/village_data_analysis/helpers.py`

 * *Files identical despite different names*

### Comparing `village-data-analysis-1.2/village_data_analysis.egg-info/PKG-INFO` & `village-data-analysis-1.3/village_data_analysis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: village-data-analysis
-Version: 1.2
+Version: 1.3
 Summary: Generates report in xlsx and csv format about the inputed geometric shape file within the provided time range.
 Author: Istvan Gallo
 Author-email: istvan.gallo@lexunit.hu
 Description-Content-Type: text/markdown
 
 # Village data analysis package
```


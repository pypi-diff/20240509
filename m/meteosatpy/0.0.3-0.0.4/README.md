# Comparing `tmp/meteosatpy-0.0.3.tar.gz` & `tmp/meteosatpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meteosatpy-0.0.3.tar", last modified: Mon Feb 26 21:36:39 2024, max compression
+gzip compressed data, was "meteosatpy-0.0.4.tar", last modified: Thu May  9 20:47:58 2024, max compression
```

## Comparing `meteosatpy-0.0.3.tar` & `meteosatpy-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 21:36:39.424502 meteosatpy-0.0.3/
--rw-rw-rw-   0        0        0     1119 2024-02-20 19:05:25.000000 meteosatpy-0.0.3/LICENCE.txt
--rw-rw-rw-   0        0        0     3978 2024-02-26 21:36:39.423502 meteosatpy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3487 2024-02-26 21:01:18.000000 meteosatpy-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-26 21:36:39.399962 meteosatpy-0.0.3/meteosatpy/
--rw-rw-rw-   0        0        0      106 2024-02-26 03:39:32.000000 meteosatpy-0.0.3/meteosatpy/__init__.py
--rw-rw-rw-   0        0        0     3110 2024-02-23 19:00:04.000000 meteosatpy-0.0.3/meteosatpy/chirps.py
--rw-rw-rw-   0        0        0     3478 2024-02-23 19:00:23.000000 meteosatpy-0.0.3/meteosatpy/cmorph.py
--rw-rw-rw-   0        0        0     6528 2024-02-26 20:30:08.000000 meteosatpy-0.0.3/meteosatpy/imerg.py
--rw-rw-rw-   0        0        0     3940 2024-02-26 14:13:10.000000 meteosatpy-0.0.3/meteosatpy/mswep.py
--rw-rw-rw-   0        0        0     6791 2024-02-26 20:29:37.000000 meteosatpy-0.0.3/meteosatpy/utils.py
--rw-rw-rw-   0        0        0       83 2024-02-21 18:57:20.000000 meteosatpy-0.0.3/meteosatpy/warnings.py
-drwxrwxrwx   0        0        0        0 2024-02-26 21:36:39.422501 meteosatpy-0.0.3/meteosatpy.egg-info/
--rw-rw-rw-   0        0        0     3978 2024-02-26 21:36:39.000000 meteosatpy-0.0.3/meteosatpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-02-26 21:36:39.000000 meteosatpy-0.0.3/meteosatpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 21:36:39.000000 meteosatpy-0.0.3/meteosatpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-02-26 21:36:39.000000 meteosatpy-0.0.3/meteosatpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-26 21:36:39.000000 meteosatpy-0.0.3/meteosatpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 21:36:39.424502 meteosatpy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1061 2024-02-26 21:36:32.000000 meteosatpy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:47:58.006329 meteosatpy-0.0.4/
+-rw-rw-rw-   0        0        0     1119 2024-02-20 19:05:25.000000 meteosatpy-0.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0     3979 2024-05-09 20:47:58.005328 meteosatpy-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3488 2024-03-05 03:57:58.000000 meteosatpy-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 20:47:57.955216 meteosatpy-0.0.4/meteosatpy/
+-rw-rw-rw-   0        0        0      106 2024-02-26 03:39:32.000000 meteosatpy-0.0.4/meteosatpy/__init__.py
+-rw-rw-rw-   0        0        0     3376 2024-05-09 20:36:48.000000 meteosatpy-0.0.4/meteosatpy/chirps.py
+-rw-rw-rw-   0        0        0     3478 2024-02-23 19:00:23.000000 meteosatpy-0.0.4/meteosatpy/cmorph.py
+-rw-rw-rw-   0        0        0     6528 2024-02-26 20:30:08.000000 meteosatpy-0.0.4/meteosatpy/imerg.py
+-rw-rw-rw-   0        0        0     3940 2024-02-26 14:13:10.000000 meteosatpy-0.0.4/meteosatpy/mswep.py
+-rw-rw-rw-   0        0        0     5273 2024-03-04 20:31:18.000000 meteosatpy-0.0.4/meteosatpy/persiann.py
+-rw-rw-rw-   0        0        0     8325 2024-03-04 20:25:46.000000 meteosatpy-0.0.4/meteosatpy/utils.py
+-rw-rw-rw-   0        0        0       83 2024-02-21 18:57:20.000000 meteosatpy-0.0.4/meteosatpy/warnings.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:47:58.004328 meteosatpy-0.0.4/meteosatpy.egg-info/
+-rw-rw-rw-   0        0        0     3979 2024-05-09 20:47:57.000000 meteosatpy-0.0.4/meteosatpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-05-09 20:47:57.000000 meteosatpy-0.0.4/meteosatpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 20:47:57.000000 meteosatpy-0.0.4/meteosatpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-09 20:47:57.000000 meteosatpy-0.0.4/meteosatpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 20:47:57.000000 meteosatpy-0.0.4/meteosatpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 20:47:58.006329 meteosatpy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1061 2024-05-09 20:44:56.000000 meteosatpy-0.0.4/setup.py
```

### Comparing `meteosatpy-0.0.3/LICENCE.txt` & `meteosatpy-0.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `meteosatpy-0.0.3/PKG-INFO` & `meteosatpy-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteosatpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library designed for downloading and managing meteorological data sourced from satellites and global models.
 Home-page: https://github.com/jusethCS/meteosatpy
 Author: Juseth Enrique Chancay Sánchez
 Author-email: juseth.chancay@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
@@ -43,15 +43,15 @@
 - [geopandas](https://readthedocs.org/projects/geopandas/): Analysis and manipulation of geographical data.
 - [request](https://requests.readthedocs.io/en/latest/): HTTP library for making requests and working with web APIs.
 
 Prior to installing **MeteoSatPy** using PyPi, we recommend creating a new conda environment with dependencies:
 
 ```sh
 # Conda
-conda create -n [env_name] geopandas rasterio xarray request
+conda create -n [env_name] geopandas rasterio xarray requests
 ```
 
 If you need to download [MSWEP](https://www.gloh2o.org/mswep/) data, you'll need to install [Rclone](https://anaconda.org/conda-forge/rclone).
 
 ```sh
 # Conda
 conda install conda-forge::rclone
```

### Comparing `meteosatpy-0.0.3/README.md` & `meteosatpy-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 - [geopandas](https://readthedocs.org/projects/geopandas/): Analysis and manipulation of geographical data.
 - [request](https://requests.readthedocs.io/en/latest/): HTTP library for making requests and working with web APIs.
 
 Prior to installing **MeteoSatPy** using PyPi, we recommend creating a new conda environment with dependencies:
 
 ```sh
 # Conda
-conda create -n [env_name] geopandas rasterio xarray request
+conda create -n [env_name] geopandas rasterio xarray requests
 ```
 
 If you need to download [MSWEP](https://www.gloh2o.org/mswep/) data, you'll need to install [Rclone](https://anaconda.org/conda-forge/rclone).
 
 ```sh
 # Conda
 conda install conda-forge::rclone
```

### Comparing `meteosatpy-0.0.3/meteosatpy/chirps.py` & `meteosatpy-0.0.4/meteosatpy/chirps.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,26 +50,32 @@
             filedate = date.strftime("%Y.%m")
         else:
             filedate = year
 
         # Construct download URL
         if timestep == "daily":
             url = f"{server}/{product}/p05/{year}/chirps-v2.0.{filedate}.tif.gz"
-        else:
+        elif timestep == "monthly":
             url = f"{server}/{product}/chirps-v2.0.{filedate}.tif.gz"
+        else:
+            url = f"{server}/{product}/chirps-v2.0.{filedate}.tif"
         
         # Download and ungzip file
         try:
-            urllib.request.urlretrieve(url, "temporal.tif.gz")        
+            if timestep != "annual":
+                urllib.request.urlretrieve(url, "temporal.tif.gz")
+            else:
+                urllib.request.urlretrieve(url, "temporal.tif")     
         except Exception as e:
             print(f"Error occurred while downloading: {e}")
             return
             
         # Ungzip the file
-        ungzip("temporal.tif.gz")
+        if timestep != "annual":
+            ungzip("temporal.tif.gz")
 
         # Mask the raster file to required extent
         if extent is None:
             shutil.copyfile("temporal.tif", outpath)
         else:
             mask = createMask(north=extent[0], south=extent[1], 
                               east=extent[2], west=extent[3])
```

### Comparing `meteosatpy-0.0.3/meteosatpy/cmorph.py` & `meteosatpy-0.0.4/meteosatpy/cmorph.py`

 * *Files identical despite different names*

### Comparing `meteosatpy-0.0.3/meteosatpy/imerg.py` & `meteosatpy-0.0.4/meteosatpy/imerg.py`

 * *Files identical despite different names*

### Comparing `meteosatpy-0.0.3/meteosatpy/mswep.py` & `meteosatpy-0.0.4/meteosatpy/mswep.py`

 * *Files identical despite different names*

### Comparing `meteosatpy-0.0.3/meteosatpy/utils.py` & `meteosatpy-0.0.4/meteosatpy/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -221,8 +221,61 @@
 
     # Set appropriate permissions for Linux/macOS
     if platform.system() != "Windows":
         subprocess.Popen('chmod og-rw ~/.netrc', shell=True)
     else:
         # Copy dodsrc to working directory in Windows  
         shutil.copy2(homeDir + '.dodsrc', os.getcwd())
-        print('Copied .dodsrc to:', os.getcwd())
+        print('Copied .dodsrc to:', os.getcwd())
+
+
+
+
+def get_params_persiann(date, timestep, data_type):
+    """
+    Get parameters for PERSIANN data download based on date, timestep, and data type.
+
+    Args:
+        date (datetime): A datetime object representing the date.
+        timestep (str): A string specifying the timestep: "hourly", "3hourly", 
+                        "6hourly", "daily", "monthly", or "yearly".
+        data_type (str): A string specifying the data type: "PERSIANN", "CCS", 
+                        "CDR", or "PDIR".
+
+    Returns:
+        dict: A dictionary containing parameters for PERSIANN data download.
+    """
+    if timestep == "hourly":
+        ds = date.strftime("%Y%m%d%H")
+        dtm = "1hrly"
+        dtx = "1h"
+    elif timestep == "3hourly":
+        ds = date.strftime("%Y%m%d%H")
+        dtm = "3hrly"
+        dtx = "3h"
+    elif timestep == "6hourly":
+        ds = date.strftime("%Y%m%d%H")
+        dtm = "6hrly"
+        dtx = "6h"
+    elif timestep == "daily":
+        ds = date.strftime("%Y%m%d")
+        dtm = timestep
+        dtx = "1d"
+    elif timestep == "monthly":
+        ds = date.strftime("%Y%m")
+        dtm = timestep
+        dtx = "1m"
+    elif timestep == "yearly":
+        ds = date.strftime("%Y")
+        dtm = timestep
+        dtx = "1y"
+
+    params = {
+        'startDate': ds,
+        'endDate': ds,
+        'timestep': dtm,
+        'timestepAlt': dtx,
+        'dataType': data_type,
+        'format': "Tif",
+        'compression': "zip"
+    }
+    return params
```

### Comparing `meteosatpy-0.0.3/meteosatpy.egg-info/PKG-INFO` & `meteosatpy-0.0.4/meteosatpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meteosatpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Library designed for downloading and managing meteorological data sourced from satellites and global models.
 Home-page: https://github.com/jusethCS/meteosatpy
 Author: Juseth Enrique Chancay Sánchez
 Author-email: juseth.chancay@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
@@ -43,15 +43,15 @@
 - [geopandas](https://readthedocs.org/projects/geopandas/): Analysis and manipulation of geographical data.
 - [request](https://requests.readthedocs.io/en/latest/): HTTP library for making requests and working with web APIs.
 
 Prior to installing **MeteoSatPy** using PyPi, we recommend creating a new conda environment with dependencies:
 
 ```sh
 # Conda
-conda create -n [env_name] geopandas rasterio xarray request
+conda create -n [env_name] geopandas rasterio xarray requests
 ```
 
 If you need to download [MSWEP](https://www.gloh2o.org/mswep/) data, you'll need to install [Rclone](https://anaconda.org/conda-forge/rclone).
 
 ```sh
 # Conda
 conda install conda-forge::rclone
```

### Comparing `meteosatpy-0.0.3/setup.py` & `meteosatpy-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """ Setup file for meteosatpy. """
 
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 PACKAGE_NAME = 'meteosatpy'
 AUTHOR = 'Juseth Enrique Chancay Sánchez'
 AUTHOR_EMAIL = 'juseth.chancay@gmail.com'
 URL = 'https://github.com/jusethCS/meteosatpy'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Library designed for downloading and managing meteorological data sourced from satellites and global models.'
```


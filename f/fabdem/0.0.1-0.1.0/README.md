# Comparing `tmp/fabdem-0.0.1.tar.gz` & `tmp/fabdem-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabdem-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fabdem-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fabdem-0.0.1.tar` & `fabdem-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       51 2024-05-08 21:54:26.981557 fabdem-0.0.1/.gitignore
--rw-r--r--   0        0        0    35823 2024-05-08 20:18:02.844371 fabdem-0.0.1/LICENSE
--rw-r--r--   0        0        0     1443 2024-05-08 21:57:41.098688 fabdem-0.0.1/README.md
--rw-r--r--   0        0        0     1097 2024-05-08 21:01:40.919396 fabdem-0.0.1/examples/narok.ipynb
--rw-r--r--   0        0        0     6117 2024-05-08 20:17:04.945650 fabdem-0.0.1/fabdem.py
--rw-r--r--   0        0        0      358 2024-05-09 13:12:59.340950 fabdem-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      331 2024-05-08 21:05:19.898275 fabdem-0.0.1/test/narok.py
--rw-r--r--   0        0        0     1736 1970-01-01 00:00:00.000000 fabdem-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       67 2024-05-09 13:45:54.394485 fabdem-0.1.0/.gitignore
+-rw-r--r--   0        0        0    35823 2024-05-08 20:18:02.844371 fabdem-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1936 2024-05-09 13:48:36.057950 fabdem-0.1.0/README.md
+-rw-r--r--   0        0        0     1097 2024-05-08 21:01:40.919396 fabdem-0.1.0/examples/narok.ipynb
+-rw-r--r--   0        0        0     6117 2024-05-09 13:51:57.333951 fabdem-0.1.0/fabdem.py
+-rw-r--r--   0        0        0      347 2024-05-09 13:45:26.669871 fabdem-0.1.0/fabdem.yml
+-rw-r--r--   0        0        0      419 2024-05-09 13:55:32.030460 fabdem-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      331 2024-05-08 21:05:19.898275 fabdem-0.1.0/test/narok.py
+-rw-r--r--   0        0        0     2267 1970-01-01 00:00:00.000000 fabdem-0.1.0/PKG-INFO
```

### Comparing `fabdem-0.0.1/LICENSE` & `fabdem-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabdem-0.0.1/README.md` & `fabdem-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Download FABDEM data: a DEM with forests and buildings removed using ML.
 
 FABDEM homepage: https://data.bris.ac.uk/data/dataset/s5hqmjcdj8yo2ibzi9b4ew3sn
 
 ## Installation
 
-To install the package using pip
+To install the package using *pip*
 ```shell
 pip install fabdem
 ```
 
 ## Usage
 
 Define coordinates bounding the area of interest:
@@ -22,28 +22,44 @@
 import fabdem
 fabdem.download(bounds, output_path="dem.tif")
 ```
 Supports any raster format supported by GDAL.
 
 ## Development
 
-To install the package locally for development, run:
+1. Clone this repository
+```shell
+git clone https://github.com/jantomec/fabdem.git
+```
+
+2. Create a new conda environment
+```shell
+conda create --file fabdem.yml
+```
+or alternatively update the existing one
+```shell
+conda env update --file fabdem.yml [--prune]
+```
+> **_NOTE:_** The `--prune` option causes conda to remove any dependencies that are no longer required from the environment.
+
+3. To install the package locally for development, run:
 ```shell
 flit install --symlink
 ```
-`--symlink` option tells flit to create a symbolic link to your package directory inside the site-packages directory of your environment instead of copying files. This is useful for development, as changes in your package directory immediately affect the installed package without needing reinstallation.
+The `--symlink` option tells flit to create a symbolic link to your package directory inside the site-packages directory of your environment instead of copying files. This is useful for development, as changes in your package directory immediately affect the installed package without needing reinstallation.
 
-Run this command to upload the code to PyPI:
+4. Run this command to upload the code to PyPI:
 ```shell
 flit publish
 ```
 
 ### TODO:
-[ ] Create a conda package.
-[ ] Download only part of a zip.
+- [ ] Create a conda package.
+- [ ] Download only part of a zip.
 
 ### Resources:
 - [Python Packaging](https://packaging.python.org/en/latest/overview/)
 - [TOML Format](https://github.com/toml-lang/toml)
 - [flit](https://flit.pypa.io/en/latest/)
 - [PEP 8 - Naming Conventions](https://peps.python.org/pep-0008/#naming-conventions)
-- [PEP 484 – Type Hints](https://peps.python.org/pep-0484/)
+- [PEP 484 – Type Hints](https://peps.python.org/pep-0484/)
+- [conda-forge](https://conda-forge.org/docs/maintainer/adding_pkgs/)
```

### Comparing `fabdem-0.0.1/examples/narok.ipynb` & `fabdem-0.1.0/examples/narok.ipynb`

 * *Files identical despite different names*

### Comparing `fabdem-0.0.1/fabdem.py` & `fabdem-0.1.0/fabdem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Download FABDEM data: a DEM with forests and buildings removed using ML."""
 
-__version__ = "0.0.1"
+__version__ = "0.1.0"
 __author__ = "Jan Tomec"
 
 
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from zipfile import ZipFile
 import requests
```

### Comparing `fabdem-0.0.1/PKG-INFO` & `fabdem-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: fabdem
-Version: 0.0.1
+Version: 0.1.0
 Summary: Download FABDEM data: a DEM with forests and buildings removed using ML.
 Author-email: Jan Tomec <jan.tomec@c3m.si>
 Description-Content-Type: text/markdown
 Requires-Dist: requests >= 2.25
 Requires-Dist: geopandas >= 0.14
 Requires-Dist: tqdm >= 4.66
 Requires-Dist: rasterio >= 1.3
+Project-URL: Home, https://github.com/jantomec/fabdem
 
 # FABDEM
 
 Download FABDEM data: a DEM with forests and buildings removed using ML.
 
 FABDEM homepage: https://data.bris.ac.uk/data/dataset/s5hqmjcdj8yo2ibzi9b4ew3sn
 
 ## Installation
 
-To install the package using pip
+To install the package using *pip*
 ```shell
 pip install fabdem
 ```
 
 ## Usage
 
 Define coordinates bounding the area of interest:
@@ -33,28 +34,44 @@
 import fabdem
 fabdem.download(bounds, output_path="dem.tif")
 ```
 Supports any raster format supported by GDAL.
 
 ## Development
 
-To install the package locally for development, run:
+1. Clone this repository
+```shell
+git clone https://github.com/jantomec/fabdem.git
+```
+
+2. Create a new conda environment
+```shell
+conda create --file fabdem.yml
+```
+or alternatively update the existing one
+```shell
+conda env update --file fabdem.yml [--prune]
+```
+> **_NOTE:_** The `--prune` option causes conda to remove any dependencies that are no longer required from the environment.
+
+3. To install the package locally for development, run:
 ```shell
 flit install --symlink
 ```
-`--symlink` option tells flit to create a symbolic link to your package directory inside the site-packages directory of your environment instead of copying files. This is useful for development, as changes in your package directory immediately affect the installed package without needing reinstallation.
+The `--symlink` option tells flit to create a symbolic link to your package directory inside the site-packages directory of your environment instead of copying files. This is useful for development, as changes in your package directory immediately affect the installed package without needing reinstallation.
 
-Run this command to upload the code to PyPI:
+4. Run this command to upload the code to PyPI:
 ```shell
 flit publish
 ```
 
 ### TODO:
-[ ] Create a conda package.
-[ ] Download only part of a zip.
+- [ ] Create a conda package.
+- [ ] Download only part of a zip.
 
 ### Resources:
 - [Python Packaging](https://packaging.python.org/en/latest/overview/)
 - [TOML Format](https://github.com/toml-lang/toml)
 - [flit](https://flit.pypa.io/en/latest/)
 - [PEP 8 - Naming Conventions](https://peps.python.org/pep-0008/#naming-conventions)
 - [PEP 484 – Type Hints](https://peps.python.org/pep-0484/)
+- [conda-forge](https://conda-forge.org/docs/maintainer/adding_pkgs/)
```


# Comparing `tmp/sweb-0.5.tar.gz` & `tmp/sweb-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweb-0.5.tar", last modified: Thu May  9 17:08:06 2024, max compression
+gzip compressed data, was "sweb-0.6.tar", last modified: Thu May  9 17:15:28 2024, max compression
```

## Comparing `sweb-0.5.tar` & `sweb-0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 17:08:06.324033 sweb-0.5/
--rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.5/LICENSE
--rw-r--r--   0 redpist    (501) staff       (20)     5857 2024-05-09 17:08:06.323322 sweb-0.5/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)     4979 2024-05-09 17:03:21.000000 sweb-0.5/README.md
--rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 17:08:06.324284 sweb-0.5/setup.cfg
--rw-r--r--   0 redpist    (501) staff       (20)     1176 2024-05-09 17:05:11.000000 sweb-0.5/setup.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 17:08:06.317848 sweb-0.5/sweb/
--rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.5/sweb/__init__.py
--rw-r--r--   0 redpist    (501) staff       (20)     3643 2024-05-09 17:07:57.000000 sweb-0.5/sweb/app.py
--rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.5/sweb/asset_manager.py
--rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.5/sweb/data_loader.py
--rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.5/sweb/style_processor.py
--rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.5/sweb/template_processor.py
-drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 17:08:06.322353 sweb-0.5/sweb.egg-info/
--rw-r--r--   0 redpist    (501) staff       (20)     5857 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/PKG-INFO
--rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/SOURCES.txt
--rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/dependency_links.txt
--rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/entry_points.txt
--rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/requires.txt
--rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 17:08:06.000000 sweb-0.5/sweb.egg-info/top_level.txt
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 17:15:28.954631 sweb-0.6/
+-rw-r--r--   0 redpist    (501) staff       (20)     1072 2024-05-09 10:54:39.000000 sweb-0.6/LICENSE
+-rw-r--r--   0 redpist    (501) staff       (20)     5787 2024-05-09 17:15:28.954122 sweb-0.6/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)     4909 2024-05-09 17:15:00.000000 sweb-0.6/README.md
+-rw-r--r--   0 redpist    (501) staff       (20)       38 2024-05-09 17:15:28.954736 sweb-0.6/setup.cfg
+-rw-r--r--   0 redpist    (501) staff       (20)     1176 2024-05-09 17:15:09.000000 sweb-0.6/setup.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 17:15:28.950493 sweb-0.6/sweb/
+-rw-r--r--   0 redpist    (501) staff       (20)        0 2024-05-09 10:58:50.000000 sweb-0.6/sweb/__init__.py
+-rw-r--r--   0 redpist    (501) staff       (20)     3643 2024-05-09 17:07:57.000000 sweb-0.6/sweb/app.py
+-rw-r--r--   0 redpist    (501) staff       (20)      449 2024-05-09 11:00:23.000000 sweb-0.6/sweb/asset_manager.py
+-rw-r--r--   0 redpist    (501) staff       (20)      832 2024-05-09 11:00:48.000000 sweb-0.6/sweb/data_loader.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1466 2024-05-09 11:00:48.000000 sweb-0.6/sweb/style_processor.py
+-rw-r--r--   0 redpist    (501) staff       (20)     1317 2024-05-09 11:00:48.000000 sweb-0.6/sweb/template_processor.py
+drwxr-xr-x   0 redpist    (501) staff       (20)        0 2024-05-09 17:15:28.953511 sweb-0.6/sweb.egg-info/
+-rw-r--r--   0 redpist    (501) staff       (20)     5787 2024-05-09 17:15:28.000000 sweb-0.6/sweb.egg-info/PKG-INFO
+-rw-r--r--   0 redpist    (501) staff       (20)      318 2024-05-09 17:15:28.000000 sweb-0.6/sweb.egg-info/SOURCES.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        1 2024-05-09 17:15:28.000000 sweb-0.6/sweb.egg-info/dependency_links.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       39 2024-05-09 17:15:28.000000 sweb-0.6/sweb.egg-info/entry_points.txt
+-rw-r--r--   0 redpist    (501) staff       (20)       16 2024-05-09 17:15:28.000000 sweb-0.6/sweb.egg-info/requires.txt
+-rw-r--r--   0 redpist    (501) staff       (20)        5 2024-05-09 17:15:28.000000 sweb-0.6/sweb.egg-info/top_level.txt
```

### Comparing `sweb-0.5/LICENSE` & `sweb-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sweb-0.5/PKG-INFO` & `sweb-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweb
-Version: 0.5
+Version: 0.6
 Summary: SWEB is a static website generator that processes templates, styles, and assets
 Author: Jeremy LECERF
 Author-email: redpist.com@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -189,27 +189,24 @@
 would generate the following CSS file `dist/styles/style.css`:
 ```css
 body h1 {
   color: red;
 }
 ```
 
-
-
-
-## assets
+## Assets
 
 ## Path
 ```
 app/assets/
 ```
 
 ### Purpose
 
-Holds static files like images, fonts, and other media which are copied directly into the output directory without modification. These files are important for the multimedia elements of the site.
+Holds static files like images, fonts, and other media which are copied directly into the output directory without modification.
 
 ### Example
 
 If you have an image `app/assets/logo.png`, it would be copied to `dist/assets/logo.png` without any changes.
 
 
 ## How SWEB works?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweb Version: 0.5 Summary: SWEB is a static website
+Metadata-Version: 2.1 Name: sweb Version: 0.6 Summary: SWEB is a static website
 generator that processes templates, styles, and assets Author: Jeremy LECERF
 Author-email: redpist.com@gmail.com License: MIT Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -54,20 +54,19 @@
 index.html` ```html
 ************ HHeelllloo,, wwoorrlldd ttoo AA sswweebb pprroojjeecctt..!! ************
 ``` ## Styles ### Path ``` app/styles/ ``` ### Purpose Stores CSS & [SASS/SCSS]
 (https://sass-lang.com/) style sheets that control the look and feel of the
 website. These stylesheets are compiled and saved in the `dist/styles/` folder.
 ### Example The following `style.scss` file in the `app/styles/` folder:
 ```scss body { h1 { color: red; } } ``` would generate the following CSS file
-`dist/styles/style.css`: ```css body h1 { color: red; } ``` ## assets ## Path
+`dist/styles/style.css`: ```css body h1 { color: red; } ``` ## Assets ## Path
 ``` app/assets/ ``` ### Purpose Holds static files like images, fonts, and
 other media which are copied directly into the output directory without
-modification. These files are important for the multimedia elements of the
-site. ### Example If you have an image `app/assets/logo.png`, it would be
-copied to `dist/assets/logo.png` without any changes. ## How SWEB works? To
+modification. ### Example If you have an image `app/assets/logo.png`, it would
+be copied to `dist/assets/logo.png` without any changes. ## How SWEB works? To
 generate a website, SWEB: 1. Load the JSON data from the `app/data/` folder, 2.
 Generate the html from the handlebar templates in the `app/templates/` folder
 and save the result in the `dist/` folder, 3. Compile The CSS/SASS/SCSS files
 in the `app/styles/` folder and save the result the `dist/styles/` folder, 4.
 The media files in the `app/assets/` folder are copied as-is to the `dist/
 assets/` folder. 5. The `dist/` folder now contains a fully functional static
 website.
```

### Comparing `sweb-0.5/README.md` & `sweb-0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -165,27 +165,24 @@
 would generate the following CSS file `dist/styles/style.css`:
 ```css
 body h1 {
   color: red;
 }
 ```
 
-
-
-
-## assets
+## Assets
 
 ## Path
 ```
 app/assets/
 ```
 
 ### Purpose
 
-Holds static files like images, fonts, and other media which are copied directly into the output directory without modification. These files are important for the multimedia elements of the site.
+Holds static files like images, fonts, and other media which are copied directly into the output directory without modification.
 
 ### Example
 
 If you have an image `app/assets/logo.png`, it would be copied to `dist/assets/logo.png` without any changes.
 
 
 ## How SWEB works?
```

#### html2text {}

```diff
@@ -43,20 +43,19 @@
 index.html` ```html
 ************ HHeelllloo,, wwoorrlldd ttoo AA sswweebb pprroojjeecctt..!! ************
 ``` ## Styles ### Path ``` app/styles/ ``` ### Purpose Stores CSS & [SASS/SCSS]
 (https://sass-lang.com/) style sheets that control the look and feel of the
 website. These stylesheets are compiled and saved in the `dist/styles/` folder.
 ### Example The following `style.scss` file in the `app/styles/` folder:
 ```scss body { h1 { color: red; } } ``` would generate the following CSS file
-`dist/styles/style.css`: ```css body h1 { color: red; } ``` ## assets ## Path
+`dist/styles/style.css`: ```css body h1 { color: red; } ``` ## Assets ## Path
 ``` app/assets/ ``` ### Purpose Holds static files like images, fonts, and
 other media which are copied directly into the output directory without
-modification. These files are important for the multimedia elements of the
-site. ### Example If you have an image `app/assets/logo.png`, it would be
-copied to `dist/assets/logo.png` without any changes. ## How SWEB works? To
+modification. ### Example If you have an image `app/assets/logo.png`, it would
+be copied to `dist/assets/logo.png` without any changes. ## How SWEB works? To
 generate a website, SWEB: 1. Load the JSON data from the `app/data/` folder, 2.
 Generate the html from the handlebar templates in the `app/templates/` folder
 and save the result in the `dist/` folder, 3. Compile The CSS/SASS/SCSS files
 in the `app/styles/` folder and save the result the `dist/styles/` folder, 4.
 The media files in the `app/assets/` folder are copied as-is to the `dist/
 assets/` folder. 5. The `dist/` folder now contains a fully functional static
 website.
```

### Comparing `sweb-0.5/setup.py` & `sweb-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sweb',
-    version='0.5',
+    version='0.6',
     packages=find_packages(),
     entry_points={
       'console_scripts': [
         'sweb=sweb.app:main',  # Define the command and point it to the entry function
       ]
     },
     description='SWEB is a static website generator that processes templates, styles, and assets',
```

### Comparing `sweb-0.5/sweb/app.py` & `sweb-0.6/sweb/app.py`

 * *Files identical despite different names*

### Comparing `sweb-0.5/sweb/data_loader.py` & `sweb-0.6/sweb/data_loader.py`

 * *Files identical despite different names*

### Comparing `sweb-0.5/sweb/style_processor.py` & `sweb-0.6/sweb/style_processor.py`

 * *Files identical despite different names*

### Comparing `sweb-0.5/sweb/template_processor.py` & `sweb-0.6/sweb/template_processor.py`

 * *Files identical despite different names*

### Comparing `sweb-0.5/sweb.egg-info/PKG-INFO` & `sweb-0.6/sweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweb
-Version: 0.5
+Version: 0.6
 Summary: SWEB is a static website generator that processes templates, styles, and assets
 Author: Jeremy LECERF
 Author-email: redpist.com@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -189,27 +189,24 @@
 would generate the following CSS file `dist/styles/style.css`:
 ```css
 body h1 {
   color: red;
 }
 ```
 
-
-
-
-## assets
+## Assets
 
 ## Path
 ```
 app/assets/
 ```
 
 ### Purpose
 
-Holds static files like images, fonts, and other media which are copied directly into the output directory without modification. These files are important for the multimedia elements of the site.
+Holds static files like images, fonts, and other media which are copied directly into the output directory without modification.
 
 ### Example
 
 If you have an image `app/assets/logo.png`, it would be copied to `dist/assets/logo.png` without any changes.
 
 
 ## How SWEB works?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweb Version: 0.5 Summary: SWEB is a static website
+Metadata-Version: 2.1 Name: sweb Version: 0.6 Summary: SWEB is a static website
 generator that processes templates, styles, and assets Author: Jeremy LECERF
 Author-email: redpist.com@gmail.com License: MIT Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -54,20 +54,19 @@
 index.html` ```html
 ************ HHeelllloo,, wwoorrlldd ttoo AA sswweebb pprroojjeecctt..!! ************
 ``` ## Styles ### Path ``` app/styles/ ``` ### Purpose Stores CSS & [SASS/SCSS]
 (https://sass-lang.com/) style sheets that control the look and feel of the
 website. These stylesheets are compiled and saved in the `dist/styles/` folder.
 ### Example The following `style.scss` file in the `app/styles/` folder:
 ```scss body { h1 { color: red; } } ``` would generate the following CSS file
-`dist/styles/style.css`: ```css body h1 { color: red; } ``` ## assets ## Path
+`dist/styles/style.css`: ```css body h1 { color: red; } ``` ## Assets ## Path
 ``` app/assets/ ``` ### Purpose Holds static files like images, fonts, and
 other media which are copied directly into the output directory without
-modification. These files are important for the multimedia elements of the
-site. ### Example If you have an image `app/assets/logo.png`, it would be
-copied to `dist/assets/logo.png` without any changes. ## How SWEB works? To
+modification. ### Example If you have an image `app/assets/logo.png`, it would
+be copied to `dist/assets/logo.png` without any changes. ## How SWEB works? To
 generate a website, SWEB: 1. Load the JSON data from the `app/data/` folder, 2.
 Generate the html from the handlebar templates in the `app/templates/` folder
 and save the result in the `dist/` folder, 3. Compile The CSS/SASS/SCSS files
 in the `app/styles/` folder and save the result the `dist/styles/` folder, 4.
 The media files in the `app/assets/` folder are copied as-is to the `dist/
 assets/` folder. 5. The `dist/` folder now contains a fully functional static
 website.
```


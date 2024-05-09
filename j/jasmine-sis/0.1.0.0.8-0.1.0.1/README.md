# Comparing `tmp/jasmine_sis-0.1.0.0.8.tar.gz` & `tmp/jasmine_sis-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jasmine_sis-0.1.0.0.8.tar", last modified: Thu May  9 17:08:49 2024, max compression
+gzip compressed data, was "jasmine_sis-0.1.0.1.tar", last modified: Tue May  7 20:53:46 2024, max compression
```

## Comparing `jasmine_sis-0.1.0.0.8.tar` & `jasmine_sis-0.1.0.1.tar`

### file list

```diff
@@ -1,23 +1,13 @@
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-09 17:08:49.001539 jasmine_sis-0.1.0.0.8/
--rw-r--r--   0 sishitan (344948379) staff       (20)     1065 2024-04-17 18:49:24.000000 jasmine_sis-0.1.0.0.8/LICENSE
--rw-r--r--   0 sishitan (344948379) staff       (20)      497 2024-05-09 17:08:49.000599 jasmine_sis-0.1.0.0.8/PKG-INFO
--rw-r--r--   0 sishitan (344948379) staff       (20)     2178 2024-05-07 21:16:55.000000 jasmine_sis-0.1.0.0.8/README.md
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-09 17:08:48.983595 jasmine_sis-0.1.0.0.8/jasmine/
--rw-r--r--   0 sishitan (344948379) staff       (20)        0 2024-03-22 15:18:25.000000 jasmine_sis-0.1.0.0.8/jasmine/__init__.py
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-09 17:08:48.992599 jasmine_sis-0.1.0.0.8/jasmine/files_organizer/
--rw-r--r--   0 sishitan (344948379) staff       (20)     4531 2024-05-09 17:07:45.000000 jasmine_sis-0.1.0.0.8/jasmine/files_organizer/RTModel_ephemerides_tools.py
--rw-r--r--   0 sishitan (344948379) staff       (20)        0 2024-03-22 15:18:25.000000 jasmine_sis-0.1.0.0.8/jasmine/files_organizer/__init__.py
--rw-r--r--   0 sishitan (344948379) staff       (20)     5001 2024-04-26 17:04:14.000000 jasmine_sis-0.1.0.0.8/jasmine/files_organizer/data_challenge_prep.py
--rw-r--r--   0 sishitan (344948379) staff       (20)     3679 2024-04-26 17:31:20.000000 jasmine_sis-0.1.0.0.8/jasmine/files_organizer/data_challenge_reader.py
--rw-r--r--   0 sishitan (344948379) staff       (20)     3863 2024-05-08 18:06:12.000000 jasmine_sis-0.1.0.0.8/jasmine/files_organizer/data_challenge_to_RTModel.py
--rw-r--r--   0 sishitan (344948379) staff       (20)    15432 2024-05-07 20:44:39.000000 jasmine_sis-0.1.0.0.8/jasmine/files_organizer/lightcurve_cls.py
--rw-r--r--   0 sishitan (344948379) staff       (20)       29 2024-05-09 17:07:46.000000 jasmine_sis-0.1.0.0.8/jasmine/files_organizer/plasticc_files_reader.py
-drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-09 17:08:48.999246 jasmine_sis-0.1.0.0.8/jasmine_sis.egg-info/
--rw-r--r--   0 sishitan (344948379) staff       (20)      497 2024-05-09 17:08:48.000000 jasmine_sis-0.1.0.0.8/jasmine_sis.egg-info/PKG-INFO
--rw-r--r--   0 sishitan (344948379) staff       (20)      583 2024-05-09 17:08:48.000000 jasmine_sis-0.1.0.0.8/jasmine_sis.egg-info/SOURCES.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-09 17:08:48.000000 jasmine_sis-0.1.0.0.8/jasmine_sis.egg-info/dependency_links.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:48:18.000000 jasmine_sis-0.1.0.0.8/jasmine_sis.egg-info/not-zip-safe
--rw-r--r--   0 sishitan (344948379) staff       (20)      111 2024-05-09 17:08:48.000000 jasmine_sis-0.1.0.0.8/jasmine_sis.egg-info/requires.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)        8 2024-05-09 17:08:48.000000 jasmine_sis-0.1.0.0.8/jasmine_sis.egg-info/top_level.txt
--rw-r--r--   0 sishitan (344948379) staff       (20)       38 2024-05-09 17:08:49.001772 jasmine_sis-0.1.0.0.8/setup.cfg
--rw-r--r--   0 sishitan (344948379) staff       (20)      740 2024-05-09 17:08:44.000000 jasmine_sis-0.1.0.0.8/setup.py
+drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 20:53:46.324549 jasmine_sis-0.1.0.1/
+-rw-r--r--   0 sishitan (344948379) staff       (20)     1065 2024-04-17 18:49:24.000000 jasmine_sis-0.1.0.1/LICENSE
+-rw-r--r--   0 sishitan (344948379) staff       (20)      435 2024-05-07 20:53:46.324005 jasmine_sis-0.1.0.1/PKG-INFO
+-rw-r--r--   0 sishitan (344948379) staff       (20)     2077 2024-05-01 23:08:17.000000 jasmine_sis-0.1.0.1/README.md
+drwxr-xr-x   0 sishitan (344948379) staff       (20)        0 2024-05-07 20:53:46.323357 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/
+-rw-r--r--   0 sishitan (344948379) staff       (20)      435 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/PKG-INFO
+-rw-r--r--   0 sishitan (344948379) staff       (20)      234 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/SOURCES.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/dependency_links.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)        1 2024-05-07 20:48:18.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/not-zip-safe
+-rw-r--r--   0 sishitan (344948379) staff       (20)       81 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/requires.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)        8 2024-05-07 20:53:46.000000 jasmine_sis-0.1.0.1/jasmine_sis.egg-info/top_level.txt
+-rw-r--r--   0 sishitan (344948379) staff       (20)       38 2024-05-07 20:53:46.324662 jasmine_sis-0.1.0.1/setup.cfg
+-rw-r--r--   0 sishitan (344948379) staff       (20)      611 2024-05-07 20:53:41.000000 jasmine_sis-0.1.0.1/setup.py
```

### Comparing `jasmine_sis-0.1.0.0.8/LICENSE` & `jasmine_sis-0.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jasmine_sis-0.1.0.0.8/README.md` & `jasmine_sis-0.1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 # jasmine
 JASMINE: **J**oint **A**nalysis of **S**imulation for **M**icrolensing **IN**terested **E**vents
 
 ---
-pip installable as `jasmine-sis`
-```
-pip install jasmine-sis
-```
----
 ## 1. Microlensing Data Challenge Simulations
 
 ### Splitting master file
 1. Make sure you downloaded the `master_file.txt` and `wfirstColumnNumbers.txt`  from the data challenge folder:  
    https://github.com/microlensing-data-challenge/data-challenge-1/tree/master/Answers
-2. Run `python jasmine/files_organizer/data_challenge_prep.py` , changing path as needed. It splits master file and create 4 new files:
+2. Run `python files_organizer/data_challenge_prep.py` , changing path as needed. It splits master file and create 4 new files:
    * binary_star.csv
    * bound_planet.csv
    * cataclysmic_variables.csv
    * single_lens.csv
 ---
 ###  Using the `LightcurveEvent` class:  
 ```
-import jasmine.files_organizer.lightcurve_cls as lc
+import files_organizer.lightcurve_cls as lc
 the_lightcurve = lc.LightcurveEvent(2) # Binary star # Call the lightcurve class
 vars(the_lightcurve).keys() # See what are the available attributes and subclasses
 the_lightcurve.lens # subclass
 lightcurve_datapoints = the_lightcurve.lightcurve_data(filter_='W149', folder_path_='../data') # Get the lightcurve datapoints
 ```
 
 See notebook `analysis/getting_information_about_a_lightcurve.ipynb` for details.
 
 ---
 If you opt to not use a class. You can use the functions below:
 See notebook `analysis/reading_the_data_challenge.ipynb` for more details.
 #### 1. Reading the four master csv files
 Call the function you need, and it returns a pandas dataframe:  
-`import jasmine.files_organizer.data_challenge_reader as dcr`
+`import files_organizer.data_challenge_reader as dcr`
 * `dataframe = dcr.binary_star_master_reader()`  
 * `dataframe = dcr.bound_planet_master_reader()`  
 * `dataframe = dcr.cataclysmic_variables_master_reader()`  
 * `dataframe = dcr.single_lens_master_reader()`  
 
 Obs: The column you are looking for is: `data_challenge_lc_number`.  
 
 #### 2. Reading the light curve data points files
 The function `lightcurve_data_reader` reads the light curve files and returns a pandas dataframe with `BJD`, `Magnitude`, `Error` and `days` (days = BJD - 2450000) ':  
 
 ```
-import jasmine.files_organizer.data_challenge_reader as dcr
+import files_organizer.data_challenge_reader as dcr
 lightcurve_df = dcr.lightcurve_data_reader(data_challenge_lc_number_=5, folder_path_='../data')
 ```
```

### Comparing `jasmine_sis-0.1.0.0.8/setup.py` & `jasmine_sis-0.1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from setuptools import setup
 
 setup(name='jasmine-sis',
-      version='0.1.0.0.8',
+      version='0.1.0.1',
       description='JASMINE: Joint Analysis of Simulations for Microlensing INterest Events',
       url='https://github.com/stelais/jasmine',
       author='Stela IS',
       author_email='stela.ishitanisilva@nasa.gov',
       license='MIT',
-      packages=['jasmine',
-                'jasmine.files_organizer'],
+      packages=['jasmine'],
       zip_safe=False,
       install_requires=["pandas==2.1.4",
                         "jupyter==1.0.0",
                         "notebook==7.1.3",
                         "ipykernel==6.29.4",
-                        "matplotlib==3.8.4",
-                        "astropy==6.1.0",
-                        "jplephem==2.22"
+                        "matplotlib==3.8.4"
                         ])
```


# Comparing `tmp/EmpireStateRunUp-0.0.7.tar.gz` & `tmp/EmpireStateRunUp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmpireStateRunUp-0.0.7.tar", last modified: Tue May  7 01:44:15 2024, max compression
+gzip compressed data, was "EmpireStateRunUp-0.0.8.tar", last modified: Thu May  9 16:28:49 2024, max compression
```

## Comparing `EmpireStateRunUp-0.0.7.tar` & `EmpireStateRunUp-0.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.206233 EmpireStateRunUp-0.0.7/
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.199233 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3255 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/PKG-INFO
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1188 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/SOURCES.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)        1 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/dependency_links.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      396 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/entry_points.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      111 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/requires.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)       29 2024-05-07 01:44:15.000000 EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/top_level.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    20137 2024-01-19 14:51:11.000000 EmpireStateRunUp-0.0.7/LICENSE
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3255 2024-05-07 01:44:15.206233 EmpireStateRunUp-0.0.7/PKG-INFO
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     2724 2024-01-01 17:18:32.000000 EmpireStateRunUp-0.0.7/README.md
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.201233 EmpireStateRunUp-0.0.7/empirestaterunup/
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)        0 2023-10-07 23:44:51.000000 EmpireStateRunUp-0.0.7/empirestaterunup/__init__.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     6194 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.7/empirestaterunup/analyze.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    19172 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.7/empirestaterunup/apps.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      262 2023-10-22 10:20:27.000000 EmpireStateRunUp-0.0.7/empirestaterunup/browser.tcss
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    20759 2023-10-28 14:39:38.000000 EmpireStateRunUp-0.0.7/empirestaterunup/country_codes.csv
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    21505 2024-05-07 01:18:00.000000 EmpireStateRunUp-0.0.7/empirestaterunup/data.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      215 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.7/empirestaterunup/five_numbers.tcss
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      257 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.7/empirestaterunup/outliers.tcss
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    32840 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.7/empirestaterunup/results-first-level-2023.csv
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    97015 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/empirestaterunup/results-full-level-2023.csv
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)       65 2023-10-27 10:47:05.000000 EmpireStateRunUp-0.0.7/empirestaterunup/runner_details.tcss
--rwxr-xr-x   0 josevnz   (1000) josevnz   (1000)     7410 2024-05-07 01:16:59.000000 EmpireStateRunUp-0.0.7/empirestaterunup/runners.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    12292 2024-05-07 01:15:19.000000 EmpireStateRunUp-0.0.7/empirestaterunup/scraper.py
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.205233 EmpireStateRunUp-0.0.7/images/
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    26334 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/age_histogram.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    13114 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/age_plot.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   479274 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/empire_state_runup.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    33396 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esrm_outlier_first_screen.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    45546 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esrm_outlier_runner_detail.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    26093 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_age_box_plot.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   188519 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_browser.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   119343 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_numbers.svg
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    47801 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_outlier-1.svg
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    82044 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/esru_outlier-2.svg
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)    43577 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/gender_distribution.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   122624 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/participants_per_country.png
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)   196079 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/images/race_runners_2023-12-31T18_35_53_558956.svg
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1406 2024-05-07 01:27:29.000000 EmpireStateRunUp-0.0.7/pyproject.toml
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)      110 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.7/requirements.txt
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)       38 2024-05-07 01:44:15.206233 EmpireStateRunUp-0.0.7/setup.cfg
-drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-07 01:44:15.206233 EmpireStateRunUp-0.0.7/test/
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3000 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.7/test/test_analyze.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1239 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/test/test_app.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     6081 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.7/test/test_data.py
--rw-r--r--   0 josevnz   (1000) josevnz   (1000)     2140 2024-05-07 01:15:55.000000 EmpireStateRunUp-0.0.7/test/test_scrapper.py
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-09 16:28:49.354332 EmpireStateRunUp-0.0.8/
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-09 16:28:49.338332 EmpireStateRunUp-0.0.8/EmpireStateRunUp.egg-info/
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3255 2024-05-09 16:28:49.000000 EmpireStateRunUp-0.0.8/EmpireStateRunUp.egg-info/PKG-INFO
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1188 2024-05-09 16:28:49.000000 EmpireStateRunUp-0.0.8/EmpireStateRunUp.egg-info/SOURCES.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)        1 2024-05-09 16:28:49.000000 EmpireStateRunUp-0.0.8/EmpireStateRunUp.egg-info/dependency_links.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      396 2024-05-09 16:28:49.000000 EmpireStateRunUp-0.0.8/EmpireStateRunUp.egg-info/entry_points.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      111 2024-05-09 16:28:49.000000 EmpireStateRunUp-0.0.8/EmpireStateRunUp.egg-info/requires.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)       29 2024-05-09 16:28:49.000000 EmpireStateRunUp-0.0.8/EmpireStateRunUp.egg-info/top_level.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    20137 2024-01-19 14:51:11.000000 EmpireStateRunUp-0.0.8/LICENSE
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3255 2024-05-09 16:28:49.354332 EmpireStateRunUp-0.0.8/PKG-INFO
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     2724 2024-01-01 17:18:32.000000 EmpireStateRunUp-0.0.8/README.md
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-09 16:28:49.342332 EmpireStateRunUp-0.0.8/empirestaterunup/
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)        0 2023-10-07 23:44:51.000000 EmpireStateRunUp-0.0.8/empirestaterunup/__init__.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     6194 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.8/empirestaterunup/analyze.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    19172 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.8/empirestaterunup/apps.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      262 2023-10-22 10:20:27.000000 EmpireStateRunUp-0.0.8/empirestaterunup/browser.tcss
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    20759 2023-10-28 14:39:38.000000 EmpireStateRunUp-0.0.8/empirestaterunup/country_codes.csv
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    21505 2024-05-07 01:18:00.000000 EmpireStateRunUp-0.0.8/empirestaterunup/data.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      215 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.8/empirestaterunup/five_numbers.tcss
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      257 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.8/empirestaterunup/outliers.tcss
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    32840 2023-11-26 23:53:15.000000 EmpireStateRunUp-0.0.8/empirestaterunup/results-first-level-2023.csv
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    97015 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/empirestaterunup/results-full-level-2023.csv
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)       65 2023-10-27 10:47:05.000000 EmpireStateRunUp-0.0.8/empirestaterunup/runner_details.tcss
+-rwxr-xr-x   0 josevnz   (1000) josevnz   (1000)     7410 2024-05-07 01:16:59.000000 EmpireStateRunUp-0.0.8/empirestaterunup/runners.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    12292 2024-05-07 01:15:19.000000 EmpireStateRunUp-0.0.8/empirestaterunup/scraper.py
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-09 16:28:49.352332 EmpireStateRunUp-0.0.8/images/
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    26334 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/age_histogram.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    13114 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/age_plot.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   479274 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/empire_state_runup.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    33396 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/esrm_outlier_first_screen.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    45546 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/esrm_outlier_runner_detail.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    26093 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/esru_age_box_plot.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   188519 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/esru_browser.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   119343 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/esru_numbers.svg
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    47801 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/esru_outlier-1.svg
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    82044 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/esru_outlier-2.svg
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)    43577 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/gender_distribution.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   122624 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/participants_per_country.png
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)   196079 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/images/race_runners_2023-12-31T18_35_53_558956.svg
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1406 2024-05-09 16:28:34.000000 EmpireStateRunUp-0.0.8/pyproject.toml
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)      110 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.8/requirements.txt
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)       38 2024-05-09 16:28:49.354332 EmpireStateRunUp-0.0.8/setup.cfg
+drwxr-xr-x   0 josevnz   (1000) josevnz   (1000)        0 2024-05-09 16:28:49.353332 EmpireStateRunUp-0.0.8/test/
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     3000 2024-03-29 19:46:08.000000 EmpireStateRunUp-0.0.8/test/test_analyze.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     1239 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/test/test_app.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     6081 2024-01-01 17:16:29.000000 EmpireStateRunUp-0.0.8/test/test_data.py
+-rw-r--r--   0 josevnz   (1000) josevnz   (1000)     2140 2024-05-07 01:15:55.000000 EmpireStateRunUp-0.0.8/test/test_scrapper.py
```

### Comparing `EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/PKG-INFO` & `EmpireStateRunUp-0.0.8/EmpireStateRunUp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmpireStateRunUp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Collection of scripts to analyze the results of the 2023 Empire State Run Up race
 Author-email: Jose Vicente Nunez <kodegeek.com@protonmail.com>
 Keywords: running,race
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `EmpireStateRunUp-0.0.7/EmpireStateRunUp.egg-info/SOURCES.txt` & `EmpireStateRunUp-0.0.8/EmpireStateRunUp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/LICENSE` & `EmpireStateRunUp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/PKG-INFO` & `EmpireStateRunUp-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EmpireStateRunUp
-Version: 0.0.7
+Version: 0.0.8
 Summary: Collection of scripts to analyze the results of the 2023 Empire State Run Up race
 Author-email: Jose Vicente Nunez <kodegeek.com@protonmail.com>
 Keywords: running,race
 Classifier: Environment :: Console
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `EmpireStateRunUp-0.0.7/README.md` & `EmpireStateRunUp-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/empirestaterunup/analyze.py` & `EmpireStateRunUp-0.0.8/empirestaterunup/analyze.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/empirestaterunup/apps.py` & `EmpireStateRunUp-0.0.8/empirestaterunup/apps.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/empirestaterunup/country_codes.csv` & `EmpireStateRunUp-0.0.8/empirestaterunup/country_codes.csv`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/empirestaterunup/data.py` & `EmpireStateRunUp-0.0.8/empirestaterunup/data.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/empirestaterunup/results-first-level-2023.csv` & `EmpireStateRunUp-0.0.8/empirestaterunup/results-first-level-2023.csv`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/empirestaterunup/results-full-level-2023.csv` & `EmpireStateRunUp-0.0.8/empirestaterunup/results-full-level-2023.csv`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/empirestaterunup/runners.py` & `EmpireStateRunUp-0.0.8/empirestaterunup/runners.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/empirestaterunup/scraper.py` & `EmpireStateRunUp-0.0.8/empirestaterunup/scraper.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/age_histogram.png` & `EmpireStateRunUp-0.0.8/images/age_histogram.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/age_plot.png` & `EmpireStateRunUp-0.0.8/images/age_plot.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/empire_state_runup.png` & `EmpireStateRunUp-0.0.8/images/empire_state_runup.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/esrm_outlier_first_screen.png` & `EmpireStateRunUp-0.0.8/images/esrm_outlier_first_screen.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/esrm_outlier_runner_detail.png` & `EmpireStateRunUp-0.0.8/images/esrm_outlier_runner_detail.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/esru_age_box_plot.png` & `EmpireStateRunUp-0.0.8/images/esru_age_box_plot.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/esru_browser.png` & `EmpireStateRunUp-0.0.8/images/esru_browser.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/esru_numbers.svg` & `EmpireStateRunUp-0.0.8/images/esru_numbers.svg`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/esru_outlier-1.svg` & `EmpireStateRunUp-0.0.8/images/esru_outlier-1.svg`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/esru_outlier-2.svg` & `EmpireStateRunUp-0.0.8/images/esru_outlier-2.svg`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/gender_distribution.png` & `EmpireStateRunUp-0.0.8/images/gender_distribution.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/participants_per_country.png` & `EmpireStateRunUp-0.0.8/images/participants_per_country.png`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/images/race_runners_2023-12-31T18_35_53_558956.svg` & `EmpireStateRunUp-0.0.8/images/race_runners_2023-12-31T18_35_53_558956.svg`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/pyproject.toml` & `EmpireStateRunUp-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "twine",
     "textual-dev"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EmpireStateRunUp"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     {name = "Jose Vicente Nunez", email = "kodegeek.com@protonmail.com"},
 ]
 description = "Collection of scripts to analyze the results of the 2023 Empire State Run Up race"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["running", "race"]
```

### Comparing `EmpireStateRunUp-0.0.7/test/test_analyze.py` & `EmpireStateRunUp-0.0.8/test/test_analyze.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/test/test_app.py` & `EmpireStateRunUp-0.0.8/test/test_app.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/test/test_data.py` & `EmpireStateRunUp-0.0.8/test/test_data.py`

 * *Files identical despite different names*

### Comparing `EmpireStateRunUp-0.0.7/test/test_scrapper.py` & `EmpireStateRunUp-0.0.8/test/test_scrapper.py`

 * *Files identical despite different names*


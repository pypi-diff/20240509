# Comparing `tmp/Stricture-1.0.5.tar.gz` & `tmp/Stricture-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Stricture-1.0.5.tar", last modified: Thu May  9 03:46:31 2024, max compression
+gzip compressed data, was "Stricture-1.0.6.tar", last modified: Thu May  9 03:55:19 2024, max compression
```

## Comparing `Stricture-1.0.5.tar` & `Stricture-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:46:31.236085 Stricture-1.0.5/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1068 2024-05-08 00:09:54.000000 Stricture-1.0.5/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6054 2024-05-09 03:46:31.236085 Stricture-1.0.5/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)    12021 2024-05-09 03:45:36.000000 Stricture-1.0.5/README.md
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:46:31.236085 Stricture-1.0.5/Stricture.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     6054 2024-05-09 03:46:30.000000 Stricture-1.0.5/Stricture.egg-info/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      411 2024-05-09 03:46:31.000000 Stricture-1.0.5/Stricture.egg-info/SOURCES.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2024-05-09 03:46:30.000000 Stricture-1.0.5/Stricture.egg-info/dependency_links.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       49 2024-05-09 03:46:30.000000 Stricture-1.0.5/Stricture.egg-info/entry_points.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       62 2024-05-09 03:46:30.000000 Stricture-1.0.5/Stricture.egg-info/requires.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       10 2024-05-09 03:46:30.000000 Stricture-1.0.5/Stricture.egg-info/top_level.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2024-05-09 03:46:31.236085 Stricture-1.0.5/setup.cfg
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1157 2024-05-09 03:46:13.000000 Stricture-1.0.5/setup.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:46:31.236085 Stricture-1.0.5/stricture/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      195 2024-05-06 00:40:54.000000 Stricture-1.0.5/stricture/__init__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     6580 2024-05-09 03:18:56.000000 Stricture-1.0.5/stricture/cli.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     5478 2024-05-07 22:26:19.000000 Stricture-1.0.5/stricture/commandstricture.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2554 2024-05-07 08:48:51.000000 Stricture-1.0.5/stricture/exceptions.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     3130 2024-05-07 05:31:31.000000 Stricture-1.0.5/stricture/processstricture.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)    14444 2024-05-07 23:46:17.000000 Stricture-1.0.5/stricture/schedule.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     4217 2024-05-04 22:11:05.000000 Stricture-1.0.5/stricture/sfm.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     7432 2024-05-07 08:48:37.000000 Stricture-1.0.5/stricture/stricture.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:55:19.560249 Stricture-1.0.6/
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     1068 2024-05-08 00:09:54.000000 Stricture-1.0.6/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6055 2024-05-09 03:55:19.560249 Stricture-1.0.6/PKG-INFO
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)    12022 2024-05-09 03:55:01.000000 Stricture-1.0.6/README.md
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:55:19.560249 Stricture-1.0.6/Stricture.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     6055 2024-05-09 03:55:19.000000 Stricture-1.0.6/Stricture.egg-info/PKG-INFO
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)      411 2024-05-09 03:55:19.000000 Stricture-1.0.6/Stricture.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2024-05-09 03:55:19.000000 Stricture-1.0.6/Stricture.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       49 2024-05-09 03:55:19.000000 Stricture-1.0.6/Stricture.egg-info/entry_points.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       62 2024-05-09 03:55:19.000000 Stricture-1.0.6/Stricture.egg-info/requires.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       10 2024-05-09 03:55:19.000000 Stricture-1.0.6/Stricture.egg-info/top_level.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2024-05-09 03:55:19.560249 Stricture-1.0.6/setup.cfg
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     1157 2024-05-09 03:54:44.000000 Stricture-1.0.6/setup.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:55:19.560249 Stricture-1.0.6/stricture/
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)      195 2024-05-06 00:40:54.000000 Stricture-1.0.6/stricture/__init__.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     6580 2024-05-09 03:18:56.000000 Stricture-1.0.6/stricture/cli.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     5478 2024-05-07 22:26:19.000000 Stricture-1.0.6/stricture/commandstricture.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     2554 2024-05-07 08:48:51.000000 Stricture-1.0.6/stricture/exceptions.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     3130 2024-05-07 05:31:31.000000 Stricture-1.0.6/stricture/processstricture.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)    14444 2024-05-07 23:46:17.000000 Stricture-1.0.6/stricture/schedule.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     4217 2024-05-04 22:11:05.000000 Stricture-1.0.6/stricture/sfm.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     7432 2024-05-07 08:48:37.000000 Stricture-1.0.6/stricture/stricture.py
```

### Comparing `Stricture-1.0.5/LICENSE` & `Stricture-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.5/PKG-INFO` & `Stricture-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stricture
-Version: 1.0.5
+Version: 1.0.6
 Summary: Stricture is a python package that provides classes and a CLI tool for easy scheduling, automating, and managing of specific operations.
 Home-page: https://github.com/moorejacob2017/Stricture/
 Author: Jacob Moore
 Author-email: moorejacob2017@gmail.com
 License: MIT
 Keywords: automation task job management date time cron schedule scheduling bash process pid command bash week month
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
     stricture -s my_schedule.yml -c "ping -c 1000 192.168.1.1"
     stricture -s my_schedule.yml -qoe -c "./my_script.sh"
     stricture -s my_schedule.json -p 13019
 ```
 
 
 ## Making a schedule in YAML
-`Schedules` have many different ways to be instantiated and initialized. On of the easiest ways to create a schedule is to import it from a yaml file with `from_yaml_file`. Below is an explaination of how to format a schedule with yaml.
+`Schedules` have many different ways to be instantiated and initialized. One of the easiest ways to create a schedule is to import it from a yaml file with `from_yaml_file`. Below is an explaination of how to format a schedule with yaml.
 ```yaml
 # Days are classified into 1 of 3 modes: restricted, unrestricted, and prohibited.
 #   restricted - Days are considered in schedule, but only for the
 #                time range defined by start_time and stop_time.
 #   unrestricted - All 24 hours of the day are considered in the schedule.
 #   prohibited - All 24 hours of the day are coonsidered out of schedule.
```

### Comparing `Stricture-1.0.5/README.md` & `Stricture-1.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     stricture -s my_schedule.yml -c "ping -c 1000 192.168.1.1"
     stricture -s my_schedule.yml -qoe -c "./my_script.sh"
     stricture -s my_schedule.json -p 13019
 ```
 
 
 ## Making a schedule in YAML
-`Schedules` have many different ways to be instantiated and initialized. On of the easiest ways to create a schedule is to import it from a yaml file with `from_yaml_file`. Below is an explaination of how to format a schedule with yaml.
+`Schedules` have many different ways to be instantiated and initialized. One of the easiest ways to create a schedule is to import it from a yaml file with `from_yaml_file`. Below is an explaination of how to format a schedule with yaml.
 ```yaml
 # Days are classified into 1 of 3 modes: restricted, unrestricted, and prohibited.
 #   restricted - Days are considered in schedule, but only for the
 #                time range defined by start_time and stop_time.
 #   unrestricted - All 24 hours of the day are considered in the schedule.
 #   prohibited - All 24 hours of the day are coonsidered out of schedule.
```

### Comparing `Stricture-1.0.5/Stricture.egg-info/PKG-INFO` & `Stricture-1.0.6/Stricture.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stricture
-Version: 1.0.5
+Version: 1.0.6
 Summary: Stricture is a python package that provides classes and a CLI tool for easy scheduling, automating, and managing of specific operations.
 Home-page: https://github.com/moorejacob2017/Stricture/
 Author: Jacob Moore
 Author-email: moorejacob2017@gmail.com
 License: MIT
 Keywords: automation task job management date time cron schedule scheduling bash process pid command bash week month
 Classifier: License :: OSI Approved :: MIT License
@@ -58,15 +58,15 @@
     stricture -s my_schedule.yml -c "ping -c 1000 192.168.1.1"
     stricture -s my_schedule.yml -qoe -c "./my_script.sh"
     stricture -s my_schedule.json -p 13019
 ```
 
 
 ## Making a schedule in YAML
-`Schedules` have many different ways to be instantiated and initialized. On of the easiest ways to create a schedule is to import it from a yaml file with `from_yaml_file`. Below is an explaination of how to format a schedule with yaml.
+`Schedules` have many different ways to be instantiated and initialized. One of the easiest ways to create a schedule is to import it from a yaml file with `from_yaml_file`. Below is an explaination of how to format a schedule with yaml.
 ```yaml
 # Days are classified into 1 of 3 modes: restricted, unrestricted, and prohibited.
 #   restricted - Days are considered in schedule, but only for the
 #                time range defined by start_time and stop_time.
 #   unrestricted - All 24 hours of the day are considered in the schedule.
 #   prohibited - All 24 hours of the day are coonsidered out of schedule.
```

### Comparing `Stricture-1.0.5/setup.py` & `Stricture-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='Stricture',
-    version='1.0.5',
+    version='1.0.6',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'stricture=stricture.cli:main'
         ]
     },
     install_requires=[
```

### Comparing `Stricture-1.0.5/stricture/cli.py` & `Stricture-1.0.6/stricture/cli.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.5/stricture/commandstricture.py` & `Stricture-1.0.6/stricture/commandstricture.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.5/stricture/exceptions.py` & `Stricture-1.0.6/stricture/exceptions.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.5/stricture/processstricture.py` & `Stricture-1.0.6/stricture/processstricture.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.5/stricture/schedule.py` & `Stricture-1.0.6/stricture/schedule.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.5/stricture/sfm.py` & `Stricture-1.0.6/stricture/sfm.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.5/stricture/stricture.py` & `Stricture-1.0.6/stricture/stricture.py`

 * *Files identical despite different names*


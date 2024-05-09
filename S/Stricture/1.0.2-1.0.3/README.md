# Comparing `tmp/Stricture-1.0.2.tar.gz` & `tmp/Stricture-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Stricture-1.0.2.tar", last modified: Thu May  9 03:22:37 2024, max compression
+gzip compressed data, was "Stricture-1.0.3.tar", last modified: Thu May  9 03:29:56 2024, max compression
```

## Comparing `Stricture-1.0.2.tar` & `Stricture-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:22:37.620712 Stricture-1.0.2/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1068 2024-05-08 00:09:54.000000 Stricture-1.0.2/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5801 2024-05-09 03:22:37.620712 Stricture-1.0.2/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)    11771 2024-05-09 03:20:49.000000 Stricture-1.0.2/README.md
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:22:37.616712 Stricture-1.0.2/Stricture.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     5801 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      411 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/SOURCES.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/dependency_links.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       49 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/entry_points.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       62 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/requires.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       10 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/top_level.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2024-05-09 03:22:37.620712 Stricture-1.0.2/setup.cfg
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1157 2024-05-09 03:21:35.000000 Stricture-1.0.2/setup.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:22:37.620712 Stricture-1.0.2/stricture/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      195 2024-05-06 00:40:54.000000 Stricture-1.0.2/stricture/__init__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     6580 2024-05-09 03:18:56.000000 Stricture-1.0.2/stricture/cli.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     5478 2024-05-07 22:26:19.000000 Stricture-1.0.2/stricture/commandstricture.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2554 2024-05-07 08:48:51.000000 Stricture-1.0.2/stricture/exceptions.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     3130 2024-05-07 05:31:31.000000 Stricture-1.0.2/stricture/processstricture.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)    14444 2024-05-07 23:46:17.000000 Stricture-1.0.2/stricture/schedule.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     4217 2024-05-04 22:11:05.000000 Stricture-1.0.2/stricture/sfm.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     7432 2024-05-07 08:48:37.000000 Stricture-1.0.2/stricture/stricture.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:29:56.300150 Stricture-1.0.3/
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     1068 2024-05-08 00:09:54.000000 Stricture-1.0.3/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5910 2024-05-09 03:29:56.300150 Stricture-1.0.3/PKG-INFO
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)    11771 2024-05-09 03:20:49.000000 Stricture-1.0.3/README.md
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:29:56.296150 Stricture-1.0.3/Stricture.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5910 2024-05-09 03:29:56.000000 Stricture-1.0.3/Stricture.egg-info/PKG-INFO
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)      411 2024-05-09 03:29:56.000000 Stricture-1.0.3/Stricture.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2024-05-09 03:29:56.000000 Stricture-1.0.3/Stricture.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       49 2024-05-09 03:29:56.000000 Stricture-1.0.3/Stricture.egg-info/entry_points.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       62 2024-05-09 03:29:56.000000 Stricture-1.0.3/Stricture.egg-info/requires.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       10 2024-05-09 03:29:56.000000 Stricture-1.0.3/Stricture.egg-info/top_level.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2024-05-09 03:29:56.300150 Stricture-1.0.3/setup.cfg
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     1157 2024-05-09 03:29:47.000000 Stricture-1.0.3/setup.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:29:56.300150 Stricture-1.0.3/stricture/
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)      195 2024-05-06 00:40:54.000000 Stricture-1.0.3/stricture/__init__.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     6580 2024-05-09 03:18:56.000000 Stricture-1.0.3/stricture/cli.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     5478 2024-05-07 22:26:19.000000 Stricture-1.0.3/stricture/commandstricture.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     2554 2024-05-07 08:48:51.000000 Stricture-1.0.3/stricture/exceptions.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     3130 2024-05-07 05:31:31.000000 Stricture-1.0.3/stricture/processstricture.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)    14444 2024-05-07 23:46:17.000000 Stricture-1.0.3/stricture/schedule.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     4217 2024-05-04 22:11:05.000000 Stricture-1.0.3/stricture/sfm.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     7432 2024-05-07 08:48:37.000000 Stricture-1.0.3/stricture/stricture.py
```

### Comparing `Stricture-1.0.2/LICENSE` & `Stricture-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.2/PKG-INFO` & `Stricture-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stricture
-Version: 1.0.2
+Version: 1.0.3
 Summary: Stricture is a python package that provides classes and a CLI tool for easy scheduling, automating, and managing of specific operations.
 Home-page: https://github.com/moorejacob2017/Stricture/
 Author: Jacob Moore
 Author-email: moorejacob2017@gmail.com
 License: MIT
 Keywords: automation task job management date time cron schedule scheduling bash process pid command bash week month
 Classifier: License :: OSI Approved :: MIT License
@@ -33,76 +33,76 @@
 
 Please review the [Stricture Documentation](https://github.com/moorejacob2017/Stricture/) for more information.
 
 
 ## Making a schedule in YAML
 `Schedules` have many different ways to be instantiated and initialized. On of the easiest ways to create a schedule is to import it from a yaml file with `from_yaml_file`. Below is an explaination of how to format a schedule with yaml.
 ```yaml
-# Days are classified into 1 of 3 modes: restricted, unrestricted, and prohibited
+# Days are classified into 1 of 3 modes: restricted, unrestricted, and prohibited.
 #   restricted - Days are considered in schedule, but only for the
-#                time range defined by start_time and stop_time
-#   unrestricted - All 24 hours of the day are considered in the schedule
-#   prohibited - All 24 hours of the day are coonsidered out of schedule
+#                time range defined by start_time and stop_time.
+#   unrestricted - All 24 hours of the day are considered in the schedule.
+#   prohibited - All 24 hours of the day are coonsidered out of schedule.
 
 # assume:
-#   The mode to use for days of the week that are not listed in the schedule
-#   Can either be unrestricted, restricted, or prohibited
-#   Defaults to restricted when not set
+#   The mode to use for days of the week that are not listed in the schedule.
+#   Can either be unrestricted, restricted, or prohibited.
+#   Defaults to restricted when not set.
 assume: "restricted"
 
 # timezone:
-#   The timezone to use when checking the schedule
-#   Uses pytz timezones (Olson Timezone IDs)
-#   Defaults to the system time when not set
+#   The timezone to use when checking the schedule.
+#   Uses pytz timezones (Olson Timezone IDs).
+#   Defaults to the system timezone when not set.
 timezone: "US/Central"
 
 # start_time:
-#   Defines what time the schedule range starts every day
-#   24-Hour Format
-#   Defaults to 00:00 when not set
+#   Defines what time the schedule range starts for every restricted day.
+#   Uses 24-Hour Format.
+#   Defaults to 00:00 when not set.
 start_time: "09:30"
 
 # stop_time:
-#   Defines what time the schedule range stops every day
-#   24-Hour Format
-#   Defaults to 00:00 when not set
+#   Defines what time the schedule range stops for every restricted day.
+#   Uses 24-Hour Format.
+#   Defaults to 00:00 when not set.
 stop_time: "17:00"
 
 # restricted_days:
-#   A list of days of the week that should 
-#   have the start_time and stop_time applied to
+#   A list of days of the week that should
+#   have the start_time and stop_time applied to.
 restricted_days:
   - "Monday"
   - "Tuesday"
   - "Wednesday"
   - "Thursday"
   - "Friday"
 
 # unrestricted_days:
 #   A list of days of the week that should 
-#   have all 24 hours considered as in the schedule
+#   have all 24 hours considered as in the schedule.
 unrestricted_days:
   - "Saturday"
 
 # prohibited_days:
 #   A list of days of the week that should 
-#   have all 24 hours considered as out of the schedule
+#   have all 24 hours considered as out of the schedule.
 prohibited_days:
   - "Sunday"
 
 # specific_dates:
 #   A list of specific date ranges that overides the main
-#   start_time, stop_time, and mode
+#   start_time, stop_time, and mode.
 #   Useful for special occasions or for more granular
-#   control
-#       mode - The mode to use for the range
-#       start_date - The start of the date range
-#       stop_date - The end of the date range (inclusively)
-#       start_time - The start_time to use when the mode for the range is restricted
-#       stop_time - The stop_time to use when the mode for the range is restricted
+#   control.
+#       mode - The mode to use for the range.
+#       start_date - The start of the date range (YYYY-MM-DD format).
+#       stop_date - The end of the date range (inclusively) (YYYY-MM-DD format).
+#       start_time - The start_time to use when the mode for the range is restricted.
+#       stop_time - The stop_time to use when the mode for the range is restricted.
 specific_dates:
   - mode: "unrestricted"
     start_date: "2024-12-12"
     stop_date: "2024-12-23"
   - mode: "prohibited"
     start_date: "2024-12-24"
     stop_date: "2024-12-26"
```

### Comparing `Stricture-1.0.2/README.md` & `Stricture-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.2/Stricture.egg-info/PKG-INFO` & `Stricture-1.0.3/Stricture.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Stricture
-Version: 1.0.2
+Version: 1.0.3
 Summary: Stricture is a python package that provides classes and a CLI tool for easy scheduling, automating, and managing of specific operations.
 Home-page: https://github.com/moorejacob2017/Stricture/
 Author: Jacob Moore
 Author-email: moorejacob2017@gmail.com
 License: MIT
 Keywords: automation task job management date time cron schedule scheduling bash process pid command bash week month
 Classifier: License :: OSI Approved :: MIT License
@@ -33,76 +33,76 @@
 
 Please review the [Stricture Documentation](https://github.com/moorejacob2017/Stricture/) for more information.
 
 
 ## Making a schedule in YAML
 `Schedules` have many different ways to be instantiated and initialized. On of the easiest ways to create a schedule is to import it from a yaml file with `from_yaml_file`. Below is an explaination of how to format a schedule with yaml.
 ```yaml
-# Days are classified into 1 of 3 modes: restricted, unrestricted, and prohibited
+# Days are classified into 1 of 3 modes: restricted, unrestricted, and prohibited.
 #   restricted - Days are considered in schedule, but only for the
-#                time range defined by start_time and stop_time
-#   unrestricted - All 24 hours of the day are considered in the schedule
-#   prohibited - All 24 hours of the day are coonsidered out of schedule
+#                time range defined by start_time and stop_time.
+#   unrestricted - All 24 hours of the day are considered in the schedule.
+#   prohibited - All 24 hours of the day are coonsidered out of schedule.
 
 # assume:
-#   The mode to use for days of the week that are not listed in the schedule
-#   Can either be unrestricted, restricted, or prohibited
-#   Defaults to restricted when not set
+#   The mode to use for days of the week that are not listed in the schedule.
+#   Can either be unrestricted, restricted, or prohibited.
+#   Defaults to restricted when not set.
 assume: "restricted"
 
 # timezone:
-#   The timezone to use when checking the schedule
-#   Uses pytz timezones (Olson Timezone IDs)
-#   Defaults to the system time when not set
+#   The timezone to use when checking the schedule.
+#   Uses pytz timezones (Olson Timezone IDs).
+#   Defaults to the system timezone when not set.
 timezone: "US/Central"
 
 # start_time:
-#   Defines what time the schedule range starts every day
-#   24-Hour Format
-#   Defaults to 00:00 when not set
+#   Defines what time the schedule range starts for every restricted day.
+#   Uses 24-Hour Format.
+#   Defaults to 00:00 when not set.
 start_time: "09:30"
 
 # stop_time:
-#   Defines what time the schedule range stops every day
-#   24-Hour Format
-#   Defaults to 00:00 when not set
+#   Defines what time the schedule range stops for every restricted day.
+#   Uses 24-Hour Format.
+#   Defaults to 00:00 when not set.
 stop_time: "17:00"
 
 # restricted_days:
-#   A list of days of the week that should 
-#   have the start_time and stop_time applied to
+#   A list of days of the week that should
+#   have the start_time and stop_time applied to.
 restricted_days:
   - "Monday"
   - "Tuesday"
   - "Wednesday"
   - "Thursday"
   - "Friday"
 
 # unrestricted_days:
 #   A list of days of the week that should 
-#   have all 24 hours considered as in the schedule
+#   have all 24 hours considered as in the schedule.
 unrestricted_days:
   - "Saturday"
 
 # prohibited_days:
 #   A list of days of the week that should 
-#   have all 24 hours considered as out of the schedule
+#   have all 24 hours considered as out of the schedule.
 prohibited_days:
   - "Sunday"
 
 # specific_dates:
 #   A list of specific date ranges that overides the main
-#   start_time, stop_time, and mode
+#   start_time, stop_time, and mode.
 #   Useful for special occasions or for more granular
-#   control
-#       mode - The mode to use for the range
-#       start_date - The start of the date range
-#       stop_date - The end of the date range (inclusively)
-#       start_time - The start_time to use when the mode for the range is restricted
-#       stop_time - The stop_time to use when the mode for the range is restricted
+#   control.
+#       mode - The mode to use for the range.
+#       start_date - The start of the date range (YYYY-MM-DD format).
+#       stop_date - The end of the date range (inclusively) (YYYY-MM-DD format).
+#       start_time - The start_time to use when the mode for the range is restricted.
+#       stop_time - The stop_time to use when the mode for the range is restricted.
 specific_dates:
   - mode: "unrestricted"
     start_date: "2024-12-12"
     stop_date: "2024-12-23"
   - mode: "prohibited"
     start_date: "2024-12-24"
     stop_date: "2024-12-26"
```

### Comparing `Stricture-1.0.2/setup.py` & `Stricture-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='Stricture',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'stricture=stricture.cli:main'
         ]
     },
     install_requires=[
```

### Comparing `Stricture-1.0.2/stricture/cli.py` & `Stricture-1.0.3/stricture/cli.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.2/stricture/commandstricture.py` & `Stricture-1.0.3/stricture/commandstricture.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.2/stricture/exceptions.py` & `Stricture-1.0.3/stricture/exceptions.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.2/stricture/processstricture.py` & `Stricture-1.0.3/stricture/processstricture.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.2/stricture/schedule.py` & `Stricture-1.0.3/stricture/schedule.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.2/stricture/sfm.py` & `Stricture-1.0.3/stricture/sfm.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.2/stricture/stricture.py` & `Stricture-1.0.3/stricture/stricture.py`

 * *Files identical despite different names*

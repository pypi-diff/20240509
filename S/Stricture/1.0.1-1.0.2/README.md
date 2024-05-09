# Comparing `tmp/Stricture-1.0.1.tar.gz` & `tmp/Stricture-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Stricture-1.0.1.tar", last modified: Wed May  8 00:27:38 2024, max compression
+gzip compressed data, was "Stricture-1.0.2.tar", last modified: Thu May  9 03:22:37 2024, max compression
```

## Comparing `Stricture-1.0.1.tar` & `Stricture-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-08 00:27:37.997052 Stricture-1.0.1/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1068 2024-05-08 00:09:54.000000 Stricture-1.0.1/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2136 2024-05-08 00:27:37.997052 Stricture-1.0.1/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     8074 2024-05-08 00:17:51.000000 Stricture-1.0.1/README.md
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-08 00:27:37.997052 Stricture-1.0.1/Stricture.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2136 2024-05-08 00:27:37.000000 Stricture-1.0.1/Stricture.egg-info/PKG-INFO
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      411 2024-05-08 00:27:37.000000 Stricture-1.0.1/Stricture.egg-info/SOURCES.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2024-05-08 00:27:37.000000 Stricture-1.0.1/Stricture.egg-info/dependency_links.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       49 2024-05-08 00:27:37.000000 Stricture-1.0.1/Stricture.egg-info/entry_points.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       62 2024-05-08 00:27:37.000000 Stricture-1.0.1/Stricture.egg-info/requires.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       10 2024-05-08 00:27:37.000000 Stricture-1.0.1/Stricture.egg-info/top_level.txt
--rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2024-05-08 00:27:37.997052 Stricture-1.0.1/setup.cfg
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     1154 2024-05-08 00:27:13.000000 Stricture-1.0.1/setup.py
-drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-08 00:27:37.997052 Stricture-1.0.1/stricture/
--rw-rw-r--   0 jacob     (1000) jacob     (1000)      195 2024-05-06 00:40:54.000000 Stricture-1.0.1/stricture/__init__.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     5014 2024-05-07 02:13:58.000000 Stricture-1.0.1/stricture/cli.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     5478 2024-05-07 22:26:19.000000 Stricture-1.0.1/stricture/commandstricture.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     2554 2024-05-07 08:48:51.000000 Stricture-1.0.1/stricture/exceptions.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     3130 2024-05-07 05:31:31.000000 Stricture-1.0.1/stricture/processstricture.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)    14444 2024-05-07 23:46:17.000000 Stricture-1.0.1/stricture/schedule.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     4217 2024-05-04 22:11:05.000000 Stricture-1.0.1/stricture/sfm.py
--rw-rw-r--   0 jacob     (1000) jacob     (1000)     7432 2024-05-07 08:48:37.000000 Stricture-1.0.1/stricture/stricture.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:22:37.620712 Stricture-1.0.2/
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     1068 2024-05-08 00:09:54.000000 Stricture-1.0.2/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5801 2024-05-09 03:22:37.620712 Stricture-1.0.2/PKG-INFO
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)    11771 2024-05-09 03:20:49.000000 Stricture-1.0.2/README.md
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:22:37.616712 Stricture-1.0.2/Stricture.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     5801 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/PKG-INFO
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)      411 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)        1 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       49 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/entry_points.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       62 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/requires.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       10 2024-05-09 03:22:37.000000 Stricture-1.0.2/Stricture.egg-info/top_level.txt
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)       38 2024-05-09 03:22:37.620712 Stricture-1.0.2/setup.cfg
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     1157 2024-05-09 03:21:35.000000 Stricture-1.0.2/setup.py
+drwxrwxr-x   0 jacob     (1000) jacob     (1000)        0 2024-05-09 03:22:37.620712 Stricture-1.0.2/stricture/
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)      195 2024-05-06 00:40:54.000000 Stricture-1.0.2/stricture/__init__.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     6580 2024-05-09 03:18:56.000000 Stricture-1.0.2/stricture/cli.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     5478 2024-05-07 22:26:19.000000 Stricture-1.0.2/stricture/commandstricture.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     2554 2024-05-07 08:48:51.000000 Stricture-1.0.2/stricture/exceptions.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     3130 2024-05-07 05:31:31.000000 Stricture-1.0.2/stricture/processstricture.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)    14444 2024-05-07 23:46:17.000000 Stricture-1.0.2/stricture/schedule.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     4217 2024-05-04 22:11:05.000000 Stricture-1.0.2/stricture/sfm.py
+-rw-rw-r--   0 jacob     (1000) jacob     (1000)     7432 2024-05-07 08:48:37.000000 Stricture-1.0.2/stricture/stricture.py
```

### Comparing `Stricture-1.0.1/LICENSE` & `Stricture-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.1/setup.py` & `Stricture-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='Stricture',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'stricture=stricture.cli:main'
         ]
     },
     install_requires=[
@@ -18,15 +18,15 @@
         'psutil',
         'pytz',
         'PyYAML',
         'freezegun'
     ],
     author='Jacob Moore',
     author_email='moorejacob2017@gmail.com',
-    description='Stricture is a python package that provides classes and a CLI tool for easy scheduling, automating, and managing specific operations.',
+    description='Stricture is a python package that provides classes and a CLI tool for easy scheduling, automating, and managing of specific operations.',
     long_description=open('description.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/moorejacob2017/Stricture/',
     license='MIT',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `Stricture-1.0.1/stricture/cli.py` & `Stricture-1.0.2/stricture/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -35,53 +35,97 @@
         raise FileNotFoundError(f"File '{file_path}' not found.")
     except json.JSONDecodeError as exc:
         raise ValueError(f"Error loading JSON from file '{file_path}': {exc}")
 
 def main():
     description = "Apply a stricture to a command or process to execute based on a given schedule."
     example_text = '''
-WARNING: Commands passed in with --command run at the speed of python, which is SLOW.
-         Running a command normally, then applying a stricture using the PID with --pid keeps
-         the command from running slowly.
     
 Examples:
     %(prog)s -s my_schedule.yml -c "ping -c 1000 192.168.1.1"
     %(prog)s -s my_schedule.yml -qoe -c "./my_script.sh"
     %(prog)s -s my_schedule.json -p 13019
 
-Example schedule format (see "Schedule" docs):
+Making a schedule in YAML format:
 =======[YAML]========
+# Days are classified into 1 of 3 modes: restricted, unrestricted, and prohibited
+#   restricted - Days are considered in schedule, but only for the
+#                time range defined by start_time and stop_time
+#   unrestricted - All 24 hours of the day are considered in the schedule
+#   prohibited - All 24 hours of the day are coonsidered out of schedule
+
+# assume:
+#   The mode to use for days of the week that are not listed in the schedule
+#   Can either be unrestricted, restricted, or prohibited
+#   Defaults to restricted when not set
 assume: "restricted"
+
+# timezone:
+#   The timezone to use when checking the schedule
+#   Uses pytz timezones (Olson Timezone IDs)
+#   Defaults to the system time when not set
 timezone: "US/Central"
+
+# start_time:
+#   Defines what time the schedule range starts every day
+#   24-Hour Format
+#   Defaults to 00:00 when not set
 start_time: "09:30"
+
+# stop_time:
+#   Defines what time the schedule range stops every day
+#   24-Hour Format
+#   Defaults to 00:00 when not set
 stop_time: "17:00"
+
+# restricted_days:
+#   A list of days of the week that should 
+#   have the start_time and stop_time applied to
 restricted_days:
   - "Monday"
   - "Tuesday"
   - "Wednesday"
   - "Thursday"
   - "Friday"
+
+# unrestricted_days:
+#   A list of days of the week that should 
+#   have all 24 hours considered as in the schedule
 unrestricted_days:
-  - "Saturday"  
+  - "Saturday"
+
+# prohibited_days:
+#   A list of days of the week that should 
+#   have all 24 hours considered as out of the schedule
 prohibited_days:
   - "Sunday"
+
+# specific_dates:
+#   A list of specific date ranges that overides the main
+#   start_time, stop_time, and mode
+#   Useful for special occasions or for more granular
+#   control
+#       mode - The mode to use for the range
+#       start_date - The start of the date range
+#       stop_date - The end of the date range (inclusively)
+#       start_time - The start_time to use when the mode for the range is restricted
+#       stop_time - The stop_time to use when the mode for the range is restricted
 specific_dates:
   - mode: "unrestricted"
     start_date: "2024-12-12"
     stop_date: "2024-12-23"
   - mode: "prohibited"
     start_date: "2024-12-24"
     stop_date: "2024-12-26"
   - mode: "restricted"
     start_date: "2024-12-27"
     stop_date: "2024-12-31"
     start_time: "18:00"
     stop_time: "08:30"
-=====================
-
+=======[YAML]========
 '''
 
     parser = argparse.ArgumentParser(
         description=description,
         epilog=example_text,
         formatter_class=argparse.RawDescriptionHelpFormatter
     )
```

### Comparing `Stricture-1.0.1/stricture/commandstricture.py` & `Stricture-1.0.2/stricture/commandstricture.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.1/stricture/exceptions.py` & `Stricture-1.0.2/stricture/exceptions.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.1/stricture/processstricture.py` & `Stricture-1.0.2/stricture/processstricture.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.1/stricture/schedule.py` & `Stricture-1.0.2/stricture/schedule.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.1/stricture/sfm.py` & `Stricture-1.0.2/stricture/sfm.py`

 * *Files identical despite different names*

### Comparing `Stricture-1.0.1/stricture/stricture.py` & `Stricture-1.0.2/stricture/stricture.py`

 * *Files identical despite different names*


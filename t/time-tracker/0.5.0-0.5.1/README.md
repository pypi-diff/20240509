# Comparing `tmp/time_tracker-0.5.0.tar.gz` & `tmp/time_tracker-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_tracker-0.5.0.tar", max compression
+gzip compressed data, was "time_tracker-0.5.1.tar", max compression
```

## Comparing `time_tracker-0.5.0.tar` & `time_tracker-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-04-22 08:00:59.639340 time_tracker-0.5.0/LICENSE
--rw-r--r--   0        0        0     1256 2024-04-22 08:00:59.639414 time_tracker-0.5.0/README.md
--rw-r--r--   0        0        0      638 2024-04-23 13:47:29.317816 time_tracker-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 08:00:59.640182 time_tracker-0.5.0/time_tracker/__init__.py
--rw-r--r--   0        0        0     2829 2024-04-23 13:42:43.505217 time_tracker-0.5.0/time_tracker/log.py
--rw-r--r--   0        0        0     5227 2024-04-23 13:41:50.606441 time_tracker-0.5.0/time_tracker/main.py
--rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 time_tracker-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-22 08:00:59.639340 time_tracker-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1256 2024-04-22 08:00:59.639414 time_tracker-0.5.1/README.md
+-rw-r--r--   0        0        0      638 2024-05-09 09:58:23.447090 time_tracker-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-22 08:00:59.640182 time_tracker-0.5.1/time_tracker/__init__.py
+-rw-r--r--   0        0        0     2831 2024-05-09 09:57:44.099761 time_tracker-0.5.1/time_tracker/log.py
+-rw-r--r--   0        0        0     5227 2024-04-23 13:41:50.606441 time_tracker-0.5.1/time_tracker/main.py
+-rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 time_tracker-0.5.1/PKG-INFO
```

### Comparing `time_tracker-0.5.0/LICENSE` & `time_tracker-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `time_tracker-0.5.0/README.md` & `time_tracker-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `time_tracker-0.5.0/pyproject.toml` & `time_tracker-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "time-tracker"
-version = "0.5.0"
+version = "0.5.1"
 description = "CLI to track time spent on tasks using pomodoro technique"
 authors = ["Jose Cabeda <jecabeda@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 tt = "time_tracker.main:app"
```

### Comparing `time_tracker-0.5.0/time_tracker/log.py` & `time_tracker-0.5.1/time_tracker/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dotenv import load_dotenv
 
 
 class Logger:
     def __init__(self):
         # Load envs
         load_dotenv()
-        self.apply_configs()
+        # self.apply_configs()
 
     def apply_configs(
         self, format: str = "%(asctime)-10s | %(levelname)s | %(message)s"
     ):
         self.log_folder = Path(os.getenv("TT_LOG_FOLDER", "."))
 
         self.log_file = self.log_folder / f"{(datetime.today()).strftime('%Y%m%d')}.log"
```

### Comparing `time_tracker-0.5.0/time_tracker/main.py` & `time_tracker-0.5.1/time_tracker/main.py`

 * *Files identical despite different names*

### Comparing `time_tracker-0.5.0/PKG-INFO` & `time_tracker-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-tracker
-Version: 0.5.0
+Version: 0.5.1
 Summary: CLI to track time spent on tasks using pomodoro technique
 Author: Jose Cabeda
 Author-email: jecabeda@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```


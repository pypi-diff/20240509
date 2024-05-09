# Comparing `tmp/realtime_operator-0.2.7.tar.gz` & `tmp/realtime_operator-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "realtime_operator-0.2.7.tar", last modified: Wed May  8 13:09:23 2024, max compression
+gzip compressed data, was "realtime_operator-0.2.8.tar", last modified: Wed May  8 16:46:28 2024, max compression
```

## Comparing `realtime_operator-0.2.7.tar` & `realtime_operator-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:09:23.814570 realtime_operator-0.2.7/
--rw-rw-rw-   0        0        0     1094 2024-04-26 14:12:08.000000 realtime_operator-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     4367 2024-05-08 13:09:23.812181 realtime_operator-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     3616 2024-04-26 14:12:08.000000 realtime_operator-0.2.7/README.md
--rw-rw-rw-   0        0        0      695 2024-05-08 13:05:19.000000 realtime_operator-0.2.7/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-08 13:09:23.744767 realtime_operator-0.2.7/realtime_operator/
--rw-rw-rw-   0        0        0        0 2024-04-26 14:12:08.000000 realtime_operator-0.2.7/realtime_operator/__init__.py
--rw-rw-rw-   0        0        0    13467 2024-05-08 13:04:57.000000 realtime_operator-0.2.7/realtime_operator/compression.py
--rw-rw-rw-   0        0        0    22844 2024-04-26 17:25:51.000000 realtime_operator-0.2.7/realtime_operator/single_operator.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:09:23.810939 realtime_operator-0.2.7/realtime_operator.egg-info/
--rw-rw-rw-   0        0        0     4367 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-08 13:09:23.000000 realtime_operator-0.2.7/realtime_operator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 13:09:23.814570 realtime_operator-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      371 2024-04-26 14:12:08.000000 realtime_operator-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:09:23.808457 realtime_operator-0.2.7/tests/
--rw-rw-rw-   0        0        0     2805 2024-04-28 19:15:16.000000 realtime_operator-0.2.7/tests/test_compression.py
--rw-rw-rw-   0        0        0     6277 2024-04-26 17:21:44.000000 realtime_operator-0.2.7/tests/test_single_operator.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:46:28.685886 realtime_operator-0.2.8/
+-rw-rw-rw-   0        0        0     1094 2024-04-26 14:12:08.000000 realtime_operator-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     4367 2024-05-08 16:46:28.685886 realtime_operator-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3616 2024-04-26 14:12:08.000000 realtime_operator-0.2.8/README.md
+-rw-rw-rw-   0        0        0      695 2024-05-08 16:46:10.000000 realtime_operator-0.2.8/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-08 16:46:28.652404 realtime_operator-0.2.8/realtime_operator/
+-rw-rw-rw-   0        0        0        0 2024-04-26 14:12:08.000000 realtime_operator-0.2.8/realtime_operator/__init__.py
+-rw-rw-rw-   0        0        0    14566 2024-05-08 16:45:55.000000 realtime_operator-0.2.8/realtime_operator/compression.py
+-rw-rw-rw-   0        0        0    22844 2024-04-26 17:25:51.000000 realtime_operator-0.2.8/realtime_operator/single_operator.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:46:28.681461 realtime_operator-0.2.8/realtime_operator.egg-info/
+-rw-rw-rw-   0        0        0     4367 2024-05-08 16:46:28.000000 realtime_operator-0.2.8/realtime_operator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2024-05-08 16:46:28.000000 realtime_operator-0.2.8/realtime_operator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 16:46:28.000000 realtime_operator-0.2.8/realtime_operator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-08 16:46:28.000000 realtime_operator-0.2.8/realtime_operator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-08 16:46:28.000000 realtime_operator-0.2.8/realtime_operator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 16:46:28.685886 realtime_operator-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      371 2024-04-26 14:12:08.000000 realtime_operator-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 16:46:28.681461 realtime_operator-0.2.8/tests/
+-rw-rw-rw-   0        0        0     2805 2024-04-28 19:15:16.000000 realtime_operator-0.2.8/tests/test_compression.py
+-rw-rw-rw-   0        0        0     6277 2024-04-26 17:21:44.000000 realtime_operator-0.2.8/tests/test_single_operator.py
```

### Comparing `realtime_operator-0.2.7/LICENSE` & `realtime_operator-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.7/PKG-INFO` & `realtime_operator-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `realtime_operator-0.2.7/README.md` & `realtime_operator-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.7/pyproject.toml` & `realtime_operator-0.2.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "realtime_operator"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="Ernst Holger Amort", email="holgeramort@gmail.com" },
 ]
 description = "A package to perfom real-time operations on time seriesdata streams."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `realtime_operator-0.2.7/realtime_operator/compression.py` & `realtime_operator-0.2.8/realtime_operator/compression.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,14 +126,23 @@
             np.array([z], dtype=np.float64),
             np.array([0], dtype=np.float64),
         )
     deviation_condition = abs(z - state[1]) >= EPSILON
     min_duration_condition = (t - state[0]) >= min_duration_seconds
     max_duration_condition = (t - state[0]) >= max_duration_seconds
 
+    # ooo condition
+    out_of_order = t <= state[0]
+    if out_of_order:
+        return (
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+        )
+
     state[2] += 1
     if (deviation_condition and min_duration_condition) or max_duration_condition:
         state[0] = t
         state[1] = z
         count = state[2]
         state[2] = 0
         return (
@@ -169,14 +178,22 @@
         state[2] = 0
         return (
             np.array([t], dtype=np.float64),
             np.array([z], dtype=np.float64),
             np.array([0], dtype=np.float64),
         )
 
+    # ooo condition
+    out_of_order = t <= state[0]
+    if out_of_order:
+        return (
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+        )
     state[2] += 1
     if t - state[0] >= duration_seconds:
         state[0] = t
         state[1] = z
         count = state[2]
         state[2] = 0
         return (
@@ -221,14 +238,23 @@
         )
 
     state[2] += 1
     deviation_condition = abs(z - state[1]) >= deviation
     min_duration_condition = (t - state[0]) >= min_duration_seconds
     max_duration_condition = (t - state[0]) >= max_duration_seconds
 
+    # ooo condition
+    out_of_order = t <= state[0]
+    if out_of_order:
+        return (
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+        )
+
     if (deviation_condition and min_duration_condition) or max_duration_condition:
         state[0] = t
         state[1] = z
         count = state[2]
         state[2] = 0
         return (
             np.array([t], dtype=np.float64),
@@ -274,14 +300,23 @@
         )
 
     state[4] += 1
     deviation_condition = abs(z - state[1]) >= deviation
     min_duration_condition = (t - state[0]) >= min_duration_seconds
     max_duration_condition = (t - state[0]) >= max_duration_seconds
 
+    # ooo condition
+    out_of_order = t <= state[0]
+    if out_of_order:
+        return (
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+        )
+
     if (deviation_condition and min_duration_condition) or max_duration_condition:
         # case 1: last hold point and previous point are the same
         count = state[4]
         if abs(state[0] - state[2]) < 1.0e-6:
             t_array = [t]
             z_array = [z]
             c_array = [count]
@@ -343,14 +378,24 @@
             np.array([0], dtype=np.float64),
         )
 
     state[6] += 1
     # calculate slopes
     # GE = deviation/2
     # PI = deviation
+
+    # ooo condition
+    if t <= state[0]:
+        # do nothing
+        return (
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+            np.zeros(0, np.float64),
+        )
+
     min_slope = (z - deviation - state[1]) / (t - state[0])
     max_slope = (z + deviation - state[1]) / (t - state[0])
 
     slope_condition = min_slope <= state[2] or max_slope >= state[3]
     min_duration_condition = (t - state[0]) >= min_duration_seconds
     max_duration_condition = (t - state[0]) >= max_duration_seconds
```

### Comparing `realtime_operator-0.2.7/realtime_operator/single_operator.py` & `realtime_operator-0.2.8/realtime_operator/single_operator.py`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.7/realtime_operator.egg-info/PKG-INFO` & `realtime_operator-0.2.8/realtime_operator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: realtime_operator
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package to perfom real-time operations on time seriesdata streams.
 Author-email: Ernst Holger Amort <holgeramort@gmail.com>
 Project-URL: Homepage, https://github.com/ErnstHolger/realtime_operator
 Project-URL: Issues, https://github.com/ErnstHolger/realtime_operator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `realtime_operator-0.2.7/tests/test_compression.py` & `realtime_operator-0.2.8/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `realtime_operator-0.2.7/tests/test_single_operator.py` & `realtime_operator-0.2.8/tests/test_single_operator.py`

 * *Files identical despite different names*


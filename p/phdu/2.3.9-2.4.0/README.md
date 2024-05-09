# Comparing `tmp/phdu-2.3.9.tar.gz` & `tmp/phdu-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.3.9.tar", last modified: Thu May  9 10:10:21 2024, max compression
+gzip compressed data, was "phdu-2.4.0.tar", last modified: Thu May  9 10:22:26 2024, max compression
```

## Comparing `phdu-2.3.9.tar` & `phdu-2.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:21.032471 phdu-2.3.9/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.3.9/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-05-09 10:10:21.036471 phdu-2.3.9/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.3.9/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.592445 phdu-2.3.9/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.3.9/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/analysis.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.3.9/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.3.9/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/geometry.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     6214 2024-04-09 08:31:50.000000 phdu-2.3.9/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.736453 phdu-2.3.9/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.3.9/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.3.9/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.3.9/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    23237 2024-04-30 08:50:03.000000 phdu-2.3.9/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.3.9/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.872461 phdu-2.3.9/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.3.9/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.3.9/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.3.9/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.3.9/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    32574 2024-05-09 10:09:46.000000 phdu-2.3.9/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.3.9/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.3.9/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.948466 phdu-2.3.9/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.3.9/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.3.9/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.3.9/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:21.016470 phdu-2.3.9/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.3.9/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.3.9/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.3.9/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.668449 phdu-2.3.9/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-05-09 10:10:21.060472 phdu-2.3.9/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-05-09 10:10:06.000000 phdu-2.3.9/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:22:26.650347 phdu-2.4.0/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.4.0/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-05-09 10:22:26.650347 phdu-2.4.0/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.4.0/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:22:26.370330 phdu-2.4.0/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.4.0/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.4.0/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.4.0/phdu/analysis.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.4.0/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.4.0/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.4.0/phdu/geometry.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.4.0/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     6214 2024-04-09 08:31:50.000000 phdu-2.4.0/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:22:26.434334 phdu-2.4.0/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.4.0/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.4.0/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.4.0/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    23237 2024-04-30 08:50:03.000000 phdu-2.4.0/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.4.0/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:22:26.574342 phdu-2.4.0/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.4.0/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.4.0/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.4.0/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.4.0/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    33300 2024-05-09 10:22:04.000000 phdu-2.4.0/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.4.0/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.4.0/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:22:26.618345 phdu-2.4.0/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.4.0/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.4.0/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.4.0/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:22:26.642346 phdu-2.4.0/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.4.0/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.4.0/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.4.0/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.4.0/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:22:26.406333 phdu-2.4.0/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-05-09 10:22:26.000000 phdu-2.4.0/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-05-09 10:22:26.000000 phdu-2.4.0/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-05-09 10:22:26.000000 phdu-2.4.0/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-05-09 10:22:26.000000 phdu-2.4.0/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-05-09 10:22:26.000000 phdu-2.4.0/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-05-09 10:22:26.658347 phdu-2.4.0/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-05-09 10:22:20.000000 phdu-2.4.0/setup.py
```

### Comparing `phdu-2.3.9/LICENSE.md` & `phdu-2.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/PKG-INFO` & `phdu-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.9
+Version: 2.4.0
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.9/README.md` & `phdu-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/__init__.py` & `phdu-2.4.0/phdu/__init__.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/_helper.py` & `phdu-2.4.0/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/analysis.py` & `phdu-2.4.0/phdu/analysis.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/clustering.py` & `phdu-2.4.0/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/decomposition.py` & `phdu-2.4.0/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/geometry.py` & `phdu-2.4.0/phdu/geometry.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/np_utils.py` & `phdu-2.4.0/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/pd_utils.py` & `phdu-2.4.0/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/plots/base.py` & `phdu-2.4.0/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/plots/plotly_utils.py` & `phdu-2.4.0/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/script_fmt.py` & `phdu-2.4.0/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/stats/_integration.py` & `phdu-2.4.0/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/stats/_plots.py` & `phdu-2.4.0/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/stats/bootstrap.py` & `phdu-2.4.0/phdu/stats/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,19 +246,34 @@
 
 @njit
 def jackknife_stat_nb(data, statistic):
     resamples = jackknife_resampling(data)
     stats = np.array([statistic(r) for r in resamples])
     return stats
 
-def jackknife_stat_two_samples(data, data2, statistic):
-    jk_X = jackknife_resampling(data)
-    jk_Y = jackknife_resampling(data2)
-    jk_XY = [*product(jk_X, jk_Y)]
-    stats = np.array([statistic(*r) for r in jk_XY])
+def jackknife_stat_two_samples(data, data2, statistic, aggregator=None):
+    if isinstance(data, np.ndarray): # not block
+        jk_X = jackknife_resampling(data)
+        jk_Y = jackknife_resampling(data2)
+        jk_XY = [*product(jk_X, jk_Y)]
+        stats = np.array([statistic(*r) for r in jk_XY])
+    elif isinstance(data, tuple): # block
+        jk_Xs = [jackknife_resampling(x) for x in data]
+        jk_Ys = [jackknife_resampling(y) for y in data2]
+        jk_X  = product(*jk_Xs)
+        jk_Y  = product(*jk_Ys)
+        jk_XY = product(jk_X, jk_Y)
+        if aggregator is None:
+            stats = np.array([statistic(*r) for r in jk_XY])
+        else:
+            def _preprocess(x):
+                return np.array([aggregator(xi) for xi in x])
+            stats = np.array([statistic(_preprocess(x), _preprocess(y)) for x, y in jk_XY])
+    else:
+        raise ValueError("data must be a tuple or np.ndarray.")
     return stats
 
 def jackknife_stat_(data, statistic):
     resamples = jackknife_resampling(data)
     stats = np.array([statistic(r) for r in resamples])
     return stats
 
@@ -390,15 +405,15 @@
     z0_hat = ndtri(percentile)
 
     # calculate a_hat
     if data2 is None:
         jackknife_computer = jackknife_stat_nb if use_numba else jackknife_stat
         theta_hat_jk = jackknife_computer(data, statistic)  # jackknife resample
     else:
-        theta_hat_jk = jackknife_stat_two_samples(data, data2, statistic)
+        theta_hat_jk = jackknife_stat_two_samples(data, data2, statistic, aggregator=aggregator)
     n = theta_hat_jk.shape[0]
     theta_hat_jk_dot = theta_hat_jk.mean(axis=0)
 
     U = (n - 1) * (theta_hat_jk_dot - theta_hat_jk)
     num = (U**3).sum(axis=0) / n**3
     den = (U**2).sum(axis=0) / n**2
     a_hat = 1/6 * num / (den**(3/2))
```

### Comparing `phdu-2.3.9/phdu/stats/conf_interval.py` & `phdu-2.4.0/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/stats/corr.py` & `phdu-2.4.0/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/stats/rtopy/_helper.py` & `phdu-2.4.0/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/stats/rtopy/resample.py` & `phdu-2.4.0/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/stats/test/permutation.py` & `phdu-2.4.0/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu/storage.py` & `phdu-2.4.0/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/phdu.egg-info/PKG-INFO` & `phdu-2.4.0/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.9
+Version: 2.4.0
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.9/phdu.egg-info/SOURCES.txt` & `phdu-2.4.0/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.3.9/setup.py` & `phdu-2.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.3.9',
+    version='2.4.0',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```


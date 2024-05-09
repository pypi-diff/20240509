# Comparing `tmp/phdu-2.3.8.tar.gz` & `tmp/phdu-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.3.8.tar", last modified: Mon Apr 29 12:09:18 2024, max compression
+gzip compressed data, was "phdu-2.3.9.tar", last modified: Thu May  9 10:10:21 2024, max compression
```

## Comparing `phdu-2.3.8.tar` & `phdu-2.3.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/
--rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-07-31 18:53:26.000000 phdu-2.3.8/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     2864 2024-04-29 12:09:18.389218 phdu-2.3.8/PKG-INFO
--rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-07-31 18:53:26.000000 phdu-2.3.8/README.md
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.385885 phdu-2.3.8/phdu/
--rw-r--r--   0 userx     (1000) wheel      (998)      590 2024-02-24 02:21:10.000000 phdu-2.3.8/phdu/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1948 2023-09-21 17:52:42.000000 phdu-2.3.8/phdu/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2484 2024-02-04 05:18:27.000000 phdu-2.3.8/phdu/analysis.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3664 2023-10-17 21:07:41.000000 phdu-2.3.8/phdu/clustering.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/decomposition.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1333 2023-12-05 04:36:26.000000 phdu-2.3.8/phdu/geometry.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3183 2024-01-23 06:00:25.000000 phdu-2.3.8/phdu/np_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     6214 2024-04-07 07:28:04.000000 phdu-2.3.8/phdu/pd_utils.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu/plots/
--rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/plots/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/plots/_mpl.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4011 2023-12-05 02:04:31.000000 phdu-2.3.8/phdu/plots/base.py
--rw-r--r--   0 userx     (1000) wheel      (998)    23237 2024-04-29 12:08:17.000000 phdu-2.3.8/phdu/plots/plotly_utils.py
--rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/script_fmt.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu/stats/
--rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/_integration.py
--rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/_plots.py
--rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/_preprocess.py
--rw-r--r--   0 userx     (1000) wheel      (998)    32282 2024-01-18 07:19:52.000000 phdu-2.3.8/phdu/stats/bootstrap.py
--rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/conf_interval.py
--rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/corr.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu/stats/rtopy/
--rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu/stats/test/
--rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/test/__init__.py
--rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/test/_adherence.py
--rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-07-31 18:53:27.000000 phdu-2.3.8/phdu/stats/test/permutation.py
--rw-r--r--   0 userx     (1000) wheel      (998)     4437 2024-02-24 02:19:42.000000 phdu-2.3.8/phdu/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-29 12:09:18.389218 phdu-2.3.8/phdu.egg-info/
--rwxr-xr-x   0 userx     (1000) wheel      (998)     2864 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)      786 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/SOURCES.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/dependency_links.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/requires.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        5 2024-04-29 12:09:18.000000 phdu-2.3.8/phdu.egg-info/top_level.txt
--rw-r--r--   0 userx     (1000) wheel      (998)      106 2024-04-29 12:09:18.389218 phdu-2.3.8/setup.cfg
--rw-r--r--   0 userx     (1000) wheel      (998)     1659 2024-04-29 12:08:50.000000 phdu-2.3.8/setup.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:21.032471 phdu-2.3.9/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.3.9/LICENSE.md
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-05-09 10:10:21.036471 phdu-2.3.9/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.3.9/README.md
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.592445 phdu-2.3.9/phdu/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.3.9/phdu/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/analysis.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.3.9/phdu/clustering.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.3.9/phdu/decomposition.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/geometry.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/np_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     6214 2024-04-09 08:31:50.000000 phdu-2.3.9/phdu/pd_utils.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.736453 phdu-2.3.9/phdu/plots/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.3.9/phdu/plots/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.3.9/phdu/plots/_mpl.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.3.9/phdu/plots/base.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    23237 2024-04-30 08:50:03.000000 phdu-2.3.9/phdu/plots/plotly_utils.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.3.9/phdu/script_fmt.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.872461 phdu-2.3.9/phdu/stats/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.3.9/phdu/stats/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.3.9/phdu/stats/_integration.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.3.9/phdu/stats/_plots.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.3.9/phdu/stats/_preprocess.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    32574 2024-05-09 10:09:46.000000 phdu-2.3.9/phdu/stats/bootstrap.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.3.9/phdu/stats/conf_interval.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.3.9/phdu/stats/corr.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.948466 phdu-2.3.9/phdu/stats/rtopy/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.3.9/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.3.9/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.3.9/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:21.016470 phdu-2.3.9/phdu/stats/test/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.3.9/phdu/stats/test/__init__.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.3.9/phdu/stats/test/_adherence.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.3.9/phdu/stats/test/permutation.py
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.3.9/phdu/storage.py
+drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-09 10:10:20.668449 phdu-2.3.9/phdu.egg-info/
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/PKG-INFO
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/SOURCES.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/dependency_links.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/requires.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-05-09 10:10:19.000000 phdu-2.3.9/phdu.egg-info/top_level.txt
+-rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-05-09 10:10:21.060472 phdu-2.3.9/setup.cfg
+-rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-05-09 10:10:06.000000 phdu-2.3.9/setup.py
```

### Comparing `phdu-2.3.8/LICENSE.md` & `phdu-2.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/PKG-INFO` & `phdu-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.8
+Version: 2.3.9
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.8/README.md` & `phdu-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/__init__.py` & `phdu-2.3.9/phdu/__init__.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/_helper.py` & `phdu-2.3.9/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/analysis.py` & `phdu-2.3.9/phdu/analysis.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/clustering.py` & `phdu-2.3.9/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/decomposition.py` & `phdu-2.3.9/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/geometry.py` & `phdu-2.3.9/phdu/geometry.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/np_utils.py` & `phdu-2.3.9/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/pd_utils.py` & `phdu-2.3.9/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/plots/base.py` & `phdu-2.3.9/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/plots/plotly_utils.py` & `phdu-2.3.9/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/script_fmt.py` & `phdu-2.3.9/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/stats/_integration.py` & `phdu-2.3.9/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/stats/_plots.py` & `phdu-2.3.9/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/stats/bootstrap.py` & `phdu-2.3.9/phdu/stats/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
         else:
             theta_hat_b = resample_func(data, data2, statistic, R=R, output_len=output_len, **resample_kwargs, **kwargs).squeeze()
             # if stack_data and is_block:
             #     data = np.hstack(data)
             #     data2 = np.hstack(data2)
     return data, data2, theta_hat_b, sample_stat, N
 
-def CI_bca(data, statistic, data2=None, alternative='two-sided', alpha=0.05, R=int(1e5), account_equal=False, use_numba=True, n_min=5, **kwargs):
+def CI_bca(data, statistic, data2=None, alternative='two-sided', alpha=0.05, R=int(1e5), account_equal=False, use_numba=True, n_min=5, aggregator=_nb_mean, **kwargs):
     """
     If data2 is provided, assumes a block resampling and statistic takes two arguments.
     Optional kwargs for aggregating data, data2 before computing the statistic:
             aggregator = @njit
                          def nb_mean(x):
                              return np.mean(x)
     """
@@ -348,20 +348,20 @@
     elif alternative == 'less':
         probs = np.array([0, 1-alpha])
     elif alternative == 'greater':
         probs = np.array([alpha, 1])
     else:
         raise ValueError(f"alternative '{alternative}' not valid. Available: 'two-sided', 'less', 'greater'.")
 
-    data, data2, theta_hat_b, sample_stat, N = _resample(data, data2, use_numba, statistic, R=R, n_min=n_min, **kwargs)
+    data, data2, theta_hat_b, sample_stat, N = _resample(data, data2, use_numba, statistic, R=R, n_min=n_min, aggregator=aggregator, **kwargs)
 
     if theta_hat_b is None:
         return np.array([np.NaN, np.NaN])
 
-    alpha_bca = _bca_interval(data, data2, statistic, probs, theta_hat_b, account_equal, use_numba)[0]
+    alpha_bca = _bca_interval(data, data2, statistic, probs, theta_hat_b, account_equal, use_numba, aggregator=aggregator)[0]
 
     if np.isnan(alpha_bca).all():
         warnings.warn('CI shows there is only one value. Check data.', RuntimeWarning)
         if data2 is None:
             sample_stat = statistic(data)
         else:
             sample_stat = statistic(data, data2)
@@ -371,21 +371,25 @@
     #elif alternative == 'two-sided':
     #    return  np.percentile(theta_hat_b, alpha_bca*100, axis=0)
     #elif alternative == 'less':
     #     return np.array([-np.inf, np.percentile(theta_hat_b, alpha_bca[0]*100, axis=0)])
     #elif alternative == 'greater':
     #    return np.array([np.percentile(theta_hat_b, alpha_bca[0]*100, axis=0), np.inf])
 
-def _bca_interval(data, data2, statistic, probs, theta_hat_b, account_equal, use_numba):
+def _bca_interval(data, data2, statistic, probs, theta_hat_b, account_equal, use_numba, aggregator=None):
     """Bias-corrected and accelerated interval."""
     # calculate z0_hat
     if data2 is None:
         theta_hat = statistic(data)
     else:
-        theta_hat = statistic(data, data2)
+        if aggregator is not None:
+            theta_hat = statistic(np.array([aggregator(di) for di in data]),
+                                  np.array([aggregator(di) for di in data2]))
+        else:
+            theta_hat = statistic(data, data2)
     percentile = _percentile_of_score(theta_hat_b, theta_hat, axis=-1, account_equal=account_equal)
     z0_hat = ndtri(percentile)
 
     # calculate a_hat
     if data2 is None:
         jackknife_computer = jackknife_stat_nb if use_numba else jackknife_stat
         theta_hat_jk = jackknife_computer(data, statistic)  # jackknife resample
```

### Comparing `phdu-2.3.8/phdu/stats/conf_interval.py` & `phdu-2.3.9/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/stats/corr.py` & `phdu-2.3.9/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/stats/rtopy/_helper.py` & `phdu-2.3.9/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/stats/rtopy/resample.py` & `phdu-2.3.9/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/stats/test/permutation.py` & `phdu-2.3.9/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu/storage.py` & `phdu-2.3.9/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/phdu.egg-info/PKG-INFO` & `phdu-2.3.9/phdu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.3.8
+Version: 2.3.9
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.3.8/phdu.egg-info/SOURCES.txt` & `phdu-2.3.9/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.3.8/setup.py` & `phdu-2.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.3.8',
+    version='2.3.9',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```


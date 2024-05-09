# Comparing `tmp/tools-jsyoo61-2024.5.2.5.tar.gz` & `tmp/tools-jsyoo61-2024.5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tools-jsyoo61-2024.5.2.5.tar", last modified: Fri May  3 18:33:18 2024, max compression
+gzip compressed data, was "tools-jsyoo61-2024.5.9.0.tar", last modified: Thu May  9 20:56:59 2024, max compression
```

## Comparing `tools-jsyoo61-2024.5.2.5.tar` & `tools-jsyoo61-2024.5.9.0.tar`

### file list

```diff
@@ -1,50 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.151652 tools-jsyoo61-2024.5.2.5/
--rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1342 2024-05-03 18:33:18.150655 tools-jsyoo61-2024.5.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 18:33:18.151652 tools-jsyoo61-2024.5.2.5/setup.cfg
--rw-rw-rw-   0        0        0      821 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.090658 tools-jsyoo61-2024.5.2.5/tools/
--rw-rw-rw-   0        0        0      292 2024-05-03 18:33:11.000000 tools-jsyoo61-2024.5.2.5/tools/__init__.py
--rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/array.py
--rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/data.py
--rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/exp.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.092679 tools-jsyoo61-2024.5.2.5/tools/hydra/
--rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/hydra/__init__.py
--rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.2.5/tools/modules.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.096660 tools-jsyoo61-2024.5.2.5/tools/numpy/
--rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/numpy/__init__.py
--rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/numpy/_f.py
--rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/numpy/_utils.py
--rw-rw-rw-   0        0        0     2279 2024-05-03 02:04:50.000000 tools-jsyoo61-2024.5.2.5/tools/os.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.098666 tools-jsyoo61-2024.5.2.5/tools/pandas/
--rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.102660 tools-jsyoo61-2024.5.2.5/tools/plot/
--rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/plot/__init__.py
--rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/plot/sklearn.py
--rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/plot/utils.py
--rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/random.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.105663 tools-jsyoo61-2024.5.2.5/tools/sklearn/
--rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/sklearn/__init__.py
--rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.2.5/tools/sklearn/model_selection.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.107663 tools-jsyoo61-2024.5.2.5/tools/stats/
--rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.2.5/tools/stats/__init__.py
--rw-rw-rw-   0        0        0    15603 2024-05-03 18:32:59.000000 tools-jsyoo61-2024.5.2.5/tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.120658 tools-jsyoo61-2024.5.2.5/tools/torch/
--rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/torch/__init__.py
--rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/torch/_pandas.py
--rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/torch/estimator.py
--rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/torch/federated_learning.py
--rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/torch/layers.py
--rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.2.5/tools/torch/model.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.125064 tools-jsyoo61-2024.5.2.5/tools/torch/optim/
--rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/torch/optim/__init__.py
--rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/torch/optim/lr_scheduler.py
--rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.2.5/tools/torch/plot.py
--rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.2.5/tools/torch/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-03 18:33:18.149655 tools-jsyoo61-2024.5.2.5/tools_jsyoo61.egg-info/
--rw-rw-rw-   0        0        0     1342 2024-05-03 18:33:17.000000 tools-jsyoo61-2024.5.2.5/tools_jsyoo61.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2024-05-03 18:33:17.000000 tools-jsyoo61-2024.5.2.5/tools_jsyoo61.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 18:33:17.000000 tools-jsyoo61-2024.5.2.5/tools_jsyoo61.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-03 18:33:17.000000 tools-jsyoo61-2024.5.2.5/tools_jsyoo61.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-03 18:33:17.000000 tools-jsyoo61-2024.5.2.5/tools_jsyoo61.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.783680 tools-jsyoo61-2024.5.9.0/
+-rw-rw-rw-   0        0        0     1089 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1338 2024-05-09 20:56:59.781680 tools-jsyoo61-2024.5.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 20:56:59.784679 tools-jsyoo61-2024.5.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      819 2024-05-09 20:56:32.000000 tools-jsyoo61-2024.5.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.658129 tools-jsyoo61-2024.5.9.0/tools/
+-rw-rw-rw-   0        0        0      292 2024-05-09 20:56:46.000000 tools-jsyoo61-2024.5.9.0/tools/__init__.py
+-rw-rw-rw-   0        0        0     1100 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/array.py
+-rw-rw-rw-   0        0        0     3207 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/data.py
+-rw-rw-rw-   0        0        0     6927 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/exp.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.661130 tools-jsyoo61-2024.5.9.0/tools/hydra/
+-rw-rw-rw-   0        0        0      143 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/hydra/__init__.py
+-rw-rw-rw-   0        0        0     3263 2022-09-12 22:10:08.000000 tools-jsyoo61-2024.5.9.0/tools/modules.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.670915 tools-jsyoo61-2024.5.9.0/tools/numpy/
+-rw-rw-rw-   0        0        0      235 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1389 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/numpy/_f.py
+-rw-rw-rw-   0        0        0      960 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/numpy/_utils.py
+-rw-rw-rw-   0        0        0     2279 2024-05-03 02:04:50.000000 tools-jsyoo61-2024.5.9.0/tools/os.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.673923 tools-jsyoo61-2024.5.9.0/tools/pandas/
+-rw-rw-rw-   0        0        0       40 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.686451 tools-jsyoo61-2024.5.9.0/tools/plot/
+-rw-rw-rw-   0        0        0       86 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/plot/__init__.py
+-rw-rw-rw-   0        0        0      809 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/plot/sklearn.py
+-rw-rw-rw-   0        0        0     2371 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/plot/utils.py
+-rw-rw-rw-   0        0        0      834 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/random.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.692450 tools-jsyoo61-2024.5.9.0/tools/sklearn/
+-rw-rw-rw-   0        0        0       33 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/sklearn/__init__.py
+-rw-rw-rw-   0        0        0     6721 2024-01-22 14:45:14.000000 tools-jsyoo61-2024.5.9.0/tools/sklearn/model_selection.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.696994 tools-jsyoo61-2024.5.9.0/tools/stats/
+-rw-rw-rw-   0        0        0     1241 2024-03-19 18:49:39.000000 tools-jsyoo61-2024.5.9.0/tools/stats/__init__.py
+-rw-rw-rw-   0        0        0    15603 2024-05-03 18:32:59.000000 tools-jsyoo61-2024.5.9.0/tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.725321 tools-jsyoo61-2024.5.9.0/tools/torch/
+-rw-rw-rw-   0        0        0      460 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/__init__.py
+-rw-rw-rw-   0        0        0      333 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/_pandas.py
+-rw-rw-rw-   0        0        0     2046 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/estimator.py
+-rw-rw-rw-   0        0        0    10951 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/federated_learning.py
+-rw-rw-rw-   0        0        0      310 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/layers.py
+-rw-rw-rw-   0        0        0    18008 2024-03-14 20:51:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/model.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.734099 tools-jsyoo61-2024.5.9.0/tools/torch/optim/
+-rw-rw-rw-   0        0        0       30 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/optim/__init__.py
+-rw-rw-rw-   0        0        0     8208 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/optim/lr_scheduler.py
+-rw-rw-rw-   0        0        0      266 2022-07-01 04:57:33.000000 tools-jsyoo61-2024.5.9.0/tools/torch/plot.py
+-rw-rw-rw-   0        0        0     2880 2022-08-18 21:12:21.000000 tools-jsyoo61-2024.5.9.0/tools/torch/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 20:56:59.778682 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/
+-rw-rw-rw-   0        0        0     1338 2024-05-09 20:56:58.000000 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2024-05-09 20:56:59.000000 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 20:56:58.000000 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-09 20:56:58.000000 tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/top_level.txt
```

### Comparing `tools-jsyoo61-2024.5.2.5/LICENSE.txt` & `tools-jsyoo61-2024.5.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/PKG-INFO` & `tools-jsyoo61-2024.5.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.2.5
+Version: 2024.5.9.0
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
-Author-email: jsyoo61@korea.ac.kr
+Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `tools-jsyoo61-2024.5.2.5/README.md` & `tools-jsyoo61-2024.5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/setup.py` & `tools-jsyoo61-2024.5.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tools-jsyoo61", # Replace with your own username
     version=__version__,
     author="JaeSung Yoo",
-    author_email="jsyoo61@korea.ac.kr",
+    author_email="jsyoo61@unc.edu",
     description="personal syntax tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jsyoo61/tools",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=['numpy','pandas','matplotlib']
+    # install_requires=['numpy','pandas','matplotlib']
 )
```

### Comparing `tools-jsyoo61-2024.5.2.5/tools/array.py` & `tools-jsyoo61-2024.5.9.0/tools/array.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/data.py` & `tools-jsyoo61-2024.5.9.0/tools/data.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/exp.py` & `tools-jsyoo61-2024.5.9.0/tools/exp.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/modules.py` & `tools-jsyoo61-2024.5.9.0/tools/modules.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/numpy/_f.py` & `tools-jsyoo61-2024.5.9.0/tools/numpy/_f.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/numpy/_utils.py` & `tools-jsyoo61-2024.5.9.0/tools/numpy/_utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/os.py` & `tools-jsyoo61-2024.5.9.0/tools/os.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/plot/sklearn.py` & `tools-jsyoo61-2024.5.9.0/tools/plot/sklearn.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/plot/utils.py` & `tools-jsyoo61-2024.5.9.0/tools/plot/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/random.py` & `tools-jsyoo61-2024.5.9.0/tools/random.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/sklearn/model_selection.py` & `tools-jsyoo61-2024.5.9.0/tools/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/stats/__init__.py` & `tools-jsyoo61-2024.5.9.0/tools/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/tools.py` & `tools-jsyoo61-2024.5.9.0/tools/tools.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/torch/estimator.py` & `tools-jsyoo61-2024.5.9.0/tools/torch/estimator.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/torch/federated_learning.py` & `tools-jsyoo61-2024.5.9.0/tools/torch/federated_learning.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/torch/model.py` & `tools-jsyoo61-2024.5.9.0/tools/torch/model.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/torch/optim/lr_scheduler.py` & `tools-jsyoo61-2024.5.9.0/tools/torch/optim/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools/torch/utils.py` & `tools-jsyoo61-2024.5.9.0/tools/torch/utils.py`

 * *Files identical despite different names*

### Comparing `tools-jsyoo61-2024.5.2.5/tools_jsyoo61.egg-info/PKG-INFO` & `tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tools-jsyoo61
-Version: 2024.5.2.5
+Version: 2024.5.9.0
 Summary: personal syntax tool
 Home-page: https://github.com/jsyoo61/tools
 Author: JaeSung Yoo
-Author-email: jsyoo61@korea.ac.kr
+Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `tools-jsyoo61-2024.5.2.5/tools_jsyoo61.egg-info/SOURCES.txt` & `tools-jsyoo61-2024.5.9.0/tools_jsyoo61.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -29,9 +29,8 @@
 tools/torch/plot.py
 tools/torch/utils.py
 tools/torch/optim/__init__.py
 tools/torch/optim/lr_scheduler.py
 tools_jsyoo61.egg-info/PKG-INFO
 tools_jsyoo61.egg-info/SOURCES.txt
 tools_jsyoo61.egg-info/dependency_links.txt
-tools_jsyoo61.egg-info/requires.txt
 tools_jsyoo61.egg-info/top_level.txt
```


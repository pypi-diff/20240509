# Comparing `tmp/deep_autoviml-0.0.85.tar.gz` & `tmp/deep_autoviml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deep_autoviml-0.0.85.tar", last modified: Thu May  9 13:43:08 2024, max compression
+gzip compressed data, was "dist/deep_autoviml-0.0.9.tar", last modified: Tue May 25 02:00:13 2021, max compression
```

## Comparing `deep_autoviml-0.0.85.tar` & `deep_autoviml-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,15 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 13:43:08.600797 deep_autoviml-0.0.85/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11560 2021-10-30 12:53:31.000000 deep_autoviml-0.0.85/LICENSE
--rwxrwxrwx   0 ram       (1000) ram       (1000)    20796 2024-05-09 13:43:08.600797 deep_autoviml-0.0.85/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    20155 2024-05-09 13:10:41.000000 deep_autoviml-0.0.85/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 13:43:07.578477 deep_autoviml-0.0.85/deep_autoviml/
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2703 2023-12-24 16:31:21.000000 deep_autoviml-0.0.85/deep_autoviml/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1160 2024-05-09 12:42:06.000000 deep_autoviml-0.0.85/deep_autoviml/__version__.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 13:43:07.744708 deep_autoviml-0.0.85/deep_autoviml/data_load/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    67470 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/data_load/classify_features.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    70595 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/data_load/extract.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    31809 2024-05-09 12:42:49.000000 deep_autoviml-0.0.85/deep_autoviml/deep_autoviml.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 13:43:07.981479 deep_autoviml-0.0.85/deep_autoviml/modeling/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    29227 2024-05-09 12:55:11.000000 deep_autoviml-0.0.85/deep_autoviml/modeling/create_model.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     5863 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/modeling/one_cycle.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    40820 2024-05-09 12:50:10.000000 deep_autoviml-0.0.85/deep_autoviml/modeling/predict_model.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    58351 2024-05-09 13:00:00.000000 deep_autoviml-0.0.85/deep_autoviml/modeling/train_custom_model.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     7228 2024-05-09 12:48:46.000000 deep_autoviml-0.0.85/deep_autoviml/modeling/train_image_model.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    21733 2024-05-09 12:57:18.000000 deep_autoviml-0.0.85/deep_autoviml/modeling/train_model.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     7597 2024-05-09 12:49:00.000000 deep_autoviml-0.0.85/deep_autoviml/modeling/train_text_model.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 13:43:08.331203 deep_autoviml-0.0.85/deep_autoviml/models/
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2315 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/models/basic.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2848 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/models/cnn1.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2511 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/models/cnn2.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2362 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/models/deep_and_wide.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2154 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/models/dnn.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2508 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/models/dnn_drop.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2498 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/models/giant_deep.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2594 2023-11-20 13:25:48.000000 deep_autoviml-0.0.85/deep_autoviml/models/gru1.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2790 2023-11-20 13:25:48.000000 deep_autoviml-0.0.85/deep_autoviml/models/lstm1.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2303 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/models/reg_dnn.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2619 2023-11-20 13:25:48.000000 deep_autoviml-0.0.85/deep_autoviml/models/rnn1.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     7814 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/models/tf_hub_lookup.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 13:43:08.447105 deep_autoviml-0.0.85/deep_autoviml/preprocessing/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    26829 2023-11-20 13:48:06.000000 deep_autoviml-0.0.85/deep_autoviml/preprocessing/preprocessing.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     5587 2024-05-09 12:45:48.000000 deep_autoviml-0.0.85/deep_autoviml/preprocessing/preprocessing_images.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    22489 2024-05-09 12:45:04.000000 deep_autoviml-0.0.85/deep_autoviml/preprocessing/preprocessing_nlp.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    91268 2024-05-09 12:44:10.000000 deep_autoviml-0.0.85/deep_autoviml/preprocessing/preprocessing_tabular.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     5895 2024-05-09 12:47:10.000000 deep_autoviml-0.0.85/deep_autoviml/preprocessing/preprocessing_text.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 13:43:08.531752 deep_autoviml-0.0.85/deep_autoviml/utilities/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    66683 2023-12-24 16:19:56.000000 deep_autoviml-0.0.85/deep_autoviml/utilities/utilities.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 13:43:08.585171 deep_autoviml-0.0.85/deep_autoviml.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    20796 2024-05-09 13:43:06.000000 deep_autoviml-0.0.85/deep_autoviml.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1337 2024-05-09 13:43:07.000000 deep_autoviml-0.0.85/deep_autoviml.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2024-05-09 13:43:06.000000 deep_autoviml-0.0.85/deep_autoviml.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      244 2024-05-09 13:43:06.000000 deep_autoviml-0.0.85/deep_autoviml.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       14 2024-05-09 13:43:06.000000 deep_autoviml-0.0.85/deep_autoviml.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2024-05-09 13:43:08.600797 deep_autoviml-0.0.85/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     2122 2024-05-09 13:20:55.000000 deep_autoviml-0.0.85/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2021-05-25 02:00:13.604371 deep_autoviml-0.0.9/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12073 2021-05-25 02:00:13.593380 deep_autoviml-0.0.9/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    10711 2021-05-19 13:32:09.000000 deep_autoviml-0.0.9/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2021-05-25 02:00:13.557702 deep_autoviml-0.0.9/deep_autoviml/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     2219 2021-05-25 01:57:03.000000 deep_autoviml-0.0.9/deep_autoviml/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1159 2021-05-25 01:58:44.000000 deep_autoviml-0.0.9/deep_autoviml/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    22123 2021-05-25 00:25:06.000000 deep_autoviml-0.0.9/deep_autoviml/deep_autoviml.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2021-05-25 02:00:13.590388 deep_autoviml-0.0.9/deep_autoviml.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12073 2021-05-25 02:00:13.000000 deep_autoviml-0.0.9/deep_autoviml.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      288 2021-05-25 02:00:13.000000 deep_autoviml-0.0.9/deep_autoviml.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2021-05-25 02:00:13.000000 deep_autoviml-0.0.9/deep_autoviml.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      108 2021-05-25 02:00:13.000000 deep_autoviml-0.0.9/deep_autoviml.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       14 2021-05-25 02:00:13.000000 deep_autoviml-0.0.9/deep_autoviml.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2021-05-25 02:00:13.604491 deep_autoviml-0.0.9/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1732 2021-05-25 01:58:31.000000 deep_autoviml-0.0.9/setup.py
```

### Comparing `deep_autoviml-0.0.85/deep_autoviml/__version__.py` & `deep_autoviml-0.0.9/deep_autoviml/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 # -*- coding: utf-8 -*-
 """Specifies the version of the deep_autoviml package."""
 
 __title__ = "deep_autoviml"
 __author__ = "Ram Seshadri"
 __description__ = "deep_autoviml - build and test multiple Tensorflow 2.0 models and pipelines"
 __url__ = "https://github.com/Auto_ViML/deep_autoviml.git"
-__version__ = "0.0.85"
+__version__ = "0.0.9"
 __license__ = "Apache License 2.0"
 __copyright__ = "2020-21 Google"
```

### Comparing `deep_autoviml-0.0.85/setup.py` & `deep_autoviml-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,46 +16,34 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="deep_autoviml",
-    version="0.0.85",
+    version="0.0.9",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Build Deep Learning Models and Pipelines fast!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/deep_autoviml",
-    packages = [
-        "deep_autoviml",
-        "deep_autoviml.data_load",
-        "deep_autoviml.modeling",
-        "deep_autoviml.models",
-        "deep_autoviml.preprocessing",
-        "deep_autoviml.utilities",
-    ],
-    include_package_data=True,
+    packages=setuptools.find_packages(exclude=("tests",)),
     install_requires=[
         "ipython",
         "jupyter",
-        "tensorflow>=2.8.0,<=2.12.1",
-        "matplotlib>3.7.4",
-        "numpy>=1.24",
-        "pandas>=1.1.3, <2.0",
-        "scikit-learn>=0.24,<=1.2.2",
+        "tensorflow>=2.4.1",
+        "pandas",
+        "matplotlib",
+        "numpy",
+        "scikit-learn>=0.23.1",
         "regex",
         "emoji",
-        "storm-tuner>=0.0.8",
-        "optuna",
-        "tensorflow_hub~=0.12.0",
-        "tensorflow-text>=2.8.0,<=2.12.1",
-        "tensorboard>=2.8.0,<=2.12.3",
+        "storm-tuner",
         "xlrd"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```


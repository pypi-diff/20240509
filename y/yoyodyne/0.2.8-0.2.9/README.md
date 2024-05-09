# Comparing `tmp/yoyodyne-0.2.8.tar.gz` & `tmp/yoyodyne-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoyodyne-0.2.8.tar", last modified: Sat Nov  4 16:34:55 2023, max compression
+gzip compressed data, was "yoyodyne-0.2.9.tar", last modified: Wed Mar  6 19:43:11 2024, max compression
```

## Comparing `yoyodyne-0.2.8.tar` & `yoyodyne-0.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2023-11-04 16:34:55.247473 yoyodyne-0.2.8/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    10814 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/LICENSE.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    16231 2023-11-04 16:34:55.238474 yoyodyne-0.2.8/PKG-INFO
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    15329 2023-11-04 16:28:34.000000 yoyodyne-0.2.8/README.md
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     1277 2023-11-04 16:28:51.000000 yoyodyne-0.2.8/pyproject.toml
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)       38 2023-11-04 16:34:55.248472 yoyodyne-0.2.8/setup.cfg
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2023-11-04 16:34:54.542904 yoyodyne-0.2.8/yoyodyne/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      289 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/__init__.py
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2023-11-04 16:34:54.842969 yoyodyne-0.2.8/yoyodyne/data/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     2431 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/data/__init__.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     3495 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/data/batches.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     5329 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/data/collators.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     6604 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/data/datamodules.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     6215 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/data/datasets.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     4486 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/data/indexes.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     4846 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/data/tsv.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      979 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/defaults.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     5056 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/evaluators.py
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2023-11-04 16:34:55.032027 yoyodyne-0.2.8/yoyodyne/models/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     2089 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/__init__.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    16952 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/base.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    17097 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/expert.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    13213 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/lstm.py
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2023-11-04 16:34:55.212473 yoyodyne-0.2.8/yoyodyne/models/modules/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     3078 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/modules/__init__.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     3305 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/modules/attention.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     4644 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/modules/base.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     1442 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/modules/linear.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     7322 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/modules/lstm.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    26606 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/modules/transformer.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    28491 2023-11-04 16:28:34.000000 yoyodyne-0.2.8/yoyodyne/models/pointer_generator.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    21488 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/transducer.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     6693 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/models/transformer.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     4330 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/predict.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     7693 2023-11-04 16:28:34.000000 yoyodyne-0.2.8/yoyodyne/schedulers.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      169 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/special.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    10572 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/train.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      599 2023-10-23 13:23:27.000000 yoyodyne-0.2.8/yoyodyne/util.py
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2023-11-04 16:34:54.662932 yoyodyne-0.2.8/yoyodyne.egg-info/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    16231 2023-11-04 16:34:54.000000 yoyodyne-0.2.8/yoyodyne.egg-info/PKG-INFO
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      982 2023-11-04 16:34:54.000000 yoyodyne-0.2.8/yoyodyne.egg-info/SOURCES.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)        1 2023-11-04 16:34:54.000000 yoyodyne-0.2.8/yoyodyne.egg-info/dependency_links.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)       96 2023-11-04 16:34:54.000000 yoyodyne-0.2.8/yoyodyne.egg-info/entry_points.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)       82 2023-11-04 16:34:54.000000 yoyodyne-0.2.8/yoyodyne.egg-info/requires.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)        9 2023-11-04 16:34:54.000000 yoyodyne-0.2.8/yoyodyne.egg-info/top_level.txt
+drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2024-03-06 19:43:11.565588 yoyodyne-0.2.9/
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    10814 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/LICENSE.txt
+-rw-r--r--   0 kbg       (1000) kbg       (1000)    16757 2024-03-06 19:43:11.565588 yoyodyne-0.2.9/PKG-INFO
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    15855 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/README.md
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     1277 2024-03-06 19:43:02.000000 yoyodyne-0.2.9/pyproject.toml
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)       38 2024-03-06 19:43:11.565588 yoyodyne-0.2.9/setup.cfg
+drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2024-03-06 19:43:11.561588 yoyodyne-0.2.9/yoyodyne/
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)      289 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/__init__.py
+drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2024-03-06 19:43:11.565588 yoyodyne-0.2.9/yoyodyne/data/
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     2431 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/data/__init__.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     3495 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/data/batches.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     5329 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/data/collators.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     6257 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/data/datamodules.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     6222 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/data/datasets.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     4486 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/data/indexes.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     4831 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/data/tsv.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)      979 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/defaults.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     5056 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/evaluators.py
+drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2024-03-06 19:43:11.565588 yoyodyne-0.2.9/yoyodyne/models/
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     2089 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/__init__.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    16952 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/base.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    17229 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/expert.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    13213 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/lstm.py
+drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2024-03-06 19:43:11.565588 yoyodyne-0.2.9/yoyodyne/models/modules/
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     3078 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/modules/__init__.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     3305 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/modules/attention.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     4636 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/modules/base.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     1442 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/modules/linear.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     7322 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/modules/lstm.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    26606 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/modules/transformer.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    28535 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/pointer_generator.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    21530 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/transducer.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     6693 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/models/transformer.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     4330 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/predict.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     7693 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/schedulers.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)      169 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/special.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    10535 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/train.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)      599 2024-03-06 19:42:48.000000 yoyodyne-0.2.9/yoyodyne/util.py
+drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2024-03-06 19:43:11.565588 yoyodyne-0.2.9/yoyodyne.egg-info/
+-rw-r--r--   0 kbg       (1000) kbg       (1000)    16757 2024-03-06 19:43:11.000000 yoyodyne-0.2.9/yoyodyne.egg-info/PKG-INFO
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)      982 2024-03-06 19:43:11.000000 yoyodyne-0.2.9/yoyodyne.egg-info/SOURCES.txt
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)        1 2024-03-06 19:43:11.000000 yoyodyne-0.2.9/yoyodyne.egg-info/dependency_links.txt
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)       96 2024-03-06 19:43:11.000000 yoyodyne-0.2.9/yoyodyne.egg-info/entry_points.txt
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)       82 2024-03-06 19:43:11.000000 yoyodyne-0.2.9/yoyodyne.egg-info/requires.txt
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)        9 2024-03-06 19:43:11.000000 yoyodyne-0.2.9/yoyodyne.egg-info/top_level.txt
```

### Comparing `yoyodyne-0.2.8/LICENSE.txt` & `yoyodyne-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/PKG-INFO` & `yoyodyne-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoyodyne
-Version: 0.2.8
+Version: 0.2.9
 Summary: Small-vocabulary neural sequence-to-sequence models
 Author: Adam Wiemerslage, Kyle Gorman, Travis Bartley
 License: Apache 2.0
 Project-URL: homepage, https://github.com/CUNY-CL/yoyodyne
 Keywords: computational linguistics,morphology,natural language processing,language
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -55,30 +55,44 @@
     architecture-specific code to handle feature information.
 -   It uses validation accuracy (not loss) for model selection and early
     stopping.
 -   Releases are made regularly.
 -   🚧 UNDER CONSTRUCTION 🚧: It has exhaustive test suites.
 -   🚧 UNDER CONSTRUCTION 🚧: It has performance benchmarks.
 
-## Install
+## Installation
+
+### Local installation
+
+Yoyodyne currently supports Python 3.9 and 3.10.
+[#60](https://github.com/CUNY-CL/yoyodyne/issues/60) is a known blocker to
+Python \> 3.10 support.
 
 First install dependencies:
 
     pip install -r requirements.txt
 
 Then install:
 
     pip install .
 
 It can then be imported like a regular Python module:
 
-``` python
+```python
 import yoyodyne
 ```
 
+### Google Colab
+
+Yoyodyne is compatible with [Google Colab](https://colab.research.google.com/)
+GPU runtimes. [This
+notebook](https://colab.research.google.com/drive/1O4VWvpqLrCxxUvyYMbGH9HOyXQSoh5bP?usp=sharing)
+provides a worked example. Colab also provides access to TPU runtimes, but this
+is not yet compatible with Yoyodyne to our knowledge.
+
 ## Usage
 
 ### Training
 
 Training is performed by the [`yoyodyne-train`](yoyodyne/train.py) script. One
 must specify the following required arguments:
```

### Comparing `yoyodyne-0.2.8/README.md` & `yoyodyne-0.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,30 +32,44 @@
     architecture-specific code to handle feature information.
 -   It uses validation accuracy (not loss) for model selection and early
     stopping.
 -   Releases are made regularly.
 -   🚧 UNDER CONSTRUCTION 🚧: It has exhaustive test suites.
 -   🚧 UNDER CONSTRUCTION 🚧: It has performance benchmarks.
 
-## Install
+## Installation
+
+### Local installation
+
+Yoyodyne currently supports Python 3.9 and 3.10.
+[#60](https://github.com/CUNY-CL/yoyodyne/issues/60) is a known blocker to
+Python \> 3.10 support.
 
 First install dependencies:
 
     pip install -r requirements.txt
 
 Then install:
 
     pip install .
 
 It can then be imported like a regular Python module:
 
-``` python
+```python
 import yoyodyne
 ```
 
+### Google Colab
+
+Yoyodyne is compatible with [Google Colab](https://colab.research.google.com/)
+GPU runtimes. [This
+notebook](https://colab.research.google.com/drive/1O4VWvpqLrCxxUvyYMbGH9HOyXQSoh5bP?usp=sharing)
+provides a worked example. Colab also provides access to TPU runtimes, but this
+is not yet compatible with Yoyodyne to our knowledge.
+
 ## Usage
 
 ### Training
 
 Training is performed by the [`yoyodyne-train`](yoyodyne/train.py) script. One
 must specify the following required arguments:
```

### Comparing `yoyodyne-0.2.8/pyproject.toml` & `yoyodyne-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.packages.find]
 include = ["yoyodyne*"]
 exclude = ["examples*"]
 
 [project]
 name = "yoyodyne"
-version = "0.2.8"
+version = "0.2.9"
 description = "Small-vocabulary neural sequence-to-sequence models"
 readme = "README.md"
 requires-python = ">= 3.9"
 license = { text = "Apache 2.0" }
 authors = [
     {name = "Adam Wiemerslage"},
     {name = "Kyle Gorman"},
```

### Comparing `yoyodyne-0.2.8/yoyodyne/data/__init__.py` & `yoyodyne-0.2.9/yoyodyne/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/data/batches.py` & `yoyodyne-0.2.9/yoyodyne/data/batches.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/data/collators.py` & `yoyodyne-0.2.9/yoyodyne/data/collators.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/data/datamodules.py` & `yoyodyne-0.2.9/yoyodyne/data/datamodules.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Data modules."""
 
-from typing import Iterator, Optional, Set
+from typing import Optional, Set
 
 import pytorch_lightning as pl
 from torch.utils import data
 
 from .. import defaults, util
 from . import collators, datasets, indexes, tsv
 
@@ -59,67 +59,55 @@
         self.separate_features = separate_features
         self.index = index if index is not None else self._make_index()
         self.collator = collators.Collator(
             pad_idx=self.index.pad_idx,
             has_features=self.has_features,
             has_target=self.has_target,
             separate_features=separate_features,
-            features_offset=self.index.source_vocab_size
-            if self.has_features
-            else 0,
+            features_offset=(
+                self.index.source_vocab_size if self.has_features else 0
+            ),
             max_source_length=max_source_length,
             max_target_length=max_target_length,
         )
 
     def _make_index(self) -> indexes.Index:
         # Computes index.
         source_vocabulary: Set[str] = set()
         features_vocabulary: Set[str] = set()
         target_vocabulary: Set[str] = set()
-        for path in self.paths:
-            if self.has_features:
-                if self.has_target:
-                    for source, features, target in self.parser.samples(path):
-                        source_vocabulary.update(source)
-                        features_vocabulary.update(features)
-                        target_vocabulary.update(target)
-                else:
-                    for source, features in self.parser.samples(path):
-                        source_vocabulary.update(source)
-                        features_vocabulary.update(features)
-            elif self.has_target:
-                for source, target in self.parser.samples(path):
+        if self.has_features:
+            if self.has_target:
+                for source, features, target in self.parser.samples(
+                    self.train
+                ):
                     source_vocabulary.update(source)
+                    features_vocabulary.update(features)
                     target_vocabulary.update(target)
             else:
-                for source in self.parser.samples(path):
+                for source, features in self.parser.samples(self.train):
                     source_vocabulary.update(source)
+                    features_vocabulary.update(features)
+        elif self.has_target:
+            for source, target in self.parser.samples(self.train):
+                source_vocabulary.update(source)
+                target_vocabulary.update(target)
+        else:
+            for source in self.parser.samples(self.train):
+                source_vocabulary.update(source)
         return indexes.Index(
             source_vocabulary=sorted(source_vocabulary),
-            features_vocabulary=sorted(features_vocabulary)
-            if features_vocabulary
-            else None,
-            target_vocabulary=sorted(target_vocabulary)
-            if target_vocabulary
-            else None,
+            features_vocabulary=(
+                sorted(features_vocabulary) if features_vocabulary else None
+            ),
+            target_vocabulary=(
+                sorted(target_vocabulary) if target_vocabulary else None
+            ),
         )
 
-    # Helpers.
-
-    @property
-    def paths(self) -> Iterator[str]:
-        if self.train is not None:
-            yield self.train
-        if self.val is not None:
-            yield self.val
-        if self.predict is not None:
-            yield self.predict
-        if self.test is not None:
-            yield self.test
-
     def log_vocabularies(self) -> None:
         """Logs this module's vocabularies."""
         util.log_info(f"Source vocabulary: {self.index.source_map.pprint()}")
         if self.has_features:
             util.log_info(
                 f"Features vocabulary: {self.index.features_map.pprint()}"
             )
```

### Comparing `yoyodyne-0.2.8/yoyodyne/data/datasets.py` & `yoyodyne-0.2.9/yoyodyne/data/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
         Args:
             symbols (List[str]).
 
         Returns:
             torch.Tensor.
         """
-        wrapped = symbols
+        wrapped = symbols.copy()
         wrapped.append(special.END)
         return self._encode(wrapped, self.index.target_map)
 
     # Decoding.
 
     def _decode(
         self,
```

### Comparing `yoyodyne-0.2.8/yoyodyne/data/indexes.py` & `yoyodyne-0.2.9/yoyodyne/data/indexes.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/data/tsv.py` & `yoyodyne-0.2.9/yoyodyne/data/tsv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """TSV parsing.
 
 The TsvParser yields data from TSV files using 1-based indexing and custom
 separators.
 """
 
-
 import csv
 import dataclasses
 from typing import Iterator, List, Tuple, Union
 
 from .. import defaults
 
 
@@ -77,17 +76,15 @@
     def has_features(self) -> bool:
         return self.features_col != 0
 
     @property
     def has_target(self) -> bool:
         return self.target_col != 0
 
-    def samples(
-        self, path: str
-    ) -> Iterator[
+    def samples(self, path: str) -> Iterator[
         Union[
             List[str],
             Tuple[List[str], List[str]],
             Tuple[List[str], List[str], List[str]],
         ]
     ]:
         """Yields source, and features and/or target if available."""
```

### Comparing `yoyodyne-0.2.8/yoyodyne/defaults.py` & `yoyodyne-0.2.9/yoyodyne/defaults.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/evaluators.py` & `yoyodyne-0.2.9/yoyodyne/evaluators.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/models/__init__.py` & `yoyodyne-0.2.9/yoyodyne/models/__init__.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/models/base.py` & `yoyodyne-0.2.9/yoyodyne/models/base.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/models/expert.py` & `yoyodyne-0.2.9/yoyodyne/models/expert.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 Also includes ActionVocabulary class for compatibility with maxwell dictionary.
 Class stores valid edit actions for given dataset.
 """
 
 import abc
 import argparse
 import dataclasses
+
 from typing import Any, Dict, Iterable, Iterator, List, Sequence, Set, Tuple
 
 import numpy
 from maxwell import actions, sed
 from torch.utils import data
-
 from .. import defaults
 
 
-class Error(Exception):
+class ActionError(Exception):
     pass
 
 
 class ActionVocabulary:
     """Manages encoding of action vocabulary for transducer training."""
 
     # TODO: Port more of the logic to the dataset class.
@@ -90,15 +90,18 @@
             self.target_characters.add(c)
 
     def encode_unseen_action(self, action: actions.Edit) -> int:
         """Encodes action unseen in training.
 
         Operates same as encode_action but does not expand lookup table.
         """
-        return self.lookup(action)
+        if action in self.w2i:
+            return self.lookup(action)
+        else:
+            raise ActionError(f"Action {action} is out of vocabulary")
 
     def __len__(self) -> int:
         return len(self.i2w)
 
     def __repr__(self) -> str:
         return f"Vocabulary({str(self.w2i)})"
 
@@ -328,15 +331,15 @@
                 elif isinstance(action, actions.Sub):
                     s_offset = alignment + 1
                     t_offset = suffix_begin + 1
                 elif isinstance(action, actions.End):
                     s_offset = alignment
                     t_offset = suffix_begin
                 else:
-                    raise Error(f"Unknown action: {action}")
+                    raise ActionError(f"Unknown action: {action}")
                 sequence_cost = self.aligner.action_sequence_cost(
                     source, target, s_offset, t_offset
                 )
                 action_cost = self.aligner.action_cost(action)
                 cost = action_cost + sequence_cost
                 if action not in costs_to_go or costs_to_go[action] > cost:
                     costs_to_go[action] = cost
```

### Comparing `yoyodyne-0.2.8/yoyodyne/models/lstm.py` & `yoyodyne-0.2.9/yoyodyne/models/lstm.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/models/modules/__init__.py` & `yoyodyne-0.2.9/yoyodyne/models/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/models/modules/attention.py` & `yoyodyne-0.2.9/yoyodyne/models/modules/attention.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/models/modules/base.py` & `yoyodyne-0.2.9/yoyodyne/models/modules/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,9 +152,8 @@
             embedded (torch.Tensor): embedded tensor of shape
                 B x seq_len x embed_dim.
         """
         embedded = self.embeddings(symbols)
         return self.dropout_layer(embedded)
 
     @property
-    def output_size(self) -> int:
-        ...
+    def output_size(self) -> int: ...
```

### Comparing `yoyodyne-0.2.8/yoyodyne/models/modules/linear.py` & `yoyodyne-0.2.9/yoyodyne/models/modules/linear.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/models/modules/lstm.py` & `yoyodyne-0.2.9/yoyodyne/models/modules/lstm.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/models/modules/transformer.py` & `yoyodyne-0.2.9/yoyodyne/models/modules/transformer.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/models/pointer_generator.py` & `yoyodyne-0.2.9/yoyodyne/models/pointer_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,18 +194,20 @@
             )
 
     def get_decoder(self) -> modules.lstm.LSTMAttentiveDecoder:
         return modules.lstm.LSTMAttentiveDecoder(
             pad_idx=self.pad_idx,
             start_idx=self.start_idx,
             end_idx=self.end_idx,
-            decoder_input_size=self.source_encoder.output_size
-            + self.features_encoder.output_size
-            if self.has_features_encoder
-            else self.source_encoder.output_size,
+            decoder_input_size=(
+                self.source_encoder.output_size
+                + self.features_encoder.output_size
+                if self.has_features_encoder
+                else self.source_encoder.output_size
+            ),
             num_embeddings=self.target_vocab_size,
             dropout=self.dropout,
             bidirectional=False,
             embedding_size=self.embedding_size,
             layers=self.decoder_layers,
             hidden_size=self.hidden_size,
             attention_input_size=self.source_encoder.output_size,
```

### Comparing `yoyodyne-0.2.8/yoyodyne/models/transducer.py` & `yoyodyne-0.2.9/yoyodyne/models/transducer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 from maxwell import actions
 from torch import nn
 
 from .. import data
 from . import expert, lstm, modules
 
 
-class ActionError(Exception):
-    pass
-
-
 class TransducerEncoderDecoder(lstm.LSTMEncoderDecoder):
     """Transducer model with an LSTM backend.
 
     After:
         Makarov, P., and Clematide, S. 2018. Imitation learning for neural
         morphological string transduction. In Proceedings of the 2018
         Conference on Empirical Methods in Natural Language Processing, pages
@@ -53,18 +49,20 @@
         self.insertions = self.actions.insertions
 
     def get_decoder(self) -> modules.lstm.LSTMDecoder:
         return modules.lstm.LSTMDecoder(
             pad_idx=self.pad_idx,
             start_idx=self.start_idx,
             end_idx=self.end_idx,
-            decoder_input_size=self.source_encoder.output_size
-            + self.features_encoder.output_size
-            if self.has_features_encoder
-            else self.source_encoder.output_size,
+            decoder_input_size=(
+                self.source_encoder.output_size
+                + self.features_encoder.output_size
+                if self.has_features_encoder
+                else self.source_encoder.output_size
+            ),
             num_embeddings=self.target_vocab_size,
             dropout=self.dropout,
             bidirectional=False,
             embedding_size=self.embedding_size,
             layers=self.decoder_layers,
             hidden_size=self.hidden_size,
         )
@@ -367,15 +365,15 @@
         remapped_action_scores = {}
         for action, score in action_scores.items():
             if isinstance(action, actions.GenerativeEdit):
                 remapped_action = action.conditional_counterpart()
             elif isinstance(action, actions.Edit):
                 remapped_action = action
             else:
-                raise ActionError(
+                raise expert.ActionError(
                     f"Unknown action: {action}, {score}, "
                     f"action_scores: {action_scores}"
                 )
             remapped_action_scores[remapped_action] = score
         return remapped_action_scores
 
     def expert_rollout(
@@ -420,17 +418,19 @@
         target: List[List[int]],
         alignment: torch.Tensor,
         prediction: List[List[int]],
         not_complete: torch.Tensor,
     ) -> List[List[int]]:
         """Performs expert rollout over batch."""
         return [
-            self.expert_rollout(s, t, align, pred)
-            if nc
-            else self.actions.end_idx
+            (
+                self.expert_rollout(s, t, align, pred)
+                if nc
+                else self.actions.end_idx
+            )
             for s, t, align, pred, nc in zip(
                 source, target, alignment, prediction, not_complete
             )
         ]
 
     def update_prediction(
         self,
@@ -467,15 +467,15 @@
                 prediction[i].append(a.new)
             elif isinstance(a, actions.ConditionalSub):
                 alignment_update[i] += 1
                 prediction[i].append(a.new)
             elif isinstance(a, actions.End):
                 prediction[i].append(self.end_idx)
             else:
-                raise ActionError(f"Unknown action: {action[i]}")
+                raise expert.ActionError(f"Unknown action: {action[i]}")
         return alignment + alignment_update
 
     @staticmethod
     def log_sum_softmax_loss(
         logits: torch.Tensor, optimal_actions: List[int]
     ) -> torch.Tensor:
         """Computes log loss.
@@ -493,15 +493,15 @@
         log_sum_exp_terms = torch.stack(
             [torch.logsumexp(act, dim=-1) for act in opt_act]
         )
         normalization_term = torch.logsumexp(logits, -1)
         return log_sum_exp_terms - normalization_term
 
     def _get_loss_func(
-        self, reduction: str
+        self,
     ) -> Callable[[torch.Tensor, torch.Tensor], torch.Tensor]:
         # Prevents base construction of unused loss function.
         return None
 
     def training_step(self, batch: data.PaddedBatch, batch_idx: int) -> Dict:
         """Runs one step of training.
```

### Comparing `yoyodyne-0.2.8/yoyodyne/models/transformer.py` & `yoyodyne-0.2.9/yoyodyne/models/transformer.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/predict.py` & `yoyodyne-0.2.9/yoyodyne/predict.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/schedulers.py` & `yoyodyne-0.2.9/yoyodyne/schedulers.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne/train.py` & `yoyodyne-0.2.9/yoyodyne/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,21 +23,19 @@
         log_wandb (bool).
 
     Returns:
         List: logger.
     """
     trainer_logger = [loggers.CSVLogger(model_dir, name=experiment)]
     if log_wandb:
-        trainer_logger.append(
-            loggers.WandbLogger(project=experiment, log_model="all")
-        )
-        # Tells PTL to log best validation acc
+        trainer_logger.append(loggers.WandbLogger(project=experiment))
+        # Tells PTL to log the best validation accuracy.
         wandb.define_metric("val_accuracy", summary="max")
         # Logs the path to local artifacts made by PTL.
-        wandb.config.update({"local_run_dir": trainer_logger[0].log_dir})
+        wandb.config["local_run_dir"] = trainer_logger[0].log_dir
     return trainer_logger
 
 
 def _get_callbacks(save_top_k: int, patience: Optional[int] = None) -> List:
     """Creates the callbacks.
 
     We will reach into the callback metrics list to picks ckp_callback to find
```

### Comparing `yoyodyne-0.2.8/yoyodyne/util.py` & `yoyodyne-0.2.9/yoyodyne/util.py`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.8/yoyodyne.egg-info/PKG-INFO` & `yoyodyne-0.2.9/yoyodyne.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoyodyne
-Version: 0.2.8
+Version: 0.2.9
 Summary: Small-vocabulary neural sequence-to-sequence models
 Author: Adam Wiemerslage, Kyle Gorman, Travis Bartley
 License: Apache 2.0
 Project-URL: homepage, https://github.com/CUNY-CL/yoyodyne
 Keywords: computational linguistics,morphology,natural language processing,language
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -55,30 +55,44 @@
     architecture-specific code to handle feature information.
 -   It uses validation accuracy (not loss) for model selection and early
     stopping.
 -   Releases are made regularly.
 -   🚧 UNDER CONSTRUCTION 🚧: It has exhaustive test suites.
 -   🚧 UNDER CONSTRUCTION 🚧: It has performance benchmarks.
 
-## Install
+## Installation
+
+### Local installation
+
+Yoyodyne currently supports Python 3.9 and 3.10.
+[#60](https://github.com/CUNY-CL/yoyodyne/issues/60) is a known blocker to
+Python \> 3.10 support.
 
 First install dependencies:
 
     pip install -r requirements.txt
 
 Then install:
 
     pip install .
 
 It can then be imported like a regular Python module:
 
-``` python
+```python
 import yoyodyne
 ```
 
+### Google Colab
+
+Yoyodyne is compatible with [Google Colab](https://colab.research.google.com/)
+GPU runtimes. [This
+notebook](https://colab.research.google.com/drive/1O4VWvpqLrCxxUvyYMbGH9HOyXQSoh5bP?usp=sharing)
+provides a worked example. Colab also provides access to TPU runtimes, but this
+is not yet compatible with Yoyodyne to our knowledge.
+
 ## Usage
 
 ### Training
 
 Training is performed by the [`yoyodyne-train`](yoyodyne/train.py) script. One
 must specify the following required arguments:
```

### Comparing `yoyodyne-0.2.8/yoyodyne.egg-info/SOURCES.txt` & `yoyodyne-0.2.9/yoyodyne.egg-info/SOURCES.txt`

 * *Files identical despite different names*


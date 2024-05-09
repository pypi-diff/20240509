# Comparing `tmp/Procpath-1.9.0.tar.gz` & `tmp/Procpath-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Procpath-1.9.0.tar", last modified: Thu Oct 26 17:25:47 2023, max compression
+gzip compressed data, was "Procpath-1.9.1.tar", last modified: Thu Feb 15 20:23:38 2024, max compression
```

## Comparing `Procpath-1.9.0.tar` & `Procpath-1.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-10-26 17:25:47.767924 Procpath-1.9.0/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5595 2023-10-26 17:25:47.767924 Procpath-1.9.0/PKG-INFO
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-10-26 17:25:47.751924 Procpath-1.9.0/Procpath.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5595 2023-10-26 17:25:47.000000 Procpath-1.9.0/Procpath.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      590 2023-10-26 17:25:47.000000 Procpath-1.9.0/Procpath.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2023-10-26 17:25:47.000000 Procpath-1.9.0/Procpath.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       47 2023-10-26 17:25:47.000000 Procpath-1.9.0/Procpath.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      155 2023-10-26 17:25:47.000000 Procpath-1.9.0/Procpath.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        9 2023-10-26 17:25:47.000000 Procpath-1.9.0/Procpath.egg-info/top_level.txt
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     4013 2023-10-26 17:09:58.000000 Procpath-1.9.0/README.rst
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-10-26 17:25:47.759924 Procpath-1.9.0/procpath/
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)       22 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/__init__.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)       62 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/__main__.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    16708 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/cli.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2023-10-26 17:25:47.763924 Procpath-1.9.0/procpath/cmd/
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)      408 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/cmd/__init__.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    12816 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/cmd/explore.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1482 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/cmd/play.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     3283 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/cmd/plot.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1588 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/cmd/query.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1887 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/cmd/record.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     5303 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/cmd/watch.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     8090 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/playbook.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    18994 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/plotting.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    27763 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/procfile.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     2860 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/procrec.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     7887 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/procret.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     8987 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/proctree.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)   192430 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/test.py
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1388 2023-10-26 17:09:58.000000 Procpath-1.9.0/procpath/utility.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2023-10-26 17:25:47.767924 Procpath-1.9.0/setup.cfg
--rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     2048 2023-10-26 17:09:58.000000 Procpath-1.9.0/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-02-15 20:23:38.981723 Procpath-1.9.1/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5558 2024-02-15 20:23:38.981723 Procpath-1.9.1/PKG-INFO
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-02-15 20:23:38.981723 Procpath-1.9.1/Procpath.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5558 2024-02-15 20:23:38.000000 Procpath-1.9.1/Procpath.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      590 2024-02-15 20:23:38.000000 Procpath-1.9.1/Procpath.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2024-02-15 20:23:38.000000 Procpath-1.9.1/Procpath.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       47 2024-02-15 20:23:38.000000 Procpath-1.9.1/Procpath.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      130 2024-02-15 20:23:38.000000 Procpath-1.9.1/Procpath.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        9 2024-02-15 20:23:38.000000 Procpath-1.9.1/Procpath.egg-info/top_level.txt
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     4013 2024-02-15 20:06:27.000000 Procpath-1.9.1/README.rst
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-02-15 20:23:38.977723 Procpath-1.9.1/procpath/
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)       22 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/__init__.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)       62 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/__main__.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    16708 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/cli.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-02-15 20:23:38.981723 Procpath-1.9.1/procpath/cmd/
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)      408 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/cmd/__init__.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    12816 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/cmd/explore.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1482 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/cmd/play.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     3283 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/cmd/plot.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1588 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/cmd/query.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1887 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/cmd/record.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     5303 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/cmd/watch.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     8090 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/playbook.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    18994 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/plotting.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)    27763 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/procfile.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     2860 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/procrec.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     7887 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/procret.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     8987 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/proctree.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)   192430 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/test.py
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     1388 2024-02-15 20:06:27.000000 Procpath-1.9.1/procpath/utility.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2024-02-15 20:23:38.981723 Procpath-1.9.1/setup.cfg
+-rw-rw-rw-   0 nobody   (65534) nogroup  (65534)     2018 2024-02-15 20:06:27.000000 Procpath-1.9.1/setup.py
```

### Comparing `Procpath-1.9.0/PKG-INFO` & `Procpath-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Procpath
-Version: 1.9.0
+Version: 1.9.1
 Summary: Procpath is a process tree analysis workbench
 Home-page: https://heptapod.host/saajns/procpath
 Author: saaj
 Author-email: mail@saaj.me
 License: LGPL-3.0-only
 Project-URL: Source Code, https://heptapod.host/saajns/procpath
 Project-URL: Documentation, https://procpath.readthedocs.io/
@@ -23,20 +23,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >= 3.8
 Requires-Dist: jsonpyth<0.2,>=0.1.3
-Requires-Dist: pygal<4,>=3.0.0
-Requires-Dist: setuptools; python_version >= "3.12"
+Requires-Dist: pygal<4,>=3.0.4
 Provides-Extra: manual
-Requires-Dist: sphinx<5,>=4; extra == "manual"
-Requires-Dist: sphinxcontrib-programoutput<0.18; extra == "manual"
-Requires-Dist: sphinx-copybutton<0.6; extra == "manual"
+Requires-Dist: sphinx<6,>=5; extra == "manual"
+Requires-Dist: sphinxcontrib-programoutput<0.18,>=0.17; extra == "manual"
+Requires-Dist: sphinx-copybutton<0.6,>=0.5.2; extra == "manual"
 
 .. image:: https://img.shields.io/pypi/l/Procpath.svg
    :target: https://spdx.org/licenses/LGPL-3.0-only.html
    :alt: PyPI - License
 .. image:: https://heptapod.host/saajns/procpath/badges/branch/default/pipeline.svg
    :target: https://heptapod.host/saajns/procpath/-/commits/branch/default
    :alt: Pipeline status
```

### Comparing `Procpath-1.9.0/Procpath.egg-info/PKG-INFO` & `Procpath-1.9.1/Procpath.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Procpath
-Version: 1.9.0
+Version: 1.9.1
 Summary: Procpath is a process tree analysis workbench
 Home-page: https://heptapod.host/saajns/procpath
 Author: saaj
 Author-email: mail@saaj.me
 License: LGPL-3.0-only
 Project-URL: Source Code, https://heptapod.host/saajns/procpath
 Project-URL: Documentation, https://procpath.readthedocs.io/
@@ -23,20 +23,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >= 3.8
 Requires-Dist: jsonpyth<0.2,>=0.1.3
-Requires-Dist: pygal<4,>=3.0.0
-Requires-Dist: setuptools; python_version >= "3.12"
+Requires-Dist: pygal<4,>=3.0.4
 Provides-Extra: manual
-Requires-Dist: sphinx<5,>=4; extra == "manual"
-Requires-Dist: sphinxcontrib-programoutput<0.18; extra == "manual"
-Requires-Dist: sphinx-copybutton<0.6; extra == "manual"
+Requires-Dist: sphinx<6,>=5; extra == "manual"
+Requires-Dist: sphinxcontrib-programoutput<0.18,>=0.17; extra == "manual"
+Requires-Dist: sphinx-copybutton<0.6,>=0.5.2; extra == "manual"
 
 .. image:: https://img.shields.io/pypi/l/Procpath.svg
    :target: https://spdx.org/licenses/LGPL-3.0-only.html
    :alt: PyPI - License
 .. image:: https://heptapod.host/saajns/procpath/badges/branch/default/pipeline.svg
    :target: https://heptapod.host/saajns/procpath/-/commits/branch/default
    :alt: Pipeline status
```

### Comparing `Procpath-1.9.0/Procpath.egg-info/SOURCES.txt` & `Procpath-1.9.1/Procpath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/README.rst` & `Procpath-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/cli.py` & `Procpath-1.9.1/procpath/cli.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/cmd/explore.py` & `Procpath-1.9.1/procpath/cmd/explore.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/cmd/play.py` & `Procpath-1.9.1/procpath/cmd/play.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/cmd/plot.py` & `Procpath-1.9.1/procpath/cmd/plot.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/cmd/query.py` & `Procpath-1.9.1/procpath/cmd/query.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/cmd/record.py` & `Procpath-1.9.1/procpath/cmd/record.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/cmd/watch.py` & `Procpath-1.9.1/procpath/cmd/watch.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/playbook.py` & `Procpath-1.9.1/procpath/playbook.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/plotting.py` & `Procpath-1.9.1/procpath/plotting.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/procfile.py` & `Procpath-1.9.1/procpath/procfile.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/procrec.py` & `Procpath-1.9.1/procpath/procrec.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/procret.py` & `Procpath-1.9.1/procpath/procret.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/proctree.py` & `Procpath-1.9.1/procpath/proctree.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/test.py` & `Procpath-1.9.1/procpath/test.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/procpath/utility.py` & `Procpath-1.9.1/procpath/utility.py`

 * *Files identical despite different names*

### Comparing `Procpath-1.9.0/setup.py` & `Procpath-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,18 +36,17 @@
         'Programming Language :: Python :: Implementation :: PyPy',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
     ],
     entry_points     = {'console_scripts': ['procpath = procpath.cli:main']},
     install_requires = [
         'jsonpyth >= 0.1.3, < 0.2',
-        'pygal >= 3.0.0, < 4',
-        'setuptools; python_version >= "3.12"',
+        'pygal >= 3.0.4, < 4',
     ],
     extras_require = {
         'manual' : [
-            'sphinx >= 4, < 5',
-            'sphinxcontrib-programoutput < 0.18',
-            'sphinx-copybutton < 0.6',
+            'sphinx >= 5, < 6',
+            'sphinxcontrib-programoutput >= 0.17, < 0.18',
+            'sphinx-copybutton >=0.5.2, < 0.6',
         ],
     },
 )
```


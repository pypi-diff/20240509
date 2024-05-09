# Comparing `tmp/pyflyde-0.0.4.tar.gz` & `tmp/pyflyde-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyflyde-0.0.4.tar", last modified: Thu May  9 19:02:08 2024, max compression
+gzip compressed data, was "pyflyde-0.0.5.tar", last modified: Thu May  9 19:27:00 2024, max compression
```

## Comparing `pyflyde-0.0.4.tar` & `pyflyde-0.0.5.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:02:08.434817 pyflyde-0.0.4/
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:02:08.323567 pyflyde-0.0.4/.github/
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:02:08.340132 pyflyde-0.0.4/.github/workflows/
--rw-r--r--   0 trustmaster   (501) staff       (20)      984 2024-05-09 11:09:26.000000 pyflyde-0.0.4/.github/workflows/python-package.yml
--rw-r--r--   0 trustmaster   (501) staff       (20)     3197 2024-05-09 10:46:21.000000 pyflyde-0.0.4/.gitignore
--rw-r--r--   0 trustmaster   (501) staff       (20)    11345 2024-04-09 17:14:23.000000 pyflyde-0.0.4/LICENSE
--rw-r--r--   0 trustmaster   (501) staff       (20)     1047 2024-05-09 19:01:54.000000 pyflyde-0.0.4/Makefile
--rw-r--r--   0 trustmaster   (501) staff       (20)    16063 2024-05-09 19:02:08.433505 pyflyde-0.0.4/PKG-INFO
--rw-r--r--   0 trustmaster   (501) staff       (20)     1887 2024-05-09 16:21:19.000000 pyflyde-0.0.4/README.md
--rw-r--r--   0 trustmaster   (501) staff       (20)   265919 2024-05-09 10:46:21.000000 pyflyde-0.0.4/clustering_example.png
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:02:08.347012 pyflyde-0.0.4/examples/
--rw-r--r--   0 trustmaster   (501) staff       (20)     4489 2024-05-09 10:46:21.000000 pyflyde-0.0.4/examples/Clustering.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)      991 2024-04-09 17:14:23.000000 pyflyde-0.0.4/examples/HelloPy.flyde
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:02:08.353196 pyflyde-0.0.4/examples/datasets/
--rw-r--r--   0 trustmaster   (501) staff       (20)    11089 2024-04-09 17:14:23.000000 pyflyde-0.0.4/examples/datasets/wine-clustering.csv
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:02:08.367460 pyflyde-0.0.4/examples/mylib/
--rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:14:23.000000 pyflyde-0.0.4/examples/mylib/__init__.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      560 2024-04-21 06:51:36.000000 pyflyde-0.0.4/examples/mylib/components.flyde.ts
--rw-r--r--   0 trustmaster   (501) staff       (20)      725 2024-04-13 14:14:04.000000 pyflyde-0.0.4/examples/mylib/components.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      684 2024-05-09 10:46:21.000000 pyflyde-0.0.4/examples/mylib/dataframe.flyde.ts
--rw-r--r--   0 trustmaster   (501) staff       (20)     1353 2024-05-09 10:46:21.000000 pyflyde-0.0.4/examples/mylib/dataframe.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     1619 2024-04-09 17:14:23.000000 pyflyde-0.0.4/examples/mylib/kmeans.flyde.ts
--rw-r--r--   0 trustmaster   (501) staff       (20)     6171 2024-05-06 19:18:33.000000 pyflyde-0.0.4/examples/mylib/kmeans.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      216 2024-04-09 17:14:23.000000 pyflyde-0.0.4/examples/pyproject.toml
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:02:08.388664 pyflyde-0.0.4/flyde/
--rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:14:23.000000 pyflyde-0.0.4/flyde/__init__.py
--rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:01:16.000000 pyflyde-0.0.4/flyde/__init__.pyi
--rw-r--r--   0 trustmaster   (501) staff       (20)     4559 2024-05-09 10:46:21.000000 pyflyde-0.0.4/flyde/flow.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      679 2024-05-09 19:02:00.000000 pyflyde-0.0.4/flyde/flow.pyi
--rw-r--r--   0 trustmaster   (501) staff       (20)     9925 2024-05-09 10:46:21.000000 pyflyde-0.0.4/flyde/io.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     2182 2024-05-09 19:02:00.000000 pyflyde-0.0.4/flyde/io.pyi
--rw-r--r--   0 trustmaster   (501) staff       (20)    17280 2024-05-09 10:46:21.000000 pyflyde-0.0.4/flyde/node.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     2115 2024-05-09 19:02:00.000000 pyflyde-0.0.4/flyde/node.pyi
--rw-r--r--   0 trustmaster   (501) staff       (20)     1670 2024-05-09 10:46:21.000000 pyflyde-0.0.4/flyde/stdlib.py
--rw-r--r--   0 trustmaster   (501) staff       (20)      500 2024-05-09 19:02:00.000000 pyflyde-0.0.4/flyde/stdlib.pyi
--rwxr-xr-x   0 trustmaster   (501) staff       (20)     2217 2024-05-04 13:30:20.000000 pyflyde-0.0.4/flyde.py
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:02:08.429828 pyflyde-0.0.4/pyflyde.egg-info/
--rw-r--r--   0 trustmaster   (501) staff       (20)    16063 2024-05-09 19:02:08.000000 pyflyde-0.0.4/pyflyde.egg-info/PKG-INFO
--rw-r--r--   0 trustmaster   (501) staff       (20)      995 2024-05-09 19:02:08.000000 pyflyde-0.0.4/pyflyde.egg-info/SOURCES.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 19:02:08.000000 pyflyde-0.0.4/pyflyde.egg-info/dependency_links.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)       64 2024-05-09 19:02:08.000000 pyflyde-0.0.4/pyflyde.egg-info/requires.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)        6 2024-05-09 19:02:08.000000 pyflyde-0.0.4/pyflyde.egg-info/top_level.txt
--rw-r--r--   0 trustmaster   (501) staff       (20)     1229 2024-05-09 18:55:49.000000 pyflyde-0.0.4/pyproject.toml
--rw-r--r--   0 trustmaster   (501) staff       (20)       38 2024-05-09 19:02:08.435029 pyflyde-0.0.4/setup.cfg
-drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:02:08.428996 pyflyde-0.0.4/tests/
--rw-r--r--   0 trustmaster   (501) staff       (20)     1744 2024-05-09 10:46:21.000000 pyflyde-0.0.4/tests/Repeat3Times.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)      782 2024-04-25 19:45:07.000000 pyflyde-0.0.4/tests/TestInOutFlow.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)      820 2024-04-24 22:56:30.000000 pyflyde-0.0.4/tests/TestIsolatedFlow.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)     1798 2024-05-09 10:46:21.000000 pyflyde-0.0.4/tests/TestNestedFlow.flyde
--rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:26:09.000000 pyflyde-0.0.4/tests/__init.py__
--rw-r--r--   0 trustmaster   (501) staff       (20)      914 2024-05-09 10:46:21.000000 pyflyde-0.0.4/tests/components.flyde.ts
--rw-r--r--   0 trustmaster   (501) staff       (20)     1185 2024-05-09 10:46:21.000000 pyflyde-0.0.4/tests/components.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     1933 2024-05-09 10:46:21.000000 pyflyde-0.0.4/tests/test_flow.py
--rw-r--r--   0 trustmaster   (501) staff       (20)    10544 2024-05-09 10:46:21.000000 pyflyde-0.0.4/tests/test_io.py
--rw-r--r--   0 trustmaster   (501) staff       (20)    11312 2024-05-09 10:46:21.000000 pyflyde-0.0.4/tests/test_node.py
--rw-r--r--   0 trustmaster   (501) staff       (20)     3754 2024-05-09 10:46:21.000000 pyflyde-0.0.4/tests/test_stdlib.py
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:27:00.182430 pyflyde-0.0.5/
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:27:00.016230 pyflyde-0.0.5/.github/
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:27:00.041649 pyflyde-0.0.5/.github/workflows/
+-rw-r--r--   0 trustmaster   (501) staff       (20)      984 2024-05-09 11:09:26.000000 pyflyde-0.0.5/.github/workflows/python-package.yml
+-rw-r--r--   0 trustmaster   (501) staff       (20)     3197 2024-05-09 10:46:21.000000 pyflyde-0.0.5/.gitignore
+-rw-r--r--   0 trustmaster   (501) staff       (20)    11345 2024-04-09 17:14:23.000000 pyflyde-0.0.5/LICENSE
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1047 2024-05-09 19:01:54.000000 pyflyde-0.0.5/Makefile
+-rw-r--r--   0 trustmaster   (501) staff       (20)    16063 2024-05-09 19:27:00.180888 pyflyde-0.0.5/PKG-INFO
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1887 2024-05-09 16:21:19.000000 pyflyde-0.0.5/README.md
+-rw-r--r--   0 trustmaster   (501) staff       (20)   265919 2024-05-09 10:46:21.000000 pyflyde-0.0.5/clustering_example.png
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:27:00.053441 pyflyde-0.0.5/examples/
+-rw-r--r--   0 trustmaster   (501) staff       (20)     4489 2024-05-09 10:46:21.000000 pyflyde-0.0.5/examples/Clustering.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)      991 2024-04-09 17:14:23.000000 pyflyde-0.0.5/examples/HelloPy.flyde
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:27:00.055204 pyflyde-0.0.5/examples/datasets/
+-rw-r--r--   0 trustmaster   (501) staff       (20)    11089 2024-04-09 17:14:23.000000 pyflyde-0.0.5/examples/datasets/wine-clustering.csv
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:27:00.072106 pyflyde-0.0.5/examples/mylib/
+-rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:14:23.000000 pyflyde-0.0.5/examples/mylib/__init__.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)      560 2024-04-21 06:51:36.000000 pyflyde-0.0.5/examples/mylib/components.flyde.ts
+-rw-r--r--   0 trustmaster   (501) staff       (20)      725 2024-04-13 14:14:04.000000 pyflyde-0.0.5/examples/mylib/components.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)      684 2024-05-09 10:46:21.000000 pyflyde-0.0.5/examples/mylib/dataframe.flyde.ts
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1353 2024-05-09 10:46:21.000000 pyflyde-0.0.5/examples/mylib/dataframe.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1619 2024-04-09 17:14:23.000000 pyflyde-0.0.5/examples/mylib/kmeans.flyde.ts
+-rw-r--r--   0 trustmaster   (501) staff       (20)     6171 2024-05-06 19:18:33.000000 pyflyde-0.0.5/examples/mylib/kmeans.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)      216 2024-04-09 17:14:23.000000 pyflyde-0.0.5/examples/pyproject.toml
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:27:00.104954 pyflyde-0.0.5/flyde/
+-rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:14:23.000000 pyflyde-0.0.5/flyde/__init__.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:01:16.000000 pyflyde-0.0.5/flyde/__init__.pyi
+-rw-r--r--   0 trustmaster   (501) staff       (20)     4559 2024-05-09 10:46:21.000000 pyflyde-0.0.5/flyde/flow.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)      679 2024-05-09 19:26:45.000000 pyflyde-0.0.5/flyde/flow.pyi
+-rw-r--r--   0 trustmaster   (501) staff       (20)     9925 2024-05-09 10:46:21.000000 pyflyde-0.0.5/flyde/io.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     2182 2024-05-09 19:26:45.000000 pyflyde-0.0.5/flyde/io.pyi
+-rw-r--r--   0 trustmaster   (501) staff       (20)    17280 2024-05-09 10:46:21.000000 pyflyde-0.0.5/flyde/node.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     2115 2024-05-09 19:26:45.000000 pyflyde-0.0.5/flyde/node.pyi
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1670 2024-05-09 10:46:21.000000 pyflyde-0.0.5/flyde/stdlib.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)      500 2024-05-09 19:26:45.000000 pyflyde-0.0.5/flyde/stdlib.pyi
+-rwxr-xr-x   0 trustmaster   (501) staff       (20)     2217 2024-05-04 13:30:20.000000 pyflyde-0.0.5/flyde.py
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:27:00.172173 pyflyde-0.0.5/pyflyde.egg-info/
+-rw-r--r--   0 trustmaster   (501) staff       (20)    16063 2024-05-09 19:26:59.000000 pyflyde-0.0.5/pyflyde.egg-info/PKG-INFO
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1029 2024-05-09 19:27:00.000000 pyflyde-0.0.5/pyflyde.egg-info/SOURCES.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)        1 2024-05-09 19:26:59.000000 pyflyde-0.0.5/pyflyde.egg-info/dependency_links.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)       40 2024-05-09 19:26:59.000000 pyflyde-0.0.5/pyflyde.egg-info/entry_points.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)       64 2024-05-09 19:26:59.000000 pyflyde-0.0.5/pyflyde.egg-info/requires.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)        6 2024-05-09 19:26:59.000000 pyflyde-0.0.5/pyflyde.egg-info/top_level.txt
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1272 2024-05-09 19:24:42.000000 pyflyde-0.0.5/pyproject.toml
+-rw-r--r--   0 trustmaster   (501) staff       (20)       38 2024-05-09 19:27:00.182659 pyflyde-0.0.5/setup.cfg
+drwxr-xr-x   0 trustmaster   (501) staff       (20)        0 2024-05-09 19:27:00.170437 pyflyde-0.0.5/tests/
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1744 2024-05-09 10:46:21.000000 pyflyde-0.0.5/tests/Repeat3Times.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)      782 2024-04-25 19:45:07.000000 pyflyde-0.0.5/tests/TestInOutFlow.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)      820 2024-04-24 22:56:30.000000 pyflyde-0.0.5/tests/TestIsolatedFlow.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1798 2024-05-09 10:46:21.000000 pyflyde-0.0.5/tests/TestNestedFlow.flyde
+-rw-r--r--   0 trustmaster   (501) staff       (20)        0 2024-04-09 17:26:09.000000 pyflyde-0.0.5/tests/__init.py__
+-rw-r--r--   0 trustmaster   (501) staff       (20)      914 2024-05-09 10:46:21.000000 pyflyde-0.0.5/tests/components.flyde.ts
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1185 2024-05-09 10:46:21.000000 pyflyde-0.0.5/tests/components.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     1933 2024-05-09 10:46:21.000000 pyflyde-0.0.5/tests/test_flow.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)    10544 2024-05-09 10:46:21.000000 pyflyde-0.0.5/tests/test_io.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)    11312 2024-05-09 10:46:21.000000 pyflyde-0.0.5/tests/test_node.py
+-rw-r--r--   0 trustmaster   (501) staff       (20)     3754 2024-05-09 10:46:21.000000 pyflyde-0.0.5/tests/test_stdlib.py
```

### Comparing `pyflyde-0.0.4/.github/workflows/python-package.yml` & `pyflyde-0.0.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/.gitignore` & `pyflyde-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/LICENSE` & `pyflyde-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/Makefile` & `pyflyde-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/PKG-INFO` & `pyflyde-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyde
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK and runtime for Flyde - a visual flow-based programming language and IDE.
 Author: Vladimir Sibirov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyflyde-0.0.4/README.md` & `pyflyde-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/clustering_example.png` & `pyflyde-0.0.5/clustering_example.png`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/examples/Clustering.flyde` & `pyflyde-0.0.5/examples/Clustering.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/examples/HelloPy.flyde` & `pyflyde-0.0.5/examples/HelloPy.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/examples/datasets/wine-clustering.csv` & `pyflyde-0.0.5/examples/datasets/wine-clustering.csv`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/examples/mylib/components.flyde.ts` & `pyflyde-0.0.5/examples/mylib/components.flyde.ts`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/examples/mylib/components.py` & `pyflyde-0.0.5/examples/mylib/components.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/examples/mylib/dataframe.flyde.ts` & `pyflyde-0.0.5/examples/mylib/dataframe.flyde.ts`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/examples/mylib/dataframe.py` & `pyflyde-0.0.5/examples/mylib/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/examples/mylib/kmeans.flyde.ts` & `pyflyde-0.0.5/examples/mylib/kmeans.flyde.ts`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/examples/mylib/kmeans.py` & `pyflyde-0.0.5/examples/mylib/kmeans.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/flyde/flow.py` & `pyflyde-0.0.5/flyde/flow.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/flyde/flow.pyi` & `pyflyde-0.0.5/flyde/flow.pyi`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/flyde/io.py` & `pyflyde-0.0.5/flyde/io.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/flyde/io.pyi` & `pyflyde-0.0.5/flyde/io.pyi`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/flyde/node.py` & `pyflyde-0.0.5/flyde/node.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/flyde/node.pyi` & `pyflyde-0.0.5/flyde/node.pyi`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/flyde/stdlib.py` & `pyflyde-0.0.5/flyde/stdlib.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/flyde.py` & `pyflyde-0.0.5/flyde.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/pyflyde.egg-info/PKG-INFO` & `pyflyde-0.0.5/pyflyde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyflyde
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python SDK and runtime for Flyde - a visual flow-based programming language and IDE.
 Author: Vladimir Sibirov
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `pyflyde-0.0.4/pyflyde.egg-info/SOURCES.txt` & `pyflyde-0.0.5/pyflyde.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 flyde/node.py
 flyde/node.pyi
 flyde/stdlib.py
 flyde/stdlib.pyi
 pyflyde.egg-info/PKG-INFO
 pyflyde.egg-info/SOURCES.txt
 pyflyde.egg-info/dependency_links.txt
+pyflyde.egg-info/entry_points.txt
 pyflyde.egg-info/requires.txt
 pyflyde.egg-info/top_level.txt
 tests/Repeat3Times.flyde
 tests/TestInOutFlow.flyde
 tests/TestIsolatedFlow.flyde
 tests/TestNestedFlow.flyde
 tests/__init.py__
```

### Comparing `pyflyde-0.0.4/pyproject.toml` & `pyflyde-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyflyde"
-version = "0.0.4"
+version = "0.0.5"
 requires-python = ">= 3.9"
 authors = [
     {name = "Vladimir Sibirov"}
 ]
 description="Python SDK and runtime for Flyde - a visual flow-based programming language and IDE."
 readme="README.md"
 classifiers = [
@@ -28,14 +28,17 @@
 ]
 license = { file = "LICENSE" }
 
 dependencies = [
     "pyyaml",
 ]
 
+[project.scripts]
+flyde = "flyde.py:main"
+
 # [tool.setuptools]
 # package-dir = { "" = "flyde" }
 # packages = ["flyde"]
 
 [project.optional-dependencies]
 dev = [
     "setuptools",
```

### Comparing `pyflyde-0.0.4/tests/Repeat3Times.flyde` & `pyflyde-0.0.5/tests/Repeat3Times.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/tests/TestInOutFlow.flyde` & `pyflyde-0.0.5/tests/TestInOutFlow.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/tests/TestIsolatedFlow.flyde` & `pyflyde-0.0.5/tests/TestIsolatedFlow.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/tests/TestNestedFlow.flyde` & `pyflyde-0.0.5/tests/TestNestedFlow.flyde`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/tests/components.flyde.ts` & `pyflyde-0.0.5/tests/components.flyde.ts`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/tests/components.py` & `pyflyde-0.0.5/tests/components.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/tests/test_flow.py` & `pyflyde-0.0.5/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/tests/test_io.py` & `pyflyde-0.0.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/tests/test_node.py` & `pyflyde-0.0.5/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyflyde-0.0.4/tests/test_stdlib.py` & `pyflyde-0.0.5/tests/test_stdlib.py`

 * *Files identical despite different names*


# Comparing `tmp/multigather-0.0.2.tar.gz` & `tmp/multigather-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Admin\Desktop\gathernous\dist\.tmp-r49d4g8_\multigather-0.0.2.tar", last modified: Thu May  9 07:39:23 2024, max compression
+gzip compressed data, was "C:\Users\Admin\Desktop\gathernous\dist\.tmp-k2ih5vxr\multigather-0.0.3.tar", last modified: Thu May  9 07:44:08 2024, max compression
```

## Comparing `multigather-0.0.2.tar` & `multigather-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 07:39:23.645489 multigather-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-09 07:39:23.614869 multigather-0.0.2/MultiGather/
--rw-rw-rw-   0        0        0     1825 2024-05-09 07:37:15.000000 multigather-0.0.2/MultiGather/Client.py
--rw-rw-rw-   0        0        0      708 2024-05-09 07:31:32.000000 multigather-0.0.2/MultiGather/Types.py
--rw-rw-rw-   0        0        0       43 2024-05-09 07:32:32.000000 multigather-0.0.2/MultiGather/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 07:39:23.642961 multigather-0.0.2/MultiGather.egg-info/
--rw-rw-rw-   0        0        0     2256 2024-05-09 07:39:23.000000 multigather-0.0.2/MultiGather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-05-09 07:39:23.000000 multigather-0.0.2/MultiGather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 07:39:23.000000 multigather-0.0.2/MultiGather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 07:39:23.000000 multigather-0.0.2/MultiGather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2256 2024-05-09 07:39:23.643466 multigather-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1755 2024-05-09 07:37:15.000000 multigather-0.0.2/README.md
--rw-rw-rw-   0        0        0      504 2024-05-09 07:38:21.000000 multigather-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 07:39:23.645489 multigather-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 07:44:08.661065 multigather-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-09 07:44:08.638834 multigather-0.0.3/MultiGather/
+-rw-rw-rw-   0        0        0     1825 2024-05-09 07:37:15.000000 multigather-0.0.3/MultiGather/Client.py
+-rw-rw-rw-   0        0        0      708 2024-05-09 07:31:32.000000 multigather-0.0.3/MultiGather/Types.py
+-rw-rw-rw-   0        0        0       45 2024-05-09 07:42:54.000000 multigather-0.0.3/MultiGather/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:44:08.661065 multigather-0.0.3/MultiGather.egg-info/
+-rw-rw-rw-   0        0        0     2256 2024-05-09 07:44:08.000000 multigather-0.0.3/MultiGather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-05-09 07:44:08.000000 multigather-0.0.3/MultiGather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 07:44:08.000000 multigather-0.0.3/MultiGather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 07:44:08.000000 multigather-0.0.3/MultiGather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2256 2024-05-09 07:44:08.661065 multigather-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1755 2024-05-09 07:37:15.000000 multigather-0.0.3/README.md
+-rw-rw-rw-   0        0        0      504 2024-05-09 07:43:52.000000 multigather-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 07:44:08.666608 multigather-0.0.3/setup.cfg
```

### Comparing `multigather-0.0.2/MultiGather/Client.py` & `multigather-0.0.3/MultiGather/Client.py`

 * *Files identical despite different names*

### Comparing `multigather-0.0.2/MultiGather/Types.py` & `multigather-0.0.3/MultiGather/Types.py`

 * *Files identical despite different names*

### Comparing `multigather-0.0.2/MultiGather.egg-info/PKG-INFO` & `multigather-0.0.3/MultiGather.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.2
+Version: 0.0.3
 Summary: Send multiple requests using 3 lines of code!
 Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multigather-0.0.2/PKG-INFO` & `multigather-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGather
-Version: 0.0.2
+Version: 0.0.3
 Summary: Send multiple requests using 3 lines of code!
 Author-email: "Mr. Mahdi" <any@hi2.in>
 Project-URL: Homepage, https://github.com/tm-sah/MultiGather
 Project-URL: Issues, https://github.com/tm-sah/MultiGather/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multigather-0.0.2/README.md` & `multigather-0.0.3/README.md`

 * *Files identical despite different names*


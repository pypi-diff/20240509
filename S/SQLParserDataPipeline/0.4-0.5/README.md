# Comparing `tmp/SQLParserDataPipeline-0.4.tar.gz` & `tmp/SQLParserDataPipeline-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLParserDataPipeline-0.4.tar", last modified: Thu May  9 16:34:09 2024, max compression
+gzip compressed data, was "SQLParserDataPipeline-0.5.tar", last modified: Thu May  9 16:38:30 2024, max compression
```

## Comparing `SQLParserDataPipeline-0.4.tar` & `SQLParserDataPipeline-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 16:34:09.050075 SQLParserDataPipeline-0.4/
-drwxrwxrwx   0        0        0        0 2024-05-09 16:34:08.997022 SQLParserDataPipeline-0.4/Library/
--rw-rw-rw-   0        0        0     1124 2024-05-09 15:01:03.000000 SQLParserDataPipeline-0.4/Library/From.py
--rw-rw-rw-   0        0        0     3142 2024-05-09 15:00:32.000000 SQLParserDataPipeline-0.4/Library/Select.py
--rw-rw-rw-   0        0        0     1460 2024-05-09 15:00:35.000000 SQLParserDataPipeline-0.4/Library/Unnest.py
--rw-rw-rw-   0        0        0        0 2024-05-09 15:33:44.000000 SQLParserDataPipeline-0.4/Library/__init__.py
--rw-rw-rw-   0        0        0     3375 2024-05-09 16:34:09.046838 SQLParserDataPipeline-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2393 2024-05-09 15:02:03.000000 SQLParserDataPipeline-0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 16:34:09.043825 SQLParserDataPipeline-0.4/SQLParserDataPipeline.egg-info/
--rw-rw-rw-   0        0        0     3375 2024-05-09 16:34:08.000000 SQLParserDataPipeline-0.4/SQLParserDataPipeline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-05-09 16:34:08.000000 SQLParserDataPipeline-0.4/SQLParserDataPipeline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 16:34:08.000000 SQLParserDataPipeline-0.4/SQLParserDataPipeline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-09 16:34:08.000000 SQLParserDataPipeline-0.4/SQLParserDataPipeline.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 16:34:09.050075 SQLParserDataPipeline-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1343 2024-05-09 16:34:01.000000 SQLParserDataPipeline-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:38:30.052354 SQLParserDataPipeline-0.5/
+-rw-rw-rw-   0        0        0     3375 2024-05-09 16:38:30.052354 SQLParserDataPipeline-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2393 2024-05-09 15:02:03.000000 SQLParserDataPipeline-0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 16:38:30.012231 SQLParserDataPipeline-0.5/SQLParserDataPipeline/
+-rw-rw-rw-   0        0        0     1124 2024-05-09 15:01:03.000000 SQLParserDataPipeline-0.5/SQLParserDataPipeline/From.py
+-rw-rw-rw-   0        0        0     3142 2024-05-09 15:00:32.000000 SQLParserDataPipeline-0.5/SQLParserDataPipeline/Select.py
+-rw-rw-rw-   0        0        0     1460 2024-05-09 15:00:35.000000 SQLParserDataPipeline-0.5/SQLParserDataPipeline/Unnest.py
+-rw-rw-rw-   0        0        0        0 2024-05-09 15:33:44.000000 SQLParserDataPipeline-0.5/SQLParserDataPipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:38:30.043191 SQLParserDataPipeline-0.5/SQLParserDataPipeline.egg-info/
+-rw-rw-rw-   0        0        0     3375 2024-05-09 16:38:29.000000 SQLParserDataPipeline-0.5/SQLParserDataPipeline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-05-09 16:38:29.000000 SQLParserDataPipeline-0.5/SQLParserDataPipeline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 16:38:29.000000 SQLParserDataPipeline-0.5/SQLParserDataPipeline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-09 16:38:29.000000 SQLParserDataPipeline-0.5/SQLParserDataPipeline.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 16:38:30.052354 SQLParserDataPipeline-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2024-05-09 16:38:23.000000 SQLParserDataPipeline-0.5/setup.py
```

### Comparing `SQLParserDataPipeline-0.4/Library/From.py` & `SQLParserDataPipeline-0.5/SQLParserDataPipeline/From.py`

 * *Files identical despite different names*

### Comparing `SQLParserDataPipeline-0.4/Library/Select.py` & `SQLParserDataPipeline-0.5/SQLParserDataPipeline/Select.py`

 * *Files identical despite different names*

### Comparing `SQLParserDataPipeline-0.4/Library/Unnest.py` & `SQLParserDataPipeline-0.5/SQLParserDataPipeline/Unnest.py`

 * *Files identical despite different names*

### Comparing `SQLParserDataPipeline-0.4/PKG-INFO` & `SQLParserDataPipeline-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLParserDataPipeline
-Version: 0.4
+Version: 0.5
 Summary: The SQLParserDataPipeline Library is a powerful Python package designed for parsing and interpreting complex SQL queries. It was developed with a focus on BigQuery but is adaptable to other SQL dialects due to its flexible parsing strategy that doesn't consider the function itself but the most inner parentheses.
 Author: Emanuele Iaccarino
 Author-email: emanueleiaccarino.ei@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SQLParserDataPipeline-0.4/README.md` & `SQLParserDataPipeline-0.5/README.md`

 * *Files identical despite different names*

### Comparing `SQLParserDataPipeline-0.4/SQLParserDataPipeline.egg-info/PKG-INFO` & `SQLParserDataPipeline-0.5/SQLParserDataPipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLParserDataPipeline
-Version: 0.4
+Version: 0.5
 Summary: The SQLParserDataPipeline Library is a powerful Python package designed for parsing and interpreting complex SQL queries. It was developed with a focus on BigQuery but is adaptable to other SQL dialects due to its flexible parsing strategy that doesn't consider the function itself but the most inner parentheses.
 Author: Emanuele Iaccarino
 Author-email: emanueleiaccarino.ei@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `SQLParserDataPipeline-0.4/setup.py` & `SQLParserDataPipeline-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 print(find_packages())
 
 setup(
     name='SQLParserDataPipeline', 
-    version='0.4',      
+    version='0.5',      
     author='Emanuele Iaccarino',  
     author_email='emanueleiaccarino.ei@gmail.com',  
     description="The SQLParserDataPipeline Library is a powerful Python package designed for parsing and interpreting complex SQL queries. It was developed with a focus on BigQuery but is adaptable to other SQL dialects due to its flexible parsing strategy that doesn't consider the function itself but the most inner parentheses.",
     long_description=open('README.md').read(),  
     long_description_content_type='text/markdown',
     packages=find_packages(), 
     install_requires=[
```


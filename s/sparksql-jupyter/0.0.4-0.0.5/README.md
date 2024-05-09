# Comparing `tmp/sparksql-jupyter-0.0.4.tar.gz` & `tmp/sparksql-jupyter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparksql-jupyter-0.0.4.tar", last modified: Mon Jan 29 12:27:26 2024, max compression
+gzip compressed data, was "sparksql-jupyter-0.0.5.tar", last modified: Thu May  9 02:02:49 2024, max compression
```

## Comparing `sparksql-jupyter-0.0.4.tar` & `sparksql-jupyter-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 grey.parrot   (502) staff       (20)        0 2024-01-29 12:27:26.426107 sparksql-jupyter-0.0.4/
--rw-r--r--   0 grey.parrot   (502) staff       (20)     1069 2024-01-17 07:04:58.000000 sparksql-jupyter-0.0.4/LICENSE
--rw-r--r--   0 grey.parrot   (502) staff       (20)     1644 2024-01-29 12:27:26.426211 sparksql-jupyter-0.0.4/PKG-INFO
--rw-r--r--   0 grey.parrot   (502) staff       (20)      978 2024-01-29 09:49:49.000000 sparksql-jupyter-0.0.4/README.md
--rw-r--r--   0 grey.parrot   (502) staff       (20)       71 2024-01-29 12:27:26.427048 sparksql-jupyter-0.0.4/setup.cfg
--rw-r--r--   0 grey.parrot   (502) staff       (20)      960 2024-01-29 12:13:27.000000 sparksql-jupyter-0.0.4/setup.py
-drwxr-xr-x   0 grey.parrot   (502) staff       (20)        0 2024-01-29 12:27:26.421922 sparksql-jupyter-0.0.4/sparksql_jupyter/
--rw-r--r--   0 grey.parrot   (502) staff       (20)      131 2024-01-28 04:22:24.000000 sparksql-jupyter-0.0.4/sparksql_jupyter/__init__.py
--rw-r--r--   0 grey.parrot   (502) staff       (20)     3407 2024-01-28 05:22:34.000000 sparksql-jupyter-0.0.4/sparksql_jupyter/sparksql.py
-drwxr-xr-x   0 grey.parrot   (502) staff       (20)        0 2024-01-29 12:27:26.425848 sparksql-jupyter-0.0.4/sparksql_jupyter.egg-info/
--rw-r--r--   0 grey.parrot   (502) staff       (20)     1644 2024-01-29 12:27:26.000000 sparksql-jupyter-0.0.4/sparksql_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 grey.parrot   (502) staff       (20)      293 2024-01-29 12:27:26.000000 sparksql-jupyter-0.0.4/sparksql_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 grey.parrot   (502) staff       (20)        1 2024-01-29 12:27:26.000000 sparksql-jupyter-0.0.4/sparksql_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 grey.parrot   (502) staff       (20)       44 2024-01-29 12:27:26.000000 sparksql-jupyter-0.0.4/sparksql_jupyter.egg-info/requires.txt
--rw-r--r--   0 grey.parrot   (502) staff       (20)       17 2024-01-29 12:27:26.000000 sparksql-jupyter-0.0.4/sparksql_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 grey.parrot   (502) staff       (20)        0 2024-05-09 02:02:49.347421 sparksql-jupyter-0.0.5/
+-rw-r--r--   0 grey.parrot   (502) staff       (20)     1069 2024-01-17 07:04:58.000000 sparksql-jupyter-0.0.5/LICENSE
+-rw-r--r--   0 grey.parrot   (502) staff       (20)     1722 2024-05-09 02:02:49.347810 sparksql-jupyter-0.0.5/PKG-INFO
+-rw-r--r--   0 grey.parrot   (502) staff       (20)     1076 2024-05-09 02:01:53.000000 sparksql-jupyter-0.0.5/README.md
+-rw-r--r--   0 grey.parrot   (502) staff       (20)       71 2024-05-09 02:02:49.349173 sparksql-jupyter-0.0.5/setup.cfg
+-rw-r--r--   0 grey.parrot   (502) staff       (20)      960 2024-05-09 01:58:17.000000 sparksql-jupyter-0.0.5/setup.py
+drwxr-xr-x   0 grey.parrot   (502) staff       (20)        0 2024-05-09 02:02:49.330215 sparksql-jupyter-0.0.5/sparksql_jupyter/
+-rw-r--r--   0 grey.parrot   (502) staff       (20)      131 2024-05-09 02:00:30.000000 sparksql-jupyter-0.0.5/sparksql_jupyter/__init__.py
+-rw-r--r--   0 grey.parrot   (502) staff       (20)     3898 2024-05-09 01:58:17.000000 sparksql-jupyter-0.0.5/sparksql_jupyter/sparksql.py
+drwxr-xr-x   0 grey.parrot   (502) staff       (20)        0 2024-05-09 02:02:49.343907 sparksql-jupyter-0.0.5/sparksql_jupyter.egg-info/
+-rw-r--r--   0 grey.parrot   (502) staff       (20)     1722 2024-05-09 02:02:49.000000 sparksql-jupyter-0.0.5/sparksql_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 grey.parrot   (502) staff       (20)      293 2024-05-09 02:02:49.000000 sparksql-jupyter-0.0.5/sparksql_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 grey.parrot   (502) staff       (20)        1 2024-05-09 02:02:49.000000 sparksql-jupyter-0.0.5/sparksql_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 grey.parrot   (502) staff       (20)       44 2024-05-09 02:02:49.000000 sparksql-jupyter-0.0.5/sparksql_jupyter.egg-info/requires.txt
+-rw-r--r--   0 grey.parrot   (502) staff       (20)       17 2024-05-09 02:02:49.000000 sparksql-jupyter-0.0.5/sparksql_jupyter.egg-info/top_level.txt
```

### Comparing `sparksql-jupyter-0.0.4/LICENSE` & `sparksql-jupyter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksql-jupyter-0.0.4/PKG-INFO` & `sparksql-jupyter-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sparksql-jupyter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spark SQL magic command for Jupyter notebooks
 Home-page: https://github.com/cryeo/sparksql-jupyter
 Author: Cinyoung Hur
 Author-email: cinyoung.hur@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
@@ -62,10 +61,12 @@
 |`-e` `--eager`|Cache dataframe with eager load|
 |`-v VIEW` `--view VIEW`|Create or replace temporary view|
 |`-l LIMIT` `--limit LIMIT`|The maximum number of rows to display (Default: `SparkSql.limit`)|
 |`variable`|Capture dataframe in a local variable|
 |`-j` `--jinja`|Capture dataframe in a local variable in jinja2 template|
 
 
+## Release Note
 
-
+- 2024/05/09
+  - stringify timestamp with timezone columns before seriealization
```

### Comparing `sparksql-jupyter-0.0.4/README.md` & `sparksql-jupyter-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -43,8 +43,12 @@
 |`-e` `--eager`|Cache dataframe with eager load|
 |`-v VIEW` `--view VIEW`|Create or replace temporary view|
 |`-l LIMIT` `--limit LIMIT`|The maximum number of rows to display (Default: `SparkSql.limit`)|
 |`variable`|Capture dataframe in a local variable|
 |`-j` `--jinja`|Capture dataframe in a local variable in jinja2 template|
 
 
+## Release Note
+
+- 2024/05/09
+  - stringify timestamp with timezone columns before seriealization
```

### Comparing `sparksql-jupyter-0.0.4/setup.py` & `sparksql-jupyter-0.0.5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import find_packages, setup
 
 import sparksql_jupyter
 
 setup(
-    name='sparksql-jupyter',
+    name="sparksql-jupyter",
     version=sparksql_jupyter.__version__,
-    description='Spark SQL magic command for Jupyter notebooks',
-    long_description=open('README.md', 'r').read(),
-    long_description_content_type='text/markdown',
-    author='Cinyoung Hur',
-    author_email='cinyoung.hur@gmail.com',
-    url='https://github.com/cryeo/sparksql-jupyter',
-    license='MIT License',
-    install_requires=['pyspark>=2.3.0', 'ipython>=7.4.0', 'jinja2>=3.0.0'],
-    packages=find_packages(exclude=('tests', 'docs')),
-    python_requires='>=3.6',
+    description="Spark SQL magic command for Jupyter notebooks",
+    long_description=open("README.md", "r").read(),
+    long_description_content_type="text/markdown",
+    author="Cinyoung Hur",
+    author_email="cinyoung.hur@gmail.com",
+    url="https://github.com/cryeo/sparksql-jupyter",
+    license="MIT License",
+    install_requires=["pyspark>=2.3.0", "ipython>=7.4.0", "jinja2>=3.0.0"],
+    packages=find_packages(exclude=("tests", "docs")),
+    python_requires=">=3.6",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        "Development Status :: 2 - Pre-Alpha",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `sparksql-jupyter-0.0.4/sparksql_jupyter.egg-info/PKG-INFO` & `sparksql-jupyter-0.0.5/sparksql_jupyter.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sparksql-jupyter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spark SQL magic command for Jupyter notebooks
 Home-page: https://github.com/cryeo/sparksql-jupyter
 Author: Cinyoung Hur
 Author-email: cinyoung.hur@gmail.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
@@ -62,10 +61,12 @@
 |`-e` `--eager`|Cache dataframe with eager load|
 |`-v VIEW` `--view VIEW`|Create or replace temporary view|
 |`-l LIMIT` `--limit LIMIT`|The maximum number of rows to display (Default: `SparkSql.limit`)|
 |`variable`|Capture dataframe in a local variable|
 |`-j` `--jinja`|Capture dataframe in a local variable in jinja2 template|
 
 
+## Release Note
 
-
+- 2024/05/09
+  - stringify timestamp with timezone columns before seriealization
```


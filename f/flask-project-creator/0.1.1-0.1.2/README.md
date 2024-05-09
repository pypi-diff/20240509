# Comparing `tmp/flask_project_creator-0.1.1.tar.gz` & `tmp/flask_project_creator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_project_creator-0.1.1.tar", last modified: Thu May  9 08:44:55 2024, max compression
+gzip compressed data, was "flask_project_creator-0.1.2.tar", last modified: Thu May  9 17:07:06 2024, max compression
```

## Comparing `flask_project_creator-0.1.1.tar` & `flask_project_creator-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 08:44:55.792843 flask_project_creator-0.1.1/
--rw-rw-rw-   0        0        0     1516 2024-05-09 08:44:55.790842 flask_project_creator-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 08:44:55.730919 flask_project_creator-0.1.1/flask_project_creator/
--rw-rw-rw-   0        0        0     3154 2024-05-08 18:06:12.000000 flask_project_creator-0.1.1/flask_project_creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 08:44:55.780758 flask_project_creator-0.1.1/flask_project_creator.egg-info/
--rw-rw-rw-   0        0        0     1516 2024-05-09 08:44:55.000000 flask_project_creator-0.1.1/flask_project_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-09 08:44:55.000000 flask_project_creator-0.1.1/flask_project_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 08:44:55.000000 flask_project_creator-0.1.1/flask_project_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2024-05-09 08:44:55.000000 flask_project_creator-0.1.1/flask_project_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-05-09 08:44:55.000000 flask_project_creator-0.1.1/flask_project_creator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-09 08:44:55.000000 flask_project_creator-0.1.1/flask_project_creator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 08:44:55.792843 flask_project_creator-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1945 2024-05-09 08:40:56.000000 flask_project_creator-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:07:06.608523 flask_project_creator-0.1.2/
+-rw-rw-rw-   0        0        0     1538 2024-05-09 17:07:06.605526 flask_project_creator-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 17:07:06.559095 flask_project_creator-0.1.2/flask_project_creator/
+-rw-rw-rw-   0        0        0     3154 2024-05-08 18:06:12.000000 flask_project_creator-0.1.2/flask_project_creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:07:06.593390 flask_project_creator-0.1.2/flask_project_creator.egg-info/
+-rw-rw-rw-   0        0        0     1538 2024-05-09 17:07:04.000000 flask_project_creator-0.1.2/flask_project_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-09 17:07:05.000000 flask_project_creator-0.1.2/flask_project_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 17:07:05.000000 flask_project_creator-0.1.2/flask_project_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-05-09 17:07:05.000000 flask_project_creator-0.1.2/flask_project_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 17:07:05.000000 flask_project_creator-0.1.2/flask_project_creator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-09 17:07:05.000000 flask_project_creator-0.1.2/flask_project_creator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 17:07:06.608523 flask_project_creator-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1963 2024-05-09 17:06:12.000000 flask_project_creator-0.1.2/setup.py
```

### Comparing `flask_project_creator-0.1.1/PKG-INFO` & `flask_project_creator-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: flask_project_creator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Flask Project Creator: A CLI tool for quickly setting up Flask web applications.
 Author: Omkar Subhash Parab
 Author-email: omkar211196@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: click
+Requires-Dist: flask
 
 
 Flask Project Creator is a command-line interface (CLI) tool designed to expedite the creation of Flask web applications. With just a single command, this tool automates the generation of a Flask project directory structure, including essential files and folders such as `run.py`, `__init__.py`, `templates`, and `static`. Additionally, it provides basic templates (`base.html` and `home.html`) along with example route definitions to jumpstart your development process.
 
 This tool leverages Click, a Python package for creating command-line interfaces, to offer a user-friendly experience with customizable options. Whether you're starting a new web project, prototyping ideas, or simply looking to streamline your Flask development workflow, Flask Project Creator simplifies the initial setup process, allowing you to focus on building your application logic without the hassle of manual configuration.
 
 Key Features:
```

### Comparing `flask_project_creator-0.1.1/flask_project_creator/__init__.py` & `flask_project_creator-0.1.2/flask_project_creator/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_project_creator-0.1.1/flask_project_creator.egg-info/PKG-INFO` & `flask_project_creator-0.1.2/flask_project_creator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: flask_project_creator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Flask Project Creator: A CLI tool for quickly setting up Flask web applications.
 Author: Omkar Subhash Parab
 Author-email: omkar211196@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: click
+Requires-Dist: flask
 
 
 Flask Project Creator is a command-line interface (CLI) tool designed to expedite the creation of Flask web applications. With just a single command, this tool automates the generation of a Flask project directory structure, including essential files and folders such as `run.py`, `__init__.py`, `templates`, and `static`. Additionally, it provides basic templates (`base.html` and `home.html`) along with example route definitions to jumpstart your development process.
 
 This tool leverages Click, a Python package for creating command-line interfaces, to offer a user-friendly experience with customizable options. Whether you're starting a new web project, prototyping ideas, or simply looking to streamline your Flask development workflow, Flask Project Creator simplifies the initial setup process, allowing you to focus on building your application logic without the hassle of manual configuration.
 
 Key Features:
```

### Comparing `flask_project_creator-0.1.1/setup.py` & `flask_project_creator-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 
 CLI Command:
 - Command Name: create-flask-project
 """
 
 setup(
     name='flask_project_creator',
-    version='0.1.1',
+    version='0.1.2',
     author='Omkar Subhash Parab',
     author_email='omkar211196@gmail.com',
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'create-flask-project=flask_project_creator.__init__:create_project',
         ],
     },
     install_requires=[
         'click',
+        'flask',
     ],
 )
```


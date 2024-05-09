# Comparing `tmp/aim_flask-1.0.0.tar.gz` & `tmp/aim_flask-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aim_flask-1.0.0.tar", last modified: Thu May  9 04:27:27 2024, max compression
+gzip compressed data, was "aim_flask-1.0.1.tar", last modified: Thu May  9 05:02:52 2024, max compression
```

## Comparing `aim_flask-1.0.0.tar` & `aim_flask-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 04:27:27.689813 aim_flask-1.0.0/
--rw-rw-rw-   0        0        0     1087 2024-05-08 23:37:10.000000 aim_flask-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-09 02:33:14.000000 aim_flask-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      907 2024-05-09 04:27:27.688815 aim_flask-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-05-08 23:37:10.000000 aim_flask-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 04:27:27.685817 aim_flask-1.0.0/aim_flask.egg-info/
--rw-rw-rw-   0        0        0      907 2024-05-09 04:27:27.000000 aim_flask-1.0.0/aim_flask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-09 04:27:27.000000 aim_flask-1.0.0/aim_flask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 04:27:27.000000 aim_flask-1.0.0/aim_flask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-09 04:27:27.000000 aim_flask-1.0.0/aim_flask.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 04:27:27.679361 aim_flask-1.0.0/app/
--rw-rw-rw-   0        0        0       40 2024-05-09 04:27:06.000000 aim_flask-1.0.0/app/__init__.py
--rw-rw-rw-   0        0        0       43 2024-05-09 04:27:06.000000 aim_flask-1.0.0/app/routes.py
--rw-rw-rw-   0        0        0       85 2024-05-09 04:27:27.703299 aim_flask-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1625 2024-05-09 04:23:11.000000 aim_flask-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 05:02:52.323252 aim_flask-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2024-05-08 23:37:10.000000 aim_flask-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-09 02:33:14.000000 aim_flask-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      907 2024-05-09 05:02:52.320258 aim_flask-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-05-08 23:37:10.000000 aim_flask-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 05:02:52.314042 aim_flask-1.0.1/aim_flask.egg-info/
+-rw-rw-rw-   0        0        0      907 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 05:02:52.305047 aim_flask-1.0.1/app/
+-rw-rw-rw-   0        0        0       40 2024-05-09 04:52:52.000000 aim_flask-1.0.1/app/__init__.py
+-rw-rw-rw-   0        0        0       43 2024-05-09 04:52:52.000000 aim_flask-1.0.1/app/routes.py
+-rw-rw-rw-   0        0        0       85 2024-05-09 05:02:52.328793 aim_flask-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1731 2024-05-09 05:02:04.000000 aim_flask-1.0.1/setup.py
```

### Comparing `aim_flask-1.0.0/LICENSE` & `aim_flask-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aim_flask-1.0.0/PKG-INFO` & `aim_flask-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aim-flask
-Version: 1.0.0
+Name: aim_flask
+Version: 1.0.1
 Summary: A CLI tool for setting up and managing AIM environments
 Home-page: https://github.com/MrMayami/AIM
 Author: Joe Mayami
 Author-email: pr.mayami@gmail.com
 Project-URL: GitHub, https://github.com/MrMayami/AIM
 Keywords: AIM Flask
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `aim_flask-1.0.0/aim_flask.egg-info/PKG-INFO` & `aim_flask-1.0.1/aim_flask.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aim-flask
-Version: 1.0.0
+Name: aim_flask
+Version: 1.0.1
 Summary: A CLI tool for setting up and managing AIM environments
 Home-page: https://github.com/MrMayami/AIM
 Author: Joe Mayami
 Author-email: pr.mayami@gmail.com
 Project-URL: GitHub, https://github.com/MrMayami/AIM
 Keywords: AIM Flask
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `aim_flask-1.0.0/setup.py` & `aim_flask-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Directory containing the setup.py file
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
-    name="aim-flask",  # Required
-    version="1.0.0",  # Required
+    name="aim_flask",  # Required
+    version="1.0.1",  # Required
     description="A CLI tool for setting up and managing AIM environments",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional
     url="https://github.com/MrMayami/AIM",  # Optional
     author="Joe Mayami",  # Optional
     author_email="pr.mayami@gmail.com",  # Optional
     classifiers=[  # Optional
@@ -33,12 +33,17 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="AIM Flask",  # Optional
     packages=find_packages(),  # Required
     python_requires=">=3.7, <4",  # Required
+     entry_points={
+        'console_scripts': [
+            'aim=aim_flask:main',
+        ],
+    },
     install_requires=[],  # Optional
     project_urls={  # Optional
         "GitHub": "https://github.com/MrMayami/AIM",
     },
 )
```


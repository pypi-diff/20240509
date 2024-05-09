# Comparing `tmp/aim_flask-1.0.1.tar.gz` & `tmp/aim_flask-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aim_flask-1.0.1.tar", last modified: Thu May  9 05:02:52 2024, max compression
+gzip compressed data, was "aim_flask-1.0.2.tar", last modified: Thu May  9 16:14:58 2024, max compression
```

## Comparing `aim_flask-1.0.1.tar` & `aim_flask-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 05:02:52.323252 aim_flask-1.0.1/
--rw-rw-rw-   0        0        0     1087 2024-05-08 23:37:10.000000 aim_flask-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-09 02:33:14.000000 aim_flask-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      907 2024-05-09 05:02:52.320258 aim_flask-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-05-08 23:37:10.000000 aim_flask-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 05:02:52.314042 aim_flask-1.0.1/aim_flask.egg-info/
--rw-rw-rw-   0        0        0      907 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2024-05-09 05:02:51.000000 aim_flask-1.0.1/aim_flask.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 05:02:52.305047 aim_flask-1.0.1/app/
--rw-rw-rw-   0        0        0       40 2024-05-09 04:52:52.000000 aim_flask-1.0.1/app/__init__.py
--rw-rw-rw-   0        0        0       43 2024-05-09 04:52:52.000000 aim_flask-1.0.1/app/routes.py
--rw-rw-rw-   0        0        0       85 2024-05-09 05:02:52.328793 aim_flask-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1731 2024-05-09 05:02:04.000000 aim_flask-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:14:58.025828 aim_flask-1.0.2/
+-rw-rw-rw-   0        0        0     1087 2024-05-08 23:37:10.000000 aim_flask-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-09 02:33:14.000000 aim_flask-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      907 2024-05-09 16:14:58.017829 aim_flask-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-05-08 23:37:10.000000 aim_flask-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 16:14:58.017829 aim_flask-1.0.2/aim_flask.egg-info/
+-rw-rw-rw-   0        0        0      907 2024-05-09 16:14:57.000000 aim_flask-1.0.2/aim_flask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-09 16:14:57.000000 aim_flask-1.0.2/aim_flask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 16:14:57.000000 aim_flask-1.0.2/aim_flask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-09 16:14:57.000000 aim_flask-1.0.2/aim_flask.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 16:14:57.000000 aim_flask-1.0.2/aim_flask.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7838 2024-05-09 05:02:46.000000 aim_flask-1.0.2/aim_flask.py
+-rw-rw-rw-   0        0        0       85 2024-05-09 16:14:58.025828 aim_flask-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1790 2024-05-09 16:12:24.000000 aim_flask-1.0.2/setup.py
```

### Comparing `aim_flask-1.0.1/LICENSE` & `aim_flask-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aim_flask-1.0.1/PKG-INFO` & `aim_flask-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim_flask
-Version: 1.0.1
+Version: 1.0.2
 Summary: A CLI tool for setting up and managing AIM environments
 Home-page: https://github.com/MrMayami/AIM
 Author: Joe Mayami
 Author-email: pr.mayami@gmail.com
 Project-URL: GitHub, https://github.com/MrMayami/AIM
 Keywords: AIM Flask
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `aim_flask-1.0.1/aim_flask.egg-info/PKG-INFO` & `aim_flask-1.0.2/aim_flask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim_flask
-Version: 1.0.1
+Version: 1.0.2
 Summary: A CLI tool for setting up and managing AIM environments
 Home-page: https://github.com/MrMayami/AIM
 Author: Joe Mayami
 Author-email: pr.mayami@gmail.com
 Project-URL: GitHub, https://github.com/MrMayami/AIM
 Keywords: AIM Flask
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `aim_flask-1.0.1/setup.py` & `aim_flask-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="aim_flask",  # Required
-    version="1.0.1",  # Required
+    version="1.0.2",  # Required
+    scripts=['aim_flask.py'],  # Add your script here
     description="A CLI tool for setting up and managing AIM environments",  # Optional
     long_description=long_description,  # Optional
     long_description_content_type="text/markdown",  # Optional
     url="https://github.com/MrMayami/AIM",  # Optional
     author="Joe Mayami",  # Optional
     author_email="pr.mayami@gmail.com",  # Optional
     classifiers=[  # Optional
@@ -35,15 +36,15 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     keywords="AIM Flask",  # Optional
     packages=find_packages(),  # Required
     python_requires=">=3.7, <4",  # Required
      entry_points={
         'console_scripts': [
-            'aim=aim_flask:main',
+            'aim=aim_flask:__main__',
         ],
     },
     install_requires=[],  # Optional
     project_urls={  # Optional
         "GitHub": "https://github.com/MrMayami/AIM",
     },
 )
```


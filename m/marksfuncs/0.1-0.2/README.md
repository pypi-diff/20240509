# Comparing `tmp/marksfuncs-0.1.tar.gz` & `tmp/marksfuncs-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marksfuncs-0.1.tar", last modified: Wed May  8 17:03:31 2024, max compression
+gzip compressed data, was "marksfuncs-0.2.tar", last modified: Thu May  9 13:39:36 2024, max compression
```

## Comparing `marksfuncs-0.1.tar` & `marksfuncs-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 17:03:31.890154 marksfuncs-0.1/
--rw-rw-rw-   0        0        0     1062 2024-05-07 19:04:53.000000 marksfuncs-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2239 2024-05-08 17:03:31.885145 marksfuncs-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1545 2024-05-08 15:43:53.000000 marksfuncs-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 17:03:31.841142 marksfuncs-0.1/marksfuncs/
--rw-rw-rw-   0        0        0       34 2024-05-07 18:33:28.000000 marksfuncs-0.1/marksfuncs/__init__.py
--rw-rw-rw-   0        0        0    54710 2024-05-07 19:04:55.000000 marksfuncs-0.1/marksfuncs/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-08 17:03:31.883145 marksfuncs-0.1/marksfuncs.egg-info/
--rw-rw-rw-   0        0        0     2239 2024-05-08 17:03:31.000000 marksfuncs-0.1/marksfuncs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-08 17:03:31.000000 marksfuncs-0.1/marksfuncs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 17:03:31.000000 marksfuncs-0.1/marksfuncs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-05-08 17:03:31.000000 marksfuncs-0.1/marksfuncs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 17:03:31.000000 marksfuncs-0.1/marksfuncs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 17:03:31.890154 marksfuncs-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1234 2024-05-08 17:02:35.000000 marksfuncs-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:39:36.425790 marksfuncs-0.2/
+-rw-rw-rw-   0        0        0     1062 2024-05-07 19:04:53.000000 marksfuncs-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2195 2024-05-09 13:39:36.422790 marksfuncs-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2024-05-08 18:32:10.000000 marksfuncs-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 13:39:36.390790 marksfuncs-0.2/marksfuncs/
+-rw-rw-rw-   0        0        0       34 2024-05-07 18:33:28.000000 marksfuncs-0.2/marksfuncs/__init__.py
+-rw-rw-rw-   0        0        0    67084 2024-05-08 18:30:47.000000 marksfuncs-0.2/marksfuncs/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:39:36.419790 marksfuncs-0.2/marksfuncs.egg-info/
+-rw-rw-rw-   0        0        0     2195 2024-05-09 13:39:36.000000 marksfuncs-0.2/marksfuncs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-09 13:39:36.000000 marksfuncs-0.2/marksfuncs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:39:36.000000 marksfuncs-0.2/marksfuncs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-09 13:39:36.000000 marksfuncs-0.2/marksfuncs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 13:39:36.000000 marksfuncs-0.2/marksfuncs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 13:39:36.428793 marksfuncs-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2024-05-08 18:06:34.000000 marksfuncs-0.2/setup.py
```

### Comparing `marksfuncs-0.1/LICENSE.txt` & `marksfuncs-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `marksfuncs-0.1/PKG-INFO` & `marksfuncs-0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: marksfuncs
-Version: 0.1
+Version: 0.2
 Summary: Graph many mathematical functions
+Home-page: https://github.com/marc1fino/marksfuncs
 Author: mark. (Marc Pérez)
 Author-email: <marcperezcarrasco2010@gmail.com>
 License: MIT
 Keywords: python,maths,graphics,functions,xy,mathematical functions
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -21,37 +22,34 @@
 
 A mathematical library to graph many mathematical functions in a plot.
 
 Developed by Marc Pérez (c) 2024
 
 ## Examples of How To Use
 
-Watch a function's parameters
+Show A Grafic
 
 ```python
-from marksfuncs import Linear
-
-# For Printing Parameters In Console
-print(Linear())
+from marksfuncs import Exponential
 
-# You Can Add It In Anything That Supports An String
-message = "I like bananas "
-print(message+Linear())
+Exponential(a=4, b=2, x_values_list=[-5, 5, 100])
 ```
 
-Make The Grafic Of Your Function
+Convert The Grafic to a Image
 
 ```python
-from marksfuncs import Exponential
+from marksfuncs import Linear
+from PIL import Image
 
-# Printing A Message When The Grafic Finished Showing
-print(Exponential(a=6, b=5, x_values_list=[-5, 5, 100]))
+# Create An Io Img Bytes
+img_buffer = Linear(m=3, b=5, x_values_list=[-5, 5, 100]).image()
 
-# Only Show The Grafic
-Exponential(a=4, b=2, x_values_list=[-5, 5, 100])
+# Will Show The Function Grafic As A Png File
+img = Image.open(img_buffer)
+img.show(title="Grafic Image")
 ```
 
 Graphics Explanation
 
 ![Graphic Example](https://i.ibb.co/fq240nZ/imagen-2024-05-07-205144279.png)
 
 ```python
```

### Comparing `marksfuncs-0.1/README.md` & `marksfuncs-0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,37 +2,34 @@
 
 A mathematical library to graph many mathematical functions in a plot.
 
 Developed by Marc Pérez (c) 2024
 
 ## Examples of How To Use
 
-Watch a function's parameters
+Show A Grafic
 
 ```python
-from marksfuncs import Linear
-
-# For Printing Parameters In Console
-print(Linear())
+from marksfuncs import Exponential
 
-# You Can Add It In Anything That Supports An String
-message = "I like bananas "
-print(message+Linear())
+Exponential(a=4, b=2, x_values_list=[-5, 5, 100])
 ```
 
-Make The Grafic Of Your Function
+Convert The Grafic to a Image
 
 ```python
-from marksfuncs import Exponential
+from marksfuncs import Linear
+from PIL import Image
 
-# Printing A Message When The Grafic Finished Showing
-print(Exponential(a=6, b=5, x_values_list=[-5, 5, 100]))
+# Create An Io Img Bytes
+img_buffer = Linear(m=3, b=5, x_values_list=[-5, 5, 100]).image()
 
-# Only Show The Grafic
-Exponential(a=4, b=2, x_values_list=[-5, 5, 100])
+# Will Show The Function Grafic As A Png File
+img = Image.open(img_buffer)
+img.show(title="Grafic Image")
 ```
 
 Graphics Explanation
 
 ![Graphic Example](https://i.ibb.co/fq240nZ/imagen-2024-05-07-205144279.png)
 
 ```python
```

### Comparing `marksfuncs-0.1/marksfuncs.egg-info/PKG-INFO` & `marksfuncs-0.2/marksfuncs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: marksfuncs
-Version: 0.1
+Version: 0.2
 Summary: Graph many mathematical functions
+Home-page: https://github.com/marc1fino/marksfuncs
 Author: mark. (Marc Pérez)
 Author-email: <marcperezcarrasco2010@gmail.com>
 License: MIT
 Keywords: python,maths,graphics,functions,xy,mathematical functions
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
@@ -21,37 +22,34 @@
 
 A mathematical library to graph many mathematical functions in a plot.
 
 Developed by Marc Pérez (c) 2024
 
 ## Examples of How To Use
 
-Watch a function's parameters
+Show A Grafic
 
 ```python
-from marksfuncs import Linear
-
-# For Printing Parameters In Console
-print(Linear())
+from marksfuncs import Exponential
 
-# You Can Add It In Anything That Supports An String
-message = "I like bananas "
-print(message+Linear())
+Exponential(a=4, b=2, x_values_list=[-5, 5, 100])
 ```
 
-Make The Grafic Of Your Function
+Convert The Grafic to a Image
 
 ```python
-from marksfuncs import Exponential
+from marksfuncs import Linear
+from PIL import Image
 
-# Printing A Message When The Grafic Finished Showing
-print(Exponential(a=6, b=5, x_values_list=[-5, 5, 100]))
+# Create An Io Img Bytes
+img_buffer = Linear(m=3, b=5, x_values_list=[-5, 5, 100]).image()
 
-# Only Show The Grafic
-Exponential(a=4, b=2, x_values_list=[-5, 5, 100])
+# Will Show The Function Grafic As A Png File
+img = Image.open(img_buffer)
+img.show(title="Grafic Image")
 ```
 
 Graphics Explanation
 
 ![Graphic Example](https://i.ibb.co/fq240nZ/imagen-2024-05-07-205144279.png)
 
 ```python
```

### Comparing `marksfuncs-0.1/setup.py` & `marksfuncs-0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.1'
+VERSION = '0.2'
 DESCRIPTION = 'Graph many mathematical functions'
 working_directory = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(working_directory, "README.md"), encoding='utf-8') as f:
     long_description1 = f.read()
 # Setting up
 setup(
     name="marksfuncs",
     version=VERSION,
     author="mark. (Marc Pérez)",
     author_email="<marcperezcarrasco2010@gmail.com>",
+    url='https://github.com/marc1fino/marksfuncs',
     description=DESCRIPTION,
     long_description=long_description1,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['numpy', 'matplotlib', 'scipy'],
     license='MIT',
     keywords=['python', 'maths', 'graphics', 'functions', 'xy', 'mathematical functions'],
```


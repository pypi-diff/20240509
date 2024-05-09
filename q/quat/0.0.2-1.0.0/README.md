# Comparing `tmp/quat-0.0.2.tar.gz` & `tmp/quat-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quat-0.0.2.tar", last modified: Thu Mar 28 00:00:26 2024, max compression
+gzip compressed data, was "quat-1.0.0.tar", last modified: Wed May  8 22:07:37 2024, max compression
```

## Comparing `quat-0.0.2.tar` & `quat-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 00:00:26.873419 quat-0.0.2/
--rw-rw-rw-   0        0        0     3244 2024-03-28 00:00:26.873419 quat-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2636 2024-03-27 22:55:11.000000 quat-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 00:00:26.842177 quat-0.0.2/quat/
--rw-rw-rw-   0        0        0       19 2024-03-26 17:54:59.000000 quat-0.0.2/quat/__init__.py
--rw-rw-rw-   0        0        0     4666 2024-03-26 17:55:05.000000 quat-0.0.2/quat/quat.py
-drwxrwxrwx   0        0        0        0 2024-03-28 00:00:26.857798 quat-0.0.2/quat.egg-info/
--rw-rw-rw-   0        0        0     3244 2024-03-28 00:00:26.000000 quat-0.0.2/quat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2024-03-28 00:00:26.000000 quat-0.0.2/quat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 00:00:26.000000 quat-0.0.2/quat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-28 00:00:26.000000 quat-0.0.2/quat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-28 00:00:26.873419 quat-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1227 2024-03-28 00:00:20.000000 quat-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:07:37.694157 quat-1.0.0/
+-rw-rw-rw-   0        0        0     3162 2024-05-08 22:07:37.693158 quat-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2555 2024-05-08 21:51:43.000000 quat-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 22:07:37.667227 quat-1.0.0/quat/
+-rw-rw-rw-   0        0        0       19 2024-03-26 17:54:59.000000 quat-1.0.0/quat/__init__.py
+-rw-rw-rw-   0        0        0     4666 2024-03-26 17:55:05.000000 quat-1.0.0/quat/quat.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:07:37.691201 quat-1.0.0/quat.egg-info/
+-rw-rw-rw-   0        0        0     3162 2024-05-08 22:07:37.000000 quat-1.0.0/quat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2024-05-08 22:07:37.000000 quat-1.0.0/quat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 22:07:37.000000 quat-1.0.0/quat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-08 22:07:37.000000 quat-1.0.0/quat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 22:07:37.695151 quat-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1231 2024-05-08 22:02:53.000000 quat-1.0.0/setup.py
```

### Comparing `quat-0.0.2/PKG-INFO` & `quat-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: quat
-Version: 0.0.2
+Version: 1.0.0
 Summary: A simple library for working with quaternions and vectors.
+Home-page: https://github.com/OmidAlek/quat
 Author: Majid Alekasir
 Author-email: <majid.alekasir@gmail.com>
 Keywords: python,quaternion,vector,XYZVector,IMU,DMP
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # Introduction
 ## Abstract
 This library is primarily derived from the contributions of Geir Istad and has been released as a pip-installable package. The main objective of this library is to streamline operations involving vectors and quaternions, particularly in the context of working with Inertial Measurement Units (IMUs).
 
-To install this package, execute the following command:
-
-`pip install quat`
-
 ## Library Structure and Functions
 * Quaternion:
     * **get_product**: Computes and returns the product of the current quaternion with another quaternion.
     * **get_conjugate**: Calculates and returns the conjugate of the quaternion.
     * **get_magnitude**: Determines and provides the magnitude of the quaternion.
     * **normalize**: Normalizes the quaternion to ensure unit length.
     * **get_normalized**: Retrieves the normalized form of the quaternion.
```

### Comparing `quat-0.0.2/README.md` & `quat-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # Introduction
 ## Abstract
 This library is primarily derived from the contributions of Geir Istad and has been released as a pip-installable package. The main objective of this library is to streamline operations involving vectors and quaternions, particularly in the context of working with Inertial Measurement Units (IMUs).
 
-To install this package, execute the following command:
-
-`pip install quat`
-
 ## Library Structure and Functions
 * Quaternion:
     * **get_product**: Computes and returns the product of the current quaternion with another quaternion.
     * **get_conjugate**: Calculates and returns the conjugate of the quaternion.
     * **get_magnitude**: Determines and provides the magnitude of the quaternion.
     * **normalize**: Normalizes the quaternion to ensure unit length.
     * **get_normalized**: Retrieves the normalized form of the quaternion.
```

### Comparing `quat-0.0.2/quat/quat.py` & `quat-1.0.0/quat/quat.py`

 * *Files identical despite different names*

### Comparing `quat-0.0.2/quat.egg-info/PKG-INFO` & `quat-1.0.0/quat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 Metadata-Version: 2.1
 Name: quat
-Version: 0.0.2
+Version: 1.0.0
 Summary: A simple library for working with quaternions and vectors.
+Home-page: https://github.com/OmidAlek/quat
 Author: Majid Alekasir
 Author-email: <majid.alekasir@gmail.com>
 Keywords: python,quaternion,vector,XYZVector,IMU,DMP
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
 # Introduction
 ## Abstract
 This library is primarily derived from the contributions of Geir Istad and has been released as a pip-installable package. The main objective of this library is to streamline operations involving vectors and quaternions, particularly in the context of working with Inertial Measurement Units (IMUs).
 
-To install this package, execute the following command:
-
-`pip install quat`
-
 ## Library Structure and Functions
 * Quaternion:
     * **get_product**: Computes and returns the product of the current quaternion with another quaternion.
     * **get_conjugate**: Calculates and returns the conjugate of the quaternion.
     * **get_magnitude**: Determines and provides the magnitude of the quaternion.
     * **normalize**: Normalizes the quaternion to ensure unit length.
     * **get_normalized**: Retrieves the normalized form of the quaternion.
```

### Comparing `quat-0.0.2/setup.py` & `quat-1.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '1.0.0'
 DESCRIPTION = 'A simple library for working with quaternions and vectors.'
 LONG_DESCRIPTION = 'This library is written by Geir Istad, aimed for working with vectors and quaternions obtained from IMU and DMP modules. I have simply made it available on PyPI.'
 
 # Setting up
 setup(
     name="quat",
     version=VERSION,
     author="Majid Alekasir",
     author_email="<majid.alekasir@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
+    url='https://github.com/OmidAlek/quat',
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'quaternion', 'vector', 'XYZVector', 'IMU', 'DMP'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
     ]
 )
```


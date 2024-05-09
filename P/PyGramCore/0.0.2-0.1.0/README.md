# Comparing `tmp/PyGramCore-0.0.2.tar.gz` & `tmp/pygramcore-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGramCore-0.0.2.tar", last modified: Mon May  6 17:10:27 2024, max compression
+gzip compressed data, was "pygramcore-0.1.0.tar", last modified: Thu May  9 13:26:07 2024, max compression
```

## Comparing `PyGramCore-0.0.2.tar` & `pygramcore-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.045757 PyGramCore-0.0.2/
--rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 PyGramCore-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4062 2024-05-06 17:10:27.044757 PyGramCore-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.043757 PyGramCore-0.0.2/PyGramCore.egg-info/
--rw-rw-rw-   0        0        0     4062 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-06 17:10:26.000000 PyGramCore-0.0.2/PyGramCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3336 2024-05-06 16:49:49.000000 PyGramCore-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-06 17:10:27.045757 PyGramCore-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1151 2024-05-06 16:54:23.000000 PyGramCore-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.033257 PyGramCore-0.0.2/src/
--rw-rw-rw-   0        0        0        0 2024-05-05 17:27:36.000000 PyGramCore-0.0.2/src/__init__.py
--rw-rw-rw-   0        0        0     6036 2024-05-06 13:11:25.000000 PyGramCore-0.0.2/src/auth.py
--rw-rw-rw-   0        0        0      240 2024-05-06 11:25:42.000000 PyGramCore-0.0.2/src/constants.py
--rw-rw-rw-   0        0        0      992 2024-05-06 13:12:51.000000 PyGramCore-0.0.2/src/driver.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.037258 PyGramCore-0.0.2/src/elements/
--rw-rw-rw-   0        0        0       71 2024-05-05 21:01:41.000000 PyGramCore-0.0.2/src/elements/Comment.py
--rw-rw-rw-   0        0        0      386 2024-05-05 20:01:12.000000 PyGramCore-0.0.2/src/elements/Post.py
--rw-rw-rw-   0        0        0      640 2024-05-05 20:01:24.000000 PyGramCore-0.0.2/src/elements/User.py
--rw-rw-rw-   0        0        0        0 2024-05-05 19:37:24.000000 PyGramCore-0.0.2/src/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.039756 PyGramCore-0.0.2/src/exceptions/
--rw-rw-rw-   0        0        0      222 2024-05-05 17:27:36.000000 PyGramCore-0.0.2/src/exceptions/Auth.py
--rw-rw-rw-   0        0        0      433 2024-05-06 11:27:24.000000 PyGramCore-0.0.2/src/exceptions/Format.py
--rw-rw-rw-   0        0        0        0 2024-05-06 13:12:23.000000 PyGramCore-0.0.2/src/exceptions/__init__.py
--rw-rw-rw-   0        0        0      364 2024-05-06 14:18:40.000000 PyGramCore-0.0.2/src/test.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:10:27.042257 PyGramCore-0.0.2/src/utils/
--rw-rw-rw-   0        0        0        0 2024-05-05 17:27:36.000000 PyGramCore-0.0.2/src/utils/__init__.py
--rw-rw-rw-   0        0        0      292 2024-05-05 19:01:19.000000 PyGramCore-0.0.2/src/utils/auth.py
--rw-rw-rw-   0        0        0     3592 2024-05-06 13:08:46.000000 PyGramCore-0.0.2/src/utils/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:07.943650 pygramcore-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 13:25:59.000000 pygramcore-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-09 13:26:07.939650 pygramcore-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:07.939650 pygramcore-0.1.0/PyGramCore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-09 13:26:07.000000 pygramcore-0.1.0/PyGramCore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 13:26:07.000000 pygramcore-0.1.0/PyGramCore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:26:07.000000 pygramcore-0.1.0/PyGramCore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 13:26:07.000000 pygramcore-0.1.0/PyGramCore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 13:26:07.000000 pygramcore-0.1.0/PyGramCore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-09 13:25:59.000000 pygramcore-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:26:07.943650 pygramcore-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-09 13:25:59.000000 pygramcore-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:07.939650 pygramcore-0.1.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:07.939650 pygramcore-0.1.0/src/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/elements/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/elements/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:07.939650 pygramcore-0.1.0/src/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/exceptions/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/exceptions/Format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/exceptions/Post.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/exceptions/User.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/pygram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:26:07.939650 pygramcore-0.1.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 13:25:59.000000 pygramcore-0.1.0/src/utils/misc.py
```

### Comparing `PyGramCore-0.0.2/LICENSE` & `pygramcore-0.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Joel Taylor
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Joel Taylor
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `PyGramCore-0.0.2/setup.py` & `pygramcore-0.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from setuptools import setup, find_packages
-from codecs import open
-from os import path
-
-NAME = "PyGramCore"
-VERSION = '0.0.2'
-DESCRIPTION = "A simple-to-use Instagram Python interface using Selenium."
-
-# Get the long description from the README file
-here = path.abspath(path.dirname(__file__))
-with open(path.join(here, "README.md"), encoding="utf-8") as f:
-    LONG_DESCRIPTION = f.read()
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type="text/markdown",
-    author="Joel Taylor",
-    author_email="contact@joeltaylor.business",
-    license="MIT",
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3.12",
-        "Programming Language :: Python :: Implementation :: CPython",
-    ],
-    keywords=["instagram", "instagram bot", "selenium", "automation", "bot"],
-    packages=find_packages(exclude=["docs", "tests"]),
-    install_requires=["selenium", "selenium-stealth"],
-    setup_requires=["setuptools>=38.6.0"],
-)
+from setuptools import setup, find_packages
+from codecs import open
+from os import path
+
+# Read version from VERSION file
+here = path.abspath(path.dirname(__file__))
+
+VERSION = "0.1.0"
+DESCRIPTION = "A simple-to-use Instagram Python interface using Selenium."
+
+# Get the long description from the README file
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
+    LONG_DESCRIPTION = f.read()
+
+setup(
+    name="PyGramCore",
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type="text/markdown",
+    author="Joel Taylor",
+    author_email="contact@joeltaylor.business",
+    license="MIT",
+    classifiers=[
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: Implementation :: CPython",
+    ],
+    keywords=["instagram", "instagram bot", "selenium", "automation", "bot"],
+    packages=find_packages(exclude=["docs", "tests"]),
+    install_requires=["selenium", "selenium-stealth"],
+    setup_requires=["setuptools>=38.6.0"],
+)
```


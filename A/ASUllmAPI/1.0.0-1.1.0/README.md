# Comparing `tmp/ASUllmAPI-1.0.0.tar.gz` & `tmp/asullmapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ASUllmAPI-1.0.0.tar", last modified: Wed Apr 10 17:55:14 2024, max compression
+gzip compressed data, was "asullmapi-1.1.0.tar", last modified: Thu May  9 17:04:11 2024, max compression
```

## Comparing `ASUllmAPI-1.0.0.tar` & `asullmapi-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 17:55:14.643378 ASUllmAPI-1.0.0/
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 17:55:14.641698 ASUllmAPI-1.0.0/ASUllmAPI/
--rw-r--r--   0 wenxing1   (503) staff       (20)      122 2024-04-10 16:26:59.000000 ASUllmAPI-1.0.0/ASUllmAPI/__init__.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     2229 2024-04-10 16:47:20.000000 ASUllmAPI-1.0.0/ASUllmAPI/api.py
--rw-r--r--   0 wenxing1   (503) staff       (20)     1910 2024-04-09 20:16:04.000000 ASUllmAPI-1.0.0/ASUllmAPI/model_config.py
-drwxr-xr-x   0 wenxing1   (503) staff       (20)        0 2024-04-10 17:55:14.642838 ASUllmAPI-1.0.0/ASUllmAPI.egg-info/
--rw-r--r--   0 wenxing1   (503) staff       (20)     7035 2024-04-10 17:55:14.000000 ASUllmAPI-1.0.0/ASUllmAPI.egg-info/PKG-INFO
--rw-r--r--   0 wenxing1   (503) staff       (20)      229 2024-04-10 17:55:14.000000 ASUllmAPI-1.0.0/ASUllmAPI.egg-info/SOURCES.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)        1 2024-04-10 17:55:14.000000 ASUllmAPI-1.0.0/ASUllmAPI.egg-info/dependency_links.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)       10 2024-04-10 17:55:14.000000 ASUllmAPI-1.0.0/ASUllmAPI.egg-info/top_level.txt
--rw-r--r--   0 wenxing1   (503) staff       (20)     1104 2024-04-09 20:19:27.000000 ASUllmAPI-1.0.0/LICENSE
--rw-r--r--   0 wenxing1   (503) staff       (20)     7035 2024-04-10 17:55:14.643139 ASUllmAPI-1.0.0/PKG-INFO
--rw-r--r--   0 wenxing1   (503) staff       (20)     6420 2024-04-10 17:44:56.000000 ASUllmAPI-1.0.0/README.md
--rw-r--r--   0 wenxing1   (503) staff       (20)      596 2024-04-10 17:54:21.000000 ASUllmAPI-1.0.0/pyproject.toml
--rw-r--r--   0 wenxing1   (503) staff       (20)       38 2024-04-10 17:55:14.643449 ASUllmAPI-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 17:04:11.475541 asullmapi-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-05-09 17:04:11.458401 asullmapi-1.1.0/ASUllmAPI/
+-rw-rw-rw-   0        0        0      169 2024-05-08 21:25:24.000000 asullmapi-1.1.0/ASUllmAPI/__init__.py
+-rw-rw-rw-   0        0        0     2980 2024-05-09 00:11:45.000000 asullmapi-1.1.0/ASUllmAPI/api.py
+-rw-rw-rw-   0        0        0     2006 2024-05-09 00:11:45.000000 asullmapi-1.1.0/ASUllmAPI/model_config.py
+-rw-rw-rw-   0        0        0     1680 2024-05-08 21:25:24.000000 asullmapi-1.1.0/ASUllmAPI/multithreading.py
+-rw-rw-rw-   0        0        0      666 2024-05-08 21:25:24.000000 asullmapi-1.1.0/ASUllmAPI/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:04:11.471183 asullmapi-1.1.0/ASUllmAPI.egg-info/
+-rw-rw-rw-   0        0        0     1367 2024-05-09 17:04:11.000000 asullmapi-1.1.0/ASUllmAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-05-09 17:04:11.000000 asullmapi-1.1.0/ASUllmAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 17:04:11.000000 asullmapi-1.1.0/ASUllmAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-09 17:04:11.000000 asullmapi-1.1.0/ASUllmAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 17:04:11.000000 asullmapi-1.1.0/ASUllmAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1124 2024-04-18 18:53:24.000000 asullmapi-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1367 2024-05-09 17:04:11.471183 asullmapi-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2024-05-09 17:00:30.000000 asullmapi-1.1.0/README.md
+-rw-rw-rw-   0        0        0      724 2024-05-08 21:25:24.000000 asullmapi-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 17:04:11.475541 asullmapi-1.1.0/setup.cfg
```

### Comparing `ASUllmAPI-1.0.0/LICENSE` & `asullmapi-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 AI Acceleration Team at Arizona State University
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
+MIT License
+
+Copyright (c) 2024 AI Acceleration Team at Arizona State University
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
 SOFTWARE.
```

### Comparing `ASUllmAPI-1.0.0/pyproject.toml` & `asullmapi-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-[project]
-name = "ASUllmAPI"
-version = "1.0.0"
-authors = [
-  { name="Stella Wenxing Liu", email="stellawenxingliu@gmail.com" },
-]
-description = "A simple python package to facilitate connection to ASU LLM API"
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization"
+[project]
+name = "ASUllmAPI"
+version = "1.1.0"
+authors = [
+    { name="Stella Wenxing Liu", email="stellawenxingliu@gmail.com" },
+    { name="Varun Shourie", email="svarun195@gmail.com" }
+]
+description = "A simple python package to facilitate connection to ASU LLM API"
+readme = "README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "requests",
+    "tqdm"
+]
+
+[project.urls]
+Homepage = "https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization"
 Issues = "https://github.com/ASU/aiml-ssmdv-student-support-ml-data-visualization/issues"
```


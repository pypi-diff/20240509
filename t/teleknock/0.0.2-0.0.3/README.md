# Comparing `tmp/teleknock-0.0.2.tar.gz` & `tmp/teleknock-0.0.3.tar.gz`

## Comparing `teleknock-0.0.2.tar` & `teleknock-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,13 @@
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 teleknock-0.0.2/teleknock/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 teleknock-0.0.2/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 teleknock-0.0.2/LICENSE
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 teleknock-0.0.2/README.md
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 teleknock-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 teleknock-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 teleknock-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 teleknock-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 teleknock-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 teleknock-0.0.3/.idea/teleknock.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 teleknock-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 teleknock-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 teleknock-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 teleknock-0.0.3/teleknock/__init__.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 teleknock-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 teleknock-0.0.3/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 teleknock-0.0.3/README.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 teleknock-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 teleknock-0.0.3/PKG-INFO
```

### Comparing `teleknock-0.0.2/LICENSE` & `teleknock-0.0.3/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-
-The MIT License (MIT)
-
-Copyright (c) 2023 Knowblesse
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
+
+The MIT License (MIT)
+
+Copyright (c) 2023 Knowblesse
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

### Comparing `teleknock-0.0.2/PKG-INFO` & `teleknock-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: teleknock
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package to call telegram
 Project-URL: Homepage, https://github.com/knowblesse/teleknock
 Project-URL: Bug Tracker, https://github.com/knowblesse/teleknock/issues
 Author-email: Knowblesse <knowblesse@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/robotcode_robot-0.82.0.tar.gz` & `tmp/robotcode_robot-0.82.1.tar.gz`

## Comparing `robotcode_robot-0.82.0.tar` & `robotcode_robot-0.82.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/__version__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/config/__init__.py
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/config/loader.py
--rw-r--r--   0        0        0    88642 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/config/model.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/config/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/__init__.py
--rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/document_cache_helper.py
--rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/entities.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/errors.py
--rw-r--r--   0        0        0    56251 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    97124 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/library_doc.py
--rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/model_helper.py
--rw-r--r--   0        0        0    89792 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/namespace.py
--rw-r--r--   0        0        0    50086 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/namespace_analyzer.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/workspace_config.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/utils/__init__.py
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/utils/ast.py
--rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/utils/markdownformatter.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/utils/match.py
--rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/utils/robot_path.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/utils/stubs.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/utils/variables.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/src/robotcode/robot/utils/visitor.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/LICENSE.txt
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/pyproject.toml
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 robotcode_robot-0.82.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/__version__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/config/__init__.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/config/loader.py
+-rw-r--r--   0        0        0    88642 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/config/model.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/config/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/__init__.py
+-rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/document_cache_helper.py
+-rw-r--r--   0        0        0    11110 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/entities.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/errors.py
+-rw-r--r--   0        0        0    56251 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    97124 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    29868 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/model_helper.py
+-rw-r--r--   0        0        0    89792 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/namespace.py
+-rw-r--r--   0        0        0    50086 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/namespace_analyzer.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/workspace_config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/__init__.py
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/ast.py
+-rw-r--r--   0        0        0    11621 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/markdownformatter.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/match.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/robot_path.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/stubs.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/variables.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/src/robotcode/robot/utils/visitor.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/LICENSE.txt
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/pyproject.toml
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 robotcode_robot-0.82.1/PKG-INFO
```

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/config/loader.py` & `robotcode_robot-0.82.1/src/robotcode/robot/config/loader.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/config/model.py` & `robotcode_robot-0.82.1/src/robotcode/robot/config/model.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/config/utils.py` & `robotcode_robot-0.82.1/src/robotcode/robot/config/utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/document_cache_helper.py` & `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/document_cache_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/entities.py` & `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/errors.py` & `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/errors.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/imports_manager.py` & `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/library_doc.py` & `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/model_helper.py` & `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/namespace.py` & `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/namespace_analyzer.py` & `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/namespace_analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/diagnostics/workspace_config.py` & `robotcode_robot-0.82.1/src/robotcode/robot/diagnostics/workspace_config.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/utils/ast.py` & `robotcode_robot-0.82.1/src/robotcode/robot/utils/ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/utils/markdownformatter.py` & `robotcode_robot-0.82.1/src/robotcode/robot/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/utils/match.py` & `robotcode_robot-0.82.1/src/robotcode/robot/utils/match.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/utils/robot_path.py` & `robotcode_robot-0.82.1/src/robotcode/robot/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/utils/stubs.py` & `robotcode_robot-0.82.1/src/robotcode/robot/utils/stubs.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/utils/variables.py` & `robotcode_robot-0.82.1/src/robotcode/robot/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/src/robotcode/robot/utils/visitor.py` & `robotcode_robot-0.82.1/src/robotcode/robot/utils/visitor.py`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/.gitignore` & `robotcode_robot-0.82.1/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/LICENSE.txt` & `robotcode_robot-0.82.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/README.md` & `robotcode_robot-0.82.1/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_robot-0.82.0/pyproject.toml` & `robotcode_robot-0.82.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
   "tomli>=1.1.0; python_version < '3.11'",
   "platformdirs>=3.2.0,<4.2.0",
-  "robotcode-core==0.82.0",
+  "robotcode-core==0.82.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://opencollective.com/robotcode"
 Documentation = "https://github.com/robotcodedev/robotcode#readme"
```

### Comparing `robotcode_robot-0.82.0/PKG-INFO` & `robotcode_robot-0.82.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-robot
-Version: 0.82.0
+Version: 0.82.1
 Summary: Support classes for RobotCode for handling Robot Framework projects.
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: platformdirs<4.2.0,>=3.2.0
-Requires-Dist: robotcode-core==0.82.0
+Requires-Dist: robotcode-core==0.82.1
 Requires-Dist: robotframework>=4.1.0
 Requires-Dist: tomli>=1.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # robotcode-robot
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-robot.svg)](https://pypi.org/project/robotcode-robot)
```


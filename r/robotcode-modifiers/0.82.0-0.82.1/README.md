# Comparing `tmp/robotcode_modifiers-0.82.0.tar.gz` & `tmp/robotcode_modifiers-0.82.1.tar.gz`

## Comparing `robotcode_modifiers-0.82.0.tar` & `robotcode_modifiers-0.82.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.0/src/robotcode/modifiers/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.0/src/robotcode/modifiers/__version__.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.0/src/robotcode/modifiers/longname_modifiers.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.0/src/robotcode/modifiers/py.typed
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.0/LICENSE.txt
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.0/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.0/pyproject.toml
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.0/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.1/src/robotcode/modifiers/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.1/src/robotcode/modifiers/__version__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.1/src/robotcode/modifiers/longname_modifiers.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.1/src/robotcode/modifiers/py.typed
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.1/LICENSE.txt
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.1/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.1/pyproject.toml
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 robotcode_modifiers-0.82.1/PKG-INFO
```

### Comparing `robotcode_modifiers-0.82.0/src/robotcode/modifiers/longname_modifiers.py` & `robotcode_modifiers-0.82.1/src/robotcode/modifiers/longname_modifiers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,61 @@
-from typing import Union
+from typing import Optional, Union
 
 from robot.api import SuiteVisitor
 from robot.running import TestCase, TestSuite
 
 
-class ByLongName(SuiteVisitor):
-    def __init__(self, *included: str) -> None:
+class _BaseSuiteVisitor(SuiteVisitor):
+    def __init__(self, *included: str, root_name: Optional[str] = None) -> None:
         super().__init__()
-        self.included = included
+        self.included = list(included)
+
+        self.root_name = root_name
+        self.real_root_name: Optional[str] = None
 
     def start_suite(self, suite: TestSuite) -> None:
-        suite.tests = [t for t in suite.tests if self._is_included(t)]
+        if self.real_root_name is None and self.root_name is not None:
+            self.real_root_name = suite.longname
+            new_included = []
+            for i in self.included:
+                if "." in i:
+                    root_name, rest = c if len(c := i.split(".", 1)) > 1 else (c, None)
+                    if root_name == self.root_name:
+                        if rest is not None:
+                            new_included.append(f"{self.real_root_name}.{rest}")
+                        else:
+                            new_included.append(f"{self.real_root_name}'")
+                    else:
+                        new_included.append(i)
+                else:
+                    new_included.append(i)
+            self.included = new_included
 
     def _is_included(self, test: Union[TestCase, TestSuite]) -> bool:
         names = []
         names.append(test.longname)
         current = test.parent
         while current:
-            names.append(current.longname)
+            if current.parent is None:
+                names.append(self.root_name if self.root_name is not None else current.longname)
+            else:
+                names.append(current.longname)
             current = current.parent
 
         return any((s in names) for s in self.included)
 
     def end_suite(self, suite: TestSuite) -> None:
         suite.suites = [s for s in suite.suites if s.test_count > 0]
 
 
-class ExcludedByLongName(SuiteVisitor):
-    def __init__(self, *included: str) -> None:
-        super().__init__()
-        self.included = included
-
+class ByLongName(_BaseSuiteVisitor):
     def start_suite(self, suite: TestSuite) -> None:
-        suite.tests = [t for t in suite.tests if not self._is_included(t)]
+        super().start_suite(suite)
 
-    def _is_included(self, test: Union[TestCase, TestSuite]) -> bool:
-        names = []
-        names.append(test.longname)
-        current = test.parent
-        while current:
-            names.append(current.longname)
-            current = current.parent
+        suite.tests = [t for t in suite.tests if self._is_included(t)]
 
-        return any((s in names) for s in self.included)
 
-    def end_suite(self, suite: TestSuite) -> None:
-        suite.suites = [s for s in suite.suites if s.test_count > 0]
+class ExcludedByLongName(_BaseSuiteVisitor):
+    def start_suite(self, suite: TestSuite) -> None:
+        super().start_suite(suite)
+
+        suite.tests = [t for t in suite.tests if not self._is_included(t)]
```

### Comparing `robotcode_modifiers-0.82.0/.gitignore` & `robotcode_modifiers-0.82.1/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_modifiers-0.82.0/LICENSE.txt` & `robotcode_modifiers-0.82.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_modifiers-0.82.0/README.md` & `robotcode_modifiers-0.82.1/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_modifiers-0.82.0/pyproject.toml` & `robotcode_modifiers-0.82.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotcode_modifiers-0.82.0/PKG-INFO` & `robotcode_modifiers-0.82.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-modifiers
-Version: 0.82.0
+Version: 0.82.1
 Summary: Some Robot Framework Modifiers for RobotCode
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
```


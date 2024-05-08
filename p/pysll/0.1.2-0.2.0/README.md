# Comparing `tmp/pysll-0.1.2.tar.gz` & `tmp/pysll-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysll-0.1.2.tar", last modified: Tue Mar 26 23:10:48 2024, max compression
+gzip compressed data, was "pysll-0.2.0.tar", last modified: Wed May  8 22:14:43 2024, max compression
```

## Comparing `pysll-0.1.2.tar` & `pysll-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2024-03-26 23:10:48.032788 pysll-0.1.2/
--rw-r--r--   0 bruno      (501) staff       (20)     1508 2024-03-06 20:19:52.000000 pysll-0.1.2/LICENSE
--rw-r--r--   0 bruno      (501) staff       (20)      297 2024-03-26 23:10:48.032379 pysll-0.1.2/PKG-INFO
--rw-r--r--   0 bruno      (501) staff       (20)     6811 2024-03-06 21:06:36.000000 pysll-0.1.2/README.md
--rw-r--r--   0 bruno      (501) staff       (20)      108 2024-03-06 20:20:06.000000 pysll-0.1.2/pyproject.toml
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2024-03-26 23:10:48.026363 pysll-0.1.2/pysll/
--rw-r--r--   0 bruno      (501) staff       (20)       94 2024-03-20 00:17:32.000000 pysll-0.1.2/pysll/__init__.py
--rw-r--r--   0 bruno      (501) staff       (20)    34766 2024-03-26 23:10:17.000000 pysll-0.1.2/pysll/constellation.py
--rw-r--r--   0 bruno      (501) staff       (20)     4370 2024-03-19 23:37:47.000000 pysll-0.1.2/pysll/decoders.py
--rw-r--r--   0 bruno      (501) staff       (20)     3482 2024-03-26 23:10:07.000000 pysll-0.1.2/pysll/exceptions.py
--rw-r--r--   0 bruno      (501) staff       (20)      332 2024-03-19 23:37:47.000000 pysll-0.1.2/pysll/feature_flags.py
--rw-r--r--   0 bruno      (501) staff       (20)   324076 2024-03-06 21:06:36.000000 pysll-0.1.2/pysll/functions.py
--rw-r--r--   0 bruno      (501) staff       (20)    33623 2024-03-19 19:53:19.000000 pysll-0.1.2/pysll/models.py
--rw-r--r--   0 bruno      (501) staff       (20)      288 2024-03-19 00:56:01.000000 pysll-0.1.2/pysll/parsers.py
--rw-r--r--   0 bruno      (501) staff       (20)     3119 2024-03-26 23:10:07.000000 pysll-0.1.2/pysll/utils.py
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2024-03-26 23:10:48.031511 pysll-0.1.2/pysll.egg-info/
--rw-r--r--   0 bruno      (501) staff       (20)      297 2024-03-26 23:10:47.000000 pysll-0.1.2/pysll.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (501) staff       (20)      525 2024-03-26 23:10:48.000000 pysll-0.1.2/pysll.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (501) staff       (20)        1 2024-03-26 23:10:47.000000 pysll-0.1.2/pysll.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (501) staff       (20)        1 2024-03-06 21:37:00.000000 pysll-0.1.2/pysll.egg-info/not-zip-safe
--rw-r--r--   0 bruno      (501) staff       (20)      105 2024-03-26 23:10:47.000000 pysll-0.1.2/pysll.egg-info/requires.txt
--rw-r--r--   0 bruno      (501) staff       (20)       12 2024-03-26 23:10:47.000000 pysll-0.1.2/pysll.egg-info/top_level.txt
--rw-r--r--   0 bruno      (501) staff       (20)      378 2024-03-26 23:10:48.033095 pysll-0.1.2/setup.cfg
--rw-r--r--   0 bruno      (501) staff       (20)       38 2024-03-06 20:20:06.000000 pysll-0.1.2/setup.py
-drwxr-xr-x   0 bruno      (501) staff       (20)        0 2024-03-26 23:10:48.030898 pysll-0.1.2/tests/
--rw-r--r--   0 bruno      (501) staff       (20)        0 2024-03-06 20:20:06.000000 pysll-0.1.2/tests/__init__.py
--rw-r--r--   0 bruno      (501) staff       (20)     1317 2024-03-20 00:40:13.000000 pysll-0.1.2/tests/conftest.py
--rw-r--r--   0 bruno      (501) staff       (20)    12987 2024-03-26 23:10:17.000000 pysll-0.1.2/tests/test_api.py
--rw-r--r--   0 bruno      (501) staff       (20)    10737 2024-03-20 00:40:13.000000 pysll-0.1.2/tests/test_constellation.py
--rw-r--r--   0 bruno      (501) staff       (20)     3638 2024-03-19 23:37:47.000000 pysll-0.1.2/tests/test_decoders.py
--rw-r--r--   0 bruno      (501) staff       (20)     2758 2024-03-06 21:06:36.000000 pysll-0.1.2/tests/test_variable_unit.py
+drwxr-xr-x   0 tfharrelson  (1000) tfharrelson  (1000)        0 2024-05-08 22:14:43.132221 pysll-0.2.0/
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)     1508 2024-03-13 16:48:12.000000 pysll-0.2.0/LICENSE
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)      321 2024-05-08 22:14:43.132221 pysll-0.2.0/PKG-INFO
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)     6811 2024-03-13 16:48:12.000000 pysll-0.2.0/README.md
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)      108 2024-03-22 03:22:12.000000 pysll-0.2.0/pyproject.toml
+drwxr-xr-x   0 tfharrelson  (1000) tfharrelson  (1000)        0 2024-05-08 22:14:43.132221 pysll-0.2.0/pysll/
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)       94 2024-03-22 03:22:12.000000 pysll-0.2.0/pysll/__init__.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)    34766 2024-04-30 21:29:36.000000 pysll-0.2.0/pysll/constellation.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)     4370 2024-03-22 03:22:12.000000 pysll-0.2.0/pysll/decoders.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)     3482 2024-03-22 03:22:12.000000 pysll-0.2.0/pysll/exceptions.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)      332 2024-03-22 03:22:12.000000 pysll-0.2.0/pysll/feature_flags.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)   324076 2024-03-22 03:22:12.000000 pysll-0.2.0/pysll/functions.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)    33904 2024-04-30 21:29:40.000000 pysll-0.2.0/pysll/models.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)    37333 2024-04-30 21:29:40.000000 pysll-0.2.0/pysll/unit_operations.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)     3119 2024-04-30 21:29:36.000000 pysll-0.2.0/pysll/utils.py
+drwxr-xr-x   0 tfharrelson  (1000) tfharrelson  (1000)        0 2024-05-08 22:14:43.132221 pysll-0.2.0/pysll.egg-info/
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)      321 2024-05-08 22:14:43.000000 pysll-0.2.0/pysll.egg-info/PKG-INFO
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)      533 2024-05-08 22:14:43.000000 pysll-0.2.0/pysll.egg-info/SOURCES.txt
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)        1 2024-05-08 22:14:43.000000 pysll-0.2.0/pysll.egg-info/dependency_links.txt
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)        1 2024-03-23 03:33:42.000000 pysll-0.2.0/pysll.egg-info/not-zip-safe
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)      105 2024-05-08 22:14:43.000000 pysll-0.2.0/pysll.egg-info/requires.txt
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)       12 2024-05-08 22:14:43.000000 pysll-0.2.0/pysll.egg-info/top_level.txt
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)      435 2024-05-08 22:14:43.132221 pysll-0.2.0/setup.cfg
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)       38 2024-03-13 16:48:12.000000 pysll-0.2.0/setup.py
+drwxr-xr-x   0 tfharrelson  (1000) tfharrelson  (1000)        0 2024-05-08 22:14:43.132221 pysll-0.2.0/tests/
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)        0 2024-03-22 03:22:12.000000 pysll-0.2.0/tests/__init__.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)     1317 2024-03-22 03:22:12.000000 pysll-0.2.0/tests/conftest.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)    14105 2024-04-30 21:29:40.000000 pysll-0.2.0/tests/test_api.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)    10737 2024-04-30 21:29:36.000000 pysll-0.2.0/tests/test_constellation.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)     3638 2024-03-22 03:22:12.000000 pysll-0.2.0/tests/test_decoders.py
+-rw-r--r--   0 tfharrelson  (1000) tfharrelson  (1000)     2758 2024-03-22 03:22:12.000000 pysll-0.2.0/tests/test_variable_unit.py
```

### Comparing `pysll-0.1.2/LICENSE` & `pysll-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/README.md` & `pysll-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/pysll/constellation.py` & `pysll-0.2.0/pysll/constellation.py`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/pysll/decoders.py` & `pysll-0.2.0/pysll/decoders.py`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/pysll/exceptions.py` & `pysll-0.2.0/pysll/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/pysll/functions.py` & `pysll-0.2.0/pysll/functions.py`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/pysll/models.py` & `pysll-0.2.0/pysll/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -726,14 +726,21 @@
             raise TypeError("The input dictionary did not have the correct 'data_type' value.")
 
         try:
             members = {
                 kname: klass
                 for (kname, klass) in inspect.getmembers(importlib.import_module("pysll.functions"), inspect.isclass)
             }
+            unit_op_members = {
+                kname: klass
+                for (kname, klass) in inspect.getmembers(
+                    importlib.import_module("pysll.unit_operations"), inspect.isclass
+                )
+            }
+            members.update(unit_op_members)
             klass = members[d["name"]]
             assert issubclass(klass, Function)
         except (KeyError, AssertionError):
             raise TypeError(
                 "Name of the input function is not supported. Either the name has been mispelled or "
                 "it is missing from this library."
             )
```

### Comparing `pysll-0.1.2/pysll/utils.py` & `pysll-0.2.0/pysll/utils.py`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/pysll.egg-info/SOURCES.txt` & `pysll-0.2.0/pysll.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 pysll/__init__.py
 pysll/constellation.py
 pysll/decoders.py
 pysll/exceptions.py
 pysll/feature_flags.py
 pysll/functions.py
 pysll/models.py
-pysll/parsers.py
+pysll/unit_operations.py
 pysll/utils.py
 pysll.egg-info/PKG-INFO
 pysll.egg-info/SOURCES.txt
 pysll.egg-info/dependency_links.txt
 pysll.egg-info/not-zip-safe
 pysll.egg-info/requires.txt
 pysll.egg-info/top_level.txt
```

### Comparing `pysll-0.1.2/tests/conftest.py` & `pysll-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/tests/test_api.py` & `pysll-0.2.0/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Option,
     Quantity,
     ResultPayload,
     Symbol,
     deserialize_item,
     serialize_item,
 )
+from pysll.unit_operations import Transfer
 
 
 def test_api_function_construction():
     """Test that checks we can properly build the Function class from a variety
     of sources, and we can serialize it into dicts."""
     func = Function([[1, 2], [2, 5], [3, 1]])
     assert func.inputs == [[[1, 2], [2, 5], [3, 1]]]
@@ -45,14 +46,33 @@
         }
     )
     assert type(func).__name__ == "AnalyzePeaks"
     assert func.inputs == [[[1, 2], [2, 5], [3, 1]]]
     assert func.options == [Option(name="AbsoluteThreshold", value=10.4)]
 
 
+def test_unit_op_construction():
+    """Test that checks we can properly build the unit operations from a
+    variety of sources, and we can serialize it into dicts."""
+
+    # make an api dict to check if we can build a function from that
+    func = Function.from_dict(
+        {
+            "name": "Transfer",
+            "data_type": "function",
+            "inputs": [],
+            "options": [
+                {"data_type": "option", "name": "AbsoluteThreshold", "value": {"data_type": "float", "value": 10.4}}
+            ],
+        }
+    )
+    assert type(func).__name__ == "Transfer"
+    assert func.options == [Option(name="AbsoluteThreshold", value=10.4)]
+
+
 def test_api_function_deserialization():
     """Test that checks we can properly deserialize a Function class into a
     dict."""
     # test out building with an option
     func = Function([[1, 2], [2, 5], [3, 1]], AbsoluteThreshold=10.4)
     func_dict = serialize_item(func)
     assert isinstance(func_dict, dict)
@@ -111,14 +131,26 @@
     assert len(peaks.options) == 2
     assert isinstance(peaks.options[0], Option)
     assert peaks.options[0].value == 10.34
     assert isinstance(peaks.options[1], Option)
     assert peaks.options[1].value is True
 
 
+def test_unit_ops_from_python():
+    """Test that AnalyzePeaks works as expected."""
+    t = Transfer(Source=Object("id:xyz"))
+    assert isinstance(t.inputs, list)
+    assert len(t.inputs) == 0
+    assert isinstance(t.options, list)
+    assert len(t.options) == 1
+    assert isinstance(t.options[0], Option)
+    assert isinstance(t.options[0].value, Object)
+    assert t.options[0].value.id == "id:xyz"
+
+
 def test_analyze_peaks_from_dict():
     """Test that creating AnalyzePeaks from dict works as expected."""
     peaks = Function.from_dict(
         {
             "data_type": "function",
             "name": "AnalyzePeaks",
             "inputs": [{"data_type": "object", "id": "id:xyz", "type": "Object.Data.Chromatography", "name": None}],
```

### Comparing `pysll-0.1.2/tests/test_constellation.py` & `pysll-0.2.0/tests/test_constellation.py`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/tests/test_decoders.py` & `pysll-0.2.0/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `pysll-0.1.2/tests/test_variable_unit.py` & `pysll-0.2.0/tests/test_variable_unit.py`

 * *Files identical despite different names*


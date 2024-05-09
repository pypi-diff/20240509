# Comparing `tmp/fontfinder-0.11.0.tar.gz` & `tmp/fontfinder-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fontfinder-0.11.0.tar", last modified: Sun Apr 28 14:02:11 2024, max compression
+gzip compressed data, was "fontfinder-0.12.0.tar", last modified: Thu May  9 12:15:46 2024, max compression
```

## Comparing `fontfinder-0.11.0.tar` & `fontfinder-0.12.0.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.863469 fontfinder-0.11.0/
--rw-r--r--   0 james      (501) staff       (20)     1070 2023-10-04 08:55:25.000000 fontfinder-0.11.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     4500 2024-04-28 14:02:11.858080 fontfinder-0.11.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     3447 2024-04-17 13:23:00.000000 fontfinder-0.11.0/README.md
--rw-r--r--   0 james      (501) staff       (20)     1140 2024-04-28 14:00:56.000000 fontfinder-0.11.0/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2024-04-28 14:02:11.863548 fontfinder-0.11.0/setup.cfg
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.806129 fontfinder-0.11.0/src/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.810732 fontfinder-0.11.0/src/fontfinder/
--rw-r--r--   0 james      (501) staff       (20)    27988 2024-04-28 13:54:54.000000 fontfinder-0.11.0/src/fontfinder/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1522 2024-04-16 12:22:58.000000 fontfinder-0.11.0/src/fontfinder/_generate_data.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.819050 fontfinder-0.11.0/src/fontfinder/_platforms/
--rw-r--r--   0 james      (501) staff       (20)     3464 2024-04-13 11:30:21.000000 fontfinder-0.11.0/src/fontfinder/_platforms/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     8109 2024-04-16 12:45:01.000000 fontfinder-0.11.0/src/fontfinder/_platforms/mac.py
--rw-r--r--   0 james      (501) staff       (20)    10212 2024-04-17 13:25:56.000000 fontfinder-0.11.0/src/fontfinder/_platforms/windows.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.844544 fontfinder-0.11.0/src/fontfinder/data/
--rw-r--r--   0 james      (501) staff       (20)  1011476 2024-04-06 08:01:13.000000 fontfinder-0.11.0/src/fontfinder/data/noto.json
--rw-r--r--   0 james      (501) staff       (20)   636190 2024-04-07 11:12:34.000000 fontfinder-0.11.0/src/fontfinder/data/small_unihan.json
--rw-r--r--   0 james      (501) staff       (20)     2408 2024-04-13 06:52:36.000000 fontfinder-0.11.0/src/fontfinder/filters.py
--rw-r--r--   0 james      (501) staff       (20)    17987 2024-04-13 11:37:30.000000 fontfinder-0.11.0/src/fontfinder/model.py
--rw-r--r--   0 james      (501) staff       (20)    11024 2023-10-05 11:12:34.000000 fontfinder-0.11.0/src/fontfinder/noto.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.855678 fontfinder-0.11.0/src/fontfinder.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     4500 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      554 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      175 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       11 2024-04-28 14:02:11.000000 fontfinder-0.11.0/src/fontfinder.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2024-04-28 14:02:11.854253 fontfinder-0.11.0/test/
--rw-r--r--   0 james      (501) staff       (20)    43525 2024-04-28 13:58:29.000000 fontfinder-0.11.0/test/test_fontfinder.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-09 12:15:46.590372 fontfinder-0.12.0/
+-rw-r--r--   0 james      (501) staff       (20)     1070 2023-10-04 08:55:25.000000 fontfinder-0.12.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     4535 2024-05-09 12:15:46.589643 fontfinder-0.12.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     3447 2024-04-17 13:23:00.000000 fontfinder-0.12.0/README.md
+-rw-r--r--   0 james      (501) staff       (20)     1258 2024-05-09 12:12:07.000000 fontfinder-0.12.0/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2024-05-09 12:15:46.590429 fontfinder-0.12.0/setup.cfg
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-09 12:15:46.573665 fontfinder-0.12.0/src/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-09 12:15:46.577872 fontfinder-0.12.0/src/fontfinder/
+-rw-r--r--   0 james      (501) staff       (20)    28232 2024-05-09 11:09:14.000000 fontfinder-0.12.0/src/fontfinder/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-09 12:15:46.584174 fontfinder-0.12.0/src/fontfinder/__pyinstaller/
+-rw-r--r--   0 james      (501) staff       (20)      202 2024-05-09 11:43:21.000000 fontfinder-0.12.0/src/fontfinder/__pyinstaller/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      198 2024-05-09 11:48:34.000000 fontfinder-0.12.0/src/fontfinder/__pyinstaller/hook-fontfinder.py
+-rw-r--r--   0 james      (501) staff       (20)     1633 2024-05-09 11:20:17.000000 fontfinder-0.12.0/src/fontfinder/_generate_data.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-09 12:15:46.585132 fontfinder-0.12.0/src/fontfinder/_platforms/
+-rw-r--r--   0 james      (501) staff       (20)     3464 2024-05-09 10:38:57.000000 fontfinder-0.12.0/src/fontfinder/_platforms/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     8109 2024-04-16 12:45:01.000000 fontfinder-0.12.0/src/fontfinder/_platforms/mac.py
+-rw-r--r--   0 james      (501) staff       (20)    10212 2024-04-17 13:25:56.000000 fontfinder-0.12.0/src/fontfinder/_platforms/windows.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-09 12:15:46.587572 fontfinder-0.12.0/src/fontfinder/data/
+-rw-r--r--   0 james      (501) staff       (20)  1011553 2024-05-09 11:12:30.000000 fontfinder-0.12.0/src/fontfinder/data/noto.json
+-rw-r--r--   0 james      (501) staff       (20)   636190 2024-05-09 11:23:22.000000 fontfinder-0.12.0/src/fontfinder/data/small_unihan.json
+-rw-r--r--   0 james      (501) staff       (20)     2408 2024-04-13 06:52:36.000000 fontfinder-0.12.0/src/fontfinder/filters.py
+-rw-r--r--   0 james      (501) staff       (20)    17987 2024-04-13 11:37:30.000000 fontfinder-0.12.0/src/fontfinder/model.py
+-rw-r--r--   0 james      (501) staff       (20)    11067 2024-05-09 11:11:20.000000 fontfinder-0.12.0/src/fontfinder/noto.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-09 12:15:46.588853 fontfinder-0.12.0/src/fontfinder.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     4535 2024-05-09 12:15:46.000000 fontfinder-0.12.0/src/fontfinder.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      684 2024-05-09 12:15:46.000000 fontfinder-0.12.0/src/fontfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2024-05-09 12:15:46.000000 fontfinder-0.12.0/src/fontfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       67 2024-05-09 12:15:46.000000 fontfinder-0.12.0/src/fontfinder.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)      195 2024-05-09 12:15:46.000000 fontfinder-0.12.0/src/fontfinder.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       11 2024-05-09 12:15:46.000000 fontfinder-0.12.0/src/fontfinder.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2024-05-09 12:15:46.588468 fontfinder-0.12.0/test/
+-rw-r--r--   0 james      (501) staff       (20)    43525 2024-04-28 13:58:29.000000 fontfinder-0.12.0/test/test_fontfinder.py
```

### Comparing `fontfinder-0.11.0/LICENSE` & `fontfinder-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fontfinder-0.11.0/PKG-INFO` & `fontfinder-0.12.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: fontfinder
-Version: 0.11.0
+Version: 0.12.0
 Summary: Package for finding and installing fonts for Unicode scripts.
 Project-URL: Documentation, https://multiscript.app/fontfinder
 Project-URL: Source, https://github.com/multiscript/fontfinder
 Project-URL: Issue Tracker, https://github.com/multiscript/fontfinder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: platformdirs>=4.2.1
 Requires-Dist: requests>=2.31
 Requires-Dist: semver>=3.0.2
 Requires-Dist: unicodedataplus>=15.1.0
 Requires-Dist: comtypes>=1.2.0; platform_system == "Windows"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: docs
```

### Comparing `fontfinder-0.11.0/README.md` & `fontfinder-0.12.0/README.md`

 * *Files identical despite different names*

### Comparing `fontfinder-0.11.0/pyproject.toml` & `fontfinder-0.12.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fontfinder"
-version = "0.11.0"
+version = "0.12.0"
 
 description = "Package for finding and installing fonts for Unicode scripts."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
+    "platformdirs>=4.2.1",
     "requests>=2.31",
     "semver>=3.0.2",
     "unicodedataplus>=15.1.0",
     "comtypes>=1.2.0;platform_system=='Windows'",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -43,7 +44,10 @@
 where = ["src"]  
 include = ["fontfinder*"]  
 exclude = ["tests*"] 
 namespaces = false
 
 [tool.setuptools.package-data]
 fontfinder = ["data/*.json"]
+
+[project.entry-points.pyinstaller40]
+hook-dirs = "fontfinder.__pyinstaller:get_hook_dirs"
```

### Comparing `fontfinder-0.11.0/src/fontfinder/__init__.py` & `fontfinder-0.12.0/src/fontfinder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,28 +74,33 @@
 '''
 from collections import Counter
 import json
 from pathlib import Path
 import tempfile
 from typing import Iterable
 
+import platformdirs
 import requests
 import unicodedataplus as udp
 
 from fontfinder.model import TextInfo
 from fontfinder.filters import *
 from fontfinder.model import *
 from fontfinder import _platforms
 
 
-_DATA_DIR_PATH = Path(__file__, "../data").resolve()
-'''Path to font data'''
-_DATA_DIR_PATH.mkdir(parents=True, exist_ok=True)
+_REF_DATA_DIR_PATH = Path(__file__, "../data").resolve()
+'''Path to reference font data (within package)'''
+_REF_DATA_DIR_PATH.mkdir(parents=True, exist_ok=True)
+
+_USER_DATA_DIR_PATH = platformdirs.user_data_path("fontfinder")
+'''Path to user data path for fontfinder (outside of package)'''
+_USER_DATA_DIR_PATH.mkdir(parents=True, exist_ok=True)
 
-_SMALL_UNIHAN_PATH = Path(_DATA_DIR_PATH, "small_unihan.json").resolve()
+_SMALL_UNIHAN_PATH = Path(_REF_DATA_DIR_PATH, "small_unihan.json").resolve()
 '''Path to subset of Unihan data neede for CJK font selection.'''
 
 # We wait until now to import Noto data so that data path constants above are set.
 from fontfinder import noto 
 
 
 class FontFinder:
```

### Comparing `fontfinder-0.11.0/src/fontfinder/_generate_data.py` & `fontfinder-0.12.0/src/fontfinder/_generate_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 
 import json
 from pathlib import Path
 import tempfile
 
-
 import fontfinder
 
-_FULL_UNIHAN_PATH = Path(fontfinder._DATA_DIR_PATH, "full_unihan.json").resolve()
-
 
 def generate_small_unihan():
     '''Utility function for creating a subset of the Unicode Unihan database needed by `fontfinder`.
-    This function recreates the local subset. As `fontfinder` is distributed with a working copy
-    of the subset (`small_unihan.json`) you should never need to call this method.'''
+    This function recreates the local subset. As `fontfinder` is distributed with a working reference
+    copy of the subset (`small_unihan.json`) you should never need to call this method.'''
     import unihan_etl.core
 
-    with tempfile.TemporaryDirectory() as work_dir:
-        packager_options = {
-            "destination": str(_FULL_UNIHAN_PATH),
-            "work_dir": work_dir,
-            "format": "json"
-        }
-        packager = unihan_etl.core.Packager(packager_options)
-        packager.download()
-        packager.export()
-
-    with open(_FULL_UNIHAN_PATH) as full_unihan_file:
-        with open(fontfinder._SMALL_UNIHAN_PATH, "w") as small_unihan_file:
-            full_records = json.load(full_unihan_file)
-            selected_keys = ['kTraditionalVariant', 'kSimplifiedVariant']
-            small_records = {}
-            for full_record in full_records:
-                small_entry = {key: value for key, value in full_record.items() if key in selected_keys}
-                if len(small_entry) > 0:
-                    small_records[full_record['char']] = small_entry
-            json.dump(small_records, small_unihan_file)
-    
-    _FULL_UNIHAN_PATH.unlink()
+    with tempfile.TemporaryDirectory() as full_unihan_dir:
+        full_unihan_path = Path(full_unihan_dir, "full_unihan.json").resolve()
 
+        with tempfile.TemporaryDirectory() as work_dir:
+            packager_options = {
+                "destination": str(full_unihan_path),
+                "work_dir": work_dir,
+                "format": "json"
+            }
+            packager = unihan_etl.core.Packager(packager_options)
+            packager.download()
+            packager.export()
+
+        with open(full_unihan_path) as full_unihan_file:
+            with open(fontfinder._SMALL_UNIHAN_PATH, "w") as small_unihan_file:
+                full_records = json.load(full_unihan_file)
+                selected_keys = ['kTraditionalVariant', 'kSimplifiedVariant']
+                small_records = {}
+                for full_record in full_records:
+                    small_entry = {key: value for key, value in full_record.items() if key in selected_keys}
+                    if len(small_entry) > 0:
+                        small_records[full_record['char']] = small_entry
+                json.dump(small_records, small_unihan_file)
+        
 
 if __name__ == '__main__':
     generate_small_unihan()
```

### Comparing `fontfinder-0.11.0/src/fontfinder/_platforms/__init__.py` & `fontfinder-0.12.0/src/fontfinder/_platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.11.0/src/fontfinder/_platforms/mac.py` & `fontfinder-0.12.0/src/fontfinder/_platforms/mac.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.11.0/src/fontfinder/_platforms/windows.py` & `fontfinder-0.12.0/src/fontfinder/_platforms/windows.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.11.0/src/fontfinder/data/noto.json` & `fontfinder-0.12.0/src/fontfinder/data/noto.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995249401363531%*

 * *Differences: {"'egyptian-hieroglyphs'": "{'families': {'Noto Sans Egyptian Hieroglyphs': {'latest_release': "*

 * *                           "{'notes': 'Noto Sans Egyptian Hieroglyphs v2.002\\n\\nThis release "*

 * *                           'adds support for various codepoints added in Unicode 14.\\nThanks to '*

 * *                           "@mercury13 (drawing) and @dwerning (consultancy).\\n', 'published': "*

 * *                           "'2024-04-15T09:29:21+00:00', 'url': "*

 * *                           "'https://github.com/notofon […]*

```diff
@@ -3069,34 +3069,29 @@
                     ],
                     "unhinted": [
                         "fonts/NotoSansEgyptianHieroglyphs/unhinted/otf/NotoSansEgyptianHieroglyphs-Regular.otf",
                         "fonts/NotoSansEgyptianHieroglyphs/unhinted/ttf/NotoSansEgyptianHieroglyphs-Regular.ttf"
                     ]
                 },
                 "latest_release": {
-                    "notes": "Noto Sans Egyptian Hieroglyphs v2.001\n\nThis release fixes a number of fontbakery fails.\n",
-                    "published": "2022-09-19T08:47:34",
-                    "url": "https://github.com/notofonts/egyptian-hieroglyphs/releases/tag/NotoSansEgyptianHieroglyphs-v2.001",
-                    "version": "v2.001"
+                    "notes": "Noto Sans Egyptian Hieroglyphs v2.002\n\nThis release adds support for various codepoints added in Unicode 14.\nThanks to @mercury13 (drawing) and @dwerning (consultancy).\n",
+                    "published": "2024-04-15T09:29:21+00:00",
+                    "url": "https://github.com/notofonts/egyptian-hieroglyphs/releases/tag/NotoSansEgyptianHieroglyphs-v2.002",
+                    "version": "v2.002"
                 }
             }
         },
         "gh_url": "https://notofonts.github.io/egyptian-hieroglyphs",
         "issues": [
             {
                 "number": 16,
                 "title": "Strange metrics?",
                 "url": "https://github.com/notofonts/egyptian-hieroglyphs/issues/16"
             },
             {
-                "number": 12,
-                "title": "Should we increase 25CC to the size of an average hiero?",
-                "url": "https://github.com/notofonts/egyptian-hieroglyphs/issues/12"
-            },
-            {
                 "number": 9,
                 "title": "May I make counting rods 3FA\u202640C thicker?",
                 "url": "https://github.com/notofonts/egyptian-hieroglyphs/issues/9"
             },
             {
                 "number": 7,
                 "title": "Font sometimes displays shifted ~200 units upwards",
@@ -5306,15 +5301,15 @@
                         "fonts/NotoRashiHebrew/full/ttf/NotoRashiHebrew-ExtraBold.ttf",
                         "fonts/NotoRashiHebrew/full/ttf/NotoRashiHebrew-ExtraLight.ttf",
                         "fonts/NotoRashiHebrew/full/ttf/NotoRashiHebrew-Light.ttf",
                         "fonts/NotoRashiHebrew/full/ttf/NotoRashiHebrew-Medium.ttf",
                         "fonts/NotoRashiHebrew/full/ttf/NotoRashiHebrew-Regular.ttf",
                         "fonts/NotoRashiHebrew/full/ttf/NotoRashiHebrew-SemiBold.ttf",
                         "fonts/NotoRashiHebrew/full/ttf/NotoRashiHebrew-Thin.ttf",
-                        "fonts/NotoRashiHebrew/full/variable-ttf/NotoRashiHebrew[wght].ttf"
+                        "fonts/NotoRashiHebrew/full/variable/NotoRashiHebrew[wght].ttf"
                     ],
                     "hinted": [
                         "fonts/NotoRashiHebrew/hinted/ttf/NotoRashiHebrew-Black.ttf",
                         "fonts/NotoRashiHebrew/hinted/ttf/NotoRashiHebrew-Bold.ttf",
                         "fonts/NotoRashiHebrew/hinted/ttf/NotoRashiHebrew-ExtraBold.ttf",
                         "fonts/NotoRashiHebrew/hinted/ttf/NotoRashiHebrew-ExtraLight.ttf",
                         "fonts/NotoRashiHebrew/hinted/ttf/NotoRashiHebrew-Light.ttf",
@@ -5339,22 +5334,22 @@
                         "fonts/NotoRashiHebrew/unhinted/ttf/NotoRashiHebrew-ExtraBold.ttf",
                         "fonts/NotoRashiHebrew/unhinted/ttf/NotoRashiHebrew-ExtraLight.ttf",
                         "fonts/NotoRashiHebrew/unhinted/ttf/NotoRashiHebrew-Light.ttf",
                         "fonts/NotoRashiHebrew/unhinted/ttf/NotoRashiHebrew-Medium.ttf",
                         "fonts/NotoRashiHebrew/unhinted/ttf/NotoRashiHebrew-Regular.ttf",
                         "fonts/NotoRashiHebrew/unhinted/ttf/NotoRashiHebrew-SemiBold.ttf",
                         "fonts/NotoRashiHebrew/unhinted/ttf/NotoRashiHebrew-Thin.ttf",
-                        "fonts/NotoRashiHebrew/unhinted/variable-ttf/NotoRashiHebrew[wght].ttf"
+                        "fonts/NotoRashiHebrew/unhinted/variable/NotoRashiHebrew[wght].ttf"
                     ]
                 },
                 "latest_release": {
-                    "notes": "Noto Rashi Hebrew v1.006\n\nThis release replaces the Latin subset in full builds with Noto Serif.\n",
-                    "published": "2022-07-25T08:08:17",
-                    "url": "https://github.com/notofonts/hebrew/releases/tag/NotoRashiHebrew-v1.006",
-                    "version": "v1.006"
+                    "notes": "Noto Rashi Hebrew v1.007\n\nThis release:\n\n* Fixes interpolation issues (#35)\n* Corrects the width (#39) and position of marks under double-yud and double-vov (#38, thanks to @markhdavid)\n* Improves the anchoring of yod (#40, thanks to @markhdavid)\n* Adds the U+053F yod triangle character (#46)\n* Improves the spacing of tsadi (#33)\n",
+                    "published": "2024-04-22T14:08:01+00:00",
+                    "url": "https://github.com/notofonts/hebrew/releases/tag/NotoRashiHebrew-v1.007",
+                    "version": "v1.007"
                 }
             },
             "Noto Sans Hebrew": {
                 "files": {
                     "full": [
                         "fonts/NotoSansHebrew/full/otf/NotoSansHebrew-Black.otf",
                         "fonts/NotoSansHebrew/full/otf/NotoSansHebrew-Bold.otf",
@@ -5425,15 +5420,15 @@
                         "fonts/NotoSansHebrew/full/ttf/NotoSansHebrew-SemiCondensedExtraBold.ttf",
                         "fonts/NotoSansHebrew/full/ttf/NotoSansHebrew-SemiCondensedExtraLight.ttf",
                         "fonts/NotoSansHebrew/full/ttf/NotoSansHebrew-SemiCondensedLight.ttf",
                         "fonts/NotoSansHebrew/full/ttf/NotoSansHebrew-SemiCondensedMedium.ttf",
                         "fonts/NotoSansHebrew/full/ttf/NotoSansHebrew-SemiCondensedSemiBold.ttf",
                         "fonts/NotoSansHebrew/full/ttf/NotoSansHebrew-SemiCondensedThin.ttf",
                         "fonts/NotoSansHebrew/full/ttf/NotoSansHebrew-Thin.ttf",
-                        "fonts/NotoSansHebrew/full/variable-ttf/NotoSansHebrew[wdth,wght].ttf"
+                        "fonts/NotoSansHebrew/full/variable/NotoSansHebrew[wdth,wght].ttf"
                     ],
                     "hinted": [
                         "fonts/NotoSansHebrew/hinted/ttf/NotoSansHebrew-Black.ttf",
                         "fonts/NotoSansHebrew/hinted/ttf/NotoSansHebrew-Bold.ttf",
                         "fonts/NotoSansHebrew/hinted/ttf/NotoSansHebrew-Condensed.ttf",
                         "fonts/NotoSansHebrew/hinted/ttf/NotoSansHebrew-CondensedBlack.ttf",
                         "fonts/NotoSansHebrew/hinted/ttf/NotoSansHebrew-CondensedBold.ttf",
@@ -5539,22 +5534,22 @@
                         "fonts/NotoSansHebrew/unhinted/ttf/NotoSansHebrew-SemiCondensedExtraBold.ttf",
                         "fonts/NotoSansHebrew/unhinted/ttf/NotoSansHebrew-SemiCondensedExtraLight.ttf",
                         "fonts/NotoSansHebrew/unhinted/ttf/NotoSansHebrew-SemiCondensedLight.ttf",
                         "fonts/NotoSansHebrew/unhinted/ttf/NotoSansHebrew-SemiCondensedMedium.ttf",
                         "fonts/NotoSansHebrew/unhinted/ttf/NotoSansHebrew-SemiCondensedSemiBold.ttf",
                         "fonts/NotoSansHebrew/unhinted/ttf/NotoSansHebrew-SemiCondensedThin.ttf",
                         "fonts/NotoSansHebrew/unhinted/ttf/NotoSansHebrew-Thin.ttf",
-                        "fonts/NotoSansHebrew/unhinted/variable-ttf/NotoSansHebrew[wdth,wght].ttf"
+                        "fonts/NotoSansHebrew/unhinted/variable/NotoSansHebrew[wdth,wght].ttf"
                     ]
                 },
                 "latest_release": {
-                    "notes": "Noto Sans Hebrew v2.003\n\nThis is an administrative release.\n",
-                    "published": "2022-07-15T08:08:34",
-                    "url": "https://github.com/notofonts/hebrew/releases/tag/NotoSansHebrew-v2.003",
-                    "version": "v2.003"
+                    "notes": "Noto Sans Hebrew v2.004\n\nThis release:\n\n* Fixes interpolation issues\n* Corrects the width (#39) and position of marks under double-yud and double-vov (#38, thanks to @markhdavid)\n* Removes semibold masters\n* Adds the U+053F yod triangle character (#46)\n* Improves the spacing of decomposed dagesh forms (#47)\n",
+                    "published": "2024-04-22T13:35:47+00:00",
+                    "url": "https://github.com/notofonts/hebrew/releases/tag/NotoSansHebrew-v2.004",
+                    "version": "v2.004"
                 }
             },
             "Noto Serif Hebrew": {
                 "files": {
                     "full": [
                         "fonts/NotoSerifHebrew/full/otf/NotoSerifHebrew-Black.otf",
                         "fonts/NotoSerifHebrew/full/otf/NotoSerifHebrew-Bold.otf",
@@ -5625,15 +5620,15 @@
                         "fonts/NotoSerifHebrew/full/ttf/NotoSerifHebrew-SemiCondensedExtraBold.ttf",
                         "fonts/NotoSerifHebrew/full/ttf/NotoSerifHebrew-SemiCondensedExtraLight.ttf",
                         "fonts/NotoSerifHebrew/full/ttf/NotoSerifHebrew-SemiCondensedLight.ttf",
                         "fonts/NotoSerifHebrew/full/ttf/NotoSerifHebrew-SemiCondensedMedium.ttf",
                         "fonts/NotoSerifHebrew/full/ttf/NotoSerifHebrew-SemiCondensedSemiBold.ttf",
                         "fonts/NotoSerifHebrew/full/ttf/NotoSerifHebrew-SemiCondensedThin.ttf",
                         "fonts/NotoSerifHebrew/full/ttf/NotoSerifHebrew-Thin.ttf",
-                        "fonts/NotoSerifHebrew/full/variable-ttf/NotoSerifHebrew[wdth,wght].ttf"
+                        "fonts/NotoSerifHebrew/full/variable/NotoSerifHebrew[wdth,wght].ttf"
                     ],
                     "hinted": [
                         "fonts/NotoSerifHebrew/hinted/ttf/NotoSerifHebrew-Black.ttf",
                         "fonts/NotoSerifHebrew/hinted/ttf/NotoSerifHebrew-Bold.ttf",
                         "fonts/NotoSerifHebrew/hinted/ttf/NotoSerifHebrew-Condensed.ttf",
                         "fonts/NotoSerifHebrew/hinted/ttf/NotoSerifHebrew-CondensedBlack.ttf",
                         "fonts/NotoSerifHebrew/hinted/ttf/NotoSerifHebrew-CondensedBold.ttf",
@@ -5739,48 +5734,53 @@
                         "fonts/NotoSerifHebrew/unhinted/ttf/NotoSerifHebrew-SemiCondensedExtraBold.ttf",
                         "fonts/NotoSerifHebrew/unhinted/ttf/NotoSerifHebrew-SemiCondensedExtraLight.ttf",
                         "fonts/NotoSerifHebrew/unhinted/ttf/NotoSerifHebrew-SemiCondensedLight.ttf",
                         "fonts/NotoSerifHebrew/unhinted/ttf/NotoSerifHebrew-SemiCondensedMedium.ttf",
                         "fonts/NotoSerifHebrew/unhinted/ttf/NotoSerifHebrew-SemiCondensedSemiBold.ttf",
                         "fonts/NotoSerifHebrew/unhinted/ttf/NotoSerifHebrew-SemiCondensedThin.ttf",
                         "fonts/NotoSerifHebrew/unhinted/ttf/NotoSerifHebrew-Thin.ttf",
-                        "fonts/NotoSerifHebrew/unhinted/variable-ttf/NotoSerifHebrew[wdth,wght].ttf"
+                        "fonts/NotoSerifHebrew/unhinted/variable/NotoSerifHebrew[wdth,wght].ttf"
                     ]
                 },
                 "latest_release": {
-                    "notes": "Noto Serif Hebrew v2.003\n\nThis is a maintenance release.\n",
-                    "published": "2022-07-13T13:28:21",
-                    "url": "https://github.com/notofonts/hebrew/releases/tag/NotoSerifHebrew-v2.003",
-                    "version": "v2.003"
+                    "notes": "Noto Serif Hebrew v2.004\n\nThis release:\n\n* Corrects the position of marks under double-yud and double-vov (#38, thanks to @markhdavid)\n* Adds the U+053F yod triangle character (#46)\n",
+                    "published": "2024-04-22T14:00:25+00:00",
+                    "url": "https://github.com/notofonts/hebrew/releases/tag/NotoSerifHebrew-v2.004",
+                    "version": "v2.004"
                 }
             }
         },
         "gh_url": "https://notofonts.github.io/hebrew",
         "issues": [
             {
-                "number": 46,
-                "title": "U+05EF missing",
-                "url": "https://github.com/notofonts/hebrew/issues/46"
+                "number": 50,
+                "title": "Overlap issues with shin dot and holam",
+                "url": "https://github.com/notofonts/hebrew/issues/50"
+            },
+            {
+                "number": 48,
+                "title": "Diamond dots?",
+                "url": "https://github.com/notofonts/hebrew/issues/48"
+            },
+            {
+                "number": 47,
+                "title": "Dagesh overlaps in heavier weights of Noto Sans Hebrew",
+                "url": "https://github.com/notofonts/hebrew/issues/47"
             },
             {
                 "number": 37,
                 "title": "Noto Rashi Hebrew - no support for U+FB4F (Hebrew Ligature Alef Lamed)",
                 "url": "https://github.com/notofonts/hebrew/issues/37"
             },
             {
                 "number": 36,
                 "title": "Noto Rashi Hebrew - no support for U+FB1E (Hebrew Point Judeo-Spanish Varika)",
                 "url": "https://github.com/notofonts/hebrew/issues/36"
             },
             {
-                "number": 33,
-                "title": "Kerning of the letter \u05e6",
-                "url": "https://github.com/notofonts/hebrew/issues/33"
-            },
-            {
                 "number": 12,
                 "title": "Overlapping Hebrew vowel signs",
                 "url": "https://github.com/notofonts/hebrew/issues/12"
             },
             {
                 "number": 10,
                 "title": "Hebrew script does not have a mono version",
@@ -8887,14 +8887,34 @@
                     "version": "v2.009"
                 }
             }
         },
         "gh_url": "https://notofonts.github.io/latin-greek-cyrillic",
         "issues": [
             {
+                "number": 476,
+                "title": "Wrong font families",
+                "url": "https://github.com/notofonts/latin-greek-cyrillic/issues/476"
+            },
+            {
+                "number": 475,
+                "title": "Kerning problem in with Greek capital A in Noto Serif italics",
+                "url": "https://github.com/notofonts/latin-greek-cyrillic/issues/475"
+            },
+            {
+                "number": 474,
+                "title": "Kerning and overlapping issues in heavier weights of Noto Serif",
+                "url": "https://github.com/notofonts/latin-greek-cyrillic/issues/474"
+            },
+            {
+                "number": 472,
+                "title": "-> symbols don't align very well",
+                "url": "https://github.com/notofonts/latin-greek-cyrillic/issues/472"
+            },
+            {
                 "number": 470,
                 "title": "Add U+1DFA",
                 "url": "https://github.com/notofonts/latin-greek-cyrillic/issues/470"
             },
             {
                 "number": 469,
                 "title": "Noto Sans Missed Characters `partialdiff`, `increment` (Delta) and more.",
@@ -10464,102 +10484,57 @@
                     "version": "v2.539"
                 }
             }
         },
         "gh_url": "https://notofonts.github.io/math",
         "issues": [
             {
-                "number": 67,
-                "title": "Request for a bold math font for use in section and title headers",
-                "url": "https://github.com/notofonts/math/issues/67"
-            },
-            {
-                "number": 66,
-                "title": "Add missing Arabic math symbols",
-                "url": "https://github.com/notofonts/math/issues/66"
+                "number": 81,
+                "title": "Sync Greek with Noto Sans",
+                "url": "https://github.com/notofonts/math/issues/81"
             },
             {
-                "number": 65,
-                "title": "Support all characters that have defined macros in unicode-math LaTeX package",
-                "url": "https://github.com/notofonts/math/issues/65"
+                "number": 77,
+                "title": "Make serif as a stub, just to recycle existing serif glyphs",
+                "url": "https://github.com/notofonts/math/issues/77"
             },
             {
-                "number": 64,
-                "title": "Arabic math alpahabet needs redesign",
-                "url": "https://github.com/notofonts/math/issues/64"
+                "number": 73,
+                "title": "Inconsistent kerning",
+                "url": "https://github.com/notofonts/math/issues/73"
             },
             {
-                "number": 63,
-                "title": "Redesigns",
-                "url": "https://github.com/notofonts/math/pull/63"
+                "number": 71,
+                "title": "Alpha and kappa are a bit too close to their latin lookalikes",
+                "url": "https://github.com/notofonts/math/issues/71"
             },
             {
-                "number": 62,
-                "title": "Why does the source include `gcommaaccent`?",
-                "url": "https://github.com/notofonts/math/issues/62"
+                "number": 67,
+                "title": "Request for a bold math font for use in section and title headers",
+                "url": "https://github.com/notofonts/math/issues/67"
             },
             {
                 "number": 61,
                 "title": "Chancery style should be the default for script math alpahebt",
                 "url": "https://github.com/notofonts/math/issues/61"
             },
             {
-                "number": 60,
-                "title": "Binary and relational operators are too small and misaligned vertically",
-                "url": "https://github.com/notofonts/math/issues/60"
-            },
-            {
-                "number": 59,
-                "title": "Monospace math alphanumeric glyphs are not distinguishable from sans-serif ones ",
-                "url": "https://github.com/notofonts/math/issues/59"
-            },
-            {
                 "number": 58,
                 "title": "`ssty` variants are too bold",
                 "url": "https://github.com/notofonts/math/issues/58"
             },
             {
-                "number": 54,
-                "title": "Request to consider splitting Noto Sans Math into two fonts---a serif and a sans serif one",
-                "url": "https://github.com/notofonts/math/issues/54"
-            },
-            {
-                "number": 53,
-                "title": "Minusplus symbol misaligned",
-                "url": "https://github.com/notofonts/math/issues/53"
-            },
-            {
-                "number": 52,
-                "title": "Sans coproduct sign is confusable with disjoint union",
-                "url": "https://github.com/notofonts/math/issues/52"
-            },
-            {
-                "number": 51,
-                "title": "Integrals are too upright and confusable with brackets/lines",
-                "url": "https://github.com/notofonts/math/issues/51"
-            },
-            {
-                "number": 44,
-                "title": "Wrong symbols for multi-storey brackets",
-                "url": "https://github.com/notofonts/math/issues/44"
-            },
-            {
                 "number": 36,
                 "title": "U+2044 FRACTION SLASH does not create vulgar fractions",
                 "url": "https://github.com/notofonts/math/issues/36"
             },
             {
                 "number": 7,
                 "title": "Best-fit Bidi_Mirroring_Glyph could be better",
                 "url": "https://github.com/notofonts/math/issues/7"
-            },
-            {
-                "number": 5,
-                "title": "Missing anchor points in Noto Sans Math",
-                "url": "https://github.com/notofonts/math/issues/5"
             }
         ],
         "repo_url": "https://www.github.com/notofonts/math",
         "tier": 3,
         "title": "Noto Math"
     },
     "mayan-numerals": {
@@ -11740,14 +11715,19 @@
                     "version": "v3.009"
                 }
             }
         },
         "gh_url": "https://notofonts.github.io/nastaliq",
         "issues": [
             {
+                "number": 66,
+                "title": "Missing ligatures",
+                "url": "https://github.com/notofonts/nastaliq/issues/66"
+            },
+            {
                 "number": 65,
                 "title": "Need Help With Android font issue",
                 "url": "https://github.com/notofonts/nastaliq/issues/65"
             },
             {
                 "number": 64,
                 "title": "dot collision, lam followed by peh",
@@ -12161,19 +12141,14 @@
                     "version": "v2.005"
                 }
             }
         },
         "gh_url": "https://notofonts.github.io/old-hungarian",
         "issues": [
             {
-                "number": 17,
-                "title": "It might to good thing add syllable like ligatures.",
-                "url": "https://github.com/notofonts/old-hungarian/issues/17"
-            },
-            {
                 "number": 16,
                 "title": "Small and capital letter must be aligned to a baseline.",
                 "url": "https://github.com/notofonts/old-hungarian/issues/16"
             },
             {
                 "number": 15,
                 "title": "Old Hungarian font need capital ligatures, and several ligspec must not in the disc regio",
@@ -14117,24 +14092,24 @@
                     "version": "v2.008"
                 }
             }
         },
         "gh_url": "https://notofonts.github.io/symbols",
         "issues": [
             {
+                "number": 83,
+                "title": "Starting work on U16 legacy ex?",
+                "url": "https://github.com/notofonts/symbols/issues/83"
+            },
+            {
                 "number": 82,
                 "title": "Character spacing problem \u266d\u266f\u266e",
                 "url": "https://github.com/notofonts/symbols/issues/82"
             },
             {
-                "number": 81,
-                "title": "U+1D377 \"\ud834\udf77\" TALLY MARK ONE is spaced improperly",
-                "url": "https://github.com/notofonts/symbols/issues/81"
-            },
-            {
                 "number": 80,
                 "title": "U+2FFC-2FFF, U+31EF: Five additional \"Ideographic description characters\", newly assigned in Unicode 15.1.0 (September, 2023)",
                 "url": "https://github.com/notofonts/symbols/issues/80"
             },
             {
                 "number": 75,
                 "title": "Alchemical symbols change in Unicode 15.1",
@@ -14292,14 +14267,19 @@
                     "version": "v3.000"
                 }
             }
         },
         "gh_url": "https://notofonts.github.io/syriac",
         "issues": [
             {
+                "number": 26,
+                "title": "Weights 200, 300, 500-800 present on Google Fonts but not here (even in googlefonts/, for all three variants)",
+                "url": "https://github.com/notofonts/syriac/issues/26"
+            },
+            {
                 "number": 24,
                 "title": "Interpolation problems in `NotoSansSyriac[wght].ttf`",
                 "url": "https://github.com/notofonts/syriac/issues/24"
             },
             {
                 "number": 22,
                 "title": "[fonts.google.com user feedback] Dot and mark positioning",
@@ -15942,18 +15922,18 @@
                     ],
                     "unhinted": [
                         "fonts/NotoSansTest/unhinted/otf/NotoSansTest-Regular.otf",
                         "fonts/NotoSansTest/unhinted/ttf/NotoSansTest-Regular.ttf"
                     ]
                 },
                 "latest_release": {
-                    "notes": "Ported from noto-source",
-                    "published": "2022-06-20T15:10:02",
-                    "url": "https://github.com/notofonts/test/releases/tag/NotoSansTest-v1.000",
-                    "version": "v1.000"
+                    "notes": "Noto Sans Test v1.002\n\nThere are no changes in this release.\n",
+                    "published": "2024-04-15T10:03:54+00:00",
+                    "url": "https://github.com/notofonts/test/releases/tag/NotoSansTest-v1.002",
+                    "version": "v1.002"
                 }
             },
             "Noto Serif Test": {
                 "files": {
                     "full": [
                         "fonts/NotoSerifTest/full/otf/NotoSerifTest-Bold.otf",
                         "fonts/NotoSerifTest/full/otf/NotoSerifTest-Regular.otf",
@@ -16870,15 +16850,15 @@
                 }
             }
         },
         "gh_url": "https://notofonts.github.io/tifinagh",
         "issues": [
             {
                 "number": 19,
-                "title": "Hello, I found an issue with a ligature, it is mentioned in the file attached",
+                "title": "Ligature issues.",
                 "url": "https://github.com/notofonts/tifinagh/issues/19"
             },
             {
                 "number": 8,
                 "title": "Half-implemented variant Tifinagh glyphs at inappropriate code points",
                 "url": "https://github.com/notofonts/tifinagh/issues/8"
             },
```

### Comparing `fontfinder-0.11.0/src/fontfinder/data/small_unihan.json` & `fontfinder-0.12.0/src/fontfinder/data/small_unihan.json`

 * *Files identical despite different names*

### Comparing `fontfinder-0.11.0/src/fontfinder/filters.py` & `fontfinder-0.12.0/src/fontfinder/filters.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.11.0/src/fontfinder/model.py` & `fontfinder-0.12.0/src/fontfinder/model.py`

 * *Files identical despite different names*

### Comparing `fontfinder-0.11.0/src/fontfinder/noto.py` & `fontfinder-0.12.0/src/fontfinder/noto.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 NOTO_MAIN_BASE_URL = "https://cdn.jsdelivr.net/gh/notofonts/notofonts.github.io/"
 '''Base URL of main Noto font download location.'''
 
 NOTO_CJK_BASE_URL = "https://github.com/notofonts/noto-cjk/raw/main/"
 '''Base URL of CJK Noto font download location.'''
 
 
-_NOTO_MAIN_JSON_REF_PATH = Path(fontfinder._DATA_DIR_PATH, "noto.json").resolve()
+_NOTO_MAIN_JSON_REF_PATH = Path(fontfinder._REF_DATA_DIR_PATH, "noto.json").resolve()
 '''Path of reference copy of noto.json distributed with this package.'''
 
-_NOTO_MAIN_JSON_PATH = Path(fontfinder._DATA_DIR_PATH, "latest", "noto.json").resolve()
+_NOTO_MAIN_JSON_USER_PATH = Path(fontfinder._USER_DATA_DIR_PATH, "cache", "noto.json").resolve()
 '''Path of updated, cached copy of noto.json.'''
 
 _NOTO_MAIN_JSON_MAX_AGE = datetime.timedelta(days=1)
 '''Max age of cached copy of noto.json, after which an updated copy will be downloaded.'''
 
 
 def get_noto_fonts(filter_func = None):
@@ -36,28 +36,28 @@
     font_infos.extend(_get_noto_cjk_fonts(filter_func))
     font_infos.extend(_get_noto_emoji_fonts(filter_func))
     font_infos.sort()
     return font_infos
 
 def _get_noto_main_data():
     '''Return main Noto JSON data as a Python object, handling cache as necessary.'''
-    if not _NOTO_MAIN_JSON_PATH.exists():
+    if not _NOTO_MAIN_JSON_USER_PATH.exists():
         # Copy noto.json distributed with this package
-        _NOTO_MAIN_JSON_PATH.parent.mkdir(parents=True, exist_ok=True)
-        shutil.copy2(_NOTO_MAIN_JSON_REF_PATH, _NOTO_MAIN_JSON_PATH)
+        _NOTO_MAIN_JSON_USER_PATH.parent.mkdir(parents=True, exist_ok=True)
+        shutil.copy2(_NOTO_MAIN_JSON_REF_PATH, _NOTO_MAIN_JSON_USER_PATH)
 
-    last_mod_time = datetime.datetime.fromtimestamp(_NOTO_MAIN_JSON_PATH.stat().st_mtime)
+    last_mod_time = datetime.datetime.fromtimestamp(_NOTO_MAIN_JSON_USER_PATH.stat().st_mtime)
     if (datetime.datetime.now() - last_mod_time) >= _NOTO_MAIN_JSON_MAX_AGE:
         # Update cached noto.json
         noto_json_text = requests.get(NOTO_MAIN_JSON_URL)
-        with open(_NOTO_MAIN_JSON_PATH, "w") as file:
+        with open(_NOTO_MAIN_JSON_USER_PATH, "w") as file:
             file.write(noto_json_text.text)
     
     # Read cached noto.json
-    with open(_NOTO_MAIN_JSON_PATH, "r") as file:
+    with open(_NOTO_MAIN_JSON_USER_PATH, "r") as file:
         noto_data = json.load(file)
     return noto_data
             
 def _get_noto_main_fonts(filter_func = None):
     '''Return a list of FontInfo records for the main (non-CJK) Google Noto fonts.'''
     font_infos = []
     noto_data = _get_noto_main_data()
```

### Comparing `fontfinder-0.11.0/src/fontfinder.egg-info/PKG-INFO` & `fontfinder-0.12.0/src/fontfinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: fontfinder
-Version: 0.11.0
+Version: 0.12.0
 Summary: Package for finding and installing fonts for Unicode scripts.
 Project-URL: Documentation, https://multiscript.app/fontfinder
 Project-URL: Source, https://github.com/multiscript/fontfinder
 Project-URL: Issue Tracker, https://github.com/multiscript/fontfinder/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: platformdirs>=4.2.1
 Requires-Dist: requests>=2.31
 Requires-Dist: semver>=3.0.2
 Requires-Dist: unicodedataplus>=15.1.0
 Requires-Dist: comtypes>=1.2.0; platform_system == "Windows"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: docs
```

### Comparing `fontfinder-0.11.0/src/fontfinder.egg-info/SOURCES.txt` & `fontfinder-0.12.0/src/fontfinder.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 src/fontfinder/_generate_data.py
 src/fontfinder/filters.py
 src/fontfinder/model.py
 src/fontfinder/noto.py
 src/fontfinder.egg-info/PKG-INFO
 src/fontfinder.egg-info/SOURCES.txt
 src/fontfinder.egg-info/dependency_links.txt
+src/fontfinder.egg-info/entry_points.txt
 src/fontfinder.egg-info/requires.txt
 src/fontfinder.egg-info/top_level.txt
+src/fontfinder/__pyinstaller/__init__.py
+src/fontfinder/__pyinstaller/hook-fontfinder.py
 src/fontfinder/_platforms/__init__.py
 src/fontfinder/_platforms/mac.py
 src/fontfinder/_platforms/windows.py
 src/fontfinder/data/noto.json
 src/fontfinder/data/small_unihan.json
 test/test_fontfinder.py
```

### Comparing `fontfinder-0.11.0/test/test_fontfinder.py` & `fontfinder-0.12.0/test/test_fontfinder.py`

 * *Files identical despite different names*


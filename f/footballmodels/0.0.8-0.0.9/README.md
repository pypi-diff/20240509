# Comparing `tmp/footballmodels-0.0.8.tar.gz` & `tmp/footballmodels-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "footballmodels-0.0.8.tar", last modified: Tue Oct 31 22:49:18 2023, max compression
+gzip compressed data, was "footballmodels-0.0.9.tar", last modified: Tue Oct 31 23:23:29 2023, max compression
```

## Comparing `footballmodels-0.0.8.tar` & `footballmodels-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.809859 footballmodels-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.793859 footballmodels-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.801859 footballmodels-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-10-31 22:49:08.000000 footballmodels-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-10-31 22:49:08.000000 footballmodels-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-10-31 22:49:08.000000 footballmodels-0.0.8/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.801859 footballmodels-0.0.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2023-10-31 22:49:08.000000 footballmodels-0.0.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-31 22:49:08.000000 footballmodels-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-10-31 22:49:18.809859 footballmodels-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-10-31 22:49:08.000000 footballmodels-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-10-31 22:49:08.000000 footballmodels-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-31 22:49:08.000000 footballmodels-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-10-31 22:49:18.809859 footballmodels-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-31 22:49:08.000000 footballmodels-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.793859 footballmodels-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.801859 footballmodels-0.0.8/src/footballmodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:08.000000 footballmodels-0.0.8/src/footballmodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.805858 footballmodels-0.0.8/src/footballmodels/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:08.000000 footballmodels-0.0.8/src/footballmodels/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15128 2023-10-31 22:49:08.000000 footballmodels-0.0.8/src/footballmodels/definitions/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.805858 footballmodels-0.0.8/src/footballmodels/player_similarity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:08.000000 footballmodels-0.0.8/src/footballmodels/player_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2023-10-31 22:49:08.000000 footballmodels-0.0.8/src/footballmodels/player_similarity/column_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2023-10-31 22:49:08.000000 footballmodels-0.0.8/src/footballmodels/player_similarity/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.805858 footballmodels-0.0.8/src/footballmodels/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:08.000000 footballmodels-0.0.8/src/footballmodels/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2023-10-31 22:49:08.000000 footballmodels-0.0.8/src/footballmodels/utils/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2023-10-31 22:49:08.000000 footballmodels-0.0.8/src/footballmodels/utils/possession_adjustment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:49:18.805858 footballmodels-0.0.8/src/footballmodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-10-31 22:49:18.000000 footballmodels-0.0.8/src/footballmodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-10-31 22:49:18.000000 footballmodels-0.0.8/src/footballmodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 22:49:18.000000 footballmodels-0.0.8/src/footballmodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-31 22:49:18.000000 footballmodels-0.0.8/src/footballmodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-31 22:49:18.000000 footballmodels-0.0.8/src/footballmodels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.831684 footballmodels-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.823684 footballmodels-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.827684 footballmodels-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2023-10-31 23:23:21.000000 footballmodels-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-10-31 23:23:21.000000 footballmodels-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-10-31 23:23:21.000000 footballmodels-0.0.9/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.827684 footballmodels-0.0.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2023-10-31 23:23:21.000000 footballmodels-0.0.9/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-31 23:23:21.000000 footballmodels-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2023-10-31 23:23:29.831684 footballmodels-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-10-31 23:23:21.000000 footballmodels-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2023-10-31 23:23:21.000000 footballmodels-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-31 23:23:21.000000 footballmodels-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2023-10-31 23:23:29.831684 footballmodels-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2023-10-31 23:23:21.000000 footballmodels-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.823684 footballmodels-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.831684 footballmodels-0.0.9/src/footballmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:21.000000 footballmodels-0.0.9/src/footballmodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.831684 footballmodels-0.0.9/src/footballmodels/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:21.000000 footballmodels-0.0.9/src/footballmodels/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15148 2023-10-31 23:23:21.000000 footballmodels-0.0.9/src/footballmodels/definitions/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.831684 footballmodels-0.0.9/src/footballmodels/player_similarity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:21.000000 footballmodels-0.0.9/src/footballmodels/player_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2023-10-31 23:23:21.000000 footballmodels-0.0.9/src/footballmodels/player_similarity/column_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2023-10-31 23:23:21.000000 footballmodels-0.0.9/src/footballmodels/player_similarity/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.831684 footballmodels-0.0.9/src/footballmodels/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:21.000000 footballmodels-0.0.9/src/footballmodels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2023-10-31 23:23:21.000000 footballmodels-0.0.9/src/footballmodels/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2023-10-31 23:23:21.000000 footballmodels-0.0.9/src/footballmodels/utils/possession_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 23:23:29.831684 footballmodels-0.0.9/src/footballmodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2023-10-31 23:23:29.000000 footballmodels-0.0.9/src/footballmodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2023-10-31 23:23:29.000000 footballmodels-0.0.9/src/footballmodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 23:23:29.000000 footballmodels-0.0.9/src/footballmodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-31 23:23:29.000000 footballmodels-0.0.9/src/footballmodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-31 23:23:29.000000 footballmodels-0.0.9/src/footballmodels.egg-info/top_level.txt
```

### Comparing `footballmodels-0.0.8/.gitignore` & `footballmodels-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.8/.vscode/settings.json` & `footballmodels-0.0.9/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.8/LICENSE` & `footballmodels-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.8/PKG-INFO` & `footballmodels-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: footballmodels
-Version: 0.0.8
+Version: 0.0.9
 Summary: Football Models library
 Home-page: https://github.com/dmoggles/footballmodels
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `footballmodels-0.0.8/setup.cfg` & `footballmodels-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.8/setup.py` & `footballmodels-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.8/src/footballmodels/definitions/templates.py` & `footballmodels-0.0.9/src/footballmodels/definitions/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,14 +422,15 @@
             "passes_completed_short",
             "passes_completed_medium",
             "passes_short",
             "passes_medium",
             "miscontrols",
             "dispossessed",
         ],
+        sig_figs=2,
     ),
 ]
 
 TeamTemplate = [
     TemplateAttribute(
         "Open Play NPxG/Shot",
         lambda df: df["live_xg_team"] / df["shots_total_team"],
```

### Comparing `footballmodels-0.0.8/src/footballmodels/player_similarity/column_defs.py` & `footballmodels-0.0.9/src/footballmodels/player_similarity/column_defs.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.8/src/footballmodels/player_similarity/models.py` & `footballmodels-0.0.9/src/footballmodels/player_similarity/models.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.8/src/footballmodels/utils/distance.py` & `footballmodels-0.0.9/src/footballmodels/utils/distance.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.8/src/footballmodels/utils/possession_adjustment.py` & `footballmodels-0.0.9/src/footballmodels/utils/possession_adjustment.py`

 * *Files identical despite different names*

### Comparing `footballmodels-0.0.8/src/footballmodels.egg-info/PKG-INFO` & `footballmodels-0.0.9/src/footballmodels.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: footballmodels
-Version: 0.0.8
+Version: 0.0.9
 Summary: Football Models library
 Home-page: https://github.com/dmoggles/footballmodels
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `footballmodels-0.0.8/src/footballmodels.egg-info/SOURCES.txt` & `footballmodels-0.0.9/src/footballmodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*


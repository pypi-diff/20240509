# Comparing `tmp/projgen-0.0.3.tar.gz` & `tmp/projgen-0.0.4.tar.gz`

## Comparing `projgen-0.0.3.tar` & `projgen-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 projgen-0.0.3/projgen.json
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 projgen-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 projgen-0.0.3/src/projgen/__init__.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 projgen-0.0.3/src/projgen/__main__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 projgen-0.0.3/.gitignore
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 projgen-0.0.3/README.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 projgen-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 projgen-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 projgen-0.0.4/projgen.json
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 projgen-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 projgen-0.0.4/src/projgen/__init__.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 projgen-0.0.4/src/projgen/__main__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 projgen-0.0.4/.gitignore
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 projgen-0.0.4/README.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 projgen-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 projgen-0.0.4/PKG-INFO
```

### Comparing `projgen-0.0.3/src/projgen/__main__.py` & `projgen-0.0.4/src/projgen/__main__.py`

 * *Files identical despite different names*

### Comparing `projgen-0.0.3/pyproject.toml` & `projgen-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "projgen"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ceayo", email="ceayo@duck.com" },
 ]
 dependencies = [
     "rich",
     "typer",
 ]
```

### Comparing `projgen-0.0.3/PKG-INFO` & `projgen-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: projgen
-Version: 0.0.3
+Version: 0.0.4
 Summary: Project Manager
 Author-email: Ceayo <ceayo@duck.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: rich
@@ -15,19 +15,26 @@
 As I want to make cool projects, but never finish them, I've made
 this program. Every 30 days a new project will be generated, and you
 get 30 days to build that.
 
 ## Getting Started
 ```bash
 pip install projgen
-python3 -m projgen new-db
-python3 -m projgen show-database
-python3 -m projgen status
+projgen new-db
+projgen show-database
+projgen status
 ```
 
 ## Adding things to the database
 ```bash
-python3 -m projgen add-db-item "type" "Cli Tool"
-python3 -m projgen add-db-requirement "type" "Cli Tool" "cliToolAction"
-python3 -m projgen add-db-item "cliToolAction" "Git Info Viewer"
-python3 -m projgen add-db-item "cliToolAction" "Project Manager Forcing You To Make Cool Stuff"
+projgen add-db-item "type" "Cli Tool"
+projgen add-db-requirement "type" "Cli Tool" "cliToolAction"
+projgen add-db-item "cliToolAction" "Git Info Viewer"
+projgen add-db-item "cliToolAction" "Project Manager Forcing You To Make Cool Stuff"
+```
+
+## Getting a project
+During the thirty days, you can't get a new project. Once these 30 days are over, 
+you can get a new project by running
+```bash
+projgen update
 ```
```


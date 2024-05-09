# Comparing `tmp/prometa-2024.1.tar.gz` & `tmp/prometa-2024.2.tar.gz`

## Comparing `prometa-2024.1.tar` & `prometa-2024.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 prometa-2024.1/CITATION.cff
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.1/TODO.md
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 prometa-2024.1/codemeta.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.1/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.1/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.1/doc/requirements.txt
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.1/doc/source/conf.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 prometa-2024.1/doc/source/index.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 prometa-2024.1/doc/source/modules.rst
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 prometa-2024.1/doc/source/prometa.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.1/doc/source/readme.md
--rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.1/scripts/publish_documentation.sh
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/__init__.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/citation.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/codemeta.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/common.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/config.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/file.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/insert.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/main.py
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/project.py
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/readme.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/version.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/gitlab/ci.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/gitlab/repo.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/id/hal.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/id/orcid.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/id/swh.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/python/common.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 prometa-2024.1/src/prometa/python/venv.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 prometa-2024.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.1/LICENSE.txt
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 prometa-2024.1/README.md
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 prometa-2024.1/pyproject.toml
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 prometa-2024.1/PKG-INFO
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 prometa-2024.2/CITATION.cff
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.2/TODO.md
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 prometa-2024.2/codemeta.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.2/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.2/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.2/doc/requirements.txt
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/conf.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/index.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/modules.rst
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/prometa.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/readme.md
+-rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.2/scripts/publish_documentation.sh
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/__init__.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/citation.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/codemeta.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/common.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/config.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/file.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/insert.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/main.py
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/project.py
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/readme.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/version.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/gitlab/ci.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/gitlab/repo.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/id/hal.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/id/orcid.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/id/swh.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/python/common.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/python/venv.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 prometa-2024.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.2/LICENSE.txt
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 prometa-2024.2/README.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 prometa-2024.2/pyproject.toml
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 prometa-2024.2/PKG-INFO
```

### Comparing `prometa-2024.1/.gitlab-ci.yml` & `prometa-2024.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/codemeta.json` & `prometa-2024.2/codemeta.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.971875%*

 * *Differences: {"'softwareRequirements'": "{insert: [(7, OrderedDict([('@type', 'SoftwareApplication'), "*

 * *                           "('identifier', 'trove-classifiers'), ('name', 'trove-classifiers'), "*

 * *                           "('runtimePlatform', 'Python 3')]))]}",*

 * * "'version'": "'2024.2'"}*

```diff
@@ -81,19 +81,25 @@
             "runtimePlatform": "Python 3"
         },
         {
             "@type": "SoftwareApplication",
             "identifier": "tomli-w",
             "name": "tomli-w",
             "runtimePlatform": "Python 3"
+        },
+        {
+            "@type": "SoftwareApplication",
+            "identifier": "trove-classifiers",
+            "name": "trove-classifiers",
+            "runtimePlatform": "Python 3"
         }
     ],
     "targetProduct": {
         "@type": "CommandLineApplication",
         "description": "Update project metadata.",
         "executableName": "prometa",
         "name": "prometa",
         "runtimePlatform": "Python 3"
     },
     "url": "https://gitlab.inria.fr/jrye/prometa",
-    "version": "2024.1"
+    "version": "2024.2"
 }
```

### Comparing `prometa-2024.1/doc/Makefile` & `prometa-2024.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/doc/make.bat` & `prometa-2024.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/doc/source/conf.py` & `prometa-2024.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/doc/source/prometa.rst` & `prometa-2024.2/doc/source/prometa.rst`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/scripts/publish_documentation.sh` & `prometa-2024.2/scripts/publish_documentation.sh`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/citation.py` & `prometa-2024.2/src/prometa/citation.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/codemeta.py` & `prometa-2024.2/src/prometa/codemeta.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/config.py` & `prometa-2024.2/src/prometa/config.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/file.py` & `prometa-2024.2/src/prometa/file.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/insert.py` & `prometa-2024.2/src/prometa/insert.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/main.py` & `prometa-2024.2/src/prometa/main.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/project.py` & `prometa-2024.2/src/prometa/project.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/readme.py` & `prometa-2024.2/src/prometa/readme.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/gitlab/ci.py` & `prometa-2024.2/src/prometa/gitlab/ci.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/gitlab/repo.py` & `prometa-2024.2/src/prometa/gitlab/repo.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/id/hal.py` & `prometa-2024.2/src/prometa/id/hal.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/id/swh.py` & `prometa-2024.2/src/prometa/id/swh.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/src/prometa/python/venv.py` & `prometa-2024.2/src/prometa/python/venv.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/LICENSE.txt` & `prometa-2024.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/README.md` & `prometa-2024.2/README.md`

 * *Files identical despite different names*

### Comparing `prometa-2024.1/pyproject.toml` & `prometa-2024.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "CodeMetaPy",
     "PyYAML",
     "python-gitlab",
     "requests",
     "spdx-license-list",
     "spdx-matcher",
     "tomli-w",
+    "trove-classifiers",
 ]
 requires-python = ">=3.6"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `prometa-2024.1/PKG-INFO` & `prometa-2024.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Prometa
-Version: 2024.1
+Version: 2024.2
 Summary: Manage project metadata.
 Project-URL: Homepage, https://gitlab.inria.fr/jrye/prometa
 Project-URL: Source, https://gitlab.inria.fr/jrye/prometa.git
 Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/prometa
 Project-URL: Issues, https://gitlab.inria.fr/jrye/prometa/-/issues
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
 License: MIT License
@@ -24,14 +24,15 @@
 Requires-Dist: codemetapy
 Requires-Dist: python-gitlab
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: spdx-license-list
 Requires-Dist: spdx-matcher
 Requires-Dist: tomli-w
+Requires-Dist: trove-classifiers
 Description-Content-Type: text/markdown
 
 ---
 title: README
 author: Jan-Michael Rye
 ---
```


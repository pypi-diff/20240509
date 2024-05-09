# Comparing `tmp/prometa-2024.2.tar.gz` & `tmp/prometa-2024.3.tar.gz`

## Comparing `prometa-2024.2.tar` & `prometa-2024.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 prometa-2024.2/CITATION.cff
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.2/TODO.md
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 prometa-2024.2/codemeta.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.2/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.2/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.2/doc/requirements.txt
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/conf.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/index.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/modules.rst
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/prometa.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.2/doc/source/readme.md
--rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.2/scripts/publish_documentation.sh
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/__init__.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/citation.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/codemeta.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/common.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/config.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/file.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/insert.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/main.py
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/project.py
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/readme.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/version.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/gitlab/ci.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/gitlab/repo.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/id/hal.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/id/orcid.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/id/swh.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/python/common.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 prometa-2024.2/src/prometa/python/venv.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 prometa-2024.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.2/LICENSE.txt
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 prometa-2024.2/README.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 prometa-2024.2/pyproject.toml
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 prometa-2024.2/PKG-INFO
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 prometa-2024.3/CITATION.cff
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.3/TODO.md
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 prometa-2024.3/codemeta.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.3/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.3/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.3/doc/requirements.txt
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.3/doc/source/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.3/doc/source/readme.md
+-rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.3/scripts/publish_documentation.sh
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/__init__.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/citation.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/codemeta.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/common.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/config.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/file.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/insert.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/main.py
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/project.py
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/readme.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/version.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/gitlab/__init__.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/gitlab/ci.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/gitlab/repo.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/id/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/id/hal.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/id/orcid.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/id/swh.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/python/__init__.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/python/common.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 prometa-2024.3/src/prometa/python/venv.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 prometa-2024.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.3/LICENSE.txt
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 prometa-2024.3/README.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 prometa-2024.3/pyproject.toml
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 prometa-2024.3/PKG-INFO
```

### Comparing `prometa-2024.2/.gitlab-ci.yml` & `prometa-2024.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/codemeta.json` & `prometa-2024.3/codemeta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'2024.3'"}*

```diff
@@ -97,9 +97,9 @@
         "@type": "CommandLineApplication",
         "description": "Update project metadata.",
         "executableName": "prometa",
         "name": "prometa",
         "runtimePlatform": "Python 3"
     },
     "url": "https://gitlab.inria.fr/jrye/prometa",
-    "version": "2024.2"
+    "version": "2024.3"
 }
```

### Comparing `prometa-2024.2/doc/Makefile` & `prometa-2024.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/doc/make.bat` & `prometa-2024.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/doc/source/conf.py` & `prometa-2024.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/scripts/publish_documentation.sh` & `prometa-2024.3/scripts/publish_documentation.sh`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/citation.py` & `prometa-2024.3/src/prometa/citation.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/codemeta.py` & `prometa-2024.3/src/prometa/codemeta.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/config.py` & `prometa-2024.3/src/prometa/config.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/file.py` & `prometa-2024.3/src/prometa/file.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/insert.py` & `prometa-2024.3/src/prometa/insert.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/main.py` & `prometa-2024.3/src/prometa/main.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/project.py` & `prometa-2024.3/src/prometa/project.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/readme.py` & `prometa-2024.3/src/prometa/readme.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/gitlab/ci.py` & `prometa-2024.3/src/prometa/gitlab/ci.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/gitlab/repo.py` & `prometa-2024.3/src/prometa/gitlab/repo.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/id/hal.py` & `prometa-2024.3/src/prometa/id/hal.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/id/swh.py` & `prometa-2024.3/src/prometa/id/swh.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/python/common.py` & `prometa-2024.3/src/prometa/python/common.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/src/prometa/python/venv.py` & `prometa-2024.3/src/prometa/python/venv.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/LICENSE.txt` & `prometa-2024.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/README.md` & `prometa-2024.3/README.md`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/pyproject.toml` & `prometa-2024.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prometa-2024.2/PKG-INFO` & `prometa-2024.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Prometa
-Version: 2024.2
+Version: 2024.3
 Summary: Manage project metadata.
 Project-URL: Homepage, https://gitlab.inria.fr/jrye/prometa
 Project-URL: Source, https://gitlab.inria.fr/jrye/prometa.git
 Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/prometa
 Project-URL: Issues, https://gitlab.inria.fr/jrye/prometa/-/issues
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
 License: MIT License
```


# Comparing `tmp/prometa-2024.4.tar.gz` & `tmp/prometa-2024.5.tar.gz`

## Comparing `prometa-2024.4.tar` & `prometa-2024.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.4/.gitlab-ci.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 prometa-2024.4/CITATION.cff
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.4/TODO.md
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 prometa-2024.4/codemeta.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.4/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.4/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.4/doc/requirements.txt
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.4/doc/source/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.4/doc/source/readme.md
--rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.4/scripts/publish_documentation.sh
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/__init__.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/citation.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/codemeta.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/common.py
--rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/config.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/file.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/insert.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/main.py
--rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/project.py
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/readme.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/version.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/gitlab/__init__.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/gitlab/ci.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/gitlab/repo.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/id/__init__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/id/hal.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/id/orcid.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/id/swh.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/python/__init__.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/python/common.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 prometa-2024.4/src/prometa/python/venv.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 prometa-2024.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.4/LICENSE.txt
--rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 prometa-2024.4/README.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 prometa-2024.4/pyproject.toml
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 prometa-2024.4/PKG-INFO
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.5/.gitlab-ci.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 prometa-2024.5/CITATION.cff
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.5/TODO.md
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 prometa-2024.5/codemeta.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.5/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.5/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.5/doc/requirements.txt
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.5/doc/source/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.5/doc/source/readme.md
+-rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.5/scripts/publish_documentation.sh
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/__init__.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/citation.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/codemeta.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/common.py
+-rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/config.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/file.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/insert.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/main.py
+-rw-r--r--   0        0        0     4268 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/project.py
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/readme.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/version.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/gitlab/__init__.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/gitlab/ci.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/gitlab/repo.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/id/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/id/hal.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/id/orcid.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/id/swh.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/python/__init__.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/python/common.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 prometa-2024.5/src/prometa/python/venv.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 prometa-2024.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.5/LICENSE.txt
+-rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 prometa-2024.5/README.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 prometa-2024.5/pyproject.toml
+-rw-r--r--   0        0        0    10216 2020-02-02 00:00:00.000000 prometa-2024.5/PKG-INFO
```

### Comparing `prometa-2024.4/.gitlab-ci.yml` & `prometa-2024.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/CITATION.cff` & `prometa-2024.5/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 - description: The Software Heritage URL.
   type: url
   value: https://archive.softwareheritage.org/browse/origin/?origin_url=https%3A//gitlab.inria.fr/jrye/prometa.git
 license: MIT
 message: If you use this software, please cite it using these metadata.
 repository-code: https://gitlab.inria.fr/jrye/prometa.git
 title: Prometa
-version: '2024.4'
+version: '2024.5'
```

### Comparing `prometa-2024.4/codemeta.json` & `prometa-2024.5/codemeta.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'2024.5'"}*

```diff
@@ -97,9 +97,9 @@
         "@type": "CommandLineApplication",
         "description": "Update project metadata.",
         "executableName": "prometa",
         "name": "prometa",
         "runtimePlatform": "Python 3"
     },
     "url": "https://gitlab.inria.fr/jrye/prometa",
-    "version": "2024.4"
+    "version": "2024.5"
 }
```

### Comparing `prometa-2024.4/doc/Makefile` & `prometa-2024.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/doc/make.bat` & `prometa-2024.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/doc/source/conf.py` & `prometa-2024.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/scripts/publish_documentation.sh` & `prometa-2024.5/scripts/publish_documentation.sh`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/citation.py` & `prometa-2024.5/src/prometa/citation.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/codemeta.py` & `prometa-2024.5/src/prometa/codemeta.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/config.py` & `prometa-2024.5/src/prometa/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,17 @@
   # python-gitlab configuration file:
   config: path/to/python-gitlab.cfg
 
   # The section of the python-gitlab configuration file to use when retrieving
   # GitLab project data.
   section: somewhere
 
+  # If true, use python-gitlab to update project hooks.
+  update_hooks: false
+
   # Map GitLab hosts to their corresponding GitLab Pages URL formats. This map
   # will be used to generate documentation links when a "pages" job is detected
   # in the CI configuration file. The namespace and name parameters correspond
   # to those of the GitLab project.
   pages_urls:
     gitlab.com: "https://{namespace}.gitlab.io/{name}"
```

### Comparing `prometa-2024.4/src/prometa/file.py` & `prometa-2024.5/src/prometa/file.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/insert.py` & `prometa-2024.5/src/prometa/insert.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/main.py` & `prometa-2024.5/src/prometa/main.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/project.py` & `prometa-2024.5/src/prometa/project.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/readme.py` & `prometa-2024.5/src/prometa/readme.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/gitlab/ci.py` & `prometa-2024.5/src/prometa/gitlab/ci.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,16 @@
                 LOGGER.info('Updating SWH hook for %s.', gproj.name)
                 swh_hook.save()
 
     def manage_hooks(self):
         '''
         Add or remove hooks depending on the current repository configuration.
         '''
+        if not self.project.config.get('gitlab', 'manage_hooks', default=False):
+            return
         with self.project.config.gitlab as glab:
             glab.auth()
             gproj = self.project.git_repo.get_gitlab_project(glab)
             self._manage_swh_hook(gproj)
 
     def add_stages(self):
         '''
```

### Comparing `prometa-2024.4/src/prometa/gitlab/repo.py` & `prometa-2024.5/src/prometa/gitlab/repo.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/id/hal.py` & `prometa-2024.5/src/prometa/id/hal.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/id/swh.py` & `prometa-2024.5/src/prometa/id/swh.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/python/common.py` & `prometa-2024.5/src/prometa/python/common.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/src/prometa/python/venv.py` & `prometa-2024.5/src/prometa/python/venv.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/LICENSE.txt` & `prometa-2024.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/README.md` & `prometa-2024.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,17 @@
   # python-gitlab configuration file:
   config: path/to/python-gitlab.cfg
 
   # The section of the python-gitlab configuration file to use when retrieving
   # GitLab project data.
   section: somewhere
 
+  # If true, use python-gitlab to update project hooks.
+  update_hooks: false
+
   # Map GitLab hosts to their corresponding GitLab Pages URL formats. This map
   # will be used to generate documentation links when a "pages" job is detected
   # in the CI configuration file. The namespace and name parameters correspond
   # to those of the GitLab project.
   pages_urls:
     gitlab.com: "https://{namespace}.gitlab.io/{name}"
```

### Comparing `prometa-2024.4/pyproject.toml` & `prometa-2024.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prometa-2024.4/PKG-INFO` & `prometa-2024.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Prometa
-Version: 2024.4
+Version: 2024.5
 Summary: Manage project metadata.
 Project-URL: Homepage, https://gitlab.inria.fr/jrye/prometa
 Project-URL: Source, https://gitlab.inria.fr/jrye/prometa.git
 Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/prometa
 Project-URL: Issues, https://gitlab.inria.fr/jrye/prometa/-/issues
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
 License: MIT License
@@ -115,14 +115,17 @@
   # python-gitlab configuration file:
   config: path/to/python-gitlab.cfg
 
   # The section of the python-gitlab configuration file to use when retrieving
   # GitLab project data.
   section: somewhere
 
+  # If true, use python-gitlab to update project hooks.
+  update_hooks: false
+
   # Map GitLab hosts to their corresponding GitLab Pages URL formats. This map
   # will be used to generate documentation links when a "pages" job is detected
   # in the CI configuration file. The namespace and name parameters correspond
   # to those of the GitLab project.
   pages_urls:
     gitlab.com: "https://{namespace}.gitlab.io/{name}"
```


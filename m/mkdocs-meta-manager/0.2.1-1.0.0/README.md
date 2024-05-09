# Comparing `tmp/mkdocs-meta-manager-0.2.1.tar.gz` & `tmp/mkdocs_meta_manager-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-meta-manager-0.2.1.tar", last modified: Fri Mar 24 13:26:42 2023, max compression
+gzip compressed data, was "mkdocs_meta_manager-1.0.0.tar", last modified: Thu May  9 20:03:13 2024, max compression
```

## Comparing `mkdocs-meta-manager-0.2.1.tar` & `mkdocs_meta_manager-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:26:42.312115 mkdocs-meta-manager-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-24 13:26:42.312115 mkdocs-meta-manager-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-24 13:26:32.000000 mkdocs-meta-manager-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:26:42.312115 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-24 13:26:42.000000 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-24 13:26:42.000000 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 13:26:42.000000 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-24 13:26:42.000000 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-24 13:26:42.000000 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-24 13:26:42.000000 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:26:42.312115 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 13:26:32.000000 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-24 13:26:32.000000 mkdocs-meta-manager-0.2.1/mkdocs_meta_manager_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 13:26:42.312115 mkdocs-meta-manager-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-24 13:26:32.000000 mkdocs-meta-manager-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:03:13.697485 mkdocs_meta_manager-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-09 20:03:13.697485 mkdocs_meta_manager-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-09 20:03:10.000000 mkdocs_meta_manager-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:03:13.697485 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-09 20:03:13.000000 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 20:03:13.000000 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 20:03:13.000000 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 20:03:13.000000 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 20:03:13.000000 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 20:03:13.000000 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:03:13.697485 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 20:03:10.000000 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-09 20:03:10.000000 mkdocs_meta_manager-1.0.0/mkdocs_meta_manager_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 20:03:13.697485 mkdocs_meta_manager-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-09 20:03:10.000000 mkdocs_meta_manager-1.0.0/setup.py
```

### Comparing `mkdocs-meta-manager-0.2.1/PKG-INFO` & `mkdocs_meta_manager-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-meta-manager
-Version: 0.2.1
+Version: 1.0.0
 Summary: MkDocs plugin for managing meta tags across folders and files.
 Home-page: https://github.com/timmeinerzhagen/mkdocs-meta-manager
 Author: Tim Jonas Meinerzhagen
 Author-email: tim@meinerzhagen.me
 License: MIT
 Keywords: mkdocs meta manager
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+Requires-Dist: mkdocs>=1.0
+Requires-Dist: jinja2
 
 # mkdocs-meta-manager
 
 MkDocs plugin for managing meta tags across folders and files
 
 ## Setup
 
@@ -45,9 +47,9 @@
 All markdown files in the same folder and in subfolders automatically get all tags that are defined in the given meta file.
 
 ## Options
 
 `meta_filename`
 Change the default name of the meta file. (default=`.meta.yml`)
 
-`merge_tags`
-Merge the tags of all relevant meta files and pages for a page (default=`false`)
+`merge_entries`
+Merge all specified entries of meta files and pages for a page that affects them according to the hirearchie (default=`[]`)
```

### Comparing `mkdocs-meta-manager-0.2.1/README.md` & `mkdocs_meta_manager-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 All markdown files in the same folder and in subfolders automatically get all tags that are defined in the given meta file.
 
 ## Options
 
 `meta_filename`
 Change the default name of the meta file. (default=`.meta.yml`)
 
-`merge_tags`
-Merge the tags of all relevant meta files and pages for a page (default=`false`)
+`merge_entries`
+Merge all specified entries of meta files and pages for a page that affects them according to the hirearchie (default=`[]`)
```

### Comparing `mkdocs-meta-manager-0.2.1/mkdocs_meta_manager.egg-info/PKG-INFO` & `mkdocs_meta_manager-1.0.0/mkdocs_meta_manager.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-meta-manager
-Version: 0.2.1
+Version: 1.0.0
 Summary: MkDocs plugin for managing meta tags across folders and files.
 Home-page: https://github.com/timmeinerzhagen/mkdocs-meta-manager
 Author: Tim Jonas Meinerzhagen
 Author-email: tim@meinerzhagen.me
 License: MIT
 Keywords: mkdocs meta manager
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+Requires-Dist: mkdocs>=1.0
+Requires-Dist: jinja2
 
 # mkdocs-meta-manager
 
 MkDocs plugin for managing meta tags across folders and files
 
 ## Setup
 
@@ -45,9 +47,9 @@
 All markdown files in the same folder and in subfolders automatically get all tags that are defined in the given meta file.
 
 ## Options
 
 `meta_filename`
 Change the default name of the meta file. (default=`.meta.yml`)
 
-`merge_tags`
-Merge the tags of all relevant meta files and pages for a page (default=`false`)
+`merge_entries`
+Merge all specified entries of meta files and pages for a page that affects them according to the hirearchie (default=`[]`)
```

### Comparing `mkdocs-meta-manager-0.2.1/mkdocs_meta_manager_plugin/plugin.py` & `mkdocs_meta_manager-1.0.0/mkdocs_meta_manager_plugin/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
 
 class MetaManagerPlugin(BasePlugin):
     config_scheme = (
         ('meta_filename', config_options.Type(str, default='.meta.yml')),
-        ('merge_tags', config_options.Type(bool, default=False)),
+        ('merge_entries', config_options.Type(list, default=[])),
     )
 
     meta_files = {}
 
     def __init__(self):
         self.enabled = True
 
@@ -27,26 +27,26 @@
                 .replace(config.docs_dir, '')
             with open(filepath, "r") as stream:
                 try:
                     self.meta_files[raw_path] = yaml.safe_load(stream)
                 except yaml.YAMLError as exc:
                     print(exc)
         logging.debug(self.meta_files)
-        
 
     def on_page_markdown(self, markdown, page, config, files):
         if not self.enabled:
             return markdown
 
         path_parts = page.file.src_path.split('/')
         for i in reversed(range(len(path_parts))):
             part = '/'.join(path_parts[0:i])
             if part in self.meta_files:
                 for key, value in self.meta_files[part].items():
                     if not key in page.meta:
                         page.meta[key] = value
-                    elif key == 'tags' and self.config['merge_tags']:
-                        page.meta[key] = page.meta[key].copy()
+                    elif key in self.config['merge_entries']:
+                        if not isinstance(page.meta[key], list):
+                            page.meta[key] = [page.meta[key]]
                         page.meta[key].extend(value)
 
         logging.debug("%s: %s", page.file.src_path, page.meta)
         return markdown
```

### Comparing `mkdocs-meta-manager-0.2.1/setup.py` & `mkdocs_meta_manager-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='mkdocs-meta-manager',
-    version='0.2.1',
+    version='1.0.0',
     description='MkDocs plugin for managing meta tags across folders and files.',    
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords='mkdocs meta manager',
     url='https://github.com/timmeinerzhagen/mkdocs-meta-manager',
     author='Tim Jonas Meinerzhagen',
     author_email='tim@meinerzhagen.me',
```


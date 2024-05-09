# Comparing `tmp/sphinx_tagtoctree-0.9.4.tar.gz` & `tmp/sphinx_tagtoctree-0.9.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_tagtoctree-0.9.4.tar", last modified: Mon Oct 17 12:26:18 2022, max compression
+gzip compressed data, was "sphinx_tagtoctree-0.9.5.0a1.tar", last modified: Thu May  9 12:08:45 2024, max compression
```

## Comparing `sphinx_tagtoctree-0.9.4.tar` & `sphinx_tagtoctree-0.9.5.0a1.tar`

### file list

```diff
@@ -1,29 +1,53 @@
--rw-r--r--   0        0        0      734 2022-10-17 07:50:29.899664 sphinx_tagtoctree-0.9.4/.github/workflows/pythonpublish.yml
--rw-r--r--   0        0        0     2012 2022-10-17 07:50:29.899835 sphinx_tagtoctree-0.9.4/.gitignore
--rw-r--r--   0        0        0      511 2022-10-17 07:50:29.900070 sphinx_tagtoctree-0.9.4/.vscode/launch.json
--rw-r--r--   0        0        0      174 2022-10-17 07:50:29.900240 sphinx_tagtoctree-0.9.4/.vscode/settings.json
--rw-r--r--   0        0        0      577 2022-10-17 07:50:29.900762 sphinx_tagtoctree-0.9.4/CONTRIBUTING.md
--rw-r--r--   0        0        0    35141 2022-10-17 07:50:29.901240 sphinx_tagtoctree-0.9.4/LICENSE
--rw-r--r--   0        0        0       36 2022-10-17 07:50:29.901450 sphinx_tagtoctree-0.9.4/MANIFEST.in
--rw-r--r--   0        0        0     1716 2022-10-17 07:50:29.901640 sphinx_tagtoctree-0.9.4/README.md
--rw-r--r--   0        0        0    11074 2022-10-17 07:50:29.901937 sphinx_tagtoctree-0.9.4/docs/2019-11-26-16-53-11.png).png
--rw-r--r--   0        0        0    10136 2022-10-17 07:50:29.902148 sphinx_tagtoctree-0.9.4/docs/2019-11-26-16-56-16.png).png
--rw-r--r--   0        0        0    10136 2022-10-17 07:50:29.902334 sphinx_tagtoctree-0.9.4/docs/2019-11-26-17-21-26.png
--rw-r--r--   0        0        0    18570 2022-10-17 07:50:29.902597 sphinx_tagtoctree-0.9.4/docs/2019-11-26-17-21-57.png
--rw-r--r--   0        0        0    11074 2022-10-17 07:50:29.902815 sphinx_tagtoctree-0.9.4/docs/2019-11-26-17-22-22.png
--rw-r--r--   0        0        0    11193 2022-10-17 07:50:29.903014 sphinx_tagtoctree-0.9.4/docs/2019-11-26-17-22-54.png
--rw-r--r--   0        0        0      638 2022-10-17 07:50:29.903329 sphinx_tagtoctree-0.9.4/example/Makefile
--rw-r--r--   0        0        0     1666 2022-10-17 07:55:55.714900 sphinx_tagtoctree-0.9.4/example/README.md
--rw-r--r--   0        0        0      770 2022-10-17 07:50:29.903587 sphinx_tagtoctree-0.9.4/example/make.bat
--rw-r--r--   0        0        0     1916 2022-10-17 07:50:29.903819 sphinx_tagtoctree-0.9.4/example/source/conf.py
--rw-r--r--   0        0        0      609 2022-10-17 07:50:29.904018 sphinx_tagtoctree-0.9.4/example/source/index.rst
--rw-r--r--   0        0        0       96 2022-10-17 07:50:29.904145 sphinx_tagtoctree-0.9.4/example/source/page1.rst
--rw-r--r--   0        0        0       89 2022-10-17 07:50:29.904275 sphinx_tagtoctree-0.9.4/example/source/page2.rst
--rw-r--r--   0        0        0       97 2022-10-17 07:50:29.904403 sphinx_tagtoctree-0.9.4/example/source/page3.rst
--rw-r--r--   0        0        0       87 2022-10-17 07:50:29.904533 sphinx_tagtoctree-0.9.4/example/source/page4.rst
--rw-r--r--   0        0        0       89 2022-10-17 07:50:29.904751 sphinx_tagtoctree-0.9.4/example/source/subpages/page5.rst
--rw-r--r--   0        0        0       87 2022-10-17 07:50:29.904956 sphinx_tagtoctree-0.9.4/example/source/subpages/page6.rst
--rw-r--r--   0        0        0      447 2022-10-17 12:26:10.928521 sphinx_tagtoctree-0.9.4/pyproject.toml
--rw-r--r--   0        0        0       64 2022-10-17 11:54:41.691763 sphinx_tagtoctree-0.9.4/requirements.txt
--rw-r--r--   0        0        0     3206 2022-10-17 12:13:01.608459 sphinx_tagtoctree-0.9.4/src/sphinx_tagtoctree/__init__.py
--rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 sphinx_tagtoctree-0.9.4/PKG-INFO
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.226038 sphinx_tagtoctree-0.9.5.0a1/
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.202288 sphinx_tagtoctree-0.9.5.0a1/.github/
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.207675 sphinx_tagtoctree-0.9.5.0a1/.github/workflows/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      734 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/.github/workflows/pythonpublish.yml
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.209184 sphinx_tagtoctree-0.9.5.0a1/.vscode/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      511 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/.vscode/launch.json
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      174 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/.vscode/settings.json
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       64 2024-05-09 12:08:44.000000 sphinx_tagtoctree-0.9.5.0a1/AUTHORS
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      935 2024-05-09 11:56:44.000000 sphinx_tagtoctree-0.9.5.0a1/CONTRIBUTING.md
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      495 2024-05-09 12:08:44.000000 sphinx_tagtoctree-0.9.5.0a1/ChangeLog
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    35141 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/LICENSE
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       36 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/MANIFEST.in
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      576 2024-05-09 12:08:45.225805 sphinx_tagtoctree-0.9.5.0a1/PKG-INFO
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     3386 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/README.md
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.214019 sphinx_tagtoctree-0.9.5.0a1/docs/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    11074 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-16-53-11.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    10136 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-16-56-16.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    10136 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-17-21-26.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    18570 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-17-21-57.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    11074 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-17-22-22.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    11193 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-17-22-54.png
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.215666 sphinx_tagtoctree-0.9.5.0a1/example/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      638 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/example/Makefile
+-rw-r--r--   0 half.scheidl   (502) staff       (20)        0 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/example/README.md
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      770 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a1/example/make.bat
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.219350 sphinx_tagtoctree-0.9.5.0a1/example/source/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     2004 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/conf.py
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     3099 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/index.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      156 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/page1.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      115 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/page2.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      161 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/page3.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      123 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/page4.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      166 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/page5.rst
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.221161 sphinx_tagtoctree-0.9.5.0a1/example/source/subpages/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      417 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/subpages/banana.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      113 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/subpages/sales.rst
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.222005 sphinx_tagtoctree-0.9.5.0a1/example/source/tags-with-hyphens/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      128 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/tags-with-hyphens/product-special.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     1423 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/example/source/tags-with-hyphens/sales-special.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       30 2024-05-09 11:37:30.000000 sphinx_tagtoctree-0.9.5.0a1/requirements.txt
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      577 2024-05-09 12:08:45.226722 sphinx_tagtoctree-0.9.5.0a1/setup.cfg
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      103 2024-05-09 11:26:54.000000 sphinx_tagtoctree-0.9.5.0a1/setup.py
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.225295 sphinx_tagtoctree-0.9.5.0a1/sphinx_tagtoctree.egg-info/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      576 2024-05-09 12:08:44.000000 sphinx_tagtoctree-0.9.5.0a1/sphinx_tagtoctree.egg-info/PKG-INFO
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     1063 2024-05-09 12:08:45.000000 sphinx_tagtoctree-0.9.5.0a1/sphinx_tagtoctree.egg-info/SOURCES.txt
+-rw-r--r--   0 half.scheidl   (502) staff       (20)        1 2024-05-09 12:08:44.000000 sphinx_tagtoctree-0.9.5.0a1/sphinx_tagtoctree.egg-info/dependency_links.txt
+-rw-r--r--   0 half.scheidl   (502) staff       (20)        1 2024-05-09 11:58:35.000000 sphinx_tagtoctree-0.9.5.0a1/sphinx_tagtoctree.egg-info/not-zip-safe
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       46 2024-05-09 12:08:44.000000 sphinx_tagtoctree-0.9.5.0a1/sphinx_tagtoctree.egg-info/pbr.json
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       31 2024-05-09 12:08:44.000000 sphinx_tagtoctree-0.9.5.0a1/sphinx_tagtoctree.egg-info/requires.txt
+-rw-r--r--   0 half.scheidl   (502) staff       (20)        1 2024-05-09 12:08:44.000000 sphinx_tagtoctree-0.9.5.0a1/sphinx_tagtoctree.egg-info/top_level.txt
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.203828 sphinx_tagtoctree-0.9.5.0a1/src/
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 12:08:45.224520 sphinx_tagtoctree-0.9.5.0a1/src/sphinx_tagtoctree/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     6933 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a1/src/sphinx_tagtoctree/__init__.py
```

### Comparing `sphinx_tagtoctree-0.9.4/.github/workflows/pythonpublish.yml` & `sphinx_tagtoctree-0.9.5.0a1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/LICENSE` & `sphinx_tagtoctree-0.9.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/docs/2019-11-26-16-53-11.png).png` & `sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-16-53-11.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/docs/2019-11-26-16-56-16.png).png` & `sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-16-56-16.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/docs/2019-11-26-17-21-26.png` & `sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-17-21-26.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/docs/2019-11-26-17-21-57.png` & `sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-17-21-57.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/docs/2019-11-26-17-22-22.png` & `sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-17-22-22.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/docs/2019-11-26-17-22-54.png` & `sphinx_tagtoctree-0.9.5.0a1/docs/2019-11-26-17-22-54.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/example/Makefile` & `sphinx_tagtoctree-0.9.5.0a1/example/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/example/make.bat` & `sphinx_tagtoctree-0.9.5.0a1/example/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.4/example/source/conf.py` & `sphinx_tagtoctree-0.9.5.0a1/example/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 # ones.
 
 extensions = [
  'sphinx_tagtoctree'
 ]
 
 tagtoctree_tag = 'tagtoctree'
+#list of characters allowed in tokens. Default = .:_
+tagtoctree_allowed_in_token=".:_-"
 keep_warnings = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
```

### Comparing `sphinx_tagtoctree-0.9.4/PKG-INFO` & `sphinx_tagtoctree-0.9.5.0a1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,64 @@
-Metadata-Version: 2.1
-Name: sphinx_tagtoctree
-Version: 0.9.4
-Summary: Sphinx table-of-contents with super powers!
-Author-email: Half Scheidl <noreply@hscheidl.com>
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: sphinx>=1.7.9
-Project-URL: Home, https://github.com/haschdl/sphinx-tagtoctree
-
 # Sphinx Extension: TagTocTree
 
 This is an extension to the documentation engine [Sphinx](http://www.sphinx-doc.org/).
-It allows you to include pages in a table-of-contents by using tags assigned to a page.
+It allows you to include pages in a table of contents by using tags assigned to a page.
 
 ## How it works
 
 This extension adds a new directive `tagtoctree`, which creates a tree-like
 table-of-contents, filtering pages by a tag filter.
 
 Directive    |   Configuration                   | Produces                          |
 -------------|-----------------------------------|-----------------------------------|
 `toctree` (*)| ![](docs/2019-11-26-17-21-26.png) | ![](docs/2019-11-26-17-21-57.png) |
 `tagtoctree` | ![](docs/2019-11-26-17-22-54.png) | ![](docs/2019-11-26-17-22-22.png) |
 
 (*) Sphinx native [`toctree`](https://www.sphinx-doc.org/en/1.8/usage/restructuredtext/directives.html#directive-toctree)
 
-## Usage
+## Installation
 
 The documentation assumes you have a Sphinx project running.
 
 - Install using PIP:
 
     ```bash
     pip install sphinx-tagtoctree
     ```
 
-- In your Sphinx configuration file (`conf.py`), add a entry for `tagtoctree`:
+- In your Sphinx configuration file (`conf.py`), add an entry for `tagtoctree`:
 
     ```python
     extensions = [
         'sphinx_tagtoctree'
     ]
     ```
 
-- (Optional) Add configuration value for `tagtoctree_tag`. If none is provided, the default `tagtoctree` will be used.
+## Configuration options
+
+Configurations that can be added to `conf.py`:
+
+1. `tagtoctree_tag`
+- (Optional) Add a configuration value for `tagtoctree_tag`. If none is provided, the default `tagtoctree` will be used. This is the tag you will add to your pages.
 
    ```python
    tagtoctree_tag = 'tagtoctree'
    ```
 
+2. `tagtoctree_allowed_in_token` 
+
+- (Optional) Add a configuration value for `tagtoctree_allowed_in_token` with a string  
+of specials characters that should be allowed in tags. If none is provided, the default `.:_` will be used. 
+
+   ```python
+   tagtoctree_allowed_in_token = '.:_-'
+   ```
+
+## Usage - simple tags
+
 - For each page, add a header on the top with the values of your tags. See examples [page1](/example/source/page1.rst) and
  [page2](/example/source/page2.rst) in this repo.
      
 - Finally, add a `tagtoctree` directive where you want your table-of-contents to be displayed. Example:
 
   ```rst
     .. tagtoctree::
@@ -60,7 +66,53 @@
     :glob:
     :caption: Pages with tag "Product"
     :tag: Product
 
     **
  ```
 
+## Usage - boolean filter
+
+You can specify a more complex filter using boolean expressions.
+Examples of valid expressions are:
+
+    * ``(Customer AND Product)`` Include pages with tags Customer and Product. 
+    * ``(Customer OR Product) AND NOT(Sales)`` Include pages that have tags Customer or Product, but which do not have tag Sales. Equivalent to ``(Customer OR Product) AND ~ Sales``
+    * ``(NOT Customer) AND NOT(Sales)`` Include pages that do have neither Customer nor Product.
+    
+Examples:
+
+```rst
+.. tagtoctree::
+   :maxdepth: 1
+   :glob:
+   :caption: Pages filtered with an expression: (Customer AND Product)
+   :tag_expr: Customer AND Product
+
+   **
+
+.. tagtoctree::
+   :maxdepth: 1
+   :glob:
+   :caption: Pages filtered with an expression: (Customer OR Product) AND Sales
+   :tag_expr: (Customer OR Product) AND Sales
+
+   **
+
+
+.. tagtoctree::
+   :maxdepth: 1
+   :glob:
+   :caption: Pages filtered with an expression: (Customer OR Product) AND NOT Sales
+   :tag_expr: (Customer OR Product) AND NOT Sales
+
+   **
+
+
+.. tagtoctree::
+   :maxdepth: 1
+   :glob:
+   :caption: Pages filtered with an expression: (NOT Customer) AND NOT(Sales)
+   :tag_expr: (NOT Customer) AND NOT(Sales)
+
+   **
+```
```


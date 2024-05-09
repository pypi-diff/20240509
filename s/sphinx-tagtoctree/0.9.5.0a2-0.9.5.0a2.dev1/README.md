# Comparing `tmp/sphinx_tagtoctree-0.9.5.0a2.tar.gz` & `tmp/sphinx_tagtoctree-0.9.5.0a2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_tagtoctree-0.9.5.0a2.tar", last modified: Thu May  9 13:22:50 2024, max compression
+gzip compressed data, was "sphinx_tagtoctree-0.9.5.0a2.dev1.tar", last modified: Thu May  9 13:19:44 2024, max compression
```

## Comparing `sphinx_tagtoctree-0.9.5.0a2.tar` & `sphinx_tagtoctree-0.9.5.0a2.dev1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.582780 sphinx_tagtoctree-0.9.5.0a2/
--rw-r--r--   0 half.scheidl   (502) staff       (20)     8196 2024-05-09 12:18:54.000000 sphinx_tagtoctree-0.9.5.0a2/.DS_Store
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.558999 sphinx_tagtoctree-0.9.5.0a2/.github/
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.564822 sphinx_tagtoctree-0.9.5.0a2/.github/workflows/
--rw-r--r--   0 half.scheidl   (502) staff       (20)      734 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/.github/workflows/pythonpublish.yml
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.566129 sphinx_tagtoctree-0.9.5.0a2/.vscode/
--rw-r--r--   0 half.scheidl   (502) staff       (20)      511 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/.vscode/launch.json
--rw-r--r--   0 half.scheidl   (502) staff       (20)      174 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/.vscode/settings.json
--rw-r--r--   0 half.scheidl   (502) staff       (20)       64 2024-05-09 13:22:49.000000 sphinx_tagtoctree-0.9.5.0a2/AUTHORS
--rw-r--r--   0 half.scheidl   (502) staff       (20)      935 2024-05-09 11:56:44.000000 sphinx_tagtoctree-0.9.5.0a2/CONTRIBUTING.md
--rw-r--r--   0 half.scheidl   (502) staff       (20)      552 2024-05-09 13:22:49.000000 sphinx_tagtoctree-0.9.5.0a2/ChangeLog
--rw-r--r--   0 half.scheidl   (502) staff       (20)    35141 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/LICENSE
--rw-r--r--   0 half.scheidl   (502) staff       (20)       36 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/MANIFEST.in
--rw-r--r--   0 half.scheidl   (502) staff       (20)      576 2024-05-09 13:22:50.582671 sphinx_tagtoctree-0.9.5.0a2/PKG-INFO
--rw-r--r--   0 half.scheidl   (502) staff       (20)     3386 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/README.md
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.569508 sphinx_tagtoctree-0.9.5.0a2/docs/
--rw-r--r--   0 half.scheidl   (502) staff       (20)    11074 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-16-53-11.png
--rw-r--r--   0 half.scheidl   (502) staff       (20)    10136 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-16-56-16.png
--rw-r--r--   0 half.scheidl   (502) staff       (20)    10136 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-17-21-26.png
--rw-r--r--   0 half.scheidl   (502) staff       (20)    18570 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-17-21-57.png
--rw-r--r--   0 half.scheidl   (502) staff       (20)    11074 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-17-22-22.png
--rw-r--r--   0 half.scheidl   (502) staff       (20)    11193 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-17-22-54.png
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.571286 sphinx_tagtoctree-0.9.5.0a2/example/
--rw-r--r--   0 half.scheidl   (502) staff       (20)      638 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/example/Makefile
--rw-r--r--   0 half.scheidl   (502) staff       (20)        0 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/example/README.md
--rw-r--r--   0 half.scheidl   (502) staff       (20)      770 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2/example/make.bat
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.575277 sphinx_tagtoctree-0.9.5.0a2/example/source/
--rw-r--r--   0 half.scheidl   (502) staff       (20)     2004 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/conf.py
--rw-r--r--   0 half.scheidl   (502) staff       (20)     3099 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/index.rst
--rw-r--r--   0 half.scheidl   (502) staff       (20)      156 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/page1.rst
--rw-r--r--   0 half.scheidl   (502) staff       (20)      115 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/page2.rst
--rw-r--r--   0 half.scheidl   (502) staff       (20)      161 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/page3.rst
--rw-r--r--   0 half.scheidl   (502) staff       (20)      123 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/page4.rst
--rw-r--r--   0 half.scheidl   (502) staff       (20)      166 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/page5.rst
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.577256 sphinx_tagtoctree-0.9.5.0a2/example/source/subpages/
--rw-r--r--   0 half.scheidl   (502) staff       (20)      417 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/subpages/banana.rst
--rw-r--r--   0 half.scheidl   (502) staff       (20)      113 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/subpages/sales.rst
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.578162 sphinx_tagtoctree-0.9.5.0a2/example/source/tags-with-hyphens/
--rw-r--r--   0 half.scheidl   (502) staff       (20)      128 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/tags-with-hyphens/product-special.rst
--rw-r--r--   0 half.scheidl   (502) staff       (20)     1423 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2/example/source/tags-with-hyphens/sales-special.rst
--rw-r--r--   0 half.scheidl   (502) staff       (20)       30 2024-05-09 11:37:30.000000 sphinx_tagtoctree-0.9.5.0a2/requirements.txt
--rw-r--r--   0 half.scheidl   (502) staff       (20)      635 2024-05-09 13:22:50.583168 sphinx_tagtoctree-0.9.5.0a2/setup.cfg
--rw-r--r--   0 half.scheidl   (502) staff       (20)      103 2024-05-09 11:26:54.000000 sphinx_tagtoctree-0.9.5.0a2/setup.py
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.560334 sphinx_tagtoctree-0.9.5.0a2/src/
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.578393 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree/
--rw-r--r--   0 half.scheidl   (502) staff       (20)     6941 2024-05-09 13:18:44.000000 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree/__init__.py
-drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:22:50.582240 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/
--rw-r--r--   0 half.scheidl   (502) staff       (20)      576 2024-05-09 13:22:50.000000 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/PKG-INFO
--rw-r--r--   0 half.scheidl   (502) staff       (20)     1101 2024-05-09 13:22:50.000000 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/SOURCES.txt
--rw-r--r--   0 half.scheidl   (502) staff       (20)        1 2024-05-09 13:22:50.000000 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/dependency_links.txt
--rw-r--r--   0 half.scheidl   (502) staff       (20)        1 2024-05-09 13:05:53.000000 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/not-zip-safe
--rw-r--r--   0 half.scheidl   (502) staff       (20)       46 2024-05-09 13:22:50.000000 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/pbr.json
--rw-r--r--   0 half.scheidl   (502) staff       (20)       31 2024-05-09 13:22:50.000000 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/requires.txt
--rw-r--r--   0 half.scheidl   (502) staff       (20)       18 2024-05-09 13:22:50.000000 sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/top_level.txt
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.946603 sphinx_tagtoctree-0.9.5.0a2.dev1/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     8196 2024-05-09 12:18:54.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/.DS_Store
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.921658 sphinx_tagtoctree-0.9.5.0a2.dev1/.github/
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.929000 sphinx_tagtoctree-0.9.5.0a2.dev1/.github/workflows/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      734 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/.github/workflows/pythonpublish.yml
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.929766 sphinx_tagtoctree-0.9.5.0a2.dev1/.vscode/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      511 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/.vscode/launch.json
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      174 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/.vscode/settings.json
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       64 2024-05-09 13:19:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/AUTHORS
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      935 2024-05-09 11:56:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/CONTRIBUTING.md
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      510 2024-05-09 13:19:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/ChangeLog
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    35141 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/LICENSE
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       36 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/MANIFEST.in
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      581 2024-05-09 13:19:44.946412 sphinx_tagtoctree-0.9.5.0a2.dev1/PKG-INFO
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     3386 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/README.md
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.934077 sphinx_tagtoctree-0.9.5.0a2.dev1/docs/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    11074 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-16-53-11.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    10136 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-16-56-16.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    10136 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-17-21-26.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    18570 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-17-21-57.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    11074 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-17-22-22.png
+-rw-r--r--   0 half.scheidl   (502) staff       (20)    11193 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-17-22-54.png
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.935070 sphinx_tagtoctree-0.9.5.0a2.dev1/example/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      638 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/Makefile
+-rw-r--r--   0 half.scheidl   (502) staff       (20)        0 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/README.md
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      770 2024-05-01 21:24:05.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/make.bat
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.938802 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     2004 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/conf.py
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     3099 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/index.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      156 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/page1.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      115 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/page2.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      161 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/page3.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      123 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/page4.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      166 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/page5.rst
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.940567 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/subpages/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      417 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/subpages/banana.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      113 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/subpages/sales.rst
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.941316 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/tags-with-hyphens/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      128 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/tags-with-hyphens/product-special.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     1423 2024-05-09 09:42:36.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/tags-with-hyphens/sales-special.rst
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       30 2024-05-09 11:37:30.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/requirements.txt
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      635 2024-05-09 13:19:44.947087 sphinx_tagtoctree-0.9.5.0a2.dev1/setup.cfg
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      103 2024-05-09 11:26:54.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/setup.py
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.923509 sphinx_tagtoctree-0.9.5.0a2.dev1/src/
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.941558 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     6941 2024-05-09 13:18:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree/__init__.py
+drwxr-xr-x   0 half.scheidl   (502) staff       (20)        0 2024-05-09 13:19:44.945559 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/
+-rw-r--r--   0 half.scheidl   (502) staff       (20)      581 2024-05-09 13:19:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/PKG-INFO
+-rw-r--r--   0 half.scheidl   (502) staff       (20)     1101 2024-05-09 13:19:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/SOURCES.txt
+-rw-r--r--   0 half.scheidl   (502) staff       (20)        1 2024-05-09 13:19:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/dependency_links.txt
+-rw-r--r--   0 half.scheidl   (502) staff       (20)        1 2024-05-09 13:05:53.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/not-zip-safe
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       47 2024-05-09 13:19:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/pbr.json
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       31 2024-05-09 13:19:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/requires.txt
+-rw-r--r--   0 half.scheidl   (502) staff       (20)       18 2024-05-09 13:19:44.000000 sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/top_level.txt
```

### Comparing `sphinx_tagtoctree-0.9.5.0a2/.DS_Store` & `sphinx_tagtoctree-0.9.5.0a2.dev1/.DS_Store`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/.github/workflows/pythonpublish.yml` & `sphinx_tagtoctree-0.9.5.0a2.dev1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/CONTRIBUTING.md` & `sphinx_tagtoctree-0.9.5.0a2.dev1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/LICENSE` & `sphinx_tagtoctree-0.9.5.0a2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/PKG-INFO` & `sphinx_tagtoctree-0.9.5.0a2.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-tagtoctree
-Version: 0.9.5.0a2
+Version: 0.9.5.0a2.dev1
 Summary: Sphinx table-of-contents with super powers
 Home-page: https://github.com/haschdl/sphinx-tagtoctree
 Author: Half Scheidl
 Author-email: noreply@hscheidl.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sphinx_tagtoctree-0.9.5.0a2/README.md` & `sphinx_tagtoctree-0.9.5.0a2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-16-53-11.png` & `sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-16-53-11.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-16-56-16.png` & `sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-16-56-16.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-17-21-26.png` & `sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-17-21-26.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-17-21-57.png` & `sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-17-21-57.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-17-22-22.png` & `sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-17-22-22.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/docs/2019-11-26-17-22-54.png` & `sphinx_tagtoctree-0.9.5.0a2.dev1/docs/2019-11-26-17-22-54.png`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/example/Makefile` & `sphinx_tagtoctree-0.9.5.0a2.dev1/example/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/example/make.bat` & `sphinx_tagtoctree-0.9.5.0a2.dev1/example/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/example/source/conf.py` & `sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/example/source/index.rst` & `sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/example/source/tags-with-hyphens/sales-special.rst` & `sphinx_tagtoctree-0.9.5.0a2.dev1/example/source/tags-with-hyphens/sales-special.rst`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/setup.cfg` & `sphinx_tagtoctree-0.9.5.0a2.dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree/__init__.py` & `sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/PKG-INFO` & `sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-tagtoctree
-Version: 0.9.5.0a2
+Version: 0.9.5.0a2.dev1
 Summary: Sphinx table-of-contents with super powers
 Home-page: https://github.com/haschdl/sphinx-tagtoctree
 Author: Half Scheidl
 Author-email: noreply@hscheidl.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sphinx_tagtoctree-0.9.5.0a2/src/sphinx_tagtoctree.egg-info/SOURCES.txt` & `sphinx_tagtoctree-0.9.5.0a2.dev1/src/sphinx_tagtoctree.egg-info/SOURCES.txt`

 * *Files identical despite different names*


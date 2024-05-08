# Comparing `tmp/unimenu-0.4.4.tar.gz` & `tmp/unimenu-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimenu-0.4.4.tar", last modified: Wed May  8 22:44:36 2024, max compression
+gzip compressed data, was "unimenu-3.0.0.tar", last modified: Thu Mar  2 15:01:18 2023, max compression
```

## Comparing `unimenu-0.4.4.tar` & `unimenu-3.0.0.tar`

### file list

```diff
@@ -1,63 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:36.291920 unimenu-0.4.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:36.279920 unimenu-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:36.279920 unimenu-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-08 22:44:31.000000 unimenu-0.4.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-08 22:44:31.000000 unimenu-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-08 22:44:31.000000 unimenu-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 22:44:31.000000 unimenu-0.4.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-08 22:44:36.291920 unimenu-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-05-08 22:44:31.000000 unimenu-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:36.283920 unimenu-0.4.4/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:36.283920 unimenu-0.4.4/dev/manual_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/manual_tests/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/manual_tests/substance_painter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:36.287920 unimenu-0.4.4/dev/unimenu_samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/any_dcc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/blender_custom_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/maya_startup_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_config_blender.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_config_unreal.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_config_unreal_append.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_screen_katana.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    45728 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_screen_krita.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    25598 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_screen_mari.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_screen_maya.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    16108 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_screen_nuke.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    27646 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_screen_substance_painter.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    71130 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_screen_system_tray.png
--rw-r--r--   0 runner    (1001) docker     (127)    45940 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_screen_unreal5.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    47311 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/menu_screen_unreal_context.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/nuke_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/qt_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/qt_system_tray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-08 22:44:31.000000 unimenu-0.4.4/dev/unimenu_samples/unreal_context_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-08 22:44:31.000000 unimenu-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:44:36.291920 unimenu-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:36.287920 unimenu-0.4.4/unimenu/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:36.287920 unimenu-0.4.4/unimenu/apps/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/hiero.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/katana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/mari.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/marmoset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/max.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/maya.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/nuke.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/qt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/apps/unreal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-08 22:44:31.000000 unimenu-0.4.4/unimenu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:36.291920 unimenu-0.4.4/unimenu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-08 22:44:36.000000 unimenu-0.4.4/unimenu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 22:44:36.000000 unimenu-0.4.4/unimenu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:44:36.000000 unimenu-0.4.4/unimenu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 22:44:36.000000 unimenu-0.4.4/unimenu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 22:44:36.000000 unimenu-0.4.4/unimenu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.114274 unimenu-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.114274 unimenu-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-03-02 15:01:06.000000 unimenu-3.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-03-02 15:01:06.000000 unimenu-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-02 15:01:06.000000 unimenu-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-02 15:01:18.118274 unimenu-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-02 15:01:06.000000 unimenu-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.114274 unimenu-3.0.0/manual_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-02 15:01:06.000000 unimenu-3.0.0/manual_tests/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-02 15:01:06.000000 unimenu-3.0.0/manual_tests/substance_painter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-02 15:01:06.000000 unimenu-3.0.0/openmenu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-02 15:01:06.000000 unimenu-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/any_dcc_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/maya_startup_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_config_blender.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_config_unreal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_config_unreal_append.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    45728 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_screen_krita.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_screen_maya.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38386 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_screen_substance_painter.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    45940 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/menu_screen_unreal5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-02 15:01:06.000000 unimenu-3.0.0/samples/qt_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 15:01:18.118274 unimenu-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/unimenu/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/unimenu/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/blender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/marmoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/maya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/apps/unreal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-03-02 15:01:06.000000 unimenu-3.0.0/unimenu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:01:18.118274 unimenu-3.0.0/unimenu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-02 15:01:18.000000 unimenu-3.0.0/unimenu.egg-info/top_level.txt
```

### Comparing `unimenu-0.4.4/.github/workflows/python-publish.yml` & `unimenu-3.0.0/.github/workflows/python-publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 permissions:
   contents: read
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
-    environment:
-      name: PyPI
-      url: https://pypi.org/p/unimenu
+
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
```

### Comparing `unimenu-0.4.4/.gitignore` & `unimenu-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.4/.pre-commit-config.yaml` & `unimenu-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.4/dev/manual_tests/generic.py` & `unimenu-3.0.0/manual_tests/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     # 'C:\\Users\\hanne\\OneDrive\\Documents\\Adobe\\Adobe Substance 3D Painter\\python\\modules\\samples\\config.json'
     config = Path(r"C:\Users\hanne\OneDrive\Documents\repos\unimenu\samples\config.json")
 
     # add single entry to menu
     menu1 = unimenu.add_item("menu1")
 
     # add menu tree from config
-    menu2 = unimenu.setup(config)[0]
+    menu2 = unimenu.setup_config(config)[0]
 
     # print(menu2)
     # in susbtance painter, this throws a
     # [Python] RuntimeError: Internal C++ object (PySide2.QtWidgets.QMenu) already deleted.
 
     # add submenu to menu
     sub_menu1 = unimenu.add_item("menu3", parent=menu2)
```

### Comparing `unimenu-0.4.4/dev/pyproject.toml` & `unimenu-3.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 #build-backend = "setuptools.build_meta"
 
 
 [tool.setuptools]
-packages = ["unimenu_samples"]  # todo later add tests
+packages = ["unimenu"]
 
 
 [project]
-name = "unimenu-dev"
+name = "unimenu"
 authors = [
     {name = "hannes"},
 ]
-description = "modules to help with unimenu development"
+description = "easy menus from a single config across apps"
 readme = "README.md"
 requires-python = ">=3.4"
-keywords = ["unimenu", "menu", "dev"]
-# license = { file = "LICENSE" }
+keywords = ["dcc", "pipeline", "menu", "config"]
+#license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 dependencies = [
-    'importlib-metadata; python_version<"3.7"', "unimenu",
+    'importlib-metadata; python_version<"3.7"',
 ]
 #dynamic = ["version"]
-version = "0.0.1"
+version = "3.0.0"
 
 [project.optional-dependencies]
 yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

### Comparing `unimenu-0.4.4/dev/unimenu_samples/any_dcc_test.py` & `unimenu-3.0.0/samples/any_dcc_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             "command": "print('Item 2')"
         }
     ]
 }
 
 
 config = {
-    'label': 'UniMenu Tools',
+    'label': 'Tools',
     'items':
         [
             {
                 'command': 'print("hello 1")',
                 'label': 'tool1',
                 "icon": ":/qt-project.org/styles/commonstyle/images/up-32.png",
                 "tooltip": "tooltip"
@@ -65,11 +65,12 @@
                     ]
             }
         ]
 }
 
 app_menu_node = unimenu.setup(config)
 
+
 # test teardown
-# node = unimenu.load(config)
-# app_node = node.setup()
-# node.teardown()
+node = unimenu.load(config)
+app_node = node.setup()
+node.teardown()
```

### Comparing `unimenu-0.4.4/dev/unimenu_samples/config.json` & `unimenu-3.0.0/samples/config.json`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.4/dev/unimenu_samples/maya_startup_plugin.py` & `unimenu-3.0.0/samples/maya_startup_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                 "label": "Item 2",
                 "command": "print('Item 2')"
             }
         ]
     }
 
     global menu
-    menu = unimenu.setup(config)
+    menu = unimenu.setup_dict(config)
     # todo use new node class
 
 
 def unload():
     import unimenu
     global menu
     unimenu.teardown_menu(menu)  # same name as top label in config
```

### Comparing `unimenu-0.4.4/dev/unimenu_samples/menu_screen_krita.jpg` & `unimenu-3.0.0/samples/menu_screen_krita.jpg`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.4/dev/unimenu_samples/menu_screen_unreal5.jpg` & `unimenu-3.0.0/samples/menu_screen_unreal5.jpg`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.4/dev/unimenu_samples/qt_sample.py` & `unimenu-3.0.0/samples/qt_sample.py`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.4/unimenu/apps/__init__.py` & `unimenu-3.0.0/unimenu/apps/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def menu_module(self) -> types.ModuleType:
         """
         the app-specific menu module, lazy import prevents import issues with other apps
         """
         return importlib.import_module(f"unimenu.apps.{self.name}")
 
     @property
-    def menu_node_class(self) -> "unimenu.apps._abstract.MenuNodeAbstract":  # typehint string to avoid circular import
+    def menu_node_class(self) -> "unimenu.apps._abstract.MenuNodeAbstract":  # " in typehint to avoid circular import
         """get the app-specific menu node class"""
         name = self.name.replace("_", " ").title().replace(" ", "")  # convert lower_case to CamelCase
         return getattr(self.menu_module, "MenuNode" + name)  # get the MenuNode class from the app module
 
 
 class SupportedApps:
     """Apps supported by this module, no need to add non QT apps here"""
@@ -45,18 +45,14 @@
     MAYA = App(name="maya", module="maya")  # pymel can be slow to import
     UNREAL = App(name="unreal", module="unreal")
     MAX = App(name="max", module="pymxs")
     KRITA = App(name="krita", module="krita")
     SUBSTANCE_DESIGNER = App(name="substance_designer", module="pysbs")
     SUBSTANCE_PAINTER = App(name="substance_painter", module="substance_painter")
     MARMOSET = App(name="marmoset", module="mset")
-    NUKE = App(name="nuke", module="nuke")
-    HIERO = App(name="hiero", module="hiero")
-    KATANA = App(name="katana", module="katana")
-    MARI = App(name="mari", module="mari")
 
     QT = App("qt", None)
 
     # ALL = [BLENDER, MAYA, UNREAL, KRITA, SUBSTANCE_PAINTER, MAX, MARMOSET]
     NON_QT = [BLENDER, UNREAL, SUBSTANCE_PAINTER, MARMOSET]
```

### Comparing `unimenu-0.4.4/unimenu/apps/_abstract.py` & `unimenu-3.0.0/unimenu/apps/_abstract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from abc import abstractmethod, ABC
 import unimenu.utils
 from pathlib import Path
-import logging
-import re
-import traceback
 
 
 class MenuNode(object):
     """
     data class for menu items, this can be loaded in python in any app
     """
     unigue_names = set()
@@ -22,75 +19,65 @@
         :param tooltip: the tooltip of the menu item
         :param separator: if True, this menu item will be a separator
         :param items: a list of menu items
         :param kwargs: the kwargs to pass to the app-node instance
         :param data: custom data to store in the node, this is not used by unimenu, e.g. category, tags, etc
         :param parent_path: used to parent the tree to a parent, only used by the root-node
         :param app_node: HELPER linking the app menu node created by a MenuNode instance, tries to create a bidirectional link
-        :param parent: HELPER linking the parent menu item, automatically set on children created from the 'items' kwarg
+        :param parent: HELPER linking the parent menu item, automatically set on child nodes when loaded from a config
         """
 
         # config data
         self.label = label or ""
         self.command = command or ""
         self.icon = icon or ""
         self.tooltip = tooltip or ""
         self.separator = separator or False
+        items = items or []
+        self.items: list[MenuNodeAbstract] = [self.__class__(**item) for item in items]
         self.kwargs = kwargs or {}
         self.data = data or {}
         self.id = id or None
 
-        # only the root node needs parent_path
-        if parent_path:
-            self.parent_path: str = parent_path.replace(" ", "_")
-        else:
-            self.parent_path = None
+        self.parent_path = parent_path  # only the root node needs this
         # todo get parent path method
 
         # helpers
         self.parent: MenuNode = parent  # some implicit code use, pay attention to parent
         self.config_path = None  # the path to the config file that created this node todo do non root nodes populate this?
         
         # todo move to abstract
         self.app_node = app_node  # the app menu node created by this MenuNode instance
         self.app_node_parent = None  # root node only
 
         self._default_id()
 
-        # since we pass parent, create items at end of init, so we first set all parent(self) attrs
-        items = items or []
-        self.items: list[MenuNodeAbstract] = [self.__class__(**item, parent=self) for item in items]
-
     def _default_id(self):
         # todo ideally should be unique
         
         if self.id:
             return
 
         label = self.label
         if not label:
             label = "TODO"  # todo unique number
 
-
-        label = re.sub('[^0-9a-zA-Z]+', '_', label)  # replace non alphanumeric with _
-
-        # add parent path to the id. ensures unique ids.
-        # note that in e.g. unreal, the "name" is a type of id, that needs to be unique. but only one level deep.
-        # so using id for name might result in repeated parent names. e.g. "parentA.ParentA_menuB"
         parent_names = []
         parent = self.parent
         while parent:
-            parent_names.append(parent.id)  # todo, since id includes parent, adding parent id adds root parent multiple times
+            parent_names.append(parent.id)
             parent = parent.parent
         parent_names.reverse()
-        parent_names.append(label)
+        parent_names.append(self.label)
         self.id = "_".join(parent_names)
-        # todo update this when parent changes, change to property
-        # but if we rely on id to identify a node, then changing it when parent changes is bad
-        # inform user that this string can change, they can save a pointer to the python instance instead
+
+
+    @property
+    def try_command(self):
+        return f"import unimenu.utils; unimenu.utils.try_command(r'{self.command}')"
 
     @property
     def children(self):
         return self.items
 
     @children.setter
     def children(self, value):
@@ -103,32 +90,32 @@
         for child in self.children:
             children.append(child)
             children.extend(child.all_children)
         return children
 
     @property
     def all_command_nodes(self):
-        """return: every menu entry that has a command"""
+        """return every menu entry that has a command"""
         commands = []
         for child in self.children:
             if child.command:
                 commands.append(child)
             commands.extend(child.all_command_nodes)
         return commands
 
     def root(self):
-        """return: the root node of the menu-tree"""
+        """Return the root node of the menu-tree"""
         # we use isinstance since sometimes parent is a string (or other type)
         # e.g. when the menu is loaded from a config file, the root node might have a string as parent
         if self.parent and isinstance(self.parent, MenuNode):
             return self.parent.root()
         return self
 
     def __dict__ (self):
-        """return: a dict representation of this menu-node, used to save to a config file """
+        # used to save back to a config file
         config = {}
         if self.label:
             config["label"] = self.label
         if self.command:
             config["command"] = self.command
         if self.icon:
             config["icon"] = self.icon
@@ -139,57 +126,44 @@
         if self.items:
             child_configs = []
             for item in self.items:
                 child_config = item.__dict__()
                 child_config.pop("parent", None)  # we only need to save the parent for the top node
                 child_configs.append(child_config)
             config["items"] = child_configs
-        if self.parent_path and isinstance(self.parent_path, str):
+        if self.parent and isinstance(self.parent, str):
             config["parent_path"] = self.parent_path
         if self.kwargs:
             config["kwargs"] = self.kwargs
         if self.data:
             config["data"] = self.data
         return config
 
-    def run(self, *args):  # some apps pass args to the command. e.g. maya passes False
+    def run(self):
         """execute the command in self.command, which accepts a function or string"""
-        try:
-            if isinstance(self.command, str):
-                # lambda: exec(self.command)
-                exec(self.command)
-            else:  # callable
-                self.command()
-        except Exception as e:
-            traceback.print_exc()
-            return e
+        if isinstance(self.command, str):
+            lambda: exec(self.command)
+        else:  # callable
+            self.command()
 
     @classmethod
     def load(cls, arg):
-        # if arg is a string, check if it's a valid Path
-        if isinstance(arg, str):
-            arg = Path(arg)
-            if not arg.exists():
-                logging.error(f"Path does not exist: {arg}")
-                return
-        # if arg is a Path, load from config
-        if isinstance(arg, Path):
+        # if arg is a Path or string, load from config
+        if isinstance(arg, (str, Path)):
             return cls.load_config(arg)
         # if arg is a dict, create a menu node from it
         elif isinstance(arg, dict):
             return cls(**arg)
         # if arg is a MenuNode, copy it
         elif isinstance(arg, MenuNode):
             return cls(**arg.__dict__())
 
     @classmethod
     def load_config(cls, config_path):
         data = unimenu.utils.load_config(config_path)
-        if not data:
-            logging.warning("Failed to load config")
         menu_node = cls(**data)
         menu_node.config_path = config_path
         for node in menu_node.all_children:
             node.config_path = config_path
         return menu_node
 
     def print_tree(self, indent=0):
@@ -211,39 +185,37 @@
     """
     Abstract class for app menu creation from a MenuNode tree
     """
 
     def setup(self, parent_app_node=None, backlink=True):
         """
         Instantiate a menu item in the app from the menu node data
-
-        parent_app_node: app menu node to parent to, not a (uni)MenuNode!
+        parent: app menu to parent to, not a MenuNode!
         backlink: if True, add an attribute to the app node instance to the app node
         """
         parent_app_node = parent_app_node or self._default_root_parent
 
         if self.separator:
             self.app_node = self._setup_separator(parent_app_node=parent_app_node)
 
         elif self.command:  # menu item
             self.app_node = self._setup_menu_item(parent_app_node=parent_app_node)
 
         elif self.items:  # submenu
             self.app_node = self._setup_sub_menu(parent_app_node=parent_app_node)
             for item in self.items:
                 item.setup(parent_app_node=self.app_node)
-        else:
-            logging.warning("Can not create a MenuNode that has no command or children: " + self.label)
 
         # some apps, e.g. unreal, don't allow adding attributes dynamically
         if backlink:
             try:
                 self.app_node.menu_node = self  # todo setproperty qt
             except AttributeError:
-                logging.warning(f"Warning: could not set backlink on {self.app_node} to {self}")
+                print(f"Warning: could not set backlink on {self.app_node} to {self}")
+                pass
 
         return self.app_node
 
     # todo consider moving to abstract, and func isntead of property
     # todo test with parent name in config for all apps
     # todo test with submenu name in config for all apps
     @property
```

### Comparing `unimenu-0.4.4/unimenu/apps/marmoset.py` & `unimenu-3.0.0/unimenu/apps/marmoset.py`

 * *Files identical despite different names*

### Comparing `unimenu-0.4.4/unimenu/apps/max.py` & `unimenu-3.0.0/unimenu/apps/max.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,25 +20,22 @@
         rt.menuMan.updateMenuBar()
 
     @property
     def _default_root_parent(self):
         return rt.menuMan.getMainMenuBar()
 
     def _setup_sub_menu(self, parent_app_node=None):
-        # todo unsure if **self.kwargs should be passed to createMenu or createSubMenuItem
         sub_menu = rt.menuMan.createMenu(self.label)
         sub_menu_item = rt.menuMan.createSubMenuItem(self.label, sub_menu)
         parent_app_node.addItem(sub_menu_item, -1)
         return sub_menu
 
     def _setup_menu_item(self, parent_app_node=None):
         tooltip = self.tooltip or ""
 
-        # todo unsure if **self.kwargs should be passed to create_macro or createActionItem
-
         # todo generated menus are persistent between sessions!
         #  this does not match the behavior of other Apps currently
         #  a macro is created at C:\Users\hanne\AppData\Local\Autodesk\3dsMax\2024 - 64bit\ENU\usermacros\
         macro_name, macro_category = create_macro(self.label, self.command)
         # todo handle case when we create a macro with the same name as an existing macro
         # since actionitems are based of macro names, we can't have two actionitems with the same name
         item = rt.menuMan.createActionItem(macro_name, macro_category)
```

### Comparing `unimenu-0.4.4/unimenu/apps/maya.py` & `unimenu-3.0.0/unimenu/apps/maya.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,113 @@
 """
 native maya menu support. not needed anymore, use the qt menu instead
-short menu names are the name of the menu node.
-long menu names are the name of the menu, and all its parents, separated by "|"
 """
+
+import pymel.core as pm  # todo replace with cmds because it's faster
 from unimenu.apps._abstract import MenuNodeAbstract
 import maya.mel
-import maya.cmds  # cmds is faster than pymel
-import re
+import maya.cmds
 
 
-def find_menu(long_name):
-    long_name = f"MayaWindow|{long_name}"  # for now we assume the menu is a child of the main window
-    long_menu_names = maya.cmds.lsUI(menus=True, long=True)
-    for long_menu_name in long_menu_names:
-        if long_menu_name == long_name:
-            return long_menu_name
+counter = 0
 
 
-def get_compatible_name(name):
-    name = re.sub('[^0-9a-zA-Z]+', '_', name)  # replace non alpha-numeric with _
-    name = name.strip("_")  # remove leading and trailing underscores
-    return name
+def get_counter():
+    global counter
+    counter += 1
+    return counter
 
 
-def get_unique_name(name, parent):
-    """
-    Guarantee a unique name compatible with maya naming conventions
-    name: str, the short name of the menu
-    parent: str, the long name of the parent menu
-    """
-    name = get_compatible_name(name)
-    long_name = f"{parent}|{name}"
-    long_menu_names = maya.cmds.lsUI(menus=True, long=True)
-    long_menu_item_names = maya.cmds.lsUI(menuItems=True, long=True)
-    if any(long_name == long_menu_name for long_menu_name in long_menu_names + long_menu_item_names):
-        # if the name is already taken, add a number to the end
-        # this could be improved by finding the next available number
-        name = f"{name}_1"
-        name = get_unique_name(name, parent)
-    return name
+def find_menu(name):
+    gMainWindow = maya.mel.eval('$temp=$gMainWindow')
+    # get all the menus that are children of the main menu
+    mainWindowMenus = maya.cmds.window(gMainWindow, query=True, menuArray=True)
+    for menu in mainWindowMenus:
+        if menu.lower() == name.lower():
+            return menu
+
+        # TODO get their children recursively
 
 
-def create_root_menu(label, window_name=None, kwargs=None) -> maya.cmds.menu:
+def create_root_menu(label, window_name=None, kwargs=None) -> pm.menu:
     """
     Create a root menu in Maya
     label: str, the label of the menu
     window_name: str, the name of the window to attach the menu to
     """
-    # todo add support for menus in other windows, e.g. the Script Editor
-    # # lsUI() might be able to replace pymel
-    # import pymel.core as pm
-    # window_name = window_name or "gMainWindow"  # default value
-    # maya_window = pm.language.melGlobals[window_name]  # returns "MayaWindow", type str
-    # same result as this
-    # maya_window = maya.mel.eval('$temp=$gMainWindow')
-    maya_window = "MayaWindow"  # hardcode main window for now
+    window_name = window_name or "gMainWindow"  # default value
+    maya_window = pm.language.melGlobals[window_name]
 
     # support adding custom kwargs from the config
     kwargs = kwargs or {}
     kwargs.setdefault("parent", maya_window)
     kwargs.setdefault("tearOff", True)
 
-    name = label.replace("_", " ")  # maya menu labels should have spaces, not underscores
+    # we require a predictable name to parent menus to from other configs, so no counter
+    # name = f"{label}_{get_counter()}"
+    name = label.replace("_", " ")  # maya menu names can't have underscores
 
-    return maya.cmds.menu(name, **kwargs)
+    return pm.menu(name, **kwargs)
 
 
 class MenuNodeMaya(MenuNodeAbstract):
 
     @property
     def _default_root_parent(self):
+
         # todo parent logic currently is re implemented in every app module
         #  can we move it to the abstract class?
         # if we provide a parent in the config, we might want to parent to a submenu
         if self.parent_path:
-            parent_path = get_compatible_name(self.parent_path)
+            parent_path = self.parent_path.replace(" ", "_")  # maya menu names can't have spaces
             return find_menu(parent_path)
 
     def _setup_sub_menu(self, parent_app_node=None):
-        self.name = get_unique_name(self.label, parent=parent_app_node)
-        kwargs = self.kwargs  # support adding custom kwargs from the config
+        # todo handle unique name, atm label can clash with other menu items
+
+        # support adding custom kwargs from the config
+        kwargs = self.kwargs
         kwargs.setdefault("tearOff", True)
+
         if not parent_app_node:
             return create_root_menu(self.label, kwargs=self.kwargs)
         else:  # make a normal sub menu
             kwargs.setdefault("subMenu", True)
             kwargs.setdefault("label", self.label)
             kwargs.setdefault("parent", parent_app_node)
-            return maya.cmds.menuItem(self.name, **kwargs)
+
+            self.name = f"{self.label}_{get_counter()}"
+            return pm.menuItem(self.name, **kwargs)
 
     def _setup_menu_item(self, parent_app_node=None):
-        self.name = get_unique_name(self.label, parent=parent_app_node)
         icon = self.icon or ""
-        tooltip = self.tooltip or "test"
-        kwargs = self.kwargs  # support adding custom kwargs from the config
+
+        # tooltip = self.tooltip or ""
+        # todo menuItem doesn't support tooltip.
+        #  could use qt instead http://discourse.techart.online/t/is-there-a-way-to-get-tooltips-for-maya-menitem/15385
+
+        # support adding custom kwargs from the config
+        kwargs = self.kwargs
         kwargs.setdefault("label", self.label)
-        kwargs.setdefault("command", self.run)
+        kwargs.setdefault("command", self.try_command)
         kwargs.setdefault("parent", parent_app_node)
         kwargs.setdefault("image", icon)
-        kwargs.setdefault("annotation", tooltip)  # shown on hover in lower left corner
-        return maya.cmds.menuItem(self.name, **kwargs)
+
+        self.name = f"{self.label}_{get_counter()}"
+
+        return pm.menuItem(self.name, **kwargs)
 
     def _setup_separator(self, parent_app_node=None):
-        self.name = get_unique_name(self.label, parent=parent_app_node)
-        kwargs = self.kwargs  # support adding custom kwargs from the config
+        self.name = f"{self.label}_{get_counter()}"
+
+        # support adding custom kwargs from the config
+        kwargs = self.kwargs
         kwargs.setdefault("divider", True)
         kwargs.setdefault("dividerLabel", self.label)
         kwargs.setdefault("parent", parent_app_node)
-        return maya.cmds.menuItem(self.name, **kwargs)
-
-    def teardown(self):
-        """Delete the menu item & its children"""
-        maya.cmds.deleteUI(self.name, menu=True)
 
+        return pm.menuItem(self.name, **kwargs)
 
-def teardown_menu(name):
-    maya.cmds.deleteUI(name, menu=True)
-    
+    def teardown(self):
+        # see https://stackoverflow.com/questions/44142119/remove-menu-item-in-maya-using-python
+        # todo can we remove self.name? bit hacky
+        pm.deleteUI(self.name, menu=True)
```

### Comparing `unimenu-0.4.4/unimenu/apps/qt.py` & `unimenu-3.0.0/unimenu/apps/qt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from unimenu.apps._abstract import MenuNodeAbstract
 import contextlib
-import logging
 
 
 with contextlib.suppress(ImportError):
     from PySide6 import QtGui, QtWidgets
     from PySide6.QtGui import QAction
 with contextlib.suppress(ImportError):
     from PyQt6 import QtGui, QtWidgets
@@ -15,87 +14,69 @@
 with contextlib.suppress(ImportError):
     from PyQt5 import QtGui, QtWidgets
     from PyQt5.QtWidgets import QAction
 
 
 menu_bar = None
 main_window = None
-
-
-def find_main_window():
-    # ideally there is only 1 main window, but there could be more
-    # e.g. Maya has a main window for arnold
-    widgets = [w for w in QtWidgets.QApplication.topLevelWidgets() if type(w) == QtWidgets.QMainWindow]
-    if len(widgets) == 1:
-        return widgets[0]
-    else:
-        logging.warning(f"found {len(widgets)} main windows,  can't auto select main window")
-
-    # a lot of apps have a main window named "mainWindow"
-    if not main_window:
-        for widget in QtWidgets.QApplication.topLevelWidgets():
-            if widget.objectName() in ("mainWindow", "MayaWindow"):  # MayaWindow hardcode hack
-                # print("FOUND MAIN WINDOW UNIMENU", main_window)
-                return widget
-
-
-def find_main_menu_bar(main_window, parent_path):
-    """
-    get the main menu bar widget from a main window,
-    or the sub menu widget if a sub path is provided
-    """
-    menu_bar = main_window.findChild(QtWidgets.QMenuBar)
-    if parent_path:
-        parent_menu = menu_bar.findChild(QtWidgets.QMenu, parent_path)
-        if not parent_menu:
-            logging.warning("Parent menu not found, using main menu bar")
-        else:
-            menu_bar = parent_menu
-    return menu_bar
-
-
 class MenuNodeQt(MenuNodeAbstract):
+
     @property
     def _default_root_parent(self):
         """
         get the default parent for the root node
         it finds the first QMainWindow in the app, and gets its menu bar
         if this is not the desired behaviour, override this method or set the parent of the root node before setup
         """
+
         # store in global, to avoid garbage collection of python pointer to c++ qt obj
-        global main_window
         global menu_bar
+        global main_window
+
+        for widget in QtWidgets.QApplication.topLevelWidgets():
+            if type(widget) == QtWidgets.QMainWindow:
+                main_window = widget
+                break
+
+        if not main_window:
+            for widget in QtWidgets.QApplication.topLevelWidgets():
+                if widget.objectName() == "mainWindow":
+                    print("FOUND MAIN WINDOW UNIMENU", main_window)
+                    main_window = widget
+                    break
 
-        main_window = find_main_window()
-        menu_bar = find_main_menu_bar(main_window, self.parent_path)
+        menu_bar = main_window.findChild(QtWidgets.QMenuBar)
         return menu_bar
 
     def _setup_sub_menu(self, parent_app_node=None) -> QtWidgets.QMenu:
-        menu = QtWidgets.QMenu(title=self.label, objectName=self.id, parent=parent_app_node, **self.kwargs)
+        menu = QtWidgets.QMenu(title=self.label, **self.kwargs)  # parent
+        global menu_bar
         if parent_app_node:
             parent_app_node.addMenu(menu)
         return menu
 
-    def _setup_menu_item(self, parent_app_node=None) -> QAction:
-        """
-        create a QAction from the MenuNode data
-        parent_app_node: the parent menu or menu bar
-        """
+    def _setup_menu_item(self, parent_app_node=None):
+        """create a QAction from the MenuNode data"""
 
         # A PySide.QtGui.QAction may contain an icon, menu text (label), a shortcut, status text,
         # “What’s This?” text, and a tooltip
 
         # todo support:
         #  openAct.setShortcuts(QKeySequence.Open)
         #  openAct.setStatusTip(tr("Open an existing file"))
         #  PySide.QtGui.QAction.setWhatsThis()
         #  PySide.QtGui.QAction.setFont()
 
-        action = QAction(self.label, objectName=self.id, **self.kwargs)
-        action.triggered.connect(self.run)
+        action = QAction(self.label, **self.kwargs)
+
+        # qt accepts callable commands, not just string commands
+        if isinstance(self.command, str):
+            action.triggered.connect(lambda: exec(self.command))
+        else:  # callable
+            action.triggered.connect(lambda: self.command())
 
         if self.tooltip:
             if parent_app_node:
                 parent_app_node.setToolTipsVisible(True)
             action.setToolTip(self.tooltip)
 
         if self.icon:
```

### Comparing `unimenu-0.4.4/unimenu/core.py` & `unimenu-3.0.0/unimenu/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import unimenu.apps._abstract
 from unimenu.apps import detect_app, App
 from unimenu.utils import getattr_recursive, load_config
 import os
 from pathlib import Path
 
 
-def load_module(module,
+def setup_module(module,
                  parent_menu: str = None,
-                 label: str = None,
+                 menu_name: str = None,
                  function_name: str = None,
                  icon: str = None,
                  tooltip: str = None,
                  app=None,
                  smart_spaces=True,
                  ):
     """
@@ -29,15 +29,15 @@
     Args:
     module: the name of the module that contains all tools. e.g.: "cool_tools"
                         cool_tools
                         ├─ __init__.py   (import cool_tools)
                         ├─ tool1.py      (import cool_tools.tool1)
                         └─ tool2.py      (import cool_tools.tool2)
     parent: the name of the parent menu to add our menu entries to
-    label: optional kwars to overwrite the name of the menu to create, defaults to module name
+    menu_name: optional kwars to overwrite the name of the menu to create, defaults to module name
     function_name: the function name to run on the module, e.g.: 'run', defaults to 'main'
                    if empty, call the module directly
     icon: the icon name to use for the menu entry, defaults to ''
     app: the app that contains the menu. if None, will try to detect app
     """
 
     function_name = function_name or "main"
@@ -85,35 +85,18 @@
         if tooltip:
             submodule_dict["tooltip"] = tooltip
         items.append(submodule_dict)
 
     data = {}
     if parent_menu:
         data["parent"] = parent_menu
-
-    label = label or parent_module.__name__
-    label = label.replace('_', ' ').title() if smart_spaces else label
-
-    data["label"] =  label
-    data["items"] =  items
+    data["items"] = [{"label": menu_name or parent_module.__name__, "items": items}]
 
     # use the generated dict to set up the menu
-    return load(data, app)
-
-
-def setup_module(module,
-                    parent_menu: str = None,
-                    label: str = None,
-                    function_name: str = None,
-                    icon: str = None,
-                    tooltip: str = None,
-                    app=None,
-                    smart_spaces=True,
-                    ):
-    return load_module(module, parent_menu, label, function_name, icon, tooltip, app, smart_spaces).setup()
+    return setup(data, app)
 
 
 def load(arg, app: App = None) -> unimenu.apps._abstract.MenuNodeAbstract:
     """
     smart menu load from a dict, config file or module
     arg: a config (dict or str/Path) or a module (to create a menu from a folder)
     """
@@ -156,16 +139,14 @@
 
 def teardown_menu(name, app=None):
     """remove the created menu"""
     # get the top menu with name X, and delete it and all submenus
     app = app or detect_app()
     return app.menu_module.teardown_menu(name)
 
-def teardown_menus(names, app=None):
-    return [teardown_menu(name, app) for name in names]
 
 def config_dir_paths() -> "list[Path]":
     raw_path = os.environ.get("UNIMENU_CONFIG_PATH", "")
     return [Path(x) for x in raw_path.split(os.pathsep) if x]
 
 
 def discover_config_paths() -> "list[Path]":
@@ -174,40 +155,38 @@
     configs = []
     for path in paths:
         configs.extend(path.rglob("*.json"))
         configs.extend(path.rglob("*.yaml"))
     return configs
 
 
-def load_all_configs() -> unimenu.apps._abstract.MenuNodeAbstract:
+def load_all_configs():
     """load all config files in the config paths"""
     nodes = []
     config_paths = discover_config_paths()
     for config_path in config_paths:
         node = load(config_path)
         nodes.append(node)
     return nodes
 
 
-def setup_all_configs() -> unimenu.apps._abstract.MenuNodeAbstract:
+def setup_all_configs():
     """setup all config files in the config paths"""
     config_paths = discover_config_paths()
 
     # register configs without parents first, to avoid creating the child before the parent.
     # note that this is not a perfect solution
 
-    root_nodes = []
-    child_nodes = []
+    configs1 = []
+    configs2 = []
 
     for config_path in config_paths:
         config_node = load(config_path)
         if not config_node.parent_path:
-            root_nodes.append(config_node)
+            configs1.append(config_node)
         else:
-            child_nodes.append(config_node)
+            configs2.append(config_node)
 
-    for node in root_nodes:
+    for node in configs1:
         node.setup()
-    for node in child_nodes:
+    for node in configs2:
         node.setup()
-
-    return root_nodes + child_nodes
```

### Comparing `unimenu-0.4.4/unimenu/utils.py` & `unimenu-3.0.0/unimenu/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,54 @@
 import json
 
 
-def load_json(config_path) -> dict:
+def load_json(config_path):
     """get json data from a file path, return None if not json"""
     path = str(config_path)
     if not path.lower().endswith(".json"):
         return
 
     with open(config_path) as file:
         data = json.load(file)
     return data
 
 
-def load_yaml(config_path) -> dict:
+def load_yaml(config_path):
     """get yaml data from a file path, return None if not yaml"""
     path = str(config_path)
     if not path.lower().endswith(".yaml"):
         return
 
     import yaml
 
     with open(config_path) as file:
         data = yaml.load(file, Loader=yaml.SafeLoader)
     return data
 
 
-def load_config(config_path) -> "dict|None":
+def load_config(config_path):
     """get data from a JSON or YAML config"""
     return load_json(config_path) or load_yaml(config_path)
 
 
-def save_json(data, path):
-    """save data to a json file"""
-    with open(path, "w") as file:
-        json.dump(data, file, indent=4)
-
-
-def save_yaml(data, path):
-    """save data to a yaml file"""
-    with open(path, "w") as file:
-        import yaml
-        yaml.dump(data, file, default_flow_style=False)
-
-
-def save_config(data, path):
-    """save data to a JSON or YAML config"""
-    if path.lower().endswith(".json"):
-        save_json(data, path)
-    elif path.lower().endswith(".yaml"):
-        save_yaml(data, path)
-    else:
-        raise ValueError("Invalid config file extension")
-
-
 def getattr_recursive(obj, attr: str):
     """
-    like getattr from python's std-lib, but recursive, supporting nested attributes
-    e.g. getattr_recursive(object, "mesh.name") is equivalent to object.mesh.name
-
+    getattr but recursive, supports nested attributes
     attr: provide either 1 attribute, or multiple separated by a dot
     """
     attributes = attr.split(".")
     for attribute in attributes:
         obj = getattr(obj, attribute)
     return obj
+
+
+def try_command(command, *args, **kwargs):
+    """try to run a command, return None if it fails & print the traceback"""
+    try:
+        # check if string
+        if isinstance(command, str):
+            return exec(command)
+        else:
+            return command(*args, **kwargs)
+    except Exception:
+        import traceback
+        traceback.print_exc()
```


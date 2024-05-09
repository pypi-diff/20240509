# Comparing `tmp/Subsearch-2.43.1.tar.gz` & `tmp/Subsearch-2.44.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.43.1.tar", last modified: Sat Jan 27 16:49:34 2024, max compression
+gzip compressed data, was "Subsearch-2.44.0.tar", last modified: Sun Jan 28 20:46:55 2024, max compression
```

## Comparing `Subsearch-2.43.1.tar` & `Subsearch-2.44.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.157012 Subsearch-2.43.1/
--rw-rw-rw-   0        0        0     1093 2024-01-27 16:48:50.000000 Subsearch-2.43.1/LICENSE
--rw-rw-rw-   0        0        0      121 2024-01-27 16:48:50.000000 Subsearch-2.43.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7765 2024-01-27 16:49:34.157012 Subsearch-2.43.1/PKG-INFO
--rw-rw-rw-   0        0        0     5961 2024-01-27 16:48:50.000000 Subsearch-2.43.1/README.md
--rw-rw-rw-   0        0        0     2609 2024-01-27 16:48:50.000000 Subsearch-2.43.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-27 16:49:34.157012 Subsearch-2.43.1/setup.cfg
--rw-rw-rw-   0        0        0      114 2024-01-27 16:48:50.000000 Subsearch-2.43.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.125837 Subsearch-2.43.1/src/
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.157012 Subsearch-2.43.1/src/Subsearch.egg-info/
--rw-rw-rw-   0        0        0     7765 2024-01-27 16:49:34.000000 Subsearch-2.43.1/src/Subsearch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2024-01-27 16:49:34.000000 Subsearch-2.43.1/src/Subsearch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-27 16:49:34.000000 Subsearch-2.43.1/src/Subsearch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-01-27 16:49:34.000000 Subsearch-2.43.1/src/Subsearch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-01-27 16:49:33.000000 Subsearch-2.43.1/src/Subsearch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      379 2024-01-27 16:49:34.000000 Subsearch-2.43.1/src/Subsearch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-27 16:49:34.000000 Subsearch-2.43.1/src/Subsearch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.141355 Subsearch-2.43.1/src/subsearch/
--rw-rw-rw-   0        0        0     1498 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/__init__.py
--rw-rw-rw-   0        0        0       38 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/__main__.py
--rw-rw-rw-   0        0        0     9175 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/core.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.141355 Subsearch-2.43.1/src/subsearch/data/
--rw-rw-rw-   0        0        0       99 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/data/__init__.py
--rw-rw-rw-   0        0        0       53 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/data/guid.py
--rw-rw-rw-   0        0        0     7704 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/data/language_data.toml
--rw-rw-rw-   0        0        0       24 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/data/version.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.141355 Subsearch-2.43.1/src/subsearch/globals/
--rw-rw-rw-   0        0        0        0 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/globals/__init__.py
--rw-rw-rw-   0        0        0      513 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/globals/constants.py
--rw-rw-rw-   0        0        0     2505 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/globals/dataclasses.py
--rw-rw-rw-   0        0        0     5622 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/globals/decorators.py
--rw-rw-rw-   0        0        0      980 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/globals/exceptions.py
--rw-rw-rw-   0        0        0      258 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/globals/metaclasses.py
--rw-rw-rw-   0        0        0     1597 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/globals/propagating_thread.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.141355 Subsearch-2.43.1/src/subsearch/gui/
--rw-rw-rw-   0        0        0      588 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/__init__.py
--rw-rw-rw-   0        0        0     3180 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/common_utils.py
--rw-rw-rw-   0        0        0     1053 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resource_loader.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.141355 Subsearch-2.43.1/src/subsearch/gui/resources/
--rw-rw-rw-   0        0        0        0 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.141355 Subsearch-2.43.1/src/subsearch/gui/resources/assets/
--rw-rw-rw-   0        0        0        0 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resources/assets/__init__.py
--rw-rw-rw-   0        0        0     7119 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resources/assets/spritesheet.png
--rw-rw-rw-   0        0        0   105808 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resources/assets/subsearch.ico
--rw-rw-rw-   0        0        0     1674 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resources/config.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.141355 Subsearch-2.43.1/src/subsearch/gui/resources/styles/
--rw-rw-rw-   0        0        0        0 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resources/styles/__init__.py
--rw-rw-rw-   0        0        0     1780 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resources/styles/sprites.tcl
--rw-rw-rw-   0        0        0     7247 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resources/styles/style_subsearch.tcl
--rw-rw-rw-   0        0        0     1451 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/resources/styles/theme_setter.tcl
--rw-rw-rw-   0        0        0     6865 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/screen_manager.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.141355 Subsearch-2.43.1/src/subsearch/gui/screens/
--rw-rw-rw-   0        0        0        0 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/screens/__init__.py
--rw-rw-rw-   0        0        0     5249 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/screens/download_manager.py
--rw-rw-rw-   0        0        0     2935 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/screens/language_options.py
--rw-rw-rw-   0        0        0    15195 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/screens/search_options.py
--rw-rw-rw-   0        0        0    12814 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/screens/subsearch_options.py
--rw-rw-rw-   0        0        0     1062 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/gui/system_tray.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.157012 Subsearch-2.43.1/src/subsearch/providers/
--rw-rw-rw-   0        0        0        2 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/providers/__init__.py
--rw-rw-rw-   0        0        0     5927 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/providers/common_utils.py
--rw-rw-rw-   0        0        0     3187 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/providers/opensubtitles.py
--rw-rw-rw-   0        0        0     3330 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/providers/subscene.py
--rw-rw-rw-   0        0        0     2459 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/providers/yifysubtitles.py
-drwxrwxrwx   0        0        0        0 2024-01-27 16:49:34.157012 Subsearch-2.43.1/src/subsearch/utils/
--rw-rw-rw-   0        0        0        2 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/utils/__init__.py
--rw-rw-rw-   0        0        0     1797 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/utils/imdb_lookup.py
--rw-rw-rw-   0        0        0     4803 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/utils/io_app.py
--rw-rw-rw-   0        0        0     5350 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/utils/io_file_system.py
--rw-rw-rw-   0        0        0     5967 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/utils/io_log.py
--rw-rw-rw-   0        0        0     3519 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/utils/io_toml.py
--rw-rw-rw-   0        0        0     4389 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/utils/io_winreg.py
--rw-rw-rw-   0        0        0     8410 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/utils/string_parser.py
--rw-rw-rw-   0        0        0     1987 2024-01-27 16:48:50.000000 Subsearch-2.43.1/src/subsearch/utils/update.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.430230 Subsearch-2.44.0/
+-rw-rw-rw-   0        0        0     1093 2024-01-28 20:46:13.000000 Subsearch-2.44.0/LICENSE
+-rw-rw-rw-   0        0        0      121 2024-01-28 20:46:13.000000 Subsearch-2.44.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7765 2024-01-28 20:46:55.430230 Subsearch-2.44.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5961 2024-01-28 20:46:13.000000 Subsearch-2.44.0/README.md
+-rw-rw-rw-   0        0        0     2609 2024-01-28 20:46:13.000000 Subsearch-2.44.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-01-28 20:46:55.430230 Subsearch-2.44.0/setup.cfg
+-rw-rw-rw-   0        0        0      114 2024-01-28 20:46:13.000000 Subsearch-2.44.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.398980 Subsearch-2.44.0/src/
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.430230 Subsearch-2.44.0/src/Subsearch.egg-info/
+-rw-rw-rw-   0        0        0     7765 2024-01-28 20:46:55.000000 Subsearch-2.44.0/src/Subsearch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2079 2024-01-28 20:46:55.000000 Subsearch-2.44.0/src/Subsearch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-28 20:46:55.000000 Subsearch-2.44.0/src/Subsearch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-01-28 20:46:55.000000 Subsearch-2.44.0/src/Subsearch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-01-28 20:46:55.000000 Subsearch-2.44.0/src/Subsearch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      379 2024-01-28 20:46:55.000000 Subsearch-2.44.0/src/Subsearch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-01-28 20:46:55.000000 Subsearch-2.44.0/src/Subsearch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.414600 Subsearch-2.44.0/src/subsearch/
+-rw-rw-rw-   0        0        0     1498 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/__init__.py
+-rw-rw-rw-   0        0        0       38 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/__main__.py
+-rw-rw-rw-   0        0        0     9400 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/core.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.414600 Subsearch-2.44.0/src/subsearch/data/
+-rw-rw-rw-   0        0        0       99 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/data/__init__.py
+-rw-rw-rw-   0        0        0       53 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/data/guid.py
+-rw-rw-rw-   0        0        0     7704 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/data/language_data.toml
+-rw-rw-rw-   0        0        0       24 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/data/version.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.414600 Subsearch-2.44.0/src/subsearch/globals/
+-rw-rw-rw-   0        0        0        0 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/globals/__init__.py
+-rw-rw-rw-   0        0        0      513 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/globals/constants.py
+-rw-rw-rw-   0        0        0     2505 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/globals/dataclasses.py
+-rw-rw-rw-   0        0        0     5622 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/globals/decorators.py
+-rw-rw-rw-   0        0        0      980 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/globals/exceptions.py
+-rw-rw-rw-   0        0        0      258 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/globals/metaclasses.py
+-rw-rw-rw-   0        0        0     1597 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/globals/propagating_thread.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.414600 Subsearch-2.44.0/src/subsearch/gui/
+-rw-rw-rw-   0        0        0      588 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/__init__.py
+-rw-rw-rw-   0        0        0     3180 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/common_utils.py
+-rw-rw-rw-   0        0        0     1053 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resource_loader.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.414600 Subsearch-2.44.0/src/subsearch/gui/resources/
+-rw-rw-rw-   0        0        0        0 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.414600 Subsearch-2.44.0/src/subsearch/gui/resources/assets/
+-rw-rw-rw-   0        0        0        0 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resources/assets/__init__.py
+-rw-rw-rw-   0        0        0     7119 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resources/assets/spritesheet.png
+-rw-rw-rw-   0        0        0   105808 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resources/assets/subsearch.ico
+-rw-rw-rw-   0        0        0     1674 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resources/config.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.414600 Subsearch-2.44.0/src/subsearch/gui/resources/styles/
+-rw-rw-rw-   0        0        0        0 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resources/styles/__init__.py
+-rw-rw-rw-   0        0        0     1780 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resources/styles/sprites.tcl
+-rw-rw-rw-   0        0        0     7247 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resources/styles/style_subsearch.tcl
+-rw-rw-rw-   0        0        0     1451 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/resources/styles/theme_setter.tcl
+-rw-rw-rw-   0        0        0     6957 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/screen_manager.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.430230 Subsearch-2.44.0/src/subsearch/gui/screens/
+-rw-rw-rw-   0        0        0        0 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/screens/__init__.py
+-rw-rw-rw-   0        0        0     5703 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/screens/download_manager.py
+-rw-rw-rw-   0        0        0     2935 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/screens/language_options.py
+-rw-rw-rw-   0        0        0    15203 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/screens/search_options.py
+-rw-rw-rw-   0        0        0    13523 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/screens/subsearch_options.py
+-rw-rw-rw-   0        0        0     1270 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/gui/system_tray.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.430230 Subsearch-2.44.0/src/subsearch/providers/
+-rw-rw-rw-   0        0        0        2 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/providers/__init__.py
+-rw-rw-rw-   0        0        0     5927 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/providers/common_utils.py
+-rw-rw-rw-   0        0        0     3187 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/providers/opensubtitles.py
+-rw-rw-rw-   0        0        0     3330 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/providers/subscene.py
+-rw-rw-rw-   0        0        0     2459 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/providers/yifysubtitles.py
+drwxrwxrwx   0        0        0        0 2024-01-28 20:46:55.430230 Subsearch-2.44.0/src/subsearch/utils/
+-rw-rw-rw-   0        0        0        2 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/utils/__init__.py
+-rw-rw-rw-   0        0        0     1797 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/utils/imdb_lookup.py
+-rw-rw-rw-   0        0        0     4803 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/utils/io_app.py
+-rw-rw-rw-   0        0        0     6415 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/utils/io_file_system.py
+-rw-rw-rw-   0        0        0     5967 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/utils/io_log.py
+-rw-rw-rw-   0        0        0     4151 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/utils/io_toml.py
+-rw-rw-rw-   0        0        0     4397 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/utils/io_winreg.py
+-rw-rw-rw-   0        0        0     8426 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/utils/string_parser.py
+-rw-rw-rw-   0        0        0     2898 2024-01-28 20:46:13.000000 Subsearch-2.44.0/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.43.1/LICENSE` & `Subsearch-2.44.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/PKG-INFO` & `Subsearch-2.44.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.43.1
+Version: 2.44.0
 Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subtitles,sub,srt,tool,tools,download,movies,shows,scrape,opensubtitles,subscene,subsearch,subtitles,yifysubtitles
 Platform: win32
```

### Comparing `Subsearch-2.43.1/README.md` & `Subsearch-2.44.0/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/pyproject.toml` & `Subsearch-2.44.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.44.0/src/Subsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.43.1
+Version: 2.44.0
 Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subtitles,sub,srt,tool,tools,download,movies,shows,scrape,opensubtitles,subscene,subsearch,subtitles,yifysubtitles
 Platform: win32
```

### Comparing `Subsearch-2.43.1/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.44.0/src/Subsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/__init__.py` & `Subsearch-2.44.0/src/subsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/core.py` & `Subsearch-2.44.0/src/subsearch/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import ctypes
-import secrets
 import time
 from pathlib import Path
 from subsearch.globals import propagating_thread
 from subsearch.globals.constants import APP_PATHS, DEVICE_INFO, FILE_PATHS, VIDEO_FILE, VERSION
 from subsearch.globals.dataclasses import Subtitle
 from subsearch.globals import decorators
 from subsearch.gui import screen_manager, system_tray
@@ -15,14 +14,15 @@
     io_toml,
     string_parser,
 )
 
 
 class Initializer:
     def __init__(self, pref_counter: float) -> None:
+        io_log.log.brackets("Initializing")
         io_log.log.stdout(f"Loading components...", level="info", end_new_line=True)
         self.file_exist = True if VIDEO_FILE else False
         self.setup_file_system()
         self.start = pref_counter
 
         self.app_config = io_toml.get_app_config(FILE_PATHS.config)
         io_log.log.dataclass(DEVICE_INFO, level="debug", print_allowed=False)
@@ -51,19 +51,22 @@
             io_log.log.dataclass(self.provider_urls, level="debug", print_allowed=False)
             self.search_kwargs = dict(
                 release_data=self.release_data,
                 app_config=self.app_config,
                 provider_urls=self.provider_urls,
                 language_data=self.language_data,
             )
+        io_log.log.task_completed()
 
     def setup_file_system(self) -> None:
+        io_log.log.stdout("Verifing files and paths", level="debug")
         io_file_system.create_directory(APP_PATHS.tmp_dir)
         io_file_system.create_directory(APP_PATHS.appdata_subsearch)
         io_toml.resolve_on_integrity_failure()
+        io_file_system.del_directory_content(APP_PATHS.tmp_dir)
         if self.file_exist:
             io_file_system.create_directory(VIDEO_FILE.subs_dir)
             io_file_system.create_directory(VIDEO_FILE.tmp_dir)
 
     def all_providers_disabled(self) -> bool:
         if (
             self.app_config.providers["subscene_site"] is False
@@ -76,15 +79,17 @@
 
 
 class SubsearchCore(Initializer):
     def __init__(self, pref_counter: float) -> None:
         Initializer.__init__(self, pref_counter)
         ctypes.windll.kernel32.SetConsoleTitleW(f"subsearch - {DEVICE_INFO.subsearch}")
         if not self.file_exist:
+            io_log.log.brackets("GUI")
             screen_manager.open_screen("search_options")
+            io_log.log.stdout("Exiting GUI", level="debug")
             return None
 
         if " " in VIDEO_FILE.filename:
             io_log.log.stdout(f"{VIDEO_FILE.filename} contains spaces, result may vary", level="warning")
 
         if not self.all_providers_disabled():
             io_log.log.brackets("Search started")
@@ -118,24 +123,22 @@
     @decorators.call_func
     def download_files(self) -> None:
         io_log.log.brackets(f"Downloading subtitles")
         index_size = len(self.accepted_subtitles)
         for enum, subtitle in enumerate(self.accepted_subtitles, 1):
             io_file_system.download_subtitle(subtitle, enum, index_size)
             self.downloaded_subtitles += 1
-        self.subtitles_found = index_size
         io_log.log.task_completed()
 
     @decorators.call_func
     def download_manager(self) -> None:
         io_log.log.brackets(f"Download Manager")
         subtitles = self.rejected_subtitles + self.accepted_subtitles
         screen_manager.open_screen("download_manager", subtitles=subtitles)
         self.manually_accepted_subtitles.extend(download_manager.DownloadManager.downloaded_subtitle)
-        self.subtitles_found += len(self.manually_accepted_subtitles)
         io_log.log.task_completed()
 
     @decorators.call_func
     def extract_files(self) -> None:
         io_log.log.brackets("Extracting downloads")
         io_file_system.extract_files_in_dir(VIDEO_FILE.tmp_dir, VIDEO_FILE.subs_dir)
         io_log.log.task_completed()
@@ -190,18 +193,19 @@
         io_file_system.del_directory_content(APP_PATHS.tmp_dir)
         io_file_system.del_directory(VIDEO_FILE.tmp_dir)
         if io_file_system.directory_is_empty(VIDEO_FILE.subs_dir):
             io_file_system.del_directory(VIDEO_FILE.subs_dir)
         io_log.log.task_completed()
 
     def core_on_exit(self) -> None:
+        io_log.log.brackets("Exit")
         elapsed = time.perf_counter() - self.start
         self.summary_notification(elapsed)
-        io_log.log.stdout(f"Finished in {elapsed} seconds", hex_color="#f2cdcd")
         self.system_tray.stop()
+        io_log.log.stdout(f"Finished in {elapsed} seconds", hex_color="#f2cdcd")
         if not self.app_config.show_terminal:
             return None
         if DEVICE_INFO.mode == "executable":
             return None
 
         try:
             input("Enter to exit")
```

### Comparing `Subsearch-2.43.1/src/subsearch/data/language_data.toml` & `Subsearch-2.44.0/src/subsearch/data/language_data.toml`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/globals/constants.py` & `Subsearch-2.44.0/src/subsearch/globals/constants.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/globals/dataclasses.py` & `Subsearch-2.44.0/src/subsearch/globals/dataclasses.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/globals/decorators.py` & `Subsearch-2.44.0/src/subsearch/globals/decorators.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/globals/exceptions.py` & `Subsearch-2.44.0/src/subsearch/globals/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/globals/propagating_thread.py` & `Subsearch-2.44.0/src/subsearch/globals/propagating_thread.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/__init__.py` & `Subsearch-2.44.0/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/common_utils.py` & `Subsearch-2.44.0/src/subsearch/gui/common_utils.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/resource_loader.py` & `Subsearch-2.44.0/src/subsearch/gui/resource_loader.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/resources/assets/spritesheet.png` & `Subsearch-2.44.0/src/subsearch/gui/resources/assets/spritesheet.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/resources/assets/subsearch.ico` & `Subsearch-2.44.0/src/subsearch/gui/resources/assets/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/resources/config.py` & `Subsearch-2.44.0/src/subsearch/gui/resources/config.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/resources/styles/sprites.tcl` & `Subsearch-2.44.0/src/subsearch/gui/resources/styles/sprites.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/resources/styles/style_subsearch.tcl` & `Subsearch-2.44.0/src/subsearch/gui/resources/styles/style_subsearch.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/resources/styles/theme_setter.tcl` & `Subsearch-2.44.0/src/subsearch/gui/resources/styles/theme_setter.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/screen_manager.py` & `Subsearch-2.44.0/src/subsearch/gui/screen_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from subsearch.gui.resources import config as cfg
 from subsearch.gui.screens import (
     download_manager,
     language_options,
     search_options,
     subsearch_options,
 )
+from subsearch.utils import io_log
 
 
 class ScreenManager(tk.Frame):
     def __init__(self, parent, available_screens: dict[str, Any], active_screen: str) -> None:
         tk.Frame.__init__(self, parent)
         self.configure(bg=cfg.color.default_bg_dark, width=cfg.size.width, height=82)
         relx_value = 0.0
@@ -135,13 +136,14 @@
         "language_options": LanguageOptions(root),
         "search_options": SearchOptions(root),
         "subsearch_options": SubsearchOptions(root),
         "download_manager": DownloadManager(root, **kwargs),
     }
     manager = ScreenManager(root, screens, tab_name.lower())
     manager.place(y=cfg.size.height - 82)
+    io_log.log.stdout("GUI is running", level="debug")
     root.mainloop()
 
 
 def close_mainloop(event):
     if event.keysym == "Escape":
         root.quit()
```

### Comparing `Subsearch-2.43.1/src/subsearch/gui/screens/download_manager.py` & `Subsearch-2.44.0/src/subsearch/gui/screens/download_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,25 @@
             yscrollcommand=self.scrollbar.set,
         )
         self.sub_listbox.pack(expand=True, fill="both")
         if self.subtitles is not None:
             self.fill_listbox()
         self.scrollbar.pack(expand=True, fill="y")
         self.scrollbar.config(command=self.sub_listbox.yview)
+        if not self.subtitles:
+            self.nothing_label = tk.Label(
+                self,
+                text="It's very empty...\n\n:(",
+                font=cfg.font.cas20b,
+                fg=cfg.color.default_fg,
+                bg=cfg.color.default_bg,
+                anchor="center",
+                justify="center"
+            )
+            self.nothing_label.place(x=cfg.size.height //2, y=cfg.size.width//4, anchor="center")
 
     def fill_listbox(self) -> None:
         accept_threshold = io_toml.load_toml_value(FILE_PATHS.config, "subtitle_filters.accept_threshold")
         no_automatic_downloads = io_toml.load_toml_value(FILE_PATHS.config, "download_manager.no_automatic_downloads")
         self.listbox_index: dict[int, Subtitle] = {}
         for enum, subtitle in enumerate(self.subtitles):
             self.sub_listbox.insert(tk.END, f"{subtitle.pct_result}% {subtitle.release_name}\n")
```

### Comparing `Subsearch-2.43.1/src/subsearch/gui/screens/language_options.py` & `Subsearch-2.44.0/src/subsearch/gui/screens/language_options.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/gui/screens/search_options.py` & `Subsearch-2.44.0/src/subsearch/gui/screens/search_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tkinter as tk
 from tkinter import ttk
 
 from subsearch.globals.constants import FILE_PATHS
 from subsearch.gui import common_utils
 from subsearch.gui.resources import config as cfg
-from subsearch.utils import io_toml, string_parser
+from subsearch.utils import io_log, io_toml, string_parser
 
 
 class Providers(ttk.Labelframe):
     def __init__(self, parent) -> None:
         ttk.Labelframe.__init__(self, parent)
         self.configure(text="Subtitle providers", padding=10)
         self.data = io_toml.load_toml_data(FILE_PATHS.config)
```

### Comparing `Subsearch-2.43.1/src/subsearch/gui/screens/subsearch_options.py` & `Subsearch-2.44.0/src/subsearch/gui/screens/subsearch_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -256,17 +256,24 @@
             width=20,
         )
         self.btn_visit_release_page = ttk.Button(
             frame_right,
             text="Open in webbrowser",
             width=20,
         )
+        self.btn_update_install = ttk.Button(
+            frame_right,
+            text="Download & Update",
+            width=20,
+        )
         self.btn_search.pack(padx=2, pady=2)
         self.btn_visit_release_page.pack(padx=2, pady=2)
         self.btn_visit_release_page.state(["disabled"])
+        self.btn_update_install.pack(padx=2, pady=2)
+        self.btn_update_install.state(["disabled"])
         self.btn_search.bind("<Enter>", self.enter_button)
 
         self.pack(anchor="center", fill="x")
         width = self.winfo_reqwidth()
         half_width = round(width // 2)
         frame_left.pack(side=tk.LEFT, anchor="n", expand=True, fill="x", ipadx=half_width)
         frame_right.pack(side=tk.LEFT, anchor="n", expand=True, fill="x", ipadx=half_width)
@@ -280,20 +287,29 @@
         new_repo_avail, repo_is_prerelease = update.is_new_version_avail()
         latest_version = update.get_latest_version()
         if new_repo_avail:
             self.var_latest.set(f"Latest version: \t\t{latest_version}")
             self.btn_search.state(["disabled"])
             self.btn_visit_release_page.state(["!disabled"])
             self.btn_visit_release_page.bind("<ButtonRelease-1>", self.visit_repository_button)
+            if DEVICE_INFO.mode == "executable": 
+                self.btn_update_install.state(["!disabled"])
+                self.btn_update_install.bind("<ButtonRelease-1>", self.download_and_update)
+            else:
+                self.btn_update_install["text"]="Only availible with MSI"
             if repo_is_prerelease:
                 self.var_misc.set(f"Pre-release")
                 self.frame_misc.configure(fg=cfg.color.orange)
             else:
                 self.var_misc.set(f"Latest")
                 self.frame_misc.configure(fg=cfg.color.green)
 
         if not new_repo_avail:
             self.var_latest.set(f"Latest version: \t\t{latest_version}")
             self.var_misc.set(f"Latest version already installed")
 
     def visit_repository_button(self, event) -> None:
         webbrowser.open(f"https://github.com/vagabondHustler/subsearch/releases")
+        
+    def download_and_update(self, event) -> None:
+        update.download_and_update()
+        self.btn_visit_release_page.state(["disabled"])
```

### Comparing `Subsearch-2.43.1/src/subsearch/gui/system_tray.py` & `Subsearch-2.44.0/src/subsearch/gui/system_tray.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import pystray
 from PIL import Image
 
 from subsearch.globals.constants import APP_PATHS, VERSION
 from subsearch.globals import decorators
 from subsearch.globals import metaclasses
+from subsearch.utils import io_log
 
 
 class SystemTray(metaclass=metaclasses.Singleton):
     @decorators.system_tray_conditions
     def __init__(self) -> None:
         title = f"Subsearch {VERSION}"
         icon = Image.open(APP_PATHS.gui_assets / "subsearch.ico")
@@ -19,16 +20,18 @@
     @decorators.system_tray_conditions
     def display_toast(self, title: str, msg: str) -> None:
         self.tray.title
         self.tray.notify(msg, title)
 
     @decorators.system_tray_conditions
     def start(self) -> None:
+        io_log.log.stdout("Subsearch was added to the system tray", level="debug")
         self.thread_tray.start()
 
     @decorators.system_tray_conditions
     def stop(self) -> None:
         self.tray.stop()
         self.thread_tray.join()
+        io_log.log.stdout("Subsearch was removed from the system tray", level="debug")
 
     def _run_pystray(self) -> None:
         self.tray.run()
```

### Comparing `Subsearch-2.43.1/src/subsearch/providers/common_utils.py` & `Subsearch-2.44.0/src/subsearch/providers/common_utils.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.44.0/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/providers/subscene.py` & `Subsearch-2.44.0/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.44.0/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.44.0/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/utils/io_app.py` & `Subsearch-2.44.0/src/subsearch/utils/io_app.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/utils/io_file_system.py` & `Subsearch-2.44.0/src/subsearch/utils/io_file_system.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import shutil
 import struct
+import time
 import zipfile
 from io import BufferedReader
 from pathlib import Path
-from typing import Any
+
+import requests
 
 from subsearch.globals.constants import VIDEO_FILE
 from subsearch.globals.dataclasses import Subtitle
 from subsearch.providers.common_utils import get_cloudscraper
 from subsearch.utils import io_log, string_parser
 
 
@@ -86,28 +88,32 @@
 
 def directory_is_empty(directory: Path) -> bool:
     if not any(directory.iterdir()):
         return True
     return False
 
 
-def del_directory_content(directory: Path):
+def del_directory_content(directory: Path) -> None:
     for item in directory.iterdir():
+        if not item.is_file():
+            return None
         io_log.log.file_system_action(action_type="remove", src=item)
         if item.is_file():
             item.unlink()
         if item.is_dir():
             shutil.rmtree(item)
 
 
-def create_directory(path: Path):
+def create_directory(path: Path) -> None:
+    io_log.log.stdout(f"Creating {path}", level="debug")
     path.mkdir(parents=True, exist_ok=True)
 
 
 def get_file_hash(file_path: Path) -> str:
+    io_log.log.stdout("Calculating hash of video file", level="debug")
     if not file_path:
         return ""
 
     hash_algorithm = MPCHashAlgorithm(file_path)
     return hash_algorithm.get_hash()
 
 
@@ -141,7 +147,25 @@
             buffer = file.read(self.byte_size)
             (chunk_value,) = struct.unpack("<q", buffer)
             self.hash_chunk += chunk_value
             self.hash_chunk = self.hash_chunk & 0xFFFFFFFFFFFFFFFF
 
     def get_hash(self) -> str:
         return self.hash
+
+
+def download_response(msi_package_path: Path, response: requests.Response):
+    start_time = time.time()
+    with open(msi_package_path, "wb") as msi_file:
+        total_size = int(response.headers.get("content-length", 0))
+        downloaded_size = 0
+        io_log.log.stdout(f"Download started for {msi_package_path.name}")
+        io_log.log.stdout(f"Downloading 0%")
+        for chunk in response.iter_content(chunk_size=128):
+            msi_file.write(chunk)
+            downloaded_size += len(chunk)
+            progress_percentage = (downloaded_size / total_size) * 100
+            elapsed_time = time.time() - start_time
+            if elapsed_time >= 0.5:
+                io_log.log.stdout(f"Downloading {progress_percentage:.2f}%")
+                start_time = time.time()
+        io_log.log.stdout(f"Download complete.")
```

### Comparing `Subsearch-2.43.1/src/subsearch/utils/io_log.py` & `Subsearch-2.44.0/src/subsearch/utils/io_log.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.43.1/src/subsearch/utils/io_toml.py` & `Subsearch-2.44.0/src/subsearch/utils/io_toml.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 from typing import Any, Union
 
 import toml
 
 from subsearch.globals.constants import DEFAULT_CONFIG, FILE_PATHS
 from subsearch.globals.dataclasses import AppConfig
+from subsearch.utils import io_log
 
 
 def load_toml_data(toml_file_path: Path) -> dict[str, Any]:
     with open(toml_file_path, "r") as f:
         return toml.load(f)
 
 
@@ -36,20 +37,23 @@
     toml_data = load_toml_data(toml_file_path)
     keys = key.split(".")
     functools.reduce(dict.get, keys[:-1], toml_data).pop(keys[-1], None)  # type: ignore
     dump_toml_data(toml_file_path, toml_data)
 
 
 def repair_toml_config(toml_file_path: Path, valid_config_keys: list[str], config_keys: list[str]) -> None:
+    io_log.log.stdout(f"Reparing config", level="debug")
     obsolete_keys = [key for key in config_keys if key not in valid_config_keys]
     for key in obsolete_keys:
+        io_log.log.stdout(f"Removing obsolete key {key}", level="debug")
         del_toml_key(toml_file_path, key)
 
     missing_keys = [key for key in valid_config_keys if key not in config_keys]
     for key in missing_keys:
+        io_log.log.stdout(f"Adding missing key {key}", level="debug")
         keys = key.split(".")
         value = functools.reduce(dict.get, keys, DEFAULT_CONFIG)  # type: ignore
         update_toml_key(FILE_PATHS.config, key, value)
 
 
 def get_keys_recursively(dictionary: dict, prefix="", keys=None) -> list[str]:
     if keys is None:
@@ -70,26 +74,31 @@
     valid_config_keys.sort()
     config_keys.sort()
     return config_keys == valid_config_keys
 
 
 def resolve_on_integrity_failure() -> None:
     if not FILE_PATHS.config.exists():
+        io_log.log.stdout(f"No config.toml exsist, creating default at {FILE_PATHS.config}", level="debug")
         dump_toml_data(FILE_PATHS.config, DEFAULT_CONFIG)
         return None
     valid_config_keys = get_keys_recursively(DEFAULT_CONFIG)
     config_keys = get_keys_recursively(load_toml_data(FILE_PATHS.config))
     valid = valid_config(valid_config_keys, config_keys)
     if valid:
+        io_log.log.stdout(f"Config is valid", level="debug")
         return None
     try:
+        io_log.log.stdout(f"Config not valid", level="debug")
         repair_toml_config(FILE_PATHS.config, valid_config_keys, config_keys)
     except Exception:
+        io_log.log.stdout(f"Repair faild, creating default at {FILE_PATHS.config}", level="debug")
         FILE_PATHS.config.unlink()
         dump_toml_data(FILE_PATHS.config, DEFAULT_CONFIG)
+    io_log.log.stdout(f"Repair succeeded", level="debug")
 
 
 def get_app_config(toml_file_path: Path) -> AppConfig:
     data = load_toml_data(toml_file_path)
     user_data = AppConfig(
         **data["subtitle_filters"],
         **data["gui"],
```

### Comparing `Subsearch-2.43.1/src/subsearch/utils/io_winreg.py` & `Subsearch-2.44.0/src/subsearch/utils/io_winreg.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from subsearch.globals.constants import (
     APP_PATHS,
     COMPUTER_NAME,
     DEVICE_INFO,
     FILE_PATHS,
     REGISTRY_PATHS,
 )
-from subsearch.utils import io_toml
+from subsearch.utils import io_log, io_toml
 
 
 class LaunchOptions:
     def __init__(self) -> None:
         self.show_terminal = io_toml.load_toml_value(FILE_PATHS.config, "gui.show_terminal")
         self.python_path = Path(sys.executable).parent
         self.console_title = "import ctypes; ctypes.windll.kernel32.SetConsoleTitleW('subsearch');"
```

### Comparing `Subsearch-2.43.1/src/subsearch/utils/string_parser.py` & `Subsearch-2.44.0/src/subsearch/utils/string_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from subsearch.globals.constants import VIDEO_FILE
 from subsearch.globals.dataclasses import (
     AppConfig,
     LanguageData,
     ProviderUrls,
     ReleaseData,
 )
-from subsearch.utils import imdb_lookup
+from subsearch.utils import imdb_lookup, io_log
 
 
 def find_year(string: str) -> int:
     re_year = re.findall(r"^.*\.([1-2][0-9]{3})\.", string)
     if re_year:
         year = re_year[0]
         return int(year)
@@ -71,15 +71,15 @@
         title = find_title_by_show(filename)
     else:
         title = filename.rsplit("-", 1)[0]
     return title
 
 
 class CreateProviderUrls:
-    def __init__(self, app_config: AppConfig, release_data: ReleaseData, language_data: dict[str, Any]):
+    def __init__(self, app_config: AppConfig, release_data: ReleaseData, language_data: dict[str, Any]) -> None:
         self.app_config = app_config
         self.release_data = release_data
         self.language_data = language_data
         self.current_language_data: LanguageData = LanguageData(**language_data[app_config.language])
 
     def retrieve_urls(self) -> ProviderUrls:
         return ProviderUrls(self.subscene(), self.opensubtitles(), self.opensubtitles_hash(), self.yifysubtitles())
```


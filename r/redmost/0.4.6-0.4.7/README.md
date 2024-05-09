# Comparing `tmp/redmost-0.4.6.tar.gz` & `tmp/redmost-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redmost-0.4.6.tar", last modified: Wed Apr 10 14:35:14 2024, max compression
+gzip compressed data, was "redmost-0.4.7.tar", last modified: Thu May  9 07:26:07 2024, max compression
```

## Comparing `redmost-0.4.6.tar` & `redmost-0.4.7.tar`

### file list

```diff
@@ -1,135 +1,162 @@
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.520009 redmost-0.4.6/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.503342 redmost-0.4.6/.github/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.506675 redmost-0.4.6/.github/workflows/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1124 2024-03-20 13:43:32.000000 redmost-0.4.6/.github/workflows/pre-release.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1051 2024-03-20 13:43:36.000000 redmost-0.4.6/.github/workflows/tagged-release.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1228 2024-03-20 13:43:41.000000 redmost-0.4.6/.github/workflows/test_linux_lint.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1462 2024-03-19 19:35:03.000000 redmost-0.4.6/.github/workflows/test_linux_pyqt5.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1525 2024-03-19 09:56:49.000000 redmost-0.4.6/.github/workflows/test_linux_pyqt6.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1468 2024-03-19 09:57:41.000000 redmost-0.4.6/.github/workflows/test_linux_pyside6.yml
--rw-r--r--   0 daddona   (1000) daddona   (1000)      652 2024-03-18 13:57:53.000000 redmost-0.4.6/.readthedocs.yaml
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1535 2024-03-11 07:22:12.000000 redmost-0.4.6/LICENSE
--rw-r--r--   0 daddona   (1000) daddona   (1000)     6878 2024-04-10 14:35:14.520009 redmost-0.4.6/PKG-INFO
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3890 2024-03-20 10:51:05.000000 redmost-0.4.6/README.md
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.506675 redmost-0.4.6/docs/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.503342 redmost-0.4.6/docs/_static/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.506675 redmost-0.4.6/docs/_static/css/
--rw-r--r--   0 daddona   (1000) daddona   (1000)       60 2023-09-21 08:50:12.000000 redmost-0.4.6/docs/_static/css/custom.css
--rw-r--r--   0 daddona   (1000) daddona   (1000)     2905 2024-03-18 14:10:16.000000 redmost-0.4.6/docs/conf.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      192 2024-03-19 12:03:17.000000 redmost-0.4.6/docs/docs.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)     2860 2024-03-20 10:51:01.000000 redmost-0.4.6/docs/index.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)     2663 2024-04-03 07:55:12.000000 redmost-0.4.6/docs/installation.rst
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.510009 redmost-0.4.6/docs/module_docs/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      113 2024-03-18 13:06:03.000000 redmost-0.4.6/docs/module_docs/backends_rrock.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       80 2024-03-18 12:38:22.000000 redmost-0.4.6/docs/module_docs/gui.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       86 2024-03-18 13:46:27.000000 redmost-0.4.6/docs/module_docs/lines.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       92 2024-03-18 13:35:21.000000 redmost-0.4.6/docs/module_docs/loaders.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       98 2024-03-19 12:02:51.000000 redmost-0.4.6/docs/module_docs/qt_compat.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       86 2024-03-18 12:59:15.000000 redmost-0.4.6/docs/module_docs/utils.rst
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.510009 redmost-0.4.6/docs/pics/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     6393 2022-12-01 11:40:24.000000 redmost-0.4.6/docs/pics/github-mark.png
--rw-r--r--   0 daddona   (1000) daddona   (1000)    75781 2024-03-18 10:56:41.000000 redmost-0.4.6/docs/pics/redmost.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      105 2024-03-18 13:56:27.000000 redmost-0.4.6/docs/requirements.txt
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.510009 redmost-0.4.6/docs/tutorials/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      116 2024-03-18 13:51:24.000000 redmost-0.4.6/docs/tutorials/tut_01.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)       63 2024-03-18 12:54:00.000000 redmost-0.4.6/docs/tutorials.rst
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1644 2024-03-20 10:48:33.000000 redmost-0.4.6/pyproject.toml
--rw-r--r--   0 daddona   (1000) daddona   (1000)       38 2024-04-10 14:35:14.520009 redmost-0.4.6/setup.cfg
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.503342 redmost-0.4.6/src/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.510009 redmost-0.4.6/src/redmost/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     2873 2024-03-20 13:21:47.000000 redmost-0.4.6/src/redmost/__init__.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)      411 2024-04-10 14:35:14.000000 redmost-0.4.6/src/redmost/_version.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.510009 redmost-0.4.6/src/redmost/backends/
--rw-r--r--   0 daddona   (1000) daddona   (1000)       72 2024-03-14 12:08:37.000000 redmost-0.4.6/src/redmost/backends/__init__.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     7860 2024-03-18 13:50:35.000000 redmost-0.4.6/src/redmost/backends/rrock.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)   118352 2024-04-10 06:13:02.000000 redmost-0.4.6/src/redmost/gui.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)    10928 2024-03-21 09:37:05.000000 redmost-0.4.6/src/redmost/lines.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)     7041 2024-04-10 14:33:59.000000 redmost-0.4.6/src/redmost/loaders.py
--rw-r--r--   0 daddona   (1000) daddona   (1000)        2 2024-03-14 08:09:46.000000 redmost-0.4.6/src/redmost/py.typed
--rw-r--r--   0 daddona   (1000) daddona   (1000)     9322 2024-03-20 13:39:09.000000 redmost-0.4.6/src/redmost/qt_compat.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.510009 redmost-0.4.6/src/redmost/ui/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     5479 2024-03-21 11:12:13.000000 redmost-0.4.6/src/redmost/ui/control_mapping_dialog.ui
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.503342 redmost-0.4.6/src/redmost/ui/icons/
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.513342 redmost-0.4.6/src/redmost/ui/icons/feather/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      343 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/book.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      358 2024-03-20 10:22:19.000000 redmost-0.4.6/src/redmost/ui/icons/feather/camera.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/check-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      320 2024-03-20 10:22:19.000000 redmost-0.4.6/src/redmost/ui/icons/feather/chevrons-left.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      320 2024-03-20 10:22:19.000000 redmost-0.4.6/src/redmost/ui/icons/feather/chevrons-right.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      371 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/delete.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      384 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/file-minus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      428 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/file-plus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      334 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/file.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      308 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/folder.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      344 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/info.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      369 2024-03-20 10:22:19.000000 redmost-0.4.6/src/redmost/ui/icons/feather/log-out.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      333 2024-03-20 10:22:19.000000 redmost-0.4.6/src/redmost/ui/icons/feather/maximize.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      327 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/minus-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      265 2024-03-20 10:22:19.000000 redmost-0.4.6/src/redmost/ui/icons/feather/play.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      370 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/plus-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      301 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/plus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      389 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/save.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      484 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/save_as.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1008 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/settings.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      361 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/share.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      608 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/sliders.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      337 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/table.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      403 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/x-octagon.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      394 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/zoom-in.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      351 2024-03-20 10:20:06.000000 redmost-0.4.6/src/redmost/ui/icons/feather/zoom-out.svg
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.513342 redmost-0.4.6/src/redmost/ui/icons/feather-dark/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/book.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      353 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/camera.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/check-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      315 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/chevrons-left.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      315 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/chevrons-right.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      371 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/delete.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      384 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/file-minus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      428 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/file-plus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      334 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/file.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      308 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/folder.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      344 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/info.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      364 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/log-out.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      328 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/maximize.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      327 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/minus-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      260 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/play.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      370 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/plus-square.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      301 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/plus.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      389 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/save.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1712 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/save_as.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1008 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/settings.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      361 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/share.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      608 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/sliders.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      337 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/table.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      403 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/x-octagon.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      394 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/zoom-in.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)      351 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/zoom-out.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1304 2024-03-20 20:08:34.000000 redmost-0.4.6/src/redmost/ui/icons/feather-dark/zoom.svg
--rw-r--r--   0 daddona   (1000) daddona   (1000)    44979 2024-03-21 09:40:40.000000 redmost-0.4.6/src/redmost/ui/main_window.ui
--rw-r--r--   0 daddona   (1000) daddona   (1000)    37667 2024-03-18 10:57:10.000000 redmost-0.4.6/src/redmost/ui/redmost.png
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3777 2024-03-20 20:53:24.000000 redmost-0.4.6/src/redmost/ui/settings_dialog.ui
--rw-r--r--   0 daddona   (1000) daddona   (1000)     4859 2024-03-20 09:06:53.000000 redmost-0.4.6/src/redmost/utils.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.520009 redmost-0.4.6/src/redmost.egg-info/
--rw-r--r--   0 daddona   (1000) daddona   (1000)     6878 2024-04-10 14:35:14.000000 redmost-0.4.6/src/redmost.egg-info/PKG-INFO
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3939 2024-04-10 14:35:14.000000 redmost-0.4.6/src/redmost.egg-info/SOURCES.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)        1 2024-04-10 14:35:14.000000 redmost-0.4.6/src/redmost.egg-info/dependency_links.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)       45 2024-04-10 14:35:14.000000 redmost-0.4.6/src/redmost.egg-info/entry_points.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)      155 2024-04-10 14:35:14.000000 redmost-0.4.6/src/redmost.egg-info/requires.txt
--rw-r--r--   0 daddona   (1000) daddona   (1000)        8 2024-04-10 14:35:14.000000 redmost-0.4.6/src/redmost.egg-info/top_level.txt
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.513342 redmost-0.4.6/test/
--rw-r--r--   0 daddona   (1000) daddona   (1000)      386 2024-03-18 14:30:36.000000 redmost-0.4.6/test/__init__.py
-drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-04-10 14:35:14.520009 redmost-0.4.6/test/data/
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:15.000000 redmost-0.4.6/test/data/spec_95.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.6/test/data/spec_955.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.6/test/data/spec_963.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.6/test/data/spec_965.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.6/test/data/spec_966.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.6/test/data/spec_971.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.6/test/data/spec_988.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.6/test/data/spec_991.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.6/test/data/spec_994.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.6/test/data/spec_997.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)     1845 2024-03-19 14:41:10.000000 redmost-0.4.6/test/data/test_project_1.json
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3549 2024-03-18 14:22:13.000000 redmost-0.4.6/test/data/test_project_2.json
--rw-r--r--   0 daddona   (1000) daddona   (1000)     8640 2024-03-18 14:28:57.000000 redmost-0.4.6/test/data/test_zcat.fits
--rw-r--r--   0 daddona   (1000) daddona   (1000)     3737 2024-03-20 21:34:44.000000 redmost-0.4.6/test/test_pyqt_basic.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.370000 redmost-0.4.7/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.343334 redmost-0.4.7/.github/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.346667 redmost-0.4.7/.github/workflows/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1124 2024-03-20 13:43:32.000000 redmost-0.4.7/.github/workflows/pre-release.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1051 2024-03-20 13:43:36.000000 redmost-0.4.7/.github/workflows/tagged-release.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1228 2024-03-20 13:43:41.000000 redmost-0.4.7/.github/workflows/test_linux_lint.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1462 2024-03-19 19:35:03.000000 redmost-0.4.7/.github/workflows/test_linux_pyqt5.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1525 2024-03-19 09:56:49.000000 redmost-0.4.7/.github/workflows/test_linux_pyqt6.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1468 2024-03-19 09:57:41.000000 redmost-0.4.7/.github/workflows/test_linux_pyside6.yml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      652 2024-03-18 13:57:53.000000 redmost-0.4.7/.readthedocs.yaml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1535 2024-03-11 07:22:12.000000 redmost-0.4.7/LICENSE
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     6995 2024-05-09 07:26:07.370000 redmost-0.4.7/PKG-INFO
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4007 2024-05-03 06:21:44.000000 redmost-0.4.7/README.md
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.346667 redmost-0.4.7/docs/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.346667 redmost-0.4.7/docs/_static/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.346667 redmost-0.4.7/docs/_static/css/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       60 2023-09-21 08:50:12.000000 redmost-0.4.7/docs/_static/css/custom.css
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     2919 2024-04-26 09:16:05.000000 redmost-0.4.7/docs/conf.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      192 2024-03-19 12:03:17.000000 redmost-0.4.7/docs/docs.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     2860 2024-03-20 10:51:01.000000 redmost-0.4.7/docs/index.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     2689 2024-04-26 10:00:48.000000 redmost-0.4.7/docs/installation.rst
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.350000 redmost-0.4.7/docs/module_docs/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      113 2024-03-18 13:06:03.000000 redmost-0.4.7/docs/module_docs/backends_rrock.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       80 2024-03-18 12:38:22.000000 redmost-0.4.7/docs/module_docs/gui.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       86 2024-03-18 13:46:27.000000 redmost-0.4.7/docs/module_docs/lines.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       92 2024-03-18 13:35:21.000000 redmost-0.4.7/docs/module_docs/loaders.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       98 2024-03-19 12:02:51.000000 redmost-0.4.7/docs/module_docs/qt_compat.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       86 2024-03-18 12:59:15.000000 redmost-0.4.7/docs/module_docs/utils.rst
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.360000 redmost-0.4.7/docs/pics/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51233 2024-04-26 08:24:08.000000 redmost-0.4.7/docs/pics/dialog_about.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    34199 2024-04-26 08:23:49.000000 redmost-0.4.7/docs/pics/dialog_controls.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)   110627 2024-04-26 09:40:51.000000 redmost-0.4.7/docs/pics/dialog_load_spectra.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    25219 2024-04-26 08:23:17.000000 redmost-0.4.7/docs/pics/dialog_settings_appearence.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    21966 2024-04-26 08:22:40.000000 redmost-0.4.7/docs/pics/dialog_settings_general.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     6393 2022-12-01 11:40:24.000000 redmost-0.4.7/docs/pics/github-mark.png
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.363334 redmost-0.4.7/docs/pics/icons/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      428 2024-03-20 10:20:06.000000 redmost-0.4.7/docs/pics/icons/file-plus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      308 2024-03-20 10:20:06.000000 redmost-0.4.7/docs/pics/icons/folder.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      333 2024-03-20 10:22:19.000000 redmost-0.4.7/docs/pics/icons/maximize.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      265 2024-03-20 10:22:19.000000 redmost-0.4.7/docs/pics/icons/play.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      389 2024-03-20 10:20:06.000000 redmost-0.4.7/docs/pics/icons/save.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      394 2024-03-20 10:20:06.000000 redmost-0.4.7/docs/pics/icons/zoom-in.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      351 2024-03-20 10:20:06.000000 redmost-0.4.7/docs/pics/icons/zoom-out.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)   203220 2024-04-29 11:04:00.000000 redmost-0.4.7/docs/pics/main_ui_add_line.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)   110167 2024-04-26 08:32:27.000000 redmost-0.4.7/docs/pics/main_ui_annotated.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    98899 2024-04-26 07:54:55.000000 redmost-0.4.7/docs/pics/main_ui_clean.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    28471 2024-04-29 14:16:04.000000 redmost-0.4.7/docs/pics/main_ui_identification.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    17586 2024-04-29 14:29:02.000000 redmost-0.4.7/docs/pics/main_ui_multi_lines.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    17767 2024-04-29 14:46:17.000000 redmost-0.4.7/docs/pics/main_ui_redrock.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)   226669 2024-04-29 11:06:12.000000 redmost-0.4.7/docs/pics/main_ui_select_lines.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)   225969 2024-04-29 07:47:11.000000 redmost-0.4.7/docs/pics/main_ui_spectrum.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    11741 2024-04-26 08:22:04.000000 redmost-0.4.7/docs/pics/menu_about.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     8915 2024-04-26 08:21:33.000000 redmost-0.4.7/docs/pics/menu_edit.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    14630 2024-04-26 08:21:49.000000 redmost-0.4.7/docs/pics/menu_file.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    14531 2024-04-26 08:21:19.000000 redmost-0.4.7/docs/pics/menu_tools.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    75781 2024-03-18 10:56:41.000000 redmost-0.4.7/docs/pics/redmost.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      105 2024-03-18 13:56:27.000000 redmost-0.4.7/docs/requirements.txt
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.363334 redmost-0.4.7/docs/tutorials/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4538 2024-04-29 12:59:43.000000 redmost-0.4.7/docs/tutorials/tut_01_load_spectra.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4173 2024-04-30 05:52:57.000000 redmost-0.4.7/docs/tutorials/tut_02_line_tools.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      125 2024-04-30 05:54:45.000000 redmost-0.4.7/docs/tutorials/tut_03_use_existing_zcat.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      145 2024-04-30 05:54:20.000000 redmost-0.4.7/docs/tutorials.rst
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1644 2024-03-20 10:48:33.000000 redmost-0.4.7/pyproject.toml
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       38 2024-05-09 07:26:07.370000 redmost-0.4.7/setup.cfg
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.346667 redmost-0.4.7/src/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.363334 redmost-0.4.7/src/redmost/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     2873 2024-03-20 13:21:47.000000 redmost-0.4.7/src/redmost/__init__.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      411 2024-05-09 07:26:07.000000 redmost-0.4.7/src/redmost/_version.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.363334 redmost-0.4.7/src/redmost/backends/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       72 2024-03-14 12:08:37.000000 redmost-0.4.7/src/redmost/backends/__init__.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     8173 2024-05-09 07:23:47.000000 redmost-0.4.7/src/redmost/backends/rrock.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)   118352 2024-04-10 06:13:02.000000 redmost-0.4.7/src/redmost/gui.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    10928 2024-03-21 09:37:05.000000 redmost-0.4.7/src/redmost/lines.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     7041 2024-04-10 14:33:59.000000 redmost-0.4.7/src/redmost/loaders.py
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        2 2024-03-14 08:09:46.000000 redmost-0.4.7/src/redmost/py.typed
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     9322 2024-03-20 13:39:09.000000 redmost-0.4.7/src/redmost/qt_compat.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.363334 redmost-0.4.7/src/redmost/ui/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     5479 2024-03-21 11:12:13.000000 redmost-0.4.7/src/redmost/ui/control_mapping_dialog.ui
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.346667 redmost-0.4.7/src/redmost/ui/icons/
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.366667 redmost-0.4.7/src/redmost/ui/icons/feather/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      343 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/book.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      358 2024-03-20 10:22:19.000000 redmost-0.4.7/src/redmost/ui/icons/feather/camera.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/check-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      320 2024-03-20 10:22:19.000000 redmost-0.4.7/src/redmost/ui/icons/feather/chevrons-left.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      320 2024-03-20 10:22:19.000000 redmost-0.4.7/src/redmost/ui/icons/feather/chevrons-right.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      371 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/delete.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      384 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/file-minus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      428 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/file-plus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      334 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/file.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      308 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/folder.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      344 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/info.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      369 2024-03-20 10:22:19.000000 redmost-0.4.7/src/redmost/ui/icons/feather/log-out.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      333 2024-03-20 10:22:19.000000 redmost-0.4.7/src/redmost/ui/icons/feather/maximize.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      327 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/minus-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      265 2024-03-20 10:22:19.000000 redmost-0.4.7/src/redmost/ui/icons/feather/play.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      370 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/plus-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      301 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/plus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      389 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/save.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      484 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/save_as.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1008 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/settings.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      361 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/share.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      608 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/sliders.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      337 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/table.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      403 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/x-octagon.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      394 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/zoom-in.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      351 2024-03-20 10:20:06.000000 redmost-0.4.7/src/redmost/ui/icons/feather/zoom-out.svg
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.366667 redmost-0.4.7/src/redmost/ui/icons/feather-dark/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/book.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      353 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/camera.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      342 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/check-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      315 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/chevrons-left.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      315 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/chevrons-right.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      371 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/delete.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      384 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/file-minus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      428 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/file-plus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      334 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/file.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      308 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/folder.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      344 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/info.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      364 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/log-out.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      328 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/maximize.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      327 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/minus-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      260 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/play.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      370 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/plus-square.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      301 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/plus.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      389 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/save.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1712 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/save_as.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1008 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/settings.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      361 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/share.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      608 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/sliders.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      337 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/table.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      403 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/x-octagon.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      394 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/zoom-in.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      351 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/zoom-out.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1304 2024-03-20 20:08:34.000000 redmost-0.4.7/src/redmost/ui/icons/feather-dark/zoom.svg
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    44979 2024-03-21 09:40:40.000000 redmost-0.4.7/src/redmost/ui/main_window.ui
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    37667 2024-03-18 10:57:10.000000 redmost-0.4.7/src/redmost/ui/redmost.png
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     3777 2024-03-20 20:53:24.000000 redmost-0.4.7/src/redmost/ui/settings_dialog.ui
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4859 2024-03-20 09:06:53.000000 redmost-0.4.7/src/redmost/utils.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.366667 redmost-0.4.7/src/redmost.egg-info/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     6995 2024-05-09 07:26:07.000000 redmost-0.4.7/src/redmost.egg-info/PKG-INFO
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     4752 2024-05-09 07:26:07.000000 redmost-0.4.7/src/redmost.egg-info/SOURCES.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        1 2024-05-09 07:26:07.000000 redmost-0.4.7/src/redmost.egg-info/dependency_links.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)       45 2024-05-09 07:26:07.000000 redmost-0.4.7/src/redmost.egg-info/entry_points.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      155 2024-05-09 07:26:07.000000 redmost-0.4.7/src/redmost.egg-info/requires.txt
+-rw-r--r--   0 daddona   (1000) daddona   (1000)        8 2024-05-09 07:26:07.000000 redmost-0.4.7/src/redmost.egg-info/top_level.txt
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.366667 redmost-0.4.7/test/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)      386 2024-03-18 14:30:36.000000 redmost-0.4.7/test/__init__.py
+drwxr-xr-x   0 daddona   (1000) daddona   (1000)        0 2024-05-09 07:26:07.366667 redmost-0.4.7/test/data/
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:15.000000 redmost-0.4.7/test/data/spec_95.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.7/test/data/spec_955.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.7/test/data/spec_963.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.7/test/data/spec_965.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.7/test/data/spec_966.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.7/test/data/spec_971.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.7/test/data/spec_988.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.7/test/data/spec_991.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.7/test/data/spec_994.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)    51840 2023-09-28 12:37:31.000000 redmost-0.4.7/test/data/spec_997.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     1845 2024-03-19 14:41:10.000000 redmost-0.4.7/test/data/test_project_1.json
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     3549 2024-03-18 14:22:13.000000 redmost-0.4.7/test/data/test_project_2.json
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     8640 2024-03-18 14:28:57.000000 redmost-0.4.7/test/data/test_zcat.fits
+-rw-r--r--   0 daddona   (1000) daddona   (1000)     3737 2024-03-20 21:34:44.000000 redmost-0.4.7/test/test_pyqt_basic.py
```

### Comparing `redmost-0.4.6/.github/workflows/pre-release.yml` & `redmost-0.4.7/.github/workflows/pre-release.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/.github/workflows/tagged-release.yml` & `redmost-0.4.7/.github/workflows/tagged-release.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/.github/workflows/test_linux_lint.yml` & `redmost-0.4.7/.github/workflows/test_linux_lint.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/.github/workflows/test_linux_pyqt5.yml` & `redmost-0.4.7/.github/workflows/test_linux_pyqt5.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/.github/workflows/test_linux_pyqt6.yml` & `redmost-0.4.7/.github/workflows/test_linux_pyqt6.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/.github/workflows/test_linux_pyside6.yml` & `redmost-0.4.7/.github/workflows/test_linux_pyside6.yml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/.readthedocs.yaml` & `redmost-0.4.7/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/LICENSE` & `redmost-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/PKG-INFO` & `redmost-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmost
-Version: 0.4.6
+Version: 0.4.7
 Summary: Display spectra and estimate their redshifts.
 Author: Maurizio D'Addona
 Author-email: mauritiusdadd@gmail.com
 Maintainer: Maurizio D'Addona
 Maintainer-email: mauritiusdadd@gmail.com
 License: BSD 3-Clause License
         
@@ -63,15 +63,17 @@
 Requires-Dist: pytest-qt; extra == "test"
 Requires-Dist: coverage; extra == "test"
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10817885.svg)](https://doi.org/10.5281/zenodo.10817885)
 [![DOCS](https://readthedocs.org/projects/redmost/badge/?version=latest)](https://redmost.readthedocs.io/en/latest/) [![Coverage Status](https://coveralls.io/repos/github/mauritiusdadd/redmost/badge.svg?branch=main)](https://coveralls.io/github/mauritiusdadd/redmost?branch=main) [![Testing PyQt6](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyqt6.yml/badge.svg)](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyqt6.yml) [![Testing PySide6](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyside6.yml/badge.svg)](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyside6.yml)
 # REDMOST 
 
-<b>RED</b>shift <b>M</b>easurement <b>O</b>f <b>S</b>pec<b>T</b>ra is a Qt6 Graphical User Interface (GUI) to do redshift measurements on 1D spectra.
+<b>RED</b>shift <b>M</b>easurements <b>O</b>f <b>S</b>pec<b>T</b>ra is a Qt6 Graphical User Interface (GUI) to do redshift measurements on 1D spectra.
+
+![Redmost main window](https://github.com/mauritiusdadd/redmost/blob/main/docs/pics/main_ui_spectrum.png?raw=true)
 
 If [redrock][1] is correctly installed, it cat be used as a backend to measure the redshift.
 
 # Installation
 
 This is a python program based on Qt6 and supports both PyQt6 and PySide6 backends. It also support PyQt5 backend but it is not fully tested and may not work as expected.
 Since it is a good practice to not mess up the system-wide python environment, you should install this program in a virtual environment. If you don't have a virtual environment yet, you can create one with the command
```

### Comparing `redmost-0.4.6/README.md` & `redmost-0.4.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10817885.svg)](https://doi.org/10.5281/zenodo.10817885)
 [![DOCS](https://readthedocs.org/projects/redmost/badge/?version=latest)](https://redmost.readthedocs.io/en/latest/) [![Coverage Status](https://coveralls.io/repos/github/mauritiusdadd/redmost/badge.svg?branch=main)](https://coveralls.io/github/mauritiusdadd/redmost?branch=main) [![Testing PyQt6](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyqt6.yml/badge.svg)](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyqt6.yml) [![Testing PySide6](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyside6.yml/badge.svg)](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyside6.yml)
 # REDMOST 
 
-<b>RED</b>shift <b>M</b>easurement <b>O</b>f <b>S</b>pec<b>T</b>ra is a Qt6 Graphical User Interface (GUI) to do redshift measurements on 1D spectra.
+<b>RED</b>shift <b>M</b>easurements <b>O</b>f <b>S</b>pec<b>T</b>ra is a Qt6 Graphical User Interface (GUI) to do redshift measurements on 1D spectra.
+
+![Redmost main window](https://github.com/mauritiusdadd/redmost/blob/main/docs/pics/main_ui_spectrum.png?raw=true)
 
 If [redrock][1] is correctly installed, it cat be used as a backend to measure the redshift.
 
 # Installation
 
 This is a python program based on Qt6 and supports both PyQt6 and PySide6 backends. It also support PyQt5 backend but it is not fully tested and may not work as expected.
 Since it is a good practice to not mess up the system-wide python environment, you should install this program in a virtual environment. If you don't have a virtual environment yet, you can create one with the command
```

### Comparing `redmost-0.4.6/docs/conf.py` & `redmost-0.4.7/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = []
 
+numfig = True
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 # html_theme = 'alabaster'
```

### Comparing `redmost-0.4.6/docs/index.rst` & `redmost-0.4.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/docs/installation.rst` & `redmost-0.4.7/docs/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _installation_guide:
+
 .. |github_mark| image:: pics/github-mark.png
    :height: 1em
    :target: github_repo
 
 Installing a Packaged Release
 =============================
 
@@ -75,14 +77,15 @@
 
     pip install .[pyqt5]
 
 
 After the installation, to update redmost use
 
 .. code-block:: bash
+
     git pull
     pip install . --upgrade
 
 Install third party backends
 ============================
 
 Redmost uses modular backends to measure the redshift, although only redrock is currently supported. Please check and follow the installation instructions of the single packages!
```

### Comparing `redmost-0.4.6/docs/pics/github-mark.png` & `redmost-0.4.7/docs/pics/github-mark.png`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/docs/pics/redmost.svg` & `redmost-0.4.7/docs/pics/redmost.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/pyproject.toml` & `redmost-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/__init__.py` & `redmost-0.4.7/src/redmost/__init__.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/backends/rrock.py` & `redmost-0.4.7/src/redmost/backends/rrock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import os
 import uuid
 import pickle
 import argparse
+from packaging import version
 from typing import Tuple, List, Dict, Optional, Any, Callable
 
 import numpy as np
 
 from scipy import sparse  # type: ignore
 
 from astropy.nddata import VarianceUncertainty  # type: ignore
 from astropy.nddata import StdDevUncertainty  # type: ignore
 from astropy.nddata import InverseVariance  # type: ignore
 
 from specutils import Spectrum1D  # type: ignore
 
+RR_GPU_MIN_VER = "0.16.0"
+
 try:
     import redrock
 except (ImportError, ModuleNotFoundError):
     HAS_REDROCK = False
 
     def get_templates(*args, **kwargs):
         raise NotImplementedError()
@@ -187,34 +190,39 @@
         start = elapsed(None, "", comm=None)
 
         dtargets = DistTargetsCopy(targets, comm=None, root=0)
 
         # Get the dictionary of wavelength grids
         dwave = dtargets.wavegrids()
 
+        print(f"Using redrock version {redrock.__version__}")
+
         _ = elapsed(
             start,
             "Distribution of {} targets".format(len(dtargets.all_target_ids)),
             comm=None
         )
 
+        opt_zfind_args = {}
+        opt_load_dist_templates_args = {}
+        use_gpu = False
+        if version.parse(redrock.__version__) >= version.parse(RR_GPU_MIN_VER):
+            print(f"GPU support: {use_gpu}")
+            opt_zfind_args['use_gpu'] = use_gpu
+            opt_load_dist_templates_args['use_gpu'] = use_gpu
+
         # Read the template data
         dtemplates = load_dist_templates(
             dwave,
             templates=None,
             comm=None,
             mp_procs=1,
-            # use_gpu=True,
-            # gpu_mode=True
+            **opt_load_dist_templates_args
         )
 
-        opt_zfind_args = {}
-        # TODO: do more tests before enabling this
-        # opt_zfind_args['use_gpu'] = False
-
         # Compute the redshifts, including both the coarse scan and the
         # refinement.  This function only returns data on the rank 0 process.
         start = elapsed(None, "", comm=None)
         scandata, zfit = zfind(
             dtargets,
             dtemplates,
             mp_procs=1,
```

### Comparing `redmost-0.4.6/src/redmost/gui.py` & `redmost-0.4.7/src/redmost/gui.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/lines.py` & `redmost-0.4.7/src/redmost/lines.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/loaders.py` & `redmost-0.4.7/src/redmost/loaders.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/qt_compat.py` & `redmost-0.4.7/src/redmost/qt_compat.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/control_mapping_dialog.ui` & `redmost-0.4.7/src/redmost/ui/control_mapping_dialog.ui`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/icons/feather/settings.svg` & `redmost-0.4.7/src/redmost/ui/icons/feather/settings.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/icons/feather/sliders.svg` & `redmost-0.4.7/src/redmost/ui/icons/feather/sliders.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/icons/feather-dark/save_as.svg` & `redmost-0.4.7/src/redmost/ui/icons/feather-dark/save_as.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/icons/feather-dark/settings.svg` & `redmost-0.4.7/src/redmost/ui/icons/feather-dark/settings.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/icons/feather-dark/sliders.svg` & `redmost-0.4.7/src/redmost/ui/icons/feather-dark/sliders.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/icons/feather-dark/zoom.svg` & `redmost-0.4.7/src/redmost/ui/icons/feather-dark/zoom.svg`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/main_window.ui` & `redmost-0.4.7/src/redmost/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/redmost.png` & `redmost-0.4.7/src/redmost/ui/redmost.png`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/ui/settings_dialog.ui` & `redmost-0.4.7/src/redmost/ui/settings_dialog.ui`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost/utils.py` & `redmost-0.4.7/src/redmost/utils.py`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/src/redmost.egg-info/PKG-INFO` & `redmost-0.4.7/src/redmost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redmost
-Version: 0.4.6
+Version: 0.4.7
 Summary: Display spectra and estimate their redshifts.
 Author: Maurizio D'Addona
 Author-email: mauritiusdadd@gmail.com
 Maintainer: Maurizio D'Addona
 Maintainer-email: mauritiusdadd@gmail.com
 License: BSD 3-Clause License
         
@@ -63,15 +63,17 @@
 Requires-Dist: pytest-qt; extra == "test"
 Requires-Dist: coverage; extra == "test"
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10817885.svg)](https://doi.org/10.5281/zenodo.10817885)
 [![DOCS](https://readthedocs.org/projects/redmost/badge/?version=latest)](https://redmost.readthedocs.io/en/latest/) [![Coverage Status](https://coveralls.io/repos/github/mauritiusdadd/redmost/badge.svg?branch=main)](https://coveralls.io/github/mauritiusdadd/redmost?branch=main) [![Testing PyQt6](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyqt6.yml/badge.svg)](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyqt6.yml) [![Testing PySide6](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyside6.yml/badge.svg)](https://github.com/mauritiusdadd/redmost/actions/workflows/test_linux_pyside6.yml)
 # REDMOST 
 
-<b>RED</b>shift <b>M</b>easurement <b>O</b>f <b>S</b>pec<b>T</b>ra is a Qt6 Graphical User Interface (GUI) to do redshift measurements on 1D spectra.
+<b>RED</b>shift <b>M</b>easurements <b>O</b>f <b>S</b>pec<b>T</b>ra is a Qt6 Graphical User Interface (GUI) to do redshift measurements on 1D spectra.
+
+![Redmost main window](https://github.com/mauritiusdadd/redmost/blob/main/docs/pics/main_ui_spectrum.png?raw=true)
 
 If [redrock][1] is correctly installed, it cat be used as a backend to measure the redshift.
 
 # Installation
 
 This is a python program based on Qt6 and supports both PyQt6 and PySide6 backends. It also support PyQt5 backend but it is not fully tested and may not work as expected.
 Since it is a good practice to not mess up the system-wide python environment, you should install this program in a virtual environment. If you don't have a virtual environment yet, you can create one with the command
```

### Comparing `redmost-0.4.6/src/redmost.egg-info/SOURCES.txt` & `redmost-0.4.7/src/redmost.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -17,17 +17,43 @@
 docs/_static/css/custom.css
 docs/module_docs/backends_rrock.rst
 docs/module_docs/gui.rst
 docs/module_docs/lines.rst
 docs/module_docs/loaders.rst
 docs/module_docs/qt_compat.rst
 docs/module_docs/utils.rst
+docs/pics/dialog_about.png
+docs/pics/dialog_controls.png
+docs/pics/dialog_load_spectra.png
+docs/pics/dialog_settings_appearence.png
+docs/pics/dialog_settings_general.png
 docs/pics/github-mark.png
+docs/pics/main_ui_add_line.png
+docs/pics/main_ui_annotated.png
+docs/pics/main_ui_clean.png
+docs/pics/main_ui_identification.png
+docs/pics/main_ui_multi_lines.png
+docs/pics/main_ui_redrock.png
+docs/pics/main_ui_select_lines.png
+docs/pics/main_ui_spectrum.png
+docs/pics/menu_about.png
+docs/pics/menu_edit.png
+docs/pics/menu_file.png
+docs/pics/menu_tools.png
 docs/pics/redmost.svg
-docs/tutorials/tut_01.rst
+docs/pics/icons/file-plus.svg
+docs/pics/icons/folder.svg
+docs/pics/icons/maximize.svg
+docs/pics/icons/play.svg
+docs/pics/icons/save.svg
+docs/pics/icons/zoom-in.svg
+docs/pics/icons/zoom-out.svg
+docs/tutorials/tut_01_load_spectra.rst
+docs/tutorials/tut_02_line_tools.rst
+docs/tutorials/tut_03_use_existing_zcat.rst
 src/redmost/__init__.py
 src/redmost/_version.py
 src/redmost/gui.py
 src/redmost/lines.py
 src/redmost/loaders.py
 src/redmost/py.typed
 src/redmost/qt_compat.py
```

### Comparing `redmost-0.4.6/test/data/spec_95.fits` & `redmost-0.4.7/test/data/spec_95.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/spec_955.fits` & `redmost-0.4.7/test/data/spec_955.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/spec_963.fits` & `redmost-0.4.7/test/data/spec_963.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/spec_965.fits` & `redmost-0.4.7/test/data/spec_965.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/spec_966.fits` & `redmost-0.4.7/test/data/spec_966.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/spec_971.fits` & `redmost-0.4.7/test/data/spec_971.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/spec_988.fits` & `redmost-0.4.7/test/data/spec_988.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/spec_991.fits` & `redmost-0.4.7/test/data/spec_991.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/spec_994.fits` & `redmost-0.4.7/test/data/spec_994.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/spec_997.fits` & `redmost-0.4.7/test/data/spec_997.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/test_project_1.json` & `redmost-0.4.7/test/data/test_project_1.json`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/test_project_2.json` & `redmost-0.4.7/test/data/test_project_2.json`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/data/test_zcat.fits` & `redmost-0.4.7/test/data/test_zcat.fits`

 * *Files identical despite different names*

### Comparing `redmost-0.4.6/test/test_pyqt_basic.py` & `redmost-0.4.7/test/test_pyqt_basic.py`

 * *Files identical despite different names*


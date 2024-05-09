# Comparing `tmp/three_d_converter-0.1.5.tar.gz` & `tmp/three_d_converter-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "three_d_converter-0.1.5.tar", max compression
+gzip compressed data, was "three_d_converter-1.0.0.tar", max compression
```

## Comparing `three_d_converter-0.1.5.tar` & `three_d_converter-1.0.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0        0 2024-03-25 09:14:32.209732 three_d_converter-0.1.5/README.md
--rw-r--r--   0        0        0      394 2024-04-09 14:35:14.568719 three_d_converter-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-04-08 08:17:05.466098 three_d_converter-0.1.5/three_d_converter/.DS_Store
--rw-r--r--   0        0        0       75 2024-03-27 09:28:17.451540 three_d_converter-0.1.5/three_d_converter/__init__.py
--rw-r--r--   0        0        0     1886 2024-03-25 11:28:49.087664 three_d_converter-0.1.5/three_d_converter/blender_installation.py
--rw-r--r--   0        0        0        0 2024-03-26 16:33:43.145406 three_d_converter-0.1.5/three_d_converter/blender_scripts/__init__.py
--rw-r--r--   0        0        0      187 2024-03-27 09:22:16.615625 three_d_converter-0.1.5/three_d_converter/blender_scripts/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      191 2024-04-09 08:40:22.685027 three_d_converter-0.1.5/three_d_converter/blender_scripts/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0        0 2024-03-26 16:34:01.604872 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__init__.py
--rw-r--r--   0        0        0      196 2024-03-27 09:22:16.633256 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      200 2024-04-09 10:34:51.344308 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      887 2024-04-09 09:29:51.917449 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1046 2024-04-09 10:34:51.345659 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-312.pyc
--rw-r--r--   0        0        0     1537 2024-04-09 14:05:35.928740 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0     1987 2024-04-09 11:02:09.386492 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-312.pyc
--rw-r--r--   0        0        0      859 2024-04-09 09:29:51.918277 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc
--rw-r--r--   0        0        0     1154 2024-04-09 10:34:51.345932 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-312.pyc
--rw-r--r--   0        0        0      967 2024-04-09 09:29:51.919353 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc
--rw-r--r--   0        0        0     1259 2024-04-09 10:34:51.346199 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-312.pyc
--rw-r--r--   0        0        0      886 2024-04-09 09:29:51.919871 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc
--rw-r--r--   0        0        0     1177 2024-04-09 10:34:51.346445 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-312.pyc
--rw-r--r--   0        0        0      903 2024-04-09 09:29:51.920379 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc
--rw-r--r--   0        0        0     1197 2024-04-09 10:34:51.346690 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-312.pyc
--rw-r--r--   0        0        0     1928 2024-04-09 09:29:51.921028 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc
--rw-r--r--   0        0        0     3136 2024-04-09 10:34:51.347101 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-312.pyc
--rw-r--r--   0        0        0      859 2024-04-09 09:29:51.921810 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc
--rw-r--r--   0        0        0     1154 2024-04-09 10:34:51.348239 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-312.pyc
--rw-r--r--   0        0        0      350 2024-04-09 09:13:58.741268 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/base.py
--rw-r--r--   0        0        0     1321 2024-04-09 11:01:41.021582 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/factory.py
--rw-r--r--   0        0        0      450 2024-04-09 09:14:20.398260 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/fbx.py
--rw-r--r--   0        0        0      602 2024-04-09 09:14:23.099228 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/gltf_glb.py
--rw-r--r--   0        0        0      498 2024-04-09 09:14:25.111303 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/obj.py
--rw-r--r--   0        0        0      517 2024-04-09 09:14:27.770992 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/stl.py
--rw-r--r--   0        0        0     1988 2024-04-09 09:14:30.358002 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/usdz.py
--rw-r--r--   0        0        0      449 2024-04-09 09:14:33.051927 three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/x3d.py
--rw-r--r--   0        0        0        0 2024-03-26 16:34:00.638176 three_d_converter-0.1.5/three_d_converter/blender_scripts/filehandler/__init__.py
--rw-r--r--   0        0        0      199 2024-03-27 09:22:16.616322 three_d_converter-0.1.5/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      203 2024-04-09 08:43:55.165250 three_d_converter-0.1.5/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     1400 2024-04-08 13:44:10.244096 three_d_converter-0.1.5/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc
--rw-r--r--   0        0        0     2128 2024-04-09 08:43:55.165642 three_d_converter-0.1.5/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-312.pyc
--rw-r--r--   0        0        0      970 2024-04-08 13:29:43.871938 three_d_converter-0.1.5/three_d_converter/blender_scripts/filehandler/filehandler.py
--rw-r--r--   0        0        0        0 2024-03-26 16:33:58.724687 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__init__.py
--rw-r--r--   0        0        0      196 2024-03-27 09:21:41.584714 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      200 2024-04-09 08:40:22.685263 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      859 2024-04-09 09:29:51.901451 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1010 2024-04-09 09:50:51.785009 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-312.pyc
--rw-r--r--   0        0        0     1525 2024-04-09 14:05:35.913742 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc
--rw-r--r--   0        0        0     1982 2024-04-09 10:28:45.392816 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-312.pyc
--rw-r--r--   0        0        0      741 2024-04-09 09:29:51.902293 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc
--rw-r--r--   0        0        0      948 2024-04-09 09:50:51.785816 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-312.pyc
--rw-r--r--   0        0        0      772 2024-04-09 09:29:51.902889 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc
--rw-r--r--   0        0        0     1013 2024-04-09 09:50:51.786414 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-312.pyc
--rw-r--r--   0        0        0      741 2024-04-09 09:29:51.903368 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc
--rw-r--r--   0        0        0      948 2024-04-09 09:50:51.787013 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-312.pyc
--rw-r--r--   0        0        0      740 2024-04-09 09:29:51.903928 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc
--rw-r--r--   0        0        0      947 2024-04-09 09:50:51.787541 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-312.pyc
--rw-r--r--   0        0        0     1442 2024-04-09 09:29:51.904523 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc
--rw-r--r--   0        0        0     2541 2024-04-09 09:50:51.788586 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-312.pyc
--rw-r--r--   0        0        0      741 2024-04-09 09:29:51.915700 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc
--rw-r--r--   0        0        0      948 2024-04-09 09:50:51.790486 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-312.pyc
--rw-r--r--   0        0        0      332 2024-04-09 09:12:24.769234 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/base.py
--rw-r--r--   0        0        0     1307 2024-04-09 09:53:43.142858 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/factory.py
--rw-r--r--   0        0        0      296 2024-04-09 09:12:31.844186 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/fbx.py
--rw-r--r--   0        0        0      335 2024-04-09 09:12:34.306412 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/gltf_glb.py
--rw-r--r--   0        0        0      295 2024-04-09 09:12:37.687378 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/obj.py
--rw-r--r--   0        0        0      294 2024-04-09 09:12:39.872242 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/stl.py
--rw-r--r--   0        0        0     1485 2024-04-09 09:12:44.984703 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/usdz.py
--rw-r--r--   0        0        0      295 2024-04-09 09:12:48.283277 three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/x3d.py
--rw-r--r--   0        0        0     1891 2024-04-09 09:29:49.597417 three_d_converter-0.1.5/three_d_converter/blender_scripts/main.py
--rw-r--r--   0        0        0      543 2024-04-09 14:05:13.234479 three_d_converter-0.1.5/three_d_converter/converter.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 three_d_converter-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-25 09:14:32.209732 three_d_converter-1.0.0/README.md
+-rw-r--r--   0        0        0      414 2024-05-09 18:59:44.686380 three_d_converter-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-04-24 14:56:42.722118 three_d_converter-1.0.0/three_d_converter/.DS_Store
+-rw-r--r--   0        0        0       75 2024-03-27 09:28:17.451540 three_d_converter-1.0.0/three_d_converter/__init__.py
+-rw-r--r--   0        0        0     1886 2024-03-25 11:28:49.087664 three_d_converter-1.0.0/three_d_converter/blender_installation.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:33:43.145406 three_d_converter-1.0.0/three_d_converter/blender_scripts/__init__.py
+-rw-r--r--   0        0        0      187 2024-03-27 09:22:16.615625 three_d_converter-1.0.0/three_d_converter/blender_scripts/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      191 2024-04-09 08:40:22.685027 three_d_converter-1.0.0/three_d_converter/blender_scripts/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0        0 2024-03-26 16:34:01.604872 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-27 09:22:16.633256 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      200 2024-04-09 10:34:51.344308 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      887 2024-04-09 09:29:51.917449 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1046 2024-04-09 10:34:51.345659 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-312.pyc
+-rw-r--r--   0        0        0     1537 2024-04-09 14:05:35.928740 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0     1987 2024-04-09 11:02:09.386492 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-312.pyc
+-rw-r--r--   0        0        0      859 2024-04-09 09:29:51.918277 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc
+-rw-r--r--   0        0        0     1154 2024-04-09 10:34:51.345932 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-312.pyc
+-rw-r--r--   0        0        0      967 2024-04-09 09:29:51.919353 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc
+-rw-r--r--   0        0        0     1259 2024-04-09 10:34:51.346199 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-312.pyc
+-rw-r--r--   0        0        0      886 2024-04-09 09:29:51.919871 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc
+-rw-r--r--   0        0        0     1177 2024-04-09 10:34:51.346445 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-312.pyc
+-rw-r--r--   0        0        0      903 2024-04-09 09:29:51.920379 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc
+-rw-r--r--   0        0        0     1197 2024-04-09 10:34:51.346690 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-312.pyc
+-rw-r--r--   0        0        0     1928 2024-04-09 09:29:51.921028 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc
+-rw-r--r--   0        0        0     3136 2024-04-09 10:34:51.347101 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-312.pyc
+-rw-r--r--   0        0        0      859 2024-04-09 09:29:51.921810 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc
+-rw-r--r--   0        0        0     1154 2024-04-09 10:34:51.348239 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-312.pyc
+-rw-r--r--   0        0        0      350 2024-04-09 09:13:58.741268 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/base.py
+-rw-r--r--   0        0        0     1321 2024-04-09 11:01:41.021582 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/factory.py
+-rw-r--r--   0        0        0      450 2024-04-09 09:14:20.398260 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/fbx.py
+-rw-r--r--   0        0        0      602 2024-04-09 09:14:23.099228 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/gltf_glb.py
+-rw-r--r--   0        0        0      498 2024-04-09 09:14:25.111303 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/obj.py
+-rw-r--r--   0        0        0      517 2024-04-09 09:14:27.770992 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/stl.py
+-rw-r--r--   0        0        0     1988 2024-04-09 09:14:30.358002 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/usdz.py
+-rw-r--r--   0        0        0      449 2024-04-09 09:14:33.051927 three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/x3d.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:34:00.638176 three_d_converter-1.0.0/three_d_converter/blender_scripts/filehandler/__init__.py
+-rw-r--r--   0        0        0      199 2024-03-27 09:22:16.616322 three_d_converter-1.0.0/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      203 2024-04-09 08:43:55.165250 three_d_converter-1.0.0/three_d_converter/blender_scripts/filehandler/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     1400 2024-04-08 13:44:10.244096 three_d_converter-1.0.0/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc
+-rw-r--r--   0        0        0     2128 2024-04-09 08:43:55.165642 three_d_converter-1.0.0/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-312.pyc
+-rw-r--r--   0        0        0      970 2024-04-12 14:49:17.986027 three_d_converter-1.0.0/three_d_converter/blender_scripts/filehandler/filehandler.py
+-rw-r--r--   0        0        0        0 2024-03-26 16:33:58.724687 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-27 09:21:41.584714 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      200 2024-04-09 08:40:22.685263 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0      859 2024-04-09 09:29:51.901451 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1010 2024-04-09 09:50:51.785009 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-312.pyc
+-rw-r--r--   0        0        0     1525 2024-04-09 14:05:35.913742 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0     1982 2024-04-09 10:28:45.392816 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-312.pyc
+-rw-r--r--   0        0        0      741 2024-04-09 09:29:51.902293 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc
+-rw-r--r--   0        0        0      948 2024-04-09 09:50:51.785816 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-312.pyc
+-rw-r--r--   0        0        0      772 2024-04-09 09:29:51.902889 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc
+-rw-r--r--   0        0        0     1013 2024-04-09 09:50:51.786414 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-312.pyc
+-rw-r--r--   0        0        0      741 2024-04-09 09:29:51.903368 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc
+-rw-r--r--   0        0        0      948 2024-04-09 09:50:51.787013 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-312.pyc
+-rw-r--r--   0        0        0      740 2024-04-09 09:29:51.903928 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc
+-rw-r--r--   0        0        0      947 2024-04-09 09:50:51.787541 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-312.pyc
+-rw-r--r--   0        0        0     1442 2024-04-09 09:29:51.904523 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc
+-rw-r--r--   0        0        0     2541 2024-04-09 09:50:51.788586 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-312.pyc
+-rw-r--r--   0        0        0      741 2024-04-09 09:29:51.915700 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc
+-rw-r--r--   0        0        0      948 2024-04-09 09:50:51.790486 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-312.pyc
+-rw-r--r--   0        0        0      332 2024-04-09 09:12:24.769234 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/base.py
+-rw-r--r--   0        0        0     1307 2024-04-09 09:53:43.142858 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/factory.py
+-rw-r--r--   0        0        0      296 2024-04-09 09:12:31.844186 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/fbx.py
+-rw-r--r--   0        0        0      335 2024-04-09 09:12:34.306412 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/gltf_glb.py
+-rw-r--r--   0        0        0      295 2024-04-09 09:12:37.687378 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/obj.py
+-rw-r--r--   0        0        0      294 2024-04-09 09:12:39.872242 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/stl.py
+-rw-r--r--   0        0        0     1485 2024-04-09 09:12:44.984703 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/usdz.py
+-rw-r--r--   0        0        0      295 2024-04-09 09:12:48.283277 three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/x3d.py
+-rw-r--r--   0        0        0     1891 2024-04-09 09:29:49.597417 three_d_converter-1.0.0/three_d_converter/blender_scripts/main.py
+-rw-r--r--   0        0        0      544 2024-04-24 14:39:46.517854 three_d_converter-1.0.0/three_d_converter/converter.py
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 three_d_converter-1.0.0/PKG-INFO
```

### Comparing `three_d_converter-0.1.5/three_d_converter/.DS_Store` & `three_d_converter-1.0.0/three_d_converter/.DS_Store`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_installation.py` & `three_d_converter-1.0.0/three_d_converter/blender_installation.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/base.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/factory.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/fbx.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/gltf_glb.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/obj.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/stl.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/usdz.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/__pycache__/x3d.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/factory.py` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/factory.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/gltf_glb.py` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/gltf_glb.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/stl.py` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/stl.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/exporter/usdz.py` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/exporter/usdz.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/filehandler/__pycache__/filehandler.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/filehandler/filehandler.py` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/filehandler/filehandler.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/base.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/factory.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/fbx.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/gltf_glb.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/obj.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/stl.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/usdz.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-312.pyc` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/__pycache__/x3d.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/factory.py` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/factory.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/importer/usdz.py` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/importer/usdz.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/blender_scripts/main.py` & `three_d_converter-1.0.0/three_d_converter/blender_scripts/main.py`

 * *Files identical despite different names*

### Comparing `three_d_converter-0.1.5/three_d_converter/converter.py` & `three_d_converter-1.0.0/three_d_converter/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,9 @@
             "-noaudio",
             "--python",
             SCRIPT_PATH.resolve().as_posix(),
             "--",
             input_file,
             output_file,
         ]
+
         subprocess.run(blender_command)
```


# Comparing `tmp/lazurite-0.1.2.tar.gz` & `tmp/lazurite-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazurite-0.1.2.tar", last modified: Sun May  5 22:10:22 2024, max compression
+gzip compressed data, was "lazurite-0.1.3.tar", last modified: Thu May  9 21:50:50 2024, max compression
```

## Comparing `lazurite-0.1.2.tar` & `lazurite-0.1.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 22:10:22.185570 lazurite-0.1.2/
--rw-rw-rw-   0        0        0    35823 2024-05-03 11:00:28.000000 lazurite-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1749 2024-05-05 22:10:22.185570 lazurite-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      659 2024-05-05 13:52:03.000000 lazurite-0.1.2/README.md
--rw-rw-rw-   0        0        0     1216 2024-05-05 22:09:19.000000 lazurite-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-05 22:10:22.185570 lazurite-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-05 22:10:22.117741 lazurite-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 22:10:22.129804 lazurite-0.1.2/src/lazurite/
--rw-rw-rw-   0        0        0        0 2024-02-13 20:06:38.000000 lazurite-0.1.2/src/lazurite/__init__.py
--rw-rw-rw-   0        0        0       73 2024-05-03 09:54:14.000000 lazurite-0.1.2/src/lazurite/__main__.py
--rw-rw-rw-   0        0        0    12806 2024-05-03 10:01:10.000000 lazurite-0.1.2/src/lazurite/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:10:22.160405 lazurite-0.1.2/src/lazurite/compiler/
--rw-rw-rw-   0        0        0       68 2024-02-13 21:47:08.000000 lazurite-0.1.2/src/lazurite/compiler/__init__.py
--rw-rw-rw-   0        0        0     2645 2024-04-30 10:45:06.000000 lazurite-0.1.2/src/lazurite/compiler/dxc.py
--rw-rw-rw-   0        0        0      766 2024-04-01 13:25:10.000000 lazurite-0.1.2/src/lazurite/compiler/macro_define.py
--rw-rw-rw-   0        0        0     6461 2024-05-03 11:38:02.000000 lazurite-0.1.2/src/lazurite/compiler/shaderc.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:10:22.161433 lazurite-0.1.2/src/lazurite/decompiler/
--rw-rw-rw-   0        0        0        0 2023-07-31 21:03:18.000000 lazurite-0.1.2/src/lazurite/decompiler/__init__.py
--rw-rw-rw-   0        0        0    25267 2024-03-31 20:06:22.000000 lazurite-0.1.2/src/lazurite/decompiler/macro_decompiler.py
--rw-rw-rw-   0        0        0     3448 2024-03-31 20:05:52.000000 lazurite-0.1.2/src/lazurite/decompiler/varying_decompiler.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:10:22.169446 lazurite-0.1.2/src/lazurite/material/
--rw-rw-rw-   0        0        0       32 2024-02-13 21:47:22.000000 lazurite-0.1.2/src/lazurite/material/__init__.py
--rw-rw-rw-   0        0        0     6210 2024-04-29 18:16:44.000000 lazurite-0.1.2/src/lazurite/material/buffer.py
--rw-rw-rw-   0        0        0      359 2024-03-20 14:54:26.000000 lazurite-0.1.2/src/lazurite/material/encryption.py
--rw-rw-rw-   0        0        0    21695 2024-04-29 14:03:32.000000 lazurite-0.1.2/src/lazurite/material/material.py
--rw-rw-rw-   0        0        0      750 2024-02-13 20:38:24.000000 lazurite-0.1.2/src/lazurite/material/platform.py
--rw-rw-rw-   0        0        0      114 2023-10-07 14:20:58.000000 lazurite-0.1.2/src/lazurite/material/precision.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:10:22.177467 lazurite-0.1.2/src/lazurite/material/shader_pass/
--rw-rw-rw-   0        0        0       28 2024-02-13 21:07:36.000000 lazurite-0.1.2/src/lazurite/material/shader_pass/__init__.py
--rw-rw-rw-   0        0        0     5398 2024-04-06 20:22:04.000000 lazurite-0.1.2/src/lazurite/material/shader_pass/bgfx_shader.py
--rw-rw-rw-   0        0        0      377 2024-02-18 16:33:18.000000 lazurite-0.1.2/src/lazurite/material/shader_pass/blend_mode.py
--rw-rw-rw-   0        0        0     4192 2024-04-06 20:22:08.000000 lazurite-0.1.2/src/lazurite/material/shader_pass/shader_definition.py
--rw-rw-rw-   0        0        0     5119 2024-04-29 18:12:28.000000 lazurite-0.1.2/src/lazurite/material/shader_pass/shader_input.py
--rw-rw-rw-   0        0        0     6354 2024-05-05 22:06:01.000000 lazurite-0.1.2/src/lazurite/material/shader_pass/shader_pass.py
--rw-rw-rw-   0        0        0     1595 2024-03-01 01:21:50.000000 lazurite-0.1.2/src/lazurite/material/shader_pass/supported_platforms.py
--rw-rw-rw-   0        0        0     3871 2024-04-06 20:22:20.000000 lazurite-0.1.2/src/lazurite/material/shader_pass/variant.py
--rw-rw-rw-   0        0        0      121 2023-09-24 16:30:26.000000 lazurite-0.1.2/src/lazurite/material/stage.py
--rw-rw-rw-   0        0        0     2502 2024-04-13 17:47:30.000000 lazurite-0.1.2/src/lazurite/material/uniform.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:10:22.181490 lazurite-0.1.2/src/lazurite/project/
--rw-rw-rw-   0        0        0        0 2024-02-13 20:05:48.000000 lazurite-0.1.2/src/lazurite/project/__init__.py
--rw-rw-rw-   0        0        0      273 2024-04-01 22:39:38.000000 lazurite-0.1.2/src/lazurite/project/compiler_type.py
--rw-rw-rw-   0        0        0     3067 2024-04-06 20:35:26.000000 lazurite-0.1.2/src/lazurite/project/material_config.py
--rw-rw-rw-   0        0        0    13430 2024-04-13 15:11:28.000000 lazurite-0.1.2/src/lazurite/project/project.py
--rw-rw-rw-   0        0        0     5513 2024-04-06 20:35:26.000000 lazurite-0.1.2/src/lazurite/project/project_config.py
--rw-rw-rw-   0        0        0     1271 2024-04-01 22:38:14.000000 lazurite-0.1.2/src/lazurite/project/shader_file_overwrite.py
--rw-rw-rw-   0        0        0      838 2024-04-29 18:29:54.000000 lazurite-0.1.2/src/lazurite/tempfile.py
--rw-rw-rw-   0        0        0     2260 2024-02-24 14:42:42.000000 lazurite-0.1.2/src/lazurite/util.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:10:22.185570 lazurite-0.1.2/src/lazurite.egg-info/
--rw-rw-rw-   0        0        0     1749 2024-05-05 22:10:22.000000 lazurite-0.1.2/src/lazurite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1522 2024-05-05 22:10:22.000000 lazurite-0.1.2/src/lazurite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 22:10:22.000000 lazurite-0.1.2/src/lazurite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-05 22:10:22.000000 lazurite-0.1.2/src/lazurite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       38 2024-05-05 22:10:22.000000 lazurite-0.1.2/src/lazurite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-05 22:10:22.000000 lazurite-0.1.2/src/lazurite.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.817446 lazurite-0.1.3/
+-rw-rw-rw-   0        0        0    35823 2024-05-03 11:00:28.000000 lazurite-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1749 2024-05-09 21:50:50.817446 lazurite-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2024-05-05 13:52:03.000000 lazurite-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1216 2024-05-09 21:49:44.000000 lazurite-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 21:50:50.817446 lazurite-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.750797 lazurite-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.772056 lazurite-0.1.3/src/lazurite/
+-rw-rw-rw-   0        0        0        0 2024-02-13 20:06:38.000000 lazurite-0.1.3/src/lazurite/__init__.py
+-rw-rw-rw-   0        0        0       73 2024-05-03 09:54:14.000000 lazurite-0.1.3/src/lazurite/__main__.py
+-rw-rw-rw-   0        0        0    12806 2024-05-09 21:47:12.000000 lazurite-0.1.3/src/lazurite/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.793267 lazurite-0.1.3/src/lazurite/compiler/
+-rw-rw-rw-   0        0        0       68 2024-02-13 21:47:08.000000 lazurite-0.1.3/src/lazurite/compiler/__init__.py
+-rw-rw-rw-   0        0        0     2645 2024-04-30 10:45:06.000000 lazurite-0.1.3/src/lazurite/compiler/dxc.py
+-rw-rw-rw-   0        0        0      766 2024-04-01 13:25:10.000000 lazurite-0.1.3/src/lazurite/compiler/macro_define.py
+-rw-rw-rw-   0        0        0     6461 2024-05-03 11:38:02.000000 lazurite-0.1.3/src/lazurite/compiler/shaderc.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.797227 lazurite-0.1.3/src/lazurite/decompiler/
+-rw-rw-rw-   0        0        0        0 2023-07-31 21:03:18.000000 lazurite-0.1.3/src/lazurite/decompiler/__init__.py
+-rw-rw-rw-   0        0        0    25267 2024-03-31 20:06:22.000000 lazurite-0.1.3/src/lazurite/decompiler/macro_decompiler.py
+-rw-rw-rw-   0        0        0     3448 2024-03-31 20:05:52.000000 lazurite-0.1.3/src/lazurite/decompiler/varying_decompiler.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.804877 lazurite-0.1.3/src/lazurite/material/
+-rw-rw-rw-   0        0        0       32 2024-02-13 21:47:22.000000 lazurite-0.1.3/src/lazurite/material/__init__.py
+-rw-rw-rw-   0        0        0     6210 2024-05-08 16:14:47.000000 lazurite-0.1.3/src/lazurite/material/buffer.py
+-rw-rw-rw-   0        0        0      359 2024-03-20 14:54:26.000000 lazurite-0.1.3/src/lazurite/material/encryption.py
+-rw-rw-rw-   0        0        0    21695 2024-04-29 14:03:32.000000 lazurite-0.1.3/src/lazurite/material/material.py
+-rw-rw-rw-   0        0        0      750 2024-02-13 20:38:24.000000 lazurite-0.1.3/src/lazurite/material/platform.py
+-rw-rw-rw-   0        0        0      114 2023-10-07 14:20:58.000000 lazurite-0.1.3/src/lazurite/material/precision.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.811391 lazurite-0.1.3/src/lazurite/material/shader_pass/
+-rw-rw-rw-   0        0        0       28 2024-02-13 21:07:36.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/__init__.py
+-rw-rw-rw-   0        0        0     5398 2024-04-06 20:22:04.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/bgfx_shader.py
+-rw-rw-rw-   0        0        0      377 2024-02-18 16:33:18.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/blend_mode.py
+-rw-rw-rw-   0        0        0     4192 2024-04-06 20:22:08.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/shader_definition.py
+-rw-rw-rw-   0        0        0     5119 2024-04-29 18:12:28.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/shader_input.py
+-rw-rw-rw-   0        0        0     6354 2024-05-05 22:06:01.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/shader_pass.py
+-rw-rw-rw-   0        0        0     1595 2024-03-01 01:21:50.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/supported_platforms.py
+-rw-rw-rw-   0        0        0     3871 2024-04-06 20:22:20.000000 lazurite-0.1.3/src/lazurite/material/shader_pass/variant.py
+-rw-rw-rw-   0        0        0      121 2023-09-24 16:30:26.000000 lazurite-0.1.3/src/lazurite/material/stage.py
+-rw-rw-rw-   0        0        0     2502 2024-04-13 17:47:30.000000 lazurite-0.1.3/src/lazurite/material/uniform.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.817446 lazurite-0.1.3/src/lazurite/project/
+-rw-rw-rw-   0        0        0        0 2024-02-13 20:05:48.000000 lazurite-0.1.3/src/lazurite/project/__init__.py
+-rw-rw-rw-   0        0        0      273 2024-04-01 22:39:38.000000 lazurite-0.1.3/src/lazurite/project/compiler_type.py
+-rw-rw-rw-   0        0        0     3067 2024-04-06 20:35:26.000000 lazurite-0.1.3/src/lazurite/project/material_config.py
+-rw-rw-rw-   0        0        0    13430 2024-05-09 21:47:01.000000 lazurite-0.1.3/src/lazurite/project/project.py
+-rw-rw-rw-   0        0        0     5513 2024-04-06 20:35:26.000000 lazurite-0.1.3/src/lazurite/project/project_config.py
+-rw-rw-rw-   0        0        0     1271 2024-04-01 22:38:14.000000 lazurite-0.1.3/src/lazurite/project/shader_file_overwrite.py
+-rw-rw-rw-   0        0        0      838 2024-04-29 18:29:54.000000 lazurite-0.1.3/src/lazurite/tempfile.py
+-rw-rw-rw-   0        0        0     2260 2024-02-24 14:42:42.000000 lazurite-0.1.3/src/lazurite/util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:50:50.817446 lazurite-0.1.3/src/lazurite.egg-info/
+-rw-rw-rw-   0        0        0     1749 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1522 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       38 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 21:50:50.000000 lazurite-0.1.3/src/lazurite.egg-info/top_level.txt
```

### Comparing `lazurite-0.1.2/LICENSE` & `lazurite-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/PKG-INFO` & `lazurite-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazurite
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine
 Author: veka0
 Project-URL: Documentation, https://veka0.github.io/lazurite
 Project-URL: Repository, https://github.com/veka0/lazurite
 Keywords: shader,minecraft,bedrock,renderdragon
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lazurite-0.1.2/README.md` & `lazurite-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/pyproject.toml` & `lazurite-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lazurite"
 description = "Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine"
 keywords = ["shader", "minecraft", "bedrock", "renderdragon"]
-version = "0.1.2"
+version = "0.1.3"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{ name = "veka0" }]
 
 classifiers = [
     # General
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `lazurite-0.1.2/src/lazurite/cli.py` & `lazurite-0.1.3/src/lazurite/cli.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/compiler/dxc.py` & `lazurite-0.1.3/src/lazurite/compiler/dxc.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/compiler/macro_define.py` & `lazurite-0.1.3/src/lazurite/compiler/macro_define.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/compiler/shaderc.py` & `lazurite-0.1.3/src/lazurite/compiler/shaderc.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/decompiler/macro_decompiler.py` & `lazurite-0.1.3/src/lazurite/decompiler/macro_decompiler.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/decompiler/varying_decompiler.py` & `lazurite-0.1.3/src/lazurite/decompiler/varying_decompiler.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/buffer.py` & `lazurite-0.1.3/src/lazurite/material/buffer.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/material.py` & `lazurite-0.1.3/src/lazurite/material/material.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/platform.py` & `lazurite-0.1.3/src/lazurite/material/platform.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/shader_pass/bgfx_shader.py` & `lazurite-0.1.3/src/lazurite/material/shader_pass/bgfx_shader.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/shader_pass/shader_definition.py` & `lazurite-0.1.3/src/lazurite/material/shader_pass/shader_definition.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/shader_pass/shader_input.py` & `lazurite-0.1.3/src/lazurite/material/shader_pass/shader_input.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/shader_pass/shader_pass.py` & `lazurite-0.1.3/src/lazurite/material/shader_pass/shader_pass.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/shader_pass/supported_platforms.py` & `lazurite-0.1.3/src/lazurite/material/shader_pass/supported_platforms.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/shader_pass/variant.py` & `lazurite-0.1.3/src/lazurite/material/shader_pass/variant.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/material/uniform.py` & `lazurite-0.1.3/src/lazurite/material/uniform.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/project/material_config.py` & `lazurite-0.1.3/src/lazurite/project/material_config.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/project/project.py` & `lazurite-0.1.3/src/lazurite/project/project.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -324,25 +324,25 @@
                     _compile_bgfx_shader_async,
                     len(shaders) * [shaderc_compiler],
                     arg_code_path,
                     arg_stage,
                     arg_platform,
                     arg_varying,
                     arg_defines,
-                    len(shaders) * [mat_config.compiler_options + dxc_args],
+                    len(shaders) * [mat_config.compiler_options + shaderc_args],
                 )
             else:
                 results = executor.map(
                     dxc_compiler.compile,
                     arg_code_path,
                     arg_platform,
                     arg_stage,
                     arg_entry_point,
                     arg_defines,
-                    len(shaders) * [mat_config.compiler_options + shaderc_args],
+                    len(shaders) * [mat_config.compiler_options + dxc_args],
                 )
 
         for shader, result in zip(shaders, results):
             if mat_config.compiler_type is CompilerType.SHADERC:
                 shader.bgfx_shader = result
             else:
                 shader.bgfx_shader.shader_bytes = result
```

### Comparing `lazurite-0.1.2/src/lazurite/project/project_config.py` & `lazurite-0.1.3/src/lazurite/project/project_config.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/project/shader_file_overwrite.py` & `lazurite-0.1.3/src/lazurite/project/shader_file_overwrite.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/tempfile.py` & `lazurite-0.1.3/src/lazurite/tempfile.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite/util.py` & `lazurite-0.1.3/src/lazurite/util.py`

 * *Files identical despite different names*

### Comparing `lazurite-0.1.2/src/lazurite.egg-info/PKG-INFO` & `lazurite-0.1.3/src/lazurite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazurite
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unofficial shader development tool for Minecraft: Bedrock Edition with RenderDragon graphics engine
 Author: veka0
 Project-URL: Documentation, https://veka0.github.io/lazurite
 Project-URL: Repository, https://github.com/veka0/lazurite
 Keywords: shader,minecraft,bedrock,renderdragon
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lazurite-0.1.2/src/lazurite.egg-info/SOURCES.txt` & `lazurite-0.1.3/src/lazurite.egg-info/SOURCES.txt`

 * *Files identical despite different names*


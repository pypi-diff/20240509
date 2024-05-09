# Comparing `tmp/nonebot_plugin_mysticism-0.1.1.tar.gz` & `tmp/nonebot_plugin_mysticism-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mysticism-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_mysticism-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_mysticism-0.1.1.tar` & `nonebot_plugin_mysticism-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11332 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/LICENSE
--rw-r--r--   0        0        0     2483 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/README.md
--rw-r--r--   0        0        0      466 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/__init__.py
--rw-r--r--   0        0        0      158 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/config.py
--rw-r--r--   0        0        0      702 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/rule.py
--rw-r--r--   0        0        0     5325 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot.py
--rw-r--r--   0        0        0     3649 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_formations.yaml
--rw-r--r--   0        0        0        0 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/__init__.py
--rw-r--r--   0        0        0     3327 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml
--rw-r--r--   0        0        0      774 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml
--rw-r--r--   0        0        0     2176 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/waite.yaml
--rw-r--r--   0        0        0    11064 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_uitls.py
--rw-r--r--   0        0        0      959 2024-05-09 12:24:29.427879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/utils.py
--rw-r--r--   0        0        0      555 2024-05-09 12:24:29.427879 nonebot_plugin_mysticism-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 nonebot_plugin_mysticism-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11332 2024-05-09 12:35:24.261096 nonebot_plugin_mysticism-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2483 2024-05-09 12:35:24.261096 nonebot_plugin_mysticism-0.1.2/README.md
+-rw-r--r--   0        0        0      466 2024-05-09 12:35:24.261096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/config.py
+-rw-r--r--   0        0        0      702 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/rule.py
+-rw-r--r--   0        0        0     5325 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot.py
+-rw-r--r--   0        0        0     3649 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_formations.yaml
+-rw-r--r--   0        0        0        0 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/__init__.py
+-rw-r--r--   0        0        0     3327 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml
+-rw-r--r--   0        0        0      774 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml
+-rw-r--r--   0        0        0     2176 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/waite.yaml
+-rw-r--r--   0        0        0    11061 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_uitls.py
+-rw-r--r--   0        0        0      959 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/utils.py
+-rw-r--r--   0        0        0      555 2024-05-09 12:35:24.265096 nonebot_plugin_mysticism-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 nonebot_plugin_mysticism-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_mysticism-0.1.1/LICENSE` & `nonebot_plugin_mysticism-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.1/README.md` & `nonebot_plugin_mysticism-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/rule.py` & `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot.py` & `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_formations.yaml` & `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_formations.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml` & `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml` & `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/waite.yaml` & `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_theme/waite.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_uitls.py` & `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/tarot_uitls.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,21 +227,21 @@
 
 BILIBILI = get_tarot(pathlib.Path(__file__).parent / "tarot_theme" / "bilibili.yaml")
 DEFAULT["cups"] = BILIBILI.cups
 DEFAULT["pentacles"] = BILIBILI.pentacles
 DEFAULT["swords"] = BILIBILI.swords
 DEFAULT["wands"] = BILIBILI.wands
 
-TOUHOU = get_tarot(pathlib.Path(__file__).parent / "tarot_theme" / "touhou.yaml")
+WAITE = get_tarot(pathlib.Path(__file__).parent / "tarot_theme" / "waite.yaml")
 BULE_ARCHIVE = get_tarot(
     pathlib.Path(__file__).parent / "tarot_theme" / "blue_archive.yaml"
 )
 
 
-THEME = [BILIBILI, BULE_ARCHIVE, TOUHOU]
+THEME = [BILIBILI, BULE_ARCHIVE, WAITE]
 
 TAROT_STACK = [
     "cups.ace",
     "cups.two",
     "cups.three",
     "cups.four",
     "cups.five",
```

### Comparing `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/utils.py` & `nonebot_plugin_mysticism-0.1.2/nonebot_plugin_mysticism/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.1/pyproject.toml` & `nonebot_plugin_mysticism-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mysticism"
-version = "0.1.1"
+version = "0.1.2"
 description = "占卜辅助工具"
 authors = ["Yan <1964649083@qq.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 keywords = ["tarot", "nonebot", "nonebot2", "bot", "qq"]
 homepage = "https://github.com/Yan-Zero/nonebot_plugin_mysticism"
```

### Comparing `nonebot_plugin_mysticism-0.1.1/PKG-INFO` & `nonebot_plugin_mysticism-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mysticism
-Version: 0.1.1
+Version: 0.1.2
 Summary: 占卜辅助工具
 Home-page: https://github.com/Yan-Zero/nonebot_plugin_mysticism
 License: Apache-2.0
 Keywords: tarot,nonebot,nonebot2,bot,qq
 Author: Yan
 Author-email: 1964649083@qq.com
 Requires-Python: >=3.11,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mysticism Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mysticism Version: 0.1.2 Summary:
 å åè¾å©å·¥å· Home-page: https://github.com/Yan-Zero/
 nonebot_plugin_mysticism License: Apache-2.0 Keywords:
 tarot,nonebot,nonebot2,bot,qq Author: Yan Author-email: 1964649083@qq.com
 Requires-Python: >=3.11,<4.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.5,<4.0.0) Requires-Dist: nonebot-
```


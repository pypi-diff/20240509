# Comparing `tmp/nonebot_plugin_mysticism-0.1.0.tar.gz` & `tmp/nonebot_plugin_mysticism-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mysticism-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_mysticism-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_mysticism-0.1.0.tar` & `nonebot_plugin_mysticism-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11332 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/LICENSE
--rw-r--r--   0        0        0     2483 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/README.md
--rw-r--r--   0        0        0      470 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/__init__.py
--rw-r--r--   0        0        0      158 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/config.py
--rw-r--r--   0        0        0      702 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/rule.py
--rw-r--r--   0        0        0     5325 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot.py
--rw-r--r--   0        0        0     3649 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_formations.yaml
--rw-r--r--   0        0        0        0 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_theme/__init__.py
--rw-r--r--   0        0        0     3327 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml
--rw-r--r--   0        0        0      774 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml
--rw-r--r--   0        0        0     2176 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_theme/waite.yaml
--rw-r--r--   0        0        0    11064 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_uitls.py
--rw-r--r--   0        0        0      959 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/utils.py
--rw-r--r--   0        0        0      537 2024-05-09 12:16:02.031117 nonebot_plugin_mysticism-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 nonebot_plugin_mysticism-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11332 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2483 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/README.md
+-rw-r--r--   0        0        0      466 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/config.py
+-rw-r--r--   0        0        0      702 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/rule.py
+-rw-r--r--   0        0        0     5325 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot.py
+-rw-r--r--   0        0        0     3649 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_formations.yaml
+-rw-r--r--   0        0        0        0 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/__init__.py
+-rw-r--r--   0        0        0     3327 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml
+-rw-r--r--   0        0        0      774 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml
+-rw-r--r--   0        0        0     2176 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/waite.yaml
+-rw-r--r--   0        0        0    11064 2024-05-09 12:24:29.423879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_uitls.py
+-rw-r--r--   0        0        0      959 2024-05-09 12:24:29.427879 nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/utils.py
+-rw-r--r--   0        0        0      555 2024-05-09 12:24:29.427879 nonebot_plugin_mysticism-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 nonebot_plugin_mysticism-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_mysticism-0.1.0/LICENSE` & `nonebot_plugin_mysticism-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/README.md` & `nonebot_plugin_mysticism-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/rule.py` & `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/rule.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot.py` & `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_formations.yaml` & `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_formations.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml` & `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/bilibili.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml` & `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/blue_archive.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_theme/waite.yaml` & `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_theme/waite.yaml`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/tarot_uitls.py` & `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/tarot_uitls.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/nonebot_plugin_mysticism/utils.py` & `nonebot_plugin_mysticism-0.1.1/nonebot_plugin_mysticism/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mysticism-0.1.0/pyproject.toml` & `nonebot_plugin_mysticism-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-mysticism"
-version = "0.1.0"
+version = "0.1.1"
 description = "占卜辅助工具"
 authors = ["Yan <1964649083@qq.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 keywords = ["tarot", "nonebot", "nonebot2", "bot", "qq"]
 homepage = "https://github.com/Yan-Zero/nonebot_plugin_mysticism"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.9.5"
 nonebot2 = "^2.3.0"
 nonebot-adapter-onebot = "^2.4.3"
 pillow = "^10.3.0"
+pyyaml = "^6.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_mysticism-0.1.0/PKG-INFO` & `nonebot_plugin_mysticism-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mysticism
-Version: 0.1.0
+Version: 0.1.1
 Summary: 占卜辅助工具
 Home-page: https://github.com/Yan-Zero/nonebot_plugin_mysticism
 License: Apache-2.0
 Keywords: tarot,nonebot,nonebot2,bot,qq
 Author: Yan
 Author-email: 1964649083@qq.com
 Requires-Python: >=3.11,<4.0
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.4.3,<3.0.0)
 Requires-Dist: nonebot2 (>=2.3.0,<3.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 
 <div align="center">
 
 # nonebot-plugin-mysticism
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mysticism Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mysticism Version: 0.1.1 Summary:
 å åè¾å©å·¥å· Home-page: https://github.com/Yan-Zero/
 nonebot_plugin_mysticism License: Apache-2.0 Keywords:
 tarot,nonebot,nonebot2,bot,qq Author: Yan Author-email: 1964649083@qq.com
 Requires-Python: >=3.11,<4.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.5,<4.0.0) Requires-Dist: nonebot-
 adapter-onebot (>=2.4.3,<3.0.0) Requires-Dist: nonebot2 (>=2.3.0,<3.0.0)
-Requires-Dist: pillow (>=10.3.0,<11.0.0) Description-Content-Type: text/
-markdown
+Requires-Dist: pillow (>=10.3.0,<11.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Description-Content-Type: text/markdown
   # nonebot-plugin-mysticism _â¨ ç¥ç§å­¦å©æ â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ð ä»ç»
 ç¥ç§å­¦åå®¹ä»ä¾å¨±ä¹åä¸ªäººæ¢ç´¢ä½¿ç¨ï¼ä¸ææä»»ä½å½¢å¼çæ³å¾ãå»å­¦æéèå»ºè®®ãä½¿ç¨ç¥ç§å­¦ç¥è¯æè·å¾çè§£éãæ´å¯åå»ºè®®åºå½è°¨æå¯¹å¾ï¼å¹¶å¨å¿è¦æ¶å¨è¯¢ä¸ä¸äººå£«çæè§ï¼ç¹å«æ¯å¨æ¶åå¥åº·ãæ³å¾æè´¢å¡ç­éè¦å³å®æ¶ãå¯¹äºåºäºç¥ç§å­¦ç¥è¯èå¯¼è´çä»»ä½è¡ä¸ºæåæï¼ä½èæ¦ä¸è´è´£ãä½¿ç¨èåºèªè¡æ¿æä½¿ç¨ç¥ç§å­¦ç¥è¯æäº§ççä¸åé£é©åè´£ä»»ã
 å³äºç¥ç§å­¦ç°è±¡æç»è§£éæå½[æ¡£æ¡é¦](https://qm.qq.com/q/
 cUe58MaTtK)ææã ## ð¿ å®è£ ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin
 install nonebot_plugin_mysticism ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2
```


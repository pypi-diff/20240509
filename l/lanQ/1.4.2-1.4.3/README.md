# Comparing `tmp/lanQ-1.4.2.tar.gz` & `tmp/lanQ-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanQ-1.4.2.tar", last modified: Tue Apr 30 07:12:41 2024, max compression
+gzip compressed data, was "lanQ-1.4.3.tar", last modified: Thu May  9 02:37:48 2024, max compression
```

## Comparing `lanQ-1.4.2.tar` & `lanQ-1.4.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:12:41.232537 lanQ-1.4.2/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-04-30 07:12:41.232537 lanQ-1.4.2/PKG-INFO
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     7759 2024-04-30 06:59:30.000000 lanQ-1.4.2/README.md
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:12:41.232537 lanQ-1.4.2/lanQ.egg-info/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-04-30 07:12:41.000000 lanQ-1.4.2/lanQ.egg-info/PKG-INFO
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      371 2024-04-30 07:12:41.000000 lanQ-1.4.2/lanQ.egg-info/SOURCES.txt
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        1 2024-04-30 07:12:41.000000 lanQ-1.4.2/lanQ.egg-info/dependency_links.txt
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       10 2024-04-30 07:12:41.000000 lanQ-1.4.2/lanQ.egg-info/top_level.txt
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:12:41.232537 lanQ-1.4.2/lanQ_rule/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4.2/lanQ_rule/__init__.py
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:12:41.232537 lanQ-1.4.2/lanQ_rule/base_func/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:11:32.000000 lanQ-1.4.2/lanQ_rule/base_func/__init__.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     4593 2024-04-26 08:10:06.000000 lanQ-1.4.2/lanQ_rule/base_func/base.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    16072 2024-04-30 03:21:14.000000 lanQ-1.4.2/lanQ_rule/common_rule.py
-drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:12:41.232537 lanQ-1.4.2/lanQ_rule/config/
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 05:56:14.000000 lanQ-1.4.2/lanQ_rule/config/__init__.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2294 2024-04-19 03:19:55.000000 lanQ-1.4.2/lanQ_rule/config/const.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      230 2024-04-30 03:33:52.000000 lanQ-1.4.2/lanQ_rule/config/customize.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      991 2024-04-30 03:33:53.000000 lanQ-1.4.2/lanQ_rule/model_rule.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1153 2024-04-24 03:44:27.000000 lanQ-1.4.2/lanQ_rule/prompt_rule.py
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       38 2024-04-30 07:12:41.232537 lanQ-1.4.2/setup.cfg
--rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      394 2024-04-30 07:12:23.000000 lanQ-1.4.2/setup.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-09 02:37:48.803319 lanQ-1.4.3/PKG-INFO
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     7759 2024-04-30 06:59:30.000000 lanQ-1.4.3/README.md
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/lanQ.egg-info/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      187 2024-05-09 02:37:48.000000 lanQ-1.4.3/lanQ.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      400 2024-05-09 02:37:48.000000 lanQ-1.4.3/lanQ.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        1 2024-05-09 02:37:48.000000 lanQ-1.4.3/lanQ.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       10 2024-05-09 02:37:48.000000 lanQ-1.4.3/lanQ.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/lanQ_rule/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-18 10:56:29.000000 lanQ-1.4.3/lanQ_rule/__init__.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/lanQ_rule/base_func/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 07:11:32.000000 lanQ-1.4.3/lanQ_rule/base_func/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     4593 2024-04-26 08:10:06.000000 lanQ-1.4.3/lanQ_rule/base_func/base.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)    15682 2024-05-09 02:36:54.000000 lanQ-1.4.3/lanQ_rule/common_rule.py
+drwxr-xr-x   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-05-09 02:37:48.803319 lanQ-1.4.3/lanQ_rule/config/
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)        0 2024-04-30 05:56:14.000000 lanQ-1.4.3/lanQ_rule/config/__init__.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     2294 2024-04-19 03:19:55.000000 lanQ-1.4.3/lanQ_rule/config/const.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      230 2024-04-30 03:33:52.000000 lanQ-1.4.3/lanQ_rule/config/customize.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1872 2024-05-06 06:02:00.000000 lanQ-1.4.3/lanQ_rule/config/rule_map.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      991 2024-04-30 03:33:53.000000 lanQ-1.4.3/lanQ_rule/model_rule.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)     1153 2024-04-24 03:44:27.000000 lanQ-1.4.3/lanQ_rule/prompt_rule.py
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)       38 2024-05-09 02:37:48.803319 lanQ-1.4.3/setup.cfg
+-rw-r--r--   0 PJLAB\shijin (409477266) PJLAB\domain^users (409469441)      394 2024-05-09 02:37:07.000000 lanQ-1.4.3/setup.py
```

### Comparing `lanQ-1.4.2/README.md` & `lanQ-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.2/lanQ_rule/base_func/base.py` & `lanQ-1.4.3/lanQ_rule/base_func/base.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.2/lanQ_rule/common_rule.py` & `lanQ-1.4.3/lanQ_rule/common_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,27 @@
             seg_list = jieba.cut(line, cut_all=True)
             for word in seg_list:
                 if len(word) == 1:
                     word_num += 1
             max_jieba_ratio = max(max_jieba_ratio, word_num / char_num)
     if max_jieba_ratio > cm.common_anti_crawler_zh['threshold']:
         res["error_status"] = True
-        res["error_type"][ERROR_CRAWL_ANTI] = ERROR_CRAWL_ANTI
-        res["error_reason"][ERROR_CRAWL_ANTI] = "包含反爬文本"
+        res["error_type"] = ERROR_CRAWL_ANTI
+        res["error_reason"] = "包含反爬文本"
     return res
 
 def common_bracket_unmatch(content: str) -> dict:
     """check whether bracket matches"""
     res = {'error_status': False}
     bracket_types = [("[", "]"), ("{", "}"), ("【", "】"), ("《", "》")]
     for open_bracket, close_bracket in bracket_types:
         if content.count(open_bracket) != content.count(close_bracket):
             res["error_status"] = True
-            res["error_type"][ERROR_BRACKET_UNMATCH] = ERROR_BRACKET_UNMATCH
-            res["error_reason"][ERROR_BRACKET_UNMATCH] = "括号数量不一致"
+            res["error_type"] = ERROR_BRACKET_UNMATCH
+            res["error_reason"] = "括号数量不一致"
     return res
 
 def common_chaos_en(content: str) -> dict:
     """check whether content has English messy code"""
     res = {'error_status': False}
     af_en = delete_punc_en(content)
     af_ch = delte_punc_ch(af_en)
@@ -171,16 +171,16 @@
 def common_emoj_characters(content: str) -> dict:
     """check whether content contains emoji charactors"""
     res = {'error_status': False}
     emoj_chars_pattern = r"U\+26[0-F][0-D]|U\+273[3-4]|U\+1F[3-6][0-4][0-F]|U\+1F6[8-F][0-F]"
     matches = re.search(emoj_chars_pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"][ERROR_EMOJ_CHAR] = ERROR_EMOJ_CHAR
-        res["error_reason"][ERROR_EMOJ_CHAR] = "包含emoji符号"
+        res["error_type"] = ERROR_EMOJ_CHAR
+        res["error_reason"] = "包含emoji符号"
     return res
 
 def common_enter_more(content: str) -> dict:
     """check whether content has more than 8 continious enter"""
     res = {'error_status': False}
     pattern = r'\n{8,}|\r{8,}'
     matches = re.findall(pattern, content)
@@ -259,16 +259,16 @@
 def common_invalid_web(content: str) -> dict:
     """check whether the content is invalid"""
     res = {'error_status': False}
     invalid_list = ["404 - Page not found\nThe requested page does not exist (or has been deleted).\nIf you typed a URL by hand, or used a bookmark, please double check the address that you used.\nIf you see this page, and the error persists, please contact Customer Care and provide details about the action you tried to perform."]
     for item in invalid_list:
         if item in content:
             res["error_status"] = True
-            res["error_type"][ERROR_INVALID_WEB] = ERROR_INVALID_WEB
-            res["error_reason"][ERROR_INVALID_WEB] = "content内容为404"
+            res["error_type"] = ERROR_INVALID_WEB
+            res["error_reason"] = "content内容为404"
     return res
 
 def common_invisible_char(content: str) -> dict:
     """check whether content has invisible char"""
     res = {'error_status': False}
     pattern = r"[\u2000-\u200F\u202F\u205F\u3000\uFEFF\u00A0\u2060-\u206F\uFEFF\xa0]"
     matches = re.findall(pattern, content)
@@ -281,16 +281,16 @@
 def common_joint_special_symbol(content: str) -> dict:
     """check if there are special symbols composed of multiple symbols spliced together"""
     res = {'error_status': False}
     pattern = r"&#247;|\? :"
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"][ERROR_JOINT_SPECIAL_SYMBOL] = ERROR_JOINT_SPECIAL_SYMBOL
-        res["error_reason"][ERROR_JOINT_SPECIAL_SYMBOL] = "包含多个符号拼接组成的特殊符号"
+        res["error_type"] = ERROR_JOINT_SPECIAL_SYMBOL
+        res["error_reason"] = "包含多个符号拼接组成的特殊符号"
     return res
 
 def common_language_mixed(content: str) -> dict:
     """check whether content is mixed in Chinese and English"""
     res = {'error_status': False}
     s = normalize(content)
     en_len = len(re.findall(r'[a-zA-Z]', s))
@@ -312,16 +312,16 @@
     "[A-Z0-9]{47}",  # 字母数字混合
     "[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{4}",  # 分段的字母数字混合
     "[A-Z0-9]{4}-\d{8}-[A-Z0-9]{4}"  # 含有特定信息的许可证密钥，例如产品ID和购买日期
     ])
     match = re.search(pattern, content, re.I)  # re.I使匹配对大小写不敏感
     if match:
         res["error_status"] = True
-        res["error_type"][ERROR_LICENSE_KEY] = ERROR_LICENSE_KEY
-        res["error_reason"][ERROR_LICENSE_KEY] = "包含license key"
+        res["error_type"] = ERROR_LICENSE_KEY
+        res["error_reason"] = "包含license key"
     return res
 
 def common_no_punc(content: str) -> dict:
     """check whether content has paragraph without punctuations"""
     res = {'error_status': False}
     paragraphs = content.split('\n')
     max_word_count = 0
@@ -365,27 +365,27 @@
 def common_special_mark(content: str) -> dict:
     """check if the content contains special mark"""
     res = {'error_status': False}
     pattern = r'keyboard_arrow_(left|right)'
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"][ERROR_SPECIAL_MARK] = ERROR_SPECIAL_MARK
-        res["error_reason"][ERROR_SPECIAL_MARK] = "元素包含特殊标记"
+        res["error_type"] = ERROR_SPECIAL_MARK
+        res["error_reason"] = "元素包含特殊标记"
     return res
 
 def common_unconverted_symbol(content: str) -> dict:
     """check if the content contains special symbols for conversion failure"""
     res = {'error_status': False}
     pattern = r'u200e'
     matches = re.findall(pattern, content)
     if matches:
         res["error_status"] = True
-        res["error_type"][ERROR_UNCONVERTED_SYMBOL] = ERROR_UNCONVERTED_SYMBOL
-        res["error_reason"][ERROR_UNCONVERTED_SYMBOL] = "包含转换失败的特殊符号"
+        res["error_type"] = ERROR_UNCONVERTED_SYMBOL
+        res["error_reason"] = "包含转换失败的特殊符号"
     return res
 
 def common_underscore_length(content: str) -> dict:
     """check whether the content contains underscores whose length is longer than 15"""
     res = {'error_status': False}
     max_underscore_count = 0
     for char in content:
@@ -393,16 +393,16 @@
             underscore_count += 1
             if underscore_count > max_underscore_count:
                 max_underscore_count = underscore_count
         else:
             underscore_count = 0
     if max_underscore_count >= 15:
         res["error_status"] = True
-        res["error_type"][ERROR_UNDERSCORE_LENGTH] = ERROR_UNDERSCORE_LENGTH
-        res["error_reason"][ERROR_UNDERSCORE_LENGTH] = "下划线长度大于15"
+        res["error_type"] = ERROR_UNDERSCORE_LENGTH
+        res["error_reason"] = "下划线长度大于15"
     return res
 
 def common_url_only(content: str) -> dict:
     """check whether content is all urls"""
     res = {'error_status': False}
     pattern = r'http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\\(\\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+'  # noqa
     s = re.sub(pattern, '', content)
```

### Comparing `lanQ-1.4.2/lanQ_rule/config/const.py` & `lanQ-1.4.3/lanQ_rule/config/const.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.2/lanQ_rule/model_rule.py` & `lanQ-1.4.3/lanQ_rule/model_rule.py`

 * *Files identical despite different names*

### Comparing `lanQ-1.4.2/lanQ_rule/prompt_rule.py` & `lanQ-1.4.3/lanQ_rule/prompt_rule.py`

 * *Files identical despite different names*


# Comparing `tmp/brazilfiscalreport-0.3.1.tar.gz` & `tmp/brazilfiscalreport-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brazilfiscalreport-0.3.1.tar", last modified: Mon May  6 23:10:10 2024, max compression
+gzip compressed data, was "brazilfiscalreport-0.3.2.tar", last modified: Wed May  8 13:30:53 2024, max compression
```

## Comparing `brazilfiscalreport-0.3.1.tar` & `brazilfiscalreport-0.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 23:10:10.000000 brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.755791 brazilfiscalreport-0.3.1/brazilfiscalreport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.755791 brazilfiscalreport-0.3.1/brazilfiscalreport/dacce/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/dacce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/dacce/dacce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    51511 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_basic_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_emit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_ident_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_verification_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/pdf_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/brazilfiscalreport/xfpdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:10.759791 brazilfiscalreport-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/test_dacce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/test_danfe.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-06 23:10:07.000000 brazilfiscalreport-0.3.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:53.633969 brazilfiscalreport-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:53.633969 brazilfiscalreport-0.3.2/BrazilFiscalReport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 13:30:53.000000 brazilfiscalreport-0.3.2/BrazilFiscalReport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-08 13:30:53.000000 brazilfiscalreport-0.3.2/BrazilFiscalReport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:30:53.000000 brazilfiscalreport-0.3.2/BrazilFiscalReport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 13:30:53.000000 brazilfiscalreport-0.3.2/BrazilFiscalReport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 13:30:53.000000 brazilfiscalreport-0.3.2/BrazilFiscalReport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-08 13:30:53.633969 brazilfiscalreport-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:53.629969 brazilfiscalreport-0.3.2/brazilfiscalreport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:53.629969 brazilfiscalreport-0.3.2/brazilfiscalreport/dacce/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/dacce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/dacce/dacce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:53.633969 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51511 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_basic_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_emit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_ident_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_verification_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/pdf_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/brazilfiscalreport/xfpdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:30:53.633969 brazilfiscalreport-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:53.633969 brazilfiscalreport-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/tests/test_dacce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/tests/test_danfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 13:30:46.000000 brazilfiscalreport-0.3.2/tests/test_utils.py
```

### Comparing `brazilfiscalreport-0.3.1/BrazilFiscalReport.egg-info/SOURCES.txt` & `brazilfiscalreport-0.3.2/BrazilFiscalReport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/LICENSE` & `brazilfiscalreport-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/README.md` & `brazilfiscalreport-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/dacce/dacce.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/dacce/dacce.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/config.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/config.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_basic_field.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_basic_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,13 +68,13 @@
             align = "C"
         else:
             pdf.set_font(pdf.default_font, "", FONT_SIZE_CONT)
             align = "R" if self.type == "number" else "L"
         self._content_lines = pdf.multi_cell(
             w=self.w,
             h=DEFAULT_HEIGHT_FONT_CONTENT,
-            text=self.content,
+            text=self.content or "",
             align=align,
             output=MethodReturnValue.LINES,
         )
         content_height = self.h - H_FONT_DESC
         self._max_content_lines = int(content_height // DEFAULT_HEIGHT_FONT_CONTENT)
```

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_block.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_block.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_code.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_code.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_emit_info.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_emit_info.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/danfe/danfe_ident_info.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/danfe/danfe_ident_info.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/pdf_element.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/pdf_element.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/utils.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/utils.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/brazilfiscalreport/xfpdf.py` & `brazilfiscalreport-0.3.2/brazilfiscalreport/xfpdf.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/tests/conftest.py` & `brazilfiscalreport-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/tests/test_dacce.py` & `brazilfiscalreport-0.3.2/tests/test_dacce.py`

 * *Files identical despite different names*

### Comparing `brazilfiscalreport-0.3.1/tests/test_danfe.py` & `brazilfiscalreport-0.3.2/tests/test_danfe.py`

 * *Files identical despite different names*


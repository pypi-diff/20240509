# Comparing `tmp/RiceXL-0.6.3.tar.gz` & `tmp/ricexl-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RiceXL-0.6.3.tar", last modified: Fri Jul 29 09:31:40 2022, max compression
+gzip compressed data, was "ricexl-0.6.4.tar", last modified: Thu May  9 03:23:47 2024, max compression
```

## Comparing `RiceXL-0.6.3.tar` & `ricexl-0.6.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-07-29 09:31:40.343030 RiceXL-0.6.3/
--rw-rw-rw-   0        0        0     1091 2021-12-01 11:11:28.000000 RiceXL-0.6.3/LICENSE
--rw-rw-rw-   0        0        0      793 2022-07-29 09:31:40.342054 RiceXL-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      133 2021-12-01 11:11:39.000000 RiceXL-0.6.3/README.md
--rw-rw-rw-   0        0        0       42 2022-07-29 09:31:40.343030 RiceXL-0.6.3/setup.cfg
--rw-rw-rw-   0        0        0      928 2022-07-29 09:28:14.000000 RiceXL-0.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-29 09:31:40.282186 RiceXL-0.6.3/src/
-drwxrwxrwx   0        0        0        0 2022-07-29 09:31:40.330057 RiceXL-0.6.3/src/RiceXL/
--rw-rw-rw-   0        0        0     2106 2021-11-29 06:29:58.000000 RiceXL-0.6.3/src/RiceXL/RiceAlignment.py
--rw-rw-rw-   0        0        0     8669 2021-12-01 11:43:00.000000 RiceXL-0.6.3/src/RiceXL/RiceBorder.py
--rw-rw-rw-   0        0        0    25278 2022-07-29 09:26:41.000000 RiceXL-0.6.3/src/RiceXL/RiceExcel.py
--rw-rw-rw-   0        0        0     4060 2021-12-01 11:43:29.000000 RiceXL-0.6.3/src/RiceXL/RiceFont.py
--rw-rw-rw-   0        0        0     2360 2021-12-01 11:43:43.000000 RiceXL-0.6.3/src/RiceXL/RicePattern.py
--rw-rw-rw-   0        0        0     3588 2022-04-02 06:52:30.000000 RiceXL-0.6.3/src/RiceXL/RiceUtils.py
--rw-rw-rw-   0        0        0      464 2021-12-01 11:52:00.000000 RiceXL-0.6.3/src/RiceXL/__init__.py
--rw-rw-rw-   0        0        0      220 2021-11-15 09:19:31.000000 RiceXL-0.6.3/src/RiceXL/xlutils_newcopy.py
-drwxrwxrwx   0        0        0        0 2022-07-29 09:31:40.340031 RiceXL-0.6.3/src/RiceXL.egg-info/
--rw-rw-rw-   0        0        0      793 2022-07-29 09:31:40.000000 RiceXL-0.6.3/src/RiceXL.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2022-07-29 09:31:40.000000 RiceXL-0.6.3/src/RiceXL.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-29 09:31:40.000000 RiceXL-0.6.3/src/RiceXL.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-07-29 09:31:40.000000 RiceXL-0.6.3/src/RiceXL.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 03:23:47.123609 ricexl-0.6.4/
+-rw-rw-rw-   0        0        0     1091 2021-12-01 11:11:28.000000 ricexl-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0      947 2024-05-09 03:23:47.120619 ricexl-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      133 2021-12-01 11:11:39.000000 ricexl-0.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 03:23:47.123609 ricexl-0.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-09 03:11:54.000000 ricexl-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 03:23:47.063770 ricexl-0.6.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 03:23:47.102665 ricexl-0.6.4/src/RiceXL/
+-rw-rw-rw-   0        0        0     2106 2021-11-29 06:29:58.000000 ricexl-0.6.4/src/RiceXL/RiceAlignment.py
+-rw-rw-rw-   0        0        0     8669 2021-12-01 11:43:00.000000 ricexl-0.6.4/src/RiceXL/RiceBorder.py
+-rw-rw-rw-   0        0        0    25405 2024-04-26 08:56:30.000000 ricexl-0.6.4/src/RiceXL/RiceExcel.py
+-rw-rw-rw-   0        0        0     4060 2021-12-01 11:43:29.000000 ricexl-0.6.4/src/RiceXL/RiceFont.py
+-rw-rw-rw-   0        0        0     2360 2021-12-01 11:43:43.000000 ricexl-0.6.4/src/RiceXL/RicePattern.py
+-rw-rw-rw-   0        0        0     3560 2022-08-01 01:38:41.000000 ricexl-0.6.4/src/RiceXL/RiceUtils.py
+-rw-rw-rw-   0        0        0      464 2021-12-01 11:52:00.000000 ricexl-0.6.4/src/RiceXL/__init__.py
+-rw-rw-rw-   0        0        0      220 2021-11-15 09:19:31.000000 ricexl-0.6.4/src/RiceXL/xlutils_newcopy.py
+drwxrwxrwx   0        0        0        0 2024-05-09 03:23:47.118624 ricexl-0.6.4/src/RiceXL.egg-info/
+-rw-rw-rw-   0        0        0      947 2024-05-09 03:23:47.000000 ricexl-0.6.4/src/RiceXL.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2024-05-09 03:23:47.000000 ricexl-0.6.4/src/RiceXL.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 03:23:47.000000 ricexl-0.6.4/src/RiceXL.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 03:23:47.000000 ricexl-0.6.4/src/RiceXL.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-09 03:23:47.000000 ricexl-0.6.4/src/RiceXL.egg-info/top_level.txt
```

### Comparing `RiceXL-0.6.3/LICENSE` & `ricexl-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `RiceXL-0.6.3/setup.py` & `ricexl-0.6.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="RiceXL",
-    version="0.6.3",
+    version="0.6.4",
     author="SNAKE",
     author_email="admin@wangbaishi.com",
     description="A tool for handling Excel easily. Handle both xls and xlsx in the same way.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wbsabc/RiceXL",
     project_urls={
@@ -19,9 +19,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
-    requires=['xlrd', 'xlwt', 'xlutils', 'openpyxl', 'os', 're', 'tempfile']
+    requires=['xlrd', 'xlwt', 'xlutils', 'openpyxl', 'os', 're', 'tempfile'],
+    install_requires=['xlrd', 'xlwt', 'xlutils', 'openpyxl', 'os', 're', 'tempfile']
 )
```

### Comparing `RiceXL-0.6.3/src/RiceXL/RiceAlignment.py` & `ricexl-0.6.4/src/RiceXL/RiceAlignment.py`

 * *Files identical despite different names*

### Comparing `RiceXL-0.6.3/src/RiceXL/RiceBorder.py` & `ricexl-0.6.4/src/RiceXL/RiceBorder.py`

 * *Files identical despite different names*

### Comparing `RiceXL-0.6.3/src/RiceXL/RiceExcel.py` & `ricexl-0.6.4/src/RiceXL/RiceExcel.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,19 +118,19 @@
     # Return sheet object
     def get_sheet(self, writable=False, sheet_name=None, sheet_index=None):
         if sheet_name is not None and sheet_index is not None:
             raise Exception('Cannot set sheet_index & sheet_name at the same time!')
         if writable:
             self.check_writable()
         if sheet_index is not None:
-            self.get_sheet_by_index(sheet_index, writable)
+            return self.get_sheet_by_index(sheet_index, writable)
         elif sheet_name is not None:
-            self.get_sheet_by_name(sheet_name, writable)
+            return self.get_sheet_by_name(sheet_name, writable)
         else:
-            self.get_current_sheet(writable)
+            return self.get_current_sheet(writable)
     
     # Return sheet object
     def get_sheet_by_index(self, sheet_index, writable=False):
         if writable:
             self.check_writable()
         if self.excel_version == 'xls':
             if writable:
@@ -222,20 +222,22 @@
         self.check_writable()
         if self.excel_version == 'xls':
             sheet_del = self.get_sheet(True, sheet_name)
             self.workbook_write._Workbook__worksheets.remove(sheet_del)
             self.handle_temp_file()
         elif self.excel_version == 'xlsx':
             sheet_del = self.get_sheet(True, sheet_name)
-            self.sheet = self.workbook.remove(sheet_del)
+            self.workbook.remove(sheet_del)
         if sheet_name == self.sheet_name:
             self.sheet_name = None
             self.sheet_index = None
             self.sheet = None
             self.sheet_write = None
+        elif self.sheet_name is not None:
+            self.set_sheet_by_name(self.sheet_name) # Update sheet index
 
     def get_active_sheet(self):
         if self.excel_version == 'xls':
             if self.writable:
                 return self.get_sheet(writable=True, sheet_index=self.workbook_write.active_sheet)
             else:
                 workbook_write = copy(self.workbook)
@@ -610,8 +612,8 @@
 
     def copy(self, pos_begin, pos_end):
         self.copied_values = self.get_values_matrix_in_area(pos_begin, pos_end)
     
     def paste(self, pos_begin):
         if self.copied_values is None:
             raise Exception('Have not copy any value!')
-        self.set_value_by_area(pos_begin, self.copied_values)
+        self.set_value_by_area(pos_begin, self.copied_values)
```

### Comparing `RiceXL-0.6.3/src/RiceXL/RiceFont.py` & `ricexl-0.6.4/src/RiceXL/RiceFont.py`

 * *Files identical despite different names*

### Comparing `RiceXL-0.6.3/src/RiceXL/RicePattern.py` & `ricexl-0.6.4/src/RiceXL/RicePattern.py`

 * *Files identical despite different names*

### Comparing `RiceXL-0.6.3/src/RiceXL/RiceUtils.py` & `ricexl-0.6.4/src/RiceXL/RiceUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from operator import index
 import re
 from openpyxl.styles.colors import COLOR_INDEX
 from openpyxl.utils import get_column_letter
 from openpyxl.utils import column_index_from_string
 
 def get_color_rgb(color):
     # Only support rgb
```


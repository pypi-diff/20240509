# Comparing `tmp/linuxdoc-20231020.tar.gz` & `tmp/linuxdoc-20240509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linuxdoc-20231020.tar", last modified: Fri Oct 20 10:28:36 2023, max compression
+gzip compressed data, was "linuxdoc-20240509.tar", last modified: Thu May  9 14:31:26 2024, max compression
```

## Comparing `linuxdoc-20231020.tar` & `linuxdoc-20240509.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-10-20 10:28:36.392590 linuxdoc-20231020/
--rw-rw-r--   0 markus   (10001) markus   (10001)    34520 2023-02-18 16:34:18.000000 linuxdoc-20231020/LICENSE
--rw-r--r--   0 markus   (10001) markus   (10001)     2305 2023-10-20 10:28:36.392590 linuxdoc-20231020/PKG-INFO
--rw-rw-r--   0 markus   (10001) markus   (10001)     1002 2023-10-20 10:26:10.000000 linuxdoc-20231020/README.rst
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-10-20 10:28:36.392590 linuxdoc-20231020/linuxdoc/
--rw-rw-r--   0 markus   (10001) markus   (10001)      777 2023-03-24 14:36:42.000000 linuxdoc-20231020/linuxdoc/__init__.py
--rw-rw-r--   0 markus   (10001) markus   (10001)     5819 2023-10-20 10:26:10.000000 linuxdoc-20231020/linuxdoc/__pkginfo__.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)     7200 2023-03-27 14:41:29.000000 linuxdoc-20231020/linuxdoc/autodoc.py
--rw-rw-r--   0 markus   (10001) markus   (10001)      560 2023-03-21 15:59:34.000000 linuxdoc-20231020/linuxdoc/cdomain.py
--rw-rw-r--   0 markus   (10001) markus   (10001)     5085 2023-03-21 15:59:38.000000 linuxdoc-20231020/linuxdoc/cdomainv2.py
--rw-rw-r--   0 markus   (10001) markus   (10001)      754 2023-03-24 14:36:42.000000 linuxdoc-20231020/linuxdoc/cdomainv3.py
--rw-rw-r--   0 markus   (10001) markus   (10001)     1734 2023-03-27 11:18:15.000000 linuxdoc-20231020/linuxdoc/compat.py
--rw-rw-r--   0 markus   (10001) markus   (10001)     1701 2023-10-01 16:14:06.000000 linuxdoc-20231020/linuxdoc/deprecated.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)     2016 2023-03-27 09:59:21.000000 linuxdoc-20231020/linuxdoc/grepdoc.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)   110357 2023-10-01 16:14:06.000000 linuxdoc-20231020/linuxdoc/kernel_doc.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)     7949 2023-03-24 14:36:42.000000 linuxdoc-20231020/linuxdoc/kernel_include.py
--rw-rw-r--   0 markus   (10001) markus   (10001)    17255 2023-10-01 16:14:06.000000 linuxdoc-20231020/linuxdoc/kfigure.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)     3321 2023-03-27 09:59:21.000000 linuxdoc-20231020/linuxdoc/lint.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)    13347 2023-03-21 16:01:21.000000 linuxdoc-20231020/linuxdoc/manKernelDoc.py
--rw-rw-r--   0 markus   (10001) markus   (10001)     6418 2023-10-01 16:14:06.000000 linuxdoc-20231020/linuxdoc/rest.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)    12757 2023-03-21 16:01:38.000000 linuxdoc-20231020/linuxdoc/rstFlatTable.py
--rwxrwxr-x   0 markus   (10001) markus   (10001)    18769 2023-03-21 16:01:49.000000 linuxdoc-20231020/linuxdoc/rstKernelDoc.py
-drwxrwxr-x   0 markus   (10001) markus   (10001)        0 2023-10-20 10:28:36.392590 linuxdoc-20231020/linuxdoc.egg-info/
--rw-r--r--   0 markus   (10001) markus   (10001)     2305 2023-10-20 10:28:36.000000 linuxdoc-20231020/linuxdoc.egg-info/PKG-INFO
--rw-rw-r--   0 markus   (10001) markus   (10001)      601 2023-10-20 10:28:36.000000 linuxdoc-20231020/linuxdoc.egg-info/SOURCES.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)        1 2023-10-20 10:28:36.000000 linuxdoc-20231020/linuxdoc.egg-info/dependency_links.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)      389 2023-10-20 10:28:36.000000 linuxdoc-20231020/linuxdoc.egg-info/entry_points.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)       34 2023-10-20 10:28:36.000000 linuxdoc-20231020/linuxdoc.egg-info/requires.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)        9 2023-10-20 10:28:36.000000 linuxdoc-20231020/linuxdoc.egg-info/top_level.txt
--rw-rw-r--   0 markus   (10001) markus   (10001)       61 2023-10-20 10:28:36.392590 linuxdoc-20231020/setup.cfg
--rwxrwxr-x   0 markus   (10001) markus   (10001)     1521 2023-10-20 10:25:23.000000 linuxdoc-20231020/setup.py
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2024-05-09 14:31:26.805099 linuxdoc-20240509/
+-rw-rw-r--   0 markus    (1001) markus    (1001)    34520 2023-03-25 08:10:56.000000 linuxdoc-20240509/LICENSE
+-rw-r--r--   0 markus    (1001) markus    (1001)     2305 2024-05-09 14:31:26.805099 linuxdoc-20240509/PKG-INFO
+-rw-rw-r--   0 markus    (1001) markus    (1001)     1002 2024-05-09 14:00:22.000000 linuxdoc-20240509/README.rst
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2024-05-09 14:31:26.801099 linuxdoc-20240509/linuxdoc/
+-rw-rw-r--   0 markus    (1001) markus    (1001)      777 2023-03-25 08:10:56.000000 linuxdoc-20240509/linuxdoc/__init__.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     5819 2024-05-09 13:58:09.000000 linuxdoc-20240509/linuxdoc/__pkginfo__.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     7200 2023-03-26 12:51:46.000000 linuxdoc-20240509/linuxdoc/autodoc.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)      560 2023-03-25 08:10:56.000000 linuxdoc-20240509/linuxdoc/cdomain.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     5085 2023-03-25 08:10:56.000000 linuxdoc-20240509/linuxdoc/cdomainv2.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)      754 2023-03-25 08:10:56.000000 linuxdoc-20240509/linuxdoc/cdomainv3.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     1734 2023-03-25 08:10:56.000000 linuxdoc-20240509/linuxdoc/compat.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     1701 2023-05-06 08:23:40.000000 linuxdoc-20240509/linuxdoc/deprecated.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     2016 2023-03-26 12:51:46.000000 linuxdoc-20240509/linuxdoc/grepdoc.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)   110357 2023-05-06 07:53:06.000000 linuxdoc-20240509/linuxdoc/kernel_doc.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     7790 2024-05-09 13:56:17.000000 linuxdoc-20240509/linuxdoc/kernel_include.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)    17255 2023-08-27 12:56:57.000000 linuxdoc-20240509/linuxdoc/kfigure.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     3321 2023-03-26 12:51:46.000000 linuxdoc-20240509/linuxdoc/lint.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)    13347 2023-03-25 08:10:56.000000 linuxdoc-20240509/linuxdoc/manKernelDoc.py
+-rw-rw-r--   0 markus    (1001) markus    (1001)     6418 2024-01-20 17:31:13.000000 linuxdoc-20240509/linuxdoc/rest.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)    12757 2024-01-21 14:46:08.000000 linuxdoc-20240509/linuxdoc/rstFlatTable.py
+-rwxrwxr-x   0 markus    (1001) markus    (1001)    18769 2023-03-25 08:10:56.000000 linuxdoc-20240509/linuxdoc/rstKernelDoc.py
+drwxrwxr-x   0 markus    (1001) markus    (1001)        0 2024-05-09 14:31:26.805099 linuxdoc-20240509/linuxdoc.egg-info/
+-rw-r--r--   0 markus    (1001) markus    (1001)     2305 2024-05-09 14:31:26.000000 linuxdoc-20240509/linuxdoc.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1001) markus    (1001)      601 2024-05-09 14:31:26.000000 linuxdoc-20240509/linuxdoc.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)        1 2024-05-09 14:31:26.000000 linuxdoc-20240509/linuxdoc.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)      389 2024-05-09 14:31:26.000000 linuxdoc-20240509/linuxdoc.egg-info/entry_points.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)       34 2024-05-09 14:31:26.000000 linuxdoc-20240509/linuxdoc.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)        9 2024-05-09 14:31:26.000000 linuxdoc-20240509/linuxdoc.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1001) markus    (1001)       61 2024-05-09 14:31:26.805099 linuxdoc-20240509/setup.cfg
+-rwxrwxr-x   0 markus    (1001) markus    (1001)     1521 2024-01-20 07:47:16.000000 linuxdoc-20240509/setup.py
```

### Comparing `linuxdoc-20231020/LICENSE` & `linuxdoc-20240509/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/PKG-INFO` & `linuxdoc-20240509/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxdoc
-Version: 20231020
+Version: 20240509
 Summary: Sphinx-doc extensions & tools to extract documentation from C/C++ source file comments.
 Home-page: https://github.com/return42/linuxdoc
 Author: Markus Heiser
 Author-email: markus.heiser@darmarIT.de
 License: AGPLv3+
 Project-URL: Documentation, https://return42.github.io/linuxdoc
 Project-URL: Code, https://github.com/return42/linuxdoc
@@ -55,13 +55,13 @@
 - Documentation:   https://return42.github.io/linuxdoc
 - Releases:        https://pypi.org/project/linuxdoc/
 - Code:            https://github.com/return42/linuxdoc
 - Issue tracker:   https://github.com/return42/linuxdoc/issues
 
 
 ============ ===============================================
-package:     linuxdoc (20231020)
+package:     linuxdoc (20240509)
 copyright:   2023 Markus Heiser
 e-mail:      markus.heiser@darmarIT.de
 license:     AGPLv3+
 ============ ===============================================
```

### Comparing `linuxdoc-20231020/README.rst` & `linuxdoc-20240509/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -25,13 +25,13 @@
 - Documentation:   https://return42.github.io/linuxdoc
 - Releases:        https://pypi.org/project/linuxdoc/
 - Code:            https://github.com/return42/linuxdoc
 - Issue tracker:   https://github.com/return42/linuxdoc/issues
 
 
 ============ ===============================================
-package:     linuxdoc (20231020)
+package:     linuxdoc (20240509)
 copyright:   2023 Markus Heiser
 e-mail:      markus.heiser@darmarIT.de
 license:     AGPLv3+
 ============ ===============================================
```

### Comparing `linuxdoc-20231020/linuxdoc/__init__.py` & `linuxdoc-20240509/linuxdoc/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/__pkginfo__.py` & `linuxdoc-20240509/linuxdoc/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # pylint: disable=line-too-long, invalid-name, consider-using-f-string
 """Python package meta informations used by setup.py and other project files.
 """
 
 from setuptools import find_packages
 
 package = 'linuxdoc'
-version = '20231020'
+version = '20240509'
 
-copyright = '2023 Markus Heiser'  # pylint: disable=redefined-builtin
+copyright = '2024 Markus Heiser'  # pylint: disable=redefined-builtin
 description = (
     'Sphinx-doc extensions & tools to extract documentation'
     ' from C/C++ source file comments.'
 )
 license   = 'AGPLv3+'  # pylint: disable=redefined-builtin
 keywords = 'sphinx extension doc source code comments kernel-doc linux'
```

### Comparing `linuxdoc-20231020/linuxdoc/autodoc.py` & `linuxdoc-20240509/linuxdoc/autodoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/cdomain.py` & `linuxdoc-20240509/linuxdoc/cdomain.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/cdomainv2.py` & `linuxdoc-20240509/linuxdoc/cdomainv2.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/cdomainv3.py` & `linuxdoc-20240509/linuxdoc/cdomainv3.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/compat.py` & `linuxdoc-20240509/linuxdoc/compat.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/deprecated.py` & `linuxdoc-20240509/linuxdoc/deprecated.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/grepdoc.py` & `linuxdoc-20240509/linuxdoc/grepdoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/kernel_doc.py` & `linuxdoc-20240509/linuxdoc/kernel_doc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/kernel_include.py` & `linuxdoc-20240509/linuxdoc/kernel_include.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,14 @@
             self.lineno - self.state_machine.input_offset - 1)
         source_dir = os.path.dirname(os.path.abspath(source))
         path = directives.path(self.arguments[0])
         if path.startswith('<') and path.endswith('>'):
             path = os.path.join(self.standard_include_path, path[1:-1])
         path = os.path.normpath(os.path.join(source_dir, path))
 
-        # HINT: this is the only line I had to change / commented out:
-        #path = utils.relative_path(None, path)
-
-        path = nodes.reprunicode(path)
         encoding = self.options.get(
             'encoding', self.state.document.settings.input_encoding)
         e_handler=self.state.document.settings.input_encoding_error_handler
         tab_width = self.options.get(
             'tab-width', self.state.document.settings.tab_width)
         try:
             self.state.document.settings.record_dependencies.add(path)
```

### Comparing `linuxdoc-20231020/linuxdoc/kfigure.py` & `linuxdoc-20240509/linuxdoc/kfigure.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/lint.py` & `linuxdoc-20240509/linuxdoc/lint.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/manKernelDoc.py` & `linuxdoc-20240509/linuxdoc/manKernelDoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/rest.py` & `linuxdoc-20240509/linuxdoc/rest.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/rstFlatTable.py` & `linuxdoc-20240509/linuxdoc/rstFlatTable.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc/rstKernelDoc.py` & `linuxdoc-20240509/linuxdoc/rstKernelDoc.py`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/linuxdoc.egg-info/PKG-INFO` & `linuxdoc-20240509/linuxdoc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxdoc
-Version: 20231020
+Version: 20240509
 Summary: Sphinx-doc extensions & tools to extract documentation from C/C++ source file comments.
 Home-page: https://github.com/return42/linuxdoc
 Author: Markus Heiser
 Author-email: markus.heiser@darmarIT.de
 License: AGPLv3+
 Project-URL: Documentation, https://return42.github.io/linuxdoc
 Project-URL: Code, https://github.com/return42/linuxdoc
@@ -55,13 +55,13 @@
 - Documentation:   https://return42.github.io/linuxdoc
 - Releases:        https://pypi.org/project/linuxdoc/
 - Code:            https://github.com/return42/linuxdoc
 - Issue tracker:   https://github.com/return42/linuxdoc/issues
 
 
 ============ ===============================================
-package:     linuxdoc (20231020)
+package:     linuxdoc (20240509)
 copyright:   2023 Markus Heiser
 e-mail:      markus.heiser@darmarIT.de
 license:     AGPLv3+
 ============ ===============================================
```

### Comparing `linuxdoc-20231020/linuxdoc.egg-info/SOURCES.txt` & `linuxdoc-20240509/linuxdoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linuxdoc-20231020/setup.py` & `linuxdoc-20240509/setup.py`

 * *Files identical despite different names*


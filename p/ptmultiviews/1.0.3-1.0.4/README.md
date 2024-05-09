# Comparing `tmp/ptmultiviews-1.0.3.tar.gz` & `tmp/ptmultiviews-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmultiviews-1.0.3.tar", last modified: Mon May  6 19:27:58 2024, max compression
+gzip compressed data, was "ptmultiviews-1.0.4.tar", last modified: Thu May  9 11:09:49 2024, max compression
```

## Comparing `ptmultiviews-1.0.3.tar` & `ptmultiviews-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-29 08:26:15.000000 ptmultiviews-1.0.3/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     3596 2024-05-06 19:22:48.000000 ptmultiviews-1.0.3/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/ptmultiviews/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:15.000000 ptmultiviews-1.0.3/ptmultiviews/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-04-29 08:26:15.000000 ptmultiviews-1.0.3/ptmultiviews/_version.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15479 2024-05-06 14:04:14.000000 ptmultiviews-1.0.3/ptmultiviews/ptmultiviews.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/ptmultiviews.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      323 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       64 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-06 19:27:58.000000 ptmultiviews-1.0.3/ptmultiviews.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-06 19:27:58.686684 ptmultiviews-1.0.3/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1255 2024-05-06 19:27:44.000000 ptmultiviews-1.0.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-29 08:26:15.000000 ptmultiviews-1.0.4/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     3596 2024-05-09 09:38:41.000000 ptmultiviews-1.0.4/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/ptmultiviews/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:15.000000 ptmultiviews-1.0.4/ptmultiviews/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-09 11:04:18.000000 ptmultiviews-1.0.4/ptmultiviews/_version.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    15483 2024-05-09 09:38:41.000000 ptmultiviews-1.0.4/ptmultiviews/ptmultiviews.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/ptmultiviews.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      323 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       64 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1254 2024-05-09 10:21:25.000000 ptmultiviews-1.0.4/setup.py
```

### Comparing `ptmultiviews-1.0.3/LICENSE` & `ptmultiviews-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ptmultiviews-1.0.3/PKG-INFO` & `ptmultiviews-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmultiviews
-Version: 1.0.3
+Version: 1.0.4
 Summary: Apache Multiviews Detection & Enumeration Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptmultiviews
```

### Comparing `ptmultiviews-1.0.3/README.md` & `ptmultiviews-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ptmultiviews-1.0.3/ptmultiviews/ptmultiviews.py` & `ptmultiviews-1.0.4/ptmultiviews/ptmultiviews.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                 rel_path = f"{url.split('/', 3)[-1]}/{found_file}"
                 if abs_path == original_url and not self.with_requested_url:
                     continue
                 path = abs_path if not self.without_domain else rel_path
                 if path not in self.result_path_list:
                     self.result_path_list.append(path)
                     if self.use_json:
-                        self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webpage", properties={"url": abs_path, "name": found_file, "WebPageType": self.ptpathtypedetector.get_type(path)}))
+                        self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webSource", properties={"url": abs_path, "name": found_file, "WebSourceType": self.ptpathtypedetector.get_type(path)}))
 
     def _strip_url_extension(self, url: str) -> str:
         parsed = urllib.parse.urlparse(url)
         path = parsed.path.rsplit("/", 1)
         if "." in path[-1]:
             new_path = f"{path[0]}/{path[-1].split('.', 1)[0]}"
             parsed = parsed._replace(path=new_path)
```

### Comparing `ptmultiviews-1.0.3/ptmultiviews.egg-info/PKG-INFO` & `ptmultiviews-1.0.4/ptmultiviews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmultiviews
-Version: 1.0.3
+Version: 1.0.4
 Summary: Apache Multiviews Detection & Enumeration Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptmultiviews
```

### Comparing `ptmultiviews-1.0.3/setup.py` & `ptmultiviews-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     license="GPLv3",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: Implementation :: CPython",
         "Environment :: Console",
         "Topic :: Security",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
     ],
     python_requires='>=3.9',
     install_requires=["ptlibs>=1.0.7,<2"],
     entry_points = {'console_scripts': ['ptmultiviews = ptmultiviews.ptmultiviews:main']},
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls = {
```


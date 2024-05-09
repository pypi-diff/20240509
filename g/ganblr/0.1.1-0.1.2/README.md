# Comparing `tmp/ganblr-0.1.1.tar.gz` & `tmp/ganblr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ganblr-0.1.1.tar", last modified: Wed Dec 14 17:27:10 2022, max compression
+gzip compressed data, was "ganblr-0.1.2.tar", last modified: Thu May  9 02:49:57 2024, max compression
```

## Comparing `ganblr-0.1.1.tar` & `ganblr-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-12-14 17:27:10.504851 ganblr-0.1.1/
--rw-rw-rw-   0        0        0     1099 2022-11-15 11:32:18.000000 ganblr-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     4309 2022-12-14 17:27:10.504851 ganblr-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3826 2022-12-14 17:22:32.000000 ganblr-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-14 17:27:10.492840 ganblr-0.1.1/ganblr/
--rw-rw-rw-   0        0        0      281 2022-12-14 17:19:32.000000 ganblr-0.1.1/ganblr/__init__.py
--rw-rw-rw-   0        0        0    12681 2022-12-14 17:18:53.000000 ganblr-0.1.1/ganblr/kdb.py
-drwxrwxrwx   0        0        0        0 2022-12-14 17:27:10.502849 ganblr-0.1.1/ganblr/models/
--rw-rw-rw-   0        0        0      120 2022-12-14 17:18:53.000000 ganblr-0.1.1/ganblr/models/__init__.py
--rw-rw-rw-   0        0        0    10654 2022-12-14 17:18:53.000000 ganblr-0.1.1/ganblr/models/ganblr.py
--rw-rw-rw-   0        0        0    12395 2022-12-14 17:18:53.000000 ganblr-0.1.1/ganblr/models/ganblrpp.py
--rw-rw-rw-   0        0        0     5255 2022-12-14 17:18:53.000000 ganblr-0.1.1/ganblr/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-14 17:27:10.500848 ganblr-0.1.1/ganblr.egg-info/
--rw-rw-rw-   0        0        0     4309 2022-12-14 17:27:10.000000 ganblr-0.1.1/ganblr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2022-12-14 17:27:10.000000 ganblr-0.1.1/ganblr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-14 17:27:10.000000 ganblr-0.1.1/ganblr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2022-12-14 17:27:10.000000 ganblr-0.1.1/ganblr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-14 17:27:10.000000 ganblr-0.1.1/ganblr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-14 17:27:10.504851 ganblr-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1089 2022-12-14 17:19:46.000000 ganblr-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:57.061464 ganblr-0.1.2/
+-rw-rw-rw-   0        0        0     1099 2022-11-15 11:32:18.000000 ganblr-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     4309 2024-05-09 02:49:57.060963 ganblr-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3826 2024-05-09 02:37:42.000000 ganblr-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:57.044449 ganblr-0.1.2/ganblr/
+-rw-rw-rw-   0        0        0      281 2024-05-09 02:39:42.000000 ganblr-0.1.2/ganblr/__init__.py
+-rw-rw-rw-   0        0        0    12681 2024-05-03 06:06:11.000000 ganblr-0.1.2/ganblr/kdb.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:57.059462 ganblr-0.1.2/ganblr/models/
+-rw-rw-rw-   0        0        0      167 2024-05-09 02:39:42.000000 ganblr-0.1.2/ganblr/models/__init__.py
+-rw-rw-rw-   0        0        0    10654 2024-05-03 06:06:11.000000 ganblr-0.1.2/ganblr/models/ganblr.py
+-rw-rw-rw-   0        0        0    12100 2024-05-09 02:39:42.000000 ganblr-0.1.2/ganblr/models/ganblrmug.py
+-rw-rw-rw-   0        0        0    12395 2022-12-14 17:18:53.000000 ganblr-0.1.2/ganblr/models/ganblrpp.py
+-rw-rw-rw-   0        0        0     5255 2024-05-03 06:06:11.000000 ganblr-0.1.2/ganblr/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:49:57.052456 ganblr-0.1.2/ganblr.egg-info/
+-rw-rw-rw-   0        0        0     4309 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-09 02:49:56.000000 ganblr-0.1.2/ganblr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 02:49:57.061965 ganblr-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1089 2024-05-09 02:39:42.000000 ganblr-0.1.2/setup.py
```

### Comparing `ganblr-0.1.1/LICENSE` & `ganblr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.1/PKG-INFO` & `ganblr-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ganblr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ganblr Toolbox
 Home-page: https://github.com/tulip-lab/ganblr
 Author: kae zhou
 Author-email: kaezhou@gmail.com
 License: MIT Licence
 Keywords: ganblr,tulip
 Platform: any
@@ -20,15 +20,15 @@
 GANBLR Toolbox contains GANBLR models proposed by `Tulip Lab` for tabular data generation, which can sample fully artificial data from real data.
 
 Currently, this package contains following GANBLR models:
 
 - GANBLR
 - GANBLR++
 
-For a quick start, you can check out this usage example in Google Colab. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1w7A26JRkrXPeeA9q1Kbi_CRjbptkr8Ls?usp=sharing]
+For a quick start, you can check out this usage example in Google Colab. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1w7A26JRkrXPeeA9q1Kbi_CRjbptkr8Ls?usp=sharing)
 
 # Install
 
 We recommend you to install ganblr through pip:
 
 ```bash
 pip install ganblr
```

### Comparing `ganblr-0.1.1/README.md` & `ganblr-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 GANBLR Toolbox contains GANBLR models proposed by `Tulip Lab` for tabular data generation, which can sample fully artificial data from real data.
 
 Currently, this package contains following GANBLR models:
 
 - GANBLR
 - GANBLR++
 
-For a quick start, you can check out this usage example in Google Colab. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1w7A26JRkrXPeeA9q1Kbi_CRjbptkr8Ls?usp=sharing]
+For a quick start, you can check out this usage example in Google Colab. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1w7A26JRkrXPeeA9q1Kbi_CRjbptkr8Ls?usp=sharing)
 
 # Install
 
 We recommend you to install ganblr through pip:
 
 ```bash
 pip install ganblr
```

### Comparing `ganblr-0.1.1/ganblr/kdb.py` & `ganblr-0.1.2/ganblr/kdb.py`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.1/ganblr/models/ganblr.py` & `ganblr-0.1.2/ganblr/models/ganblr.py`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.1/ganblr/models/ganblrpp.py` & `ganblr-0.1.2/ganblr/models/ganblrpp.py`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.1/ganblr/utils.py` & `ganblr-0.1.2/ganblr/utils.py`

 * *Files identical despite different names*

### Comparing `ganblr-0.1.1/ganblr.egg-info/PKG-INFO` & `ganblr-0.1.2/ganblr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ganblr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Ganblr Toolbox
 Home-page: https://github.com/tulip-lab/ganblr
 Author: kae zhou
 Author-email: kaezhou@gmail.com
 License: MIT Licence
 Keywords: ganblr,tulip
 Platform: any
@@ -20,15 +20,15 @@
 GANBLR Toolbox contains GANBLR models proposed by `Tulip Lab` for tabular data generation, which can sample fully artificial data from real data.
 
 Currently, this package contains following GANBLR models:
 
 - GANBLR
 - GANBLR++
 
-For a quick start, you can check out this usage example in Google Colab. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1w7A26JRkrXPeeA9q1Kbi_CRjbptkr8Ls?usp=sharing]
+For a quick start, you can check out this usage example in Google Colab. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1w7A26JRkrXPeeA9q1Kbi_CRjbptkr8Ls?usp=sharing)
 
 # Install
 
 We recommend you to install ganblr through pip:
 
 ```bash
 pip install ganblr
```

### Comparing `ganblr-0.1.1/setup.py` & `ganblr-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   with open(os.path.join(path, 'README.md')) as f:
     long_description = f.read()
 except Exception as e:
   long_description = "Ganblr Toolbox"
 
 setup(
     name = "ganblr",
-    version = "0.1.1",
+    version = "0.1.2",
     keywords = ["ganblr", "tulip"],
     description = "Ganblr Toolbox",
     long_description = long_description,
     long_description_content_type='text/markdown',
     python_requires=">=3.5.0",
     license = "MIT Licence",
```


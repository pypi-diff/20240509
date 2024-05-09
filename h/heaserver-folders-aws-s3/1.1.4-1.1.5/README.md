# Comparing `tmp/heaserver_folders_aws_s3-1.1.4.tar.gz` & `tmp/heaserver_folders_aws_s3-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_folders_aws_s3-1.1.4.tar", last modified: Tue May  7 21:46:19 2024, max compression
+gzip compressed data, was "heaserver_folders_aws_s3-1.1.5.tar", last modified: Thu May  9 16:26:17 2024, max compression
```

## Comparing `heaserver_folders_aws_s3-1.1.4.tar` & `heaserver_folders_aws_s3-1.1.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.704315 heaserver_folders_aws_s3-1.1.4/
--rw-rw-rw-   0        0        0      261 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.4/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.4/.gitignore
--rw-rw-rw-   0        0        0     1664 2024-05-07 21:12:58.000000 heaserver_folders_aws_s3-1.1.4/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      272 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6721 2024-05-07 21:46:19.703314 heaserver_folders_aws_s3-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5479 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.4/README.md
--rw-rw-rw-   0        0        0     1777 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.4/RELEASING.md
--rw-rw-rw-   0        0        0      658 2024-05-07 21:12:58.000000 heaserver_folders_aws_s3-1.1.4/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.561853 heaserver_folders_aws_s3-1.1.4/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.561853 heaserver_folders_aws_s3-1.1.4/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.627529 heaserver_folders_aws_s3-1.1.4/integrationtests/heaserver/folderawss3integrationtest/
--rw-rw-rw-   0        0        0        0 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.4/integrationtests/heaserver/folderawss3integrationtest/__init__.py
--rw-rw-rw-   0        0        0    38201 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.4/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
--rw-rw-rw-   0        0        0    40185 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.4/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
--rw-rw-rw-   0        0        0    30533 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.4/integrationtests/heaserver/folderawss3integrationtest/test_all.py
--rw-rw-rw-   0        0        0      111 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.4/pytest.ini
--rw-rw-rw-   0        0        0      261 2023-11-06 17:01:54.000000 heaserver_folders_aws_s3-1.1.4/requirements_dev.txt
--rw-rw-rw-   0        0        0    14460 2024-03-11 17:23:33.000000 heaserver_folders_aws_s3-1.1.4/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-07 21:46:19.704315 heaserver_folders_aws_s3-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2473 2024-05-07 21:45:14.000000 heaserver_folders_aws_s3-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.563852 heaserver_folders_aws_s3-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.562852 heaserver_folders_aws_s3-1.1.4/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.654643 heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/
--rw-rw-rw-   0        0        0        0 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/__init__.py
--rw-rw-rw-   0        0        0   154476 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/projectservice.py
--rw-rw-rw-   0        0        0   157027 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/service.py
--rw-rw-rw-   0        0        0     8385 2024-02-08 15:54:03.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/util.py
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.659644 heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/wstl/
--rw-rw-rw-   0        0        0    33203 2024-05-07 21:19:48.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.702313 heaserver_folders_aws_s3-1.1.4/src/heaserver_folders_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     6721 2024-05-07 21:46:19.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1196 2024-05-07 21:46:19.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 21:46:19.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-07 21:46:19.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 21:46:19.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver_folders_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 21:46:19.000000 heaserver_folders_aws_s3-1.1.4/src/heaserver_folders_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.563852 heaserver_folders_aws_s3-1.1.4/tests/
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.563852 heaserver_folders_aws_s3-1.1.4/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.695313 heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/
--rw-rw-rw-   0        0        0        0 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/__init__.py
--rw-rw-rw-   0        0        0    37459 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/folderawss3testcase.py
--rw-rw-rw-   0        0        0    38816 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/projectawss3testcase.py
--rw-rw-rw-   0        0        0     2608 2023-12-12 15:20:12.000000 heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/test_all.py
-drwxrwxrwx   0        0        0        0 2024-05-07 21:46:19.701320 heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/wstl/
--rw-rw-rw-   0        0        0    14496 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.219562 heaserver_folders_aws_s3-1.1.5/
+-rw-rw-rw-   0        0        0      261 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/.gitignore
+-rw-rw-rw-   0        0        0     1664 2024-05-07 21:12:58.000000 heaserver_folders_aws_s3-1.1.5/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6721 2024-05-09 16:26:17.218563 heaserver_folders_aws_s3-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5479 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/README.md
+-rw-rw-rw-   0        0        0     1777 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/RELEASING.md
+-rw-rw-rw-   0        0        0      658 2024-05-07 21:12:58.000000 heaserver_folders_aws_s3-1.1.5/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.053485 heaserver_folders_aws_s3-1.1.5/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.053485 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.128491 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/
+-rw-rw-rw-   0        0        0        0 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/__init__.py
+-rw-rw-rw-   0        0        0    38201 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    40185 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
+-rw-rw-rw-   0        0        0    30533 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/test_all.py
+-rw-rw-rw-   0        0        0      111 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/pytest.ini
+-rw-rw-rw-   0        0        0      261 2023-11-06 17:01:54.000000 heaserver_folders_aws_s3-1.1.5/requirements_dev.txt
+-rw-rw-rw-   0        0        0    14460 2024-03-11 17:23:33.000000 heaserver_folders_aws_s3-1.1.5/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 16:26:17.219562 heaserver_folders_aws_s3-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2473 2024-05-09 16:17:34.000000 heaserver_folders_aws_s3-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.055485 heaserver_folders_aws_s3-1.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.054485 heaserver_folders_aws_s3-1.1.5/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.158487 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/
+-rw-rw-rw-   0        0        0        0 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/__init__.py
+-rw-rw-rw-   0        0        0   154476 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/projectservice.py
+-rw-rw-rw-   0        0        0   157027 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/service.py
+-rw-rw-rw-   0        0        0     8385 2024-02-08 15:54:03.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.164492 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/wstl/
+-rw-rw-rw-   0        0        0    33202 2024-05-08 14:18:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.217562 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     6721 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1196 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.055485 heaserver_folders_aws_s3-1.1.5/tests/
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.055485 heaserver_folders_aws_s3-1.1.5/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.209568 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/
+-rw-rw-rw-   0        0        0        0 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/__init__.py
+-rw-rw-rw-   0        0        0    37459 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    38816 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/projectawss3testcase.py
+-rw-rw-rw-   0        0        0     2608 2023-12-12 15:20:12.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.216562 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/wstl/
+-rw-rw-rw-   0        0        0    14496 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/wstl/all.json
```

### Comparing `heaserver_folders_aws_s3-1.1.4/Dockerfile` & `heaserver_folders_aws_s3-1.1.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/LICENSE` & `heaserver_folders_aws_s3-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/PKG-INFO` & `heaserver_folders_aws_s3-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.1.4
+Version: 1.1.5
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `heaserver_folders_aws_s3-1.1.4/README.md` & `heaserver_folders_aws_s3-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/RELEASING.md` & `heaserver_folders_aws_s3-1.1.5/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/docker-entrypoint.sh` & `heaserver_folders_aws_s3-1.1.5/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py` & `heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py` & `heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/integrationtests/heaserver/folderawss3integrationtest/test_all.py` & `heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/run-swaggerui.py` & `heaserver_folders_aws_s3-1.1.5/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/setup.py` & `heaserver_folders_aws_s3-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaserver-folders-aws-s3',
-                 version='1.1.4',
+                 version='1.1.5',
                  description='The HEA AWS S3 bucket folder service.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/projectservice.py` & `heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/projectservice.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/service.py` & `heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/service.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/util.py` & `heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/util.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/src/heaserver/folderawss3/wstl/all.json` & `heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/wstl/all.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999925595238095%*

 * *Differences: {"'wstl'": "{'actions': {49: {'inputs': {1: {'required': True}}}}}"}*

```diff
@@ -909,15 +909,15 @@
                         ],
                         "type": "select",
                         "value": "Standard"
                     },
                     {
                         "name": "days",
                         "prompt": "Restore duration",
-                        "required": false,
+                        "required": true,
                         "suggest": [
                             {
                                 "text": "1 day",
                                 "value": "1"
                             },
                             {
                                 "text": "3 days",
```

### Comparing `heaserver_folders_aws_s3-1.1.4/src/heaserver_folders_aws_s3.egg-info/PKG-INFO` & `heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.1.4
+Version: 1.1.5
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `heaserver_folders_aws_s3-1.1.4/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt` & `heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/folderawss3testcase.py` & `heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/folderawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/projectawss3testcase.py` & `heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/projectawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/test_all.py` & `heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.4/tests/heaserver/folderawss3test/wstl/all.json` & `heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/wstl/all.json`

 * *Files identical despite different names*


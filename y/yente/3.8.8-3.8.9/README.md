# Comparing `tmp/yente-3.8.8.tar.gz` & `tmp/yente-3.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yente-3.8.8.tar", last modified: Wed Apr 17 08:16:54 2024, max compression
+gzip compressed data, was "yente-3.8.9.tar", last modified: Thu May  9 09:18:23 2024, max compression
```

## Comparing `yente-3.8.8.tar` & `yente-3.8.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.137381 yente-3.8.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 08:15:08.000000 yente-3.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 08:15:08.000000 yente-3.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-17 08:16:54.137381 yente-3.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-17 08:15:08.000000 yente-3.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:16:54.137381 yente-3.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 08:15:08.000000 yente-3.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.129381 yente-3.8.8/yente/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:08.000000 yente-3.8.8/yente/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-17 08:15:08.000000 yente-3.8.8/yente/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-17 08:15:08.000000 yente-3.8.8/yente/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.133381 yente-3.8.8/yente/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/freebase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-17 08:15:08.000000 yente-3.8.8/yente/data/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-17 08:15:08.000000 yente-3.8.8/yente/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:08.000000 yente-3.8.8/yente/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-17 08:15:08.000000 yente-3.8.8/yente/reindex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.133381 yente-3.8.8/yente/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-17 08:15:08.000000 yente-3.8.8/yente/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.133381 yente-3.8.8/yente/routers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/match.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-17 08:15:08.000000 yente-3.8.8/yente/routers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 08:15:08.000000 yente-3.8.8/yente/scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.137381 yente-3.8.8/yente/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-17 08:15:08.000000 yente-3.8.8/yente/search/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-17 08:15:08.000000 yente-3.8.8/yente/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-17 08:15:08.000000 yente-3.8.8/yente/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-17 08:15:08.000000 yente-3.8.8/yente/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:16:54.137381 yente-3.8.8/yente.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:16:01.000000 yente-3.8.8/yente.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 08:16:54.000000 yente-3.8.8/yente.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:18:23.796887 yente-3.8.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-09 09:16:41.000000 yente-3.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 09:16:41.000000 yente-3.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-09 09:18:23.796887 yente-3.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-09 09:16:41.000000 yente-3.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:18:23.796887 yente-3.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-09 09:16:41.000000 yente-3.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:18:23.788887 yente-3.8.9/yente/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:16:41.000000 yente-3.8.9/yente/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-09 09:16:41.000000 yente-3.8.9/yente/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-09 09:16:41.000000 yente-3.8.9/yente/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:18:23.792887 yente-3.8.9/yente/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-09 09:16:41.000000 yente-3.8.9/yente/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-09 09:16:41.000000 yente-3.8.9/yente/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-09 09:16:41.000000 yente-3.8.9/yente/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-09 09:16:41.000000 yente-3.8.9/yente/data/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-09 09:16:41.000000 yente-3.8.9/yente/data/freebase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-09 09:16:41.000000 yente-3.8.9/yente/data/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-09 09:16:41.000000 yente-3.8.9/yente/data/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-09 09:16:41.000000 yente-3.8.9/yente/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-09 09:16:41.000000 yente-3.8.9/yente/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:16:41.000000 yente-3.8.9/yente/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 09:16:41.000000 yente-3.8.9/yente/reindex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:18:23.792887 yente-3.8.9/yente/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-09 09:16:41.000000 yente-3.8.9/yente/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:18:23.792887 yente-3.8.9/yente/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:16:41.000000 yente-3.8.9/yente/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-09 09:16:41.000000 yente-3.8.9/yente/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-09 09:16:41.000000 yente-3.8.9/yente/routers/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-09 09:16:41.000000 yente-3.8.9/yente/routers/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-09 09:16:41.000000 yente-3.8.9/yente/routers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-09 09:16:41.000000 yente-3.8.9/yente/routers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 09:16:41.000000 yente-3.8.9/yente/scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:18:23.792887 yente-3.8.9/yente/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:16:41.000000 yente-3.8.9/yente/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-09 09:16:41.000000 yente-3.8.9/yente/search/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-05-09 09:16:41.000000 yente-3.8.9/yente/search/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-09 09:16:41.000000 yente-3.8.9/yente/search/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-09 09:16:41.000000 yente-3.8.9/yente/search/nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-09 09:16:41.000000 yente-3.8.9/yente/search/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-05-09 09:16:41.000000 yente-3.8.9/yente/search/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-09 09:16:41.000000 yente-3.8.9/yente/search/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 09:16:41.000000 yente-3.8.9/yente/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-05-09 09:16:41.000000 yente-3.8.9/yente/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-09 09:16:41.000000 yente-3.8.9/yente/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:18:23.792887 yente-3.8.9/yente.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-09 09:18:23.000000 yente-3.8.9/yente.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-09 09:18:23.000000 yente-3.8.9/yente.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:18:23.000000 yente-3.8.9/yente.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 09:18:23.000000 yente-3.8.9/yente.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:18:23.000000 yente-3.8.9/yente.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:17:32.000000 yente-3.8.9/yente.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-09 09:18:23.000000 yente-3.8.9/yente.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 09:18:23.000000 yente-3.8.9/yente.egg-info/top_level.txt
```

### Comparing `yente-3.8.8/LICENSE` & `yente-3.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/PKG-INFO` & `yente-3.8.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.8.8
+Version: 3.8.9
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: followthemoney==3.5.9
+Requires-Dist: followthemoney==3.6.0
 Requires-Dist: nomenklatura==3.10.6
 Requires-Dist: rigour==0.5.2
-Requires-Dist: asyncstdlib==3.12.2
+Requires-Dist: asyncstdlib==3.12.3
 Requires-Dist: aiocron==1.8
-Requires-Dist: aiocsv==1.3.1
+Requires-Dist: aiocsv==1.3.2
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: types-aiofiles<23.3,>=23.1.0.4
-Requires-Dist: aiohttp[speedups]==3.9.3
-Requires-Dist: elasticsearch[async]==8.13.0
-Requires-Dist: fastapi==0.110.1
+Requires-Dist: aiohttp[speedups]==3.9.5
+Requires-Dist: elasticsearch[async]==8.13.1
+Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn[standard]==0.29.0
 Requires-Dist: httpx[http2]==0.27.0
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: email-validator==2.1.1
 Requires-Dist: structlog==24.1.0
-Requires-Dist: pyicu==2.12
+Requires-Dist: pyicu==2.13.1
 Requires-Dist: jellyfish==1.0.3
-Requires-Dist: orjson==3.10.0
+Requires-Dist: orjson==3.10.3
 Requires-Dist: text-unidecode==1.3
 Requires-Dist: click==8.1.6
 Requires-Dist: normality==2.5.0
 Requires-Dist: countrynames==1.15.3
 Requires-Dist: fingerprints==1.2.3
 Requires-Dist: pantomime==0.6.1
-Requires-Dist: cryptography==42.0.5
+Requires-Dist: cryptography==42.0.7
 Provides-Extra: dev
 Requires-Dist: pip>=10.0.0; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: wheel>=0.29.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
```

### Comparing `yente-3.8.8/README.md` & `yente-3.8.9/README.md`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/setup.py` & `yente-3.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="yente",
-    version="3.8.8",
+    version="3.8.9",
     url="https://opensanctions.org/docs/api/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="OpenSanctions",
     author_email="info@opensanctions.org",
     packages=find_packages(exclude=["examples", "tests"]),
     namespace_packages=[],
     install_requires=[
-        "followthemoney==3.5.9",
+        "followthemoney==3.6.0",
         "nomenklatura==3.10.6",
         "rigour==0.5.2",
-        "asyncstdlib==3.12.2",
+        "asyncstdlib==3.12.3",
         "aiocron==1.8",
-        "aiocsv==1.3.1",
+        "aiocsv==1.3.2",
         "aiofiles==23.2.1",
         "types-aiofiles>=23.1.0.4,<23.3",
-        "aiohttp[speedups]==3.9.3",
-        "elasticsearch[async]==8.13.0",
-        "fastapi==0.110.1",
+        "aiohttp[speedups]==3.9.5",
+        "elasticsearch[async]==8.13.1",
+        "fastapi==0.111.0",
         "uvicorn[standard]==0.29.0",
         "httpx[http2]==0.27.0",
         "python-multipart==0.0.9",
         "email-validator==2.1.1",
         "structlog==24.1.0",
-        "pyicu==2.12",
+        "pyicu==2.13.1",
         "jellyfish==1.0.3",
-        "orjson==3.10.0",
+        "orjson==3.10.3",
         "text-unidecode==1.3",
         "click==8.1.6",
         "normality==2.5.0",
         "countrynames==1.15.3",
         "fingerprints==1.2.3",
         "pantomime==0.6.1",
-        "cryptography==42.0.5",
+        "cryptography==42.0.7",
     ],
     extras_require={
         "dev": [
             "pip>=10.0.0",
             "bump2version",
             "wheel>=0.29.0",
             "twine",
```

### Comparing `yente-3.8.8/yente/app.py` & `yente-3.8.9/yente/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 import aiocron  # type: ignore
 from uuid import uuid4
 from typing import AsyncGenerator, Dict, Type, Callable, Any, Coroutine, Union
 from contextlib import asynccontextmanager
 from elasticsearch import ApiError, TransportError
+from pydantic import ValidationError
 from fastapi import FastAPI
 from fastapi import Request, Response
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.middleware.gzip import GZipMiddleware
 from starlette.middleware.base import RequestResponseEndpoint
 from fastapi.responses import JSONResponse
 from structlog.contextvars import clear_contextvars, bind_contextvars
@@ -83,17 +84,24 @@
 
 
 async def transport_error_handler(request: Request, exc: TransportError) -> Response:
     log.exception(f"Transport: {exc.message}")
     return JSONResponse(status_code=500, content={"detail": exc.message})
 
 
+async def validation_error_handler(request: Request, exc: ValidationError) -> Response:
+    log.warn(f"Validation error: {exc}")
+    body = {"detail": exc.title, "errors": exc.errors()}
+    return JSONResponse(status_code=400, content=body)
+
+
 HANDLERS: Dict[Union[Type[Exception], int], ExceptionHandler] = {
     ApiError: api_error_handler,
     TransportError: transport_error_handler,
+    ValidationError: validation_error_handler,
 }
 
 
 def create_app() -> FastAPI:
     app = FastAPI(
         title=settings.TITLE,
         description=settings.DESCRIPTION,
```

### Comparing `yente-3.8.8/yente/cli.py` & `yente-3.8.9/yente/cli.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/data/__init__.py` & `yente-3.8.9/yente/data/__init__.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/data/common.py` & `yente-3.8.9/yente/data/common.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/data/dataset.py` & `yente-3.8.9/yente/data/dataset.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/data/entity.py` & `yente-3.8.9/yente/data/entity.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/data/freebase.py` & `yente-3.8.9/yente/data/freebase.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/data/loader.py` & `yente-3.8.9/yente/data/loader.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/data/manifest.py` & `yente-3.8.9/yente/data/manifest.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/data/util.py` & `yente-3.8.9/yente/data/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/logs.py` & `yente-3.8.9/yente/logs.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/resources/favicon.ico` & `yente-3.8.9/yente/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/routers/admin.py` & `yente-3.8.9/yente/routers/admin.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/routers/match.py` & `yente-3.8.9/yente/routers/match.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/routers/reconcile.py` & `yente-3.8.9/yente/routers/reconcile.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/routers/search.py` & `yente-3.8.9/yente/routers/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/routers/util.py` & `yente-3.8.9/yente/routers/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/scoring.py` & `yente-3.8.9/yente/scoring.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/search/base.py` & `yente-3.8.9/yente/search/base.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/search/indexer.py` & `yente-3.8.9/yente/search/indexer.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/search/mapping.py` & `yente-3.8.9/yente/search/mapping.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/search/nested.py` & `yente-3.8.9/yente/search/nested.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/search/queries.py` & `yente-3.8.9/yente/search/queries.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/search/search.py` & `yente-3.8.9/yente/search/search.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/search/status.py` & `yente-3.8.9/yente/search/status.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente/settings.py` & `yente-3.8.9/yente/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 def env_str(name: str, default: str) -> str:
     """Ensure the env returns a string even on Windows (#100)."""
     value = stringify(env.get(name))
     return default if value is None else value
 
 
-VERSION = "3.8.8"
+VERSION = "3.8.9"
 AUTHOR = "OpenSanctions"
 HOME_PAGE = "https://www.opensanctions.org"
 EMAIL = "info@opensanctions.org"
 CONTACT = {"name": AUTHOR, "url": HOME_PAGE, "email": EMAIL}
 
 TITLE = env_str("YENTE_TITLE", "yente")
 DESCRIPTION = """
```

### Comparing `yente-3.8.8/yente/util.py` & `yente-3.8.9/yente/util.py`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente.egg-info/PKG-INFO` & `yente-3.8.9/yente.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: yente
-Version: 3.8.8
+Version: 3.8.9
 Home-page: https://opensanctions.org/docs/api/
 Author: OpenSanctions
 Author-email: info@opensanctions.org
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: followthemoney==3.5.9
+Requires-Dist: followthemoney==3.6.0
 Requires-Dist: nomenklatura==3.10.6
 Requires-Dist: rigour==0.5.2
-Requires-Dist: asyncstdlib==3.12.2
+Requires-Dist: asyncstdlib==3.12.3
 Requires-Dist: aiocron==1.8
-Requires-Dist: aiocsv==1.3.1
+Requires-Dist: aiocsv==1.3.2
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: types-aiofiles<23.3,>=23.1.0.4
-Requires-Dist: aiohttp[speedups]==3.9.3
-Requires-Dist: elasticsearch[async]==8.13.0
-Requires-Dist: fastapi==0.110.1
+Requires-Dist: aiohttp[speedups]==3.9.5
+Requires-Dist: elasticsearch[async]==8.13.1
+Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn[standard]==0.29.0
 Requires-Dist: httpx[http2]==0.27.0
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: email-validator==2.1.1
 Requires-Dist: structlog==24.1.0
-Requires-Dist: pyicu==2.12
+Requires-Dist: pyicu==2.13.1
 Requires-Dist: jellyfish==1.0.3
-Requires-Dist: orjson==3.10.0
+Requires-Dist: orjson==3.10.3
 Requires-Dist: text-unidecode==1.3
 Requires-Dist: click==8.1.6
 Requires-Dist: normality==2.5.0
 Requires-Dist: countrynames==1.15.3
 Requires-Dist: fingerprints==1.2.3
 Requires-Dist: pantomime==0.6.1
-Requires-Dist: cryptography==42.0.5
+Requires-Dist: cryptography==42.0.7
 Provides-Extra: dev
 Requires-Dist: pip>=10.0.0; extra == "dev"
 Requires-Dist: bump2version; extra == "dev"
 Requires-Dist: wheel>=0.29.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
```

### Comparing `yente-3.8.8/yente.egg-info/SOURCES.txt` & `yente-3.8.9/yente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yente-3.8.8/yente.egg-info/requires.txt` & `yente-3.8.9/yente.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-followthemoney==3.5.9
+followthemoney==3.6.0
 nomenklatura==3.10.6
 rigour==0.5.2
-asyncstdlib==3.12.2
+asyncstdlib==3.12.3
 aiocron==1.8
-aiocsv==1.3.1
+aiocsv==1.3.2
 aiofiles==23.2.1
 types-aiofiles<23.3,>=23.1.0.4
-aiohttp[speedups]==3.9.3
-elasticsearch[async]==8.13.0
-fastapi==0.110.1
+aiohttp[speedups]==3.9.5
+elasticsearch[async]==8.13.1
+fastapi==0.111.0
 uvicorn[standard]==0.29.0
 httpx[http2]==0.27.0
 python-multipart==0.0.9
 email-validator==2.1.1
 structlog==24.1.0
-pyicu==2.12
+pyicu==2.13.1
 jellyfish==1.0.3
-orjson==3.10.0
+orjson==3.10.3
 text-unidecode==1.3
 click==8.1.6
 normality==2.5.0
 countrynames==1.15.3
 fingerprints==1.2.3
 pantomime==0.6.1
-cryptography==42.0.5
+cryptography==42.0.7
 
 [dev]
 pip>=10.0.0
 bump2version
 wheel>=0.29.0
 twine
 mypy
```


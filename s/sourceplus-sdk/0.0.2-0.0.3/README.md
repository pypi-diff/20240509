# Comparing `tmp/sourceplus_sdk-0.0.2.tar.gz` & `tmp/sourceplus_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourceplus_sdk-0.0.2.tar", last modified: Thu May  9 16:53:33 2024, max compression
+gzip compressed data, was "sourceplus_sdk-0.0.3.tar", last modified: Thu May  9 18:53:41 2024, max compression
```

## Comparing `sourceplus_sdk-0.0.2.tar` & `sourceplus_sdk-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.841229 sourceplus_sdk-0.0.2/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      597 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/.coveragerc
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      566 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/.gitignore
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      530 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/.readthedocs.yml
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       74 2024-05-09 14:50:35.000000 sourceplus_sdk-0.0.2/AUTHORS.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       77 2024-05-09 15:07:32.000000 sourceplus_sdk-0.0.2/CHANGELOG.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1079 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/LICENSE.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3139 2024-05-09 16:53:33.841163 sourceplus_sdk-0.0.2/PKG-INFO
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2071 2024-05-09 15:26:48.000000 sourceplus_sdk-0.0.2/README.rst
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.837990 sourceplus_sdk-0.0.2/docs/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1154 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/Makefile
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.838127 sourceplus_sdk-0.0.2/docs/_static/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       18 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/_static/.gitignore
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       41 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/authors.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       43 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/changelog.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9769 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/conf.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1386 2024-05-09 15:49:09.000000 sourceplus_sdk-0.0.2/docs/index.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       67 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/license.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       39 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/readme.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      233 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/docs/requirements.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      346 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/pyproject.toml
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1539 2024-05-09 16:53:33.841563 sourceplus_sdk-0.0.2/setup.cfg
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      709 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/setup.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.834688 sourceplus_sdk-0.0.2/src/
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.838729 sourceplus_sdk-0.0.2/src/sourceplus_sdk/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      625 2024-05-08 17:29:55.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk/__init__.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      393 2024-05-08 19:56:34.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk/libs.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)    12944 2024-05-09 14:40:10.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk/main.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.840719 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3139 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/PKG-INFO
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      792 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       50 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/entry_points.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/not-zip-safe
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      120 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/requires.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       15 2024-05-09 16:53:33.000000 sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.840088 sourceplus_sdk-0.0.2/tests/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      282 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.2/tests/conftest.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 16:53:33.840461 sourceplus_sdk-0.0.2/tests/files/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 12:40:19.000000 sourceplus_sdk-0.0.2/tests/files/bad.parquet
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 12:48:45.000000 sourceplus_sdk-0.0.2/tests/files/bad.tsv
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1027 2024-05-09 12:56:36.000000 sourceplus_sdk-0.0.2/tests/files/good.parquet
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1140 2024-05-09 12:58:10.000000 sourceplus_sdk-0.0.2/tests/test_libs.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     6491 2024-05-09 14:43:09.000000 sourceplus_sdk-0.0.2/tests/test_main.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2766 2024-05-09 16:49:30.000000 sourceplus_sdk-0.0.2/tox.ini
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 18:53:41.566567 sourceplus_sdk-0.0.3/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      597 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/.coveragerc
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      566 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/.gitignore
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      530 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/.readthedocs.yml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       74 2024-05-09 14:50:35.000000 sourceplus_sdk-0.0.3/AUTHORS.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       77 2024-05-09 15:07:32.000000 sourceplus_sdk-0.0.3/CHANGELOG.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1079 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/LICENSE.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3139 2024-05-09 18:53:41.566496 sourceplus_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2071 2024-05-09 15:26:48.000000 sourceplus_sdk-0.0.3/README.rst
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 18:53:41.562491 sourceplus_sdk-0.0.3/docs/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1154 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/docs/Makefile
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 18:53:41.562652 sourceplus_sdk-0.0.3/docs/_static/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       18 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/docs/_static/.gitignore
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       41 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/docs/authors.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       43 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/docs/changelog.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9769 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/docs/conf.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1386 2024-05-09 15:49:09.000000 sourceplus_sdk-0.0.3/docs/index.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       67 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/docs/license.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       39 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/docs/readme.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      233 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/docs/requirements.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      346 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1539 2024-05-09 18:53:41.566910 sourceplus_sdk-0.0.3/setup.cfg
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      709 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/setup.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 18:53:41.559194 sourceplus_sdk-0.0.3/src/
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 18:53:41.563268 sourceplus_sdk-0.0.3/src/sourceplus_sdk/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      625 2024-05-08 17:29:55.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk/__init__.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      393 2024-05-08 19:56:34.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk/libs.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)    13144 2024-05-09 18:51:59.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk/main.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 18:53:41.565999 sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3139 2024-05-09 18:53:41.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      792 2024-05-09 18:53:41.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2024-05-09 18:53:41.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       50 2024-05-09 18:53:41.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2024-05-09 18:53:41.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      120 2024-05-09 18:53:41.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/requires.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       15 2024-05-09 18:53:41.000000 sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 18:53:41.565243 sourceplus_sdk-0.0.3/tests/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      282 2024-05-08 16:20:06.000000 sourceplus_sdk-0.0.3/tests/conftest.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 18:53:41.565670 sourceplus_sdk-0.0.3/tests/files/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 12:40:19.000000 sourceplus_sdk-0.0.3/tests/files/bad.parquet
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        0 2024-05-09 12:48:45.000000 sourceplus_sdk-0.0.3/tests/files/bad.tsv
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1027 2024-05-09 12:56:36.000000 sourceplus_sdk-0.0.3/tests/files/good.parquet
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1140 2024-05-09 12:58:10.000000 sourceplus_sdk-0.0.3/tests/test_libs.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     6720 2024-05-09 18:45:13.000000 sourceplus_sdk-0.0.3/tests/test_main.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2766 2024-05-09 16:49:30.000000 sourceplus_sdk-0.0.3/tox.ini
```

### Comparing `sourceplus_sdk-0.0.2/.coveragerc` & `sourceplus_sdk-0.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/.gitignore` & `sourceplus_sdk-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/.readthedocs.yml` & `sourceplus_sdk-0.0.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/LICENSE.txt` & `sourceplus_sdk-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/PKG-INFO` & `sourceplus_sdk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourceplus-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Search, curate, and enrich collections for AI training.
 Home-page: https://github.com/Spawning-Inc/sourceplus-sdk/
 Author: Nick Padgett
 Author-email: nick@spawning.ai
 License: MIT
 Project-URL: Documentation, https://sourceplus-sdk.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spawning-Inc/sourceplus-sdk
```

### Comparing `sourceplus_sdk-0.0.2/README.rst` & `sourceplus_sdk-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/docs/Makefile` & `sourceplus_sdk-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/docs/conf.py` & `sourceplus_sdk-0.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/docs/index.rst` & `sourceplus_sdk-0.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/setup.cfg` & `sourceplus_sdk-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/setup.py` & `sourceplus_sdk-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/src/sourceplus_sdk/__init__.py` & `sourceplus_sdk-0.0.3/src/sourceplus_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/src/sourceplus_sdk/main.py` & `sourceplus_sdk-0.0.3/src/sourceplus_sdk/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 import pandas as pd
 import aiofiles
 
 
 def download_images(
     file_path: str,
     output_folder: str,
-    num_download_jobs: int = 10,
+    num_download_jobs: int = 50,
     limit_images: int = -1,
     url_column_name: str = "url",
     show_progress: bool = False,
 ):
     """Download images from the given file path to the destination folder.
 
     Args:
         file_path (str): The path to the file containing the URLs of the images to download.
         output_folder (str): The path to the folder where the images will be saved.
-        num_download_jobs (int, optional): The maximum number of parallel downloads. Defaults to 10.
+        num_download_jobs (int, optional): The maximum number of parallel downloads. Defaults to 50.
         limit_images (int, optional): The maximum number of images to download. Defaults to -1, which means all images.
         url_column_name (str, optional): The name of the column containing the URLs in the file. Defaults to "url".
         show_progress (bool, optional): Whether to show a progress bar. Defaults to False.
 
     """
 
     # validate the input arguments
@@ -176,25 +176,33 @@
     semaphore = asyncio.Semaphore(max_parallel_downloads)
     download_queue = df.iterrows()
 
     # start the download manager
     success_counter = AsyncCounter()
     failure_counter = AsyncCounter()
     tasks = []
+
+    # make http client
+    http_client = httpx.AsyncClient(timeout=10)
+
+    # create tasks
     for i in range(0, max_images if max_images > 0 else len(df)):
         row = next(download_queue)
         url = row[1]["url"]
-        tasks.append(download_image(url, semaphore, success_counter, failure_counter, destination_folder, api_key))
+        tasks.append(download_image(http_client, url, semaphore, success_counter, failure_counter, destination_folder, api_key))
 
     # start the progress monitor
     if show_progress:
         tasks.insert(0, progress_monitor(success_counter, failure_counter, max_images))
 
-    # wait for all tasks to complete
-    await asyncio.gather(*tasks)
+    # wait for all tasks to complete and close client
+    try:
+        await asyncio.gather(*tasks)
+    finally:
+        await http_client.aclose()
 
 
 async def progress_monitor(success_counter: AsyncCounter, failure_counter: AsyncCounter, total_images: int):
     """
     Monitors the progress of the downloads.
 
     Args:
@@ -221,24 +229,25 @@
         bar_length = 50
         bar = "#" * int(bar_length * progress)
         elapsed_time = time.time() - start_time
         print(f"[{bar.ljust(bar_length)}] {progress * 100:.2f}% - Elapsed Time: {elapsed_time:.2f}s")
 
         if num_completed == total_images:
             break
-        await asyncio.sleep(.5)
+        await asyncio.sleep(.1)
 
     print(f"Total images: {total_images}. Successes: {successes}. Failures: {failures}")
 
 
-async def download_image(url: str, semaphore: asyncio.Semaphore, success_counter: AsyncCounter, failure_counter: AsyncCounter, destination_folder: str, api_key: str):
+async def download_image(client: httpx.AsyncClient,  url: str, semaphore: asyncio.Semaphore, success_counter: AsyncCounter, failure_counter: AsyncCounter, destination_folder: str, api_key: str):
     """
     Downloads an image from the given URL, using the semaphore to control the number of parallel downloads.
 
     Args:
+        client (httpx.AsyncClient): The HTTP client to use for downloading the image.
         url (str): The URL of the image to download.
         semaphore (asyncio.Semaphore): The semaphore to control the number of parallel downloads.
         success_counter (AsyncCounter): The counter to keep track of the number of successful downloads.
         failure_counter (AsyncCounter): The counter to keep track of the number of failed downloads.
         destination_folder (str): The path to the folder where the image will be saved.
         api_key (str): The Source+ download key.
 
@@ -250,28 +259,27 @@
         file_path = os.path.join(destination_folder, file_name)
 
         # if file exists, skip it, so we don't download it twice
         if os.path.exists(file_path):
             await success_counter.increment()
             return
 
-        async with httpx.AsyncClient(timeout=10) as client:
-            try:
-                async with client.stream("GET", url, headers={"Authorization": f"API {api_key}"}, follow_redirects=True) as response:
-                    if response.status_code == 200:
-                        image_data = await response.aread()
-                        async with aiofiles.open(file_path, "wb") as f:
-                            await f.write(image_data)
-                        await success_counter.increment()
-                    else:
-                        #logging.error(f"Failed to download image from URL: {url} - {response.status_code}")
-                        await failure_counter.increment()
-            except Exception as e:
-                #logging.error(f"Failed to download image from URL: {url} - {e}")
-                await failure_counter.increment()
+        try:
+            async with client.stream("GET", url, headers={"Authorization": f"API {api_key}"}, follow_redirects=True) as response:
+                if response.status_code == 200:
+                    image_data = await response.aread()
+                    async with aiofiles.open(file_path, "wb") as f:
+                        await f.write(image_data)
+                    await success_counter.increment()
+                else:
+                    #logging.error(f"Failed to download image from URL: {url} - {response.status_code}")
+                    await failure_counter.increment()
+        except Exception as e:
+            #logging.error(f"Failed to download image from URL: {url} - {e}")
+            await failure_counter.increment()
 
 # ---- CLI ----
 # The functions defined in this section are wrappers around the main Python
 # API allowing them to be called directly from the terminal as a CLI
 # executable/script.
 
 
@@ -285,15 +293,15 @@
     Returns:
       :obj:`argparse.Namespace`: command line parameters namespace
     """
     parser = argparse.ArgumentParser(description="Download images.")
     parser.add_argument("command", help="Command to execute. Valid commands: download_images", type=str)
     parser.add_argument("-f", "--file", dest="file_path", help="Path to the file which contains the image URLs.", type=str)
     parser.add_argument("-o", "--output", dest="output_folder", help="Path to the destination folder to download the images.", type=str)
-    parser.add_argument("-j", "--jobs", dest="num_download_jobs", default=10, help="The maximum number of download jobs running in parallel. A value too high will cause resource contention and slow down the overall download rate.", type=int)
+    parser.add_argument("-j", "--jobs", dest="num_download_jobs", default=50, help="The maximum number of download jobs running in parallel. Default is 50. A value too high will cause resource contention and slow down the overall download rate.", type=int)
     parser.add_argument("-l", "--limit", dest="limit_images", default=-1, help="The maximum number of images you want to download from the file.", type=int)
     parser.add_argument("-n", "--name", dest="url_column_name", default="url", help="The column name for the url field.", type=str)
     parser.add_argument("-p", "--progress", dest="show_progress", default=True, help="Show progress bar.", type=bool)
 
     parser.add_argument(
         "--version",
         action="version",
```

### Comparing `sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/PKG-INFO` & `sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourceplus-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Search, curate, and enrich collections for AI training.
 Home-page: https://github.com/Spawning-Inc/sourceplus-sdk/
 Author: Nick Padgett
 Author-email: nick@spawning.ai
 License: MIT
 Project-URL: Documentation, https://sourceplus-sdk.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spawning-Inc/sourceplus-sdk
```

### Comparing `sourceplus_sdk-0.0.2/src/sourceplus_sdk.egg-info/SOURCES.txt` & `sourceplus_sdk-0.0.3/src/sourceplus_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/tests/files/good.parquet` & `sourceplus_sdk-0.0.3/tests/files/good.parquet`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/tests/test_libs.py` & `sourceplus_sdk-0.0.3/tests/test_libs.py`

 * *Files identical despite different names*

### Comparing `sourceplus_sdk-0.0.2/tests/test_main.py` & `sourceplus_sdk-0.0.3/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from unittest import TestCase
 from unittest.mock import patch
 import os
 import asyncio
 
+import httpx
+
 import sourceplus_sdk.main
 from sourceplus_sdk.libs import AsyncCounter
 
 
 class TestMain(TestCase):
 
     def test_validate_args(self):
@@ -82,28 +84,32 @@
 
         os.mkdir(destination_folder)
 
         async def async_test_image():
             sem = asyncio.Semaphore(1)
             success_counter = AsyncCounter()
             failure_counter = AsyncCounter()
+            httpx_client = httpx.AsyncClient()
 
-            await sourceplus_sdk.main.download_image(url, sem, success_counter, failure_counter, destination_folder, api_key)
-            self.assertEqual(await success_counter.get(), 1)
-            self.assertEqual(await failure_counter.get(), 0)
-
-            # test same url
-            await sourceplus_sdk.main.download_image(url, sem, success_counter, failure_counter, destination_folder, api_key)
-            self.assertEqual(await success_counter.get(), 2)
-            self.assertEqual(await failure_counter.get(), 0)
-
-            # test bad url
-            await sourceplus_sdk.main.download_image("https://spawning.substack.com/sdk.test.jpg", sem, success_counter, failure_counter, destination_folder, api_key)
-            self.assertEqual(await success_counter.get(), 2)
-            self.assertEqual(await failure_counter.get(), 1)
+            try:
+                await sourceplus_sdk.main.download_image(httpx_client, url, sem, success_counter, failure_counter, destination_folder, api_key)
+                self.assertEqual(await success_counter.get(), 1)
+                self.assertEqual(await failure_counter.get(), 0)
+
+                # test same url
+                await sourceplus_sdk.main.download_image(httpx_client, url, sem, success_counter, failure_counter, destination_folder, api_key)
+                self.assertEqual(await success_counter.get(), 2)
+                self.assertEqual(await failure_counter.get(), 0)
+
+                # test bad url
+                await sourceplus_sdk.main.download_image(httpx_client, "https://spawning.substack.com/sdk.test.jpg", sem, success_counter, failure_counter, destination_folder, api_key)
+                self.assertEqual(await success_counter.get(), 2)
+                self.assertEqual(await failure_counter.get(), 1)
+            finally:
+                await httpx_client.aclose()
 
         asyncio.run(async_test_image())
 
     @patch('getpass.getpass', return_value='test')
     def test_download_images(self, mock_getpass):
         # create outputs folder
         os.mkdir("./tests/output")
```

### Comparing `sourceplus_sdk-0.0.2/tox.ini` & `sourceplus_sdk-0.0.3/tox.ini`

 * *Files identical despite different names*


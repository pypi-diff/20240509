# Comparing `tmp/athena_starship-0.0.1.tar.gz` & `tmp/athena_starship-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_starship-0.0.1.tar", max compression
+gzip compressed data, was "athena_starship-0.0.2.tar", max compression
```

## Comparing `athena_starship-0.0.1.tar` & `athena_starship-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1074 2024-03-04 04:39:01.432725 athena_starship-0.0.1/LICENSE
--rw-r--r--   0        0        0     1739 2024-03-04 04:39:01.432927 athena_starship-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-03-04 06:58:05.607012 athena_starship-0.0.1/athena_starship/__init__.py
--rw-r--r--   0        0        0     2272 2024-05-08 23:14:06.039278 athena_starship-0.0.1/athena_starship/data_connectors.py
--rw-r--r--   0        0        0      760 2024-03-05 03:34:59.479475 athena_starship-0.0.1/athena_starship/first.py
--rw-r--r--   0        0        0     1010 2024-03-05 03:43:11.478883 athena_starship-0.0.1/athena_starship/ghost_datasource_urls.py
--rw-r--r--   0        0        0     1822 2024-05-08 23:14:06.430402 athena_starship-0.0.1/athena_starship/tool_schemas.py
--rw-r--r--   0        0        0     2478 2024-05-08 23:14:06.127654 athena_starship-0.0.1/athena_starship/youtube_utils.py
--rw-r--r--   0        0        0     1341 2024-05-08 23:16:36.308212 athena_starship-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 athena_starship-0.0.1/setup.py
--rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 athena_starship-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        1 2024-05-08 23:20:52.861407 athena_starship-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1290 2024-05-08 23:56:29.101861 athena_starship-0.0.2/README.md
+-rw-r--r--   0        0        0      116 2024-05-08 23:58:01.824713 athena_starship-0.0.2/athena_starship/__init__.py
+-rw-r--r--   0        0        0     2375 2024-05-08 23:34:28.241612 athena_starship-0.0.2/athena_starship/data_connectors.py
+-rw-r--r--   0        0        0     1010 2024-05-08 23:20:52.885141 athena_starship-0.0.2/athena_starship/ghost_datasource_urls.py
+-rw-r--r--   0        0        0      158 2024-05-08 23:42:10.513806 athena_starship-0.0.2/athena_starship/llama.py
+-rw-r--r--   0        0        0     5403 2024-05-08 23:39:54.739467 athena_starship-0.0.2/athena_starship/memory.py
+-rw-r--r--   0        0        0     1822 2024-05-08 23:20:52.886160 athena_starship-0.0.2/athena_starship/tool_schemas.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:27:03.908694 athena_starship-0.0.2/athena_starship/tools/__init__.py
+-rw-r--r--   0        0        0     2932 2024-05-08 23:33:29.346598 athena_starship-0.0.2/athena_starship/tools/google_calendar.py
+-rw-r--r--   0        0        0     2478 2024-05-08 23:20:52.886402 athena_starship-0.0.2/athena_starship/youtube_utils.py
+-rw-r--r--   0        0        0     1341 2024-05-08 23:58:08.022029 athena_starship-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2014 1970-01-01 00:00:00.000000 athena_starship-0.0.2/setup.py
+-rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 athena_starship-0.0.2/PKG-INFO
```

### Comparing `athena_starship-0.0.1/athena_starship/data_connectors.py` & `athena_starship-0.0.2/athena_starship/data_connectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import os
 
 import requests
 from llama_index import download_loader
 from swarms import create_file
+from swarms.tools import tool
 
 
-def load_airtable_data(
-    airtable_token: str, table_id: str, base_id: str
-):
+@tool
+def load_airtable_data(table_id: str, base_id: str):
     """
     Loads data from Airtable using the provided credentials.
 
     Args:
         airtable_token (str): The API token for accessing Airtable.
         table_id (str): The ID of the table to load data from.
         base_id (str): The ID of the base containing the table.
 
     Returns:
         list: A list of documents retrieved from Airtable.
     """
+    airtable_token = os.getenv("AIRTABLE_TOKEN")
     AirtableReader = download_loader("AirtableReader")
     reader = AirtableReader(airtable_token)
     documents = reader.load_data(table_id=table_id, base_id=base_id)
 
     return documents
 
 
 # # Usage:
 # airtable_token = os.getenv("AIRTABLE_TOKEN")
 # table_id = os.getenv("TABLE_ID")
 # base_id = os.getenv("BASE_ID")
 # data = load_airtable_data(airtable_token, table_id, base_id)
 
 
-NOTION_TOKEN = os.getenv("NOTION_TOKEN")
-DATABASE_ID = os.getenv("DATABASE_ID")
-
-notion_headers = {
-    "Authorization": "Bearer " + NOTION_TOKEN,
-    "Content-Type": "application/json",
-    "Notion-Version": "2022-06-28",
-}
-
-
 def get_notion_pages(
-    num_pages: int = None, headers: dict = notion_headers
+    num_pages: int = None,
 ):
     """
     If num_pages is None, get all pages, otherwise just the defined number.
     """
+    NOTION_TOKEN = os.getenv("NOTION_TOKEN")
+    DATABASE_ID = os.getenv("DATABASE_ID")
+
+    notion_headers = {
+        "Authorization": "Bearer " + NOTION_TOKEN,
+        "Content-Type": "application/json",
+        "Notion-Version": "2022-06-28",
+    }
     url = f"https://api.notion.com/v1/databases/{DATABASE_ID}/query"
 
     get_all = num_pages is None
     page_size = 100 if get_all else num_pages
 
     payload = {"page_size": page_size}
-    response = requests.post(url, json=payload, headers=headers)
+    response = requests.post(
+        url, json=payload, headers=notion_headers
+    )
 
     data = response.json()
 
     # Comment this out to dump all data to a file
     # import json
     # with open('db.json', 'w', encoding='utf8') as f:
     #    json.dump(data, f, ensure_ascii=False, indent=4)
@@ -69,14 +70,16 @@
         payload = {
             "page_size": page_size,
             "start_cursor": data["next_cursor"],
         }
         url = (
             f"https://api.notion.com/v1/databases/{DATABASE_ID}/query"
         )
-        response = requests.post(url, json=payload, headers=headers)
+        response = requests.post(
+            url, json=payload, headers=notion_headers
+        )
         data = response.json()
         results.extend(data["results"])
 
     create_file(results, "notion_blob.txt")
 
     return results
```

### Comparing `athena_starship-0.0.1/athena_starship/ghost_datasource_urls.py` & `athena_starship-0.0.2/athena_starship/ghost_datasource_urls.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.1/athena_starship/tool_schemas.py` & `athena_starship-0.0.2/athena_starship/tool_schemas.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.1/athena_starship/youtube_utils.py` & `athena_starship-0.0.2/athena_starship/youtube_utils.py`

 * *Files identical despite different names*

### Comparing `athena_starship-0.0.1/pyproject.toml` & `athena_starship-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "athena-starship"
-version = "0.0.1"
+version = "0.0.2"
 description = "Paper - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/Starship-Ventures/Athena"
 documentation = "https://github.com/Starship-Ventures/Athena"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/Starship-Ventures/Athena"
```


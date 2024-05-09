# Comparing `tmp/firecrawl-py-0.0.6.tar.gz` & `tmp/firecrawl-py-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firecrawl-py-0.0.6.tar", last modified: Thu Apr 25 18:11:13 2024, max compression
+gzip compressed data, was "firecrawl-py-0.0.7.tar", last modified: Thu May  9 00:17:57 2024, max compression
```

## Comparing `firecrawl-py-0.0.6.tar` & `firecrawl-py-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-25 18:11:13.958743 firecrawl-py-0.0.6/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-04-25 18:11:13.958635 firecrawl-py-0.0.6/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)     3363 2024-04-18 02:03:35.000000 firecrawl-py-0.0.6/README.md
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-25 18:11:13.957776 firecrawl-py-0.0.6/firecrawl/
--rw-r--r--   0 nicolascamara   (501) staff       (20)       36 2024-04-15 21:00:54.000000 firecrawl-py-0.0.6/firecrawl/__init__.py
--rw-r--r--   0 nicolascamara   (501) staff       (20)     5168 2024-04-25 18:06:19.000000 firecrawl-py-0.0.6/firecrawl/firecrawl.py
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-25 18:11:13.958488 firecrawl-py-0.0.6/firecrawl_py.egg-info/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/SOURCES.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/dependency_links.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/requires.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-04-25 18:11:13.000000 firecrawl-py-0.0.6/firecrawl_py.egg-info/top_level.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-04-25 18:11:13.958781 firecrawl-py-0.0.6/setup.cfg
--rw-r--r--   0 nicolascamara   (501) staff       (20)      346 2024-04-25 18:10:23.000000 firecrawl-py-0.0.6/setup.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-05-09 00:17:57.617854 firecrawl-py-0.0.7/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-05-09 00:17:57.617723 firecrawl-py-0.0.7/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     3561 2024-04-26 21:23:35.000000 firecrawl-py-0.0.7/README.md
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-05-09 00:17:57.616840 firecrawl-py-0.0.7/firecrawl/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       36 2024-04-15 21:00:54.000000 firecrawl-py-0.0.7/firecrawl/__init__.py
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     7145 2024-05-09 00:12:12.000000 firecrawl-py-0.0.7/firecrawl/firecrawl.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-05-09 00:17:57.617543 firecrawl-py-0.0.7/firecrawl_py.egg-info/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      196 2024-05-09 00:17:57.000000 firecrawl-py-0.0.7/firecrawl_py.egg-info/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-05-09 00:17:57.000000 firecrawl-py-0.0.7/firecrawl_py.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-05-09 00:17:57.000000 firecrawl-py-0.0.7/firecrawl_py.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-05-09 00:17:57.000000 firecrawl-py-0.0.7/firecrawl_py.egg-info/requires.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-05-09 00:17:57.000000 firecrawl-py-0.0.7/firecrawl_py.egg-info/top_level.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-05-09 00:17:57.617912 firecrawl-py-0.0.7/setup.cfg
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      346 2024-05-09 00:16:16.000000 firecrawl-py-0.0.7/setup.py
```

### Comparing `firecrawl-py-0.0.6/README.md` & `firecrawl-py-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,23 @@
 To scrape a single URL, use the `scrape_url` method. It takes the URL as a parameter and returns the scraped data as a dictionary.
 
 ```python
 url = 'https://example.com'
 scraped_data = app.scrape_url(url)
 ```
 
+### Search for a query
+
+Used to search the web, get the most relevant results, scrap each page and return the markdown.
+
+```python
+query = 'what is mendable?'
+search_result = app.search(query)
+```
+
 ### Crawling a Website
 
 To crawl a website, use the `crawl_url` method. It takes the starting URL and optional parameters as arguments. The `params` argument allows you to specify additional options for the crawl job, such as the maximum number of pages to crawl, allowed domains, and the output format.
 
 The `wait_until_done` parameter determines whether the method should wait for the crawl job to complete before returning the result. If set to `True`, the method will periodically check the status of the crawl job until it is completed or the specified `timeout` (in seconds) is reached. If set to `False`, the method will return immediately with the job ID, and you can manually check the status of the crawl job using the `check_crawl_status` method.
 
 ```python
```


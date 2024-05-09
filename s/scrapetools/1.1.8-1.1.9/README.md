# Comparing `tmp/scrapetools-1.1.8.tar.gz` & `tmp/scrapetools-1.1.9.tar.gz`

## Comparing `scrapetools-1.1.8.tar` & `scrapetools-1.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 scrapetools-1.1.8/src/scrapetools/__init__.py
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 scrapetools-1.1.8/src/scrapetools/email_scraper.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 scrapetools-1.1.8/src/scrapetools/input_scraper.py
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 scrapetools-1.1.8/src/scrapetools/link_scraper.py
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 scrapetools-1.1.8/src/scrapetools/phone_scraper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapetools-1.1.8/src/scrapetools/py.typed
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 scrapetools-1.1.8/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scrapetools-1.1.8/LICENSE.txt
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 scrapetools-1.1.8/README.md
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 scrapetools-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 scrapetools-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 scrapetools-1.1.9/src/scrapetools/__init__.py
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 scrapetools-1.1.9/src/scrapetools/email_scraper.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 scrapetools-1.1.9/src/scrapetools/input_scraper.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 scrapetools-1.1.9/src/scrapetools/link_scraper.py
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 scrapetools-1.1.9/src/scrapetools/phone_scraper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrapetools-1.1.9/src/scrapetools/py.typed
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 scrapetools-1.1.9/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 scrapetools-1.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 scrapetools-1.1.9/README.md
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 scrapetools-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 scrapetools-1.1.9/PKG-INFO
```

### Comparing `scrapetools-1.1.8/src/scrapetools/email_scraper.py` & `scrapetools-1.1.9/src/scrapetools/email_scraper.py`

 * *Files identical despite different names*

### Comparing `scrapetools-1.1.8/src/scrapetools/input_scraper.py` & `scrapetools-1.1.9/src/scrapetools/input_scraper.py`

 * *Files identical despite different names*

### Comparing `scrapetools-1.1.8/src/scrapetools/link_scraper.py` & `scrapetools-1.1.9/src/scrapetools/link_scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import html
+import re
 from typing import Any
 from urllib.parse import urlparse, urlunparse
 
 from bs4 import BeautifulSoup
 
 
 class LinkScraper:
     def __init__(self, html_src: str, page_url: str):
+        self.source = html_src
         self.soup = BeautifulSoup(html_src, features="html.parser")
         self.parsed_url = urlparse(page_url)
         self.page_links = []
         self.img_links = []
         self.script_links = []
 
     def format_relative_links(self, links: list[str]) -> list[str]:
@@ -73,14 +76,15 @@
             ("source", "src"),
             ("div", "src"),
             ("div", "data-src"),
             ("div", "data-url"),
             ("div", "href"),
         ]:
             links.extend(self.find_all(tag, attribute))
+        links.extend(self.scrape_regex())
         self.page_links = self.process_links(links)
 
     def scrape_img_links(self):
         """Scrape links from src attribute of <img> tags."""
         self.img_links = self.process_links(
             self.find_all("img", "src") + self.find_all("img", "data-src")
         )
@@ -106,29 +110,34 @@
         formats = [
             ".jpg",
             ".jpeg",
             ".png",
             ".svg",
             ".bmp",
             ".tiff",
-            ".pdf",
             ".eps",
             ".gif",
             ".jfif",
             ".webp",
             ".heif",
             ".avif",
             ".bat",
             ".bpg",
         ]
         for link in self.script_links + self.page_links:
             if any(ext in link for ext in formats):
                 self.img_links.append(link)
         self.img_links = sorted(self.remove_duplicates(self.img_links))
 
+    def scrape_regex(self) -> list[str]:
+        """Use regex to scrape page source for `http` and `https` urls."""
+        pattern = r"https?://(?:www\.)?[-a-zA-Z0-9@:%._\+~#=]{2,256}\.[a-z]{2,6}\b(?:[-a-zA-Z0-9@:%_\+.~#?&//=]*)"
+        matches = re.findall(pattern, html.unescape(self.source))
+        return matches
+
     def get_links(
         self,
         link_type: str = "all",
         same_site_only: bool = False,
         excluded_links: list[str] | None = None,
     ) -> list[str]:
         """Returns a list of urls found on the page.
```

### Comparing `scrapetools-1.1.8/src/scrapetools/phone_scraper.py` & `scrapetools-1.1.9/src/scrapetools/phone_scraper.py`

 * *Files identical despite different names*

### Comparing `scrapetools-1.1.8/LICENSE.txt` & `scrapetools-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapetools-1.1.8/README.md` & `scrapetools-1.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # Scrapetools
-A collection of tools to aid in web scraping.<br>
+
+A collection of tools to aid in web scraping.  
+
 Install using:
-<pre>pip install scrapetools</pre>
+
+```console
+pip install scrapetools
+```
+
 Scrapetools contains three functions (scrape_emails, scrape_phone_numbers, scrape_inputs)
-and one class (LinkScraper).
-<br>
+and one class (LinkScraper).  
+
 ## Basic usage
-<pre>
+
+```python
 import scrapetools
 import requests
 
 url = 'https://somewebsite.com'
 source = requests.get(url).text
 
 emails = scrapetools.scrape_emails(source)
@@ -22,8 +29,8 @@
 # links can be accessed and filtered via the get_links() function
 same_site_links = scraper.get_links(same_site_only=True)
 same_site_image_links = scraper.get_links(link_type='img', same_site_only=True)
 external_image_links = scraper.get_links(link_type='img', excluded_links=same_site_image_links)
 
 # scrape_inputs() returns a tuple of BeautifulSoup Tag elements for various user input elements
 forms, inputs, buttons, selects, text_areas = scrapetools.scrape_inputs(source)
-</pre>
+```
```

### Comparing `scrapetools-1.1.8/pyproject.toml` & `scrapetools-1.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "scrapetools"
 description = "A collection of tools to aid in web scraping."
-version = "1.1.8"
-dependencies = ["bs4", "phonenumbers", "beautifulsoup4"]
+version = "1.1.9"
+dependencies = ["phonenumbers", "beautifulsoup4"]
 readme = "README.md"
 keywords = ["webscraping", "web", "html", "email", "scrape", "scraping"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 requires-python = ">=3.10"
 
 [[project.authors]]
 name = "Matt Manes"
-email = ""
+email = "mattmanes@pm.me"
 
 [project.urls]
 Homepage = "https://github.com/matt-manes/scrapetools"
 Documentation = "https://github.com/matt-manes/scrapetools/tree/main/docs"
 "Source code" = "https://github.com/matt-manes/scrapetools/tree/main/src/scrapetools"
 
 [project.scripts]
```

### Comparing `scrapetools-1.1.8/PKG-INFO` & `scrapetools-1.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,41 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: scrapetools
-Version: 1.1.8
+Version: 1.1.9
 Summary: A collection of tools to aid in web scraping.
 Project-URL: Homepage, https://github.com/matt-manes/scrapetools
 Project-URL: Documentation, https://github.com/matt-manes/scrapetools/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/scrapetools/tree/main/src/scrapetools
-Author: Matt Manes
+Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: email,html,scrape,scraping,web,webscraping
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: beautifulsoup4
-Requires-Dist: bs4
 Requires-Dist: phonenumbers
 Description-Content-Type: text/markdown
 
 # Scrapetools
-A collection of tools to aid in web scraping.<br>
+
+A collection of tools to aid in web scraping.  
+
 Install using:
-<pre>pip install scrapetools</pre>
+
+```console
+pip install scrapetools
+```
+
 Scrapetools contains three functions (scrape_emails, scrape_phone_numbers, scrape_inputs)
-and one class (LinkScraper).
-<br>
+and one class (LinkScraper).  
+
 ## Basic usage
-<pre>
+
+```python
 import scrapetools
 import requests
 
 url = 'https://somewebsite.com'
 source = requests.get(url).text
 
 emails = scrapetools.scrape_emails(source)
@@ -41,8 +47,8 @@
 # links can be accessed and filtered via the get_links() function
 same_site_links = scraper.get_links(same_site_only=True)
 same_site_image_links = scraper.get_links(link_type='img', same_site_only=True)
 external_image_links = scraper.get_links(link_type='img', excluded_links=same_site_image_links)
 
 # scrape_inputs() returns a tuple of BeautifulSoup Tag elements for various user input elements
 forms, inputs, buttons, selects, text_areas = scrapetools.scrape_inputs(source)
-</pre>
+```
```


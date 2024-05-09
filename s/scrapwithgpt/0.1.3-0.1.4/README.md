# Comparing `tmp/scrapwithgpt-0.1.3.tar.gz` & `tmp/scrapwithgpt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.1.3.tar", last modified: Thu May  9 14:16:56 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.1.4.tar", last modified: Thu May  9 14:22:27 2024, max compression
```

## Comparing `scrapwithgpt-0.1.3.tar` & `scrapwithgpt-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 14:16:56.787886 scrapwithgpt-0.1.3/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 14:16:56.787659 scrapwithgpt-0.1.3/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.3/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 14:16:56.786619 scrapwithgpt-0.1.3/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.3/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3639 2024-05-09 13:30:00.000000 scrapwithgpt-0.1.3/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.3/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4324 2024-05-09 13:49:38.000000 scrapwithgpt-0.1.3/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     5122 2024-05-09 13:47:50.000000 scrapwithgpt-0.1.3/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3262 2024-05-09 13:51:07.000000 scrapwithgpt-0.1.3/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    16548 2024-05-09 14:16:53.000000 scrapwithgpt-0.1.3/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 14:16:56.787389 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 14:16:56.787928 scrapwithgpt-0.1.3/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:47:23.000000 scrapwithgpt-0.1.3/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 14:22:27.751127 scrapwithgpt-0.1.4/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 14:22:27.750853 scrapwithgpt-0.1.4/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.4/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 14:22:27.749422 scrapwithgpt-0.1.4/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.4/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3639 2024-05-09 13:30:00.000000 scrapwithgpt-0.1.4/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.4/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4324 2024-05-09 13:49:38.000000 scrapwithgpt-0.1.4/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     5122 2024-05-09 13:47:50.000000 scrapwithgpt-0.1.4/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3262 2024-05-09 13:51:07.000000 scrapwithgpt-0.1.4/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    16221 2024-05-09 14:22:24.000000 scrapwithgpt-0.1.4/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 14:22:27.750490 scrapwithgpt-0.1.4/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 14:22:27.000000 scrapwithgpt-0.1.4/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 14:22:27.000000 scrapwithgpt-0.1.4/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 14:22:27.000000 scrapwithgpt-0.1.4/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 14:22:27.000000 scrapwithgpt-0.1.4/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 14:22:27.000000 scrapwithgpt-0.1.4/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 14:22:27.751172 scrapwithgpt-0.1.4/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 14:18:05.000000 scrapwithgpt-0.1.4/setup.py
```

### Comparing `scrapwithgpt-0.1.3/PKG-INFO` & `scrapwithgpt-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.3/scrapwithgpt/config.py` & `scrapwithgpt-0.1.4/scrapwithgpt/config.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.3/scrapwithgpt/oai.py` & `scrapwithgpt-0.1.4/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.3/scrapwithgpt/prompts.py` & `scrapwithgpt-0.1.4/scrapwithgpt/prompts.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.3/scrapwithgpt/scrap.py` & `scrapwithgpt-0.1.4/scrapwithgpt/scrap.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.3/scrapwithgpt/utils.py` & `scrapwithgpt-0.1.4/scrapwithgpt/utils.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.3/scrapwithgpt/web.py` & `scrapwithgpt-0.1.4/scrapwithgpt/web.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,32 +232,26 @@
     except SSLError as e:
         log_issue(e, fetch_content_url, f"SSL/TLS error for url {url}")
         return None
     except Exception as e:
         log_issue(e, fetch_content_url, f"For url {url}")
         return None
 
-def get_emails_from_soup(soup, domain, dom_only = True) -> list:
+def get_emails_from_soup(soup) -> list:
     """
     Function to extract all email addresses from the soup object.
     The function looks in the text of the soup.
     
     Args:
         soup (bs4.BeautifulSoup): BeautifulSoup object to search.
-        domain (str): Domain to restrict the emails to.
-        dom_only (bool): If True, restricts search to @domain emails only. If False, searches all emails.
         
     Returns:
         list: List of unique emails found. Can be empty.
     """
-    if dom_only:
-        emails = re.findall(r'\b[A-Za-z0-9._%+-]+@'+domain+r'\b', soup.get_text(), flags=re.IGNORECASE)
-    else:
-        emails = re.findall(r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', soup.get_text(), flags=re.IGNORECASE)
-    
+    emails = re.findall(r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', soup.get_text(), flags=re.IGNORECASE)
     # Convert emails to lowercase and ensures it is a valid email
     valid_emails = [email.lower() for email in emails if is_valid_email(email)]
     return list(set(valid_emails))  # Remove potential duplicates
 
 def get_linkedin_profiles_from_soup(soup) -> list:
     """
     Function to extract all LinkedIn profile links from the soup object.
```

### Comparing `scrapwithgpt-0.1.3/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.1.4/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.3/setup.py` & `scrapwithgpt-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.1.3", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.1.4", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```


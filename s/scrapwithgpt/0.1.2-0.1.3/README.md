# Comparing `tmp/scrapwithgpt-0.1.2.tar.gz` & `tmp/scrapwithgpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapwithgpt-0.1.2.tar", last modified: Thu May  9 13:43:23 2024, max compression
+gzip compressed data, was "scrapwithgpt-0.1.3.tar", last modified: Thu May  9 14:16:56 2024, max compression
```

## Comparing `scrapwithgpt-0.1.2.tar` & `scrapwithgpt-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:43:23.113040 scrapwithgpt-0.1.2/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:43:23.112812 scrapwithgpt-0.1.2/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.2/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:43:23.111760 scrapwithgpt-0.1.2/scrapwithgpt/
--rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.2/scrapwithgpt/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)     3639 2024-05-09 13:30:00.000000 scrapwithgpt-0.1.2/scrapwithgpt/config.py
--rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.2/scrapwithgpt/oai.py
--rw-r--r--   0 henry      (501) staff       (20)     4283 2024-05-09 13:30:52.000000 scrapwithgpt-0.1.2/scrapwithgpt/prompts.py
--rw-r--r--   0 henry      (501) staff       (20)     5096 2024-05-09 13:43:16.000000 scrapwithgpt-0.1.2/scrapwithgpt/scrap.py
--rw-r--r--   0 henry      (501) staff       (20)     3108 2024-05-09 09:34:18.000000 scrapwithgpt-0.1.2/scrapwithgpt/utils.py
--rw-r--r--   0 henry      (501) staff       (20)    13604 2024-05-09 13:33:33.000000 scrapwithgpt-0.1.2/scrapwithgpt/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 13:43:23.112591 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 13:43:23.000000 scrapwithgpt-0.1.2/scrapwithgpt.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 13:43:23.113087 scrapwithgpt-0.1.2/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:34:50.000000 scrapwithgpt-0.1.2/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 14:16:56.787886 scrapwithgpt-0.1.3/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 14:16:56.787659 scrapwithgpt-0.1.3/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      278 2024-05-09 12:31:59.000000 scrapwithgpt-0.1.3/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 14:16:56.786619 scrapwithgpt-0.1.3/scrapwithgpt/
+-rw-r--r--   0 henry      (501) staff       (20)      159 2024-05-09 12:31:09.000000 scrapwithgpt-0.1.3/scrapwithgpt/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)     3639 2024-05-09 13:30:00.000000 scrapwithgpt-0.1.3/scrapwithgpt/config.py
+-rw-r--r--   0 henry      (501) staff       (20)     7885 2024-05-09 13:31:23.000000 scrapwithgpt-0.1.3/scrapwithgpt/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)     4324 2024-05-09 13:49:38.000000 scrapwithgpt-0.1.3/scrapwithgpt/prompts.py
+-rw-r--r--   0 henry      (501) staff       (20)     5122 2024-05-09 13:47:50.000000 scrapwithgpt-0.1.3/scrapwithgpt/scrap.py
+-rw-r--r--   0 henry      (501) staff       (20)     3262 2024-05-09 13:51:07.000000 scrapwithgpt-0.1.3/scrapwithgpt/utils.py
+-rw-r--r--   0 henry      (501) staff       (20)    16548 2024-05-09 14:16:53.000000 scrapwithgpt-0.1.3/scrapwithgpt/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-09 14:16:56.787389 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)      539 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      353 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       51 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)       13 2024-05-09 14:16:56.000000 scrapwithgpt-0.1.3/scrapwithgpt.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-09 14:16:56.787928 scrapwithgpt-0.1.3/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      566 2024-05-09 13:47:23.000000 scrapwithgpt-0.1.3/setup.py
```

### Comparing `scrapwithgpt-0.1.2/PKG-INFO` & `scrapwithgpt-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.2/scrapwithgpt/config.py` & `scrapwithgpt-0.1.3/scrapwithgpt/config.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.2/scrapwithgpt/oai.py` & `scrapwithgpt-0.1.3/scrapwithgpt/oai.py`

 * *Files identical despite different names*

### Comparing `scrapwithgpt-0.1.2/scrapwithgpt/prompts.py` & `scrapwithgpt-0.1.3/scrapwithgpt/prompts.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         You are a rigorous analyst. 
         The user will provide you with content extracted from a website. You must analyze this content and return a JSON object with the information filled when available.
         ONLY use the content available, NEVER INVENT anything and follow strictly the below Instructions:
 
         ### Instructions: 
         1. Take your time and think step by step.
         2. Review and keep in mind ALL the fields of the below json structure: {json_output}
-        3. Go through the content provided by the user and try your best to fill the json accordingly. 
+        3. Go through the content provided by the user and try your best to fill the json accordingly. Take your time. Review the content several times.
         4. If the information is NOT in the content AT ALL, put NA.
         {example}
         ### Important considerations:
         - Follow strictly the Instructions. 
         - Remember that you must construct a JSON object with the provided keys, populated with the relevant information. If an information is not available at ALL or does not apply, use 'NA' for those fields.
         - Return the JSON and the JSON only. Do not preface by anything not even ```json before. 
         - Do your best, my job depends on the quality of your output.
@@ -58,16 +58,17 @@
     return remove_excess("""
     You are an expert at making summarizations that preserve ALL useful information.
     You take the text submitted by the user and return a detailed summary.
     You MUST ensure that you keep ALL relevant information about the main topic of the content.
                         
     ### Important Considerations: 
     - Do not include anything that is not in the provided text. ALWAYS be truthfull.
-    - Avoid puting recommendations like 'Subscribe to their newsletter for more information and updates'. REMOVE ALL reference to user action like 'individuals can subscribe to their monthly newsletter'.
+    - Do not include any recommendation. IMPORTANT, do not add useless suggestions like 'individuals can subscribe to their monthly newsletter'.
     - Do not preface the summary with anything. Do not put a title. Only return the summary and nothing else.
     - Ensure you keep ALL contact details (email or phone number). Do not consider a website URL as a contact information.
-    - Ensure you keep ALL numbers and factual informations.           
+    - Ensure you keep ALL numbers and factual informations.
+    Do your best, my job depends on the quality of your work.
     """)
 
 # *************************************************************
 if __name__ == "__main__":
     pass
```

### Comparing `scrapwithgpt-0.1.2/scrapwithgpt/scrap.py` & `scrapwithgpt-0.1.3/scrapwithgpt/scrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,18 @@
             if not answer_from_filtergpt:
                 if verbose: print("Couldn't check the Criteria - END")
                 return
             elif "false" in answer_from_filtergpt[:10].lower(): 
                 if verbose: print(f"The website is NOT relevant according to the Criteria. Response: {answer_from_filtergpt} - END")
                 return
         if summarization:
-            if verbose: print(f"👷‍♂️ Generating a summary")   
+            if verbose: print(f"👷‍♂️ Generating a summary of the website content")   
             summary = ask_question_gpt(content, gen_role_summarizer(), max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE,  verbose=False)
         
-        if verbose: print(f"👷‍♂️ Using GPT 4 to  the requested data")  
+        if verbose: print(f"👷‍♂️ Using GPT 4 to get the requested data")  
         result = ask_question_gpt4(content, gen_prompt_result(desired_output, example_output, additional_consideration), max_tokens=MAX_TOKEN_GPT4_RESULT,  verbose=False)
         if result:
             title = f"scrapwithgpt_{clean_url_to_filename(url)}.txt"
             if os.path.exists(title):
                 title = f"scrapwithgpt_{clean_url_to_filename(url)}_{get_now(True)}.txt" # To avoid overwriting
             if summary:
                 final_content = f"### SUMMARY of {url}:\n" + summary.replace(".", ".\n") + "\n\n"
```

### Comparing `scrapwithgpt-0.1.2/scrapwithgpt/utils.py` & `scrapwithgpt-0.1.3/scrapwithgpt/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,10 +82,16 @@
     Small function to get the timestamp in string format.
     By default we return the following format: "10_Jan_2023" but if exact is True, we will return 10_Jan_2023_@15h23s33
     """
     now = datetime.datetime.now()
     return datetime.datetime.strftime(now, "%d_%b_%Y@%Hh%Ms%S") if exact else datetime.datetime.strftime(now, "%d_%b_%Y")
 
 
+def is_valid_email(email):
+    '''
+    Not the best but a first regex protection.
+    '''
+    return bool(re.search(r"^[\w\.-]+@[\w\.-]+\.\w+$", email))
+
 # *************************************************************
 if __name__ == "__main__":
     pass
```

### Comparing `scrapwithgpt-0.1.2/scrapwithgpt/web.py` & `scrapwithgpt-0.1.3/scrapwithgpt/web.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #   Functions related to fetching content from the web
 
 
 from .config import HEADERS, HTTP_URL_PATTERN
-from .utils import log_issue, remove_excess, remove_non_printable
+from .utils import log_issue, remove_excess, remove_non_printable, is_valid_email
 
 
 from urllib.parse import urlparse, urlunparse, quote, unquote
 from requests.adapters import HTTPAdapter
 from requests.exceptions import SSLError
 from urllib3.util.retry import Retry
 from urllib.parse import urljoin
@@ -137,14 +137,15 @@
     """
     submitted = 0
     if not memory_store:
         memory_store = {}  # In-memory storage for crawled data
     local_domain = urlparse(url).netloc 
     queue = deque([url])
     seen = set([url])
+    linkedin, emails = [], []
     with concurrent.futures.ThreadPoolExecutor() as executor:
         while queue:
             url = queue.pop()
             if not check_valid_url(url):
                 continue
             response = session.head(url, headers=HEADERS)
             content_type = response.headers.get("content-type", "")
@@ -152,42 +153,62 @@
                 continue
             data_name = clean_url_into_title(url)
             future = executor.submit(fetch_content_url, url)
             submitted += 1
             if submitted == how_many_pages:
                 break
             future.add_done_callback(lambda future: wrap_handle_fetch_result(future, data_name, memory_store))
-            for link in fetch_domain_links(local_domain, url):
+            links_contact = fetch_domain_links_and_contact(local_domain, url)
+            linkedin += links_contact["linkedin"]
+            emails += links_contact["emails"]
+            for link in links_contact["links"]:
                 if link not in seen:
                     queue.append(link)
                     seen.add(link)
+    # Adding linkedin and emails info at the beginning
+    linkedin = list(set(linkedin))
+    if linkedin: 
+        linkedin = ", ".join(str(elem) for elem in linkedin)
+        dict_linkedin = {"linkedin_found": linkedin}
+        memory_store = {**dict_linkedin, **memory_store}
+    emails = list(set(emails))
+    if emails: 
+        emails = ", ".join(str(elem) for elem in emails)
+        dict_emails = {"email_found": emails}
+        memory_store = {**dict_emails, **memory_store}
     return memory_store
 
-def fetch_hyperlinks(url: str) -> list[str]:
+
+def fetch_hyperlinks_and_contact(url: str) -> dict:
     """
-    Fetch and returns all hyperlinks from a given URL, filtering out non-HTML content and irrelevant links.
+    Fetch and returns all hyperlinks, emails, and linkeding profile from a given URL, filtering out non-HTML content and irrelevant links.
 
-    Returns a list with all the useful links present in a page.
+    Returns a dict with the following structure:
+        {"links":[], "emails":[], "linkedin":[]}
     """
+    result = {"links":[], "emails":[], "linkedin":[]}
     try:
         response = requests.get(url, headers=HEADERS)
         if not response.headers.get('Content-Type', '').startswith('text/html'):
             return []
         html = response.text
     except Exception as e:
-        log_issue(e, fetch_hyperlinks, f"Couldn't fetch the links of url {url}")
+        log_issue(e, fetch_hyperlinks_and_contact, f"Couldn't fetch the links of url {url}")
         return []
 
     soup = BeautifulSoup(html, 'html.parser')
     links = [link.get('href') for link in soup.find_all('a') if link.get('href')]
 
     filtered_links = [link for link in links if not (
         link.startswith(('javascript:', 'mailto:', '#')) or '://' not in link and not link.startswith('/')
     )]
-    return filtered_links
+    result["links"] = filtered_links
+    result["emails"] = get_emails_from_soup(soup)
+    result["linkedin"] = get_linkedin_profiles_from_soup(soup)
+    return result
 
 # Fetch URL - works as a standalone
 # Might want to test the driver version with selenium - driver = webdriver.Firefox()
 def fetch_content_url(url: str, attempt: int = 0) -> Optional[str]:
     """
     Fetch and clean content from a webpage. 
     Returns the clean content or None if issue.
@@ -211,14 +232,56 @@
     except SSLError as e:
         log_issue(e, fetch_content_url, f"SSL/TLS error for url {url}")
         return None
     except Exception as e:
         log_issue(e, fetch_content_url, f"For url {url}")
         return None
 
+def get_emails_from_soup(soup, domain, dom_only = True) -> list:
+    """
+    Function to extract all email addresses from the soup object.
+    The function looks in the text of the soup.
+    
+    Args:
+        soup (bs4.BeautifulSoup): BeautifulSoup object to search.
+        domain (str): Domain to restrict the emails to.
+        dom_only (bool): If True, restricts search to @domain emails only. If False, searches all emails.
+        
+    Returns:
+        list: List of unique emails found. Can be empty.
+    """
+    if dom_only:
+        emails = re.findall(r'\b[A-Za-z0-9._%+-]+@'+domain+r'\b', soup.get_text(), flags=re.IGNORECASE)
+    else:
+        emails = re.findall(r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b', soup.get_text(), flags=re.IGNORECASE)
+    
+    # Convert emails to lowercase and ensures it is a valid email
+    valid_emails = [email.lower() for email in emails if is_valid_email(email)]
+    return list(set(valid_emails))  # Remove potential duplicates
+
+def get_linkedin_profiles_from_soup(soup) -> list:
+    """
+    Function to extract all LinkedIn profile links from the soup object.
+    The function looks for href attributes within 'a' tags in the HTML.
+    
+    Args:
+        soup (bs4.BeautifulSoup): BeautifulSoup object to search.
+        
+    Returns:
+        list: List of unique LinkedIn profile links found. Can be empty.
+    """
+    linkedin_urls = set()
+    for a_tag in soup.find_all('a', href=True):
+        href = a_tag['href']
+        # Regular expression to match LinkedIn profile URLs
+        if re.search(r'https?://www\.linkedin\.com/in/[^/]+/?$', href):
+            linkedin_urls.add(href)
+
+    return list(linkedin_urls)
+
 def is_useful_link(tag) -> bool:
     """
     Mini function to check if a link is surrounded with content, hence useful, or alone.
     Return True if useful, False otherwise.
     """
    # Check previous and next siblings
     prev_sibling = tag.previous_sibling
@@ -231,25 +294,30 @@
     parent = tag.parent
     if parent:
         text_without_link = parent.get_text().replace(tag.get_text(), '').strip()
         if text_without_link:
             return True
     return False
 
-def fetch_domain_links(local_domain, url) -> set:
+def fetch_domain_links_and_contact(local_domain, url) -> set:
     """
-    Returns the list of all unique urls of a given domain. Search start from a specific page (url).
+    Returns the list of all unique urls of a given domain and the related contact info of the page. Search start from a specific page (url).
     Doesn't return links that are not part of the domain.
+    
+    Returns:
+        (dict) with the following structure {"links":[], "emails":[], "linkedin":[]}
     """
     clean_links = set()
     try:
-        raw_links = fetch_hyperlinks(url)
+        result = fetch_hyperlinks_and_contact(url)
+        raw_links = result["links"]
         if raw_links is None:
-            print("No hyperlink", fetch_domain_links, f"For {url} and {local_domain}")
-            return []
+            log_issue("No hyperlink", fetch_domain_links_and_contact, f"For {url} and {local_domain}")
+            result["links"] = []
+            return result
         for link in set(raw_links):
             if link is None:
                 continue
             valid_link = False
             # If the link is a URL, check if it is within the same domain
             if re.search(HTTP_URL_PATTERN, link):
                 if urlparse(link).netloc == local_domain: # to check that the domain is the same
@@ -264,17 +332,17 @@
                 else:
                     valid_link = urljoin(url, link)            
             if valid_link:
                 if valid_link.endswith("/"):
                     valid_link = valid_link[:-1]
                 clean_links.add(valid_link)
     except Exception as e:
-        log_issue(e, fetch_domain_links, f"For {url} and {local_domain}")
-    return clean_links
-
+        log_issue(e, fetch_domain_links_and_contact, f"For {url} and {local_domain}")
+    result["links"] = clean_links
+    return result
 
 def remove_citations(soup: BeautifulSoup) -> BeautifulSoup:
     """
     Remove citation tags from a BeautifulSoup object.
     """
     for tag in soup.find_all(lambda t: t.has_attr('id') and 'cite_note' in t['id']):
         tag.decompose()
```

### Comparing `scrapwithgpt-0.1.2/scrapwithgpt.egg-info/PKG-INFO` & `scrapwithgpt-0.1.3/scrapwithgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapwithgpt
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/HenryObj/scrapwithgpt
 Description-Content-Type: text/markdown
 Requires-Dist: openai>=1.9.0
 Requires-Dist: tiktoken>=0.5.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: bs4
```

### Comparing `scrapwithgpt-0.1.2/setup.py` & `scrapwithgpt-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="scrapwithgpt",
-    version="0.1.2", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.1.3", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/scrapwithgpt',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```


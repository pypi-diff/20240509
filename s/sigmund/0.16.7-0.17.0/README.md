# Comparing `tmp/sigmund-0.16.7.tar.gz` & `tmp/sigmund-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmund-0.16.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sigmund-0.17.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sigmund-0.16.7.tar` & `sigmund-0.17.0.tar`

### file list

```diff
@@ -1,58 +1,61 @@
--rw-r--r--   0        0        0    35147 2024-05-02 08:58:09.926576 sigmund-0.16.7/COPYING
--rw-r--r--   0        0        0     1017 2024-05-02 08:58:09.926576 sigmund-0.16.7/pyproject.toml
--rw-r--r--   0        0        0     3037 2024-05-02 08:58:09.926576 sigmund-0.16.7/readme.md
--rw-r--r--   0        0        0      101 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/__init__.py
--rw-r--r--   0        0        0     2746 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/attachments.py
--rw-r--r--   0        0        0     9770 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/config.py
--rw-r--r--   0        0        0        0 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/database/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/database/encryption.py
--rw-r--r--   0        0        0    14378 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/database/manager.py
--rw-r--r--   0        0        0     3213 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/database/models.py
--rw-r--r--   0        0        0     6331 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/documentation.py
--rw-r--r--   0        0        0      389 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/forms.py
--rw-r--r--   0        0        0     2547 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/library.py
--rw-r--r--   0        0        0    10115 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/messages.py
--rw-r--r--   0        0        0     1252 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/model/__init__.py
--rw-r--r--   0        0        0     5297 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/model/_anthropic_model.py
--rw-r--r--   0        0        0     4756 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/model/_base_model.py
--rw-r--r--   0        0        0      379 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/model/_dummy_model.py
--rw-r--r--   0        0        0     2700 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/model/_mistral_model.py
--rw-r--r--   0        0        0     3428 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/model/_openai_model.py
--rw-r--r--   0        0        0     2141 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/prompt.py
--rw-r--r--   0        0        0      160 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/routes/__init__.py
--rw-r--r--   0        0        0     7298 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/routes/api.py
--rw-r--r--   0        0        0     5775 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/routes/app.py
--rw-r--r--   0        0        0     3769 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/routes/google_login.py
--rw-r--r--   0        0        0     7733 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/routes/subscribe.py
--rw-r--r--   0        0        0     1494 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/server.py
--rw-r--r--   0        0        0     9354 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/sigmund.py
--rw-r--r--   0        0        0     4471 2024-05-02 08:58:09.926576 sigmund-0.16.7/sigmund/static/about.md
--rw-r--r--   0        0        0  4708018 2024-05-02 08:58:09.934576 sigmund-0.16.7/sigmund/static/background.png
--rw-r--r--   0        0        0      386 2024-05-02 08:58:09.934576 sigmund-0.16.7/sigmund/static/favicon.svg
--rw-r--r--   0        0        0     1433 2024-05-02 08:58:09.934576 sigmund-0.16.7/sigmund/static/login.md
--rw-r--r--   0        0        0     4976 2024-05-02 08:58:09.934576 sigmund-0.16.7/sigmund/static/pygments.css
--rw-r--r--   0        0        0   708136 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/static/sofa-with-sigmund.png
--rw-r--r--   0        0        0   684883 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/static/sofa.png
--rw-r--r--   0        0        0     3428 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/static/terms.md
--rw-r--r--   0        0        0     1359 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/chat.html
--rw-r--r--   0        0        0      242 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/footer.html
--rw-r--r--   0        0        0      574 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/head.html
--rw-r--r--   0        0        0      244 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/header.html
--rw-r--r--   0        0        0      329 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/info-page.html
--rw-r--r--   0        0        0     3739 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/login.html
--rw-r--r--   0        0        0    10786 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/main.js
--rw-r--r--   0        0        0    12359 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/menu.html
--rw-r--r--   0        0        0       80 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/sign-out.html
--rw-r--r--   0        0        0     6380 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/stylesheet.css.jinja
--rw-r--r--   0        0        0      531 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/subscribe-error.html
--rw-r--r--   0        0        0     1555 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/subscribe-now.html
--rw-r--r--   0        0        0      515 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/templates/subscribe-success.html
--rw-r--r--   0        0        0      265 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/tools/__init__.py
--rw-r--r--   0        0        0     2231 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/tools/_base_tool.py
--rw-r--r--   0        0        0     2920 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/tools/_download.py
--rw-r--r--   0        0        0     2085 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/tools/_execute_code.py
--rw-r--r--   0        0        0     1846 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/tools/_read_attachment.py
--rw-r--r--   0        0        0     2076 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/tools/_search_documentation.py
--rw-r--r--   0        0        0     1275 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/tools/_search_google_scholar.py
--rw-r--r--   0        0        0     4335 2024-05-02 08:58:09.938577 sigmund-0.16.7/sigmund/utils.py
--rw-r--r--   0        0        0     4228 1970-01-01 00:00:00.000000 sigmund-0.16.7/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-09 09:19:47.574150 sigmund-0.17.0/COPYING
+-rw-r--r--   0        0        0     1036 2024-05-09 09:19:47.574150 sigmund-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0     3037 2024-05-09 09:19:47.574150 sigmund-0.17.0/readme.md
+-rw-r--r--   0        0        0      101 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/__init__.py
+-rw-r--r--   0        0        0     2746 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/attachments.py
+-rw-r--r--   0        0        0    10293 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/config.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/database/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/database/encryption.py
+-rw-r--r--   0        0        0    14378 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/database/manager.py
+-rw-r--r--   0        0        0     3213 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/database/models.py
+-rw-r--r--   0        0        0     7153 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/documentation.py
+-rw-r--r--   0        0        0      389 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/forms.py
+-rw-r--r--   0        0        0     2541 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/library.py
+-rw-r--r--   0        0        0    10115 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/messages.py
+-rw-r--r--   0        0        0     1415 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/model/__init__.py
+-rw-r--r--   0        0        0     5297 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/model/_anthropic_model.py
+-rw-r--r--   0        0        0     4756 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/model/_base_model.py
+-rw-r--r--   0        0        0      379 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/model/_dummy_model.py
+-rw-r--r--   0        0        0     2700 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/model/_mistral_model.py
+-rw-r--r--   0        0        0     3428 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/model/_openai_model.py
+-rw-r--r--   0        0        0     2384 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/prompt.py
+-rw-r--r--   0        0        0      197 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/routes/__init__.py
+-rw-r--r--   0        0        0     7334 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/routes/api.py
+-rw-r--r--   0        0        0     5776 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/routes/app.py
+-rw-r--r--   0        0        0     3769 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/routes/google_login.py
+-rw-r--r--   0        0        0     1838 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/routes/public.py
+-rw-r--r--   0        0        0     7733 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/routes/subscribe.py
+-rw-r--r--   0        0        0     1580 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/server.py
+-rw-r--r--   0        0        0     9430 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/sigmund.py
+-rw-r--r--   0        0        0     4471 2024-05-09 09:19:47.574150 sigmund-0.17.0/sigmund/static/about.md
+-rw-r--r--   0        0        0  4708018 2024-05-09 09:19:47.582150 sigmund-0.17.0/sigmund/static/background.png
+-rw-r--r--   0        0        0      386 2024-05-09 09:19:47.582150 sigmund-0.17.0/sigmund/static/favicon.svg
+-rw-r--r--   0        0        0     1433 2024-05-09 09:19:47.582150 sigmund-0.17.0/sigmund/static/login.md
+-rw-r--r--   0        0        0     4976 2024-05-09 09:19:47.582150 sigmund-0.17.0/sigmund/static/pygments.css
+-rw-r--r--   0        0        0   708136 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/static/sofa-with-sigmund.png
+-rw-r--r--   0        0        0   684883 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/static/sofa.png
+-rw-r--r--   0        0        0     3428 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/static/terms.md
+-rw-r--r--   0        0        0     1359 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/chat.html
+-rw-r--r--   0        0        0      242 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/footer.html
+-rw-r--r--   0        0        0      574 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/head.html
+-rw-r--r--   0        0        0      244 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/header.html
+-rw-r--r--   0        0        0      329 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/info-page.html
+-rw-r--r--   0        0        0     3739 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/login.html
+-rw-r--r--   0        0        0    10786 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/main.js
+-rw-r--r--   0        0        0    12359 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/menu.html
+-rw-r--r--   0        0        0      503 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/search-widget.html
+-rw-r--r--   0        0        0     7676 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/search-widget.js
+-rw-r--r--   0        0        0       80 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/sign-out.html
+-rw-r--r--   0        0        0     6380 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/stylesheet.css.jinja
+-rw-r--r--   0        0        0      531 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/subscribe-error.html
+-rw-r--r--   0        0        0     1555 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/subscribe-now.html
+-rw-r--r--   0        0        0      515 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/templates/subscribe-success.html
+-rw-r--r--   0        0        0      265 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/tools/__init__.py
+-rw-r--r--   0        0        0     2231 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/tools/_base_tool.py
+-rw-r--r--   0        0        0     2920 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/tools/_download.py
+-rw-r--r--   0        0        0     2085 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/tools/_execute_code.py
+-rw-r--r--   0        0        0     1846 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/tools/_read_attachment.py
+-rw-r--r--   0        0        0     2076 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/tools/_search_documentation.py
+-rw-r--r--   0        0        0     1275 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/tools/_search_google_scholar.py
+-rw-r--r--   0        0        0     4335 2024-05-09 09:19:47.586150 sigmund-0.17.0/sigmund/utils.py
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 sigmund-0.17.0/PKG-INFO
```

### Comparing `sigmund-0.16.7/COPYING` & `sigmund-0.17.0/COPYING`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/pyproject.toml` & `sigmund-0.17.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "anthropic",
     "cryptography",
     "faiss-cpu",
     "flask",
     "flask-login",
     "flask-sqlalchemy",
     "flask-wtf",
+    "flask-cors",
     "jinja2",
     "jq",
     "langchain",
     "langchain_core",
     "langchain_community",
     "langchain_openai",
     "langchain_anthropic",
@@ -43,8 +44,8 @@
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov"
 ]
 [project.urls]
 Documentation = "https://sigmundai.eu"
-Source = "https://github.com/smathot/sigmundai"
+Source = "https://github.com/smathot/sigmundai"
```

### Comparing `sigmund-0.16.7/readme.md` & `sigmund-0.17.0/readme.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/attachments.py` & `sigmund-0.17.0/sigmund/attachments.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/config.py` & `sigmund-0.17.0/sigmund/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,29 +104,33 @@
 #   conversation becomes too long. This can also be a cheap model.
 # - The answermodel generates the actual answer. This should be a very capable
 #   model
 model_config = {
     'openai': {
         'search_model': 'gpt-3.5',
         'condense_model': 'gpt-3.5',
+        'public_model': 'claude-3-haiku',
         'answer_model': 'gpt-4'
     },
     'anthropic': {
         'search_model': 'claude-3-sonnet',
         'condense_model': 'claude-3-sonnet',
+        'public_model': 'claude-3-haiku',
         'answer_model': 'claude-3-opus'
     },
     'mistral': {
         'search_model': 'mistral-large',
         'condense_model': 'mistral-medium',
+        'public_model': 'claude-3-haiku',
         'answer_model': 'mistral-large'
     },
     'dummy': {
         'search_model': 'dummy',
         'condense_model': 'dummy',
+        'public_model': 'dummy',
         'answer_model': 'dummy'
     }
 }
 # Model-specific keyword arguments that are passed to the message generation
 # functions
 anthropic_kwargs = {
     'max_tokens': 1024
@@ -171,21 +175,32 @@
     'data_analysis': 'sources/topics/datamatrix.py',
     'questions_howto': 'sources/topics/questions-how-to.md',
 }
 # The number of documents that is considered for each search query
 search_docs_per_query = 20
 # The number of documents that is kept for all search queries combined
 search_docs_max = 6
+# The distance metric to search through documentation. Should be 'cosine' or
+# 'euclidean_distance'
+search_docs_distance_metric = 'cosine'
+# The number of documents and maximum number of words that is kept for public 
+# search
+public_search_docs_max = 6
+public_search_max_doc_length = 1000
 # The distance metric used for search. The cosine metric is useful because it
 # is somewhat invariant to changes in document length
 search_metric = 'cosine'
-# The cache folder for the library that is used to chat
-db_cache = '.db.cache'
-# The cache folder for the library that is used for public search
-public_search_cache = '.ps.cache'
+# The cache folder for the library that contains documentation
+db_cache = 'default'
+db_cache_sources = {
+    'default': '.db.cache',
+    'public-with-forum': '.public-with-forum.db.cache',
+    'public-without-forum': '.public-without-forum.db.cache'
+}
+
 
 def process_ai_message(msg):
     # This pattern looks for a colon possibly followed by any number of 
     # whitespaces # and/or HTML tags, followed by a newline and a dash, and 
     # replaces it with a colon, newline, newline, and dash
     pattern = r':\s*(<[^>]+>\s*)?\n-'
     replacement = ':\n\n-'
```

### Comparing `sigmund-0.16.7/sigmund/database/encryption.py` & `sigmund-0.17.0/sigmund/database/encryption.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/database/manager.py` & `sigmund-0.17.0/sigmund/database/manager.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/database/models.py` & `sigmund-0.17.0/sigmund/database/models.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/documentation.py` & `sigmund-0.17.0/sigmund/documentation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import json
 from pathlib import Path
 from langchain_openai import OpenAIEmbeddings
 from langchain_community.vectorstores import FAISS
+from langchain_community.vectorstores.utils import DistanceStrategy
 from langchain_core.documents import Document
 import logging
 from . import config
 from . import prompt
 logger = logging.getLogger('sigmund')
 
 
 class Documentation:
     
     def __init__(self, sigmund, sources=[]):
         self._sigmund = sigmund
         self._documents = []
         self._sources = sources
         
+    def _doc_to_str(self, doc):
+        s = '<document>\n'
+        if doc.metadata.get('title', None):
+            s += f'# {doc.metadata["title"]}\n\n'
+        if doc.metadata.get('url', None):
+            s += f'Source: {doc.metadata["url"]}\n\n'
+        return s + doc.page_content + '\n</document>'
+        
     def __str__(self):
         if not self._documents:
             return ''
-        return '\n\n'.join(
-            f"<document>{doc.page_content}</document>" for doc in self._documents)
+        return '\n\n'.join(self._doc_to_str(doc) for doc in self._documents)
         
     def to_json(self):
         return json.dumps([{'page_content': doc.page_content,
                             'url': doc.metadata.get('url', None)}
                            for doc in self])
         
     def __iter__(self):
@@ -113,25 +121,33 @@
         if config.openai_api_key is None:
             logger.warning(
                 'No OpenAI API key provided, no documentation available')
             return
         self._embeddings_model = OpenAIEmbeddings(
             openai_api_key=config.openai_api_key)
         logger.info('reading FAISS documentation cache')
-        self._db = FAISS.load_local(Path('.db.cache'), self._embeddings_model,
+        db_cache = config.db_cache_sources[config.db_cache]
+        self._db = FAISS.load_local(Path(db_cache), self._embeddings_model,
                                     allow_dangerous_deserialization=True)
-    
+        if config.search_docs_distance_metric == 'cosine':
+            self._db.distance_strategy = DistanceStrategy.COSINE
+        elif config.search_docs_distance_metric == 'euclidean_distance':
+            self._db.distance_strategy = DistanceStrategy.EUCLIDEAN_DISTANCE
+        else:
+            raise ValueError(
+                f'invalid search_docs_distance_metric: {config.search_docs_distance_metric}')
+
     def search(self, queries):
         if config.openai_api_key is None:
             return []
         docs = []
         for query in queries:
             if config.log_replies:
                 logger.info(f'documentation search query: {query}')
-            for doc, score in self._db.similarity_search_with_score(
+            for doc, score in self._db.similarity_search_with_relevance_scores(
                     query, k=config.search_docs_per_query):
                 doc_desc = f'{doc.metadata["url"]} ({doc.metadata["seq_num"]})'
                 if any(doc.page_content == ref.page_content for ref, _ in docs):
                     continue
                 if doc.page_content not in self._sigmund.documentation and \
                         doc.page_content not in docs:
                     docs.append((doc, score))
```

### Comparing `sigmund-0.16.7/sigmund/library.py` & `sigmund-0.17.0/sigmund/library.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 import openai
 import time
 from . import config
 logger = logging.getLogger('sigmund')
 
 
 def load_library(force_reindex=False, cache_folder=config.db_cache,
-                 exclude_filter=None):
+                 exclude_filter=[]):
     db_cache = Path(cache_folder)
     src_path = Path('sources')
     embeddings_model = OpenAIEmbeddings(openai_api_key=config.openai_api_key)
     if not force_reindex and db_cache.exists():
         logger.info('loading library from cache')
         db = FAISS.load_local(db_cache, embeddings_model,
                               allow_dangerous_deserialization=True)
     else:
         from langchain_community.document_loaders import TextLoader, \
             PyPDFLoader, JSONLoader
         logger.info('initializing library')
         data = []
         # PDF files are unstructured. They can be named through config.sources
         for src in src_path.glob('pdf/**/*.pdf'):
-            if exclude_filter and exclude_filter in str(src):
+            if any(f in str(src) for f in exclude_filter):
                 logger.info(f'skipping pdf: {src}')
                 continue
             logger.info(f'indexing pdf: {src}')
             data += PyPDFLoader(str(src)).load_and_split()
         # jsonl is mainly for documentation
         for src in src_path.glob('jsonl/*.jsonl'):
             logger.info(f'indexing json: {src}')
-            if exclude_filter and exclude_filter in str(src):
+            if any(f in str(src) for f in exclude_filter):
                 logger.info(f'skipping json: {src}')
                 continue            
-            loader = JSONLoader(src, jq_schema='', content_key='content',
+            loader = JSONLoader(src, jq_schema='.', content_key='content',
                                 json_lines=True,
                                 metadata_func=_extract_metadata)
             data += loader.load()
         # To avoid running into rate limits, we throttle the ingestion of the
         # documents
         for i in range(0, len(data), config.chunk_size):
             logger.info(
@@ -54,8 +54,8 @@
         logger.info(f'libary initialized')
     return db.as_retriever()
 
 
 def _extract_metadata(record, metadata):
     metadata['url'] = record.get('url', record.get('source', None))
     metadata['title'] = record['title']
-    return metadata
+    return metadata
```

### Comparing `sigmund-0.16.7/sigmund/messages.py` & `sigmund-0.17.0/sigmund/messages.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/model/__init__.py` & `sigmund-0.17.0/sigmund/model/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,17 @@
         return AnthropicModel(sigmund, 'claude-2.1', **kwargs)
     if model == 'claude-3-opus':
         from ._anthropic_model import AnthropicModel
         return AnthropicModel(sigmund, 'claude-3-opus-20240229', **kwargs)
     if model == 'claude-3-sonnet':
         from ._anthropic_model import AnthropicModel
         return AnthropicModel(sigmund, 'claude-3-sonnet-20240229', **kwargs)
+    if model == 'claude-3-haiku':
+        from ._anthropic_model import AnthropicModel
+        return AnthropicModel(sigmund, 'claude-3-haiku-20240307', **kwargs)
     if model.startswith('mistral-'):
         from ._mistral_model import MistralModel
         if not model.endswith('-latest'):
             model += '-latest'
         return MistralModel(sigmund, model, **kwargs)
     if model == 'dummy':
         from ._dummy_model import DummyModel
```

### Comparing `sigmund-0.16.7/sigmund/model/_anthropic_model.py` & `sigmund-0.17.0/sigmund/model/_anthropic_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/model/_base_model.py` & `sigmund-0.17.0/sigmund/model/_base_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/model/_mistral_model.py` & `sigmund-0.17.0/sigmund/model/_mistral_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/model/_openai_model.py` & `sigmund-0.17.0/sigmund/model/_openai_model.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/prompt.py` & `sigmund-0.17.0/sigmund/prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,11 +49,15 @@
 DESCRIBE_PROMPT = '''Provide a brief description of the following text:
         
 Filename: {{ name }}
         
 <TEXT>
 {{ text_representation }}
 </TEXT>'''
+PUBLIC_SEARCH_PROMPT = '''For each of the documentation sections below, provide a summary in a single bullet point using this format: "- [title](url): description (max 2 sentences)". Only reply with bullet points.
+    
+{{ documentation }}
+'''
 
 
 def render(tmpl, **kwargs):
     return jinja2.Template(tmpl).render(**kwargs)
```

### Comparing `sigmund-0.16.7/sigmund/routes/api.py` & `sigmund-0.17.0/sigmund/routes/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import base64
 import logging
 from werkzeug.utils import secure_filename
 from flask import request, jsonify, Response, redirect, session, \
     stream_with_context, make_response, Blueprint
 from flask_login import login_required
 from .. import config, utils, attachments
+from ..sigmund import Sigmund
 from .app import get_sigmund
 from redis import Redis
 logger = logging.getLogger('sigmund')
 api_blueprint = Blueprint('api', __name__)
 redis_client = Redis()
 
 
@@ -207,8 +208,9 @@
     if value is None:
         if key in config.settings_default:
             value = config.settings_default[key]
             logger.info(f'using default setting for {key}: {value}')
         else:
             return jsonify(success=False, value=value)
     logger.info(f'get setting: {key} = {value}')
-    return jsonify(success=True, value=value)
+    return jsonify(success=True, value=value)
+
```

### Comparing `sigmund-0.16.7/sigmund/routes/app.py` & `sigmund-0.17.0/sigmund/routes/app.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -147,8 +147,8 @@
     return redirect(url_for('app.login'))
 
 
 @app_blueprint.route('/chat')
 def chat():
     if current_user.is_authenticated:
         return chat_page()
-    return redirect(url_for('app.login'))
+    return redirect(url_for('app.login'))
```

### Comparing `sigmund-0.16.7/sigmund/routes/google_login.py` & `sigmund-0.17.0/sigmund/routes/google_login.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/routes/subscribe.py` & `sigmund-0.17.0/sigmund/routes/subscribe.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/server.py` & `sigmund-0.17.0/sigmund/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 os.environ['USE_FLASK_SQLALCHEMY'] = '1'
 from flask import Flask, Config, request
 from flask_login import LoginManager
 from . import config
 from .routes import api_blueprint, app_blueprint, User, subscribe_blueprint, \
-    google_login_blueprint
+    google_login_blueprint, public_blueprint
 from .database.models import db
 import logging
 logger = logging.getLogger('sigmund')
 logging.basicConfig(level=logging.INFO, force=True)
 
 
 class SigmundConfig(Config):
@@ -19,14 +19,15 @@
 def create_app(config_class=SigmundConfig):
     app = Flask(__name__, static_url_path='/static')
     app.config.from_object(config_class)
     app.register_blueprint(app_blueprint)
     app.register_blueprint(api_blueprint, url_prefix='/api')
     app.register_blueprint(subscribe_blueprint, url_prefix='/subscribe')
     app.register_blueprint(google_login_blueprint, url_prefix='/google_login')
+    app.register_blueprint(public_blueprint, url_prefix='/public')
     # Initialize the databasea
     db.init_app(app)
     with app.app_context():
         db.create_all()
     # Initialize login manager
     login_manager = LoginManager()
     
@@ -39,8 +40,8 @@
     @app.after_request
     def log_request(response):
         user_agent = request.headers.get('User-Agent')
         if user_agent is not None and 'bot' not in user_agent.lower():
             logger.info(f'request: {request.full_path}')
         return response
 
-    return app
+    return app
```

### Comparing `sigmund-0.16.7/sigmund/sigmund.py` & `sigmund-0.17.0/sigmund/sigmund.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         self.search_model = model(self, self.model_config['search_model'],
                                   tools=self.search_tools, 
                                   tool_choice=search_tool_choice)
         self.answer_model = model(self, self.model_config['answer_model'],
                                   tools=self.answer_tools,
                                   tool_choice=answer_tool_choice)
         self.condense_model = model(self, self.model_config['condense_model'])
+        self.public_model = model(self, self.model_config['public_model'])
     
     def send_user_message(self, message: str,
                           message_id: str=None) -> GeneratorType:
         """The main function that takes a user message and returns one or 
         replies. This is a generator function where each yield gives a tuple.
         
         This tuple can be (dict, dict) in which case the first dict contains an 
@@ -181,8 +182,8 @@
                 needs_feedback = True
             else:
                 needs_feedback = False
         # If feedback is required, either because the tools require it or 
         # because the AI sent a NOT_DONE_YET marker, go for another round.
         if needs_feedback and not self._rate_limit_exceeded():
             for reply, metadata in self._answer(state='feedback'):
-                yield reply, metadata
+                yield reply, metadata
```

### Comparing `sigmund-0.16.7/sigmund/static/about.md` & `sigmund-0.17.0/sigmund/static/about.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/static/background.png` & `sigmund-0.17.0/sigmund/static/background.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/static/login.md` & `sigmund-0.17.0/sigmund/static/login.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/static/pygments.css` & `sigmund-0.17.0/sigmund/static/pygments.css`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/static/sofa-with-sigmund.png` & `sigmund-0.17.0/sigmund/static/sofa-with-sigmund.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/static/sofa.png` & `sigmund-0.17.0/sigmund/static/sofa.png`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/static/terms.md` & `sigmund-0.17.0/sigmund/static/terms.md`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/templates/chat.html` & `sigmund-0.17.0/sigmund/templates/chat.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/templates/head.html` & `sigmund-0.17.0/sigmund/templates/head.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/templates/login.html` & `sigmund-0.17.0/sigmund/templates/login.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/templates/main.js` & `sigmund-0.17.0/sigmund/templates/main.js`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/templates/menu.html` & `sigmund-0.17.0/sigmund/templates/menu.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/templates/stylesheet.css.jinja` & `sigmund-0.17.0/sigmund/templates/stylesheet.css.jinja`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/templates/subscribe-error.html` & `sigmund-0.17.0/sigmund/templates/subscribe-error.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/templates/subscribe-now.html` & `sigmund-0.17.0/sigmund/templates/subscribe-now.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/templates/subscribe-success.html` & `sigmund-0.17.0/sigmund/templates/subscribe-success.html`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/tools/_base_tool.py` & `sigmund-0.17.0/sigmund/tools/_base_tool.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/tools/_download.py` & `sigmund-0.17.0/sigmund/tools/_download.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/tools/_execute_code.py` & `sigmund-0.17.0/sigmund/tools/_execute_code.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/tools/_read_attachment.py` & `sigmund-0.17.0/sigmund/tools/_read_attachment.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/tools/_search_documentation.py` & `sigmund-0.17.0/sigmund/tools/_search_documentation.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/tools/_search_google_scholar.py` & `sigmund-0.17.0/sigmund/tools/_search_google_scholar.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/sigmund/utils.py` & `sigmund-0.17.0/sigmund/utils.py`

 * *Files identical despite different names*

### Comparing `sigmund-0.16.7/PKG-INFO` & `sigmund-0.17.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sigmund
-Version: 0.16.7
+Version: 0.17.0
 Summary: AI-based chatbot that provides sensible answers based on documentation
 Keywords: ai,chatbot,llm
 Author-email: Sebastiaan Mathôt <s.mathot@cogsci.nl>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anthropic
 Requires-Dist: cryptography
 Requires-Dist: faiss-cpu
 Requires-Dist: flask
 Requires-Dist: flask-login
 Requires-Dist: flask-sqlalchemy
 Requires-Dist: flask-wtf
+Requires-Dist: flask-cors
 Requires-Dist: jinja2
 Requires-Dist: jq
 Requires-Dist: langchain
 Requires-Dist: langchain_core
 Requires-Dist: langchain_community
 Requires-Dist: langchain_openai
 Requires-Dist: langchain_anthropic
```


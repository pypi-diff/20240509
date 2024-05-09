# Comparing `tmp/gmail_draft_creator-1.2.2.tar.gz` & `tmp/gmail_draft_creator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_draft_creator-1.2.2.tar", max compression
+gzip compressed data, was "gmail_draft_creator-1.3.0.tar", max compression
```

## Comparing `gmail_draft_creator-1.2.2.tar` & `gmail_draft_creator-1.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1071 2024-04-24 18:00:55.034434 gmail_draft_creator-1.2.2/LICENSE
--rw-r--r--   0        0        0     4848 2024-04-24 18:00:55.034434 gmail_draft_creator-1.2.2/gmail_draft_creator/__init__.py
--rw-r--r--   0        0        0     1326 2024-04-24 18:01:23.778924 gmail_draft_creator-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2820 2024-04-24 18:00:55.034434 gmail_draft_creator-1.2.2/readme.md
--rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 gmail_draft_creator-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-09 15:35:39.570277 gmail_draft_creator-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5110 2024-05-09 15:35:39.570277 gmail_draft_creator-1.3.0/gmail_draft_creator/__init__.py
+-rw-r--r--   0        0        0     1326 2024-05-09 15:36:05.334327 gmail_draft_creator-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3082 2024-05-09 15:35:39.570277 gmail_draft_creator-1.3.0/readme.md
+-rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 gmail_draft_creator-1.3.0/PKG-INFO
```

### Comparing `gmail_draft_creator-1.2.2/LICENSE` & `gmail_draft_creator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_draft_creator-1.2.2/gmail_draft_creator/__init__.py` & `gmail_draft_creator-1.3.0/gmail_draft_creator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,15 +69,22 @@
             if email:
                 email = email.strip()
 
             if email is None:
                 print("No email found for row, skipping")
                 continue
 
-            template_params = {k.lower().strip(): v.strip() for k, v in row.items()}
+
+            def normalize_key(key):
+                cleaned_key = key.lower().strip()
+                cleaned_key = re.sub(r'\W+', '', cleaned_key)
+                return cleaned_key
+
+            # each column in the CSV is passed as a parameter to the template
+            template_params = {normalize_key(k): v.strip() for k, v in row.items()}
 
             if email is not None:
                 create_draft(email, template_string, template_params, subject, dry_run)
 
 
 # TODO this should really be much smarter
 def _extract_credentials():
```

### Comparing `gmail_draft_creator-1.2.2/pyproject.toml` & `gmail_draft_creator-1.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmail_draft_creator"
-version = "1.2.2"
+version = "1.3.0"
 description = "Simple tool to take a CSV and a template and create drafts in your Gmail. Can be used as a command line tool, or as a library."
 authors = ["Michael Bianco <mike@mikebian.co>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/iloveitaly/gmail-draft-creator"
 keywords = ["gmail", "email", "gmail-api"]
```

### Comparing `gmail_draft_creator-1.2.2/readme.md` & `gmail_draft_creator-1.3.0/readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Simple tool to take a CSV and a template and create drafts in your Gmail. Useful for sending emails to large-ish numbers
 of people where you want to slightly customize the emails for each user. You can quickly run through drafts, customize it, and send.
 
 ## Installation
 
 ```shell
-pip install gmail-draft-creator
+pip install -U gmail-draft-creator
 ```
 
 ## Usage
 
 ```shell
 Usage: gmail-draft-creator [OPTIONS]
 
@@ -24,14 +24,16 @@
 
 You can also import the `create_draft` function and use it in your own scripts.
 
 ### CSV Files
 
 Must contain an `email` column (case insensitive).
 
+Each column in the CSV is passed as a parameter to the provided template. The column name is stripped of whitespace, lowercased, and stripped all non-alpha characters. For example, a column named `First Name` would be passed as `$firstname` in the template.
+
 ### Template Files
 
 You can include subject line and variables in the template file:
 
 ```text
 Subject: Hello $NAME
```

### Comparing `gmail_draft_creator-1.2.2/PKG-INFO` & `gmail_draft_creator-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmail-draft-creator
-Version: 1.2.2
+Version: 1.3.0
 Summary: Simple tool to take a CSV and a template and create drafts in your Gmail. Can be used as a command line tool, or as a library.
 Home-page: https://github.com/iloveitaly/gmail-draft-creator
 License: MIT
 Keywords: gmail,email,gmail-api
 Author: Michael Bianco
 Author-email: mike@mikebian.co
 Requires-Python: >=3.9,<4.0
@@ -25,15 +25,15 @@
 
 Simple tool to take a CSV and a template and create drafts in your Gmail. Useful for sending emails to large-ish numbers
 of people where you want to slightly customize the emails for each user. You can quickly run through drafts, customize it, and send.
 
 ## Installation
 
 ```shell
-pip install gmail-draft-creator
+pip install -U gmail-draft-creator
 ```
 
 ## Usage
 
 ```shell
 Usage: gmail-draft-creator [OPTIONS]
 
@@ -47,14 +47,16 @@
 
 You can also import the `create_draft` function and use it in your own scripts.
 
 ### CSV Files
 
 Must contain an `email` column (case insensitive).
 
+Each column in the CSV is passed as a parameter to the provided template. The column name is stripped of whitespace, lowercased, and stripped all non-alpha characters. For example, a column named `First Name` would be passed as `$firstname` in the template.
+
 ### Template Files
 
 You can include subject line and variables in the template file:
 
 ```text
 Subject: Hello $NAME
```


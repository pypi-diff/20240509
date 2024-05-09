# Comparing `tmp/resend-0.8.0.tar.gz` & `tmp/resend-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resend-0.8.0.tar", last modified: Wed Mar  6 02:49:05 2024, max compression
+gzip compressed data, was "resend-1.0.0.tar", last modified: Thu May  9 01:40:50 2024, max compression
```

## Comparing `resend-0.8.0.tar` & `resend-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,18 @@
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-03-06 02:49:05.495586 resend-0.8.0/
--rw-r--r--   0 derich     (501) staff       (20)     1070 2023-08-19 17:45:00.000000 resend-0.8.0/LICENSE.md
--rw-r--r--   0 derich     (501) staff       (20)     2208 2024-03-06 02:49:05.495506 resend-0.8.0/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)     1438 2023-08-25 00:15:51.000000 resend-0.8.0/README.md
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-03-06 02:49:05.494361 resend-0.8.0/resend/
--rw-r--r--   0 derich     (501) staff       (20)      604 2024-01-15 21:39:10.000000 resend-0.8.0/resend/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     1069 2024-01-05 01:54:46.000000 resend-0.8.0/resend/api.py
--rw-r--r--   0 derich     (501) staff       (20)      796 2023-08-19 17:45:00.000000 resend-0.8.0/resend/api_keys.py
--rw-r--r--   0 derich     (501) staff       (20)     1017 2024-01-05 01:54:46.000000 resend-0.8.0/resend/audiences.py
--rw-r--r--   0 derich     (501) staff       (20)      396 2024-01-05 01:54:46.000000 resend-0.8.0/resend/batch.py
--rw-r--r--   0 derich     (501) staff       (20)     1579 2024-01-18 01:55:56.000000 resend-0.8.0/resend/contacts.py
--rw-r--r--   0 derich     (501) staff       (20)     1515 2024-03-05 23:14:12.000000 resend-0.8.0/resend/domains.py
--rw-r--r--   0 derich     (501) staff       (20)      588 2023-08-19 17:45:00.000000 resend-0.8.0/resend/emails.py
--rw-r--r--   0 derich     (501) staff       (20)     4766 2024-01-05 01:54:46.000000 resend-0.8.0/resend/exceptions.py
--rw-r--r--   0 derich     (501) staff       (20)     1655 2024-01-05 01:54:46.000000 resend-0.8.0/resend/request.py
--rw-r--r--   0 derich     (501) staff       (20)      163 2024-03-06 02:49:01.000000 resend-0.8.0/resend/version.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-03-06 02:49:05.495269 resend-0.8.0/resend.egg-info/
--rw-r--r--   0 derich     (501) staff       (20)     2208 2024-03-06 02:49:05.000000 resend-0.8.0/resend.egg-info/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)      416 2024-03-06 02:49:05.000000 resend-0.8.0/resend.egg-info/SOURCES.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-03-06 02:49:05.000000 resend-0.8.0/resend.egg-info/dependency_links.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-01-18 02:00:41.000000 resend-0.8.0/resend.egg-info/not-zip-safe
--rw-r--r--   0 derich     (501) staff       (20)       17 2024-03-06 02:49:05.000000 resend-0.8.0/resend.egg-info/requires.txt
--rw-r--r--   0 derich     (501) staff       (20)        7 2024-03-06 02:49:05.000000 resend-0.8.0/resend.egg-info/top_level.txt
--rw-r--r--   0 derich     (501) staff       (20)       67 2024-03-06 02:49:05.495770 resend-0.8.0/setup.cfg
--rw-r--r--   0 derich     (501) staff       (20)     1112 2023-08-19 17:45:00.000000 resend-0.8.0/setup.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 01:40:50.684505 resend-1.0.0/
+-rw-r--r--   0 derich     (501) staff       (20)     1070 2023-08-19 17:45:00.000000 resend-1.0.0/LICENSE.md
+-rw-r--r--   0 derich     (501) staff       (20)     2408 2024-05-09 01:40:50.684424 resend-1.0.0/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)     1605 2024-05-09 01:36:14.000000 resend-1.0.0/README.md
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 01:40:50.683156 resend-1.0.0/resend/
+-rw-r--r--   0 derich     (501) staff       (20)      743 2024-05-09 01:36:14.000000 resend-1.0.0/resend/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     5985 2024-05-09 01:36:14.000000 resend-1.0.0/resend/exceptions.py
+-rw-r--r--   0 derich     (501) staff       (20)     2331 2024-05-09 01:36:14.000000 resend-1.0.0/resend/request.py
+-rw-r--r--   0 derich     (501) staff       (20)      133 2024-05-09 01:36:14.000000 resend-1.0.0/resend/version.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 01:40:50.683851 resend-1.0.0/resend.egg-info/
+-rw-r--r--   0 derich     (501) staff       (20)     2408 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)      293 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/not-zip-safe
+-rw-r--r--   0 derich     (501) staff       (20)       35 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/requires.txt
+-rw-r--r--   0 derich     (501) staff       (20)        7 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/top_level.txt
+-rw-r--r--   0 derich     (501) staff       (20)       67 2024-05-09 01:40:50.684681 resend-1.0.0/setup.cfg
+-rw-r--r--   0 derich     (501) staff       (20)     1112 2023-08-19 17:45:00.000000 resend-1.0.0/setup.py
```

### Comparing `resend-0.8.0/LICENSE.md` & `resend-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resend-0.8.0/PKG-INFO` & `resend-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.8.0
+Version: 1.0.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 Keywords: email,email platform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,23 +15,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests==2.31.0
+Requires-Dist: typing_extensions
 
 # Resend Python SDK
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Build](https://github.com/drish/resend-py/actions/workflows/test.yaml/badge.svg)
 [![codecov](https://codecov.io/gh/drish/resend-py/branch/main/graph/badge.svg?token=GGD39PPFM0)](https://codecov.io/gh/drish/resend-py)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/resend)](https://pypi.org/project/resend/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resend)](https://pypi.org/project/resend)
+
 ---
 
 ## Installation
 
 To install Resend Python SDK, simply execute the following command in a terminal:
 
 ```
@@ -47,22 +49,24 @@
 import os
 
 resend.api_key = "re_yourkey"
 ```
 
 ## Example
 
+You can get an overview about all parameters in the [Send Email](https://resend.com/docs/api-reference/emails/send-email) API reference.
+
 ```py
 import os
 import resend
 
 resend.api_key = "re_yourkey"
 
-params = {
-    "from": "onboarding@resend.dev",
+params: resend.Emails.SendParams = {
+    "sender": "onboarding@resend.dev",
     "to": ["delivered@resend.dev"],
     "subject": "hi",
     "html": "<strong>hello, world!</strong>",
     "reply_to": "to@gmail.com",
     "bcc": "bcc@resend.dev",
     "cc": ["cc@resend.dev"],
     "tags": [
```

### Comparing `resend-0.8.0/README.md` & `resend-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Build](https://github.com/drish/resend-py/actions/workflows/test.yaml/badge.svg)
 [![codecov](https://codecov.io/gh/drish/resend-py/branch/main/graph/badge.svg?token=GGD39PPFM0)](https://codecov.io/gh/drish/resend-py)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/resend)](https://pypi.org/project/resend/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resend)](https://pypi.org/project/resend)
+
 ---
 
 ## Installation
 
 To install Resend Python SDK, simply execute the following command in a terminal:
 
 ```
@@ -25,22 +26,24 @@
 import os
 
 resend.api_key = "re_yourkey"
 ```
 
 ## Example
 
+You can get an overview about all parameters in the [Send Email](https://resend.com/docs/api-reference/emails/send-email) API reference.
+
 ```py
 import os
 import resend
 
 resend.api_key = "re_yourkey"
 
-params = {
-    "from": "onboarding@resend.dev",
+params: resend.Emails.SendParams = {
+    "sender": "onboarding@resend.dev",
     "to": ["delivered@resend.dev"],
     "subject": "hi",
     "html": "<strong>hello, world!</strong>",
     "reply_to": "to@gmail.com",
     "bcc": "bcc@resend.dev",
     "cc": ["cc@resend.dev"],
     "tags": [
```

### Comparing `resend-0.8.0/resend/exceptions.py` & `resend-1.0.0/resend/exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Resend Exceptions module.
 
 This module defines the base types for platform-wide error
 codes as outlined in https://resend.com/docs/errors.
 """
 
-
 from typing import Dict
 
 
 class ResendError(Exception):
     """Base class for all errors raised by Resend SDK.
     This is the parent class of all exceptions (server side)
     raised by the Resend SDK. Developers can simply catch
@@ -25,51 +24,54 @@
     """
 
     def __init__(
         self,
         code: str,
         error_type: str,
         message: str,
-        suggested_action: str = None,
+        suggested_action: str,
     ):
         Exception.__init__(self, message)
         self.code = code
+        self.message = message
         self.suggested_action = suggested_action
         self.error_type = error_type
 
 
 class MissingApiKeyError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
-        message,
-        error_type,
-        code,
+        message: str,
+        error_type: str,
+        code: str,
     ):
         suggested_action = """Include the following header
         Authorization: Bearer YOUR_API_KEY in the request."""
 
+        message = "Missing API key in the authorization header."
+
         ResendError.__init__(
             self,
-            message="Missing API key in the authorization header.",
+            message=message,
             suggested_action=suggested_action,
             code=code,
             error_type=error_type,
         )
 
 
 class InvalidApiKeyError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
-        message,
-        error_type,
-        code,
+        message: str,
+        error_type: str,
+        code: str,
     ):
         suggested_action = """Generate a new API key in the dashboard."""
 
         ResendError.__init__(
             self,
             message=message,
             suggested_action=suggested_action,
@@ -79,102 +81,139 @@
 
 
 class ValidationError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
-        message,
-        error_type,
-        code,
+        message: str,
+        error_type: str,
+        code: str,
     ):
         default_message = """
         The request body is missing one or more required fields."""
 
         suggested_action = """Check the error message
         to see the list of missing fields."""
 
         if message == "":
             message = default_message
 
         ResendError.__init__(
             self,
-            code=code or 400,
+            code=code or "400",
             message=message,
             suggested_action=suggested_action,
             error_type=error_type,
         )
 
 
 class MissingRequiredFieldsError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
-        message,
-        error_type,
-        code,
+        message: str,
+        error_type: str,
+        code: str,
     ):
         default_message = """
         The request body is missing one or more required fields."""
 
         suggested_action = """Check the error message
         to see the list of missing fields."""
 
         if message == "":
             message = default_message
 
         ResendError.__init__(
             self,
-            code=code or 422,
+            code=code or "422",
             message=message,
             suggested_action=suggested_action,
             error_type=error_type,
         )
 
 
 class ApplicationError(ResendError):
     """see https://resend.com/docs/errors"""
 
     def __init__(
         self,
-        message,
-        error_type,
-        code,
+        message: str,
+        error_type: str,
+        code: str,
     ):
         default_message = """
         Something went wrong."""
 
         suggested_action = """Contact Resend support."""
 
         if message == "":
             message = default_message
 
         ResendError.__init__(
             self,
-            code=code or 500,
+            code=code or "500",
             message=message,
             suggested_action=suggested_action,
             error_type=error_type,
         )
 
 
-ERRORS: Dict[str, Dict[str, ResendError]] = {
+# Dict with error code -> error type mapping
+ERRORS: Dict = {
     "400": {"validation_error": ValidationError},
-    "422": {"missing_required_fields": MissingRequiredFieldsError},
+    "422": {
+        "missing_required_fields": MissingRequiredFieldsError,
+        "validation_error": ValidationError,
+    },
     "401": {"missing_api_key": MissingApiKeyError},
     "403": {"invalid_api_key": InvalidApiKeyError},
     "500": {"application_error": ApplicationError},
 }
 
 
-def raise_for_code_and_type(code, error_type, message: str) -> ResendError:
+def raise_for_code_and_type(code: str, error_type: str, message: str) -> None:
+    """Raise the appropriate error based on the code and type.
+
+    Args:
+        code (str): The error code
+        error_type (str): The error type
+        message (str): The error message
+
+    Raises:
+        ResendError: If it is a Resend err
+            or
+        ValidationError: If the error type is validation_error
+            or
+        MissingRequiredFieldsError: If the error type is missing_required_fields
+            or
+        MissingApiKeyError: If the error type is missing_api_key
+            or
+        InvalidApiKeyError: If the error type is invalid_api_key
+            or
+        ApplicationError: If the error type is application_error
+            or
+        TypeError: If the error type is not found
+    """
     error = ERRORS.get(str(code))
 
     # Handle the case where the error might be unknown
-    if error is None or error.get(error_type) is None:
-        raise ResendError(code=code, message=message, error_type=error_type)
+    if error is None:
+        raise ResendError(
+            code=code, message=message, error_type=error_type, suggested_action=""
+        )
 
     # Raise error from errors list
-    error: ResendError = error.get(error_type)
+    error_from_list = error.get(error_type)
 
-    raise error(code=code, message=message, error_type=error_type)
+    if error_from_list is not None:
+        raise error_from_list(
+            code=code,
+            message=message,
+            error_type=error_type,
+        )
+    # defaults to ResendError if finally can't find error type
+    raise ResendError(
+        code=code, message=message, error_type=error_type, suggested_action=""
+    )
```

### Comparing `resend-0.8.0/resend/request.py` & `resend-1.0.0/resend/request.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 class Request:
     def __init__(self, path: str, params: Dict, verb: str):
         self.path = path
         self.params = params
         self.verb = verb
 
     def perform(self):
+        """Is the main function that makes the HTTP request
+        to the Resend API. It uses the path, params, and verb attributes
+        to make the request.
+
+        Returns:
+            Dict: The JSON response from the API
+
+        Raises:
+            requests.HTTPError: If the request fails
+        """
         resp = self.make_request(url=f"{resend.api_url}{self.path}")
 
         # delete calls do not return a body
         if resp.text == "" and resp.status_code == 200:
             return None
 
         # handle error in case there is a statusCode attr present
@@ -41,15 +51,27 @@
         """
         return {
             "Accept": "application/json",
             "Authorization": f"Bearer {resend.api_key}",
             "User-Agent": f"resend-python:{get_version()}",
         }
 
-    def make_request(self, url: str):
+    def make_request(self, url: str) -> requests.Response:
+        """make_request is a helper function that makes the actual
+        HTTP request to the Resend API.
+
+        Args:
+            url (str): The URL to make the request to
+
+        Returns:
+            requests.Response: The response object from the request
+
+        Raises:
+            requests.HTTPError: If the request fails
+        """
         headers = self.__get_headers()
         params = self.params
         verb = self.verb
 
         try:
             return requests.request(verb, url, json=params, headers=headers)
         except requests.HTTPError as e:
```

### Comparing `resend-0.8.0/resend.egg-info/PKG-INFO` & `resend-1.0.0/resend.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 0.8.0
+Version: 1.0.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 Keywords: email,email platform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,23 +15,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests==2.31.0
+Requires-Dist: typing_extensions
 
 # Resend Python SDK
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Build](https://github.com/drish/resend-py/actions/workflows/test.yaml/badge.svg)
 [![codecov](https://codecov.io/gh/drish/resend-py/branch/main/graph/badge.svg?token=GGD39PPFM0)](https://codecov.io/gh/drish/resend-py)
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/resend)](https://pypi.org/project/resend/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resend)](https://pypi.org/project/resend)
+
 ---
 
 ## Installation
 
 To install Resend Python SDK, simply execute the following command in a terminal:
 
 ```
@@ -47,22 +49,24 @@
 import os
 
 resend.api_key = "re_yourkey"
 ```
 
 ## Example
 
+You can get an overview about all parameters in the [Send Email](https://resend.com/docs/api-reference/emails/send-email) API reference.
+
 ```py
 import os
 import resend
 
 resend.api_key = "re_yourkey"
 
-params = {
-    "from": "onboarding@resend.dev",
+params: resend.Emails.SendParams = {
+    "sender": "onboarding@resend.dev",
     "to": ["delivered@resend.dev"],
     "subject": "hi",
     "html": "<strong>hello, world!</strong>",
     "reply_to": "to@gmail.com",
     "bcc": "bcc@resend.dev",
     "cc": ["cc@resend.dev"],
     "tags": [
```

### Comparing `resend-0.8.0/setup.py` & `resend-1.0.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/payload-api-0.4.8.tar.gz` & `tmp/payload-api-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payload-api-0.4.8.tar", last modified: Wed Apr 10 03:18:33 2024, max compression
+gzip compressed data, was "payload-api-0.4.9.tar", last modified: Wed Apr 10 03:30:36 2024, max compression
```

## Comparing `payload-api-0.4.8.tar` & `payload-api-0.4.9.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1089 2024-04-10 03:18:24.723776 payload-api-0.4.8/LICENSE
--rw-r--r--   0        0        0      673 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/__init__.py
--rw-r--r--   0        0        0      122 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/__init__.py
--rw-r--r--   0        0        0     2104 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/attr.py
--rw-r--r--   0        0        0     3930 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/object.py
--rw-r--r--   0        0        0     7240 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/request.py
--rw-r--r--   0        0        0      989 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/arm/session.py
--rw-r--r--   0        0        0     1282 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/exceptions.py
--rw-r--r--   0        0        0     2356 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/objects.py
--rw-r--r--   0        0        0     2782 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/utils.py
--rw-r--r--   0        0        0      495 2024-04-10 03:18:24.723776 payload-api-0.4.8/payload/version.py
--rw-r--r--   0        0        0      767 2024-04-10 03:18:24.727776 payload-api-0.4.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/__init__.py
--rw-r--r--   0        0        0     4866 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/fixtures.py
--rw-r--r--   0        0        0      430 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_access_token.py
--rw-r--r--   0        0        0     3252 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_account.py
--rw-r--r--   0        0        0     1419 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_billing.py
--rw-r--r--   0        0        0     1660 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_invoice.py
--rw-r--r--   0        0        0     1416 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_payment_link.py
--rw-r--r--   0        0        0     3655 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_payment_method.py
--rw-r--r--   0        0        0    27269 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_request.py
--rw-r--r--   0        0        0     3515 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_session.py
--rw-r--r--   0        0        0     1473 2024-04-10 03:18:24.727776 payload-api-0.4.8/tests/test_transaction.py
--rw-r--r--   0        0        0      166 1970-01-01 00:00:00.000000 payload-api-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-10 03:30:22.867094 payload-api-0.4.9/LICENSE
+-rw-r--r--   0        0        0     2458 2024-04-10 03:30:22.867094 payload-api-0.4.9/README.md
+-rw-r--r--   0        0        0      673 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/arm/__init__.py
+-rw-r--r--   0        0        0     2104 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/arm/attr.py
+-rw-r--r--   0        0        0     3930 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/arm/object.py
+-rw-r--r--   0        0        0     7240 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/arm/request.py
+-rw-r--r--   0        0        0      989 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/arm/session.py
+-rw-r--r--   0        0        0     1282 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/exceptions.py
+-rw-r--r--   0        0        0     2356 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/objects.py
+-rw-r--r--   0        0        0     2782 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/utils.py
+-rw-r--r--   0        0        0      495 2024-04-10 03:30:22.867094 payload-api-0.4.9/payload/version.py
+-rw-r--r--   0        0        0      937 2024-04-10 03:30:22.867094 payload-api-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/__init__.py
+-rw-r--r--   0        0        0     4866 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/fixtures.py
+-rw-r--r--   0        0        0      430 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/test_access_token.py
+-rw-r--r--   0        0        0     3252 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/test_account.py
+-rw-r--r--   0        0        0     1419 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/test_billing.py
+-rw-r--r--   0        0        0     1660 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/test_invoice.py
+-rw-r--r--   0        0        0     1416 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/test_payment_link.py
+-rw-r--r--   0        0        0     3655 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/test_payment_method.py
+-rw-r--r--   0        0        0    27269 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/test_request.py
+-rw-r--r--   0        0        0     3515 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/test_session.py
+-rw-r--r--   0        0        0     1473 2024-04-10 03:30:22.867094 payload-api-0.4.9/tests/test_transaction.py
+-rw-r--r--   0        0        0     2829 1970-01-01 00:00:00.000000 payload-api-0.4.9/PKG-INFO
```

### Comparing `payload-api-0.4.8/LICENSE` & `payload-api-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/payload/__init__.py` & `payload-api-0.4.9/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/payload/arm/attr.py` & `payload-api-0.4.9/payload/arm/attr.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/payload/arm/object.py` & `payload-api-0.4.9/payload/arm/object.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/payload/arm/request.py` & `payload-api-0.4.9/payload/arm/request.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/payload/arm/session.py` & `payload-api-0.4.9/payload/arm/session.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/payload/exceptions.py` & `payload-api-0.4.9/payload/exceptions.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/payload/objects.py` & `payload-api-0.4.9/payload/objects.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/payload/utils.py` & `payload-api-0.4.9/payload/utils.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/pyproject.toml` & `payload-api-0.4.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 [project]
 name = "payload-api"
-version = "0.4.8"
+version = "0.4.9"
 description = "Payload Python Library"
 authors = [
-    { name = "Ian Halpern", email = "ian@payload.co" },
+    { name = "Payload", email = "help@payload.co" },
 ]
 dependencies = [
     "requests",
     "six",
     "urllib3>=1.26.5",
 ]
 requires-python = ">=3.7"
+readme = "README.md"
 
 [project.license]
 text = "MIT"
 
+[project.urls]
+Homepage = "https://payload.co"
+Documentation = "https://docs.payload.co"
+Repository = "https://github.com/payload-code/payload-python"
+
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
 ]
 build-backend = "pdm.pep517.api"
 
 [tool.pdm]
```

### Comparing `payload-api-0.4.8/tests/fixtures.py` & `payload-api-0.4.9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/tests/test_account.py` & `payload-api-0.4.9/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/tests/test_billing.py` & `payload-api-0.4.9/tests/test_billing.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/tests/test_invoice.py` & `payload-api-0.4.9/tests/test_invoice.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/tests/test_payment_link.py` & `payload-api-0.4.9/tests/test_payment_link.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/tests/test_payment_method.py` & `payload-api-0.4.9/tests/test_payment_method.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/tests/test_request.py` & `payload-api-0.4.9/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/tests/test_session.py` & `payload-api-0.4.9/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `payload-api-0.4.8/tests/test_transaction.py` & `payload-api-0.4.9/tests/test_transaction.py`

 * *Files identical despite different names*


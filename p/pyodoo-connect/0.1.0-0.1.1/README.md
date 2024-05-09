# Comparing `tmp/pyodoo_connect-0.1.0.tar.gz` & `tmp/pyodoo_connect-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodoo_connect-0.1.0.tar", last modified: Wed May  8 12:53:47 2024, max compression
+gzip compressed data, was "pyodoo_connect-0.1.1.tar", last modified: Thu May  9 08:52:42 2024, max compression
```

## Comparing `pyodoo_connect-0.1.0.tar` & `pyodoo_connect-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:53:47.892889 pyodoo_connect-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-08 12:53:47.892889 pyodoo_connect-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:53:47.888888 pyodoo_connect-0.1.0/pyodoo_connect/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/pyodoo_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/pyodoo_connect/odoo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/pyodoo_connect/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/pyodoo_connect/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:53:47.892889 pyodoo_connect-0.1.0/pyodoo_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-08 12:53:47.000000 pyodoo_connect-0.1.0/pyodoo_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-08 12:53:47.000000 pyodoo_connect-0.1.0/pyodoo_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 12:53:47.000000 pyodoo_connect-0.1.0/pyodoo_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 12:53:47.000000 pyodoo_connect-0.1.0/pyodoo_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 12:53:47.892889 pyodoo_connect-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 12:53:47.892889 pyodoo_connect-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-08 12:53:35.000000 pyodoo_connect-0.1.0/tests/test_odoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:42.506308 pyodoo_connect-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-09 08:52:42.506308 pyodoo_connect-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:42.502308 pyodoo_connect-0.1.1/pyodoo_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/pyodoo_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/pyodoo_connect/odoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/pyodoo_connect/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/pyodoo_connect/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:42.502308 pyodoo_connect-0.1.1/pyodoo_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-09 08:52:42.000000 pyodoo_connect-0.1.1/pyodoo_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-09 08:52:42.000000 pyodoo_connect-0.1.1/pyodoo_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:52:42.000000 pyodoo_connect-0.1.1/pyodoo_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-09 08:52:42.000000 pyodoo_connect-0.1.1/pyodoo_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 08:52:42.506308 pyodoo_connect-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:42.502308 pyodoo_connect-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-09 08:52:28.000000 pyodoo_connect-0.1.1/tests/test_odoo.py
```

### Comparing `pyodoo_connect-0.1.0/LICENSE` & `pyodoo_connect-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodoo_connect-0.1.0/PKG-INFO` & `pyodoo_connect-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodoo_connect
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to interact with Odoo via JSON-RPC.
 Home-page: https://github.com/fasilwdr/pyodoo_connector
 Author: Fasil
 Author-email: Fasil <fasilwdr@hotmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Fasil]
@@ -37,17 +37,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# Odoo Connector
+# PyOdoo Connector
 
-Odoo Connector is a Python package providing a convenient way to interact with Odoo platforms via JSON-RPC. It simplifies operations like logging in, executing commands, and managing records in an Odoo database.
+PyOdoo Connector is a Python package providing a convenient way to interact with Odoo platforms via JSON-RPC. It simplifies operations like logging in, executing commands, and managing records in an Odoo database.
 
 ## Features
 
 - **Session Management**: Handles login and session management automatically.
 - **CRUD Operations**: Easy-to-use functions for creating, reading, updating, and deleting records.
 - **Method Execution**: Supports calling custom methods defined in Odoo models.
 - **Error Handling**: Implements error handling for HTTP and URL request errors.
@@ -91,40 +91,39 @@
 partner = odoo.env['res.partner'].browse(9)
 partner.name = 'New Partner Name'
 ```
 
 - Execute a Method on a Record
 ```python
 partner.action_archive()
-partner.update(values={'mobile': '12345678'})
+partner.update({'mobile': '12345678'})
 ```
 - Search for Records
 ```python
-search_check = odoo.env['res.partner'].search(domain=[('name', '=', 'Abigail Peterson')])
-print("search_check", search_check)
+partner_ids = odoo.env['res.partner'].search(domain=[('name', '=', 'Abigail Peterson')])
+print(partner_ids)
 ```
 - Read Records
 ```python
-read_check = odoo.env['res.partner'].read(ids=search_check, fields=['name', 'email'])
-print("read_check", read_check)
+print(partner.name)
+records = odoo.env['res.partner'].read(ids=search_check, fields=['name', 'email'])
+print(records)
 ```
 - Create a New Record
 ```python
-create_check = odoo.env['res.partner'].create({'name': 'New Partner', 'email': 'new@partner.com', 'is_company': True})
-print("create_check", create_check)
+new_partner_id = odoo.env['res.partner'].create({'name': 'New Partner', 'email': 'new@partner.com', 'is_company': True})
+print(new_partner_id)
 ```
 - Update Records
 ```python
-write_check = odoo.env['res.partner'].write(ids=[create_check], values={'phone': '1234567890'})
-print("write_check", write_check)
+odoo.env['res.partner'].write(ids=new_partner_id, values={'phone': '1234567890'})
 ```
 - Delete Records
 ```python
-unlink_check = odoo.env['res.partner'].unlink(ids=[create_check])
-print("unlink_check", unlink_check)
+odoo.env['res.partner'].unlink(ids=new_partner_id)
 ```
 - Download a QWeb Report
 ```python
 odoo.download_report(report_name='sale.report_saleorder', record_ids=[52], file_name='Sales Report')
 ```
 
 ## Contributing
```

### Comparing `pyodoo_connect-0.1.0/README.md` & `pyodoo_connect-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-# Odoo Connector
+# PyOdoo Connector
 
-Odoo Connector is a Python package providing a convenient way to interact with Odoo platforms via JSON-RPC. It simplifies operations like logging in, executing commands, and managing records in an Odoo database.
+PyOdoo Connector is a Python package providing a convenient way to interact with Odoo platforms via JSON-RPC. It simplifies operations like logging in, executing commands, and managing records in an Odoo database.
 
 ## Features
 
 - **Session Management**: Handles login and session management automatically.
 - **CRUD Operations**: Easy-to-use functions for creating, reading, updating, and deleting records.
 - **Method Execution**: Supports calling custom methods defined in Odoo models.
 - **Error Handling**: Implements error handling for HTTP and URL request errors.
@@ -49,40 +49,39 @@
 partner = odoo.env['res.partner'].browse(9)
 partner.name = 'New Partner Name'
 ```
 
 - Execute a Method on a Record
 ```python
 partner.action_archive()
-partner.update(values={'mobile': '12345678'})
+partner.update({'mobile': '12345678'})
 ```
 - Search for Records
 ```python
-search_check = odoo.env['res.partner'].search(domain=[('name', '=', 'Abigail Peterson')])
-print("search_check", search_check)
+partner_ids = odoo.env['res.partner'].search(domain=[('name', '=', 'Abigail Peterson')])
+print(partner_ids)
 ```
 - Read Records
 ```python
-read_check = odoo.env['res.partner'].read(ids=search_check, fields=['name', 'email'])
-print("read_check", read_check)
+print(partner.name)
+records = odoo.env['res.partner'].read(ids=search_check, fields=['name', 'email'])
+print(records)
 ```
 - Create a New Record
 ```python
-create_check = odoo.env['res.partner'].create({'name': 'New Partner', 'email': 'new@partner.com', 'is_company': True})
-print("create_check", create_check)
+new_partner_id = odoo.env['res.partner'].create({'name': 'New Partner', 'email': 'new@partner.com', 'is_company': True})
+print(new_partner_id)
 ```
 - Update Records
 ```python
-write_check = odoo.env['res.partner'].write(ids=[create_check], values={'phone': '1234567890'})
-print("write_check", write_check)
+odoo.env['res.partner'].write(ids=new_partner_id, values={'phone': '1234567890'})
 ```
 - Delete Records
 ```python
-unlink_check = odoo.env['res.partner'].unlink(ids=[create_check])
-print("unlink_check", unlink_check)
+odoo.env['res.partner'].unlink(ids=new_partner_id)
 ```
 - Download a QWeb Report
 ```python
 odoo.download_report(report_name='sale.report_saleorder', record_ids=[52], file_name='Sales Report')
 ```
 
 ## Contributing
```

### Comparing `pyodoo_connect-0.1.0/pyodoo_connect/odoo.py` & `pyodoo_connect-0.1.1/pyodoo_connect/odoo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# -*- coding: utf-8 -*-
+#############################################################################
+# Author: Fasil
+# Email: fasilwdr@hotmail.com
+# WhatsApp: https://wa.me/966538952934
+# Facebook: https://www.facebook.com/fasilwdr
+# Instagram: https://www.instagram.com/fasilwdr
+#############################################################################
+
 import json
 import random
 import logging
 import urllib.request
 from urllib.error import URLError, HTTPError
 from .proxies import ModelProxy
```

### Comparing `pyodoo_connect-0.1.0/pyodoo_connect/tools.py` & `pyodoo_connect-0.1.1/pyodoo_connect/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# -*- coding: utf-8 -*-
+#############################################################################
+# Author: Fasil
+# Email: fasilwdr@hotmail.com
+# WhatsApp: https://wa.me/966538952934
+# Facebook: https://www.facebook.com/fasilwdr
+# Instagram: https://www.instagram.com/fasilwdr
+#############################################################################
+
 
 CREATE = 0
 UPDATE = 1
 DELETE = 2
 UNLINK = 3
 LINK = 4
 CLEAR = 5
```

### Comparing `pyodoo_connect-0.1.0/pyodoo_connect.egg-info/PKG-INFO` & `pyodoo_connect-0.1.1/pyodoo_connect.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodoo_connect
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package to interact with Odoo via JSON-RPC.
 Home-page: https://github.com/fasilwdr/pyodoo_connector
 Author: Fasil
 Author-email: Fasil <fasilwdr@hotmail.com>
 License: MIT License
         
         Copyright (c) [2024] [Fasil]
@@ -37,17 +37,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
-# Odoo Connector
+# PyOdoo Connector
 
-Odoo Connector is a Python package providing a convenient way to interact with Odoo platforms via JSON-RPC. It simplifies operations like logging in, executing commands, and managing records in an Odoo database.
+PyOdoo Connector is a Python package providing a convenient way to interact with Odoo platforms via JSON-RPC. It simplifies operations like logging in, executing commands, and managing records in an Odoo database.
 
 ## Features
 
 - **Session Management**: Handles login and session management automatically.
 - **CRUD Operations**: Easy-to-use functions for creating, reading, updating, and deleting records.
 - **Method Execution**: Supports calling custom methods defined in Odoo models.
 - **Error Handling**: Implements error handling for HTTP and URL request errors.
@@ -91,40 +91,39 @@
 partner = odoo.env['res.partner'].browse(9)
 partner.name = 'New Partner Name'
 ```
 
 - Execute a Method on a Record
 ```python
 partner.action_archive()
-partner.update(values={'mobile': '12345678'})
+partner.update({'mobile': '12345678'})
 ```
 - Search for Records
 ```python
-search_check = odoo.env['res.partner'].search(domain=[('name', '=', 'Abigail Peterson')])
-print("search_check", search_check)
+partner_ids = odoo.env['res.partner'].search(domain=[('name', '=', 'Abigail Peterson')])
+print(partner_ids)
 ```
 - Read Records
 ```python
-read_check = odoo.env['res.partner'].read(ids=search_check, fields=['name', 'email'])
-print("read_check", read_check)
+print(partner.name)
+records = odoo.env['res.partner'].read(ids=search_check, fields=['name', 'email'])
+print(records)
 ```
 - Create a New Record
 ```python
-create_check = odoo.env['res.partner'].create({'name': 'New Partner', 'email': 'new@partner.com', 'is_company': True})
-print("create_check", create_check)
+new_partner_id = odoo.env['res.partner'].create({'name': 'New Partner', 'email': 'new@partner.com', 'is_company': True})
+print(new_partner_id)
 ```
 - Update Records
 ```python
-write_check = odoo.env['res.partner'].write(ids=[create_check], values={'phone': '1234567890'})
-print("write_check", write_check)
+odoo.env['res.partner'].write(ids=new_partner_id, values={'phone': '1234567890'})
 ```
 - Delete Records
 ```python
-unlink_check = odoo.env['res.partner'].unlink(ids=[create_check])
-print("unlink_check", unlink_check)
+odoo.env['res.partner'].unlink(ids=new_partner_id)
 ```
 - Download a QWeb Report
 ```python
 odoo.download_report(report_name='sale.report_saleorder', record_ids=[52], file_name='Sales Report')
 ```
 
 ## Contributing
```

### Comparing `pyodoo_connect-0.1.0/pyproject.toml` & `pyodoo_connect-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyodoo_connect"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python package to interact with Odoo via JSON-RPC."
 authors = [{ name = "Fasil", email = "fasilwdr@hotmail.com" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `pyodoo_connect-0.1.0/setup.cfg` & `pyodoo_connect-0.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyodoo_connect
-version = 0.1.0
+version = 0.1.1
 author = Fasil
 author_email = fasilwdr@hotmail.com
 description = A Python package to interact with Odoo via JSON-RPC.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fasilwdr/pyodoo_connector
 classifiers =
```

### Comparing `pyodoo_connect-0.1.0/tests/test_odoo.py` & `pyodoo_connect-0.1.1/tests/test_odoo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# -*- coding: utf-8 -*-
+#############################################################################
+# Author: Fasil
+# Email: fasilwdr@hotmail.com
+# WhatsApp: https://wa.me/966538952934
+# Facebook: https://www.facebook.com/fasilwdr
+# Instagram: https://www.instagram.com/fasilwdr
+#############################################################################
 import json
 import pytest
 from unittest.mock import patch, MagicMock
 from pyodoo_connect.odoo import Odoo
 
 
 class TestOdoo:
```


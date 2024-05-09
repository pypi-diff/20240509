# Comparing `tmp/contact_phone_local-0.0.13.tar.gz` & `tmp/contact_phone_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_phone_local-0.0.13.tar", last modified: Thu May  9 05:50:54 2024, max compression
+gzip compressed data, was "contact_phone_local-0.0.9.tar", last modified: Tue May  7 15:33:35 2024, max compression
```

## Comparing `contact_phone_local-0.0.13.tar` & `contact_phone_local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:50:54.827654 contact_phone_local-0.0.13/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-09 05:50:54.827654 contact_phone_local-0.0.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 05:50:33.000000 contact_phone_local-0.0.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:50:54.823654 contact_phone_local-0.0.13/contact_phone_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:50:54.827654 contact_phone_local-0.0.13/contact_phone_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:50:33.000000 contact_phone_local-0.0.13/contact_phone_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-09 05:50:33.000000 contact_phone_local-0.0.13/contact_phone_local/src/contact_phone_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-09 05:50:33.000000 contact_phone_local-0.0.13/contact_phone_local/src/contact_phone_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:50:54.827654 contact_phone_local-0.0.13/contact_phone_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-09 05:50:54.000000 contact_phone_local-0.0.13/contact_phone_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 05:50:54.000000 contact_phone_local-0.0.13/contact_phone_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:50:54.000000 contact_phone_local-0.0.13/contact_phone_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 05:50:54.000000 contact_phone_local-0.0.13/contact_phone_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-09 05:50:54.000000 contact_phone_local-0.0.13/contact_phone_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-09 05:50:33.000000 contact_phone_local-0.0.13/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:50:54.827654 contact_phone_local-0.0.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-09 05:50:33.000000 contact_phone_local-0.0.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/contact_phone_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/contact_phone_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/contact_phone_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/contact_phone_local/src/contact_phones_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/contact_phone_local/src/contact_phones_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/contact_phone_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 15:33:35.000000 contact_phone_local-0.0.9/contact_phone_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:33:35.277199 contact_phone_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-07 15:33:14.000000 contact_phone_local-0.0.9/setup.py
```

### Comparing `contact_phone_local-0.0.13/PKG-INFO` & `contact_phone_local-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: contact-phone-local
-Version: 0.0.13
-Summary: PyPI Package for Circles contact-phone-local Python
+Version: 0.0.9
+Summary: PyPI Package for Circles contact-phones-local Python
 Home-page: https://github.com/circles-zone/contact-phone-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
 Requires-Dist: user-context-remote>=0.0.17
 Requires-Dist: python-sdk-remote>=0.0.27
 
-PyPI Package for Circles contact-phone-local Python
+PyPI Package for Circles contact-phones-local Python
```

### Comparing `contact_phone_local-0.0.13/contact_phone_local/src/contact_phone_local.py` & `contact_phone_local-0.0.9/contact_phone_local/src/contact_phones_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from .contact_phone_local_constants import CONTACT_PHONE_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
+from .contact_phones_local_constants import CONTACT_PHONES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT
 from logger_local.Logger import Logger
 from database_mysql_local.generic_mapping import GenericMapping
 from phone_local.phones_local import PhonesLocal
 from phonenumbers import (NumberParseException, PhoneNumberFormat,
                           format_number, parse)
 
 DEFAULT_SCHEMA_NAME = 'contact_phone'
 DEFAULT_ENTITY_NAME1 = 'contact'
 DEFAULT_ENTITY_NAME2 = 'phone'
 DEFAULT_ID_COLUMN_NAME = 'contact_phone_id'
 DEFAULT_TABLE_NAME = 'contact_phone_table'
 DEFAULT_VIEW_TABLE_NAME = 'contact_phone_view'
 
 
-class ContactPhoneLocal(GenericMapping):
+class ContactPhonesLocal(GenericMapping):
     def __init__(self, default_schema_name: str = DEFAULT_SCHEMA_NAME, default_entity_name1: str = DEFAULT_ENTITY_NAME1,
                  default_entity_name2: str = DEFAULT_ENTITY_NAME2, default_id_column_name: str = DEFAULT_ID_COLUMN_NAME,
                  default_table_name: str = DEFAULT_TABLE_NAME, default_view_table_name: str = DEFAULT_VIEW_TABLE_NAME,
                  is_test_data: bool = False):
 
         super().__init__(default_schema_name=default_schema_name, default_entity_name1=default_entity_name1,
                          default_entity_name2=default_entity_name2, default_id_column_name=default_id_column_name,
                          default_table_name=default_table_name, default_view_table_name=default_view_table_name,
                          is_test_data=is_test_data)
         self.phones_local = PhonesLocal()
-        self.logger = Logger.create_logger(object=CONTACT_PHONE_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
+        self.logger = Logger.create_logger(object=CONTACT_PHONES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 
     # UPSERT
     # TODO Why do we have region as a parameter? - Should be able to extract it from the phone or contact_id
     # TODO Expected phone_number is original_phone_number of processed_phone_number?
     def insert_contact_and_link_to_existing_or_new_phone(self, contact_dict: dict, phone_number: str,
                                                          contact_id: int, region: str = None) -> int:
         """
@@ -39,18 +39,18 @@
         :param region: region (For example, 'US' stands for the United States, 'GB' for the United Kingdom)
         :return: contact_phone_id
         """
         self.logger.start(object={"contact_dict": contact_dict, "phone_number": phone_number,
                                   "contact_id": contact_id, "region": region})
 
         # phone = new PhoneLocal( phone_number );
-
+                                                           
         proccessed_phone_number = self.process_phone_number(original_number=phone_number, region=region)
 
-        # Add the people(person/contact/profile/user) to the Country Group based on their phone internationa_dialing_code
+        # Add the people(person/contact/profile/user) to the Country Group based on their phone internationa_dialing_code                                                   
         # TODO call process_people_phone_number( entity_name='Contact', phone) from phone-local-python-package
 
         # I would recommend moving this code to the PhoneLocal class and calling it in the Phone constructor
         # TODO Can we replace this by UPSERT?
         phone_id_tuple = self.phones_local.select_one_tuple_by_where(
             select_clause_value="phone_id",
             where="full_number_normalized = %s",
@@ -100,11 +100,12 @@
             number_info = {
                 "number_original": original_number,
                 "international_code": international_code,
                 "full_number_normalized": full_number_normalized,
                 "local_number_normalized": local_number_normalized,
             }
             return number_info
-        except NumberParseException as exception:
+        #TODO e -> exception
+        except NumberParseException as e:
             self.logger.error(
                 # TODO Add a second parameter with exception and all parameters of the method
-                f"Invalid phone number: {original_number}. Exception: {str(exception)}")
+                f"Invalid phone number: {original_number}. Exception: {str(e)}")
```

### Comparing `contact_phone_local-0.0.13/contact_phone_local/src/contact_phone_local_constants.py` & `contact_phone_local-0.0.9/contact_phone_local/src/contact_phones_local_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 
-CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_ID = 278
-CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_NAME = "contact-phone-local-python-package"
+CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_ID = 278
+CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_NAME = "contact-phones-local-python-package"
 DEVELOPER_EMAIL = "tal.g@circ.zone"
-CONTACT_PHONE_PYTHON_PACKAGE_CODE_LOGGER_OBJECT = {
-    'component_id': CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_ID,
-    'component_name': CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_NAME,
+CONTACT_PHONES_PYTHON_PACKAGE_CODE_LOGGER_OBJECT = {
+    'component_id': CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_ID,
+    'component_name': CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': DEVELOPER_EMAIL
 }
 
-CONTACT_PHONE_PYTHON_PACKAGE_TEST_LOGGER_OBJECT = {
-    'component_id': CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_ID,
-    'component_name': CONTACT_PHONE_LOCAL_PYTHON_COMPONENT_NAME,
+CONTACT_PHONES_PYTHON_PACKAGE_TEST_LOGGER_OBJECT = {
+    'component_id': CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_ID,
+    'component_name': CONTACT_PHONES_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Unit_Test.value,
     'testing_framework': LoggerComponentEnum.testingFramework.pytest.value,
     'developer_email': DEVELOPER_EMAIL
 }
```

### Comparing `contact_phone_local-0.0.13/contact_phone_local.egg-info/PKG-INFO` & `contact_phone_local-0.0.9/contact_phone_local.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: contact-phone-local
-Version: 0.0.13
-Summary: PyPI Package for Circles contact-phone-local Python
+Version: 0.0.9
+Summary: PyPI Package for Circles contact-phones-local Python
 Home-page: https://github.com/circles-zone/contact-phone-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: PyMySQL>=1.0.2
 Requires-Dist: pytest>=7.4.0
 Requires-Dist: mysql-connector>=2.2.9
 Requires-Dist: logzio-python-handler>=4.1.0
 Requires-Dist: user-context-remote>=0.0.17
 Requires-Dist: python-sdk-remote>=0.0.27
 
-PyPI Package for Circles contact-phone-local Python
+PyPI Package for Circles contact-phones-local Python
```

### Comparing `contact_phone_local-0.0.13/setup.py` & `contact_phone_local-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 PACKAGE_NAME = "contact-phone-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.13',  # update only the minor version each time # https://pypi.org/project/contact-phone-local/
+    version='0.0.9',  # update only the minor version each time # https://pypi.org/project/contact-phones-local/
     author="Circles",
     author_email="info@circlez.ai",
-    description="PyPI Package for Circles contact-phone-local Python",
-    long_description="PyPI Package for Circles contact-phone-local Python",
+    description="PyPI Package for Circles contact-phones-local Python",
+    long_description="PyPI Package for Circles contact-phones-local Python",
     long_description_content_type='text/markdown',
-    url="https://github.com/circles-zone/contact-phone-local-python-package",  # https://pypi.org/project/contact-phone-local/
+    url="https://github.com/circles-zone/contact-phone-local-python-package",  # https://pypi.org/project/contact-phones-local/
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
```


# Comparing `tmp/phones-local-0.0.18.tar.gz` & `tmp/phones_local-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones-local-0.0.18.tar", last modified: Sat Jan 20 20:40:45 2024, max compression
+gzip compressed data, was "phones_local-0.0.19.tar", last modified: Thu May  9 07:25:56 2024, max compression
```

## Comparing `phones-local-0.0.18.tar` & `phones_local-0.0.19.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:40:45.252663 phones-local-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-20 20:40:45.252663 phones-local-0.0.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-01-20 20:40:08.000000 phones-local-0.0.18/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:40:45.248662 phones-local-0.0.18/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:40:45.252663 phones-local-0.0.18/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-20 20:40:08.000000 phones-local-0.0.18/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-01-20 20:40:08.000000 phones-local-0.0.18/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-01-20 20:40:08.000000 phones-local-0.0.18/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 20:40:45.252663 phones-local-0.0.18/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-01-20 20:40:45.000000 phones-local-0.0.18/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-20 20:40:45.000000 phones-local-0.0.18/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 20:40:45.000000 phones-local-0.0.18/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-20 20:40:45.000000 phones-local-0.0.18/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-20 20:40:45.000000 phones-local-0.0.18/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-20 20:40:08.000000 phones-local-0.0.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 20:40:45.252663 phones-local-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-20 20:40:08.000000 phones-local-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:56.277891 phones_local-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-09 07:25:56.277891 phones_local-0.0.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-09 07:25:28.000000 phones_local-0.0.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:56.273891 phones_local-0.0.19/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:56.277891 phones_local-0.0.19/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:28.000000 phones_local-0.0.19/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-09 07:25:28.000000 phones_local-0.0.19/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8971 2024-05-09 07:25:28.000000 phones_local-0.0.19/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:25:56.277891 phones_local-0.0.19/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 07:25:56.000000 phones_local-0.0.19/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-09 07:25:28.000000 phones_local-0.0.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:25:56.277891 phones_local-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-09 07:25:28.000000 phones_local-0.0.19/setup.py
```

### Comparing `phones-local-0.0.18/README.md` & `phones_local-0.0.19/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 # python-package-template
+
 To create local package and remote package layers (not to create GraphQL and REST-API layers)
 
 # directory structure
-Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e. location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br> 
+
+Root directory should have only .github/, ,gitignore, README.md and the project directory (i.e.
+location_local_python_package same as repo) - This will allow is to easily switch to mono repo<br>
 /location_local<br>
 /location_local/get_country_name<br>
 /location_local/get_country_name/src<br>
 /location_local/get_country_name/src/get_country_name.py<br>
 /location_local/get_country_name/tests<br>
 /location_local/get_country_name/tests/test_get_country_name.py<br>
 
 # database Python scripts in /db folder
+
 Please place <table-name>.py in /db<br>
 No need for seperate file for _ml table<br>
 Please delete the example file if not needed<br>
-  
+
 # Create the files to create the database schema, tables, view and populate Meta Data and Test Date
+
 /db/<table-name>.py - CREATE SCHEMA ... CREATE TABLE ... CREATE VIEW ...<br>
 /db/<table-name>_insert.py to create records
 
 # Update the setup.py (i.e.name, version)
- 
+
 # Please create test directory inside the directory of the project i.e. /<project-name>/tests
 
 # Update the serverless.yml in the root directory
+
 provider:
-  stage: play1
-  
+stage: play1
+
 Update the endpoints in serverless.yml
 
 # Working with VS Code
+
 Please make sure you push to the repo launch.json fie that enables to run and debug the code<br>
 
 # Unit-Test
+
 We prefer using pytest and not unittest package<br>
 
 Please create pytest.init in the project directory and not in the root directory
+
 ```
 [pytest]
 markers =
     test: custom mark for tests
 ```
```

### Comparing `phones-local-0.0.18/phones_local/src/phone_local_constans.py` & `phones_local-0.0.19/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones-local-0.0.18/phones_local/src/phones_local.py` & `phones_local-0.0.19/phones_local/src/phones_local.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from circles_local_database_python.generic_mapping import GenericMapping
-from logger_local.Logger import Logger
+from database_mysql_local.generic_mapping import GenericMapping
+from logger_local.LoggerLocal import Logger
 from phonenumbers import (NumberParseException, PhoneNumberFormat,
                           format_number, parse)
 
 from .phone_local_constans import code_object_init
 
 logger = Logger.create_logger(object=code_object_init)
 
@@ -62,72 +62,125 @@
             "international_code": 972,
             "full_number_normalized": "+972549338666"
         }
         """
         try:
             parsed_number = parse(original_number, region)
             international_code = parsed_number.country_code
-            full_number_normalized = format_number(
-                parsed_number, PhoneNumberFormat.E164)
+            full_number_normalized = format_number(parsed_number, PhoneNumberFormat.E164)
             number_info = {
                 "international_code": international_code,
-                "full_number_normalized": full_number_normalized
+                "full_number_normalized": full_number_normalized,
+                "extension": parsed_number.extension,
             }
             return number_info
         except NumberParseException as e:
-            logger.error(
-                f"Invalid phone number: {original_number}. Exception: {str(e)}")
+            logger.error(f"Invalid phone number: {original_number}.", object=e)
+            raise e
 
-    def process_phone(self, original_phone_number: str, contact_id: int = None) -> dict:
+    def get_country_iso_code(self, details: dict) -> str:
+        contact_id = details.get('contact_id')
+        profile_id = details.get('profile_id')
+        location_id = details.get('location_id')
+        country_id = details.get('country_id')
+
+        if not country_id:  # get country_id from location_id
+            if not location_id:  # get location_id from contact_id or profile_id
+                if contact_id and not profile_id:  # get profile_id from contact_id
+                    profile_id = self.select_one_value_by_id(
+                        schema_name="contact_profile",
+                        view_table_name='contact_profile_view', select_clause_value='profile_id',
+                        id_column_name='contact_id', id_column_value=contact_id)
+                    details['profile_id'] = profile_id
+                assert profile_id, "profile_id is required for getting location_id"
+                location_id = self.select_one_value_by_id(
+                    schema_name="location_profile",
+                    view_table_name='location_profile_view', select_clause_value='location_id',
+                    id_column_name='profile_id', id_column_value=profile_id)
+
+            assert location_id, "location_id is required for getting country_id"
+            country_id = self.select_one_value_by_id(
+                schema_name="location", view_table_name='location_view', select_clause_value='country_id',
+                id_column_name='location_id', id_column_value=location_id)
+
+        country_iso_code = self.select_one_value_by_id(
+            schema_name="country", view_table_name='country_ml_view', select_clause_value='iso',
+            id_column_name='country_id', id_column_value=country_id)
+        return country_iso_code
+
+    # TODO: Is it really necessary to access the database for location?
+    # I think it's possible to get the normalized phone number and the international code
+    # from original_phone_number
+    def process_phone(self, original_phone_number: str, country_iso_code: str = None, details: dict = None) -> dict:
         """
         Process phone number and return normalized phone number.
         :param original_phone_number: Original phone number.
-        :param contact_id: Contact id.
+        :param country_iso_code: Country ISO code.
+        :param details: Dictionary with the details of the phone number
+                (at least one of: country_id, location_id, profile_id, contact_id).
         :return: Dictionary with the normalized phone number and the international code.
         """
+        details = details or {}
+        assert country_iso_code or details, "country_iso_code or details is required"
         logger.start(object={'original_phone_number': original_phone_number})
-        self.set_schema(schema_name='location_profile')
-        profile_id = logger.user_context.get_effective_profile_id()
-        location_id = self.select_one_tuple_by_id(view_table_name='location_profile_view', select_clause_value='location_id',
-                                                  id_column_name='profile_id', id_column_value=profile_id)[0]
-        if location_id is None:
-            logger.error(
-                f"profile {profile_id} location is not set phone number will cannot normalized")
-            return None
-        self.set_schema(schema_name='location')
-        country_id = self.select_one_tuple_by_id(view_table_name='location_view',  select_clause_value='country_id',
-                                                 id_column_name='location_id', id_column_value=location_id)[0]
-        country_iso_code = self.select_one_tuple_by_id(view_table_name='country_ml_view', select_clause_value='iso',
-                                                       id_column_name='country_id', id_column_value=country_id)[0]
+        country_iso_code = country_iso_code or self.get_country_iso_code(details)
         normalized_phone_number = self.normalize_phone_number(
             original_number=original_phone_number, region=country_iso_code)
         phone_data = {
             'number_original': original_phone_number,
             'international_code': normalized_phone_number['international_code'],
             'full_number_normalized': normalized_phone_number['full_number_normalized'],
             'local_number_normalized': int(str(normalized_phone_number['full_number_normalized'])
                                            .replace(str(normalized_phone_number['international_code']), '')),
             'created_user_id': logger.user_context.get_effective_user_id(),
         }
-        self.set_schema(schema_name='phone')
         phone_id = self.insert(data_json=phone_data)
 
-        self.set_schema(schema_name='phone_profile')
         # link phone to profile
-        phone_profile_id = self.insert_mapping(
-            entity_name1='phone', entity_name2='profile', entity_id1=phone_id, entity_id2=profile_id)
+        profile_id = details.get('profile_id')
+        if profile_id:
+            phone_profile_id = self.insert_mapping(
+                schema_name='phone_profile',
+                entity_name1='phone', entity_name2='profile', entity_id1=phone_id, entity_id2=profile_id)
+        else:
+            phone_profile_id = None
 
         # link phone to contact
-        if contact_id is not None:
-            self.set_schema(schema_name='contact_phone')
+        contact_id = details.get('contact_id')
+        if contact_id:
             contact_phone_id = self.insert_mapping(
-                entity_name1='contact', entity_name2='phone', entity_id1=contact_id, entity_id2=phone_id)
+                schema_name='contact_phone', entity_name1='contact', entity_name2='phone',
+                entity_id1=contact_id, entity_id2=phone_id)
+        else:
+            contact_phone_id = None
 
         result = {
             'phone_profile_id': phone_profile_id,
             'phone_id': phone_id,
             'normalized_phone_number': normalized_phone_number,
             'original_phone_number': original_phone_number,
-            'contact_phone_id': contact_phone_id if contact_id is not None else None,
+            'contact_phone_id': contact_phone_id,
         }
         logger.end("success processing phone number", object=result)
         return result
+
+    def insert_phone(self, phone_data: dict) -> int:
+        """
+        Insert phone data into the phone table.
+        :param phone_data: Dictionary with the phone data.
+        :return: Phone id.
+        """
+        logger.start(object={'phone_data': phone_data})
+        phone_id = self.insert(data_json=phone_data)
+        logger.end("success inserting phone", object={'phone_id': phone_id})
+        return phone_id
+
+    def get_test_phone_id(self, number_original: str, international_code: int = 972) -> int:
+        phone_data = {
+            'number_original': number_original,
+            'local_number_normalized': int(number_original[3:]),  # must be unique
+            'full_number_normalized': f'+{international_code}{number_original[1:]}',
+            'international_code': international_code,
+            'area_code': int(number_original[1:3]),
+            'extension': number_original[3],
+        }
+        return self.insert_phone(phone_data=phone_data)
```

### Comparing `phones-local-0.0.18/pyproject.toml` & `phones_local-0.0.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones-local-0.0.18/setup.py` & `phones_local-0.0.19/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.18',  # https://pypi.org/project/phones-local/
+    version='0.0.19',  # https://pypi.org/project/phones-local/
     author="Circles",
-    author_email="info@circles.life",
+    author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'logger-local>=0.0.76',
-        'database-mysql-local>=0.0.107',
-        'phonenumbers'
+        'logger-local>=0.0.135',
+        'database-mysql-local>=0.0.290',
+        'phonenumbers>=8.13.36'
     ]
 )
```


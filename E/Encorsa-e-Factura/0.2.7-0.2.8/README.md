# Comparing `tmp/encorsa_e_factura-0.2.7.tar.gz` & `tmp/encorsa_e_factura-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encorsa_e_factura-0.2.7.tar", last modified: Mon Apr 29 09:36:52 2024, max compression
+gzip compressed data, was "encorsa_e_factura-0.2.8.tar", last modified: Thu May  9 16:58:26 2024, max compression
```

## Comparing `encorsa_e_factura-0.2.7.tar` & `encorsa_e_factura-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-29 09:36:50.000000 encorsa_e_factura-0.2.7/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/
--rw-r--r--   0 vsts      (1001) docker     (127)     7507 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/WebConRequestUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15500 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/XMLUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/runLocaly.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18434 2024-04-29 09:36:35.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/sincronizare.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-29 09:36:52.947126 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-29 09:36:52.000000 encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-05-09 16:58:23.000000 encorsa_e_factura-0.2.8/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8253 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/WebConRequestUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15963 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/XMLUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/runLocaly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24808 2024-05-09 16:58:11.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/sincronizare.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 16:58:26.646337 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-09 16:58:26.000000 encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/top_level.txt
```

### Comparing `encorsa_e_factura-0.2.7/LICENCE` & `encorsa_e_factura-0.2.8/LICENCE`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.7/PKG-INFO` & `encorsa_e_factura-0.2.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.2.7
+Version: 0.2.8
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `encorsa_e_factura-0.2.7/README.md` & `encorsa_e_factura-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.7/setup.cfg` & `encorsa_e_factura-0.2.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Encorsa_e_Factura
-version = 0.2.7
+version = 0.2.8
 author = Dan Popescu, Razvan Ogrezeanu
 author_email = dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 description = A small example package
 long_description = file: README.md
 url = https://encorsa.ro
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/WebConRequestUtils.py` & `encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/WebConRequestUtils.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,38 +49,43 @@
             "id": parameters['webcon_bentity']
         }
     }
 
     if "webcon_parent_wfdid" in parameters and parameters['webcon_parent_wfdid'] is not None and parameters['webcon_parent_wfdid'] not in ['', 0]:
         body["parentInstanceId"] = parameters['webcon_parent_wfdid']
 
-    add_value_to_form_field(parameters, "duplicate_wfdid_field_guid", body, wfd_id_duplicate)
-    add_value_to_form_field(parameters, "tipInregistrare_Nota_sau_Factura", body, document_type)
+    add_value_to_form_field(
+        parameters, "duplicate_wfdid_field_guid", body, wfd_id_duplicate)
+    add_value_to_form_field(
+        parameters, "tipInregistrare_Nota_sau_Factura", body, document_type)
     add_value_to_form_field(parameters, "ID_Descarcare_ANAF", body, id_anaf)
-    add_value_to_form_field(parameters, "Data_Creare_ANAF", body, iso_data_creare)
+    add_value_to_form_field(
+        parameters, "Data_Creare_ANAF", body, iso_data_creare)
 
     return body
 
+
 def add_value_to_form_field(parameters, parameter_key, body, value):
     if value is None:
         value = ''
-    
+
     value = str(value)
 
     if parameter_key in parameters and parameters[parameter_key] is not None and parameters[parameter_key] not in ['', 0]:
         found = False
         for body_field in body["formFields"]:
             if body_field["guid"] == parameters[parameter_key]:
                 body_field["svalue"] = value
                 found = True
                 break
         if not found:
             body["formFields"].append(
                 {"guid": parameters[parameter_key], "svalue": value})
 
+
 def create_list_of_dicts(data_dict):
     result_list = []
     for item_list_guid, rows in data_dict.items():
         item_list_wrapper = {}
         item_list_wrapper['guid'] = item_list_guid
         row_lists = []
         for row in rows:
@@ -132,22 +137,27 @@
                                  data=json.dumps(payload), proxies=proxies)
 
         if response.status_code == 200:
             try:
                 return response.json()["token"]
             except KeyError:
                 # Key 'token' does not exist in the response
+                print(
+                    "Error at getting WebCon TOKEN: The response JSON does not contain a 'token' key")
                 raise Exception(
                     "Error at getting WebCon TOKEN: The response JSON does not contain a 'token' key")
         else:
             # For non-successful responses, raise an exception with status code and error
+            print(
+                f"Error at getting WebCon TOKEN: HTTP {response.status_code} - {response.text}")
             raise Exception(
                 f"Error at getting WebCon TOKEN: HTTP {response.status_code} - {response.text}")
     except Exception as e:
         # A single catch-all for any exception, including request errors, HTTP errors, and JSON parsing errors
+        print(f"Error at getting WebCon TOKEN: {str(e)}")
         raise Exception(f"Error at getting WebCon TOKEN: {str(e)}")
 
 
 def create_invoice_instance(parameters, token, body):
     url = f"{parameters['webcon_base_url']}/api/data/{parameters['webcon_api_version']}/db/{parameters['webcon_dbid']}/elements?path={parameters['webcon_path']}&mode={parameters['webcon_mode']}"
 
     headers = {
@@ -157,26 +167,31 @@
 
     proxies = {
         'http': None,
         'https': None
     }
 
     try:
-        response = requests.post(url, headers=headers, data=json.dumps(body), proxies=proxies)
+        response = requests.post(url, headers=headers,
+                                 data=json.dumps(body), proxies=proxies)
 
         if response.status_code == 200:
             return response.json()
         else:
             error_message = response.json().get('description', 'Unknown error occurred')
             error_code = response.status_code
             # Including more detailed information in the exception
+            print(
+                f"Failed to create WebCon invoice instance. Error code: {error_code}, Message: {error_message}")
             raise Exception(
                 f"Failed to create WebCon invoice instance. Error code: {error_code}, Message: {error_message}")
     except Exception as e:
         # Catching any other exceptions that weren't anticipated
+        print(
+            f"Failed to create WebCon invoice instance. An unexpected error occurred: {str(e)}")
         raise Exception(
             f"Failed to create WebCon invoice instance. An unexpected error occurred: {str(e)}")
 
 
 """
 Functia trebuie sa isi ia datele dintr-un raport cu facturi care
 contine numai doua coloane: ID-factura si CUI, fara a schimba ordinea lor
@@ -189,32 +204,35 @@
 
     headers = {
         'Content-Type': 'application/json',
         'Authorization': f'Bearer {token}'
     }
 
     proxies = {
-            'http': None,
-            'https': None
+        'http': None,
+        'https': None
     }
 
     filters = {
         f'{parameters["invoice_id_url_filter"]}': invoice_id,
         f'{parameters["supplier_company_id_url_filter"]}': supplier_company_id,
         'page': 1,
         'size': 1
     }
 
     try:
-        response = requests.get(url, headers=headers, params=filters, proxies=proxies)
+        response = requests.get(url, headers=headers,
+                                params=filters, proxies=proxies)
         response.raise_for_status()
         data = response.json()
         count = len(data['rows'])
 
     except Exception as err:
+        print(
+            f"Failed to get Invoices list from WebCon report. An unexpected error occurred: {str(err)}")
         raise Exception(
             f"Failed to get Invoices list from WebCon report. An unexpected error occurred: {str(err)}")
 
     if count <= 0:
         return False, 0
     else:
         max_id = min(data['rows'], key=lambda x: x['id'])['id']
```

### Comparing `encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/XMLUtils.py` & `encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/XMLUtils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import xml.etree.ElementTree as ET
 import os
 
+
 def find_nodes_by_path(root, path, namespaces):
     """
     Find nodes in an XML tree using an absolute path, accounting for the root node.
     :param root: The root node of the XML tree.
     :param path: The absolute path to find nodes, starting from the root.
     :param namespaces: A dictionary mapping namespace prefixes to URIs.
     :return: A list of all nodes matching the path. Empty if no match is found.
     """
     def _find_recursive(node, parts, namespaces):
         # If there are no more parts, return the current node
         # This is the base case of the recursive function
         if not parts:
             return [node]
-        
+
         # Get the next parts of the path
         # If there are no next parts, set next_parts to an empty list
         # This is the recursive case of the function
         next_parts = parts[1:] if len(parts) > 1 else []
 
         # Get the current part of the path
         part = parts[0]
@@ -28,15 +29,15 @@
             prefix, tag = part.split(':', 1)
             # Get the URI corresponding to the prefix
             uri = namespaces.get(prefix, '')
             # Replace the part with the full namespace URI and tag
             # Example: replace 'ubl:Invoice' with '{urn:oasis:names:specification:ubl:schema:xsd:Invoice-2}Invoice'
             # This is the format ElementTree uses for namespaces
             part = f"{{{uri}}}{tag}"
-       
+
         # At the first level, compare part with the root's tag; check if the tag ends with the part
         # This check is made to account for the path starting with the root node
         if node == root:
             # If the root node's tag ends with the part, remove the first part from the list of parts
             if node.tag.endswith(part):
                 # Update the part and next_parts based on the root node's tag
                 part = parts[1]
@@ -48,25 +49,27 @@
                     uri = namespaces.get(prefix, '')
                     part = f"{{{uri}}}{tag}"
 
         found_nodes = []
         # Recursively search for nodes matching the current part in the children of the current node
         for child in node:
             if child.tag.endswith(part):
-                found_nodes.extend(_find_recursive(child, next_parts, namespaces))
+                found_nodes.extend(_find_recursive(
+                    child, next_parts, namespaces))
         return found_nodes
 
     # Normalize and split the path, removing the initial '/' if present
     parts = path[1:].split('/') if path.startswith('/') else path.split('/')
 
     # Start the recursive search from the root with the given path parts
     matched_nodes = _find_recursive(root, parts, namespaces)
-    
+
     return matched_nodes
 
+
 class XMLDataExtractorItemLists:
     def __init__(self, xml_tree, result_dict, namespaces=None):
         self.xml_tree = xml_tree
         self.result_dict = result_dict
         self.namespaces = namespaces if namespaces is not None else {}
 
     def extract_list_data(self, parent_path, columns):
@@ -75,37 +78,41 @@
         :param parent_path: The path to the parent node of the list.
         :param columns: A list of tuples containing the path to the data and the corresponding column name.
             The column name is the field guid from WebCon that will be used in the body for the API request.
         :return: A list of dictionaries, where each dictionary contains the extracted data for an item in the list.
         """
         list_data = []
         # Try to find the parent node based on the parent_path
-        child_row_nodes = find_nodes_by_path(self.xml_tree, parent_path, self.namespaces)
+        child_row_nodes = find_nodes_by_path(
+            self.xml_tree, parent_path, self.namespaces)
         # For each child node, extract the data based on the columns
         for row_node in child_row_nodes:
             row_data = {}
             # For each column, extract the data
             # The column_path is the path is a sub-path of the parent_path
             for column_path, column_name in columns:
                 # If the column_path contains an '@', then it is an attribute
                 if '@' in column_path:
                     # Split the path and attribute name by the '@' character which separates the path from the attribute name
                     element_path, attribute_name = column_path.rsplit('@', 1)
-                    child = find_nodes_by_path(row_node, element_path, self.namespaces)
+                    child = find_nodes_by_path(
+                        row_node, element_path, self.namespaces)
                     # If the child list is not empty, then extract the attribute value
                     if len(child) > 0:
                         child = child[0]
                     # If the child list is empty, then the attribute value is None
                     else:
                         child = None
                     # Extract the attribute value
-                    value = child.get(attribute_name) if child is not None else None
+                    value = child.get(
+                        attribute_name) if child is not None else None
                 else:
                     # If the column_path does not contain an '@', then it is a sub-element
-                    child = find_nodes_by_path(row_node, column_path, self.namespaces)
+                    child = find_nodes_by_path(
+                        row_node, column_path, self.namespaces)
                     # If the child list is not empty, then extract the text value
                     if len(child) > 0:
                         child = child[0]
                     else:
                         child = None
                     # Extract the text value only if the child list is not empty
                     # Otherwise, the value is None
@@ -118,18 +125,21 @@
 
     def extract_all_lists(self):
         all_lists_data = {}
         # For each item list, extract the data
         for list_id, info in self.result_dict.items():
             parent_path, columns = info
             # Extract the data for the current list
-            all_lists_data[list_id] = self.extract_list_data(parent_path, columns)
+            all_lists_data[list_id] = self.extract_list_data(
+                parent_path, columns)
         return all_lists_data
 
 # Step 1 - Extract the template data
+
+
 class XMLTemplateParser:
     def __init__(self, xml_tree, namespaces):
         self.xml_tree = xml_tree
         self.namespaces = namespaces
 
     def parse_template(self):
         template_data = {}
@@ -153,20 +163,23 @@
             else:
                 current_path = f"{path}/{node_tag}"
 
             node_list_id = node.attrib.get("itemList", "")
             node_is_list = node_list_id != ""
 
             if node_is_list and isParentList:
-                raise Exception("Template incorrectly configured. You cannot have nested lists in template configuration!")
+                print(
+                    "Template incorrectly configured. You cannot have nested lists in template configuration!")
+                raise Exception(
+                    "Template incorrectly configured. You cannot have nested lists in template configuration!")
 
             for attr_name, attr_value in node.attrib.items():
                 if attr_name == "itemList":
                     continue
-                
+
                 # Handling attributes with potential namespaces
                 attr_ns_uri = None
                 attr_localname = attr_name
                 if attr_name[0] == "{":
                     attr_ns_uri, attr_localname = attr_name[1:].split("}", 1)
                     attr_namespace_prefix = None
                     for prefix, uri in self.namespaces.items():
@@ -174,40 +187,47 @@
                             attr_namespace_prefix = prefix
                             break
                     full_attr_name = f"{attr_namespace_prefix}:{attr_localname}" if attr_namespace_prefix else attr_localname
                 else:
                     full_attr_name = attr_localname
 
                 if node_is_list:
-                    template_data[f"{current_path}@{full_attr_name}"] = (attr_value, node_list_id)
+                    template_data[f"{current_path}@{full_attr_name}"] = (
+                        attr_value, node_list_id)
                 elif isParentList:
-                    template_data[f"{current_path}@{full_attr_name}"] = (attr_value, parentListID)
+                    template_data[f"{current_path}@{full_attr_name}"] = (
+                        attr_value, parentListID)
                 else:
-                    template_data[f"{current_path}@{full_attr_name}"] = (attr_value, "")
+                    template_data[f"{current_path}@{full_attr_name}"] = (
+                        attr_value, "")
 
             if node.text and node.text.strip():
                 if node_is_list:
-                    template_data[current_path] = (node.text.strip(), node_list_id)
+                    template_data[current_path] = (
+                        node.text.strip(), node_list_id)
                 elif isParentList:
-                    template_data[current_path] = (node.text.strip(), parentListID)
+                    template_data[current_path] = (
+                        node.text.strip(), parentListID)
                 else:
                     template_data[current_path] = (node.text.strip(), "")
 
             for child in node:
-                    if node_is_list:
-                        traverse(child, current_path, True, node_list_id)
-                    elif isParentList:
-                        traverse(child, current_path, True, parentListID)
-                    else:
-                        traverse(child, current_path, False, "")
+                if node_is_list:
+                    traverse(child, current_path, True, node_list_id)
+                elif isParentList:
+                    traverse(child, current_path, True, parentListID)
+                else:
+                    traverse(child, current_path, False, "")
 
         traverse(self.xml_tree.getroot())
         return template_data
 
 # Step 2 - Extract the data from the XML file with form fields values
+
+
 class XMLDataProcessorFormFields:
     def __init__(self, data_xml_tree, template_keys, namespaces):
         """
         Initialize the XMLDataProcessorFormFields object.
         :param data_xml_tree: The XML tree containing the data.
         :param template_keys: A dictionary containing the template keys and their corresponding paths in the XML tree.
         The keys in the dictionary are the paths in the XML tree, and the values are tuples containing the key name and an empty string.
@@ -231,30 +251,32 @@
         # For each path in the template keys, extract the data from the XML tree
         for path, (key, _) in self.template_keys.items():
             # If the path contains an '@', then it is an attribute
             if "@" in path:
                 # Split the path and attribute name by the '@' character which separates the path from the attribute name
                 element_path, attribute_name = path.rsplit('@', 1)
                 # Find the node in the XML tree based on the element_path
-                node = find_nodes_by_path(self.data_xml_tree, element_path, self.namespaces)
+                node = find_nodes_by_path(
+                    self.data_xml_tree, element_path, self.namespaces)
                 # If the node list is not empty, then extract the attribute value
                 if len(node) > 0:
                     node = node[0]
                 else:
                     node = None
                 # Extract the attribute value
                 if node is not None:
                     # Access the attribute directly
                     attr_value = node.get(attribute_name)
                     if attr_value:
                         # Store the attribute value in the extracted data dictionary
                         extracted_data[key] = attr_value
             else:
                 # Adjusted for ET: find the first node that matches the path
-                node = find_nodes_by_path(self.data_xml_tree, path, self.namespaces)
+                node = find_nodes_by_path(
+                    self.data_xml_tree, path, self.namespaces)
                 # Same as before, extract the text value only if the node list is not empty
                 if len(node) > 0:
                     node = node[0]
                 else:
                     node = None
                 # Extract the text value
                 if node is not None:
@@ -263,14 +285,16 @@
                     value = node.text.strip() if node.text else None
                     # Store the text value in the extracted data dictionary
                     extracted_data[key] = value
 
         return extracted_data
 
 # Main Class for XML Processing
+
+
 class XMLProcessor:
     def __init__(self, template_xml_path, xml_string_file_data, namespaces):
         self.template_xml_path = template_xml_path
         self.xml_string_file_data = xml_string_file_data
         self.namespaces = namespaces
 
     def process_xml(self):
@@ -291,26 +315,30 @@
                 else:
                     removed_elements[second_val].append((key, first_val))
                 del template_form_fields_data[key]
 
         item_lists_dict = {}
 
         for key, paths_list in removed_elements.items():
-            common_prefix = os.path.commonprefix([path[0] for path in paths_list])
+            common_prefix = os.path.commonprefix(
+                [path[0] for path in paths_list])
             common_base_path = common_prefix.rsplit('/', 1)[0]
 
             for path, value in paths_list:
-                paths_list[paths_list.index((path, value))] = (path.replace(common_base_path, ''), value)
+                paths_list[paths_list.index((path, value))] = (
+                    path.replace(common_base_path, ''), value)
 
             item_lists_dict[key] = (common_base_path, paths_list)
 
         # Parse the XML data
         data_tree = ET.fromstring(self.xml_string_file_data)
 
         # Assuming XMLDataProcessor and XMLDataProcessorFormFields can work with an Element (root) object
-        data_processor = XMLDataProcessorFormFields(data_tree, template_form_fields_data, self.namespaces)
+        data_processor = XMLDataProcessorFormFields(
+            data_tree, template_form_fields_data, self.namespaces)
         form_fields_data = data_processor.apply_template()
 
-        extractor = XMLDataExtractorItemLists(data_tree, item_lists_dict, self.namespaces)
+        extractor = XMLDataExtractorItemLists(
+            data_tree, item_lists_dict, self.namespaces)
         all_lists_data = extractor.extract_all_lists()
 
-        return all_lists_data, form_fields_data
+        return all_lists_data, form_fields_data
```

### Comparing `encorsa_e_factura-0.2.7/src/Encorsa_e_Factura/runLocaly.py` & `encorsa_e_factura-0.2.8/src/Encorsa_e_Factura/runLocaly.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.7/src/Encorsa_e_Factura.egg-info/PKG-INFO` & `encorsa_e_factura-0.2.8/src/Encorsa_e_Factura.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.2.7
+Version: 0.2.8
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


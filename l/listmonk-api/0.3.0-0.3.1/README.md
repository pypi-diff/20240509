# Comparing `tmp/listmonk_api-0.3.0-py2.py3-none-any.whl.zip` & `tmp/listmonk_api-0.3.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7318 bytes, number of entries: 10
--rw-r--r--  2.0 unx      284 b- defN 23-Oct-15 15:18 listmonk_api/__init__.py
--rw-r--r--  2.0 unx      519 b- defN 23-Oct-15 15:18 listmonk_api/decorators.py
--rw-r--r--  2.0 unx      463 b- defN 23-Oct-15 15:18 listmonk_api/exceptions.py
--rw-r--r--  2.0 unx    24826 b- defN 23-Oct-15 15:18 listmonk_api/listmonk_api.py
--rw-r--r--  2.0 unx      116 b- defN 23-Oct-28 03:22 listmonk_api/version.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Oct-28 03:22 listmonk_api-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3860 b- defN 23-Oct-28 03:22 listmonk_api-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Oct-28 03:22 listmonk_api-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Oct-28 03:22 listmonk_api-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      821 b- defN 23-Oct-28 03:22 listmonk_api-0.3.0.dist-info/RECORD
-10 files, 32071 bytes uncompressed, 5914 bytes compressed:  81.6%
+Zip file size: 7410 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      303 b- defN 24-May-09 03:50 listmonk_api/__init__.py
+-rw-r--r--  2.0 unx      523 b- defN 24-May-09 03:50 listmonk_api/decorators.py
+-rw-r--r--  2.0 unx      469 b- defN 24-May-09 03:50 listmonk_api/exceptions.py
+-rw-r--r--  2.0 unx    25986 b- defN 24-May-09 03:50 listmonk_api/listmonk_api.py
+-rw-r--r--  2.0 unx      116 b- defN 24-May-09 03:50 listmonk_api/version.py
+-rw-r--r--  2.0 unx     1060 b- defN 24-May-09 03:50 listmonk_api-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3859 b- defN 24-May-09 03:50 listmonk_api-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-09 03:50 listmonk_api-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-09 03:50 listmonk_api-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      821 b- defN 24-May-09 03:50 listmonk_api-0.3.1.dist-info/RECORD
+10 files, 33260 bytes uncompressed, 6006 bytes compressed:  81.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: listmonk_api/listmonk_api.py
 Comment: 
 
 Filename: listmonk_api/version.py
 Comment: 
 
-Filename: listmonk_api-0.3.0.dist-info/LICENSE
+Filename: listmonk_api-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: listmonk_api-0.3.0.dist-info/METADATA
+Filename: listmonk_api-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: listmonk_api-0.3.0.dist-info/WHEEL
+Filename: listmonk_api-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: listmonk_api-0.3.0.dist-info/top_level.txt
+Filename: listmonk_api-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: listmonk_api-0.3.0.dist-info/RECORD
+Filename: listmonk_api-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## listmonk_api/__init__.py

```diff
@@ -8,7 +8,9 @@
 
 A Python Wrapper for Listmonk API
 """
 
 __version__ = __version__
 __author__ = __author__
 __credits__ = __credits__
+
+__all__ = ["Api"]
```

## listmonk_api/decorators.py

```diff
@@ -1,20 +1,24 @@
 #!/usr/bin/python
 # coding: utf-8
 
 import functools
+
 try:
     from listmonk_api.exceptions import LoginRequiredError
 except ModuleNotFoundError:
     from exceptions import LoginRequiredError
 
+
 def require_auth(function):
     """
     Wraps API calls in function that ensures headers are passed
     with a token
     """
+
     @functools.wraps(function)
     def wrapper(self, *args, **kwargs):
         if not self.headers:
             raise LoginRequiredError
         return function(self, *args, **kwargs)
+
     return wrapper
```

## listmonk_api/exceptions.py

```diff
@@ -1,36 +1,42 @@
 #!/usr/bin/python
 # coding: utf-8
 
+
 class AuthError(Exception):
     """
     Authentication error
     """
+
     pass
 
 
 class UnauthorizedError(AuthError):
     """
     Unauthorized error
     """
+
     pass
 
 
 class MissingParameterError(Exception):
     """
     Missing Parameter error
     """
+
     pass
 
 
 class ParameterError(Exception):
     """
     Parameter error
     """
+
     pass
 
 
 class LoginRequiredError(Exception):
     """
     Authentication error
     """
+
     pass
```

## listmonk_api/listmonk_api.py

```diff
@@ -7,17 +7,27 @@
 from base64 import b64encode
 
 try:
     from listmonk_api.decorators import require_auth
 except ModuleNotFoundError:
     from decorators import require_auth
 try:
-    from listmonk_api.exceptions import (AuthError, UnauthorizedError, ParameterError, MissingParameterError)
+    from listmonk_api.exceptions import (
+        AuthError,
+        UnauthorizedError,
+        ParameterError,
+        MissingParameterError,
+    )
 except ModuleNotFoundError:
-    from exceptions import (AuthError, UnauthorizedError, ParameterError, MissingParameterError)
+    from exceptions import (
+        AuthError,
+        UnauthorizedError,
+        ParameterError,
+        MissingParameterError,
+    )
 
 
 class Api(object):
 
     def __init__(self, url=None, username=None, password=None, token=None, verify=True):
         if url is None:
             raise MissingParameterError
@@ -28,551 +38,698 @@
         self.verify = verify
 
         if self.verify is False:
             urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
         if token:
             self.headers = {
-                'Authorization': f'Bearer {token}',
-                'Content-Type': 'application/json'
+                "Authorization": f"Bearer {token}",
+                "Content-Type": "application/json",
             }
         elif username and password:
-            user_pass = f'{username}:{password}'.encode()
+            user_pass = f"{username}:{password}".encode()
             user_pass_encoded = b64encode(user_pass).decode()
             self.headers = {
-                'Authorization': f'Basic {user_pass_encoded}',
-                'Content-Type': 'application/json'
+                "Authorization": f"Basic {user_pass_encoded}",
+                "Content-Type": "application/json",
             }
         else:
             raise MissingParameterError
 
-        response = self._session.get(f'{self.url}/subscribers', headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/subscribers", headers=self.headers, verify=self.verify
+        )
 
         if response.status_code == 403:
             raise UnauthorizedError
         elif response.status_code == 401:
             raise AuthError
         elif response.status_code == 404:
             raise ParameterError
 
     ####################################################################################################################
     #                                              Subscribers API                                                     #
     ####################################################################################################################
     @require_auth
     def get_subscribers(self, query=None, list_id=None, max_pages=0, per_page=100):
         data = None
-        response = self._session.get(f'{self.url}/subscribers?per_page={per_page}&x-total-pages',
-                                     headers=self.headers, verify=self.verify)
-        total_pages = int(response.headers['X-Total-Pages'])
+        response = self._session.get(
+            f"{self.url}/subscribers?per_page={per_page}&x-total-pages",
+            headers=self.headers,
+            verify=self.verify,
+        )
+        total_pages = int(response.headers["X-Total-Pages"])
         response = []
-        subscriber_filter = f'?per_page={per_page}'
+        subscriber_filter = f"?per_page={per_page}"
         if query:
             try:
                 data = json.dumps(query, indent=4)
             except ValueError:
                 raise ParameterError
         if list_id:
             if not isinstance(list_id, int) and not isinstance(list_id, list):
                 raise ParameterError
             if isinstance(list_id, list):
                 for single_list_id in list_id:
-                    subscriber_filter = f'{subscriber_filter}&list_id={single_list_id}'
+                    subscriber_filter = f"{subscriber_filter}&list_id={single_list_id}"
             else:
-                subscriber_filter = f'{subscriber_filter}&list_id={list_id}'
+                subscriber_filter = f"{subscriber_filter}&list_id={list_id}"
         if max_pages == 0 or max_pages > total_pages:
             max_pages = total_pages
         for page in range(0, max_pages):
-            response_page = self._session.get(f'{self.url}/subscribers{subscriber_filter}&page={page}',
-                                              headers=self.headers, data=data, verify=self.verify)
-            response_page = json.loads(response_page.text.replace('"', '\"'))
+            response_page = self._session.get(
+                f"{self.url}/subscribers{subscriber_filter}&page={page}",
+                headers=self.headers,
+                data=data,
+                verify=self.verify,
+            )
+            response_page = json.loads(response_page.text.replace('"', '"'))
             response = response + response_page
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def get_subscriber(self, subscriber_id=None):
         if subscriber_id is None:
             raise MissingParameterError
-        response = self._session.get(f'{self.url}/subscribers/{subscriber_id}',
-                                     headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/subscribers/{subscriber_id}",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def get_subscribers_from_list(self, list_id=None):
         if list_id is None:
             raise MissingParameterError
-        response = self._session.get(f'{self.url}/subscribers/lists/{list_id}',
-                                     headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/subscribers/lists/{list_id}",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
-    def create_subscriber(self, email=None, name=None, status=None, lists=None, attributes=None,
-                          preconfirm_subscriptions=True):
+    def create_subscriber(
+        self,
+        email=None,
+        name=None,
+        status=None,
+        lists=None,
+        attributes=None,
+        preconfirm_subscriptions=True,
+    ):
         if email is None or name is None or status is None:
             raise MissingParameterError
         if isinstance(email, str) and isinstance(name, str) and isinstance(status, str):
-            data = {'email': email, 'name': name, 'status': status}
+            data = {"email": email, "name": name, "status": status}
         else:
             raise ParameterError
         if lists and isinstance(lists, list):
-            data['lists'] = lists
+            data["lists"] = lists
         if attributes and isinstance(attributes, dict):
-            data['attribs'] = attributes
+            data["attribs"] = attributes
         if isinstance(preconfirm_subscriptions, bool):
-            data['preconfirm_subscriptions'] = preconfirm_subscriptions
+            data["preconfirm_subscriptions"] = preconfirm_subscriptions
         try:
             data = json.dumps(data, indent=4)
         except ValueError:
             raise ParameterError
-        response = self._session.post(f'{self.url}/subscribers',
-                                      headers=self.headers, data=data, verify=self.verify)
+        response = self._session.post(
+            f"{self.url}/subscribers",
+            headers=self.headers,
+            data=data,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     ####################################################################################################################
     #                                                  Lists API                                                       #
     ####################################################################################################################
     @require_auth
-    def get_lists(self, query=None, order_by=None, order=None, max_pages=0, per_page=100):
+    def get_lists(
+        self, query=None, order_by=None, order=None, max_pages=0, per_page=100
+    ):
         data = None
-        response = self._session.get(f'{self.url}/lists?per_page={per_page}&x-total-pages',
-                                     headers=self.headers, verify=self.verify)
-        total_pages = int(response.headers['X-Total-Pages'])
+        response = self._session.get(
+            f"{self.url}/lists?per_page={per_page}&x-total-pages",
+            headers=self.headers,
+            verify=self.verify,
+        )
+        total_pages = int(response.headers["X-Total-Pages"])
         response = []
-        list_filter = f'?per_page={per_page}'
+        list_filter = f"?per_page={per_page}"
         if query:
             try:
                 data = json.dumps(query, indent=4)
             except ValueError:
                 raise ParameterError
-        if order_by and order_by in ['name', 'status', 'created_at', 'updated_at']:
-            list_filter = f'{list_filter}&order_by={order_by}'
-        if order and order.upper() in ['ASC', 'DESC']:
-            list_filter = f'{list_filter}&order={order}'
+        if order_by and order_by in ["name", "status", "created_at", "updated_at"]:
+            list_filter = f"{list_filter}&order_by={order_by}"
+        if order and order.upper() in ["ASC", "DESC"]:
+            list_filter = f"{list_filter}&order={order}"
         if max_pages == 0 or max_pages > total_pages:
             max_pages = total_pages
         for page in range(0, max_pages):
-            response_page = self._session.get(f'{self.url}/lists{list_filter}&page={page}',
-                                              headers=self.headers, data=data, verify=self.verify)
-            response_page = json.loads(response_page.text.replace('"', '\"'))
+            response_page = self._session.get(
+                f"{self.url}/lists{list_filter}&page={page}",
+                headers=self.headers,
+                data=data,
+                verify=self.verify,
+            )
+            response_page = json.loads(response_page.text.replace('"', '"'))
             response = response + response_page
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def get_list(self, list_id=None):
         if list_id is None:
             raise MissingParameterError
-        response = self._session.get(f'{self.url}/lists/{list_id}', headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/lists/{list_id}", headers=self.headers, verify=self.verify
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def create_list(self, name=None, visibility_type=None, optin=None, tags=None):
         if name is None or type is None or optin is None:
             raise MissingParameterError
         data = {}
         if name:
             if not isinstance(name, str):
                 raise ParameterError
             else:
-                data['name'] = name
+                data["name"] = name
         if visibility_type:
-            if not isinstance(visibility_type, str) and optin not in ['private', 'public']:
+            if not isinstance(visibility_type, str) and optin not in [
+                "private",
+                "public",
+            ]:
                 raise ParameterError
             else:
-                data['type'] = visibility_type
+                data["type"] = visibility_type
         if optin:
-            if not isinstance(optin, str) and optin not in ['single', 'double']:
+            if not isinstance(optin, str) and optin not in ["single", "double"]:
                 raise ParameterError
             else:
-                data['optin'] = optin
+                data["optin"] = optin
         if tags:
             if not isinstance(tags, list):
                 raise ParameterError
             else:
-                data['tags'] = tags
+                data["tags"] = tags
         try:
             data = json.dumps(data, indent=4)
         except ValueError:
             raise ParameterError
-        response = self._session.post(f'{self.url}/lists', data=data, headers=self.headers, verify=self.verify)
+        response = self._session.post(
+            f"{self.url}/lists", data=data, headers=self.headers, verify=self.verify
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
-    def edit_list(self, list_id=None, name=None, visibility_type=None, optin=None, tags=None):
+    def edit_list(
+        self, list_id=None, name=None, visibility_type=None, optin=None, tags=None
+    ):
         if list_id is None:
             raise MissingParameterError
         data = {}
         if name:
             if not isinstance(name, str):
                 raise ParameterError
             else:
-                data['name'] = name
+                data["name"] = name
         if visibility_type:
-            if not isinstance(visibility_type, str) and optin not in ['private', 'public']:
+            if not isinstance(visibility_type, str) and optin not in [
+                "private",
+                "public",
+            ]:
                 raise ParameterError
             else:
-                data['type'] = visibility_type
+                data["type"] = visibility_type
         if optin:
-            if not isinstance(optin, str) and optin not in ['single', 'double']:
+            if not isinstance(optin, str) and optin not in ["single", "double"]:
                 raise ParameterError
             else:
-                data['optin'] = optin
+                data["optin"] = optin
         if tags:
             if not isinstance(tags, list):
                 raise ParameterError
             else:
-                data['tags'] = tags
+                data["tags"] = tags
         try:
             data = json.dumps(data, indent=4)
         except ValueError:
             raise ParameterError
-        response = self._session.put(f'{self.url}/lists/{list_id}', data=data, headers=self.headers, verify=self.verify)
+        response = self._session.put(
+            f"{self.url}/lists/{list_id}",
+            data=data,
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     ####################################################################################################################
     #                                                 Import API                                                       #
     ####################################################################################################################
     @require_auth
     def get_subscriber_import_status(self):
-        response = self._session.get(f'{self.url}/import/subscribers', headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/import/subscribers", headers=self.headers, verify=self.verify
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def get_subscriber_import_logs(self):
-        response = self._session.get(f'{self.url}/import/subscribers/logs', headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/import/subscribers/logs",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
-    def import_subscribers(self, file=None, mode=None, delimiter=',', id_list=None, overwrite=True):
+    def import_subscribers(
+        self, file=None, mode=None, delimiter=",", id_list=None, overwrite=True
+    ):
         if file is None or mode is None or id_list is None:
             raise MissingParameterError
         if not isinstance(id_list, list):
             raise ParameterError
-        if mode not in ['subscribe', 'blocklist']:
+        if mode not in ["subscribe", "blocklist"]:
             raise ParameterError
         if not isinstance(delimiter, str):
             raise ParameterError
         if not isinstance(overwrite, bool):
             raise ParameterError
         data = {
-            'file': file,
-            'mode': mode,
-            'delim': delimiter,
-            'lists': id_list,
-            'overwrite': overwrite
+            "file": file,
+            "mode": mode,
+            "delim": delimiter,
+            "lists": id_list,
+            "overwrite": overwrite,
         }
         try:
             data = json.dumps(data, indent=4)
         except ValueError:
             raise ParameterError
-        response = self._session.get(f'{self.url}/import/subscribers/', headers=self.headers, data=data,
-                                     verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/import/subscribers/",
+            headers=self.headers,
+            data=data,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def delete_subscriber_import(self):
-        response = self._session.delete(f'{self.url}/import/subscribers/logs', headers=self.headers, verify=self.verify)
+        response = self._session.delete(
+            f"{self.url}/import/subscribers/logs",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     ####################################################################################################################
     #                                                Campaigns API                                                     #
     ####################################################################################################################
     @require_auth
-    def get_campaigns(self, query=None, order_by=None, order=None, max_pages=0, per_page=100):
+    def get_campaigns(
+        self, query=None, order_by=None, order=None, max_pages=0, per_page=100
+    ):
         data = None
-        response = self._session.get(f'{self.url}/campaigns?per_page={per_page}&x-total-pages',
-                                     headers=self.headers, verify=self.verify)
-        total_pages = int(response.headers['X-Total-Pages'])
+        response = self._session.get(
+            f"{self.url}/campaigns?per_page={per_page}&x-total-pages",
+            headers=self.headers,
+            verify=self.verify,
+        )
+        total_pages = int(response.headers["X-Total-Pages"])
         response = []
-        campaign_filter = f'?per_page={per_page}'
+        campaign_filter = f"?per_page={per_page}"
         if query:
             try:
                 data = json.dumps(query, indent=4)
             except ValueError:
                 raise ParameterError
-        if order_by and order_by in ['name', 'status', 'created_at', 'updated_at']:
-            campaign_filter = f'{campaign_filter}&order_by={order_by}'
-        if order and order.upper() in ['ASC', 'DESC']:
-            campaign_filter = f'{campaign_filter}&order={order}'
+        if order_by and order_by in ["name", "status", "created_at", "updated_at"]:
+            campaign_filter = f"{campaign_filter}&order_by={order_by}"
+        if order and order.upper() in ["ASC", "DESC"]:
+            campaign_filter = f"{campaign_filter}&order={order}"
         if max_pages == 0 or max_pages > total_pages:
             max_pages = total_pages
         for page in range(0, max_pages):
-            response_page = self._session.get(f'{self.url}/campaigns{campaign_filter}&page={page}',
-                                              headers=self.headers, data=data, verify=self.verify)
-            response_page = json.loads(response_page.text.replace('"', '\"'))
+            response_page = self._session.get(
+                f"{self.url}/campaigns{campaign_filter}&page={page}",
+                headers=self.headers,
+                data=data,
+                verify=self.verify,
+            )
+            response_page = json.loads(response_page.text.replace('"', '"'))
             response = response + response_page
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def get_campaign(self, campaign_id=None):
         if campaign_id is None:
             raise MissingParameterError
-        response = self._session.get(f'{self.url}/campaigns/{campaign_id}', headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/campaigns/{campaign_id}",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def get_campaign_preview(self, campaign_id=None):
         if campaign_id is None:
             raise MissingParameterError
-        response = self._session.get(f'{self.url}/campaigns/{campaign_id}/preview', headers=self.headers,
-                                     verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/campaigns/{campaign_id}/preview",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def get_campaign_stats(self, campaign_id=None):
         if campaign_id is None:
             raise MissingParameterError
-        response = self._session.get(f'{self.url}/campaigns/{campaign_id}/running/stats?campaign_id={campaign_id}',
-                                     headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/campaigns/{campaign_id}/running/stats?campaign_id={campaign_id}",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
-    def create_campaign(self, name=None, subject=None, lists=None, from_email=None, send_type=None, content_type=None,
-                        body=None, altbody=None, send_at=None, messenger=None, template_id=None, tags=None):
-        if name is None or subject is None or lists is None or send_type is None or content_type is None \
-                or body is None:
+    def create_campaign(
+        self,
+        name=None,
+        subject=None,
+        lists=None,
+        from_email=None,
+        send_type=None,
+        content_type=None,
+        body=None,
+        altbody=None,
+        send_at=None,
+        messenger=None,
+        template_id=None,
+        tags=None,
+    ):
+        if (
+            name is None
+            or subject is None
+            or lists is None
+            or send_type is None
+            or content_type is None
+            or body is None
+        ):
             raise MissingParameterError
         data = {}
         if isinstance(name, str):
-            data['name'] = name
+            data["name"] = name
         if isinstance(subject, str):
-            data['subject'] = subject
+            data["subject"] = subject
         if isinstance(lists, list):
-            data['lists'] = lists
+            data["lists"] = lists
         if isinstance(from_email, str):
-            data['from_email'] = from_email
-        if send_type in ['regular', 'optin']:
-            data['send_type'] = send_type
+            data["from_email"] = from_email
+        if send_type in ["regular", "optin"]:
+            data["send_type"] = send_type
         else:
             raise ParameterError
-        if content_type in ['richtext', 'html', 'markdown', 'plain']:
-            data['content_type'] = content_type
+        if content_type in ["richtext", "html", "markdown", "plain"]:
+            data["content_type"] = content_type
         else:
             raise ParameterError
         if isinstance(body, str):
-            data['body'] = body
+            data["body"] = body
         if isinstance(altbody, str):
-            data['altbody'] = altbody
+            data["altbody"] = altbody
         if isinstance(send_at, str):
-            data['send_at'] = send_at
+            data["send_at"] = send_at
         if isinstance(messenger, str):
-            data['messenger'] = messenger
+            data["messenger"] = messenger
         if isinstance(template_id, int):
-            data['template_id'] = template_id
+            data["template_id"] = template_id
         if isinstance(tags, list):
-            data['tags'] = tags
+            data["tags"] = tags
         try:
             data = json.dumps(data, indent=4)
         except ValueError or AttributeError:
             raise ParameterError
-        response = self._session.post(f'{self.url}/campaigns', data=data, headers=self.headers, verify=self.verify)
+        response = self._session.post(
+            f"{self.url}/campaigns", data=data, headers=self.headers, verify=self.verify
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def set_campaign_status(self, campaign_id=None, status=None):
         if campaign_id is None or status is None:
             raise MissingParameterError
-        if status and status in ['scheduled', 'running', 'paused', 'cancelled']:
-            data = {
-                'status': status
-            }
+        if status and status in ["scheduled", "running", "paused", "cancelled"]:
+            data = {"status": status}
             try:
                 data = json.dumps(data, indent=4)
             except ValueError or AttributeError:
                 raise ParameterError
         else:
             raise ParameterError
-        response = self._session.put(f'{self.url}/campaigns/{campaign_id}/status', data=data, headers=self.headers,
-                                     verify=self.verify)
+        response = self._session.put(
+            f"{self.url}/campaigns/{campaign_id}/status",
+            data=data,
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def delete_campaign(self, campaign_id=None):
         if campaign_id is None:
             raise MissingParameterError
-        response = self._session.delete(f'{self.url}/campaigns/{campaign_id}', headers=self.headers,
-                                      verify=self.verify)
+        response = self._session.delete(
+            f"{self.url}/campaigns/{campaign_id}",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     ####################################################################################################################
     #                                                  Media API                                                       #
     ####################################################################################################################
     @require_auth
     def get_media(self, media_id=None):
         if media_id is None:
             raise MissingParameterError
-        response = self._session.get(f'{self.url}/media', headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/media", headers=self.headers, verify=self.verify
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def upload_media(self, file=None):
         if file is None:
             raise MissingParameterError
-        data = {'file': file}
-        response = self._session.post(f'{self.url}/media', data=data, headers=self.headers, verify=self.verify)
+        data = {"file": file}
+        response = self._session.post(
+            f"{self.url}/media", data=data, headers=self.headers, verify=self.verify
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def delete_media(self, media_id=None):
         if media_id is None:
             raise MissingParameterError
-        response = self._session.delete(f'{self.url}/media/{media_id}', headers=self.headers, verify=self.verify)
+        response = self._session.delete(
+            f"{self.url}/media/{media_id}", headers=self.headers, verify=self.verify
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
+
     ####################################################################################################################
     #                                               Templates API                                                      #
     ####################################################################################################################
     @require_auth
     def get_templates(self, max_pages=0, per_page=100):
         data = None
-        response = self._session.get(f'{self.url}/templates?per_page={per_page}&x-total-pages',
-                                     headers=self.headers, verify=self.verify)
-        total_pages = int(response.headers['X-Total-Pages'])
+        response = self._session.get(
+            f"{self.url}/templates?per_page={per_page}&x-total-pages",
+            headers=self.headers,
+            verify=self.verify,
+        )
+        total_pages = int(response.headers["X-Total-Pages"])
         response = []
-        campaign_filter = f'?per_page={per_page}'
+        campaign_filter = f"?per_page={per_page}"
         if max_pages == 0 or max_pages > total_pages:
             max_pages = total_pages
         for page in range(0, max_pages):
-            response_page = self._session.get(f'{self.url}/templates{campaign_filter}&page={page}',
-                                              headers=self.headers, data=data, verify=self.verify)
-            response_page = json.loads(response_page.text.replace('"', '\"'))
+            response_page = self._session.get(
+                f"{self.url}/templates{campaign_filter}&page={page}",
+                headers=self.headers,
+                data=data,
+                verify=self.verify,
+            )
+            response_page = json.loads(response_page.text.replace('"', '"'))
             response = response + response_page
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def get_template(self, template_id=None):
         if template_id is None:
             raise MissingParameterError
-        response = self._session.get(f'{self.url}/templates/{template_id}', headers=self.headers, verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/templates/{template_id}",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def get_template_preview(self, template_id=None):
         if template_id is None:
             raise MissingParameterError
-        response = self._session.get(f'{self.url}/templates/{template_id}/preview', headers=self.headers,
-                                     verify=self.verify)
+        response = self._session.get(
+            f"{self.url}/templates/{template_id}/preview",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def set_default_template(self, template_id=None):
         if template_id is None:
             raise MissingParameterError
-        response = self._session.put(f'{self.url}/templates/{template_id}/default', headers=self.headers,
-                                     verify=self.verify)
+        response = self._session.put(
+            f"{self.url}/templates/{template_id}/default",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     @require_auth
     def delete_template(self, template_id=None):
         if template_id is None:
             raise MissingParameterError
-        response = self._session.delete(f'{self.url}/templates/{template_id}', headers=self.headers,
-                                     verify=self.verify)
+        response = self._session.delete(
+            f"{self.url}/templates/{template_id}",
+            headers=self.headers,
+            verify=self.verify,
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
 
     ####################################################################################################################
     #                                           Transactional API                                                      #
     ####################################################################################################################
     @require_auth
-    def transactional_message(self, template_id=None, subscriber_email=None, subscriber_id=None, additional_data=None,
-                              headers=None, content_type=None):
+    def transactional_message(
+        self,
+        template_id=None,
+        subscriber_email=None,
+        subscriber_id=None,
+        additional_data=None,
+        headers=None,
+        content_type=None,
+    ):
         if template_id is None:
             raise MissingParameterError
-        data = {
-            'template_id': template_id
-        }
+        data = {"template_id": template_id}
         if subscriber_id:
-            data['subscriber_id']: subscriber_id
+            data["subscriber_id"]: subscriber_id
         elif subscriber_email:
-            data['subscriber_email']: subscriber_email
+            data["subscriber_email"]: subscriber_email
         if additional_data:
-            data['data']: additional_data
+            data["data"]: additional_data
         if headers:
-            data['headers']: headers
+            data["headers"]: headers
         if content_type:
-            if content_type in ['html', 'markdown', 'plain']:
-                data['content_type']: content_type
+            if content_type in ["html", "markdown", "plain"]:
+                data["content_type"]: content_type
             else:
                 raise ParameterError
-        response = self._session.post(f'{self.url}/tx', data=data, headers=self.headers, verify=self.verify)
+        response = self._session.post(
+            f"{self.url}/tx", data=data, headers=self.headers, verify=self.verify
+        )
         try:
             return response.json()
         except ValueError or AttributeError:
             return response
```

## listmonk_api/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.3.0'
-__author__ = 'Audel Rouhi'
-__credits__ = 'Audel Rouhi'
+__version__ = '0.3.1'
+__author__ = "Audel Rouhi"
+__credits__ = "Audel Rouhi"
```

## Comparing `listmonk_api-0.3.0.dist-info/LICENSE` & `listmonk_api-0.3.1.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `listmonk_api-0.3.0.dist-info/METADATA` & `listmonk_api-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: listmonk-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Listmonk API Python Wrapper
 Home-page: https://github.com/Knuckles-Team/listmonk-api
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,15 +39,15 @@
 ![GitHub top language](https://img.shields.io/github/languages/top/Knuckles-Team/listmonk-api)
 ![GitHub language count](https://img.shields.io/github/languages/count/Knuckles-Team/listmonk-api)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Knuckles-Team/listmonk-api)
 ![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/Knuckles-Team/listmonk-api)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/listmonk-api)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/listmonk-api)
 
-*Version: 0.3.0*
+*Version: 0.3.1*
 
 Listmonk API Python Wrapper
 
 This repository is actively maintained - Contributions are welcome!
 
 ### API Calls:
 - Subscribers
@@ -105,8 +105,7 @@
 <img width="100%" height="180em" src="https://github-readme-stats.vercel.app/api?username=Knucklessg1&show_icons=true&hide_border=true&&count_private=true&include_all_commits=true" />
 
 ![GitHub followers](https://img.shields.io/github/followers/Knucklessg1)
 ![GitHub User's stars](https://img.shields.io/github/stars/Knucklessg1)
 </details>
 
 
-
```


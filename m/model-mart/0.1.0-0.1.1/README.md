# Comparing `tmp/model-mart-0.1.0.tar.gz` & `tmp/model-mart-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model-mart-0.1.0.tar", last modified: Mon May  6 09:46:48 2024, max compression
+gzip compressed data, was "model-mart-0.1.1.tar", last modified: Thu May  9 06:17:07 2024, max compression
```

## Comparing `model-mart-0.1.0.tar` & `model-mart-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-05-06 09:46:48.405123 model-mart-0.1.0/
--rw-r--r--   0 lizhengnan   (501) staff       (20)      460 2024-05-06 09:46:48.404918 model-mart-0.1.0/PKG-INFO
--rw-r--r--   0 lizhengnan   (501) staff       (20)       41 2023-09-27 08:51:53.000000 model-mart-0.1.0/README.md
-drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-05-06 09:46:48.403479 model-mart-0.1.0/model_mart/
--rw-r--r--   0 lizhengnan   (501) staff       (20)       41 2023-09-28 09:46:18.000000 model-mart-0.1.0/model_mart/__init__.py
--rw-r--r--   0 lizhengnan   (501) staff       (20)    26576 2024-05-06 09:45:34.000000 model-mart-0.1.0/model_mart/model_mart_utils.py
-drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-05-06 09:46:48.404603 model-mart-0.1.0/model_mart.egg-info/
--rw-r--r--   0 lizhengnan   (501) staff       (20)      460 2024-05-06 09:46:48.000000 model-mart-0.1.0/model_mart.egg-info/PKG-INFO
--rw-r--r--   0 lizhengnan   (501) staff       (20)      241 2024-05-06 09:46:48.000000 model-mart-0.1.0/model_mart.egg-info/SOURCES.txt
--rw-r--r--   0 lizhengnan   (501) staff       (20)        1 2024-05-06 09:46:48.000000 model-mart-0.1.0/model_mart.egg-info/dependency_links.txt
--rw-r--r--   0 lizhengnan   (501) staff       (20)       31 2024-05-06 09:46:48.000000 model-mart-0.1.0/model_mart.egg-info/requires.txt
--rw-r--r--   0 lizhengnan   (501) staff       (20)       11 2024-05-06 09:46:48.000000 model-mart-0.1.0/model_mart.egg-info/top_level.txt
--rw-r--r--   0 lizhengnan   (501) staff       (20)       38 2024-05-06 09:46:48.405196 model-mart-0.1.0/setup.cfg
--rw-r--r--   0 lizhengnan   (501) staff       (20)      791 2024-05-06 09:46:32.000000 model-mart-0.1.0/setup.py
+drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-05-09 06:17:07.072845 model-mart-0.1.1/
+-rw-r--r--   0 lizhengnan   (501) staff       (20)      460 2024-05-09 06:17:07.072695 model-mart-0.1.1/PKG-INFO
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       41 2023-09-27 08:51:53.000000 model-mart-0.1.1/README.md
+drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-05-09 06:17:07.071457 model-mart-0.1.1/model_mart/
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       41 2023-09-28 09:46:18.000000 model-mart-0.1.1/model_mart/__init__.py
+-rw-r--r--   0 lizhengnan   (501) staff       (20)    31058 2024-05-09 06:10:07.000000 model-mart-0.1.1/model_mart/model_mart_utils.py
+drwxr-xr-x   0 lizhengnan   (501) staff       (20)        0 2024-05-09 06:17:07.072436 model-mart-0.1.1/model_mart.egg-info/
+-rw-r--r--   0 lizhengnan   (501) staff       (20)      460 2024-05-09 06:17:07.000000 model-mart-0.1.1/model_mart.egg-info/PKG-INFO
+-rw-r--r--   0 lizhengnan   (501) staff       (20)      241 2024-05-09 06:17:07.000000 model-mart-0.1.1/model_mart.egg-info/SOURCES.txt
+-rw-r--r--   0 lizhengnan   (501) staff       (20)        1 2024-05-09 06:17:07.000000 model-mart-0.1.1/model_mart.egg-info/dependency_links.txt
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       31 2024-05-09 06:17:07.000000 model-mart-0.1.1/model_mart.egg-info/requires.txt
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       11 2024-05-09 06:17:07.000000 model-mart-0.1.1/model_mart.egg-info/top_level.txt
+-rw-r--r--   0 lizhengnan   (501) staff       (20)       38 2024-05-09 06:17:07.072893 model-mart-0.1.1/setup.cfg
+-rw-r--r--   0 lizhengnan   (501) staff       (20)      791 2024-05-09 06:15:43.000000 model-mart-0.1.1/setup.py
```

### Comparing `model-mart-0.1.0/model_mart/model_mart_utils.py` & `model-mart-0.1.1/model_mart/model_mart_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)s: %(message)s', datefmt='%Y-%m-%d %H:%M:%S',
                     stream=sys.stdout)
 
 
 class PandoraBox:
     def __init__(self, username, password, admin_host):
         self.is_login = False
+        self.is_admin = False
         self.user = None
         self.client = None
         self.bucket = None
         self.endpoint = None
         self.region = None
         self.expire = None
         self.session = None
@@ -54,63 +55,50 @@
 
         try:
             if not username or not password:
                 raise ValueError("登录失败，用户名或密码为空")
 
             info = json.dumps({
                 'username': username,
-                'password': password
+                'password': password,
             })
             resp = self._login_req(info)
-
-            if resp.status_code == http.HTTPStatus.BAD_REQUEST:
-                if not resp.text:
-                    return
-                raise ValueError(f"登录失败，错误消息: {resp.json().get('msg')}")
-
             if resp.status_code == http.HTTPStatus.OK:
                 if not resp.text:
                     return
                 code = resp.json().get("code")
                 if code != 0:
                     raise ValueError(f"登录失败，错误消息: {resp.json().get('msg')}")
-                self.key = resp.json()['sts_gateway_info']['access_key']
-                self.secret = resp.json()['sts_gateway_info']['access_secret']
-                self.bucket = resp.json()['sts_gateway_info']['bucket']
-                self.endpoint = resp.json()['sts_gateway_info']['endpoint']
-                self.region = resp.json()['sts_gateway_info']['region']
-                self.expire = resp.json()['sts_gateway_info']['expire']
-                self.session = resp.json()['sts_gateway_info']['session']
-
+                self.key = resp.json()['data']['sts_gateway_info']['access_key']
+                self.secret = resp.json()['data']['sts_gateway_info']['access_secret']
+                self.bucket = resp.json()['data']['sts_gateway_info']['bucket']
+                self.endpoint = resp.json()['data']['sts_gateway_info']['endpoint']
+                self.region = resp.json()['data']['sts_gateway_info']['region']
+                self.expire = resp.json()['data']['sts_gateway_info']['expire']
+                self.session = resp.json()['data']['sts_gateway_info']['session']
+                self.is_admin = resp.json()['data']['is_admin']
+                self.is_sa = resp.json()['data']['is_service_account']
+                self.sa_token = resp.json()['data']['service_account_token']
                 self.client = Minio(
                     self.endpoint,
                     access_key=self.key,
                     secret_key=self.secret,
                     session_token=self.session,
                     region=self.region,
                     secure=False,
                 )
                 self.user = username
                 self.is_login = True
                 logging.info("登录成功")
+            else:
+                resp.raise_for_status()
 
         except Exception as e:
             logging.error(f"登录过程中发生错误: {str(e)}")
 
-    def _handle_error(self, error_message):
-        logging.error(error_message)
-
-    def _handle_request_exception(self, e):
-        if isinstance(e, RequestException):
-            logging.error(f"HTTP请求错误: {str(e)}")
-        elif isinstance(e, HTTPError):
-            logging.error(f"HTTP错误: {str(e)}")
-        else:
-            logging.error(f"发生未知错误: {str(e)}")
-
     def model_init(self, model_name, description, library, data_set, task) -> bool:
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
             if not model_name:
                 raise ValueError("参数 model_name 为空")
 
@@ -118,65 +106,83 @@
                 'model_name': model_name,
                 'description': description,
                 'library': library,
                 'data_set': data_set,
                 'task': task,
                 'creator': self.user,
             })
-
             resp = self._new_model_req(info)
-            resp.raise_for_status()  # 引发HTTP错误
             if resp.status_code == http.HTTPStatus.OK:
-                logging.info("模型创建成功")
-                return True
+                code = resp.json().get("code")
+                if code != 0:
+                    _handle_error(f"Error:  {resp.json().get('msg')}")
+                else:
+                    logging.info("模型创建成功")
+                    return True
+            else:
+                resp.raise_for_status()  # 引发HTTP错误
 
         except ValueError as ve:
-            self._handle_error(f"Error: {str(ve)}")
+            _handle_error(f"Error: {str(ve)}")
             return False
 
         except Exception as e:
-            self._handle_request_exception(e)
+            _handle_request_exception(e)
             return False
 
     def my_models(self):
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
-
-            resp = self._get_user_model_list_req()
-            resp.raise_for_status()
-
+            if not self.is_sa:
+                resp = self._get_user_model_list_req()
+            else:
+                resp = self._sa_get_model_list_req()
             if resp.status_code == http.HTTPStatus.OK:
+                code = resp.json().get("code")
+                if code != 0:
+                    _handle_error(f"Error:  {resp.json().get('msg')}")
+                    return
                 data = resp.json().get("data")
                 return data
+            else:
+                resp.raise_for_status()
 
         except ValueError as ve:
-            self._handle_error(f"Error: {str(ve)}")
+            _handle_error(f"Error: {str(ve)}")
 
         except Exception as e:
-            self._handle_request_exception(e)
+            _handle_request_exception(e)
 
     def get_model(self, model_name, tag, destination_path) -> bool:
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
             if not tag:
                 raise ValueError("参数 tag 为空")
             if not model_name:
                 raise ValueError("参数 model_name 为空")
             if os.path.isfile(destination_path):
                 raise ValueError("参数 destination_path 必须是一个文件夹")
             if not os.path.exists(destination_path):
                 raise ValueError("目标路径不存在")
 
-            resp = self._get_tag_storage_path_req(model_name, tag)
-            resp.raise_for_status()
-
-            blob_path = resp.json().get("blob_path")
+            if not self.is_sa:
+                resp = self._get_tag_storage_path_req(model_name, tag)
+            else:
+                resp = self._sa_get_tag_storage_path_req(model_name, tag)
 
+            if resp.status_code == http.HTTPStatus.OK:
+                code = resp.json().get("code")
+                if code != 0:
+                    _handle_error(f"Error:  {resp.json().get('msg')}")
+                    return False
+                blob_path = resp.json().get("blob_path")
+            else:
+                resp.raise_for_status()
             objects = self.client.list_objects(
                 self.bucket,
                 recursive=True,
                 prefix=blob_path,
             )
 
             for obj in objects:
@@ -188,19 +194,19 @@
                 if err:
                     raise ValueError(f"下载文件时发生错误: {err}")
 
             logging.info("文件下载成功")
             return True
 
         except ValueError as ve:
-            self._handle_error(f"Error: {str(ve)}")
+            _handle_error(f"Error: {str(ve)}")
             return False
 
         except Exception as e:
-            self._handle_request_exception(e)
+            _handle_request_exception(e)
             return False
 
     def get_model_file(self, model_name, tag, rel_path, destination_path) -> bool:
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
             if not tag:
@@ -208,57 +214,74 @@
             if not model_name:
                 raise ValueError("参数 model_name 为空")
             if os.path.isfile(destination_path):
                 raise ValueError("参数 destination_path 必须是一个文件夹")
             if not os.path.exists(destination_path):
                 raise ValueError("目标路径不存在")
 
-            resp = self._get_tag_storage_path_req(model_name, tag)
-            resp.raise_for_status()
-
-            blob_path = resp.json().get("blob_path")
+            if not self.is_sa:
+                resp = self._get_tag_storage_path_req(model_name, tag)
+            else:
+                resp = self._sa_get_tag_storage_path_req(model_name, tag)
 
+            if resp.status_code == http.HTTPStatus.OK:
+                code = resp.json().get("code")
+                if code != 0:
+                    _handle_error(f"Error:  {resp.json().get('msg')}")
+                    return False
+                blob_path = resp.json().get("blob_path")
+            else:
+                resp.raise_for_status()
             object_path = os.path.join(blob_path, rel_path)
 
             # 检查对象是否存在
             try:
-                stat_info = self.client.stat_object(self.bucket, object_name=object_path)
+                self.client.stat_object(self.bucket, object_name=object_path)
             except S3Error as e:
                 if e.code == 'NoSuchKey':
-                    raise ValueError(f"文件 {object_path} 不存在")
+                    _handle_error(f"文件 {object_path} 不存在")
+                    return False
                 else:
-                    raise ValueError(f"检查文件时发生错误: {e}")
+                    _handle_error(f"检查文件时发生错误: {e}")
+                    return False
             file_name = os.path.basename(object_path)
             err = self._download(object_path, os.path.join(destination_path, file_name))
             if err:
                 raise ValueError(f"下载文件时发生错误: {err}")
 
             logging.info('文件下载成功')
             return True
 
         except ValueError as ve:
-            self._handle_error(f"Error: {str(ve)}")
+            _handle_error(f"Error: {str(ve)}")
             return False
 
         except Exception as e:
-            self._handle_request_exception(e)
+            _handle_request_exception(e)
             return False
 
     def version_list(self, model_name):
         try:
             if not self.is_login:
                 raise ValueError("用户未登录")
-
-            resp = self._get_model_version_list_req(model_name)
-            resp.raise_for_status()
+            if not self.is_sa:
+                resp = self._get_model_version_list_req(model_name)
+            else:
+                resp = self._sa_get_model_version_list_req(model_name)
 
             if resp.status_code == http.HTTPStatus.OK:
+                code = resp.json().get("code")
+                if code != 0:
+                    _handle_error(f"Error:  {resp.json().get('msg')}")
+                    return
                 version_list = resp.json().get("version_list")
                 logging.info(version_list)
                 return version_list
+            else:
+                resp.raise_for_status()
 
         except ValueError as ve:
             logging.error(f"错误: {str(ve)}")
 
         except requests.RequestException as re:
             logging.error(f"HTTP请求错误: {str(re)}")
 
@@ -272,19 +295,23 @@
             if not model_name:
                 raise ValueError("参数 model_name 为空")
             if not local_path:
                 raise ValueError("参数 local_path 为空")
             if not tag:
                 raise ValueError("参数 tag 为空")
 
-            blob_path = ""
             guid = str(uuid.uuid4())
 
             resp = self._get_model_id_req(model_name)
-            resp.raise_for_status()
+            if resp.status_code == http.HTTPStatus.OK:
+                code = resp.json().get("code")
+                if code != 0:
+                    _handle_error(f"Error:  {resp.json().get('msg')}")
+            else:
+                resp.raise_for_status()
 
             # 获取文件名和哈希值列表
             file_hash = []
 
             if os.path.isfile(local_path):
                 file_info = hash_files(local_path)
                 file_hash.append(file_info)
@@ -321,21 +348,23 @@
             info = json.dumps({
                 'model_name': model_name,
                 'tag': tag,
                 'blob_path': blob_path,
                 'guid': str(guid),
                 'files_list': file_hash,
             })
-
             address = self._add_model_version_req(info)
             address.raise_for_status()
-
-            if address.status_code == http.HTTPStatus.BAD_REQUEST:
-                raise ValueError(address.json().get("msg"))
-
+            if address.status_code == http.HTTPStatus.OK:
+                code = resp.json().get("code")
+                if code != 0:
+                    _handle_error(f"Error:  {resp.json().get('msg')}")
+                    return False
+            else:
+                resp.raise_for_status()
             logging.info(f"模型{str(model_name)}版本{str(tag)}注册成功")
             return True
 
         except ValueError as ve:
             logging.error(f"错误: {str(ve)}")
 
         except requests.RequestException as re:
@@ -351,19 +380,27 @@
             if not self.is_login:
                 raise ValueError("用户未登录")
             if not tag:
                 raise ValueError("参数 tag 为空")
             if not model_name:
                 raise ValueError("参数 model_name 为空")
 
-            resp = self._get_model_tag_files_req(model_name, tag)
-            resp.raise_for_status()
+            if not self.is_sa:
+                resp = self._get_model_tag_files_req(model_name, tag)
+            else:
+                resp = self._sa_get_model_tag_files_req(model_name, tag)
 
             if resp.status_code == http.HTTPStatus.OK:
+                code = resp.json().get("code")
+                if code != 0:
+                    _handle_error(f"Error:  {resp.json().get('msg')}")
+                    return
                 return resp.json().get("data")
+            else:
+                resp.raise_for_status()
 
         except ValueError as ve:
             logging.error(f"错误: {str(ve)}")
 
         except requests.RequestException as re:
             logging.error(f"HTTP请求错误: {str(re)}")
 
@@ -438,49 +475,84 @@
     def _get_model_id_req(self, model_name):
         headers = {'username': self.user}
         base_url = "{host}/api/v1/model/{model_name}/id" \
             .format(host=self.admin_host, model_name=model_name)
         resp = requests.get(url=base_url, headers=headers)
         return resp
 
+    def _sa_get_model_id_req(self, model_name):
+        headers = {'username': self.user, 'Access-Token': self.sa_token}
+        base_url = "{host}/api/v1/sa/model/{model_name}/id" \
+            .format(host=self.admin_host, model_name=model_name)
+        resp = requests.get(url=base_url, headers=headers)
+        return resp
+
     def _get_model_info_req(self, model_name):
         headers = {'username': self.user}
         base_url = "{host}/api/v1/model/{model_name}/info" \
             .format(host=self.admin_host, model_name=model_name)
         resp = requests.get(url=base_url, headers=headers)
         return resp
 
+    def _sa_get_model_info_req(self, model_name):
+        headers = {'username': self.user, 'Access-Token': self.sa_token}
+        base_url = "{host}/api/v1/sa/model/{model_name}/info" \
+            .format(host=self.admin_host, model_name=model_name)
+        resp = requests.get(url=base_url, headers=headers)
+        return resp
+
     def _get_tag_storage_path_req(self, model_name, model_tag):
         headers = {'username': self.user}
         base_url = "{host}/api/v1/model/tag/{model_name}/{model_tag}/storage" \
             .format(host=self.admin_host, model_name=model_name, model_tag=model_tag)
         resp = requests.get(url=base_url, headers=headers)
         return resp
 
+    def _sa_get_tag_storage_path_req(self, model_name, model_tag):
+        headers = {'username': self.user, 'Access-Token': self.sa_token}
+        base_url = "{host}/api/v1/sa/model/tag/{model_name}/{model_tag}/storage" \
+            .format(host=self.admin_host, model_name=model_name, model_tag=model_tag)
+        resp = requests.get(url=base_url, headers=headers)
+        return resp
+
     def _get_version_storage_path_req(self, model_name, model_version):
         headers = {'username': self.user}
         base_url = "{host}/api/v1/model/version/{model_name}/{model_version}/storage" \
             .format(host=self.admin_host, model_name=model_name, model_version=model_version)
         resp = requests.get(url=base_url, headers=headers)
         return resp
 
     def _get_model_version_list_req(self, model_name):
         headers = {'username': self.user}
         base_url = "{host}/api/v1/model/{model_name}/version/list" \
             .format(host=self.admin_host, model_name=model_name)
         resp = requests.get(url=base_url, headers=headers)
         return resp
 
+    def _sa_get_model_version_list_req(self, model_name):
+        headers = {'username': self.user, 'Access-Token': self.sa_token}
+        base_url = "{host}/api/v1/sa/model/{model_name}/version/list" \
+            .format(host=self.admin_host, model_name=model_name)
+        resp = requests.get(url=base_url, headers=headers)
+        return resp
+
     def _get_user_model_list_req(self):
         headers = {'username': self.user}
         base_url = "{host}/api/v1/{username}/model/list" \
             .format(host=self.admin_host, username=self.user)
         resp = requests.get(url=base_url, headers=headers)
         return resp
 
+    def _sa_get_model_list_req(self):
+        headers = {'username': self.user, 'Access-Token': self.sa_token}
+        base_url = "{host}/api/v1/sa/{username}/model/list" \
+            .format(host=self.admin_host, username=self.user)
+        resp = requests.get(url=base_url, headers=headers)
+        return resp
+
     def _add_model_version_req(self, json_info):
         headers = {'Content-Type': 'application/json', 'username': self.user}
         base_url = "{host}/api/v1/model/version/add".format(host=self.admin_host)
         resp = requests.post(url=base_url, data=json_info, headers=headers)
         return resp
 
     def _new_model_req(self, json_info):
@@ -498,14 +570,21 @@
     def _get_model_tag_files_req(self, model_name, model_tag):
         headers = {'username': self.user}
         base_url = "{host}/api/v1/model/tag/{model_name}/{model_tag}/files" \
             .format(host=self.admin_host, model_name=model_name, model_tag=model_tag)
         resp = requests.get(url=base_url, headers=headers)
         return resp
 
+    def _sa_get_model_tag_files_req(self, model_name, model_tag):
+        headers = {'username': self.user, 'Access-Token': self.sa_token}
+        base_url = "{host}/api/v1/sa/model/tag/{model_name}/{model_tag}/files" \
+            .format(host=self.admin_host, model_name=model_name, model_tag=model_tag)
+        resp = requests.get(url=base_url, headers=headers)
+        return resp
+
     def get_login_status(self):
         return self.is_login
 
 
 def _allfiles(folder):
     try:
         filepath_list = []
@@ -725,7 +804,20 @@
                 hasher.update(chunk)
 
     except Exception as e:
         raise Exception(f"Error reading file '{file_path}': {str(e)}")
 
     # 返回最终的哈希值
     return hasher.hexdigest()
+
+
+def _handle_error(error_message):
+    logging.error(error_message)
+
+
+def _handle_request_exception(e):
+    if isinstance(e, RequestException):
+        logging.error(f"HTTP请求错误: {str(e)}")
+    elif isinstance(e, HTTPError):
+        logging.error(f"HTTP错误: {str(e)}")
+    else:
+        logging.error(f"发生未知错误: {str(e)}")
```

### Comparing `model-mart-0.1.0/setup.py` & `model-mart-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = None
 
 setuptools.setup(
     name="model-mart",  # Replace with your own name
-    version="0.1.0",
+    version="0.1.1",
     author="SoutherLea",
     author_email="lizhengnan@stonewise.cn",
     description="sdk help users to use model market",
     long_description="sdk help users to use model market",
     long_description_content_type="text/markdown",
     url="https://gitlab.stonewise.cn/mlsys/model-mart.git",
     install_requires=[
```


# Comparing `tmp/domolibrary_execution-0.0.7.tar.gz` & `tmp/domolibrary_execution-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary_execution-0.0.7.tar", last modified: Tue Apr 23 17:55:32 2024, max compression
+gzip compressed data, was "domolibrary_execution-0.0.8.tar", last modified: Thu May  9 19:49:19 2024, max compression
```

## Comparing `domolibrary_execution-0.0.7.tar` & `domolibrary_execution-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-23 17:55:32.483271 domolibrary_execution-0.0.7/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.7/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.7/MANIFEST.in
--rw-r--r--   0 codespace  (1000) codespace  (1000)      810 2024-04-23 17:55:32.483271 domolibrary_execution-0.0.7/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.7/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-23 17:55:32.479271 domolibrary_execution-0.0.7/domolibrary_execution/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6798 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.7/domolibrary_execution/FactoryAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5818 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.7/domolibrary_execution/FactoryJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    14659 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.7/domolibrary_execution/FactoryUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.7/domolibrary_execution/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10634 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.7/domolibrary_execution/_modidx.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2668 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.7/domolibrary_execution/core.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.7/domolibrary_execution/process.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2950 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.7/domolibrary_execution/utils.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-23 17:55:32.483271 domolibrary_execution-0.0.7/domolibrary_execution.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      810 2024-04-23 17:55:32.000000 domolibrary_execution-0.0.7/domolibrary_execution.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      642 2024-04-23 17:55:32.000000 domolibrary_execution-0.0.7/domolibrary_execution.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-23 17:55:32.000000 domolibrary_execution-0.0.7/domolibrary_execution.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-04-23 17:55:32.000000 domolibrary_execution-0.0.7/domolibrary_execution.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.7/domolibrary_execution.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-04-23 17:55:32.000000 domolibrary_execution-0.0.7/domolibrary_execution.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-23 17:55:32.000000 domolibrary_execution-0.0.7/domolibrary_execution.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      923 2024-04-23 17:55:19.000000 domolibrary_execution-0.0.7/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-23 17:55:32.483271 domolibrary_execution-0.0.7/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.7/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:19.596207 domolibrary_execution-0.0.8/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.8/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.8/MANIFEST.in
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      810 2024-05-09 19:49:19.596207 domolibrary_execution-0.0.8/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       32 2024-04-19 18:24:29.000000 domolibrary_execution-0.0.8/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:19.592207 domolibrary_execution-0.0.8/domolibrary_execution/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4304 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/FactoryAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5903 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/FactoryRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3582 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/FactoryUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.8/domolibrary_execution/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15277 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/_modidx.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2680 2024-04-23 17:55:23.000000 domolibrary_execution-0.0.8/domolibrary_execution/process.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:19.592207 domolibrary_execution-0.0.8/domolibrary_execution/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2968 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/utils/domojupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7104 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/domolibrary_execution/utils/factory.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-09 19:49:19.592207 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)      810 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      700 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-19 18:25:06.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       22 2024-05-09 19:49:19.000000 domolibrary_execution-0.0.8/domolibrary_execution.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      923 2024-05-09 19:49:16.000000 domolibrary_execution-0.0.8/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-09 19:49:19.596207 domolibrary_execution-0.0.8/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2596 2024-04-19 18:17:25.000000 domolibrary_execution-0.0.8/setup.py
```

### Comparing `domolibrary_execution-0.0.7/LICENSE` & `domolibrary_execution-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary_execution-0.0.7/PKG-INFO` & `domolibrary_execution-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary_execution
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com//domolibrary_execution
 Author: 
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary_execution-0.0.7/domolibrary_execution/FactoryAuth.py` & `domolibrary_execution-0.0.8/domolibrary_execution/FactoryAuth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,216 +1,163 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_FactoryAuth.ipynb.
 
 # %% auto 0
-__all__ = ['generate_config_auth', 'Config_GenerateConfigAuth', 'get_domoaccount', 'Config_DomoJupyterToDomoAccount',
-           'upsert_domoaccount', 'Config_UpsertDomoAccount']
+__all__ = ['generate_config_auth', 'Config_GenerateConfigAuth', 'upsert_domoaccount', 'generate_config_access_token',
+           'Config_UpsertDomoAccessTokenAccount']
 
 # %% ../nbs/00_FactoryAuth.ipynb 1
-from domolibrary_extensions.utils.factory import (
+from .utils.factory import (
     factory_function,
     FactoryLogs, 
     FactoryResponse, FactoryConfig, FactoryMessage)
 
-from domolibrary.client.DomoAuth import DomoAuth
+# %% ../nbs/00_FactoryAuth.ipynb 2
+from dataclasses import dataclass
+from typing import Callable
 
+import domolibrary.client.DomoAuth as dmda
+import domolibrary.classes.DomoAccount as dmac
+import domolibrary_execution.utils.domojupyter as dxdj
 
-# %% ../nbs/00_FactoryAuth.ipynb 2
 import httpx
-from dataclasses import dataclass, field
-from typing import List, Callable
 
-import domolibrary.classes.DomoAccount as dmac
+# %% ../nbs/00_FactoryAuth.ipynb 5
+@factory_function
+async def generate_config_auth(
+    config : FactoryConfig,
+    res: FactoryResponse,
+    
+    config_auth_standard : dmda.DomoAuth,
+    config_auth_exception : dmda.DomoAuth,
+    target_instance_use_exception_pw : bool,
+    target_instance : str,
 
-# %% ../nbs/00_FactoryAuth.ipynb 4
-@factory_function(config_id_col = "domo_instance")
-async def generate_config_auth(config, 
-                               res : FactoryResponse,
-                               logs : FactoryLogs,
-                               session : httpx.AsyncClient = None,  
-                               debug_api : bool = False):
-    
-    config_auth_standard = config.config_auth_standard
-    config_auth_exception = config.config_auth_exception
+    # ouptut
+    auth : dmda.DomoAuth =None, # will be updated during execution
     
-    domo_instance = config.domo_instance
-    
-    res.location = domo_instance    
-    step = FactoryMessage(stage = 'generate_config_auth', message = 'using standard auth')
+    **kwargs
+):
+
+    res.location = target_instance
+    step = FactoryMessage(stage="generate_config_auth", message="using standard auth")
     res.add_message(step)
     auth = config_auth_standard
     step.is_success = True
-    
-    if config.target_instance_use_exception_pw == 1:
+
+    if target_instance_use_exception_pw == 1:
         auth = config_auth_exception
         step.message = "using exception auth"
         step.is_success = True
-        
-    auth.domo_instance = domo_instance
 
-    step = FactoryMessage(stage = 'test is valid auth')
+    auth.domo_instance = target_instance
+
+    step = FactoryMessage(stage="test is valid auth")
     res.add_message(step)
-        
+
     try:
         await auth.print_is_token()
         step.is_success = True
-        step.message = 'valid auth'
-         
+        step.message = "valid auth"
+
     except Exception as e:
         step.message = e
         step.is_success = False
-        
+
     config.auth = auth
     res.response = auth
     return res
 
-# %% ../nbs/00_FactoryAuth.ipynb 5
 @dataclass
 class Config_GenerateConfigAuth(FactoryConfig):
-    config_auth_exception : DomoAuth = None
-    config_auth_standard : DomoAuth = None
-    domo_instance : str = None
-    target_instance_use_exception_pw : int = None
-    factory_fn_ls : List[Callable] = field(default_factory =  lambda : [generate_config_auth])
-
-# %% ../nbs/00_FactoryAuth.ipynb 6
-@factory_function(config_id_col = "account_name")
-async def get_domoaccount(
-    config,
+    config_auth_exception : dmda.DomoAuth
+    config_auth_standard : dmda.DomoAuth
+    target_instance : str
+    target_instance_use_exception_pw : bool = True
+
+    # updated during execution
+    auth: dmda.DomoAuth = None
+
+# %% ../nbs/00_FactoryAuth.ipynb 8
+@factory_function
+async def upsert_domoaccount(
+    config: FactoryConfig,
     res : FactoryResponse,
-    logs : FactoryLogs,
-    session : httpx.AsyncClient = None,  
-    debug_api : bool = False
-    ) -> FactoryResponse:
-    
-    account_name = config.account_name
-    domojupyter_fn = config.domojupyter_fn
-    is_abstract = config.account_is_abstract
-    
-    
-    
-    
-    if not account_name or not domojupyter_fn or is_abstract is None:
-        raise Exception("must pass account_name, dj_fn, and config_is_abstract")
-    
-    step = FactoryMessage(stage = 'get domojupyter creds')
-    res.add_message(step)
-    
-    creds = None
-    try:    
-        creds = dxut.read_domo_jupyter_account(account_name = account_name, 
-                                               domojupyter_fn = domojupyter_fn, 
-                                               is_abstract = is_abstract)
-        step.is_success = True
-        step.message = creds
-    
-    except Exception as e:
-        step.is_success = False
-        step.message = e
-    
-    if not creds:
-        res.response = 'no creds'
-        return res
-    
-    step = FactoryMessage(stage = 'get config for account')
-    res.add_message(step)
 
-    config = None
-    if not is_abstract:
-        config = dmac.AccountConfig.domo_access_token.value
-        config = config(username = creds['username'],
-               password = creds['password'],
-               domo_access_token = creds['domoAccessToken'])
+    auth : dmda.DomoAuth,
     
+    account_name : str,
+    account_config_cls : str,
+    generate_config_fn : Callable,
 
-        
-    creds = {"access_token" : access_token,
-             "password" : creds['DOMO_PASSWORD'] if is_abstract else creds['password'],
-             "username" :creds['DOMO_USERNAME'] if is_abstract else creds['username'],
-             "account_name" : account_name 
-            }
-    
-    step.message = "reformated creds output"
-    return creds
+    modify_config_fn: Callable = None,
+    session : httpx.AsyncClient = None,
+    debug_api: bool = False,
 
-@dataclass
-class Config_DomoJupyterToDomoAccount(FactoryConfig):
-    account_name : str = None, 
-    domojupyter_fn : Callable = None,
-    account_is_abstract : bool = None, 
-    # domo_instance : str = None
-    factory_fn_ls : List[Callable] = field(default_factory =  lambda : [domojupyter_account_to_domoaccount])
+    # used by wrapper
+    **kwargs
 
-# %% ../nbs/00_FactoryAuth.ipynb 7
-@factory_function(config_id_col = "account_name")
-async def upsert_domoaccount(
-    config,
-    res : FactoryResponse,
-    logs : FactoryLogs,
-    session : httpx.AsyncClient = None,
-    debug_api: bool = False
 ):
-    access_token = config.access_token or ""
-    username = config.email or ""
-    password = config.password or ""
-    account_name = config.account_name
-    auth = config.auth
-    config_auth = config.config_auth
-    
     res.location = auth.domo_instance
 
     step = FactoryMessage( stage="upsert domo account", is_success=False)
     res.add_message( step )
     
-    account_config = dmac.AccountConfig['domo_access_token'].value(
-        domo_access_token = access_token,
-        username = username,
-        password = password
-    )
     
     domo_account = None
     try:
+        account_config = generate_config_fn(config, account_config_cls)
+    
         domo_account = await dmac.DomoAccounts.upsert_account(
             auth = auth,
             account_config = account_config,
             account_name = account_name,
             session = session,
             debug_api = debug_api
         )
+
+        config.domo_account = domo_account
+    
         step.is_success = True
-        step.message = 'account upserted'
+        step.message = f'account {account_name} upserted'
         
     except Exception as e:
         step.message = e
         step.is_success = False
         
-    if config_auth:
-        step = FactoryMessage( stage="upsert config instance", is_success=False)
+
+    if modify_config_fn:
+        step = FactoryMessage( stage="modify config", is_success=False)
         res.add_message( step )
     
-        try:
-            domo_account = await dmac.DomoAccounts.upsert_account(
-                auth = config_auth,
-                account_config = account_config,
-                account_name = account_name,
-                session = session,
-                debug_api = False
-            )
-            step.is_success = True
-            step.message = 'account upserted'
+        modify_config_fn(config = config, step = step, 
+                         domo_account = domo_account)
         
-        except Exception as e:
-            step.message = e
-            step.is_success = False
            
-    config.domo_account = domo_account
     res.response = domo_account or 'no account'
         
     return res
 
+
+
+# for different accounts  config object will need different fields
+def generate_config_access_token(config, account_config_cls : dmac.AccountConfig.domo_access_token):
+    return account_config_cls(
+        domo_access_token = config.access_token,
+        username = config.username,
+        password = config.password
+    )
+
 @dataclass
-class Config_UpsertDomoAccount(FactoryConfig):
-    account_name : str = None 
-    access_token : str = ""
-    username : str = ""
-    password : str = ""
-    
-    factory_fn_ls : List[Callable] = field(default_factory =  lambda : [upsert_domoaccount])
+class Config_UpsertDomoAccessTokenAccount(FactoryConfig):
+    account_name : str 
+    generate_config_fn : Callable
+    account_config_cls : dmac.AccountConfig.domo_access_token.value
+
+    ## account params
+    username : str
+    access_token : str = None
+    password : str = None
+
+    # updated during execution
+    domo_account : dmac.DomoAccount = None
+
+
```

### Comparing `domolibrary_execution-0.0.7/domolibrary_execution/core.py` & `domolibrary_execution-0.0.8/domolibrary_execution/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_process.ipynb.
 
 # %% auto 0
 __all__ = ['ResponseProcess', 'ProcessFunction_ResponseTypeError', 'ProcessFunction_Error', 'process_function']
 
-# %% ../nbs/00_core.ipynb 2
+# %% ../nbs/00_process.ipynb 2
 from dataclasses import dataclass, field
 from typing import Any, Callable, List
 from functools import wraps
 import httpx
 
-# %% ../nbs/00_core.ipynb 3
+# %% ../nbs/00_process.ipynb 3
 @dataclass
 class ResponseProcess:
     function_name : str
     id : str
     message: List = field(default_factory = lambda: ['init'])
     response : Any = field(repr = False, default = None)
     is_success : bool = False,
     
     def to_json(self):
         return [ {** self.__dict__, 'message' : msg} for msg in self.message]
 
-# %% ../nbs/00_core.ipynb 5
+# %% ../nbs/00_process.ipynb 5
 class ProcessFunction_ResponseTypeError(TypeError):
     def __init__(self, result):
         super().__init__(
             f"Expected function to return an instance of ResponseProcess got {type(result)} instead.  Refactor function to return ResponseGetData class"
         )
 
 class ProcessFunction_Error(Exception):
```

### Comparing `domolibrary_execution-0.0.7/domolibrary_execution/utils.py` & `domolibrary_execution-0.0.8/domolibrary_execution/utils/domojupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_utils.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/00_utils.ipynb.
 
 # %% auto 0
 __all__ = ['which_environment', 'read_domo_jupyter_account', 'domojupyter_to_domoauth']
 
-# %% ../nbs/00_utils.ipynb 2
+# %% ../../nbs/00_utils.ipynb 2
 import os 
 import urllib.parse as urllib_parse
 import json
 
 
 from operator import itemgetter
 
 import json
 from typing import Callable
 
 import domolibrary.client.DomoAuth as dmda
 
-# %% ../nbs/00_utils.ipynb 3
+# %% ../../nbs/00_utils.ipynb 3
 def which_environment():
     return urllib_parse.urlparse(os.environ.get('DOMO_HOSTNAME')).netloc.replace('.domo.com', '')
     
 
-# %% ../nbs/00_utils.ipynb 4
+# %% ../../nbs/00_utils.ipynb 4
 def read_domo_jupyter_account(account_name,
                               domojupyter_fn : Callable,
                               is_abstract: bool = False,
                               is_dict : bool = True
                             
                              ):
 
@@ -44,21 +44,21 @@
     if not is_dict:
         return creds.strip()
     
     return json.loads(
         creds
     )
 
-# %% ../nbs/00_utils.ipynb 5
+# %% ../../nbs/00_utils.ipynb 5
 def remove_asterix(text):
     if text == '' or text == '********':
         return None
     return text
 
-# %% ../nbs/00_utils.ipynb 6
+# %% ../../nbs/00_utils.ipynb 6
 async def domojupyter_to_domoauth(
     account_name,
     instance,
     domojupyter_fn: Callable,
     is_abstract: bool,
     is_test: bool = True
 ) -> dict:
```

### Comparing `domolibrary_execution-0.0.7/domolibrary_execution.egg-info/PKG-INFO` & `domolibrary_execution-0.0.8/domolibrary_execution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary-execution
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com//domolibrary_execution
 Author: 
 Author-email: 
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `domolibrary_execution-0.0.7/domolibrary_execution.egg-info/SOURCES.txt` & `domolibrary_execution-0.0.8/domolibrary_execution.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 domolibrary_execution/FactoryAuth.py
-domolibrary_execution/FactoryJupyter.py
+domolibrary_execution/FactoryRole.py
 domolibrary_execution/FactoryUser.py
 domolibrary_execution/__init__.py
 domolibrary_execution/_modidx.py
-domolibrary_execution/core.py
 domolibrary_execution/process.py
-domolibrary_execution/utils.py
 domolibrary_execution.egg-info/PKG-INFO
 domolibrary_execution.egg-info/SOURCES.txt
 domolibrary_execution.egg-info/dependency_links.txt
 domolibrary_execution.egg-info/entry_points.txt
 domolibrary_execution.egg-info/not-zip-safe
 domolibrary_execution.egg-info/requires.txt
-domolibrary_execution.egg-info/top_level.txt
+domolibrary_execution.egg-info/top_level.txt
+domolibrary_execution/utils/__init__.py
+domolibrary_execution/utils/domojupyter.py
+domolibrary_execution/utils/factory.py
```

### Comparing `domolibrary_execution-0.0.7/settings.ini` & `domolibrary_execution-0.0.8/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domolibrary_execution
 lib_name = %(repo)s
-version = 0.0.7
+version = 0.0.8
 min_python = 3.8
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = %(repo)s
```

### Comparing `domolibrary_execution-0.0.7/setup.py` & `domolibrary_execution-0.0.8/setup.py`

 * *Files identical despite different names*


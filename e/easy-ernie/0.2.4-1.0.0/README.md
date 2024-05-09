# Comparing `tmp/easy_ernie-0.2.4.tar.gz` & `tmp/easy_ernie-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_ernie-0.2.4.tar", last modified: Fri May  3 04:29:20 2024, max compression
+gzip compressed data, was "easy_ernie-1.0.0.tar", last modified: Thu May  9 13:06:08 2024, max compression
```

## Comparing `easy_ernie-0.2.4.tar` & `easy_ernie-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:29:20.889052 easy_ernie-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-03 04:29:09.000000 easy_ernie-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-03 04:29:20.889052 easy_ernie-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-03 04:29:09.000000 easy_ernie-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 04:29:20.889052 easy_ernie-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-03 04:29:09.000000 easy_ernie-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:29:20.885052 easy_ernie-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:29:20.889052 easy_ernie-0.2.4/src/easy_ernie/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-03 04:29:09.000000 easy_ernie-0.2.4/src/easy_ernie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 04:29:09.000000 easy_ernie-0.2.4/src/easy_ernie/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)    12255 2024-05-03 04:29:09.000000 easy_ernie-0.2.4/src/easy_ernie/ernie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-03 04:29:09.000000 easy_ernie-0.2.4/src/easy_ernie/fast_ernie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 04:29:20.889052 easy_ernie-0.2.4/src/easy_ernie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-03 04:29:20.000000 easy_ernie-0.2.4/src/easy_ernie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-03 04:29:20.000000 easy_ernie-0.2.4/src/easy_ernie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 04:29:20.000000 easy_ernie-0.2.4/src/easy_ernie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-03 04:29:20.000000 easy_ernie-0.2.4/src/easy_ernie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 04:29:20.000000 easy_ernie-0.2.4/src/easy_ernie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/src/easy_ernie/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/ernie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/fast_ernie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 13:05:53.000000 easy_ernie-1.0.0/src/easy_ernie/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:06:08.368991 easy_ernie-1.0.0/src/easy_ernie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 13:06:08.000000 easy_ernie-1.0.0/src/easy_ernie.egg-info/top_level.txt
```

### Comparing `easy_ernie-0.2.4/LICENSE` & `easy_ernie-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_ernie-0.2.4/PKG-INFO` & `easy_ernie-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 0.2.4
+Version: 1.0.0
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -14,20 +14,21 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
+## Easy-Ernie原仓库误删,新建的
 ## 提示
 1. 有封号风险.
 2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
-3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/6)回复,我会及时更新Acs-Token算法的参数.
+3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/1)回复,我会及时更新Acs-Token算法的参数.
 ---
-![Release](https://img.shields.io/badge/Release-0.2.4-blue)
+![Release](https://img.shields.io/badge/Release-1.0.0-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI.
 ## 需求
 1. 语言: Python3.8+.
 2. 其他: 文心一言账户.
 ## 安装
@@ -37,36 +38,34 @@
 1. 访问[文心一言](https://yiyan.baidu.com).
 2. 打开开发者工具.
 3. 找到应用程序(Application).
 4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
 5. 在列表中点击BAIDUID.
 6. 复制下方Value的值.
 7. BDUSS_BFESS同理.
-## 使用
+## 示例
 ### Ernie
 ```python
 from easy_ernie import Ernie
 
 if __name__ == '__main__':
     ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
     sessionName = '你好'
-    result1 = ernie.ask('你好', sessionName=sessionName)
-    sessionId = result1['sessionId']
-    chatBotId = result1['chatBotId']
-    print(result1)
-    result2 = ernie.ask('我给你发的上一个消息是什么', sessionId=sessionId, sessionName=sessionName, parentChatId=chatBotId)
-    print(result2)
-    ernie.deleteConversation(sessionId)
+    response1 = ernie.ask('你好', sessionName=sessionName)
+    print(response1.answer)
+    response2 = ernie.ask('我给你发的上一个消息是什么', sessionId=response1.sessionId, sessionName=sessionName, parentChatId=response1.botChatId)
+    print(response2.answer)
+    ernie.deleteSession(response1.sessionId)
 ```
 ### FastErinie
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
-    print(fastErnie.ask('你好'))
-    print(fastErnie.ask('我给你发的上一个消息是什么'))
+    print(fastErnie.ask('你好').answer)
+    print(fastErnie.ask('我给你发的上一个消息是什么').answer)
     fastErnie.close()
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## 感谢
 灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy_ernie-0.2.4/README.md` & `easy_ernie-1.0.0/src/easy_ernie.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,34 @@
+Metadata-Version: 2.1
+Name: easy-ernie
+Version: 1.0.0
+Summary: 简洁的调用文心一言的WebAPI
+Home-page: https://github.com/XiaoXinYo/Easy-Ernie
+Author: XiaoXinYo
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
+## Easy-Ernie原仓库误删,新建的
 ## 提示
 1. 有封号风险.
 2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
-3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/6)回复,我会及时更新Acs-Token算法的参数.
+3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/1)回复,我会及时更新Acs-Token算法的参数.
 ---
-![Release](https://img.shields.io/badge/Release-0.2.4-blue)
+![Release](https://img.shields.io/badge/Release-1.0.0-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI.
 ## 需求
 1. 语言: Python3.8+.
 2. 其他: 文心一言账户.
 ## 安装
@@ -17,36 +38,34 @@
 1. 访问[文心一言](https://yiyan.baidu.com).
 2. 打开开发者工具.
 3. 找到应用程序(Application).
 4. 在左侧点击存储(Storage)-Cookies-https://yiyan.baidu.com.
 5. 在列表中点击BAIDUID.
 6. 复制下方Value的值.
 7. BDUSS_BFESS同理.
-## 使用
+## 示例
 ### Ernie
 ```python
 from easy_ernie import Ernie
 
 if __name__ == '__main__':
     ernie = Ernie('BAIDUID', 'BDUSS_BFESS')
     sessionName = '你好'
-    result1 = ernie.ask('你好', sessionName=sessionName)
-    sessionId = result1['sessionId']
-    chatBotId = result1['chatBotId']
-    print(result1)
-    result2 = ernie.ask('我给你发的上一个消息是什么', sessionId=sessionId, sessionName=sessionName, parentChatId=chatBotId)
-    print(result2)
-    ernie.deleteConversation(sessionId)
+    response1 = ernie.ask('你好', sessionName=sessionName)
+    print(response1.answer)
+    response2 = ernie.ask('我给你发的上一个消息是什么', sessionId=response1.sessionId, sessionName=sessionName, parentChatId=response1.botChatId)
+    print(response2.answer)
+    ernie.deleteSession(response1.sessionId)
 ```
 ### FastErinie
 ```python
 from easy_ernie import FastErnie
 
 if __name__ == '__main__':
     fastErnie = FastErnie('BAIDUID', 'BDUSS_BFESS')
-    print(fastErnie.ask('你好'))
-    print(fastErnie.ask('我给你发的上一个消息是什么'))
+    print(fastErnie.ask('你好').answer)
+    print(fastErnie.ask('我给你发的上一个消息是什么').answer)
     fastErnie.close()
 ```
 更多方法查看[Wiki](https://github.com/XiaoXinYo/Easy-Ernie/wiki).
 ## 感谢
-灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
+灵感来源自[acheong08](https://github.com/acheong08),[ls233](https://github.com/lss233).
```

### Comparing `easy_ernie-0.2.4/setup.py` & `easy_ernie-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r', encoding='utf-8') as file:
-    long_description = file.read()
+    readMe = file.read()
 
 setup(
     name='easy-ernie',
-    version='0.2.4',
+    version='1.0.0',
     description='简洁的调用文心一言的WebAPI',
-    long_description=long_description,
+    long_description=readMe,
     long_description_content_type='text/markdown',
     author='XiaoXinYo',
     url='https://github.com/XiaoXinYo/Easy-Ernie',
     packages=find_packages('./src'),
     license='MIT',
     package_dir={'': './src'},
     classifiers=[
```

### Comparing `easy_ernie-0.2.4/src/easy_ernie/ernie.py` & `easy_ernie-1.0.0/src/easy_ernie/ernie.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,333 +1,245 @@
 from typing import Generator, Optional
-from . import auxiliary
+from . import auxiliary, model
 import requests
 import re
 import json
 
 class Ernie:
     def __init__(self, BAIDUID: str, BDUSS_BFESS: str):
         self.BAIDUID = BAIDUID
         self.session = requests.Session()
         self.session.headers = {
             'Accept': '*/*',
-            'Accept-Encoding': 'gzip, deflate, br',
+            'Accept-Encoding': 'gzip, deflate, br, zstd',
             'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
             'Connection': 'keep-alive',
+            'Content-Length': '0',
             'Content-Type': 'application/json',
             'Cookie': f'BDUSS_BFESS={BDUSS_BFESS};',
             'Host': 'yiyan.baidu.com',
             'Origin': 'https://yiyan.baidu.com',
             'Referer': 'https://yiyan.baidu.com/',
-            'Sec-Ch-Ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Microsoft Edge";v="114"',
+            'Sec-Ch-Ua': '"Chromium";v="124", "Microsoft Edge";v="124", "Not-A.Brand";v="99"',
             'Sec-Ch-Ua-Mobile': '?0',
             'Sec-Ch-Ua-Platform': '"Windows"',
             'Sec-Fetch-Dest': 'empty',
             'Sec-Fetch-Mode': 'cors',
-            'Sec-Fetch-Site': 'same-site',
-            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.67'
+            'Sec-Fetch-Site': 'same-origin',
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36 Edg/124.0.0.0'
         }
 
     def getAcsToken(self) -> str:
-        return requests.get(f'https://api.api.h2oye.com/other/get_ernie_acs_token?BAIDUID={self.BAIDUID}',).json()['data']
+        return requests.get(f'https://api.api.h2oye.com/other/get_ernie_acs_token?BAIDUID={self.BAIDUID}', ).json()['data']
 
     def checkJson(self, data: str) -> None:
         try:
             data = json.loads(data)
         except:
             raise Exception('请求失败,响应格式错误')
 
-        if 'task_id' not in data and data['code'] != 0:
+        if data['code'] != 0:
             raise Exception(f'请求失败,{data["msg"]}')
 
-    def request(self, method: str, url: str, data: Optional[dict]=None, stream=False, check=True) -> requests.Response:
+    def request(self, method: str, url: str, data: Optional[dict]=None, stream: bool=False, check: bool=True) -> requests.Response:
         if method == 'get':
             self.response = self.session.get(url, params=data, stream=stream)
         else:
             self.session.headers['Content-Length'] = str(len(data))
             self.response = self.session.request(method, url, data=json.dumps(data), stream=stream)
 
         if not stream and check:
             self.checkJson(self.response.text)
         return self.response
 
-    def get(self, url: str, data: Optional[dict]=None, stream=False, check=True) -> requests.Response:
-        return self.request('get', url, data, stream=stream, check=check)
-
-    def post(self, url: str, data: dict, stream=False, check=True) -> requests.Response:
+    def post(self, url: str, data: dict, stream: bool=False, check: bool=True) -> requests.Response:
         return self.request('post', url, data, stream=stream, check=check)
 
-    def delete(self, url: str, data: dict, stream=False, check=True) -> requests.Response:
-        return self.request('delete', url, data, stream=stream, check=check)
-    
-    def getConversation(self) -> dict:
-        topData = self.post(
+    def getSession(self) -> model.Session:
+        top = self.post(
             'https://yiyan.baidu.com/eb/session/top/list',
             {
                 'deviceType': 'pc',
-                'timestamp': auxiliary.getTimestamp()
+                'timestamp': auxiliary.getTimestamp(ms=True)
             }
         ).json()
-        normalData = self.post(
-            f'https://yiyan.baidu.com/eb/session/list',
+        normal = self.post(
+            'https://yiyan.baidu.com/eb/session/list',
             {
                 'deviceType': 'pc',
                 'pageSize': 1000,
-                'timestamp': auxiliary.getTimestamp()
+                'timestamp': auxiliary.getTimestamp(ms=True)
             }
         ).json()
-        topSession = topData['data']['sessions']
-        normalSession = normalData['data']['sessions'] or []
+        originalTops = top['data']['sessions']
+        originalNormals = normal['data']['sessions'] or []
 
-        tops = []
-        normals = []
-        for session in topSession + normalSession:
-            conversation = {
-                'sessionId': session['sessionId'],
-                'name': session['sessionName'],
-                'state': session['state'],
-                'creationTimestamp': auxiliary.timeToTimestamp(session['createTime']),
-            }
-            if session in topSession:
-                tops.append(conversation)
+        resultTops = []
+        resultNormals = []
+        for session in originalTops + originalNormals:
+            conversation = model.SessionBase(sessionId=session['sessionId'], name=session['sessionName'], botModel=session['model'], creationTimestamp=auxiliary.timeToTimestamp(session['createTime']))
+            if session in originalTops:
+                resultTops.append(conversation)
             else:
-                normals.append(conversation)
-        return {
-            'top': tops,
-            'normal': normals
-        }
+                resultNormals.append(conversation)
+        return model.Session(tops=resultTops, normals=resultNormals)
 
-    def newConversation(self, name: str) -> str:
-        data = self.post(
-            'https://yiyan.baidu.com/eb/session/new',
-            {
-                'deviceType': 'pc',
-                'plugins': [],
-                'sessionName': name,
-                'timestamp': auxiliary.getTimestamp()
-            }
-        ).json()
-        return data['data']['sessionId']
-
-    def renameConversation(self, sessionId: str, name: str) -> bool:
+    def renameSession(self, sessionId: str, name: str) -> bool:
         self.post(
             'https://yiyan.baidu.com/eb/session/new',
             {
                 'deviceType': 'pc',
                 'sessionId': sessionId,
                 'sessionName': name,
-                'timestamp': auxiliary.getTimestamp()
+                'timestamp': auxiliary.getTimestamp(ms=True)
             }
         )
         return True
 
-    def deleteConversation(self, sessionId: str) -> bool:
+    def deleteSession(self, sessionId: str) -> bool:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/delete',
             {
                 'deviceType': 'pc',
                 'sessionId': sessionId,
-                'timestamp': auxiliary.getTimestamp()
+                'timestamp': auxiliary.getTimestamp(ms=True)
             },
             check=False
         ).json()
         return data['code'] == 0
 
-    def deleteConversations(self, sessionIds: list) -> bool:
+    def deleteSessions(self, sessionIds: list) -> bool:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/delete',
             {
                 'deviceType': 'pc',
                 'sessionIds': sessionIds,
-                'timestamp': auxiliary.getTimestamp()
+                'timestamp': auxiliary.getTimestamp(ms=True)
             },
             check=False
         ).json()
         return data['code'] == 0
 
-    def topConversation(self, sessionId: str) -> bool:
+    def topSession(self, sessionId: str) -> bool:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/top/move',
             {
                 'deviceType': 'pc',
                 'sessionId': sessionId,
-                'timestamp': auxiliary.getTimestamp()
+                'timestamp': auxiliary.getTimestamp(ms=True)
             },
             check=False
         ).json()
         return data['code'] == 0
 
-    def cancelTopConversation(self, sessionId: str) -> bool:
+    def cancelTopSession(self, sessionId: str) -> bool:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/top/cancel',
             {
                 'deviceType': 'pc',
                 'sessionId': sessionId,
-                'timestamp': auxiliary.getTimestamp()
+                'timestamp': auxiliary.getTimestamp(ms=True)
             },
             check=False
         ).json()
         return data['code'] == 0
 
-    def getConversationDetail(self, sessionId: str) -> Optional[dict]:
-        conversationG = self.getConversation()
-        conversations = conversationG['top'] + conversationG['normal']
-        if not conversations:
+    def getSessionDetail(self, sessionId: str) -> Optional[model.SessionDetail]:
+        session = self.getSession()
+        sessions = session.tops + session.normals
+        if not sessions:
             return None
-        base = {}
-        for conversation in conversations:
-            if conversation['sessionId'] == sessionId:
-                base = conversation
+        base = None
+        for sessionS in sessions:
+            if sessionS.sessionId == sessionId:
+                base = model.SessionDetailBase(name=sessionS.name, botModel=sessionS.botModel, creationTimestamp=sessionS.creationTimestamp)
                 break
         if not base:
             return None
-        del base['sessionId']
 
-        data = self.post(
+        history = self.post(
             'https://yiyan.baidu.com/eb/chat/history',
             {
                 'deviceType': 'pc',
                 'pageSize': 2000,
                 'sessionId': sessionId,
-                'timestamp': auxiliary.getTimestamp(),
+                'timestamp': auxiliary.getTimestamp(ms=True)
             }
         ).json()
-        chats = data['data']['chats']
+        chats = history['data']['chats']
         histories = []
         chats = sorted(chats.values(), key=lambda data: data['createTime'])
         for chat in chats:
-            histories.append({
-                'chatId': chat['id'],
-                'role': chat['role'],
-                'text': chat['message'][0]['content'],
-                'creationTimestamp': auxiliary.timeToTimestamp(chat['createTime'])
-            })
-        currentChatId = data['data']['currentChatId']
-        return {
-            'base': base,
-            'histories': histories,
-            'currentChatId': str(currentChatId) if currentChatId else '0'
-        }
-
-    def getShareConversation(self) -> list:
-        data = self.get('https://yiyan.baidu.com/eb/share/list').json()
-        conversations = []
-        for conversation in data['data']:
-            conversations.append({
-                'shareId': str(conversation['id']),
-                'sessionId': str(conversation['sessionId']),
-                'chatIds': conversation['chatIds'].split(','),
-                'key': conversation['shareKey'],
-                'creationTimestamp': auxiliary.timeToTimestamp(data['createTime']),
-                'userId': conversation['userId']
-            })
-        return conversations
-
-    def deleteShareConversation(self, shareId: str) -> bool:
-        data = self.delete(
-            f'https://yiyan.baidu.com/eb/share/{shareId}',
-            {}
-        ).json()
-        return data['code'] == 1
-
-    def deleteAllShareConversation(self, userId: str) -> bool:
-        data = self.delete(
-            'https://yiyan.baidu.com/eb/share/all',
-            {
-                'userId': userId
-            }
-        ).json()
-        return data['code'] == 1
+            histories.append(model.SessionDetailHistory(chatId=chat['id'], role=chat['role'], text=chat['message'][0]['content'], creationTimestamp=auxiliary.timeToTimestamp(chat['createTime'])))
+        currentChatId = history['data']['currentChatId']
+        return model.SessionDetail(base=base, histories=histories, currentChatId=str(currentChatId))
 
-    def shareConversation(self, sessionId: str, chatIds: list) -> str:
-        data = self.post(
-            'https://yiyan.baidu.com/eb/share/key/gen',
-            {
-                'botChatId': chatIds,
-                'deviceType': 'pc',
-                'sessionId': sessionId,
-                'timestamp': auxiliary.getTimestamp()
-            }
-        ).json()
-        return data['data']['key']
-
-    def askStream(self, question: str, sessionId: str='', sessionName: str='', parentChatId: str='0') -> Generator:
+    def askStream(self, question: str, sessionId: str='', sessionName: str='', parentChatId: str='0', botModel: model.BotModel=model.BotModel.EB3_5) -> Generator[model.AskStreamResponse, None, None]:
         acsToken = self.getAcsToken()
-        self.session.headers['Acs-Token'] = acsToken
         self.session.headers['Accept'] = 'text/event-stream, application/json'
-        data = self.post(
+        self.session.headers['Acs-Token'] = acsToken
+        response = self.post(
             'https://yiyan.baidu.com/eb/chat/conversation/v2',
             {
                 'code': 0,
                 'deviceType': 'pc',
+                'file_ids': [],
                 'jt': '',
-                'model': 'EB35',
+                'model': botModel.value,
                 'msg': '',
                 'newAppSessionId': '',
-                'parentChatId': parentChatId,
+                'parentChatId': parentChatId,  # 官方上新会话时为数字0(但为了方便统一,初始为字符串0),之后官方是字符串
                 'pluginInfo': [],
                 'plugins': [],
                 'sessionId': sessionId,
-                'sessionName': sessionName,
+                'sessionName': sessionName or question,
                 'sign': acsToken,
                 'text': question,
-                'timestamp': auxiliary.getTimestamp(),
+                'timestamp': auxiliary.getTimestamp(ms=True),
                 'type': 10
             },
             stream=True,
             check=False
         )
 
+        if 'application/json' in response.headers.get('Content-Type'):
+            self.checkJson(response.text)
+
         imageUrlPattern = r'<img[^>]*\ssrc=[\'"]([^\'"]+)[\'"][^>]*\s/>'
-        for line in data.iter_lines():
+        for line in response.iter_lines(decode_unicode=True):
             if not line:
                 continue
 
-            line = line.decode('utf-8')
             if line.startswith('event:'):
                 event = line[6:]
                 continue
-            elif not line.startswith('data:'):
-                self.checkJson(line)
-
-            data = line[5:]
-            data = json.loads(data)
-            if 'task_id' in data:
+            elif event == 'state':
                 continue
+            elif line.startswith('data:'):
+                data = line[5:]
+                self.checkJson(data)
+                data = json.loads(data)
 
             dataD = data['data']
             if event == 'major':
                 sessionId = dataD['createSessionResponseVoCommonResult']['data']['sessionId']
                 botChatId = dataD['createChatResponseVoCommonResult']['data']['botChat']['id']
             elif event == 'message':
                 done = dataD['is_end']
                 if done == 0:
                     answer = dataD['content']
                     urls = re.findall(imageUrlPattern, answer)
                     answer = re.sub(imageUrlPattern, '', answer)
                     answer = answer.replace('<br>', '\n')
-                    yield {
-                        'answer': answer,
-                        'urls': urls,
-                        'sessionId': sessionId,
-                        'botChatId': botChatId,
-                        'done': False
-                    }
+                    yield model.AskStreamResponse(answer=answer, urls=urls, sessionId=sessionId, botChatId=botChatId, done=False)
                 else:
                     answer = dataD['tokens_all']
                     urls = re.findall(imageUrlPattern, answer)
                     answer = re.sub(imageUrlPattern, '', answer)
                     answer = answer.replace('<br>', '\n')
                     answer = answer.strip()
-                    yield {
-                        'answer': answer,
-                        'urls': urls,
-                        'sessionId': sessionId,
-                        'botChatId': botChatId,
-                        'done': True
-                    }
-
-    def ask(self, question: str, sessionId: str='', sessionName: str='', parentChatId: str='0') -> dict:
-        data = list(self.askStream(question, sessionId, sessionName, parentChatId))
-        result = data[-1]
-        del result['done']
-        return result
+                    yield model.AskStreamResponse(answer=answer, urls=urls, sessionId=sessionId, botChatId=botChatId, done=True)
+
+    def ask(self, question: str, sessionId: str='', sessionName: str='', parentChatId: str='0', botModel: model.BotModel=model.BotModel.EB3_5) -> model.AskResponse:
+        data = list(self.askStream(question, sessionId=sessionId, sessionName=sessionName, parentChatId=parentChatId, botModel=botModel))
+        doneData = data[-1]
+        return model.AskResponse(answer=doneData.answer, urls=doneData.urls, sessionId=doneData.sessionId, botChatId=doneData.botChatId)
```


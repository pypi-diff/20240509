# Comparing `tmp/trio_bybit-0.2.0.tar.gz` & `tmp/trio_bybit-0.2.1.tar.gz`

## Comparing `trio_bybit-0.2.0.tar` & `trio_bybit-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/keypair.pem
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/pkcs8.key
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/pytest.ini
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/tests/test_async_client.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/tests/test_rsa.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/tests/test_streams.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/__init__.py
--rw-r--r--   0        0        0     8421 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/client.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/enums.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/exceptions.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/helpers.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/trio_bybit/streams.py
--rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/LICENSE
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/README.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 trio_bybit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/keypair.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/pkcs8.key
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/pytest.ini
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/tests/test_async_client.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/tests/test_rsa.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/tests/test_streams.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/trio_bybit/__init__.py
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/trio_bybit/client.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/trio_bybit/enums.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/trio_bybit/exceptions.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/trio_bybit/helpers.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/trio_bybit/streams.py
+-rw-r--r--   0        0        0    11828 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/LICENSE
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/README.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 trio_bybit-0.2.1/PKG-INFO
```

### Comparing `trio_bybit-0.2.0/keypair.pem` & `trio_bybit-0.2.1/keypair.pem`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/pkcs8.key` & `trio_bybit-0.2.1/pkcs8.key`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/test.py` & `trio_bybit-0.2.1/test.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/tests/test_async_client.py` & `trio_bybit-0.2.1/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/tests/test_rsa.py` & `trio_bybit-0.2.1/tests/test_rsa.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,17 @@
 # Generate key pair by 3 steps: generate pairs file, extract pub key and private key
 # openssl genrsa -out keypair.pem 2048
 # openssl rsa -in keypair.pem -pubout -out publickey.crt
 # openssl pkcs8 -topk8 -inform PEM -outform PEM -nocrypt -in keypair.pem -out pkcs8.key
 
 
 async def test_get_wallet():
-    with open(os.getenv("BYBIT_PRIVATE_KEY_PATH"), "r") as f:
-        private_key = f.read()
-
     client = await AsyncClient.create(
         api_key=os.getenv("BYBIT_API_KEY"),
-        api_secret=private_key,
+        api_secret=os.getenv("BYBIT_PRIVATE_KEY_PATH"),
         sign_style="RSA",
     )
 
     async with client:
         wallet = await client.get_wallet_balance(accountType="UNIFIED")
         assert wallet["retCode"] == 0
         assert wallet["retMsg"] == "OK"
```

### Comparing `trio_bybit-0.2.0/tests/test_streams.py` & `trio_bybit-0.2.1/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/trio_bybit/client.py` & `trio_bybit-0.2.1/trio_bybit/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import os
 
 import httpx
 import hashlib
 import time
 
 import orjson
-from Crypto.Hash import SHA256
-from Crypto.Signature import PKCS1_v1_5
-from Crypto.PublicKey import RSA
+from cryptography.hazmat.primitives import hashes
+from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
+from cryptography.hazmat.primitives.serialization import load_pem_private_key
 
 from .exceptions import BybitAPIException, BybitRequestException
 
 
 class BaseClient:
     API_URL = "https://api.bybit.com/"
     # SECONDARY_API_URL = "https://api.bytick.com/"
@@ -36,14 +37,21 @@
         :param api_secret: Api Secret
         :param receive_window: Receive Window
         :param sign_style: Sign Style. Default HMAC. Choices: ["HMAC", "RSA"]
         :param alternative_net: Alternative network. Default empty to use mainnet. Choices: "test", "demo"
         """
         self.API_KEY = api_key
         self.API_SECRET = api_secret
+        self.API_SECRET: RSAPrivateKey | str
+        self.sign_style = sign_style
+        if self.sign_style != "HMAC":
+            with open(api_secret, "rb") as f:
+                self.API_SECRET = load_pem_private_key(f.read(), password=None)
+        else:
+            self.API_SECRET = api_secret
         self.response = None
         self.receive_window = receive_window
         if sign_style != "HMAC" and sign_style != "RSA":
             raise ValueError("Invalid sign style. Must be HMAC or RSA")
         self.sign_style = sign_style
         self.timestamp_offset = 0
         if alternative_net == "test":
@@ -74,17 +82,15 @@
             prepared_str = (
                 str(timestamp_milli) + self.API_KEY + str(self.receive_window) + request.content.decode("utf-8")
             )
         prepared_bytes = prepared_str.encode("utf-8")
         if self.sign_style == "HMAC":
             return hmac.new(self.API_SECRET.encode("utf-8"), prepared_bytes, hashlib.sha256).hexdigest()
         else:  # RSA
-            encoded_param = SHA256.new(prepared_bytes)
-            signature = PKCS1_v1_5.new(RSA.importKey(self.API_SECRET)).sign(encoded_param)
-
+            signature = self.API_SECRET.sign(prepared_bytes, padding.PKCS1v15(), hashes.SHA256())
             return base64.b64encode(signature).decode()
 
     def _get_request(self, method, uri, signed: bool, **kwargs) -> httpx.Request:
         timestamp = int(time.time() * 1000 + self.timestamp_offset)
         headers = self._get_headers(timestamp, signed)
         if method.lower() == "get":
             req = self.session.build_request(method, uri, headers=headers, params=kwargs)
```

### Comparing `trio_bybit-0.2.0/trio_bybit/exceptions.py` & `trio_bybit-0.2.1/trio_bybit/exceptions.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/trio_bybit/helpers.py` & `trio_bybit-0.2.1/trio_bybit/helpers.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/trio_bybit/streams.py` & `trio_bybit-0.2.1/trio_bybit/streams.py`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/.gitignore` & `trio_bybit-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/LICENSE` & `trio_bybit-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/README.md` & `trio_bybit-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `trio_bybit-0.2.0/pyproject.toml` & `trio_bybit-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "trio-bybit"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python bybit async SDK based on trio."
 authors = [
     { name = "Shu Wang", email = "halfelf.ronin@gmail.com" }
 ]
 dependencies = [
     "trio>=0.25.0",
     "httpx[http2]>=0.27.0",
     "orjson>=3.10.0",
     "dateparser>=1.2.0",
     "pytz>=2024.1",
     "trio-websocket>=0.11.1",
-    "pycryptodome>=3.20.0",
+    "cryptography>=42.0.7",
 ]
 readme = "README.md"
 requires-python = ">= 3.12"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Libraries",
```

### Comparing `trio_bybit-0.2.0/PKG-INFO` & `trio_bybit-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: trio-bybit
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python bybit async SDK based on trio.
 Project-URL: Repository, https://github.com/halfelf/trio-bybit
 Author-email: Shu Wang <halfelf.ronin@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Shu Wang <halfelf.ronin@gmail.com>
         
@@ -29,18 +29,18 @@
 Keywords: bybit,crypto
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.12
+Requires-Dist: cryptography>=42.0.7
 Requires-Dist: dateparser>=1.2.0
 Requires-Dist: httpx[http2]>=0.27.0
 Requires-Dist: orjson>=3.10.0
-Requires-Dist: pycryptodome>=3.20.0
 Requires-Dist: pytz>=2024.1
 Requires-Dist: trio-websocket>=0.11.1
 Requires-Dist: trio>=0.25.0
 Description-Content-Type: text/markdown
 
 # Welcome to trio-bybit
```


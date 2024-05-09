# Comparing `tmp/prompt_defender-0.0.12.tar.gz` & `tmp/prompt_defender-0.0.28.tar.gz`

## Comparing `prompt_defender-0.0.12.tar` & `prompt_defender-0.0.28.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/.coverage
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/.coveragerc
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/example.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/requirements.txt
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/.github/workflows/deploy-prod.yml
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/.github/workflows/python-app.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/drawbridge/__init__.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/drawbridge/drawbridge.py
--rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/scripts/build.sh
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/scripts/deploy-prod.sh
--rwxr-xr-x   0        0        0      225 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/scripts/deploy.sh
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/scripts/set_version.py
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/scripts/tests.sh
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/tests/test_prompt_defender_client.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/tests/test_prompt_validator.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/tests/test_xml_scanner.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/tests/wall_test.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/wall/__init__.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/wall/example.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/wall/prompt_defender_client.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/wall/prompt_validator.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/wall/wall_builder.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/wall/wall_executor.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/wall/xml_scanner.py
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/README.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/pyproject.toml
--rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 prompt_defender-0.0.12/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.coverage
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.coveragerc
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/example.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/requirements.txt
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.github/workflows/deploy-prod.yml
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/drawbridge/__init__.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/drawbridge/drawbridge.py
+-rwxr-xr-x   0        0        0       56 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/build.sh
+-rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/deploy-prod.sh
+-rwxr-xr-x   0        0        0      225 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/deploy.sh
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/set_version.py
+-rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/scripts/tests.sh
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/test_prompt_defender_client.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/test_prompt_validator.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/test_xml_scanner.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/tests/wall_test.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/__init__.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/example.py
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/prompt_defender_client.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/prompt_defender_client_rapidapi.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/prompt_validator.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/wall_builder.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/wall_executor.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/wall/xml_scanner.py
+-rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/README.md
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/pyproject.toml
+-rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 prompt_defender-0.0.28/PKG-INFO
```

### Comparing `prompt_defender-0.0.12/.coverage` & `prompt_defender-0.0.28/.coverage`

 * *Files 15% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -26,14 +26,15 @@
 );
 INSERT INTO file VALUES(1,'/home/runner/work/PromptDefender-py/PromptDefender-py/wall/__init__.py');
 INSERT INTO file VALUES(2,'/home/runner/work/PromptDefender-py/PromptDefender-py/wall/wall_executor.py');
 INSERT INTO file VALUES(3,'/home/runner/work/PromptDefender-py/PromptDefender-py/wall/prompt_defender_client.py');
 INSERT INTO file VALUES(4,'/home/runner/work/PromptDefender-py/PromptDefender-py/wall/prompt_validator.py');
 INSERT INTO file VALUES(5,'/home/runner/work/PromptDefender-py/PromptDefender-py/wall/xml_scanner.py');
 INSERT INTO file VALUES(6,'/home/runner/work/PromptDefender-py/PromptDefender-py/wall/wall_builder.py');
+INSERT INTO file VALUES(7,'/home/runner/work/PromptDefender-py/PromptDefender-py/wall/prompt_defender_client_rapidapi.py');
 CREATE TABLE context (
     -- A row per context measured.
     id integer primary key,
     context text,
     unique (context)
 );
 INSERT INTO context VALUES(1,'');
@@ -45,18 +46,19 @@
     numbits blob,               -- see the numbits functions in coverage.numbits
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'06');
 INSERT INTO line_bits VALUES(2,1,X'eafc04bce338c1bdef07');
-INSERT INTO line_bits VALUES(3,1,X'6e7e7e7e1dff06');
+INSERT INTO line_bits VALUES(3,1,X'6ef307e59f9fff3adb9f37');
 INSERT INTO line_bits VALUES(4,1,X'e602b6');
 INSERT INTO line_bits VALUES(5,1,X'96dbb2');
-INSERT INTO line_bits VALUES(6,1,X'7afe07');
+INSERT INTO line_bits VALUES(6,1,X'fafc3f');
+INSERT INTO line_bits VALUES(7,1,X'9ef80b');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `prompt_defender-0.0.12/example.py` & `prompt_defender-0.0.28/wall/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from wall import should_block_prompt
-from wall import create_wall
+from wall_executor import should_block_prompt
+from wall_builder import create_wall
 
 wall = create_wall(
     # These options first require you to have a Prompt Defender account which you can sign up for at
     # https://defender.safetorun.com. Once you have an account you can get an API key  to use with the wall.
     remote_jailbreak_check=True,
     api_key="test_key",
     user_id="test_user",
```

### Comparing `prompt_defender-0.0.12/.github/workflows/deploy-prod.yml` & `prompt_defender-0.0.28/.github/workflows/deploy-prod.yml`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/.github/workflows/deploy.yml` & `prompt_defender-0.0.28/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/.github/workflows/python-app.yml` & `prompt_defender-0.0.28/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/drawbridge/drawbridge.py` & `prompt_defender-0.0.28/drawbridge/drawbridge.py`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/scripts/set_version.py` & `prompt_defender-0.0.28/scripts/set_version.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,11 +24,15 @@
     # Write the file out again
     with open(file_path, 'w') as file:
         file.write(file_data)
 
 
 # Replace version in the files
 try:
+    print("Going to update version in pyproject.toml")
     replace_version('pyproject.toml', latest_tag)
 except FileNotFoundError:
     print("File not found. Exiting.")
     os._exit(1)
+
+print("Version updated successfully.")
+print(open("pyproject.toml").read())
```

### Comparing `prompt_defender-0.0.12/tests/test_prompt_defender_client.py` & `prompt_defender-0.0.28/tests/test_prompt_defender_client.py`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/tests/test_prompt_validator.py` & `prompt_defender-0.0.28/tests/test_prompt_validator.py`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/tests/wall_test.py` & `prompt_defender-0.0.28/tests/wall_test.py`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/wall/example.py` & `prompt_defender-0.0.28/example.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from wall_executor import should_block_prompt
-from wall_builder import create_wall
+from wall import should_block_prompt
+from wall import create_wall
 
 wall = create_wall(
     # These options first require you to have a Prompt Defender account which you can sign up for at
     # https://defender.safetorun.com. Once you have an account you can get an API key  to use with the wall.
     remote_jailbreak_check=True,
-    api_key="test_key",
+    api_key="your_api_key_here",  # Get this from https://defender.safetorun.com
+    rapid_api_key="your_api_key_here",  # Get this from https://rapidapi.com/promptdefender-promptdefender-default/api/prompt-defender
     user_id="test_user",
     session_id="test_session",
     allow_pii=False,
 
-
     # When you create a prompt, with Prompt Defender - Keep, you will get
     # an XML tag that wraps user input. Pass this tag to the remote endpoint
     # in order to check for potential XML escaping which is likely because
     # someone is trying to attack your system
     xml_tag="tag",
 
     # The following are used for prompt validation - if you are only
@@ -30,8 +30,8 @@
 if validation_response.contains_pii:
     print("Prompt contains PII")
 elif validation_response.suspicious_user:  # etc etc etc
     print("Prompt is suspicious")
 elif should_block_prompt(validation_response):
     print("Prompt should be blocked")
 else:
-    print("Prompt is OK")
+    print("Prompt is OK")
```

### Comparing `prompt_defender-0.0.12/wall/prompt_defender_client.py` & `prompt_defender-0.0.28/wall/prompt_defender_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 import logging
 import os
-from typing import Optional
+from typing import Optional, Dict
 
 import requests
 from pydantic import BaseModel
 
+import time
+from functools import wraps
+
+
+def retry(attempts=3, delay=1):
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            for _ in range(attempts):
+                try:
+                    return func(*args, **kwargs)
+                except Exception as e:
+                    print(f"Failed to execute {func.__name__}, retrying in {delay} seconds... {e}")
+                    time.sleep(delay)
+            raise Exception(f"Failed to execute {func.__name__} after {attempts} attempts")
+
+        return wrapper
+
+    return decorator
+
 
 class WallRequest(BaseModel):
     prompt: str
     user_id: Optional[str] = None
     session_id: Optional[str] = None
     scan_pii: Optional[bool] = None
     xml_tag: Optional[str] = None
+    check_badwords: Optional[bool] = None
+    fast_check: Optional[bool] = None
 
 
 class WallResponse(BaseModel):
     potential_jailbreak: bool
     contains_pii: Optional[bool] = None
     potential_xml_escaping: Optional[bool] = None
     suspicious_user: Optional[bool] = None
@@ -24,30 +46,43 @@
 
 class PromptDefenderClient(BaseModel):
     user_id: Optional[str] = None
     session_id: Optional[str] = None
     allow_pii: Optional[bool] = None
     api_key: Optional[str] = None
     api_url: str = "https://prompt.safetorun.com/wall"
+    check_badwords: Optional[bool] = None
+    fast_check: Optional[bool] = None
+    headers: Dict[str, str] = {}
 
     def __init__(self, /, **kwargs):
 
         super().__init__(**kwargs)
         self.api_key = kwargs["api_key"] if kwargs["api_key"] is not None else os.getenv("PROMPT_DEFENDER_API_KEY")
         if not self.api_key:
             raise ValueError("API key must be provided via environment variable or parameter "
                              "(Use PROMPT_DEFENDER_API_KEY for environment variable)")
+        self.headers = {"x-api-key": self.api_key, "Content-Type": "application/json",
+                        "User-Agent": "PromptDefenderClient-v1.0"}
 
+    @retry(attempts=5, delay=2)
     def call_remote_wall(self, prompt: str) -> WallResponse:
-        headers = {"x-api-key": self.api_key, "Content-Type": "application/json",
-                   "User-Agent": "PromptDefenderClient-v1.0"}
-        request = WallRequest(prompt=prompt, user_id=self.user_id, session_id=self.session_id, scan_pii=self.allow_pii)
+
+        request = WallRequest(
+            prompt=prompt,
+            user_id=self.user_id,
+            session_id=self.session_id,
+            scan_pii=self.allow_pii,
+            check_badwords=self.check_badwords,
+            fast_check=self.fast_check
+        )
+        
         request = request.json(exclude_none=True)
         logging.info(f"Calling /wall endpoint with request: {request}")
-        response = requests.post(self.api_url, headers=headers, data=request)
+        response = requests.post(self.api_url, headers=self.headers, data=request, timeout=25)
         logging.info(f"Response from /wall endpoint: {response.status_code}, {response.text}")
 
         if response.status_code == 200:
             return WallResponse(**response.json())
         else:
             raise Exception(
                 f"Failed to call /wall endpoint: {response.status_code}, {response.text}, Request: {request}")
```

### Comparing `prompt_defender-0.0.12/wall/prompt_validator.py` & `prompt_defender-0.0.28/wall/prompt_validator.py`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/wall/wall_builder.py` & `prompt_defender-0.0.28/wall/wall_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from typing import Optional, List
 
 from .wall_executor import WallExecutor
 from .prompt_validator import PromptValidator
 from .xml_scanner import BasicXmlScanner
 from .prompt_defender_client import PromptDefenderClient
+from .prompt_defender_client_rapidapi import PromptDefenderClientRapidApi, rapid_api_check
 
 
 def create_wall(
         remote_jailbreak_check: bool = False,
         allow_pii: Optional[bool] = None,
         xml_tag: Optional[str] = None,
         api_key: Optional[str] = None,
         user_id: Optional[str] = None,
         session_id: Optional[str] = None,
         max_prompt_length: Optional[int] = None,
         allowed_prompt_values: Optional[List[str]] = None,
+        check_badwords: Optional[bool] = None,
+        fast_check: Optional[bool] = None
 ) -> WallExecutor:
     """
     Create a wall with the given configuration
 
     :param allow_pii: Whether to allow PII to be scanned
     :param xml_tag: The XML tag to scan for
     :param api_key: The API key to use for the remote wall checker
@@ -37,15 +40,18 @@
         scanner = BasicXmlScanner(xml_tag=xml_tag)
 
     if remote_jailbreak_check:
         remote_wall_checker = PromptDefenderClient(
             scan_pii=allow_pii,
             api_key=api_key,
             user_id=user_id,
-            session_id=session_id)
+            session_id=session_id,
+            check_badwords=check_badwords,
+            fast_check=fast_check
+        )
 
     if max_prompt_length is not None or allowed_prompt_values is not None:
         prompt_validator = PromptValidator(
             max_prompt_length=max_prompt_length,
             allowed_prompt_values=allowed_prompt_values)
 
     if scanner is None and remote_wall_checker is None and prompt_validator is None:
```

### Comparing `prompt_defender-0.0.12/wall/wall_executor.py` & `prompt_defender-0.0.28/wall/wall_executor.py`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/wall/xml_scanner.py` & `prompt_defender-0.0.28/wall/xml_scanner.py`

 * *Files identical despite different names*

### Comparing `prompt_defender-0.0.12/README.md` & `prompt_defender-0.0.28/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Prompt Defender
+![PyPI](https://img.shields.io/pypi/v/prompt-defender)
 
 Read the documentation at [Prompt Defender - Docs](https://promptshield.readme.io/docs)
 
 ## Installation
 
 ```pip install prompt-defender```
 
 ## Quick start
 
 ```python
-from wall.wall_executor import should_block_prompt
-from wall.wall_builder import create_wall
+from wall.wall_executor import should_block_prompt, create_wall
 
 wall = create_wall(
     # These options first require you to have a Prompt Defender account which you can sign up for at
     # https://defender.safetorun.com. Once you have an account you can get an API key  to use with the wall.
     remote_jailbreak_check=True,
     api_key="test_key",
     user_id="test_user",
@@ -122,8 +122,8 @@
 
 Next, we have a response string that we want to validate and clean. We pass this response to the
 validate_response_and_clean method of our Drawbridge instance. This method returns two values:
 
 * response_ok: This is a boolean value that indicates whether the canary was found in the response.
 * cleaned_response: This is the cleaned version of the response. If allow_unsafe_scripts is False (which is the
   default),
-  any scripts in the response will be removed.
+  any scripts in the response will be removed.
```

### Comparing `prompt_defender-0.0.12/pyproject.toml` & `prompt_defender-0.0.28/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 [project]
 name = "prompt-defender"
-version = "0.0.12"
+version = "0.0.28"
 authors = [
-    { name="Daniel Llewellyn", email="admin@safetorun.com" },
+    { name = "Daniel Llewellyn", email = "admin@safetorun.com" },
+]
+dependencies = [
+    "dataclasses-json==0.6.4",
+    "pydantic==2.6.3",
+    "pydantic_core==2.16.3",
+    "requests==2.31.0",
+    "bleach==6.1.0"
 ]
 description = "Prompt Defender. A package to help you defend against prompt injection attacks."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -19,7 +26,8 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["wall", "drawbridge"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
+
```

### Comparing `prompt_defender-0.0.12/PKG-INFO` & `prompt_defender-0.0.28/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.3
 Name: prompt-defender
-Version: 0.0.12
+Version: 0.0.28
 Summary: Prompt Defender. A package to help you defend against prompt injection attacks.
 Project-URL: Homepage, https://github.com/safetorun/PromptDefender-py
 Project-URL: Issues, https://github.com/safetorun/PromptDefender-py/issues
 Author-email: Daniel Llewellyn <admin@safetorun.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: bleach==6.1.0
+Requires-Dist: dataclasses-json==0.6.4
+Requires-Dist: pydantic-core==2.16.3
+Requires-Dist: pydantic==2.6.3
+Requires-Dist: requests==2.31.0
 Description-Content-Type: text/markdown
 
 # Prompt Defender
+![PyPI](https://img.shields.io/pypi/v/prompt-defender)
 
 Read the documentation at [Prompt Defender - Docs](https://promptshield.readme.io/docs)
 
 ## Installation
 
 ```pip install prompt-defender```
 
 ## Quick start
 
 ```python
-from wall.wall_executor import should_block_prompt
-from wall.wall_builder import create_wall
+from wall.wall_executor import should_block_prompt, create_wall
 
 wall = create_wall(
     # These options first require you to have a Prompt Defender account which you can sign up for at
     # https://defender.safetorun.com. Once you have an account you can get an API key  to use with the wall.
     remote_jailbreak_check=True,
     api_key="test_key",
     user_id="test_user",
@@ -135,8 +140,8 @@
 
 Next, we have a response string that we want to validate and clean. We pass this response to the
 validate_response_and_clean method of our Drawbridge instance. This method returns two values:
 
 * response_ok: This is a boolean value that indicates whether the canary was found in the response.
 * cleaned_response: This is the cleaned version of the response. If allow_unsafe_scripts is False (which is the
   default),
-  any scripts in the response will be removed.
+  any scripts in the response will be removed.
```


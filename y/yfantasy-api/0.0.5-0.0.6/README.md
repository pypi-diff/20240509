# Comparing `tmp/yfantasy-api-0.0.5.tar.gz` & `tmp/yfantasy-api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfantasy-api-0.0.5.tar", last modified: Sat Feb 25 22:40:32 2023, max compression
+gzip compressed data, was "yfantasy-api-0.0.6.tar", last modified: Thu May  9 03:43:50 2024, max compression
```

## Comparing `yfantasy-api-0.0.5.tar` & `yfantasy-api-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:40:32.197749 yfantasy-api-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-02-25 22:40:32.197749 yfantasy-api-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 22:40:32.197749 yfantasy-api-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:40:32.189750 yfantasy-api-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/tests/test_api_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/tests/test_auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/tests/test_game_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/tests/test_league_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/tests/test_team_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/tests/test_user_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:40:32.189750 yfantasy-api-0.0.5/yfantasy_api/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:40:32.193750 yfantasy-api-0.0.5/yfantasy_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/api/game.py
--rw-r--r--   0 runner    (1001) docker     (123)    10542 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/api/league.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/api/team.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/api/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:40:32.197749 yfantasy-api-0.0.5/yfantasy_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/models/game.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/models/league.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/models/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-25 22:40:23.000000 yfantasy-api-0.0.5/yfantasy_api/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 22:40:32.193750 yfantasy-api-0.0.5/yfantasy_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-02-25 22:40:32.000000 yfantasy-api-0.0.5/yfantasy_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-25 22:40:32.000000 yfantasy-api-0.0.5/yfantasy_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 22:40:32.000000 yfantasy-api-0.0.5/yfantasy_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-25 22:40:32.000000 yfantasy-api-0.0.5/yfantasy_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:43:50.655112 yfantasy-api-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-09 03:43:50.655112 yfantasy-api-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 03:43:50.655112 yfantasy-api-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:43:50.651112 yfantasy-api-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/tests/test_api_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/tests/test_auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/tests/test_game_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/tests/test_league_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/tests/test_team_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/tests/test_user_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:43:50.655112 yfantasy-api-0.0.6/yfantasy_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-09 03:43:42.000000 yfantasy-api-0.0.6/yfantasy_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:43:50.655112 yfantasy-api-0.0.6/yfantasy_api/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/api/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/api/league.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/api/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/api/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:43:50.655112 yfantasy-api-0.0.6/yfantasy_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/models/game.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/models/league.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/models/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 03:43:41.000000 yfantasy-api-0.0.6/yfantasy_api/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:43:50.655112 yfantasy-api-0.0.6/yfantasy_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-09 03:43:50.000000 yfantasy-api-0.0.6/yfantasy_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 03:43:50.000000 yfantasy-api-0.0.6/yfantasy_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 03:43:50.000000 yfantasy-api-0.0.6/yfantasy_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 03:43:50.000000 yfantasy-api-0.0.6/yfantasy_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 03:43:50.000000 yfantasy-api-0.0.6/yfantasy_api.egg-info/top_level.txt
```

### Comparing `yfantasy-api-0.0.5/LICENSE` & `yfantasy-api-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yfantasy-api-0.0.5/PKG-INFO` & `yfantasy-api-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfantasy-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package to access the Yahoo! Fantasy APIs
 Home-page: https://github.com/hkyplyr/yfantasy-api
 Author: Travis Paquette
 Author-email: tpaqu15@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -23,15 +23,15 @@
 pip install yfantasy_api
 ```
 
 ## Usage examples
 ### Obtain team information, including the roster with player stats for March 31st 2021
 ``` python
 # The request url created is: /team/nhl.l.12345.t.1/roster/players/stats;type=date;date=2021-03-31
-from yfantasy_api.api import YahooFantasyApi
+from yfantasy_api import YahooFantasyApi
 
 league_id = 12345  # This should be the id of the league you are querying
 game_id = 'nhl'    # This should be the id of the game you are querying
 team_id = 1        # This should be the id of the team you are querying
 
 api = YahooFantasyApi(league_id, game_id)
 team = api \
@@ -51,15 +51,15 @@
 # Jake Guentzel 0.00
 # ...truncated for brevity...
 ```
 
 ### Obtain draft_results, including player information for each pick.
 ``` python
 # The request url created is: /league/nhl.l.12345/draft_results/players
-from yfantasy_api.api import YahooFantasyApi
+from yfantasy_api import YahooFantasyApi
 
 league_id = 12345  # This should be the id of the league you are querying
 game_id = 'nhl'    # This should be the id of the game you are querying
 team_id = 1        # This should be the id of the team you are querying
 
 api = YahooFantasyApi(league_id, game_id)
 league = api \
```

### Comparing `yfantasy-api-0.0.5/README.md` & `yfantasy-api-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pip install yfantasy_api
 ```
 
 ## Usage examples
 ### Obtain team information, including the roster with player stats for March 31st 2021
 ``` python
 # The request url created is: /team/nhl.l.12345.t.1/roster/players/stats;type=date;date=2021-03-31
-from yfantasy_api.api import YahooFantasyApi
+from yfantasy_api import YahooFantasyApi
 
 league_id = 12345  # This should be the id of the league you are querying
 game_id = 'nhl'    # This should be the id of the game you are querying
 team_id = 1        # This should be the id of the team you are querying
 
 api = YahooFantasyApi(league_id, game_id)
 team = api \
@@ -38,15 +38,15 @@
 # Jake Guentzel 0.00
 # ...truncated for brevity...
 ```
 
 ### Obtain draft_results, including player information for each pick.
 ``` python
 # The request url created is: /league/nhl.l.12345/draft_results/players
-from yfantasy_api.api import YahooFantasyApi
+from yfantasy_api import YahooFantasyApi
 
 league_id = 12345  # This should be the id of the league you are querying
 game_id = 'nhl'    # This should be the id of the game you are querying
 team_id = 1        # This should be the id of the team you are querying
 
 api = YahooFantasyApi(league_id, game_id)
 league = api \
```

### Comparing `yfantasy-api-0.0.5/tests/test_api_authentication.py` & `yfantasy-api-0.0.6/tests/test_api_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,60 @@
-import requests_mock
 import time
 
+import requests_mock
 from pytest import fixture, raises
 from pytest_mock import mocker
 
-from yfantasy_api.api.api import YahooFantasyApi
+from yfantasy_api import YahooFantasyApi
 from yfantasy_api.api.auth import AuthenticationService
 
 
 @fixture(autouse=True)
 def setup(mocker):
-    mocker.patch.object(AuthenticationService, '_AuthenticationService__cache_tokens').return_val = None
-    mocker.patch.object(AuthenticationService, '_AuthenticationService__set_tokens').return_val = None
-    mocker.patch.object(AuthenticationService, 'get_access_token').return_val = 'access_token'
-    mocker.patch.object(AuthenticationService, 'get_expires_by').return_val = 'expires_by'
-    mocker.patch.object(AuthenticationService, 'get_refresh_token').return_val = 'refresh_token'
-    mocker.patch.object(AuthenticationService, 'refresh_tokens').return_val = None
+    mocker.patch.object(
+        AuthenticationService, "_AuthenticationService__cache_tokens"
+    ).return_val = None
+    mocker.patch.object(
+        AuthenticationService, "_AuthenticationService__set_tokens"
+    ).return_val = None
+    mocker.patch.object(AuthenticationService, "get_access_token").return_val = (
+        "access_token"
+    )
+    mocker.patch.object(AuthenticationService, "get_expires_by").return_val = (
+        "expires_by"
+    )
+    mocker.patch.object(AuthenticationService, "get_refresh_token").return_val = (
+        "refresh_token"
+    )
+    mocker.patch.object(AuthenticationService, "refresh_tokens").return_val = None
 
 
 def get_response_stub():
-    with open('tests/resources/game/game.json') as f:
+    with open("tests/resources/game/game.json") as f:
         return f.read()
 
 
 def test_get_resource_valid_tokens(requests_mock):
-    requests_mock.get(f'{YahooFantasyApi.base_url}/game/nhl', text=get_response_stub())
+    requests_mock.get(f"{YahooFantasyApi.base_url}/game/nhl", text=get_response_stub())
     yfs, _ = make_api_call(is_valid=True)
     yfs.auth_service.refresh_tokens.assert_not_called()
 
 
 def test_get_resource_invalid_tokens(requests_mock):
-    requests_mock.get(f'{YahooFantasyApi.base_url}/game/nhl', text=get_response_stub())
+    requests_mock.get(f"{YahooFantasyApi.base_url}/game/nhl", text=get_response_stub())
     yfs, _ = make_api_call(is_valid=False)
     yfs.auth_service.refresh_tokens.assert_called_with()
 
 
 def test_response_code_not_200(requests_mock, mocker):
-    requests_mock.get(f'{YahooFantasyApi.base_url}/game/nhl', text='Error!', status_code=400)
+    requests_mock.get(
+        f"{YahooFantasyApi.base_url}/game/nhl", text="Error!", status_code=400
+    )
     with raises(SystemExit) as sys_exit_e:
         make_api_call()
     assert sys_exit_e.type == SystemExit
 
 
 def make_api_call(is_valid=True, with_metadata=False):
-    yfs = YahooFantasyApi(123456, 'nhl', timeout=0)
+    yfs = YahooFantasyApi(123456, "nhl", timeout=0)
     yfs.expires_by = time.time() + 1000 if is_valid else time.time() - 1000
     return yfs, yfs.game().get()
```

### Comparing `yfantasy-api-0.0.5/tests/test_auth_service.py` & `yfantasy-api-0.0.6/tests/test_auth_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 import json
 import time
-import requests_mock
+from unittest import mock
 
+import requests_mock
 from pytest import fixture
-from unittest import mock
 
 from yfantasy_api.api import auth
 
 
 @fixture(autouse=True)
 def setup(tmpdir):
-    auth.TOKEN_FILE = str(tmpdir.mkdir('load_tokens').join('.tokens.json'))
+    auth.TOKEN_FILE = str(tmpdir.mkdir("load_tokens").join(".tokens.json"))
 
 
 def test_load_tokens(tmpdir):
     existing_tokens = {
         "access_token": "ex_access_token",
         "refresh_token": "ex_refresh_token",
-        "expires_by": "ex_expires_by"
+        "expires_by": "ex_expires_by",
     }
-    with open(auth.TOKEN_FILE, 'w') as token_file:
+    with open(auth.TOKEN_FILE, "w") as token_file:
         json.dump(existing_tokens, token_file)
 
     auth_service = auth.AuthenticationService()
-    assert auth_service.get_access_token() == 'ex_access_token'
-    assert auth_service.get_refresh_token() == 'ex_refresh_token'
-    assert auth_service.get_expires_by() == 'ex_expires_by'
+    assert auth_service.get_access_token() == "ex_access_token"
+    assert auth_service.get_refresh_token() == "ex_refresh_token"
+    assert auth_service.get_expires_by() == "ex_expires_by"
 
 
 def test_refresh_tokens(requests_mock, tmpdir):
     initial_tokens = {
         "access_token": "access_token",
         "refresh_token": "refresh_token",
-        "expires_in": 3600
+        "expires_in": 3600,
     }
 
     refreshed_tokens = {
         "access_token": "ref_access_token",
         "refresh_token": "ref_refresh_token",
-        "expires_in": 3600
+        "expires_in": 3600,
     }
 
-    requests_mock.post(f'{auth.AUTHORIZE_URL}', text='d')
-    __builtins__['input'] = lambda _: 'code'
+    requests_mock.post(f"{auth.AUTHORIZE_URL}", text="d")
+    __builtins__["input"] = lambda _: "code"
 
-    auth.TOKEN_FILE = str(tmpdir.mkdir('refresh_tokens').join('.tokens.json'))
+    auth.TOKEN_FILE = str(tmpdir.mkdir("refresh_tokens").join(".tokens.json"))
     requests_mock.post(auth.TOKEN_URL, text=json.dumps(initial_tokens))
 
     auth_service = auth.AuthenticationService()
-    assert auth_service.get_access_token() == 'access_token'
-    assert auth_service.get_refresh_token() == 'refresh_token'
+    assert auth_service.get_access_token() == "access_token"
+    assert auth_service.get_refresh_token() == "refresh_token"
     initial_expires_by = auth_service.get_expires_by()
     assert initial_expires_by > time.time()
 
     requests_mock.post(auth.TOKEN_URL, text=json.dumps(refreshed_tokens))
     auth_service.refresh_tokens()
-    assert auth_service.get_access_token() == 'ref_access_token'
-    assert auth_service.get_refresh_token() == 'ref_refresh_token'
+    assert auth_service.get_access_token() == "ref_access_token"
+    assert auth_service.get_refresh_token() == "ref_refresh_token"
     assert auth_service.get_expires_by() > initial_expires_by
```

### Comparing `yfantasy-api-0.0.5/tests/test_game_api.py` & `yfantasy-api-0.0.6/tests/test_game_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 import requests_mock
 
-from yfantasy_api.api import YahooFantasyApi
+from yfantasy_api import YahooFantasyApi
 
 
 def mock_request(requests_mock, path, response_name):
-    with open(f'tests/resources/game/{response_name}.json') as f:
-        print(YahooFantasyApi.base_url + '/' + path)
-        requests_mock.get(f'{YahooFantasyApi.base_url}/{path}', text=f.read())
+    with open(f"tests/resources/game/{response_name}.json") as f:
+        requests_mock.get(f"{YahooFantasyApi.base_url}/{path}", text=f.read())
 
 
 def test_game_weeks(requests_mock):
-    sub_resource = 'game_weeks'
-    path = f'game/nhl/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "game_weeks"
+    path = f"game/nhl/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.game().game_weeks().get(), sub_resource)
 
 
 def test_game_old(requests_mock):
-    path = 'game/nhl'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'old')
+    path = "game/nhl"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "old")
 
-    hasattr(api.game().get(), 'game_key')
+    hasattr(api.game().get(), "game_key")
 
 
 def test_position_types(requests_mock):
-    sub_resource = 'position_types'
-    path = f'game/nhl/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "position_types"
+    path = f"game/nhl/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.game().position_types().get(), sub_resource)
 
 
 def test_roster_positions(requests_mock):
-    sub_resource = 'roster_positions'
-    path = f'game/nhl/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "roster_positions"
+    path = f"game/nhl/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.game().roster_positions().get(), sub_resource)
 
 
 def test_stat_categories(requests_mock):
-    sub_resource = 'stat_categories'
-    path = f'game/nhl/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "stat_categories"
+    path = f"game/nhl/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.game().stat_categories().get(), sub_resource)
 
 
 def test_games(requests_mock):
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    path = 'games;is_available=1;game_codes=nhl;seasons=2020'
-    mock_request(requests_mock, path, 'games')
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    path = "games;is_available=1;game_codes=nhl;seasons=2020"
+    mock_request(requests_mock, path, "games")
 
-    api.games().get(is_available=True, game_codes=['nhl'], seasons=[2020])
+    api.games().get(is_available=True, game_codes=["nhl"], seasons=[2020])
```

### Comparing `yfantasy-api-0.0.5/tests/test_league_api.py` & `yfantasy-api-0.0.6/tests/test_league_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,195 +1,199 @@
 import requests_mock
-
 from pytest import raises
-from yfantasy_api.api import YahooFantasyApi
+
+from yfantasy_api import YahooFantasyApi
 
 
 def mock_request(requests_mock, path, response_name):
-    with open(f'tests/resources/league/{response_name}.json') as f:
-        requests_mock.get(f'{YahooFantasyApi.base_url}/{path}', text=f.read())
+    with open(f"tests/resources/league/{response_name}.json") as f:
+        requests_mock.get(f"{YahooFantasyApi.base_url}/{path}", text=f.read())
 
 
 def test_draft_results(requests_mock):
-    sub_resource = 'draftresults'
-    path = f'league/nhl.l.123456/{sub_resource}/players'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "draftresults"
+    path = f"league/nhl.l.123456/{sub_resource}/players"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.league().draft_results().get(), sub_resource)
 
 
 def test_meta(requests_mock):
-    path = 'league/nhl.l.123456'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'meta')
+    path = "league/nhl.l.123456"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "meta")
 
-    hasattr(api.league().meta().get(), 'league_id')
+    hasattr(api.league().meta().get(), "league_id")
 
 
 def test_players(requests_mock):
-    sub_resource = 'players'
-    path = f'league/nhl.l.123456/{sub_resource};search=search;status=K'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "players"
+    path = f"league/nhl.l.123456/{sub_resource};search=search;status=K"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
-    hasattr(api.league().players(search='search', status='K').get(), sub_resource)
+    hasattr(api.league().players(search="search", status="K").get(), sub_resource)
+
 
 def test_players_empty(requests_mock):
-    path = f'league/nhl.l.123456/players;search=search;status=K'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    path = f"league/nhl.l.123456/players;search=search;status=K"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, "players_empty")
 
-    hasattr(api.league().players(search='search', status='K').get(), 'players')
+    hasattr(api.league().players(search="search", status="K").get(), "players")
+
 
 def test_players_with_draft_analysis(requests_mock):
-    path = 'league/nhl.l.123456/players;start=0;count=25/draft_analysis'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'players_with_draft_analysis')
+    path = "league/nhl.l.123456/players;start=0;count=25/draft_analysis"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "players_with_draft_analysis")
 
-    hasattr(api.league().players().draft_analysis().get(), 'players')
+    hasattr(api.league().players().draft_analysis().get(), "players")
 
 
 def test_players_with_ownership(requests_mock):
-    path = 'league/nhl.l.123456/players;start=0;count=25/ownership'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'players_with_ownership')
+    path = "league/nhl.l.123456/players;start=0;count=25/ownership"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "players_with_ownership")
 
-    hasattr(api.league().players().ownership().get(), 'players')
+    hasattr(api.league().players().ownership().get(), "players")
 
 
 def test_players_with_percent_owned(requests_mock):
-    path = 'league/nhl.l.123456/players;start=0;count=25/percent_owned'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'players_with_percent_owned')
+    path = "league/nhl.l.123456/players;start=0;count=25/percent_owned"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "players_with_percent_owned")
 
-    hasattr(api.league().players().percent_owned().get(), 'players')
+    hasattr(api.league().players().percent_owned().get(), "players")
 
 
 def test_players_with_stats(requests_mock):
-    path = 'league/nhl.l.123456/players;start=0;count=25/stats'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'players_with_stats')
+    path = "league/nhl.l.123456/players;start=0;count=25/stats"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "players_with_stats")
 
-    hasattr(api.league().players().stats().get(), 'players')
+    hasattr(api.league().players().stats().get(), "players")
 
 
 def test_players_with_stats_filter_date(requests_mock):
-    path = 'league/nhl.l.123456/players;start=0;count=25/stats;date=2021-03-01'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'players_with_stats')
+    path = "league/nhl.l.123456/players;start=0;count=25/stats;date=2021-03-01"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "players_with_stats")
 
-    hasattr(api.league().players().stats(date='2021-03-01').get(), 'players')
+    hasattr(api.league().players().stats(date="2021-03-01").get(), "players")
 
 
 def test_players_with_stats_filter_season(requests_mock):
-    path = 'league/nhl.l.123456/players;start=0;count=25/stats;season=2021'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'players_with_stats')
+    path = "league/nhl.l.123456/players;start=0;count=25/stats;season=2021"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "players_with_stats")
 
-    hasattr(api.league().players().stats(season=2021).get(), 'players')
+    hasattr(api.league().players().stats(season=2021).get(), "players")
 
 
 def test_players_with_stats_filter_week(requests_mock):
-    path = 'league/nhl.l.123456/players;start=0;count=25/stats;week=1'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'players_with_stats')
+    path = "league/nhl.l.123456/players;start=0;count=25/stats;week=1"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "players_with_stats")
 
-    hasattr(api.league().players().stats(week=1).get(), 'players')
+    hasattr(api.league().players().stats(week=1).get(), "players")
 
 
 def test_players_with_stats_more_than_one_coverage(requests_mock):
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
 
     with raises(Exception) as sys_exit_e:
-        api.league().players().stats(date='2021-03-01', season=2020).get()
+        api.league().players().stats(date="2021-03-01", season=2020).get()
     assert sys_exit_e.type == Exception
 
 
 def test_scoreboard(requests_mock):
-    sub_resource = 'scoreboard'
-    path = f'league/nhl.l.123456/{sub_resource};week=1'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "scoreboard"
+    path = f"league/nhl.l.123456/{sub_resource};week=1"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.league().scoreboard(week=1).get(), sub_resource)
 
 
 def test_scoreboard_nfl(requests_mock):
-    sub_resource = 'scoreboard'
-    path = f'league/nhl.l.123456/{sub_resource};week=1'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'scoreboard_nfl')
+    sub_resource = "scoreboard"
+    path = f"league/nhl.l.123456/{sub_resource};week=1"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "scoreboard_nfl")
 
     hasattr(api.league().scoreboard(week=1).get(), sub_resource)
 
 
 def test_settings(requests_mock):
-    sub_resource = 'settings'
-    path = f'league/nhl.l.123456/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "settings"
+    path = f"league/nhl.l.123456/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.league().settings().get(), sub_resource)
 
 
 def test_settings_nfl(requests_mock):
-    sub_resource = 'settings'
-    path = f'league/nhl.l.123456/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'settings_nfl')
+    sub_resource = "settings"
+    path = f"league/nhl.l.123456/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "settings_nfl")
 
     hasattr(api.league().settings().get(), sub_resource)
 
 
-
 def test_standings(requests_mock):
-    sub_resource = 'standings'
-    path = f'league/nhl.l.123456/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "standings"
+    path = f"league/nhl.l.123456/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.league().standings().get(), sub_resource)
 
 
 def test_teams(requests_mock):
-    sub_resource = 'teams'
-    path = f'league/nhl.l.123456/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "teams"
+    path = f"league/nhl.l.123456/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.league().teams().get(), sub_resource)
 
 
 def test_transactions(requests_mock):
-    sub_resource = 'transactions'
-    path = f'league/nhl.l.123456/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "transactions"
+    path = f"league/nhl.l.123456/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.league().transactions().get(), sub_resource)
 
 
 def test_transactions_empty(requests_mock):
-    sub_resource = 'transactions'
-    path = f'league/nhl.l.123456/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'transactions_empty')
+    sub_resource = "transactions"
+    path = f"league/nhl.l.123456/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "transactions_empty")
 
     hasattr(api.league().transactions().get(), sub_resource)
 
 
 def test_transactions_waiver_missing_team():
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
 
     with raises(Exception) as sys_exit_e:
-        api.league().transactions(ttype='waiver').get()
+        api.league().transactions(ttype="waiver").get()
     assert sys_exit_e.type == Exception
 
 
 def test_transactions_waiver(requests_mock):
-    sub_resource = 'transactions'
-    path = f'league/nhl.l.123456/{sub_resource};type=waiver;team_key=nhl.l.123456.t.1;count=1;start=1'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "transactions"
+    path = f"league/nhl.l.123456/{sub_resource};type=waiver;team_key=nhl.l.123456.t.1;count=1;start=1"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
-    hasattr(api.league().transactions(ttype='waiver', team_id=1, count=1, start=1).get(), sub_resource)
+    hasattr(
+        api.league().transactions(ttype="waiver", team_id=1, count=1, start=1).get(),
+        sub_resource,
+    )
```

### Comparing `yfantasy-api-0.0.5/tests/test_team_api.py` & `yfantasy-api-0.0.6/tests/test_team_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,118 +1,115 @@
 import requests_mock
-
 from pytest import raises
-from yfantasy_api.api import YahooFantasyApi
+
+from yfantasy_api import YahooFantasyApi
 
 
 def mock_request(requests_mock, path, response_name):
-    with open(f'tests/resources/team/{response_name}.json') as f:
-        requests_mock.get(f'{YahooFantasyApi.base_url}/{path}', text=f.read())
+    with open(f"tests/resources/team/{response_name}.json") as f:
+        requests_mock.get(f"{YahooFantasyApi.base_url}/{path}", text=f.read())
 
 
 def test_meta(requests_mock):
-    path = 'team/nhl.l.123456.t.1'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'meta')
+    path = "team/nhl.l.123456.t.1"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "meta")
 
-    hasattr(api.team(1).meta().get(), 'info')
+    hasattr(api.team(1).meta().get(), "info")
 
 
 def test_matchups(requests_mock):
-    sub_resource = 'matchups'
-    path = f'team/nhl.l.123456.t.1/{sub_resource};weeks=1'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "matchups"
+    path = f"team/nhl.l.123456.t.1/{sub_resource};weeks=1"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.team(1).matchups(week=1).get(), sub_resource)
 
 
 def test_roster(requests_mock):
-    sub_resource = 'roster'
-    path = f'team/nhl.l.123456.t.1/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "roster"
+    path = f"team/nhl.l.123456.t.1/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.team(1).roster().get(), sub_resource)
 
 
 def test_roster_week(requests_mock):
-    sub_resource = 'roster'
-    path = f'team/nhl.l.123456.t.1/{sub_resource};week=1'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "roster"
+    path = f"team/nhl.l.123456.t.1/{sub_resource};week=1"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.team(1).roster(week=1).get(), sub_resource)
 
 
 def test_roster_date(requests_mock):
-    sub_resource = 'roster'
-    path = f'team/nhl.l.123456.t.1/{sub_resource};date=2021-03-01'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "roster"
+    path = f"team/nhl.l.123456.t.1/{sub_resource};date=2021-03-01"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
-    hasattr(api.team(1).roster(date='2021-03-01').get(), sub_resource)
+    hasattr(api.team(1).roster(date="2021-03-01").get(), sub_resource)
 
 
 def test_roster_with_more_than_one_coverage(requests_mock):
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
 
     with raises(Exception) as sys_exit_e:
-        api.team(1).roster(date='2021-03-01', week=1).get()
+        api.team(1).roster(date="2021-03-01", week=1).get()
     assert sys_exit_e.type == Exception
 
 
 def test_standings(requests_mock):
-    sub_resource = 'standings'
-    path = f'team/nhl.l.123456.t.1/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "standings"
+    path = f"team/nhl.l.123456.t.1/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.team(1).standings().get(), sub_resource)
 
 
 def test_standings_with_divisions(requests_mock):
-    sub_resource = 'standings'
-    path = f'team/nhl.l.123456.t.1/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'standings_with_divisions')
+    sub_resource = "standings"
+    path = f"team/nhl.l.123456.t.1/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "standings_with_divisions")
 
     hasattr(api.team(1).standings().get(), sub_resource)
 
 
 def test_stats(requests_mock):
-    sub_resource = 'stats'
-    path = f'team/nhl.l.123456.t.1/{sub_resource}'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "stats"
+    path = f"team/nhl.l.123456.t.1/{sub_resource}"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.team(1).stats().get(), sub_resource)
 
 
 def test_roster_with_stats(requests_mock):
-    sub_resource = 'roster'
-    path = f'team/nhl.l.123456.t.1/{sub_resource}/players/stats'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'roster_with_stats')
+    sub_resource = "roster"
+    path = f"team/nhl.l.123456.t.1/{sub_resource}/players/stats"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "roster_with_stats")
 
-    hasattr(api.team(1).roster().stats().get(), 'roster')
+    hasattr(api.team(1).roster().stats().get(), "roster")
 
 
 def test_roster_with_stats_week(requests_mock):
-    sub_resource = 'roster'
-    path = f'team/nhl.l.123456.t.1/{sub_resource};week=1/players/stats'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'roster_with_stats')
+    sub_resource = "roster"
+    path = f"team/nhl.l.123456.t.1/{sub_resource};week=1/players/stats"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "roster_with_stats")
 
-    hasattr(api.team(1).roster(week=1).stats().get(), 'roster')
+    hasattr(api.team(1).roster(week=1).stats().get(), "roster")
 
 
 def test_roster_with_stats_date(requests_mock):
-    sub_resource = 'roster'
-    path = f'team/nhl.l.123456.t.1/{sub_resource};date=2021-03-01/players/stats'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'roster_with_stats')
-
-    hasattr(api.team(1).roster(date='2021-03-01').stats().get(), 'roster')
-
-
+    sub_resource = "roster"
+    path = f"team/nhl.l.123456.t.1/{sub_resource};date=2021-03-01/players/stats"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "roster_with_stats")
 
+    hasattr(api.team(1).roster(date="2021-03-01").stats().get(), "roster")
```

### Comparing `yfantasy-api-0.0.5/tests/test_user_api.py` & `yfantasy-api-0.0.6/tests/test_user_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import requests_mock
-
 from pytest import raises
-from yfantasy_api.api import YahooFantasyApi
+
+from yfantasy_api import YahooFantasyApi
 
 
 def mock_request(requests_mock, path, response_name):
-    with open(f'tests/resources/user/{response_name}.json') as f:
-        requests_mock.get(f'{YahooFantasyApi.base_url}/{path}', text=f.read())
+    with open(f"tests/resources/user/{response_name}.json") as f:
+        requests_mock.get(f"{YahooFantasyApi.base_url}/{path}", text=f.read())
 
 
 def test_meta(requests_mock):
-    path = 'users;user_login=1'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
-    mock_request(requests_mock, path, 'meta')
+    path = "users;user_login=1"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
+    mock_request(requests_mock, path, "meta")
 
-    hasattr(api.user().meta().get(), 'guid')
+    hasattr(api.user().meta().get(), "guid")
 
 
 def test_games(requests_mock):
-    sub_resource = 'games'
-    path = 'users;use_login=1/games'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "games"
+    path = "users;use_login=1/games"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.user().games().get(), sub_resource)
 
 
 def test_teams(requests_mock):
-    sub_resource = 'teams'
-    path = 'users;use_login=1/teams'
-    api = YahooFantasyApi(123456, 'nhl', timeout=0)
+    sub_resource = "teams"
+    path = "users;use_login=1/teams"
+    api = YahooFantasyApi(123456, "nhl", timeout=0)
     mock_request(requests_mock, path, sub_resource)
 
     hasattr(api.user().teams().get(), sub_resource)
-
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/api/api.py` & `yfantasy-api-0.0.6/yfantasy_api/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import requests
 import sys
 import time
 
+import requests
+
 from yfantasy_api.api.auth import AuthenticationService
 from yfantasy_api.api.game import GameApi, GamesApi
 from yfantasy_api.api.league import LeagueApi
 from yfantasy_api.api.team import TeamApi
 from yfantasy_api.api.user import UserApi
 
 
@@ -37,15 +38,15 @@
     expires_by: float
         The timestamp indicating when the current access_token expires
     __timout: int
         The timeout that the client should wait before sending an http
         request. Used to avoid errors caused by too many requests
     """
 
-    base_url = 'https://fantasysports.yahooapis.com/fantasy/v2'
+    base_url = "https://fantasysports.yahooapis.com/fantasy/v2"
 
     def __init__(self, league_id, game_id, timeout=1):
         self.league_id = league_id
         self.game_id = game_id
         self.auth_service = AuthenticationService()
         self.__timeout = timeout
         self.__set_tokens()
@@ -103,23 +104,23 @@
         path: str
             The path built by the api object calling this method
         """
         return self.__get_resource(path)
 
     def __get_resource(self, path):
         self.__check_tokens()
-        params = {'format': 'json'}
-        headers = {'Authorization': 'Bearer {}'.format(self.access_token)}
-        url = '{}/{}'.format(self.base_url, path)
+        params = {"format": "json"}
+        headers = {"Authorization": "Bearer {}".format(self.access_token)}
+        url = "{}/{}".format(self.base_url, path)
 
         time.sleep(self.__timeout)
 
         response = requests.get(url, params=params, headers=headers)
         if response.status_code == 200:
-            return response.json()['fantasy_content']
+            return response.json()["fantasy_content"]
         else:
             print(response.status_code, response.text)
             sys.exit()
 
     def __set_tokens(self):
         self.access_token = self.auth_service.get_access_token()
         self.refresh_token = self.auth_service.get_refresh_token()
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/api/auth.py` & `yfantasy-api-0.0.6/yfantasy_api/api/auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import os
-import requests
 import time
 
-ACCESS_TOKEN = 'access_token'
-EXPIRES_BY = 'expires_by'
-EXPIRES_IN = 'expires_in'
-REFRESH_TOKEN = 'refresh_token'
-TOKEN_FILE = '.tokens.json'
-
-AUTHORIZE_URL = 'https://api.login.yahoo.com/oauth2/request_auth'
-TOKEN_URL = 'https://api.login.yahoo.com/oauth2/get_token'
-BASE_URL = 'https://fantasysports.yahooapis.com/fantasy/v2'
+import requests
+
+ACCESS_TOKEN = "access_token"
+EXPIRES_BY = "expires_by"
+EXPIRES_IN = "expires_in"
+REFRESH_TOKEN = "refresh_token"
+TOKEN_FILE = ".tokens.json"
+
+AUTHORIZE_URL = "https://api.login.yahoo.com/oauth2/request_auth"
+TOKEN_URL = "https://api.login.yahoo.com/oauth2/get_token"
+BASE_URL = "https://fantasysports.yahooapis.com/fantasy/v2"
 
 
 class AuthenticationService:
     """Responsible for obtaining, checking, and refreshing tokens as needed
 
     This service has two main ways to authenticate a user with Yahoo.
     If the user hasn't used this library before the service obtains a new set
@@ -55,51 +56,48 @@
         """Retrieve a new access token using the refresh token.
 
         When this method is called a new request is built to obtain
         a new set of oauth tokens from Yahoo by providing the
         `__client_id`, `__client_secret`, and `__refresh_token`.
         """
         data = {
-            'client_id': self.__client_id,
-            'client_secret': self.__client_secret,
-            'redirect_uri': 'oob',
-            'refresh_token': self.__refresh_token,
-            'grant_type': 'refresh_token',
+            "client_id": self.__client_id,
+            "client_secret": self.__client_secret,
+            "redirect_uri": "oob",
+            "refresh_token": self.__refresh_token,
+            "grant_type": "refresh_token",
         }
 
         tokens = requests.post(TOKEN_URL, data=data).json()
         self.__cache_refreshed_tokens(tokens)
 
     def get_access_token(self):
-        """A simple getter for obtaining the access token.
-        """
+        """A simple getter for obtaining the access token."""
         return self.__access_token
 
     def get_refresh_token(self):
-        """A simple getter for obtaining the refresh token.
-        """
+        """A simple getter for obtaining the refresh token."""
         return self.__refresh_token
 
     def get_expires_by(self):
-        """A simple getter for obtaining the access token expiry.
-        """
+        """A simple getter for obtaining the access token expiry."""
         return self.__expires_by
 
     def __set_credentials(self):
-        self.__client_id = os.getenv('CLIENT_ID')
-        self.__client_secret = os.getenv('CLIENT_SECRET')
+        self.__client_id = os.getenv("CLIENT_ID")
+        self.__client_secret = os.getenv("CLIENT_SECRET")
 
     def __set_tokens(self):
         if os.path.exists(TOKEN_FILE):
             self.__load_tokens()
         else:
             self.__get_tokens()
 
     def __load_tokens(self):
-        with open(TOKEN_FILE, 'r') as f:
+        with open(TOKEN_FILE, "r") as f:
             loaded_tokens = json.loads(f.read())
         self.__access_token = loaded_tokens[ACCESS_TOKEN]
         self.__refresh_token = loaded_tokens[REFRESH_TOKEN]
         self.__expires_by = loaded_tokens[EXPIRES_BY]
 
     def __get_tokens(self):
         code = self.__get_auth_code()
@@ -107,49 +105,47 @@
 
         self.__access_token = requested_tokens[ACCESS_TOKEN]
         self.__refresh_token = requested_tokens[REFRESH_TOKEN]
         self.__expires_by = requested_tokens[EXPIRES_IN] + time.time()
 
     def __get_auth_code(self):
         params = {
-            'client_id': self.__client_id,
-            'client_secret': self.__client_secret,
-            'redirect_uri': 'oob',
-            'response_type': 'code',
-            'language': 'en-us',
+            "client_id": self.__client_id,
+            "client_secret": self.__client_secret,
+            "redirect_uri": "oob",
+            "response_type": "code",
+            "language": "en-us",
         }
 
-        headers = {
-            'Content-Type': 'application/json'
-        }
+        headers = {"Content-Type": "application/json"}
 
         response = requests.post(AUTHORIZE_URL, params=params, headers=headers)
         print(response.url)
 
-        return input('Enter code: ')
+        return input("Enter code: ")
 
     def __request_tokens(self, code):
         data = {
-            'client_id': self.__client_id,
-            'client_secret': self.__client_secret,
-            'redirect_uri': 'oob',
-            'code': code,
-            'grant_type': 'authorization_code',
+            "client_id": self.__client_id,
+            "client_secret": self.__client_secret,
+            "redirect_uri": "oob",
+            "code": code,
+            "grant_type": "authorization_code",
         }
 
         return requests.post(TOKEN_URL, data=data).json()
 
     def __cache_tokens(self):
         tokens = {
             ACCESS_TOKEN: self.__access_token,
             REFRESH_TOKEN: self.__refresh_token,
-            EXPIRES_BY: self.__expires_by
+            EXPIRES_BY: self.__expires_by,
         }
 
-        with open(TOKEN_FILE, 'w+') as f:
+        with open(TOKEN_FILE, "w+") as f:
             f.write(json.dumps(tokens))
 
     def __cache_refreshed_tokens(self, tokens):
         self.__access_token = tokens[ACCESS_TOKEN]
         self.__refresh_token = tokens[REFRESH_TOKEN]
         self.__expires_by = tokens[EXPIRES_IN] + time.time()
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/api/game.py` & `yfantasy-api-0.0.6/yfantasy_api/api/game.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         Parameters
         ----------
         yfantasy_api: YahooFantasyApi
             The api class responsible for checking tokens and sending
             the http request
         """
         self.__yfantasy_api = yfantasy_api
-        self.__url = 'games'
-        self.path = ''
+        self.__url = "games"
+        self.path = ""
 
     def get(self, is_available=None, game_codes=[], seasons=[]):
         """Invoke the Yahoo Fantasy API GET call to query the Game Collections
 
         The response json is transformed into a a list of Game models
 
         Parameters
@@ -45,24 +45,24 @@
                 A list of game codes (ex. 'nfl', 'nhl', 403, 386, etc)
                 used to filter the list of games
             seasons: list
                 A list of seasons (ex. 2021, 2020, etc) used to filter
                 the list of games
         """
         if is_available is not None:
-            self.path += f';is_available={int(is_available)}'
+            self.path += f";is_available={int(is_available)}"
         if game_codes:
-            game_codes = ','.join(game_codes)
-            self.path += f';game_codes={game_codes}'
+            game_codes = ",".join(game_codes)
+            self.path += f";game_codes={game_codes}"
         if seasons:
-            seasons = ','.join(map(str, seasons))
-            self.path += f';seasons={seasons}'
+            seasons = ",".join(map(str, seasons))
+            self.path += f";seasons={seasons}"
 
-        games = self.__yfantasy_api.get(f'{self.__url}{self.path}')['games']
-        return [Game(games[str(d)]['game']) for d in range(games['count'])]
+        games = self.__yfantasy_api.get(f"{self.__url}{self.path}")["games"]
+        return [Game(games[str(d)]["game"]) for d in range(games["count"])]
 
 
 class GameApi:
     """Game Resource API: An api used for querying game resources
 
     Attributes
     ----------
@@ -82,52 +82,52 @@
         Parameters
         ----------
         yfantasy_api: YahooFantasyApi
             The api class responsible for checking tokens and sending
             the http request
         """
         self.__yfantasy_api = yfantasy_api
-        self.__url = f'game/{self.__yfantasy_api.game_id}'
-        self.path = ''
+        self.__url = f"game/{self.__yfantasy_api.game_id}"
+        self.path = ""
 
     def game_weeks(self):
         """Updates the path to include the `game_weeks` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/game_weeks'
+        self.path += "/game_weeks"
         return TerminalApi(self)
 
     def position_types(self):
         """Updates the path to include the `position_types` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/position_types'
+        self.path += "/position_types"
         return TerminalApi(self)
 
     def roster_positions(self):
         """Updates the path to include the `roster_positions` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/roster_positions'
+        self.path += "/roster_positions"
         return TerminalApi(self)
 
     def stat_categories(self):
         """Updates the path to include the `stat_categories` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/stat_categories'
+        self.path += "/stat_categories"
         return TerminalApi(self)
 
     def get(self):
         """Invoke the Yahoo Fantasy API GET call to query the Game Resource
 
         The response json is transformed into a Game model
         """
-        return Game(self.__yfantasy_api.get(f'{self.__url}{self.path}')['game'])
+        return Game(self.__yfantasy_api.get(f"{self.__url}{self.path}")["game"])
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/api/league.py` & `yfantasy-api-0.0.6/yfantasy_api/api/league.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,28 +26,30 @@
         Parameters
         ----------
         yfantasy_api: YahooFantasyApi
             The api class responsible for checking tokens and sending
             the http request
         """
         self.__yfantasy_api = yfantasy_api
-        self.__league_key = f'{self.__yfantasy_api.game_id}.l.{self.__yfantasy_api.league_id}'
-        self.__url = f'league/{self.__league_key}'
-        self.path = ''
+        self.__league_key = (
+            f"{self.__yfantasy_api.game_id}.l.{self.__yfantasy_api.league_id}"
+        )
+        self.__url = f"league/{self.__league_key}"
+        self.path = ""
 
     def draft_results(self):
         """Updates the path to include the `draftresults` sub-resource
 
         The draft results will include the `players` sub-resource in the
         response automatically.
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/draftresults/players'
+        self.path += "/draftresults/players"
         return TerminalApi(self)
 
     def meta(self):
         """Leaves the path empty to make the call return meta information
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
@@ -78,21 +80,21 @@
         search: str
             A string to used to filter the list by player names. If
             a value is provided, this will add a `;search=<value>`
             filter to the path. The server accepts any string and
             performs substring matching for all player names. If a
             match isn't found the list of players will be empy.
         """
-        self.path += f'/players;start={start};count={count}'
+        self.path += f"/players;start={start};count={count}"
 
         if search:
-            self.path += f';search={search}'
+            self.path += f";search={search}"
 
         if status:
-            self.path += f';status={status}'
+            self.path += f";status={status}"
 
         return PlayersCollectionApi(self)
 
     def scoreboard(self, week=None):
         """Updates the path to include the `scoreboard` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
@@ -102,46 +104,46 @@
         ----------
         week: int
             If a value is provided this will add a `week=<value>`
             filter to the path that filters the results by week.
             If nothing is provided the server will default to the
             current week.
         """
-        self.path += '/scoreboard'
+        self.path += "/scoreboard"
 
         if week:
-            self.path += f';week={week}'
+            self.path += f";week={week}"
 
         return TerminalApi(self)
 
     def settings(self):
         """Updates the path to include the `settings` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/settings'
+        self.path += "/settings"
         return TerminalApi(self)
 
     def standings(self):
         """Updates the path to include the `standings` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/standings'
+        self.path += "/standings"
         return TerminalApi(self)
 
     def teams(self):
         """Updates the path to include the `teams` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/teams'
+        self.path += "/teams"
         return TerminalApi(self)
 
     def transactions(self, ttype=None, team_id=None, count=None, start=None):
         """Updates the path to include the `transactions` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
@@ -166,36 +168,36 @@
             a maximum value for transactions. (default: 25)
         start: int
             The value to indicate what offset to start the transactions
             list at. For example: `start=0` begins at the most recent
             transaction while `start=1` begins at the second most recent.
             (default: 0)
         """
-        self.path += '/transactions'
+        self.path += "/transactions"
 
-        if ttype in ['waiver', 'pending_trade'] and not team_id:
-            raise Exception(f'\'team_id\' must be provided when using \'{ttype}\'.')
+        if ttype in ["waiver", "pending_trade"] and not team_id:
+            raise Exception(f"'team_id' must be provided when using '{ttype}'.")
 
         if ttype:
-            self.path += f';type={ttype}'
+            self.path += f";type={ttype}"
         if team_id:
-            self.path += f';team_key={self.__league_key}.t.{team_id}'
+            self.path += f";team_key={self.__league_key}.t.{team_id}"
         if count:
-            self.path += f';count={count}'
+            self.path += f";count={count}"
         if start:
-            self.path += f';start={start}'
+            self.path += f";start={start}"
 
         return TerminalApi(self)
 
     def get(self):
         """Invoke the Yahoo Fantasy API GET call to query the League Resource
 
         The response json is transformed into a League model
         """
-        return League(self.__yfantasy_api.get(f'{self.__url}{self.path}')['league'])
+        return League(self.__yfantasy_api.get(f"{self.__url}{self.path}")["league"])
 
 
 class PlayersCollectionApi:
     """Players Collection API: Supports querying players sub-resources
 
     Attributes
     ----------
@@ -219,33 +221,33 @@
 
     def draft_analysis(self):
         """Updates the path to include the 'draft_analysis' sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.__parent_api.path += '/draft_analysis'
+        self.__parent_api.path += "/draft_analysis"
         return TerminalApi(self.__parent_api)
 
     def ownership(self):
         """Updates the path to include the 'ownership' sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.__parent_api.path += '/ownership'
+        self.__parent_api.path += "/ownership"
         return TerminalApi(self.__parent_api)
 
     def percent_owned(self):
         """Updates the path to include the 'percent_owned' sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.__parent_api.path += '/percent_owned'
+        self.__parent_api.path += "/percent_owned"
         return TerminalApi(self.__parent_api)
 
     def stats(self, date=None, season=None, week=None):
         """Updates the path to include the 'stats' sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
@@ -266,26 +268,27 @@
             filter.
         week:int
             The value to indicate the week of the players stats to return.
             If a value is provided this will add a `;type=week;week=<value>`
             filter.
         """
         coverage_filter = self.__build_coverage_filter(date, season, week)
-        self.__parent_api.path += f'/stats{coverage_filter}'
+        self.__parent_api.path += f"/stats{coverage_filter}"
         return TerminalApi(self.__parent_api)
 
     def get(self):
-        """Invoke the parent API `get()` call
-        """
+        """Invoke the parent API `get()` call"""
         return self.__parent_api.get()
 
     def __build_coverage_filter(self, date, season, week):
         if bool(date) + bool(season) + bool(week) > 1:
-            raise Exception('Only one of \'date\', \'season\', or \'week\' should be provided.')
+            raise Exception(
+                "Only one of 'date', 'season', or 'week' should be provided."
+            )
         elif date:
-            return f';type=date;date={date}'
+            return f";type=date;date={date}"
         elif season:
-            return f';type=season;season={season}'
+            return f";type=season;season={season}"
         elif week:
-            return f';type=week;week={week}'
+            return f";type=week;week={week}"
         else:
-            return ''
+            return ""
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/api/team.py` & `yfantasy-api-0.0.6/yfantasy_api/api/team.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,27 +16,28 @@
         format is <game-code>.l.<league-id>.t.<team-id>
     __url: str
         The base url for team resources
     path: str
         The path to append to the base url; can contain subresources,
         filters, or nothing depending on the builder methods called
     """
+
     def __init__(self, yfantasy_api, team_id):
         """Initialize a new Team Resource API
 
         Parameters
         ----------
         yfantasy_api: YahooFantasyApi
             The api class responsible for checking tokens and sending
             the http request
         """
         self.__yfantasy_api = yfantasy_api
-        self.__team_key = f'{self.__yfantasy_api.game_id}.l.{self.__yfantasy_api.league_id}.t.{team_id}'
-        self.__url = f'team/{self.__team_key}'
-        self.path = ''
+        self.__team_key = f"{self.__yfantasy_api.game_id}.l.{self.__yfantasy_api.league_id}.t.{team_id}"
+        self.__url = f"team/{self.__team_key}"
+        self.path = ""
 
     def meta(self):
         """Leaves the path empty to make the call return meta information
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
@@ -52,18 +53,18 @@
         ----------
         week: int
             If a value is provided this will add a `week=<value>`
             filter to the path that filters the results by week.
             If nothing is provided the server will default to the
             current week.
         """
-        self.path += '/matchups'
+        self.path += "/matchups"
 
         if week:
-            self.path += f';week={week}'
+            self.path += f";week={week}"
 
         return TerminalApi(self)
 
     def roster(self, date=None, week=None):
         """Updates the path to include the `roster` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
@@ -78,67 +79,68 @@
         week: int
             The value to indicate what week the roster data should be
             scoped. If a value is provided this will add a `week=<value>`
             filter. The server uses the first date in the week when
             returning the filtered roster.
         """
         coverage_filter = self.__build_coverage_filter(week, date)
-        self.path += f'/roster{coverage_filter}'
+        self.path += f"/roster{coverage_filter}"
         return PlayerCollectionApi(self)
 
     def standings(self):
         """Updates the path to include the `standings` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/standings'
+        self.path += "/standings"
         return TerminalApi(self)
 
     def stats(self, week=None):
         """Updates the path to include the `stats` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
 
-        self.path += '/stats'
-        
+        self.path += "/stats"
+
         if week:
-            self.path += f';type=week;week={week}' # pragma: no cover
+            self.path += f";type=week;week={week}"  # pragma: no cover
         return TerminalApi(self)
 
     def get(self):
         """Invoke the Yahoo Fantasy API GET call to query the Team Resource
 
         The response json is transformed into a Team model
         """
-        return Team(self.__yfantasy_api.get(f'{self.__url}{self.path}')['team'])
+        return Team(self.__yfantasy_api.get(f"{self.__url}{self.path}")["team"])
 
     def __build_coverage_filter(self, week, date):
         if week and date:
-            raise Exception('Only one of \'date\' or \'week\' should be provided.')
+            raise Exception("Only one of 'date' or 'week' should be provided.")
         elif week:
-            return f';week={week}'
+            return f";week={week}"
         elif date:
-            return f';date={date}'
+            return f";date={date}"
         else:
-            return ''
+            return ""
 
 
 class PlayerCollectionApi:
     """Players Collection API: Supports querying players sub-resources
 
     Attributes
     ----------
     __parent_api
         The parent api class that created this object, this parent
         api is used when invoking the query or creating the terminal
         api object.
     """
+
     def __init__(self, parent_api):
         """Initialize a new Players Collection API object
 
         Parameters
         ----------
         parent_api
             The parent api class that created this object, this parent
@@ -149,22 +151,21 @@
 
     def stats(self):
         """Updates the path to include the 'stats' sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.__parent_api.path += '/players/stats'
+        self.__parent_api.path += "/players/stats"
         return TerminalApi(self.__parent_api)
-    
+
     def percent_owned(self):
-        self.__parent_api.path += '/players/percent_owned' # pragma: no cover
-        return TerminalApi(self.__parent_api) # pragma: no cover
-    
+        self.__parent_api.path += "/players/percent_owned"  # pragma: no cover
+        return TerminalApi(self.__parent_api)  # pragma: no cover
+
     def draft_analysis(self):
-        self.__parent_api.path += '/players/draft_analysis' # pragma: no cover
-        return TerminalApi(self.__parent_api) # pragma: no cover
+        self.__parent_api.path += "/players/draft_analysis"  # pragma: no cover
+        return TerminalApi(self.__parent_api)  # pragma: no cover
 
     def get(self):
-        """Invoke the parent API `get()` call
-        """
+        """Invoke the parent API `get()` call"""
         return self.__parent_api.get()
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/api/terminal.py` & `yfantasy-api-0.0.6/yfantasy_api/api/terminal.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,10 +22,9 @@
         parent_api
             The parent api class that created this object, this parent
             api is used when invoking the query.
         """
         self.__parent_api = parent_api
 
     def get(self):
-        """Invoke the parent API `get()` call
-        """
+        """Invoke the parent API `get()` call"""
         return self.__parent_api.get()
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/api/user.py` & `yfantasy-api-0.0.6/yfantasy_api/api/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         Parameters
         ----------
         yfantasy_api: YahooFantasyApi
             The api class responsible for checking tokens and sending
             the http request
         """
         self.__yfantasy_api = yfantasy_api
-        self.__url = 'users;use_login=1'
-        self.path = ''
+        self.__url = "users;use_login=1"
+        self.path = ""
 
     def meta(self):
         """Leaves the path empty to make the call return meta information
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
@@ -45,25 +45,27 @@
 
     def games(self):
         """Updates the path to include the `games` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/games'
+        self.path += "/games"
         return TerminalApi(self)
 
     def teams(self):
         """Updates the path to include the `teams` sub-resource
 
         Returns a TerminalApi object that provides a `get()` call to
         invoke the query.
         """
-        self.path += '/teams'
+        self.path += "/teams"
         return TerminalApi(self)
 
     def get(self):
         """Invoke the Yahoo Fantasy API GET call to query the User Resource
 
         The response json is transformed into a User model
         """
-        return User(self.__yfantasy_api.get(f'{self.__url}{self.path}')['users']['0']['user'])
+        return User(
+            self.__yfantasy_api.get(f"{self.__url}{self.path}")["users"]["0"]["user"]
+        )
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/models/common.py` & `yfantasy-api-0.0.6/yfantasy_api/models/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,175 +1,183 @@
-from yfantasy_api.models.helpers import flatten_attributes, as_float, as_bool, as_int
+from yfantasy_api.models.helpers import as_bool, as_float, as_int, flatten_attributes
 
 
 class Team:
     def __init__(self, json):
         attributes = self.__flatten_attributes(json)
-        self.key = attributes.get('team_key')
-        self.id = as_int(attributes.get('team_id'))
-        self.name = attributes.get('name')
-        self.priority = as_int(attributes.get('waiver_priority'))
-        self.faab = as_int(attributes.get('faab_balance'))
-        self.moves = as_int(attributes.get('number_of_moves'))
-        self.trades = as_int(attributes.get('number_of_trades'))
-        self.draft_grade = attributes.get('draft_grade')
+        self.key = attributes.get("team_key")
+        self.id = as_int(attributes.get("team_id"))
+        self.name = attributes.get("name")
+        self.priority = as_int(attributes.get("waiver_priority"))
+        self.faab = as_int(attributes.get("faab_balance"))
+        self.moves = as_int(attributes.get("number_of_moves"))
+        self.trades = as_int(attributes.get("number_of_trades"))
+        self.draft_grade = attributes.get("draft_grade")
         self.managers = self.__parse_managers(attributes)
-        self.clinched_playoffs = as_bool(attributes.get('clinched_playoffs'))
-        self.url = attributes.get('url')
+        self.clinched_playoffs = as_bool(attributes.get("clinched_playoffs"))
+        self.url = attributes.get("url")
         self.team_logos = self.__parse_team_logo(attributes)
 
         self.__parse_sub_resources(json)
 
     def __repr__(self):
-        return str(self.__dict__) # pragma: no cover
+        return str(self.__dict__)  # pragma: no cover
 
     def __flatten_attributes(self, json):
         json = json[0] if type(json) == list else [json]
         return flatten_attributes(json)
 
     def __parse_sub_resources(self, json):
         for data in json:
-            if 'roster' in data:
+            if "roster" in data:
                 self.__parse_roster(data)
-            if 'team_standings' in data:
+            if "team_standings" in data:
                 self.__parse_team_standings(data)
-            if 'team_points' in data:
+            if "team_points" in data:
                 self.__parse_team_points(data)
-            if 'team_projected_points' in data:
+            if "team_projected_points" in data:
                 self.__parse_projected_points(data)
-            if 'team_stats' in data:
+            if "team_stats" in data:
                 self.__parse_team_stats(data)
 
     def __parse_roster(self, json):
-        json = json['roster']['0']['players']
-        self.players = [Player(json[p]['player']) for p in json if p != 'count']
+        json = json["roster"]["0"]["players"]
+        self.players = [Player(json[p]["player"]) for p in json if p != "count"]
 
     def __parse_team_standings(self, json):
-        json = json['team_standings']
-        self.rank = as_int(json['rank'])
-        self.playoff_seed = as_int(json.get('playoff_seed', 0))
-        self.wins = as_int(json['outcome_totals']['wins'])
-        self.losses = as_int(json['outcome_totals']['losses'])
-        self.ties = as_int(json['outcome_totals']['ties'])
-        self.percentage = as_float(json['outcome_totals']['percentage'])
-        self.points_for = as_float(json['points_for'])
-        self.points_against = as_float(json['points_against'])
-
-        if 'divisional_outcome_totals' in json:
-            self.div_wins = as_int(json['divisional_outcome_totals']['wins'])
-            self.div_losses = as_int(json['divisional_outcome_totals']['losses'])
-            self.div_ties = as_int(json['divisional_outcome_totals']['ties'])
-
-        if 'streak' in json:
-            self.streak_type = json['streak']['type']
-            self.streak_value = as_int(json['streak']['value'])
+        json = json["team_standings"]
+        self.rank = as_int(json["rank"])
+        self.playoff_seed = as_int(json.get("playoff_seed", 0))
+        self.wins = as_int(json["outcome_totals"]["wins"])
+        self.losses = as_int(json["outcome_totals"]["losses"])
+        self.ties = as_int(json["outcome_totals"]["ties"])
+        self.percentage = as_float(json["outcome_totals"]["percentage"])
+        self.points_for = as_float(json["points_for"])
+        self.points_against = as_float(json["points_against"])
+
+        if "divisional_outcome_totals" in json:
+            self.div_wins = as_int(json["divisional_outcome_totals"]["wins"])
+            self.div_losses = as_int(json["divisional_outcome_totals"]["losses"])
+            self.div_ties = as_int(json["divisional_outcome_totals"]["ties"])
+
+        if "streak" in json:
+            self.streak_type = json["streak"]["type"]
+            self.streak_value = as_int(json["streak"]["value"])
 
     def __parse_team_points(self, json):
-        self.points = as_float(json['team_points']['total'])
-    
+        self.points = as_float(json["team_points"]["total"])
+
     def __parse_projected_points(self, json):
-        self.projected_points = as_float(json['team_projected_points']['total'])
+        self.projected_points = as_float(json["team_projected_points"]["total"])
 
     def __parse_team_stats(self, json):
-        self.stats = {d['stat']['stat_id']: d['stat']['value'] for d in json['team_stats']['stats']}
-    
+        self.stats = {
+            d["stat"]["stat_id"]: d["stat"]["value"]
+            for d in json["team_stats"]["stats"]
+        }
+
     def __parse_team_logo(self, json):
-        json = json.get('team_logos')
+        json = json.get("team_logos")
         if not json:
             return None
-        return json[0]['team_logo']['url']
-    
+        return json[0]["team_logo"]["url"]
+
     def __parse_managers(self, json):
-        return [Manager(m) for m in json.get('managers', [])]
+        return [Manager(m) for m in json.get("managers", [])]
 
 
 class Manager:
     def __init__(self, json):
-        json = json['manager']
-        self.manager_id = as_int(json['manager_id'])
-        self.name = json['nickname']
-        self.felo_score = as_int(json.get('felo_score'))
-        self.felo_tier = json.get('felo_tier')
-        self.is_commissioner = as_bool(json.get('is_commissioner'))
-    
+        json = json["manager"]
+        self.manager_id = as_int(json["manager_id"])
+        self.name = json["nickname"]
+        self.felo_score = as_int(json.get("felo_score"))
+        self.felo_tier = json.get("felo_tier")
+        self.is_commissioner = as_bool(json.get("is_commissioner"))
+
     def __repr__(self):
-        return str(self.__dict__) # pragma: no cover
+        return str(self.__dict__)  # pragma: no cover
 
 
 class Player:
     def __init__(self, json):
         attributes = flatten_attributes(json[0])
-        self.key = attributes['player_key']
-        self.id = as_int(attributes['player_id'])
-        self.name = attributes['name']['full']
-        self.first_name = attributes['name']['first']
-        self.last_name = attributes['name']['last']
-        self.pro_team = attributes.get('editorial_team_abbr').upper()
-        self.team_name = attributes.get('editorial_team_full_name')
-        self.number = as_int(attributes.get('uniform_number'))
-        self.position = attributes.get('display_position')
-        self.is_undroppable = as_bool(attributes.get('is_undroppable'))
-        self.status = attributes.get('status')
-        self.status_full = attributes.get('status_full')
-        self.injury_note = attributes.get('injury_note')
-        self.bye_week = as_int(attributes.get('bye_weeks', {}).get('week'))
+        self.key = attributes["player_key"]
+        self.id = as_int(attributes["player_id"])
+        self.name = attributes["name"]["full"]
+        self.first_name = attributes["name"]["first"]
+        self.last_name = attributes["name"]["last"]
+        self.pro_team = attributes.get("editorial_team_abbr").upper()
+        self.team_name = attributes.get("editorial_team_full_name")
+        self.number = as_int(attributes.get("uniform_number"))
+        self.position = attributes.get("display_position")
+        self.is_undroppable = as_bool(attributes.get("is_undroppable"))
+        self.status = attributes.get("status")
+        self.status_full = attributes.get("status_full")
+        self.injury_note = attributes.get("injury_note")
+        self.bye_week = as_int(attributes.get("bye_weeks", {}).get("week"))
 
         self.eligible_positions = self.__parse_eligible_positions(attributes)
         self.image_url = self.__parse_image_url(attributes)
 
         self.__parse_sub_resources(json)
-    
+
     def __repr__(self):
-        return str(self.__dict__) # pragma: no cover
+        return str(self.__dict__)  # pragma: no cover
 
     def __parse_sub_resources(self, json):
         for data in json:
-            if 'player_stats' in data:
+            if "player_stats" in data:
                 self.__parse_stats(data)
-            if 'player_points' in data:
+            if "player_points" in data:
                 self.__parse_points(data)
-            if 'ownership' in data:
+            if "ownership" in data:
                 self.__parse_ownership(data)
-            if 'percent_owned' in data:
+            if "percent_owned" in data:
                 self.__parse_percent_owned(data)
-            if 'draft_analysis' in data:
+            if "draft_analysis" in data:
                 self.__parse_draft_analysis(data)
-            if 'selected_position' in data:
+            if "selected_position" in data:
                 self.__parse_selected_position(data)
 
     def __parse_stats(self, json):
-        json = json['player_stats']['stats']
-        self.stats = {as_int(s['stat']['stat_id']): as_int(s['stat']['value']) for s in json}
+        json = json["player_stats"]["stats"]
+        self.stats = {
+            as_int(s["stat"]["stat_id"]): as_int(s["stat"]["value"]) for s in json
+        }
 
     def __parse_points(self, json):
-        self.points = as_float(json['player_points']['total'])
+        self.points = as_float(json["player_points"]["total"])
 
     def __parse_ownership(self, json):
         # TODO
-        json = json['ownership']
-        self.team = None if json['ownership_type'] != 'team' \
-            else Team(json['0']['teams']['0']['team'])
+        json = json["ownership"]
+        self.team = (
+            None
+            if json["ownership_type"] != "team"
+            else Team(json["0"]["teams"]["0"]["team"])
+        )
 
     def __parse_percent_owned(self, json):
-        json = flatten_attributes(json['percent_owned'])
-        self.percent_owned = as_int(json.get('value'))
-        self.percent_changed = as_int(json.get('delta'))
+        json = flatten_attributes(json["percent_owned"])
+        self.percent_owned = as_int(json.get("value"))
+        self.percent_changed = as_int(json.get("delta"))
 
     def __parse_draft_analysis(self, json):
-        json = flatten_attributes(json['draft_analysis'])
-        self.average_pick = as_float(json['average_pick'])
-        self.average_round = as_float(json['average_round'])
-        self.average_cost = as_float(json['average_cost'])
-        self.percent_drafted = as_float(json['percent_drafted'])
+        json = flatten_attributes(json["draft_analysis"])
+        self.average_pick = as_float(json["average_pick"])
+        self.average_round = as_float(json["average_round"])
+        self.average_cost = as_float(json["average_cost"])
+        self.percent_drafted = as_float(json["percent_drafted"])
 
     def __parse_selected_position(self, json):
-        json = flatten_attributes(json['selected_position'])
-        self.selected_position = json['position']
-        self.is_flex = as_bool(json['is_flex'])
-    
+        json = flatten_attributes(json["selected_position"])
+        self.selected_position = json["position"]
+        self.is_flex = as_bool(json["is_flex"])
+
     def __parse_eligible_positions(self, json):
-        return [ep['position'] for ep in json.get('eligible_positions', [])]
-    
+        return [ep["position"] for ep in json.get("eligible_positions", [])]
+
     def __parse_image_url(self, json):
-        image_url = json.get('image_url', '')
-        start = image_url.find('/https') + 1
+        image_url = json.get("image_url", "")
+        start = image_url.find("/https") + 1
         return image_url[start:]
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/models/game.py` & `yfantasy-api-0.0.6/yfantasy_api/models/game.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,76 +8,82 @@
         if type(json) == list:
             return GameInfo(json[0])
         else:
             return GameInfo(json)
 
     def __parse_sub_resources(self, json):
         for data in json:
-            if 'game_weeks' in data:
-                self.__parse_game_weeks(data['game_weeks'])
-            if 'position_types' in data:
-                self.__parse_position_types(data['position_types'])
-            if 'roster_positions' in data:
-                self.__parse_roster_positions(data['roster_positions'])
-            if 'stat_categories' in data:
-                self.__parse_stat_categories(data['stat_categories'])
+            if "game_weeks" in data:
+                self.__parse_game_weeks(data["game_weeks"])
+            if "position_types" in data:
+                self.__parse_position_types(data["position_types"])
+            if "roster_positions" in data:
+                self.__parse_roster_positions(data["roster_positions"])
+            if "stat_categories" in data:
+                self.__parse_stat_categories(data["stat_categories"])
 
     def __parse_game_weeks(self, json):
-        self.game_weeks = [GameWeek(json[str(d)]['game_week']) for d in range(json['count'])]
+        self.game_weeks = [
+            GameWeek(json[str(d)]["game_week"]) for d in range(json["count"])
+        ]
 
     def __parse_position_types(self, json):
-        self.position_types = [PositionType(d['position_type']) for d in json]
+        self.position_types = [PositionType(d["position_type"]) for d in json]
 
     def __parse_roster_positions(self, json):
-        self.roster_positions = [RosterPosition(d['roster_position']) for d in json]
+        self.roster_positions = [RosterPosition(d["roster_position"]) for d in json]
 
     def __parse_stat_categories(self, json):
-        self.stat_categories = [StatCategory(d['stat']) for d in json['stats']]
+        self.stat_categories = [StatCategory(d["stat"]) for d in json["stats"]]
 
 
 class GameInfo:
     def __init__(self, json):
-        self.game_key = json['game_key']
-        self.game_id = json['game_id']
-        self.name = json['name']
-        self.code = json['code']
-        self.type = json['type']
-        self.url = json['url']
-        self.season = json['season']
-        self.is_registration_over = json['is_registration_over']
-        self.is_game_over = json['is_game_over']
-        self.is_offseason = json['is_offseason']
+        self.game_key = json["game_key"]
+        self.game_id = json["game_id"]
+        self.name = json["name"]
+        self.code = json["code"]
+        self.type = json["type"]
+        self.url = json["url"]
+        self.season = json["season"]
+        self.is_registration_over = json["is_registration_over"]
+        self.is_game_over = json["is_game_over"]
+        self.is_offseason = json["is_offseason"]
 
 
 class GameWeek:
     def __init__(self, json):
-        self.week = json['week']
-        self.display_name = json['display_name']
-        self.start = json['start']
-        self.end = json['end']
+        self.week = json["week"]
+        self.display_name = json["display_name"]
+        self.start = json["start"]
+        self.end = json["end"]
 
 
 class PositionType:
     def __init__(self, json):
-        self.type = json['type']
-        self.display_name = json['display_name']
+        self.type = json["type"]
+        self.display_name = json["display_name"]
 
 
 class RosterPosition:
     def __init__(self, json):
-        self.position = json['position']
-        self.abbreviation = json['abbreviation']
-        self.display_name = json['display_name']
-        self.position_type = json.get('position_type')
-        self.is_bench = json.get('is_bench')
-        self.is_disabled_list = json.get('is_disabled_list')
+        self.position = json["position"]
+        self.abbreviation = json["abbreviation"]
+        self.display_name = json["display_name"]
+        self.position_type = json.get("position_type")
+        self.is_bench = json.get("is_bench")
+        self.is_disabled_list = json.get("is_disabled_list")
 
 
 class StatCategory:
     def __init__(self, json):
-        self.stat_id = json['stat_id']
-        self.name = json['name']
-        self.display_name = json['display_name']
-        self.sort_order = json['sort_order']
-        self.position_types = [d['position_type'] for d in json.get('position_types', [])]
-        self.is_composite_stat = json.get('is_composite_stat')
-        self.base_stats = [d['base_stat']['stat_id'] for d in json.get('base_stats', [])]
+        self.stat_id = json["stat_id"]
+        self.name = json["name"]
+        self.display_name = json["display_name"]
+        self.sort_order = json["sort_order"]
+        self.position_types = [
+            d["position_type"] for d in json.get("position_types", [])
+        ]
+        self.is_composite_stat = json.get("is_composite_stat")
+        self.base_stats = [
+            d["base_stat"]["stat_id"] for d in json.get("base_stats", [])
+        ]
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/models/helpers.py` & `yfantasy-api-0.0.6/yfantasy_api/models/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,22 +2,27 @@
     attributes = {}
     for d in json:
         if type(d) == list and len(d) == 0:
             continue
         attributes.update(d)
     return attributes
 
-EMPTY_VALUES = [None, '-', '']
+
+EMPTY_VALUES = [None, "-", ""]
+
+
 def as_float(value):
     if value in EMPTY_VALUES:
         return None
     return float(value)
 
+
 def as_int(value):
     if value in EMPTY_VALUES:
         return None
     return int(value)
 
+
 def as_bool(value):
     if value in EMPTY_VALUES:
         return False
-    return True if as_int(value) else False
+    return True if as_int(value) else False
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/models/league.py` & `yfantasy-api-0.0.6/yfantasy_api/models/league.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,202 +1,213 @@
 from yfantasy_api.models.common import Player, Team
-from yfantasy_api.models.helpers import flatten_attributes, as_float, as_bool, as_int
+from yfantasy_api.models.helpers import as_bool, as_float, as_int, flatten_attributes
 from yfantasy_api.models.transaction import Add, AddDrop, Drop, Trade
 
 
 class League:
     def __init__(self, json):
         attributes = flatten_attributes(json)
-        self.key = attributes.get('league_key')
-        self.id = as_int(attributes.get('league_id'))
-        self.name = attributes.get('name')
-        self.url = attributes.get('url')
-        self.logo_url = attributes.get('logo_url')
-        self.draft_status = attributes.get('draft_status')
-        self.num_teams = as_int(attributes.get('num_teams'))
-        self.scoring_type = attributes.get('scoring_type')
-        self.league_type = attributes.get('league_type')
-        self.add_injured_to_ir = as_bool(attributes.get('allow_add_to_dl_extra_pos'))
-        self.current_week = as_int(attributes.get('current_week'))
-        self.start_week = as_int(attributes.get('start_week'))
-        self.start_date = attributes.get('start_date')
-        self.end_week = as_int(attributes.get('end_week'))
-        self.end_date = attributes.get('end_date')
-        self.game_code = attributes.get('game_code')
-        self.season = as_int(attributes.get('season'))
+        self.key = attributes.get("league_key")
+        self.id = as_int(attributes.get("league_id"))
+        self.name = attributes.get("name")
+        self.url = attributes.get("url")
+        self.logo_url = attributes.get("logo_url")
+        self.draft_status = attributes.get("draft_status")
+        self.num_teams = as_int(attributes.get("num_teams"))
+        self.scoring_type = attributes.get("scoring_type")
+        self.league_type = attributes.get("league_type")
+        self.add_injured_to_ir = as_bool(attributes.get("allow_add_to_dl_extra_pos"))
+        self.current_week = as_int(attributes.get("current_week"))
+        self.start_week = as_int(attributes.get("start_week"))
+        self.start_date = attributes.get("start_date")
+        self.end_week = as_int(attributes.get("end_week"))
+        self.end_date = attributes.get("end_date")
+        self.game_code = attributes.get("game_code")
+        self.season = as_int(attributes.get("season"))
         self.__parse_sub_resources(json)
-    
+
     def __repr__(self):
-        return str(self.__dict__) # pragma: no cover
+        return str(self.__dict__)  # pragma: no cover
 
     def __parse_sub_resources(self, json):
         for data in json:
-            if 'draft_results' in data:
-                self.__parse_draft_results(data['draft_results'])
-            if 'players' in data:
-                self.__parse_players(data['players'])
-            if 'scoreboard' in data:
-                self.__parse_scoreboard(data['scoreboard'])
-            if 'settings' in data:
-                self.__parse_settings(data['settings'])
-            if 'standings' in data:
-                self.__parse_standings(data['standings'])
-            if 'teams' in data:
-                self.__parse_teams(data['teams'])
-            if 'transactions' in data:
-                self.__parse_transactions(data['transactions'])
+            if "draft_results" in data:
+                self.__parse_draft_results(data["draft_results"])
+            if "players" in data:
+                self.__parse_players(data["players"])
+            if "scoreboard" in data:
+                self.__parse_scoreboard(data["scoreboard"])
+            if "settings" in data:
+                self.__parse_settings(data["settings"])
+            if "standings" in data:
+                self.__parse_standings(data["standings"])
+            if "teams" in data:
+                self.__parse_teams(data["teams"])
+            if "transactions" in data:
+                self.__parse_transactions(data["transactions"])
 
     def __parse_draft_results(self, json):
-        self.draft_results = [DraftResult(json[str(d)]['draft_result']) for d in range(json['count'])]
+        self.draft_results = [
+            DraftResult(json[str(d)]["draft_result"]) for d in range(json["count"])
+        ]
 
     def __parse_players(self, json):
         if not json:
             self.players = []
         else:
-            self.players = [Player(json[str(d)]['player']) for d in range(json['count'])]
+            self.players = [
+                Player(json[str(d)]["player"]) for d in range(json["count"])
+            ]
 
     def __parse_scoreboard(self, json):
-        json = json['0']['matchups']
-        self.matchups = [Matchup(json[str(d)]['matchup']) for d in range(json['count'])]
+        json = json["0"]["matchups"]
+        self.matchups = [Matchup(json[str(d)]["matchup"]) for d in range(json["count"])]
 
     def __parse_settings(self, json):
         self.settings = Settings(json)
 
     def __parse_standings(self, json):
-        json = json[0]['teams']
-        self.standings = [Team(json[str(d)]['team']) for d in range(json['count'])]
+        json = json[0]["teams"]
+        self.standings = [Team(json[str(d)]["team"]) for d in range(json["count"])]
 
     def __parse_teams(self, json):
-        self.teams = [Team(json[str(d)]['team']) for d in range(json['count'])]
+        self.teams = [Team(json[str(d)]["team"]) for d in range(json["count"])]
 
     def __parse_transactions(self, json):
         self.transactions = []
 
         if not json:
             return
 
-        for t in reversed(range(json['count'])):
-            transaction = json[str(t)]['transaction']
-            transaction_type = transaction[0]['type']
+        for t in reversed(range(json["count"])):
+            transaction = json[str(t)]["transaction"]
+            transaction_type = transaction[0]["type"]
 
-            if transaction_type == 'add':
+            if transaction_type == "add":
                 self.transactions.append(Add(transaction))
-            elif transaction_type == 'drop':
+            elif transaction_type == "drop":
                 self.transactions.append(Drop(transaction))
-            elif transaction_type == 'add/drop':
+            elif transaction_type == "add/drop":
                 self.transactions.append(AddDrop(transaction))
-            elif transaction_type == 'trade':
+            elif transaction_type == "trade":
                 self.transactions.append(Trade(transaction))
 
 
 class DraftResult:
     def __init__(self, json):
-        self.pick = as_int(json['pick'])
-        self.round = as_int(json['round'])
-        self.team_key = json['team_key']
-        self.player = Player(json['0']['players']['0']['player'])
-    
+        self.pick = as_int(json["pick"])
+        self.round = as_int(json["round"])
+        self.team_key = json["team_key"]
+        self.player = Player(json["0"]["players"]["0"]["player"])
+
     def __repr__(self):
-        return str(self.__dict__) # pragma: no cover
+        return str(self.__dict__)  # pragma: no cover
+
 
 class Matchup:
     def __init__(self, json):
-        self.week = as_int(json.get('week'))
-        self.week_start = json.get('week_start')
-        self.week_end = json.get('week_end')
-        self.status = json.get('status')
-        self.is_current = self.status == 'midevent'
-        self.is_playoffs = as_bool(json.get('is_playoffs'))
-        self.is_consolation = as_bool(json.get('is_consolation'))
-        self.is_tied = as_bool(json.get('is_tied'))
-        
+        self.week = as_int(json.get("week"))
+        self.week_start = json.get("week_start")
+        self.week_end = json.get("week_end")
+        self.status = json.get("status")
+        self.is_current = self.status == "midevent"
+        self.is_playoffs = as_bool(json.get("is_playoffs"))
+        self.is_consolation = as_bool(json.get("is_consolation"))
+        self.is_tied = as_bool(json.get("is_tied"))
+
         self.__parse_teams(json)
 
     def __parse_winning_team(self, teams, winning_team_key):
         return next(team for team in teams if team.key == winning_team_key)
 
     def __parse_losing_team(self, teams, winning_team_key):
         return next(team for team in teams if team.key != winning_team_key)
 
     def __parse_teams(self, json):
-        winning_team_key = json.get('winner_team_key')
-        json = json['0']['teams']
-        self.teams = [Team(json[str(t)]['team']) for t in range(json['count'])]
+        winning_team_key = json.get("winner_team_key")
+        json = json["0"]["teams"]
+        self.teams = [Team(json[str(t)]["team"]) for t in range(json["count"])]
         if winning_team_key:
             self.winning_team = self.__parse_winning_team(self.teams, winning_team_key)
             self.losing_team = self.__parse_losing_team(self.teams, winning_team_key)
 
     def __repr__(self):
-        return str(self.__dict__) # pragma: no cover
+        return str(self.__dict__)  # pragma: no cover
 
 
 class Settings:
     def __init__(self, json):
         json = json[0]
-        self.draft_type = json.get('draft_type')
-        self.is_auction = as_bool(json.get('is_auction_draft'))
-        self.scoring_type = json.get('scoring_type')
-        self.persistent_url = json.get('persistent_url')
-        self.has_playoff = as_bool(json.get('uses_playoff'))
-        self.has_consolation = as_bool(json.get('has_playoff_consolation_games'))
-        self.playoff_start_week = as_int(json.get('playoff_start_week'))
-        self.has_reseeding = as_bool(json.get('uses_playoff_reseeding'))
-        self.lock_eliminatd_teams = as_bool(json.get('uses_lock_eliminated_teams'))
-        self.num_playoff_teams = as_int(json.get('num_playoff_teams'))
-        self.num_consolation_teams = as_int(json.get('num_playoff_consolation_teams'))
-        self.has_multiweek_championship = json.get('has_multiweek_championship')
-        self.waiver_type = json.get('waiver_type')
-        self.waiver_rule = json.get('waiver_rule')
-        self.uses_faab = as_bool(json.get('uses_faab'))
-        self.seconds_per_pick = as_int(json.get('draft_pick_time'))
-        self.post_draft_players = json.get('post_draft_players')
-        self.max_teams = as_int(json.get('max_teams'))
-        self.days_on_waivers = as_int(json.get('waiver_time'))
-        self.trade_end_date = json.get('trade_end_date')
-        self.trade_ratify_type = json.get('trade_ratify_type')
-        self.days_to_veto = as_int(json.get('trade_reject_time'))
-        self.player_pool = json.get('player_pool')
-        self.cant_cut_list = json.get('cant_cut_list')
-        self.trade_draft_picks = as_bool(json.get('can_trade_draft_picks'))
-        self.fractional_points = as_bool(json.get('uses_fractional_points'))
-        self.negative_points = as_bool(json.get('uses_negative_points'))
+        self.draft_type = json.get("draft_type")
+        self.is_auction = as_bool(json.get("is_auction_draft"))
+        self.scoring_type = json.get("scoring_type")
+        self.persistent_url = json.get("persistent_url")
+        self.has_playoff = as_bool(json.get("uses_playoff"))
+        self.has_consolation = as_bool(json.get("has_playoff_consolation_games"))
+        self.playoff_start_week = as_int(json.get("playoff_start_week"))
+        self.has_reseeding = as_bool(json.get("uses_playoff_reseeding"))
+        self.lock_eliminatd_teams = as_bool(json.get("uses_lock_eliminated_teams"))
+        self.num_playoff_teams = as_int(json.get("num_playoff_teams"))
+        self.num_consolation_teams = as_int(json.get("num_playoff_consolation_teams"))
+        self.has_multiweek_championship = json.get("has_multiweek_championship")
+        self.waiver_type = json.get("waiver_type")
+        self.waiver_rule = json.get("waiver_rule")
+        self.uses_faab = as_bool(json.get("uses_faab"))
+        self.seconds_per_pick = as_int(json.get("draft_pick_time"))
+        self.post_draft_players = json.get("post_draft_players")
+        self.max_teams = as_int(json.get("max_teams"))
+        self.days_on_waivers = as_int(json.get("waiver_time"))
+        self.trade_end_date = json.get("trade_end_date")
+        self.trade_ratify_type = json.get("trade_ratify_type")
+        self.days_to_veto = as_int(json.get("trade_reject_time"))
+        self.player_pool = json.get("player_pool")
+        self.cant_cut_list = json.get("cant_cut_list")
+        self.trade_draft_picks = as_bool(json.get("can_trade_draft_picks"))
+        self.fractional_points = as_bool(json.get("uses_fractional_points"))
+        self.negative_points = as_bool(json.get("uses_negative_points"))
         self.divisions = self.__parse_divisions(json)
         self.roster_positions = self.__parse_roster_positions(json)
         self.stat_categories = self.__parse_stat_categories(json)
-    
+
     def __repr__(self):
-        return str(self.__dict__) # pragma: no cover
+        return str(self.__dict__)  # pragma: no cover
 
     def __parse_roster_positions(self, json):
-        json = json.get('roster_positions')
+        json = json.get("roster_positions")
         return {
-            data['roster_position']['position']: as_int(data['roster_position']['count'])
+            data["roster_position"]["position"]: as_int(
+                data["roster_position"]["count"]
+            )
             for data in json
         }
 
     def __parse_stat_categories(self, json):
-        modifiers = {s['stat']['stat_id']: as_float(s['stat']['value']) for s in json['stat_modifiers']['stats']}
-        categories = json['stat_categories']['stats']
-        return [Stat(cat['stat'], modifiers) for cat in categories]
+        modifiers = {
+            s["stat"]["stat_id"]: as_float(s["stat"]["value"])
+            for s in json["stat_modifiers"]["stats"]
+        }
+        categories = json["stat_categories"]["stats"]
+        return [Stat(cat["stat"], modifiers) for cat in categories]
 
     def __parse_divisions(self, json):
-        json = json.get('divisions', [])
-        return [Division(d['division']) for d in json]
+        json = json.get("divisions", [])
+        return [Division(d["division"]) for d in json]
 
 
 class Division:
     def __init__(self, json):
-        self.id = as_int(json['division_id'])
-        self.name = json['name']
-    
+        self.id = as_int(json["division_id"])
+        self.name = json["name"]
+
     def __repr__(self):
-        return str(self.__dict__) # pragma: no cover
+        return str(self.__dict__)  # pragma: no cover
+
 
 class Stat:
     def __init__(self, category, modifiers):
-        self.id = category['stat_id']
-        self.name = category['name']
-        self.display_name = category['display_name']
+        self.id = category["stat_id"]
+        self.name = category["name"]
+        self.display_name = category["display_name"]
         self.value = modifiers.get(self.id)
-    
+
     def __repr__(self):
-        return str(self.__dict__) # pragma: no cover
+        return str(self.__dict__)  # pragma: no cover
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api/models/user.py` & `yfantasy-api-0.0.6/yfantasy_api/models/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from yfantasy_api.models.game import Game
 from yfantasy_api.models.league import League
 
 
 class User:
     def __init__(self, json):
         self.json = json
-        self.guid = json[0]['guid']
+        self.guid = json[0]["guid"]
         self.__parse_sub_resources(json)
 
     def __parse_sub_resources(self, json):
         for data in json:
-            if 'games' in data:
-                self.__parse_games(data['games'])
-            if 'teams' in data:
-                self.__parse_teams(data['teams'])
+            if "games" in data:
+                self.__parse_games(data["games"])
+            if "teams" in data:
+                self.__parse_teams(data["teams"])
 
     def __parse_games(self, json):
-        self.games = [Game(json[str(d)]['game']) for d in range(json['count'])]
+        self.games = [Game(json[str(d)]["game"]) for d in range(json["count"])]
 
     def __parse_teams(self, json):
-        self.teams = [Team(json[str(d)]['team']) for d in range(json['count'])]
+        self.teams = [Team(json[str(d)]["team"]) for d in range(json["count"])]
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api.egg-info/PKG-INFO` & `yfantasy-api-0.0.6/yfantasy_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfantasy-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package to access the Yahoo! Fantasy APIs
 Home-page: https://github.com/hkyplyr/yfantasy-api
 Author: Travis Paquette
 Author-email: tpaqu15@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -23,15 +23,15 @@
 pip install yfantasy_api
 ```
 
 ## Usage examples
 ### Obtain team information, including the roster with player stats for March 31st 2021
 ``` python
 # The request url created is: /team/nhl.l.12345.t.1/roster/players/stats;type=date;date=2021-03-31
-from yfantasy_api.api import YahooFantasyApi
+from yfantasy_api import YahooFantasyApi
 
 league_id = 12345  # This should be the id of the league you are querying
 game_id = 'nhl'    # This should be the id of the game you are querying
 team_id = 1        # This should be the id of the team you are querying
 
 api = YahooFantasyApi(league_id, game_id)
 team = api \
@@ -51,15 +51,15 @@
 # Jake Guentzel 0.00
 # ...truncated for brevity...
 ```
 
 ### Obtain draft_results, including player information for each pick.
 ``` python
 # The request url created is: /league/nhl.l.12345/draft_results/players
-from yfantasy_api.api import YahooFantasyApi
+from yfantasy_api import YahooFantasyApi
 
 league_id = 12345  # This should be the id of the league you are querying
 game_id = 'nhl'    # This should be the id of the game you are querying
 team_id = 1        # This should be the id of the team you are querying
 
 api = YahooFantasyApi(league_id, game_id)
 league = api \
```

### Comparing `yfantasy-api-0.0.5/yfantasy_api.egg-info/SOURCES.txt` & `yfantasy-api-0.0.6/yfantasy_api.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 tests/test_league_api.py
 tests/test_team_api.py
 tests/test_user_api.py
 yfantasy_api/__init__.py
 yfantasy_api.egg-info/PKG-INFO
 yfantasy_api.egg-info/SOURCES.txt
 yfantasy_api.egg-info/dependency_links.txt
+yfantasy_api.egg-info/requires.txt
 yfantasy_api.egg-info/top_level.txt
 yfantasy_api/api/__init__.py
 yfantasy_api/api/api.py
 yfantasy_api/api/auth.py
 yfantasy_api/api/game.py
 yfantasy_api/api/league.py
 yfantasy_api/api/team.py
```


# Comparing `tmp/py3-pinterest-1.3.0.tar.gz` & `tmp/py3_pinterest-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py3-pinterest-1.3.0.tar", last modified: Tue May  3 16:29:34 2022, max compression
+gzip compressed data, was "py3_pinterest-1.4.0.tar", last modified: Thu May  9 11:00:28 2024, max compression
```

## Comparing `py3-pinterest-1.3.0.tar` & `py3_pinterest-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 b.stoilov (1052132106) LMS\Domain Users (150487713)        0 2022-05-03 16:29:34.740183 py3-pinterest-1.3.0/
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)     1056 2022-05-03 15:30:00.000000 py3-pinterest-1.3.0/LICENSE
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)       26 2022-05-03 15:30:00.000000 py3-pinterest-1.3.0/MANIFEST.in
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)     9907 2022-05-03 16:29:34.739660 py3-pinterest-1.3.0/PKG-INFO
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)     7269 2022-05-03 15:30:00.000000 py3-pinterest-1.3.0/README.md
-drwxr-xr-x   0 b.stoilov (1052132106) LMS\Domain Users (150487713)        0 2022-05-03 16:29:34.732037 py3-pinterest-1.3.0/py3_pinterest.egg-info/
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)     9907 2022-05-03 16:29:34.000000 py3-pinterest-1.3.0/py3_pinterest.egg-info/PKG-INFO
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)      389 2022-05-03 16:29:34.000000 py3-pinterest-1.3.0/py3_pinterest.egg-info/SOURCES.txt
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)        1 2022-05-03 16:29:34.000000 py3-pinterest-1.3.0/py3_pinterest.egg-info/dependency_links.txt
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)        1 2022-05-03 15:32:10.000000 py3-pinterest-1.3.0/py3_pinterest.egg-info/not-zip-safe
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)       69 2022-05-03 16:29:34.000000 py3-pinterest-1.3.0/py3_pinterest.egg-info/requires.txt
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)        7 2022-05-03 16:29:34.000000 py3-pinterest-1.3.0/py3_pinterest.egg-info/top_level.txt
-drwxr-xr-x   0 b.stoilov (1052132106) LMS\Domain Users (150487713)        0 2022-05-03 16:29:34.738930 py3-pinterest-1.3.0/py3pin/
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)      869 2022-05-03 15:30:00.000000 py3-pinterest-1.3.0/py3pin/BookmarkManager.py
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)    46490 2022-05-03 16:12:27.000000 py3-pinterest-1.3.0/py3pin/Pinterest.py
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)     1239 2022-05-03 15:30:00.000000 py3-pinterest-1.3.0/py3pin/Registry.py
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)     1047 2022-05-03 15:30:00.000000 py3-pinterest-1.3.0/py3pin/RequestBuilder.py
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)       20 2022-05-03 15:30:00.000000 py3-pinterest-1.3.0/py3pin/__init__.py
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)       22 2022-05-03 16:21:43.000000 py3-pinterest-1.3.0/py3pin/__version__.py
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)       38 2022-05-03 16:29:34.740309 py3-pinterest-1.3.0/setup.cfg
--rw-r--r--   0 b.stoilov (1052132106) LMS\Domain Users (150487713)     2790 2022-05-03 16:02:15.000000 py3-pinterest-1.3.0/setup.py
+drwxr-xr-x   0 borislav.stoilov   (502) staff       (20)        0 2024-05-09 11:00:28.626884 py3_pinterest-1.4.0/
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)     1056 2024-05-09 10:56:39.000000 py3_pinterest-1.4.0/LICENSE
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)       26 2024-05-09 10:56:39.000000 py3_pinterest-1.4.0/MANIFEST.in
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)     8191 2024-05-09 11:00:28.625892 py3_pinterest-1.4.0/PKG-INFO
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)     7274 2024-05-09 10:56:39.000000 py3_pinterest-1.4.0/README.md
+drwxr-xr-x   0 borislav.stoilov   (502) staff       (20)        0 2024-05-09 11:00:28.625338 py3_pinterest-1.4.0/py3_pinterest.egg-info/
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)     8191 2024-05-09 11:00:28.000000 py3_pinterest-1.4.0/py3_pinterest.egg-info/PKG-INFO
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)      389 2024-05-09 11:00:28.000000 py3_pinterest-1.4.0/py3_pinterest.egg-info/SOURCES.txt
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)        1 2024-05-09 11:00:28.000000 py3_pinterest-1.4.0/py3_pinterest.egg-info/dependency_links.txt
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)        1 2024-05-09 11:00:28.000000 py3_pinterest-1.4.0/py3_pinterest.egg-info/not-zip-safe
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)       69 2024-05-09 11:00:28.000000 py3_pinterest-1.4.0/py3_pinterest.egg-info/requires.txt
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)        7 2024-05-09 11:00:28.000000 py3_pinterest-1.4.0/py3_pinterest.egg-info/top_level.txt
+drwxr-xr-x   0 borislav.stoilov   (502) staff       (20)        0 2024-05-09 11:00:28.624771 py3_pinterest-1.4.0/py3pin/
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)      869 2024-05-09 10:56:39.000000 py3_pinterest-1.4.0/py3pin/BookmarkManager.py
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)    48612 2024-05-09 10:56:39.000000 py3_pinterest-1.4.0/py3pin/Pinterest.py
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)     1239 2024-05-09 10:56:39.000000 py3_pinterest-1.4.0/py3pin/Registry.py
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)     1047 2024-05-09 10:56:39.000000 py3_pinterest-1.4.0/py3pin/RequestBuilder.py
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)       20 2024-05-09 10:56:39.000000 py3_pinterest-1.4.0/py3pin/__init__.py
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)       22 2024-05-09 10:58:14.000000 py3_pinterest-1.4.0/py3pin/__version__.py
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)       38 2024-05-09 11:00:28.626989 py3_pinterest-1.4.0/setup.cfg
+-rw-r--r--   0 borislav.stoilov   (502) staff       (20)     2790 2024-05-09 10:56:39.000000 py3_pinterest-1.4.0/setup.py
```

### Comparing `py3-pinterest-1.3.0/LICENSE` & `py3_pinterest-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py3-pinterest-1.3.0/PKG-INFO` & `py3_pinterest-1.4.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,253 +1,228 @@
-Metadata-Version: 2.1
-Name: py3-pinterest
-Version: 1.3.0
-Summary: Unofficial pinterest api implemented in python 3
-Home-page: https://github.com/bstoilov/py3-pinterest
-Author: Borislav Stoilov
-Author-email: boriostoilov@gmail.com
-License: MIT
-Description: 
-        # py3-pinterest
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        Unofficial Pinterest API implemented in python 3 that can do all Pinterest tasks like comment, pin, repin, follow, unfollow and more.
-        
-        It is implemented by directly calling the pinterest servers, mimicking an actual browser, so you don't need pinterest API key.
-        
-        If you see any issues, or find bugs feel free to report them here on the github repo.
-        
-        ## Community guides
-        [Get started with pinterest automation](https://martechwithme.com/how-to-automate-pinterest-interactions-python "Martechwithme.com")
-        
-        [Automated posting to Pinterest (in Russian)](https://www.youtube.com/watch?v=TQBceIiv_Gk&ab_channel=Analitiq "Analitiq YouTube")
-        
-        
-        ## Install using pip
-        ```pip install py3-pinterest```
-        
-        
-        ### NOTE: for each of the functionalities listed below there is a working example under the project root.
-        
-        ### Create new instance of the API
-        
-        ```pinterest = Pinterest(email='your email goes here', password='password goes here', username='look in pinterest url', cred_root='cred root dir')```
-        
-        cred_root is the dir (automatically created if missing) that will store some cookies nad sessions, so you don't need to login before each request.
-        Make sure you specify a path with read/write permissions.
-        
-        Proxies example:
-        
-        ```
-        proxies = {"http":"http://username:password@proxy_ip:proxy_port"}
-        Pinterest(email='emai', password='pass', username='name', cred_root='cred_root', proxies=proxies)
-        ```
-        
-        # The following features are currently supported
-        
-        ## Login/Logout
-        ## NOTE: Pinterest integrated google recaptcha. This means we have to use web driver to login. For that reason you must have chrome installed on you computer, in order for the login to work.
-        ### If you want to use many accounts, you should associate proxy with each one of them and login only with that proxy
-        ### pinterest.login(proxy='ip_address:port')
-        Login will store auth cookies for later use. These cookies are usually valid for ~15 days, then you will start getting 403 and 401 errors, which means you need to call login again. 
-        ## Login
-        Login is required to permit actions to the Pinterest servers. Login will store auth cookies for later use. These cookies are usually valid for ~15 days, then you will start getting 403 and 401 errors, which means you need to call login again. 
-        
-        ```pinterest.login()```
-        
-        ```pinterest.logout()```
-        
-        
-        
-        ## Load profile
-        You can load profile for currently logged in user or any user specified by username.
-        
-        ```user_profile = pinterest.get_user_overview()```
-        
-        
-        ## Board and pin management
-        
-        ### Get all boards of user:
-        
-        ```boards = pinterest.boards(username='username')```
-        
-        ### List all pins in board
-        ```pins = pinterest.board_feed(board_id=board_id)```
-        
-        If username is left blank, current logged in user will be used.
-        
-        
-        ### Delete pin
-        ```pinterest.delete_pin(pin_id='pin_id')```
-        
-        ### Repin
-        
-        ```pinterest.repin(board_id='board_id', pin_id='pin_id')```
-        
-        ### Get ID of created pin, section, or board
-        
-        All functions return the post/get data from the request. If you dig a little deeper by going myrequest.content you get the actual HTML response, which can then be turned into a dict by using JSON.
-        
-        Example:
-        
-        ```py
-        import json
-        
-        pin_response = upload_pin(board_id='',
-                     image_path='test.png',
-                     description='TESTING PIN FUNCTIONALITY WITH ID FETCHING',
-                     title='Foobar Barfood',
-                     section_id=None,
-                     link='')
-        
-        response_data = json.loads(pin_response.content)
-        ```
-        
-        Some helpful notes on the response:
-        Everything is stored inside the "resource_response" key. You can use that and grab all sorts of data like so:
-        
-        ```py
-        # This is how you would access this information when creating a pin
-        
-        id = response_data["resource_response"]["data"]["id"]
-        board_id = response_data["resource_response"]["data"]["board"]["id"]
-        section_id = response_data["resource_response"]["data"]["section"]["id"]
-        pinner_username = response_data["resource_response"]["data"]["pinner"]["username"]
-        pinner_id = response_data["resource_response"]["data"]["pinner"]["id"]
-        
-        # If you wanted to access this information in a different circumstance,
-        # keep in mind that whatever your creating should be the first level under "data"
-        # I.e, I created a board, and I want to get the board ID. It would now be:
-        
-        board_id = response_data["resource_response"]["data"]["id"]
-        ```
-        
-        ### Get pinnable images
-        A pinterest feature they use to pin from websites
-        
-        ```pinterest.get_pinnable_images(url='https://www.tumblr.com/search/food')```
-        
-        ### Pin
-        
-        Pin image by web url:
-        
-        ```pinterest.pin(board_id=board_id, image_url=image_url, description=description, title=title)```
-        
-        Pin image from local file:
-        
-        ```pinterest.upload_pin(board_id=board_id, section_id=section_id, image_file=image_path, description=description, title=title, link=link)```
-        
-        ### Get home feed pins
-        
-        ``` home_feed_batch = pinterest.home_feed()```
-        
-        ### Get board recommendations (this is the 'more ideas' api)
-        
-        ```rec_batch = pinterest.board_recommendations(board_id=board_id)```
-        
-        ### Get pin information by id
-        
-        ```pinterest.load_pin(pin_id='pin_id')```
-        
-        ### Board Section support
-        ```pinterest.create_board_section(board_id=board_id, section_name=section_name)```
-        ```pinterest.delete_board_section(section_id=section_id)```
-        ```pinterest.get_board_sections(board_id=board_id)```
-        
-        You can also pin and repin to sections.
-        
-        
-        ## Follow/Unfollow
-        
-        ### Follow
-        ```pinterest.follow_user(user_id='target_user_id', username='target_username')```
-        
-        Follow limit is 300 per day, after that they might place you on watch list
-        
-        
-        ### Unfollow
-        
-        ```pinterest.unfollow_user(user_id='target_user_id', username='target_username')```
-        
-        Unfollow limit is 350 per day, after that they might place you on watch list
-        
-        ### Get following
-        
-        ```following_batch = pinterest.get_following(username='some_user')```
-        
-        If username is not provided current user will be used
-        
-        ### Get followers
-        
-        ```followers_batch=pinterest.get_user_followers(username='some_user')```
-        
-        If username is not provided current user will be used
-        
-        ### Follow board
-        
-        ```pinterest.follow_board(board_id=board_id)```
-        
-        ### Unfollow board
-        
-        ```pinterest.unfollow_board(board_id=board_id)```
-        
-        
-        ## Search
-        
-        ```search_batch = pinterest.search(scope='boards', query='food')```
-        
-        Current pinterest scopes are: pins, buyable_pins, my_pins, videos, boards
-        
-        ### Visual Search
-        
-        ```
-          pin_data = pinterest.load_pin(pin_id='pin_id')
-          search_batch = pinterest.visual_search(pin_data, x=10, y=50, w=100, h=100)
-        ```
-        ## User interactions
-        ### Invite to board
-        
-        ```pinterest.invite(board_id=board_id, user_id=target_user_id)```
-        
-        ### Delete board invite
-        
-        ```pinterest.delete_invite(board_id=board_id, invited_user_id=target_user_id)```
-        
-        ### Get board invites
-        
-        ```invites_batch = pinterest.get_board_invites(board_id=board_id)```
-        
-        ### Comment
-        
-        ```pinterest.comment(pin_id=pin_id, text=comment_text)```
-        
-        ### Delete comment 
-        ```pinterest.delete_comment(pin_id=pin_id, comment_id=comment_id)```
-        
-        ### Get Pin comments
-        
-        ```pinterest.get_comments(pin_id='pin_id')```
-        
-        
-        ### Send personal message
-        ```pinterest.send_message(conversation_id=conversation_id, pin_id="(pin_id)", message="hey")```
-        
-        
-        ### Access to type suggestions you see in the search input
-        ```pinterest.type_ahead(term='apple')```
-        
-        
-        
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.5.0
-Description-Content-Type: text/markdown
+# py3-pinterest
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+Unofficial Pinterest API implemented in python 3 that can do all Pinterest tasks like comment, pin, repin, follow, unfollow, and more.
+
+It is implemented by directly calling the pinterest servers, mimicking an actual browser, so you don't need pinterest API key.
+
+If you see any issues, or find bugs feel free to report them here on the github repo.
+
+## Community guides
+[Get started with pinterest automation](https://martechwithme.com/how-to-automate-pinterest-interactions-python "Martechwithme.com")
+
+[Automated posting to Pinterest (in Russian)](https://www.youtube.com/watch?v=TQBceIiv_Gk&ab_channel=Analitiq "Analitiq YouTube")
+
+
+## Install using pip
+```pip install py3-pinterest```
+
+
+### NOTE: for each of the functionalities listed below there is a working example under the project root.
+
+### Create new instance of the API
+
+```pinterest = Pinterest(email='your email goes here', password='password goes here', username='look in pinterest url', cred_root='cred root dir')```
+
+cred_root is the dir (automatically created if missing) that will store some cookies and sessions, so you don't need to login before each request.
+Make sure you specify a path with read/write permissions.
+
+Proxies example:
+
+```
+proxies = {"http":"http://username:password@proxy_ip:proxy_port"}
+Pinterest(email='emai', password='pass', username='name', cred_root='cred_root', proxies=proxies)
+```
+
+# The following features are currently supported
+
+## Login/Logout
+## NOTE: Pinterest integrated google recaptcha. This means we have to use web driver to login. For that reason you must have chrome installed on you computer, in order for the login to work.
+### If you want to use many accounts, you should associate proxy with each one of them and login only with that proxy
+### pinterest.login(proxy='ip_address:port')
+Login will store auth cookies for later use. These cookies are usually valid for ~15 days, then you will start getting 403 and 401 errors, which means you need to call login again. 
+## Login
+Login is required to permit actions to the Pinterest servers. Login will store auth cookies for later use. These cookies are usually valid for ~15 days, then you will start getting 403 and 401 errors, which means you need to call login again. 
+
+```pinterest.login()```
+
+```pinterest.logout()```
+
+
+
+## Load profile
+You can load profile for currently logged in user or any user specified by username.
+
+```user_profile = pinterest.get_user_overview()```
+
+
+## Board and pin management
+
+### Get all boards of user:
+
+```boards = pinterest.boards(username='username')```
+
+### List all pins in board
+```pins = pinterest.board_feed(board_id=board_id)```
+
+If username is left blank, current logged in user will be used.
+
+
+### Delete pin
+```pinterest.delete_pin(pin_id='pin_id')```
+
+### Repin
+
+```pinterest.repin(board_id='board_id', pin_id='pin_id')```
+
+### Get ID of created pin, section, or board
+
+All functions return the post/get data from the request. If you dig a little deeper by going myrequest.content you get the actual HTML response, which can then be turned into a dict by using JSON.
+
+Example:
+
+```py
+import json
+
+pin_response = upload_pin(board_id='',
+             image_path='test.png',
+             description='TESTING PIN FUNCTIONALITY WITH ID FETCHING',
+             title='Foobar Barfood',
+             section_id=None,
+             link='')
+
+response_data = json.loads(pin_response.content)
+```
+
+Some helpful notes on the response:
+Everything is stored inside the "resource_response" key. You can use that and grab all sorts of data like so:
+
+```py
+# This is how you would access this information when creating a pin
+
+id = response_data["resource_response"]["data"]["id"]
+board_id = response_data["resource_response"]["data"]["board"]["id"]
+section_id = response_data["resource_response"]["data"]["section"]["id"]
+pinner_username = response_data["resource_response"]["data"]["pinner"]["username"]
+pinner_id = response_data["resource_response"]["data"]["pinner"]["id"]
+
+# If you wanted to access this information in a different circumstance,
+# keep in mind that whatever you are creating should be the first level under "data"
+# I.e, I created a board, and I want to get the board ID. It would now be:
+
+board_id = response_data["resource_response"]["data"]["id"]
+```
+
+### Get pinnable images
+A pinterest feature they use to pin from websites
+
+```pinterest.get_pinnable_images(url='https://www.tumblr.com/search/food')```
+
+### Pin
+
+Pin image by web url:
+
+```pinterest.pin(board_id=board_id, image_url=image_url, description=description, title=title)```
+
+Pin image from local file:
+
+```pinterest.upload_pin(board_id=board_id, section_id=section_id, image_file=image_path, description=description, title=title, link=link)```
+
+### Get home feed pins
+
+``` home_feed_batch = pinterest.home_feed()```
+
+### Get board recommendations (this is the 'more ideas' api)
+
+```rec_batch = pinterest.board_recommendations(board_id=board_id)```
+
+### Get pin information by id
+
+```pinterest.load_pin(pin_id='pin_id')```
+
+### Board Section support
+```pinterest.create_board_section(board_id=board_id, section_name=section_name)```
+```pinterest.delete_board_section(section_id=section_id)```
+```pinterest.get_board_sections(board_id=board_id)```
+
+You can also pin and repin to sections.
+
+
+## Follow/Unfollow
+
+### Follow
+```pinterest.follow_user(user_id='target_user_id', username='target_username')```
+
+Follow limit is 300 per day, after that they might place you on a watch list
+
+
+### Unfollow
+
+```pinterest.unfollow_user(user_id='target_user_id', username='target_username')```
+
+Unfollow limit is 350 per day, after that they might place you on a watch list
+
+### Get following
+
+```following_batch = pinterest.get_following(username='some_user')```
+
+If username is not provided current user will be used
+
+### Get followers
+
+```followers_batch=pinterest.get_user_followers(username='some_user')```
+
+If username is not provided current user will be used
+
+### Follow board
+
+```pinterest.follow_board(board_id=board_id)```
+
+### Unfollow board
+
+```pinterest.unfollow_board(board_id=board_id)```
+
+
+## Search
+
+```search_batch = pinterest.search(scope='boards', query='food')```
+
+Current pinterest scopes are: pins, buyable_pins, my_pins, videos, boards
+
+### Visual Search
+
+```
+  pin_data = pinterest.load_pin(pin_id='pin_id')
+  search_batch = pinterest.visual_search(pin_data, x=10, y=50, w=100, h=100)
+```
+## User interactions
+### Invite to board
+
+```pinterest.invite(board_id=board_id, user_id=target_user_id)```
+
+### Delete board invite
+
+```pinterest.delete_invite(board_id=board_id, invited_user_id=target_user_id)```
+
+### Get board invites
+
+```invites_batch = pinterest.get_board_invites(board_id=board_id)```
+
+### Comment
+
+```pinterest.comment(pin_id=pin_id, text=comment_text)```
+
+### Delete comment 
+```pinterest.delete_comment(pin_id=pin_id, comment_id=comment_id)```
+
+### Get Pin comments
+
+```pinterest.get_comments(pin_id='pin_id')```
+
+
+### Send personal message
+```pinterest.send_message(conversation_id=conversation_id, pin_id="(pin_id)", message="hey")```
+
+
+### Access to type suggestions you see in the search input
+```pinterest.type_ahead(term='apple')```
+
```

### Comparing `py3-pinterest-1.3.0/README.md` & `py3_pinterest-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,38 @@
+Metadata-Version: 2.1
+Name: py3-pinterest
+Version: 1.4.0
+Summary: Unofficial pinterest api implemented in python 3
+Home-page: https://github.com/bstoilov/py3-pinterest
+Author: Borislav Stoilov
+Author-email: boriostoilov@gmail.com
+License: MIT
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.5.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: beautifulsoup4
+Requires-Dist: requests-toolbelt
+Requires-Dist: selenium
+Requires-Dist: webdriver-manager
+
+
 # py3-pinterest
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-Unofficial Pinterest API implemented in python 3 that can do all Pinterest tasks like comment, pin, repin, follow, unfollow and more.
+Unofficial Pinterest API implemented in python 3 that can do all Pinterest tasks like comment, pin, repin, follow, unfollow, and more.
 
 It is implemented by directly calling the pinterest servers, mimicking an actual browser, so you don't need pinterest API key.
 
 If you see any issues, or find bugs feel free to report them here on the github repo.
 
 ## Community guides
 [Get started with pinterest automation](https://martechwithme.com/how-to-automate-pinterest-interactions-python "Martechwithme.com")
@@ -19,15 +46,15 @@
 
 ### NOTE: for each of the functionalities listed below there is a working example under the project root.
 
 ### Create new instance of the API
 
 ```pinterest = Pinterest(email='your email goes here', password='password goes here', username='look in pinterest url', cred_root='cred root dir')```
 
-cred_root is the dir (automatically created if missing) that will store some cookies nad sessions, so you don't need to login before each request.
+cred_root is the dir (automatically created if missing) that will store some cookies and sessions, so you don't need to login before each request.
 Make sure you specify a path with read/write permissions.
 
 Proxies example:
 
 ```
 proxies = {"http":"http://username:password@proxy_ip:proxy_port"}
 Pinterest(email='emai', password='pass', username='name', cred_root='cred_root', proxies=proxies)
@@ -102,15 +129,15 @@
 id = response_data["resource_response"]["data"]["id"]
 board_id = response_data["resource_response"]["data"]["board"]["id"]
 section_id = response_data["resource_response"]["data"]["section"]["id"]
 pinner_username = response_data["resource_response"]["data"]["pinner"]["username"]
 pinner_id = response_data["resource_response"]["data"]["pinner"]["id"]
 
 # If you wanted to access this information in a different circumstance,
-# keep in mind that whatever your creating should be the first level under "data"
+# keep in mind that whatever you are creating should be the first level under "data"
 # I.e, I created a board, and I want to get the board ID. It would now be:
 
 board_id = response_data["resource_response"]["data"]["id"]
 ```
 
 ### Get pinnable images
 A pinterest feature they use to pin from websites
@@ -148,22 +175,22 @@
 
 
 ## Follow/Unfollow
 
 ### Follow
 ```pinterest.follow_user(user_id='target_user_id', username='target_username')```
 
-Follow limit is 300 per day, after that they might place you on watch list
+Follow limit is 300 per day, after that they might place you on a watch list
 
 
 ### Unfollow
 
 ```pinterest.unfollow_user(user_id='target_user_id', username='target_username')```
 
-Unfollow limit is 350 per day, after that they might place you on watch list
+Unfollow limit is 350 per day, after that they might place you on a watch list
 
 ### Get following
 
 ```following_batch = pinterest.get_following(username='some_user')```
 
 If username is not provided current user will be used
 
@@ -222,10 +249,7 @@
 ### Send personal message
 ```pinterest.send_message(conversation_id=conversation_id, pin_id="(pin_id)", message="hey")```
 
 
 ### Access to type suggestions you see in the search input
 ```pinterest.type_ahead(term='apple')```
 
-
-
-
```

### Comparing `py3-pinterest-1.3.0/py3_pinterest.egg-info/PKG-INFO` & `py3_pinterest-1.4.0/py3_pinterest.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,253 +1,255 @@
 Metadata-Version: 2.1
 Name: py3-pinterest
-Version: 1.3.0
+Version: 1.4.0
 Summary: Unofficial pinterest api implemented in python 3
 Home-page: https://github.com/bstoilov/py3-pinterest
 Author: Borislav Stoilov
 Author-email: boriostoilov@gmail.com
 License: MIT
-Description: 
-        # py3-pinterest
-        [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-        
-        Unofficial Pinterest API implemented in python 3 that can do all Pinterest tasks like comment, pin, repin, follow, unfollow and more.
-        
-        It is implemented by directly calling the pinterest servers, mimicking an actual browser, so you don't need pinterest API key.
-        
-        If you see any issues, or find bugs feel free to report them here on the github repo.
-        
-        ## Community guides
-        [Get started with pinterest automation](https://martechwithme.com/how-to-automate-pinterest-interactions-python "Martechwithme.com")
-        
-        [Automated posting to Pinterest (in Russian)](https://www.youtube.com/watch?v=TQBceIiv_Gk&ab_channel=Analitiq "Analitiq YouTube")
-        
-        
-        ## Install using pip
-        ```pip install py3-pinterest```
-        
-        
-        ### NOTE: for each of the functionalities listed below there is a working example under the project root.
-        
-        ### Create new instance of the API
-        
-        ```pinterest = Pinterest(email='your email goes here', password='password goes here', username='look in pinterest url', cred_root='cred root dir')```
-        
-        cred_root is the dir (automatically created if missing) that will store some cookies nad sessions, so you don't need to login before each request.
-        Make sure you specify a path with read/write permissions.
-        
-        Proxies example:
-        
-        ```
-        proxies = {"http":"http://username:password@proxy_ip:proxy_port"}
-        Pinterest(email='emai', password='pass', username='name', cred_root='cred_root', proxies=proxies)
-        ```
-        
-        # The following features are currently supported
-        
-        ## Login/Logout
-        ## NOTE: Pinterest integrated google recaptcha. This means we have to use web driver to login. For that reason you must have chrome installed on you computer, in order for the login to work.
-        ### If you want to use many accounts, you should associate proxy with each one of them and login only with that proxy
-        ### pinterest.login(proxy='ip_address:port')
-        Login will store auth cookies for later use. These cookies are usually valid for ~15 days, then you will start getting 403 and 401 errors, which means you need to call login again. 
-        ## Login
-        Login is required to permit actions to the Pinterest servers. Login will store auth cookies for later use. These cookies are usually valid for ~15 days, then you will start getting 403 and 401 errors, which means you need to call login again. 
-        
-        ```pinterest.login()```
-        
-        ```pinterest.logout()```
-        
-        
-        
-        ## Load profile
-        You can load profile for currently logged in user or any user specified by username.
-        
-        ```user_profile = pinterest.get_user_overview()```
-        
-        
-        ## Board and pin management
-        
-        ### Get all boards of user:
-        
-        ```boards = pinterest.boards(username='username')```
-        
-        ### List all pins in board
-        ```pins = pinterest.board_feed(board_id=board_id)```
-        
-        If username is left blank, current logged in user will be used.
-        
-        
-        ### Delete pin
-        ```pinterest.delete_pin(pin_id='pin_id')```
-        
-        ### Repin
-        
-        ```pinterest.repin(board_id='board_id', pin_id='pin_id')```
-        
-        ### Get ID of created pin, section, or board
-        
-        All functions return the post/get data from the request. If you dig a little deeper by going myrequest.content you get the actual HTML response, which can then be turned into a dict by using JSON.
-        
-        Example:
-        
-        ```py
-        import json
-        
-        pin_response = upload_pin(board_id='',
-                     image_path='test.png',
-                     description='TESTING PIN FUNCTIONALITY WITH ID FETCHING',
-                     title='Foobar Barfood',
-                     section_id=None,
-                     link='')
-        
-        response_data = json.loads(pin_response.content)
-        ```
-        
-        Some helpful notes on the response:
-        Everything is stored inside the "resource_response" key. You can use that and grab all sorts of data like so:
-        
-        ```py
-        # This is how you would access this information when creating a pin
-        
-        id = response_data["resource_response"]["data"]["id"]
-        board_id = response_data["resource_response"]["data"]["board"]["id"]
-        section_id = response_data["resource_response"]["data"]["section"]["id"]
-        pinner_username = response_data["resource_response"]["data"]["pinner"]["username"]
-        pinner_id = response_data["resource_response"]["data"]["pinner"]["id"]
-        
-        # If you wanted to access this information in a different circumstance,
-        # keep in mind that whatever your creating should be the first level under "data"
-        # I.e, I created a board, and I want to get the board ID. It would now be:
-        
-        board_id = response_data["resource_response"]["data"]["id"]
-        ```
-        
-        ### Get pinnable images
-        A pinterest feature they use to pin from websites
-        
-        ```pinterest.get_pinnable_images(url='https://www.tumblr.com/search/food')```
-        
-        ### Pin
-        
-        Pin image by web url:
-        
-        ```pinterest.pin(board_id=board_id, image_url=image_url, description=description, title=title)```
-        
-        Pin image from local file:
-        
-        ```pinterest.upload_pin(board_id=board_id, section_id=section_id, image_file=image_path, description=description, title=title, link=link)```
-        
-        ### Get home feed pins
-        
-        ``` home_feed_batch = pinterest.home_feed()```
-        
-        ### Get board recommendations (this is the 'more ideas' api)
-        
-        ```rec_batch = pinterest.board_recommendations(board_id=board_id)```
-        
-        ### Get pin information by id
-        
-        ```pinterest.load_pin(pin_id='pin_id')```
-        
-        ### Board Section support
-        ```pinterest.create_board_section(board_id=board_id, section_name=section_name)```
-        ```pinterest.delete_board_section(section_id=section_id)```
-        ```pinterest.get_board_sections(board_id=board_id)```
-        
-        You can also pin and repin to sections.
-        
-        
-        ## Follow/Unfollow
-        
-        ### Follow
-        ```pinterest.follow_user(user_id='target_user_id', username='target_username')```
-        
-        Follow limit is 300 per day, after that they might place you on watch list
-        
-        
-        ### Unfollow
-        
-        ```pinterest.unfollow_user(user_id='target_user_id', username='target_username')```
-        
-        Unfollow limit is 350 per day, after that they might place you on watch list
-        
-        ### Get following
-        
-        ```following_batch = pinterest.get_following(username='some_user')```
-        
-        If username is not provided current user will be used
-        
-        ### Get followers
-        
-        ```followers_batch=pinterest.get_user_followers(username='some_user')```
-        
-        If username is not provided current user will be used
-        
-        ### Follow board
-        
-        ```pinterest.follow_board(board_id=board_id)```
-        
-        ### Unfollow board
-        
-        ```pinterest.unfollow_board(board_id=board_id)```
-        
-        
-        ## Search
-        
-        ```search_batch = pinterest.search(scope='boards', query='food')```
-        
-        Current pinterest scopes are: pins, buyable_pins, my_pins, videos, boards
-        
-        ### Visual Search
-        
-        ```
-          pin_data = pinterest.load_pin(pin_id='pin_id')
-          search_batch = pinterest.visual_search(pin_data, x=10, y=50, w=100, h=100)
-        ```
-        ## User interactions
-        ### Invite to board
-        
-        ```pinterest.invite(board_id=board_id, user_id=target_user_id)```
-        
-        ### Delete board invite
-        
-        ```pinterest.delete_invite(board_id=board_id, invited_user_id=target_user_id)```
-        
-        ### Get board invites
-        
-        ```invites_batch = pinterest.get_board_invites(board_id=board_id)```
-        
-        ### Comment
-        
-        ```pinterest.comment(pin_id=pin_id, text=comment_text)```
-        
-        ### Delete comment 
-        ```pinterest.delete_comment(pin_id=pin_id, comment_id=comment_id)```
-        
-        ### Get Pin comments
-        
-        ```pinterest.get_comments(pin_id='pin_id')```
-        
-        
-        ### Send personal message
-        ```pinterest.send_message(conversation_id=conversation_id, pin_id="(pin_id)", message="hey")```
-        
-        
-        ### Access to type suggestions you see in the search input
-        ```pinterest.type_ahead(term='apple')```
-        
-        
-        
-        
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.5.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: beautifulsoup4
+Requires-Dist: requests-toolbelt
+Requires-Dist: selenium
+Requires-Dist: webdriver-manager
+
+
+# py3-pinterest
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+Unofficial Pinterest API implemented in python 3 that can do all Pinterest tasks like comment, pin, repin, follow, unfollow, and more.
+
+It is implemented by directly calling the pinterest servers, mimicking an actual browser, so you don't need pinterest API key.
+
+If you see any issues, or find bugs feel free to report them here on the github repo.
+
+## Community guides
+[Get started with pinterest automation](https://martechwithme.com/how-to-automate-pinterest-interactions-python "Martechwithme.com")
+
+[Automated posting to Pinterest (in Russian)](https://www.youtube.com/watch?v=TQBceIiv_Gk&ab_channel=Analitiq "Analitiq YouTube")
+
+
+## Install using pip
+```pip install py3-pinterest```
+
+
+### NOTE: for each of the functionalities listed below there is a working example under the project root.
+
+### Create new instance of the API
+
+```pinterest = Pinterest(email='your email goes here', password='password goes here', username='look in pinterest url', cred_root='cred root dir')```
+
+cred_root is the dir (automatically created if missing) that will store some cookies and sessions, so you don't need to login before each request.
+Make sure you specify a path with read/write permissions.
+
+Proxies example:
+
+```
+proxies = {"http":"http://username:password@proxy_ip:proxy_port"}
+Pinterest(email='emai', password='pass', username='name', cred_root='cred_root', proxies=proxies)
+```
+
+# The following features are currently supported
+
+## Login/Logout
+## NOTE: Pinterest integrated google recaptcha. This means we have to use web driver to login. For that reason you must have chrome installed on you computer, in order for the login to work.
+### If you want to use many accounts, you should associate proxy with each one of them and login only with that proxy
+### pinterest.login(proxy='ip_address:port')
+Login will store auth cookies for later use. These cookies are usually valid for ~15 days, then you will start getting 403 and 401 errors, which means you need to call login again. 
+## Login
+Login is required to permit actions to the Pinterest servers. Login will store auth cookies for later use. These cookies are usually valid for ~15 days, then you will start getting 403 and 401 errors, which means you need to call login again. 
+
+```pinterest.login()```
+
+```pinterest.logout()```
+
+
+
+## Load profile
+You can load profile for currently logged in user or any user specified by username.
+
+```user_profile = pinterest.get_user_overview()```
+
+
+## Board and pin management
+
+### Get all boards of user:
+
+```boards = pinterest.boards(username='username')```
+
+### List all pins in board
+```pins = pinterest.board_feed(board_id=board_id)```
+
+If username is left blank, current logged in user will be used.
+
+
+### Delete pin
+```pinterest.delete_pin(pin_id='pin_id')```
+
+### Repin
+
+```pinterest.repin(board_id='board_id', pin_id='pin_id')```
+
+### Get ID of created pin, section, or board
+
+All functions return the post/get data from the request. If you dig a little deeper by going myrequest.content you get the actual HTML response, which can then be turned into a dict by using JSON.
+
+Example:
+
+```py
+import json
+
+pin_response = upload_pin(board_id='',
+             image_path='test.png',
+             description='TESTING PIN FUNCTIONALITY WITH ID FETCHING',
+             title='Foobar Barfood',
+             section_id=None,
+             link='')
+
+response_data = json.loads(pin_response.content)
+```
+
+Some helpful notes on the response:
+Everything is stored inside the "resource_response" key. You can use that and grab all sorts of data like so:
+
+```py
+# This is how you would access this information when creating a pin
+
+id = response_data["resource_response"]["data"]["id"]
+board_id = response_data["resource_response"]["data"]["board"]["id"]
+section_id = response_data["resource_response"]["data"]["section"]["id"]
+pinner_username = response_data["resource_response"]["data"]["pinner"]["username"]
+pinner_id = response_data["resource_response"]["data"]["pinner"]["id"]
+
+# If you wanted to access this information in a different circumstance,
+# keep in mind that whatever you are creating should be the first level under "data"
+# I.e, I created a board, and I want to get the board ID. It would now be:
+
+board_id = response_data["resource_response"]["data"]["id"]
+```
+
+### Get pinnable images
+A pinterest feature they use to pin from websites
+
+```pinterest.get_pinnable_images(url='https://www.tumblr.com/search/food')```
+
+### Pin
+
+Pin image by web url:
+
+```pinterest.pin(board_id=board_id, image_url=image_url, description=description, title=title)```
+
+Pin image from local file:
+
+```pinterest.upload_pin(board_id=board_id, section_id=section_id, image_file=image_path, description=description, title=title, link=link)```
+
+### Get home feed pins
+
+``` home_feed_batch = pinterest.home_feed()```
+
+### Get board recommendations (this is the 'more ideas' api)
+
+```rec_batch = pinterest.board_recommendations(board_id=board_id)```
+
+### Get pin information by id
+
+```pinterest.load_pin(pin_id='pin_id')```
+
+### Board Section support
+```pinterest.create_board_section(board_id=board_id, section_name=section_name)```
+```pinterest.delete_board_section(section_id=section_id)```
+```pinterest.get_board_sections(board_id=board_id)```
+
+You can also pin and repin to sections.
+
+
+## Follow/Unfollow
+
+### Follow
+```pinterest.follow_user(user_id='target_user_id', username='target_username')```
+
+Follow limit is 300 per day, after that they might place you on a watch list
+
+
+### Unfollow
+
+```pinterest.unfollow_user(user_id='target_user_id', username='target_username')```
+
+Unfollow limit is 350 per day, after that they might place you on a watch list
+
+### Get following
+
+```following_batch = pinterest.get_following(username='some_user')```
+
+If username is not provided current user will be used
+
+### Get followers
+
+```followers_batch=pinterest.get_user_followers(username='some_user')```
+
+If username is not provided current user will be used
+
+### Follow board
+
+```pinterest.follow_board(board_id=board_id)```
+
+### Unfollow board
+
+```pinterest.unfollow_board(board_id=board_id)```
+
+
+## Search
+
+```search_batch = pinterest.search(scope='boards', query='food')```
+
+Current pinterest scopes are: pins, buyable_pins, my_pins, videos, boards
+
+### Visual Search
+
+```
+  pin_data = pinterest.load_pin(pin_id='pin_id')
+  search_batch = pinterest.visual_search(pin_data, x=10, y=50, w=100, h=100)
+```
+## User interactions
+### Invite to board
+
+```pinterest.invite(board_id=board_id, user_id=target_user_id)```
+
+### Delete board invite
+
+```pinterest.delete_invite(board_id=board_id, invited_user_id=target_user_id)```
+
+### Get board invites
+
+```invites_batch = pinterest.get_board_invites(board_id=board_id)```
+
+### Comment
+
+```pinterest.comment(pin_id=pin_id, text=comment_text)```
+
+### Delete comment 
+```pinterest.delete_comment(pin_id=pin_id, comment_id=comment_id)```
+
+### Get Pin comments
+
+```pinterest.get_comments(pin_id='pin_id')```
+
+
+### Send personal message
+```pinterest.send_message(conversation_id=conversation_id, pin_id="(pin_id)", message="hey")```
+
+
+### Access to type suggestions you see in the search input
+```pinterest.type_ahead(term='apple')```
+
```

### Comparing `py3-pinterest-1.3.0/py3pin/BookmarkManager.py` & `py3_pinterest-1.4.0/py3pin/BookmarkManager.py`

 * *Files identical despite different names*

### Comparing `py3-pinterest-1.3.0/py3pin/Pinterest.py` & `py3_pinterest-1.4.0/py3pin/Pinterest.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 from requests_toolbelt import MultipartEncoder
 from bs4 import BeautifulSoup
 from py3pin.BookmarkManager import BookmarkManager
 from py3pin.Registry import Registry
 from py3pin.RequestBuilder import RequestBuilder
 from requests.structures import CaseInsensitiveDict
 from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
+from selenium.webdriver import ChromeOptions
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.proxy import Proxy, ProxyType
+from selenium.webdriver.chrome.service import Service
+from selenium.webdriver.common.by import By
+
 
 AGENT_STRING = (
     "Mozilla/5.0 (Windows NT 6.1; Win64; x64) "
     "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/61.0.3163.100 Safari/537.36"
 )
 
 # Pinterest endpoints
@@ -174,45 +177,44 @@
         )
 
     def login(self, headless=True, wait_time=15, proxy=None, lang="en"):
         """
         Logs user in with the provided credentials
         User session is stored in the 'cred_root' folder
         and reused so there is no need to login every time.
-        Pinterest sessions lasts for about 15 days
+        Pinterest sessions last for about 15 days
         Ideally you need to call this method 3-4 times a month at most.
         :return python dict object describing the pinterest response
         """
-        chrome_options = Options()
-        chrome_options.add_argument("--lang=%s" % lang)
+        chrome_options = ChromeOptions()
+        chrome_options.add_experimental_option('prefs', {'intl.accept_languages': lang})
         if headless:
             chrome_options.add_argument("--headless")
 
         if proxy is not None:
             http_proxy = Proxy()
             http_proxy.proxy_type = ProxyType.MANUAL
             http_proxy.http_proxy = proxy
             http_proxy.socks_proxy = proxy
             http_proxy.ssl_proxy = proxy
             http_proxy.add_to_capabilities(chrome_options)
 
-        driver = webdriver.Chrome(
-            ChromeDriverManager().install(), options=chrome_options
-        )
+        driver = webdriver.Chrome(options=chrome_options)
         driver.get("https://pinterest.com/login")
 
         try:
             WebDriverWait(driver, wait_time).until(
                 EC.element_to_be_clickable((By.ID, "email"))
             )
 
-            driver.find_element_by_id("email").send_keys(self.email)
-            driver.find_element_by_id("password").send_keys(self.password)
+            driver.find_element(by = By.ID, value='email').send_keys(self.email)
+            driver.find_element(by= By.ID, value="password").send_keys(self.password)
+
+            logins = driver.find_elements(by=By.XPATH, value="//*[contains(text(), 'Log in')]")
 
-            logins = driver.find_elements_by_xpath("//*[contains(text(), 'Log in')]")
 
             for login in logins:
                 login.click()
 
             WebDriverWait(driver, wait_time).until(
                 EC.invisibility_of_element((By.ID, "email"))
             )
@@ -220,23 +222,25 @@
             cookies = driver.get_cookies()
 
             self.http.cookies.clear()
             for cookie in cookies:
                 self.http.cookies.set(cookie["name"], cookie["value"])
 
             self.registry.update_all(self.http.cookies.get_dict())
+
+            print("Successfully logged in with account " + self.email)
         except Exception as e:
             print("Failed to login", e)
 
-        print("Successfully logged in with account " + self.email)
         driver.close()
 
     def logout(self):
         """
-        Logs current user out. Takes few seconds for the session to be invalidated on pinterest's side
+        Logs the current user out.
+        Takes a few seconds for the session to be invalidated on pinterest's side
         """
         options = {"disable_auth_failure_redirect": True}
 
         data = self.req_builder.buildPost(options=options)
         return self.post(url=DELETE_USER_SESSION, data=data)
 
     def get_board_followers(self, board_id, page_size=50, source_url=None):
@@ -278,29 +282,37 @@
             "field_set_key": "profile",
         }
         url = self.req_builder.buildGet(url=USER_RESOURCE, options=options)
         result = self.get(url=url).json()
 
         return result["resource_response"]["data"]
 
-    def boards(self, username=None, page_size=50):
+    def boards(self, username=None, page_size=50, reset_bookmark=False):
         """
         The data returned is chunked, this comes from pinterest's rest api.
-        Some users might have huge number of boards that is why it make sense to chunk the data.
-        In order to obtain all boards this method needs to be called until it returns empty list
-        :param username: target username, if left blank current user is assumed
+        This method is batched. In order to obtain all boards
+        you need to call it until an empty list is returned.
+        :param username: target username. If left blank, the current user is assumed
         :param page_size: controls the batch size for each request
         :return python dict describing all the boards of a user.
         """
         if username is None:
             username = self.username
 
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="boards", secondary=username
         )
+
+        if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(
+                    primary="boards", secondary=username
+                )
+            return []
+
         options = {
             "page_size": page_size,
             "privacy_filter": "all",
             "sort": "custom",
             "username": username,
             "isPrefetch": False,
             "include_archived": True,
@@ -334,62 +346,64 @@
         board_batch = self.boards(username=username)
         while len(board_batch) > 0:
             boards += board_batch
             board_batch = self.boards(username=username)
 
         return boards
 
-    def get_user_pins(self, username=None, page_size=250):
+    def get_user_pins(self, username=None, page_size=250, reset_bookmark=False):
         """
         Obtains all the pins of a user.
-        This method is batched, meaning in order to obtain all pins you need
-        to call it until empty list is returned.
+        This method is batched. In order to obtain all pins
+        you need to call it until an empty list is returned.
         :return all pins under all pins board
         :param username: target user, if left blank current user is assumed
         """
         if username is None:
             username = self.username
-            own_profile = True 
+            own_profile = True
         else:
             own_profile = False
 
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="pins", secondary=username
         )
 
         if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(primary="pins", secondary=username)
             return []
 
         options = {
             "username": username,
             "is_own_profile_pins": own_profile,
             "field_set_key": "grid_item",
-            "pin_filter": None,  
+            "pin_filter": None,
             "bookmarks": [next_bookmark],
             "page_size": page_size,
         }
         url = self.req_builder.buildGet(url=USER_PIN_RESOURCE, options=options)
 
         response = self.get(url=url).json()
         bookmark = response["resource"]["options"]["bookmarks"][0]
         self.bookmark_manager.add_bookmark(
-            primary="board_feed", secondary=username, bookmark=bookmark
+            primary="pins", secondary=username, bookmark=bookmark
         )
 
         return response["resource_response"]["data"]
 
     def create_board(
         self, name, description="", category="other", privacy="public", layout="default"
     ):
         """
         Creates a new board and returns the response from pinterest.
         :param name: board name (should be unique per user)
         :param description: board description
         :param category: if you have defined categories (it is not visible to external users)
-        :param privace: can be public or private
+        :param privacy: can be public or private
         :param layout: looks like a legacy parameter but it is mandatory (can be left as default)
         """
         options = {
             "name": name,
             "description": description,
             "category": category,
             "privacy": privacy,
@@ -410,15 +424,15 @@
         """
         options = {"board_id": board_id}
         data = self.req_builder.buildPost(options=options)
         return self.post(url=FOLLOW_BOARD_RESOURCE, data=data)
 
     def unfollow_board(self, board_id):
         """
-        UnFollows a board with current user.
+        Unfollows a board with current user.
         :param board_id: the id of the board to follow
         :return python dict with the pinterest response
         """
         options = {"board_id": board_id}
         data = self.req_builder.buildPost(options=options)
         return self.post(url=UNFOLLOW_BOARD_RESOURCE, data=data)
 
@@ -430,38 +444,43 @@
         """
         options = {"user_id": user_id}
         data = self.req_builder.buildPost(options=options)
         return self.post(url=FOLLOW_USER_RESOURCE, data=data)
 
     def unfollow_user(self, user_id):
         """
-        UnFollows a user with current user.
+        Unfollows a user with current user.
         :param user_id: the id of the user to follow
         :return python dict with the pinterest response
         """
         options = {"user_id": user_id}
         data = self.req_builder.buildPost(options=options)
         return self.post(url=UNFOLLOW_USER_RESOURCE, data=data)
 
-    def get_following(self, username=None, page_size=250):
+    def get_following(self, username=None, page_size=250, reset_bookmark=False):
         """
         Get all users following this particular user.
-        The response of this method is batched, meaning it needs to be called
-        until empty list is returned
+        This method is batched. In order to obtain all following users
+        you need to call it until an empty list is returned.
         :param username: target user, if left blank current user is assumed
         :param page_size:
         :return: python dict describing the 'following' list
         """
         if username is None:
             username = self.username
 
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="following", secondary=username
         )
+
         if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(
+                    primary="following", secondary=username
+                )
             return []
 
         source_url = "/{}/_following/".format(self.email)
         options = {
             "isPrefetch": "false",
             "hide_find_friends_rep": "false",
             "username": username,
@@ -498,30 +517,35 @@
         following_batch = self.get_following(username=username)
         while len(following_batch) > 0:
             following += following_batch
             following_batch = self.get_following(username=username)
 
         return following
 
-    def get_user_followers(self, username=None, page_size=250):
+    def get_user_followers(self, username=None, page_size=250, reset_bookmark=False):
         """
         Obtains a list of user's followers.
-        The response from this method is batched, meaning it needs to be called until empty list is returned.
+        This method is batched. In order to obtain all user followers
+        you need to call it until an empty list is returned.
         :param username: target username, is left blank current user is assumed
         :param page_size: batch size
         :return: python dict describing user followers
         """
         if username is None:
             username = self.username
 
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="followers", secondary=username
         )
 
         if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(
+                    primary="followers", secondary=username
+                )
             return []
 
         options = {
             "isPrefetch": False,
             "hide_find_friends_rep": True,
             "username": username,
             "page_size": page_size,
@@ -559,24 +583,32 @@
         while len(followers_batch) > 0:
             followers += followers_batch
             followers_batch = self.get_user_followers(username=username)
 
         return followers
 
     def pin(
-        self, board_id, image_url, description="", link="", title="", alt_text="", section_id=None
+        self,
+        board_id,
+        image_url,
+        description="",
+        link="",
+        title="",
+        alt_text="",
+        section_id=None,
     ):
         """
-        Perfoms a pin operation. If you want to upload local image use 'upload_pin'
+        Perfoms a pin operation.
+        If you want to upload a local image use 'upload_pin'
         :param board_id: id of the target board (current user should have rights to pin to it)
         :param image_url: web url of an image (not local one)
-        :param description: pin description (can be blank)
-        :param link: link to include (can be blank)
+        :param description: pin description. Optional
+        :param link: link to include. Optional
         :param title: title can be blank
-        :param section_id: board section should be previously defined and its optional
+        :param section_id: board section should be previously defined. Optional
         :return: python dict describing the pinterest response
         """
         options = {
             "board_id": board_id,
             "image_url": image_url,
             "description": description,
             "link": link if link else image_url,
@@ -588,35 +620,36 @@
         }
         source_url = "/pin/find/?url={}".format(self.req_builder.url_encode(image_url))
         data = self.req_builder.buildPost(options=options, source_url=source_url)
 
         return self.post(url=PIN_RESOURCE_CREATE, data=data)
 
     def upload_pin(
-        self, board_id, image_file, description="", link="", title="", section_id=None
+        self, board_id, image_file, description="", link="", title="", alt_text = "", section_id=None
     ):
         """
-        This method is simmilar to 'pin' except the image for the pin is local file.
+        This method is similar to 'pin' except the image for the pin is a local file.
         """
         image_url = self._upload_image(image_file=image_file).json()["image_url"]
         return self.pin(
             board_id=board_id,
             description=description,
             image_url=image_url,
             link=link,
             title=title,
+            alt_text=alt_text,
             section_id=section_id,
         )
 
     def repin(self, board_id, pin_id, section_id=None):
         """
         Repin/Save action
         :param board_id: board id, current user should have right to pin to this board
         :param pin_id: pin id to repin
-        :param section_id:  board section should be previously defined and its optional
+        :param section_id:  board section should be previously defined. Optional
         :return: python dict describing the pinterest response
         """
         options = {
             "board_id": board_id,
             "pin_id": pin_id,
             "section": section_id,
             "is_buyable_pin": False,
@@ -639,15 +672,15 @@
             "X-UPLOAD-SOURCE": "pinner_uploader",
         }
 
         return self.post(url=UPLOAD_IMAGE, data=form_data, headers=headers)
 
     def delete_pin(self, pin_id):
         """
-        Deletes a pint the user owns
+        Deletes a pin the user owns
         :param pin_id: pin id to delete
         :return: python dict describing the pinterest response
         """
         options = {"id": pin_id}
         source_url = "/{}/".format(self.username)
         data = self.req_builder.buildPost(options=options, source_url=source_url)
         return self.post(url=DELETE_PIN_RESOURCE, data=data)
@@ -675,38 +708,44 @@
         Loads full information about a pin
         :param pin_id: pin id to load
         :return: python dict describing the pinterest response
         """
         resp = self.get(url=LOAD_PIN_URL_FORMAT.format(pin_id))
         soup = BeautifulSoup(resp.text, "html.parser")
         scripts = soup.findAll("script")
-        pin_data = {}
+        pin_data = None
         for s in scripts:
-            if 'id' in s.attrs and s.attrs['id'] == '__PWS_DATA__':
-                pinJsonData = json.loads(s.contents[0])['props']['initialReduxState']['resources']['PinResource']
-                pinJsonData = pinJsonData[list(pinJsonData.keys())[0]]['data']
-                return pinJsonData
+            if "data-relay-response" in s.attrs and s.attrs["data-relay-response"] == "true":
+                pinJsonData = json.loads(s.contents[0])["response"]["data"]["v3GetPinQuery"]["data"]
+                pin_data = pinJsonData
+        if pin_data:
+            return pin_data
 
         raise Exception("Pin data not found. Probably pintereset chagned their API")
 
-    def get_comments(self, pin_id, page_size=50):
+    def get_comments(self, pin_id, page_size=50, reset_bookmark=False):
         """
         Get comments on a pin.
-        The response is batched, meaning this method should be called util empty list is returned
+        This method is batched. In order to obtain all comments
+        you need to call it until an empty list is returned.
         :param pin_id: target pin id
         :param page_size:  batch size
         :return: list of comment objects
         """
         pin_data = self.load_pin(pin_id=pin_id)
 
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="pin_comments", secondary=pin_id
         )
 
         if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(
+                    primary="pin_comments", secondary=pin_id
+                )
             return []
 
         options = {
             "isPrefetch": False,
             "objectId": pin_data["aggregated_pin_data"]["id"],
             "page_size": page_size,
             "redux_normalize_feed": True,
@@ -728,15 +767,15 @@
         )
 
         return resp["data"]
 
     def get_comments_all(self, pin_id):
         """
         Obtains all comments of a pin.
-        NOTE: IF pin has too many comments this might cause memory issues.
+        NOTE: If pin has too many comments this might cause memory issues.
         In such cases use 'get_comments' which is batched
         :param pin_id:
         :return: list of comment objects
         """
         results = []
         search_batch = self.get_comments(pin_id=pin_id)
         while len(search_batch) > 0:
@@ -767,15 +806,16 @@
         options = {"board_id": board_id, "invited_user_ids": [user_id]}
         data = self.req_builder.buildPost(options=options)
         return self.post(url=BOARD_INVITE_RESOURCE, data=data)
 
     def get_board_invites(self, board_id, page_size=100):
         """
         Returns a list of users invited to the specified board.
-        This method is batched and needs to be called until empty list is returned.
+        This method is batched. In order to obtain all board invites
+        you need to call it until an empty list is returned.
         :param board_id: id of target board
         :param page_size: batch size
         :return: list of board objects
         """
         options = {
             "isPrefetch": False,
             "board_id": board_id,
@@ -820,18 +860,21 @@
             "board_id": board_id,
             "field_set_key": "boardEdit",
             "invited_user_id": invited_user_id,
         }
         data = self.req_builder.buildPost(options=options)
         return self.post(url=BOARD_DELETE_INVITE_RESOURCE, data=data)
 
-    def visual_search(self, pin_data, x=None, y=None, w=None, h=None, padding=10):
+    def visual_search(
+        self, pin_data, x=None, y=None, w=None, h=None, padding=10, reset_bookmark=False
+    ):
         """
         Gives access to pinterest search api
-        This method is batched, meaning is needs to be called until empty list is returned.
+        This method is batched. In order to obtain all search results
+        you need to call it until an empty list is returned.
         :param pin_data: pin data
         :param x: x position of the cropped part of the image used for searching
         :param y: y position of the cropped part of the image used for searching
         :param w: width of the cropped part of the image used for searching
         :param h: height of the cropped part of the image used for searching
         :param padding: Default padding for cropped image.
 
@@ -853,14 +896,18 @@
             pin_id, x, y, w, h
         )
 
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="visual_search", secondary=source_url
         )
         if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(
+                    primary="visual_search", secondary=source_url
+                )
             return []
 
         options = {
             "isPrefetch": False,
             "pin_id": pin_id,
             "image_signature": image_signature,
             "crop": {"x": x / width, "y": y / height, "w": w / width, "h": h / height},
@@ -876,30 +923,33 @@
 
         self.bookmark_manager.add_bookmark(
             primary="visual_search", secondary=source_url, bookmark=bookmark
         )
 
         return resp["resource_response"]["data"]["results"]
 
-    def search(self, scope, query, page_size=250):
+    def search(self, scope, query, page_size=250, reset_bookmark=False):
         """
         Gives access to pinterest search api
-        This method is batched, meaning is needs to be called until empty list is returned.
+        This method is batched. In order to obtain all search results
+        you need to call it until an empty list is returned.
         NOTE: there is a max number of results set by Pinterest -> 1000
-        :param scope: can be pins, buyable_pins, my_pins, videos, boards
+        :param scope: can be pins, buyable_pins, my_pins, videos, or boards
         :param query: search phrase
         :param page_size: batch size
         :return: list of search results
         """
 
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="search", secondary=query
         )
 
         if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(primary="search", secondary=query)
             return []
 
         terms = query.split(" ")
         escaped_query = "%20".join(terms)
         term_meta_arr = []
         for t in terms:
             term_meta_arr.append("term_meta[]=" + t)
@@ -925,28 +975,32 @@
         bookmark = resp["resource"]["options"]["bookmarks"][0]
 
         self.bookmark_manager.add_bookmark(
             primary="search", secondary=query, bookmark=bookmark
         )
         return resp["resource_response"]["data"]["results"]
 
-    def board_recommendations(self, board_id="", page_size=50):
+    def board_recommendations(self, board_id="", page_size=50, reset_bookmark=False):
         """
         This gives the list of pins you see when you open a board and click on 'More Ideas'
-        This method is batched and needs to be called until empty list is returned in order to obtain all
-        of the results.
+        This method is batched. In order to obtain all board recommendations
+        you need to call it until an empty list is returned.
         :param board_id: target board id
         :param page_size: batch size
-        :return:
+        :return: list of board recommendations
         """
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="boards", secondary=board_id
         )
 
         if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(
+                    primary="boards", secondary=board_id
+                )
             return []
 
         options = {
             "isPrefetch": False,
             "type": "board",
             "id": board_id,
             "page_size": page_size,
@@ -981,24 +1035,26 @@
         res = res["resource_response"]["data"]["items"]
         urls = []
         for item in res:
             if "url" in item:
                 urls.append(item["url"])
         return urls
 
-    def home_feed(self, page_size=100):
+    def home_feed(self, page_size=100, reset_bookmark=False):
         """
         This gives the list of pins you see when you open the pinterest home page.
-        This method is batched, in order to obtain all home feed items
-        it needs to be called until empty list is returned
+        This method is batched. In order to obtain all home feed items
+        you need to call it until an empty list is returned.
         :param page_size:
         :return:
         """
         next_bookmark = self.bookmark_manager.get_bookmark(primary="home_feed")
         if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(primary="home_feed")
             return []
 
         options = {
             "bookmarks": [next_bookmark],
             "isPrefetch": False,
             "field_set_key": "hf_grid_partner",
             "in_nux": False,
@@ -1016,25 +1072,29 @@
         if "bookmark" in response["resource_response"]:
             bookmark = response["resource_response"]["bookmark"]
 
         self.bookmark_manager.add_bookmark(primary="home_feed", bookmark=bookmark)
 
         return response["resource_response"]["data"]
 
-    def board_feed(self, board_id="", page_size=250):
+    def board_feed(self, board_id="", page_size=250, reset_bookmark=False):
         """
         Gives a list of all pins in a board.
-        This method is batched, meaning in order to obtain all pins in a board you need
-        to call it until empty list is returned.
+        This method is batched. In order to obtain all pins in a board
+        you need to call it until an empty list is returned.
         """
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="board_feed", secondary=board_id
         )
 
         if next_bookmark == "-end-":
+            if reset_bookmark:
+                self.bookmark_manager.reset_bookmark(
+                    primary="board_feed", secondary=board_id
+                )
             return []
 
         options = {
             "isPrefetch": False,
             "board_id": board_id,
             "field_set_key": "partner_react_grid_pin",
             "filter_section_pins": True,
@@ -1187,16 +1247,16 @@
         )
 
         return response["resource_response"]["data"]
 
     def get_section_pins(self, section_id="", page_size=250, reset_bookmark=False):
         """
         Returns a list of all pins in a board section.
-        This method is batched meaning in order to obtain all pins in the section
-        you need to call is until empty list is returned
+        This method is batched. In order to obtain all pins in the section
+        you need to call it until an empty list is returned.
         """
         next_bookmark = self.bookmark_manager.get_bookmark(
             primary="section_pins", secondary=section_id
         )
         if next_bookmark == "-end-":
             if reset_bookmark:
                 self.bookmark_manager.reset_bookmark(
@@ -1233,15 +1293,15 @@
         return self.post(url=BOARD_SECTION_EDIT_RESOURCE, data=data)
 
     def type_ahead(self, scope="pins", count=5, term=""):
         """
         returns Pinterest predictions for given term.
         Response may include user profiles.
         Example term "dada" gives ["dadaism","dada art"] etc.
-        :param scope:  always "pins"
+        :param scope: always "pins"
         :param count: max guess number
         :param term: word to be typed ahead
         :return: response items
         """
 
         source_url = "/"
         options = {
@@ -1253,19 +1313,18 @@
         url = self.req_builder.buildGet(TYPE_AHEAD_RESOURCE, options, source_url)
 
         resp = self.get(url=url).json()
         return resp["resource_response"]["data"]["items"]
 
     def add_pin_note(self, pin_id, note):
         """
-          Adds a note to pin
+        Adds a note to a pin
         """
         options = {
             "url": "/v3/pins/{}/notes/".format(pin_id),
-            "data": {
-                "pin_note_content": note
-            }
+            "data": {"pin_note_content": note},
         }
 
-        data = self.req_builder.buildPost(options=options, source_url="/pin/{}/".format(pin_id))
+        data = self.req_builder.buildPost(
+            options=options, source_url="/pin/{}/".format(pin_id)
+        )
         return self.post(url=ADD_PIN_NOTE, data=data)
-
```

### Comparing `py3-pinterest-1.3.0/py3pin/Registry.py` & `py3_pinterest-1.4.0/py3pin/Registry.py`

 * *Files identical despite different names*

### Comparing `py3-pinterest-1.3.0/py3pin/RequestBuilder.py` & `py3_pinterest-1.4.0/py3pin/RequestBuilder.py`

 * *Files identical despite different names*

### Comparing `py3-pinterest-1.3.0/setup.py` & `py3_pinterest-1.4.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/profile-reddit-restapi-imp-local-0.0.35.tar.gz` & `tmp/profile_reddit_restapi_imp_local-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile-reddit-restapi-imp-local-0.0.35.tar", last modified: Tue Jan 30 10:18:35 2024, max compression
+gzip compressed data, was "profile_reddit_restapi_imp_local-0.0.36.tar", last modified: Thu May  9 00:13:34 2024, max compression
```

## Comparing `profile-reddit-restapi-imp-local-0.0.35.tar` & `profile_reddit_restapi_imp_local-0.0.36.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 10:18:35.025021 profile-reddit-restapi-imp-local-0.0.35/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-30 10:18:35.021021 profile-reddit-restapi-imp-local-0.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-30 10:18:03.000000 profile-reddit-restapi-imp-local-0.0.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 10:18:35.017021 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 10:18:35.021021 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-30 10:18:03.000000 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local/src/ProfileRedditConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 10:18:03.000000 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6740 2024-01-30 10:18:03.000000 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local/src/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-01-30 10:18:03.000000 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local/src/search_reddit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 10:18:35.021021 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-30 10:18:35.000000 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-01-30 10:18:35.000000 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 10:18:35.000000 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-30 10:18:35.000000 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-30 10:18:35.000000 profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-01-30 10:18:03.000000 profile-reddit-restapi-imp-local-0.0.35/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 10:18:35.025021 profile-reddit-restapi-imp-local-0.0.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-01-30 10:18:03.000000 profile-reddit-restapi-imp-local-0.0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:13:34.210774 profile_reddit_restapi_imp_local-0.0.36/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-09 00:13:34.210774 profile_reddit_restapi_imp_local-0.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-09 00:13:01.000000 profile_reddit_restapi_imp_local-0.0.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:13:34.206774 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:13:34.206774 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-09 00:13:01.000000 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local/src/ProfileRedditConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 00:13:01.000000 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-09 00:13:01.000000 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local/src/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-05-09 00:13:01.000000 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local/src/search_reddit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:13:34.210774 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-09 00:13:34.000000 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-09 00:13:34.000000 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:13:34.000000 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 00:13:34.000000 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-09 00:13:34.000000 profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-09 00:13:01.000000 profile_reddit_restapi_imp_local-0.0.36/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:13:34.210774 profile_reddit_restapi_imp_local-0.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-09 00:13:01.000000 profile_reddit_restapi_imp_local-0.0.36/setup.py
```

### Comparing `profile-reddit-restapi-imp-local-0.0.35/PKG-INFO` & `profile_reddit_restapi_imp_local-0.0.36/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: profile-reddit-restapi-imp-local
-Version: 0.0.35
+Version: 0.0.36
 Home-page: https://github.com/circles-zone/profile-reddit-restapi-imp-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: praw>=7.4.0
 Requires-Dist: tqdm>=4.64.1
-Requires-Dist: database-mysql-local>=0.0.11
-Requires-Dist: importer-local>=0.0.6
-Requires-Dist: logzio-python-handler>=4.1.0
-Requires-Dist: profiles-local>=0.0.11
-Requires-Dist: url-remote>=0.0.22
-Requires-Dist: python-dotenv>=1.0.0
-Requires-Dist: logger-local>=0.0.46
+Requires-Dist: requests
+Requires-Dist: data-source-local
 Requires-Dist: entity-type-local>=0.0.13
-Requires-Dist: group-remote>=0.0.85
-Requires-Dist: source-data-local>=0.0.3
+Requires-Dist: importer-local>=0.0.43
+Requires-Dist: location-local
+Requires-Dist: logger-local>=0.0.93
+Requires-Dist: profile-local>=0.0.61
+Requires-Dist: group-remote>=0.0.105
+Requires-Dist: python-sdk-remote>=0.0.65
+Requires-Dist: user-context-remote>=0.0.54
 
 Profile Reddit REST API Implementation Local Python Package
```

### Comparing `profile-reddit-restapi-imp-local-0.0.35/README.md` & `profile_reddit_restapi_imp_local-0.0.36/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Reddit Profile Importer
 
 With this importer you can import reddit profiles from specific subreddits and insert them into the database.
 
 ## Prerequisits
+
 You will need:
+
 * A reddit account
 * A reddit app, in order to get one, use this link : https://www.reddit.com/prefs/apps.
 * Here is a video tutorial for creating an app:
-    https://www.youtube.com/watch?v=4Lmfgw4RZCM
+  https://www.youtube.com/watch?v=4Lmfgw4RZCM
 
 * once you have the app, you will need to add to the python 2 enviorment variables:
-    REDDIT_CLIENT_ID: you can find the value under the app name at  https://www.reddit.com/prefs/apps
-    REDDIT_CLIENT_SECRET: also can be found in the app window you created
-    REDDIT_USERNAME: your reddit username
+  REDDIT_CLIENT_ID: you can find the value under the app name at  https://www.reddit.com/prefs/apps
+  REDDIT_CLIENT_SECRET: also can be found in the app window you created
+  REDDIT_USERNAME: your reddit username
+
+https://www.reddit.com/dev/api/<br>
```

### Comparing `profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local/src/handler.py` & `profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local/src/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,48 @@
+from data_source_local.data_source_enum import DataSource
+from entity_type_local.entity_enum import EntityTypeId
+from importer_local.ImportersLocal import ImportersLocal
 from location_local.location_local_constants import LocationLocalConstants
-from data_source_local.src.data_source_enum import DataSource
-from entity_type.entity_enum import EntityType
-from .search_reddit import Reddit
+from logger_local.LoggerComponentEnum import LoggerComponentEnum
+from logger_local.LoggerLocal import Logger
+from profile_local.comprehensive_profile import ComprehensiveProfileLocal
+from python_sdk_remote.utilities import get_brand_name, get_environment_name
+from user_context_remote.user_context import UserContext
+
 from .ProfileRedditConstants import (
     PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
     PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME
 )
-from logger_local.LoggerComponentEnum import LoggerComponentEnum
-import json
-from importer_local.ImportersLocal import ImportersLocal
-
-from dotenv import load_dotenv
-import sys
-import os
-sys.path.append(sys.path.append(os.getcwd()))
-load_dotenv()
-from logger_local.Logger import Logger  # noqa: E402
-from user_context_remote.user_context import UserContext  # noqa: E402
-from profiles_local.comprehensive_profile import ComprehensiveProfilesLocal  # noqa: E402
+from .search_reddit import Reddit
 
-BRAND_NAME = os.environ.get('BRAND_NAME')
-ENVIRONMENT_NAME = os.environ.get('ENVIRONMENT_NAME')
+BRAND_NAME = get_brand_name()
+ENVIRONMENT_NAME = get_environment_name()
 
 object_to_insert = {
     'component_id': PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
     'component_name': PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': 'yoav.e@circ.zone'
 }
 
 logger = Logger.create_logger(object=object_to_insert)
 
-user_context = UserContext.login_using_user_identification_and_password()
-
-
-if BRAND_NAME != 'Circlez':
-    error = "please add BRAND_NAME to be Circlez to .env"
-    logger.exception(error)
-    raise Exception(error)
-
-if ENVIRONMENT_NAME is None:
-    error = "please add ENVIRONMENT_NAME to .env"
-    logger.exception(error)
-    raise Exception(error)
+user_context = UserContext()
 
 
 # TODO Is it relevant to inherit Comprehensive Profile Class?
 class RedditImporter:
-    def __init__(self):
-        super().__init__()
+    def __init__(self, is_test_data: bool = False):
         self.importer = ImportersLocal()
         self.user = UserContext()
+        self.reddit = Reddit(is_test_data=is_test_data)
+        self.comprehensive_profile_local = ComprehensiveProfileLocal()
 
     # We don't use this method anymore
-    def process_reddit_user(reddit_user: dict) -> dict:
+    def process_reddit_user(self, reddit_user: dict) -> dict:
         logger.start(object={"reddit_user": reddit_user})
 
         comments = reddit_user['results']['profile']['comments']
         submissions = reddit_user['results']['profile']['submissions']
 
         comments_processed = []
         submissions_processed = []
@@ -79,15 +64,15 @@
     # This method gets data of reddit users and saves it to the database
     # event is a json formatted as such:
     # {
     #     "subreddit_name": "subreddit_name",
     #     "user_count": "user_count"
     # }
     # It gets input from stdin if event is None, the input is the subreddit name(the group) and the number of users to save
-    def handle(self, event: dict = None) -> None:
+    def handle(self, event: dict = None) -> list[int]:
         """
         purpose:
             collect data on reddit users for a certain subreddit
         args:
             event: None for manual input(terminal),
             or a json formatted as such:
             {
@@ -102,25 +87,25 @@
 
             main(None) asks for user input for subreddit name and user count
         """
 
         logger.start(object={"event": event})
 
         # collect the subreddit name and user count
-        reddit = Reddit()
-        subreddit_name, user_count = reddit.get_subreddit_and_query(event)
-        subreddit = reddit.reddit.subreddit(subreddit_name)
+        subreddit_name = event.get('subreddit_name')
+        user_count = int(event.get('user_count', float('inf')))
+        subreddit = self.reddit.subreddit(subreddit_name)
 
         ##########################################################################
         # Here we need to add the subreddit to the groups table in the database,
         # so we can later add the users to the users table with the group name
         # as a foreign key
         ##########################################################################
 
-        reddit_users_in_profile_json = reddit.get_reddit_users_by_subreddit(subreddit, user_count)
+        reddit_users_in_profile_json = self.reddit.get_reddit_users_by_subreddit(subreddit, user_count)
         inserted_ids = []
 
         # add a new group with the name of the subreddit, if DNE
 
         # try to fetch the group by name from the DB
         # if DNE, create a new group with the name of the subreddit
         # and send a event to insert it, else, do nothing
@@ -129,16 +114,17 @@
         # group_id = get_group_by_name(subreddit_name) // pseudo code
         if reddit_users_in_profile_json:
             for reddit_user_in_profile_json in reddit_users_in_profile_json:
 
                 # this step is inserting the user to the database
                 # this needs to return the profile_id for us to be able to use the importer
                 try:
-                    profile_id = ComprehensiveProfilesLocal.insert(json.dumps(reddit_user_in_profile_json),
-                                                                   user_context.get_effective_profile_preferred_lang_code())
+                    profile_id = self.comprehensive_profile_local.insert(
+                        reddit_user_in_profile_json,
+                        user_context.get_effective_profile_preferred_lang_code())
                 except Exception as e:
                     logger.error("an exception occurred while inserting profile " + str(reddit_user_in_profile_json)
                                  + " " + str(e))
                     continue
 
                 if not profile_id:
                     logger.error("error inserting profile " + str(reddit_user_in_profile_json))
@@ -147,18 +133,18 @@
                 # insert_to_group_profile(profile_id, group_id) // pseudo code
 
                 # register in importer
 
                 self.importer.insert(
                     data_source_id=DataSource.REDDIT_DATA_SOURCE_ID.value,
                     location_id=LocationLocalConstants.UNKNOWN_LOCATION_ID,
-                    entity_type_id=EntityType.PERSONAL_PROFILE_ENTITY_TYPE_ID.value,
+                    entity_type_id=EntityTypeId.PERSONAL_PROFILE.value,
                     entity_id=profile_id,
                     url=f"https://www.reddit.com/r/{subreddit_name}",
-                    user_id=self.user.get_effective_user_id()
+                    user_external_id=self.user.get_effective_user_id()
                 )
                 inserted_ids.append(profile_id)
 
         else:
             logger.error("error no Reddit users found")
 
         logger.end(object={"inserted_ids": inserted_ids})
```

### Comparing `profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local/src/search_reddit.py` & `profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local/src/search_reddit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,128 +1,99 @@
-import json
 import sys
-from .ProfileRedditConstants import (
-    PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
-    PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME
-)
-import os
-import tqdm
-from logger_local.Logger import Logger
-from logger_local.LoggerComponentEnum import LoggerComponentEnum
+
 import praw
 import requests
+import tqdm
 from group_remote.group_remote import GroupsRemote
-from dotenv import load_dotenv
-load_dotenv()
+# from profile_local.comprehensive_profile import ComprehensiveProfileLocal
+from logger_local.LoggerComponentEnum import LoggerComponentEnum
+from logger_local.LoggerLocal import Logger
+from python_sdk_remote.utilities import our_get_env
 
+from .ProfileRedditConstants import (
+    PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
+    PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME
+)
 
-# TODO Use function from python-sdk to access environment vairables
-REDDIT_CLIENT_ID = os.environ.get('REDDIT_CLIENT_ID')
-REDDIT_CLIENT_SECRET = os.environ.get('REDDIT_CLIENT_SECRET')
-REDDIT_USERNAME = os.environ.get('REDDIT_USERNAME')
+REDDIT_CLIENT_ID = our_get_env('REDDIT_CLIENT_ID')
+REDDIT_CLIENT_SECRET = our_get_env('REDDIT_CLIENT_SECRET')
+REDDIT_USERNAME = our_get_env('REDDIT_USERNAME')
 
 GROUP_PROFILE_RELATIONSHIP_TYPE_ID = 1
 
 object_to_insert = {
     'component_id': PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
     'component_name': PROFILE_REDDIT_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': 'yoav.e@circ.zone'
 }
 
 logger = Logger.create_logger(object=object_to_insert)
 
 
-class Reddit:
-
-    def __init__(self):
-        logger.start()
-        self.reddit = self._authenticate_reddit()
-        logger.end()
-
-    def _authenticate_reddit(self) -> praw.Reddit:
+# TODO: get meaningful data from Reddit API
+class Reddit(praw.Reddit):
 
+    def __init__(self, is_test_data: bool = False):
         logger.start()
         # TODO Let's add API-Management Indirect around it.
-        reddit = praw.Reddit(
+        super().__init__(
             client_id=REDDIT_CLIENT_ID,
             client_secret=REDDIT_CLIENT_SECRET,
             user_agent=f"random_names (by u/{REDDIT_USERNAME})"
         )
+        self.is_test_data = is_test_data
+        # self.comprehensive_profile_local = ComprehensiveProfileLocal()
+        logger.end()
 
-        logger.end(object={'reddit': reddit})
-        return reddit
-
-    def get_subreddit_and_query(self, request: dict = None) -> dict:
-
-        logger.start(object={'request': request})
-        if request:
-            subreddit_name, user_count = request['subreddit_name'], request['user_count']
-            logger.end(object={'subreddit_name': subreddit_name, 'user_count': user_count})
-            return subreddit_name, user_count
-
-        subreddit_name = input("Enter subreddit name: ")
-
-        num = input("Enter number of users to fetch (defult is no cap): ")
-
-        user_count = int(num) if len(num) > 0 else None
-
-        logger.end(object={'subreddit_name': subreddit_name, 'user_count': user_count})
-        return subreddit_name, user_count
-
-    def get_reddit_users_by_subreddit(self, subreddit, user_count: int):
+    def get_reddit_users_by_subreddit(self, subreddit, user_count: int) -> list[dict]:
         logger.start(object={'subreddit': subreddit.name, 'user_count': user_count})
         reddit_users_in_profile_json = []
-        total = user_count
-
-        total = float('inf') if total is None else total
 
         # TODO: when 'group' section is ready in ComprehensiveProfilesLocal, delete this line and
         #  add 'group' to reddit_users.append
         group_id = self._create_group_if_not_exists(subreddit.name)
         iteration = 0
 
-        with tqdm.tqdm(total=total, desc="Getting users", file=sys.stdout) as pbar:
+        with tqdm.tqdm(total=user_count, desc="Getting users", file=sys.stdout) as pbar:
             for submission in subreddit.new(limit=None):
-                if len(reddit_users_in_profile_json) >= total:
+                if len(reddit_users_in_profile_json) >= user_count:
                     return reddit_users_in_profile_json
                 for comment in submission.comments.list():
                     logger.info("Reddit user comment, iteration: " + str(iteration))
-                    if len(reddit_users_in_profile_json) >= total:
+                    if len(reddit_users_in_profile_json) >= user_count:
                         return reddit_users_in_profile_json
                     if comment.author.name == 'AutoModerator':
                         continue
+                    # TODO: get contact / useful info from comment.author
                     reddit_user_json = {
                         'profile': {
                             'name': str(comment.author.name),
-                            'name_approved': False,
-                            # TODO Please use Lang Code enum
+                            'name_approved': True,
                             'lang_code': "en",
-                            # TODO Create and use enum VISIBILITY.CREATOR =1 from visibility-local-python-package 
                             'visibility_id': True,
-                            'is_approved': False,
-                            # TODO Please use profile enum
+                            'is_approved': True,
                             'profile_type_id': 1,
-                            'stars': 0,
-                            # TODO Let's create use DEFAULT_DIALOG_WORKFLOW_STATE_ID = 1 from dialog-workflow-local-python-package enum
+                            'stars': 2,
                             'last_dialog_workflow_state_id': 1,
                             'comments': str(comment.author.comments),
                             'submissions': str(comment.author.submissions),
                             'created_utc': str(comment.author.created_utc),
                             'has_verified_email': str(comment.author.has_verified_email),
                             'is_employee': str(comment.author.is_employee),
                             'is_mod': str(comment.author.is_mod),
                             'is_gold': str(comment.author.is_gold),
                             'link_karma': str(comment.author.link_karma)
                         },
 
                         'storage': {
                             "url": str(comment.author.icon_img),
                             "filename": f'{comment.author.name}.jpg',
-                                        "file_type": "Profile Image"
+                            "file_type": "Profile Image",
+                            "file_extension": "jpg"
                         },
 
                         'reaction': {
                             'value': str(comment.author.comment_karma),
                             'image': None,
                             'title': 'comment karma',
                             'description': None
@@ -133,33 +104,33 @@
                             'parent_group_id': None,
                             'is_interest': False,
                             'image': None,
                         },
                         'group_profile': {
                             'group_id': group_id,
                             'relationship_type_id': GROUP_PROFILE_RELATIONSHIP_TYPE_ID
-                        }
+                        },
+                        'is_test_data': self.is_test_data
                     }
                     reddit_users_in_profile_json.append(reddit_user_json)
                     logger.info("Reddit user data: " + str(reddit_user_json))
                     iteration += 1
 
-                    # TODO Please update comment
                     pbar.update(1)
         logger.end(object={'reddit_users_in_profile_json': reddit_users_in_profile_json})
         return reddit_users_in_profile_json
 
     # TODO: when 'group' section is ready in ComprehensiveProfilesLocal, delete this private method
-    # TODO Please don't delete this method until we see it is working
     def _create_group_if_not_exists(self, group_name: str):
         logger.start(object={'group_name': group_name})
 
         groups_remote_object = GroupsRemote()
-        group = groups_remote_object.get_group_by_group_name(group_name)
-        if group.status_code == requests.codes.no_content:
-            group = groups_remote_object.create_group(group_name)
-        group_content = json.loads(group.content.decode('utf-8'))
-        group_id_str = group_content['data'][0]['id']
-        group_id = int(group_id_str)
-
+        group_response = groups_remote_object.get_group_response_by_group_name(group_name)
+        if group_response.status_code == requests.codes.no_content:
+            group_response = groups_remote_object.create_group(group_name)
+        if group_response.status_code != requests.codes.ok:
+            raise Exception(f"Failed to create group: {group_name} with status code: {group_response.status_code}."
+                            f" Response: {group_response.text}. Url: {group_response.url}")
+        group_json = group_response.json()
+        group_id = int(group_json['data'][0]['id'])
         logger.end(object={'group_id': group_id})
         return group_id
```

### Comparing `profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local.egg-info/PKG-INFO` & `profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: profile-reddit-restapi-imp-local
-Version: 0.0.35
+Version: 0.0.36
 Home-page: https://github.com/circles-zone/profile-reddit-restapi-imp-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: praw>=7.4.0
 Requires-Dist: tqdm>=4.64.1
-Requires-Dist: database-mysql-local>=0.0.11
-Requires-Dist: importer-local>=0.0.6
-Requires-Dist: logzio-python-handler>=4.1.0
-Requires-Dist: profiles-local>=0.0.11
-Requires-Dist: url-remote>=0.0.22
-Requires-Dist: python-dotenv>=1.0.0
-Requires-Dist: logger-local>=0.0.46
+Requires-Dist: requests
+Requires-Dist: data-source-local
 Requires-Dist: entity-type-local>=0.0.13
-Requires-Dist: group-remote>=0.0.85
-Requires-Dist: source-data-local>=0.0.3
+Requires-Dist: importer-local>=0.0.43
+Requires-Dist: location-local
+Requires-Dist: logger-local>=0.0.93
+Requires-Dist: profile-local>=0.0.61
+Requires-Dist: group-remote>=0.0.105
+Requires-Dist: python-sdk-remote>=0.0.65
+Requires-Dist: user-context-remote>=0.0.54
 
 Profile Reddit REST API Implementation Local Python Package
```

### Comparing `profile-reddit-restapi-imp-local-0.0.35/profile_reddit_restapi_imp_local.egg-info/SOURCES.txt` & `profile_reddit_restapi_imp_local-0.0.36/profile_reddit_restapi_imp_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `profile-reddit-restapi-imp-local-0.0.35/setup.py` & `profile_reddit_restapi_imp_local-0.0.36/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-import setuptools
+﻿import setuptools
 
-REPO_NAME = 'profile-reddit-restapi-imp-local'
-# TODO Please replace with the function we have in our template
-package_dir = 'profile_reddit_restapi_imp_local'
+PACKAGE_NAME = 'profile-reddit-restapi-imp-local'
+package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
-     name=REPO_NAME,
-     version='0.0.35',  # https://pypi.org/project/profile-reddit-restapi-imp-local/
-     author="Circles",
-     author_email="info@circles.life",
-     url="https://github.com/circles-zone/profile-reddit-restapi-imp-local-python-package",
-     packages=[package_dir],
-     package_dir={package_dir: f'{package_dir}/src'},
-     package_data={package_dir: ['*.py']},
-     long_description="Profile Reddit REST API Implementation Local Python Package",
-     long_description_content_type='text/markdown',
-     classifiers=[
-         "Programming Language :: Python :: 3",
-         "License :: Other/Proprietary License",
-         "Operating System :: OS Independent",
-     ],
-     install_requires=[
+    name=PACKAGE_NAME,
+    version='0.0.36',  # https://pypi.org/project/profile-reddit-restapi-imp-local/
+    author="Circles",
+    author_email="info@circles.life",
+    url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
+    packages=[package_dir],
+    package_dir={package_dir: f'{package_dir}/src'},
+    package_data={package_dir: ['*.py']},
+    long_description="Profile Reddit REST API Implementation Local Python Package",
+    long_description_content_type='text/markdown',
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: Other/Proprietary License",
+        "Operating System :: OS Independent",
+    ],
+    install_requires=[
         'praw>=7.4.0',
         'tqdm>=4.64.1',
-        'database-mysql-local>=0.0.11',
-        'importer-local>=0.0.6',
-        'logzio-python-handler>=4.1.0',
-        'profiles-local>=0.0.11',
-        'url-remote>=0.0.22',
-        'python-dotenv>=1.0.0',
-        'logger-local>=0.0.46',
+        'requests',
+        'data-source-local',
         'entity-type-local>=0.0.13',
-        'group-remote>=0.0.85',
-        'source-data-local>=0.0.3'
-        ]
+        'importer-local>=0.0.43',
+        'location-local',
+        'logger-local>=0.0.93',
+        'profile-local>=0.0.61',
+        'group-remote>=0.0.105',
+        'python-sdk-remote>=0.0.65',
+        'user-context-remote>=0.0.54',
+    ],
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


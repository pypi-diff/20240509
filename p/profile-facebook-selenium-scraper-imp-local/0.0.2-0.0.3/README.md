# Comparing `tmp/profile-facebook-selenium-scraper-imp-local-0.0.2.tar.gz` & `tmp/profile_facebook_selenium_scraper_imp_local-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile-facebook-selenium-scraper-imp-local-0.0.2.tar", last modified: Mon Dec 11 12:40:38 2023, max compression
+gzip compressed data, was "profile_facebook_selenium_scraper_imp_local-0.0.3.tar", last modified: Thu May  9 02:53:46 2024, max compression
```

## Comparing `profile-facebook-selenium-scraper-imp-local-0.0.2.tar` & `profile_facebook_selenium_scraper_imp_local-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 12:40:38.549785 profile-facebook-selenium-scraper-imp-local-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-11 12:40:38.549785 profile-facebook-selenium-scraper-imp-local-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-11 12:38:02.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 12:40:38.549785 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 12:40:38.549785 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-11 12:38:02.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-12-11 12:38:02.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local/src/date_time_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-12-11 12:38:02.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    18853 2023-12-11 12:38:02.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 12:40:38.549785 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2023-12-11 12:40:38.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-11 12:40:38.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 12:40:38.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-11 12:40:38.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-11 12:40:38.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-11 12:38:02.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-11 12:40:38.549785 profile-facebook-selenium-scraper-imp-local-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2023-12-11 12:38:02.000000 profile-facebook-selenium-scraper-imp-local-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17749 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 02:53:46.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 02:53:46.312955 profile_facebook_selenium_scraper_imp_local-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-09 02:53:05.000000 profile_facebook_selenium_scraper_imp_local-0.0.3/setup.py
```

### Comparing `profile-facebook-selenium-scraper-imp-local-0.0.2/PKG-INFO` & `profile_facebook_selenium_scraper_imp_local-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: profile-facebook-selenium-scraper-imp-local
-Version: 0.0.2
-Summary: PyPI Package for Circles <short-project-name-with-dash> Python
-Home-page: https://github.com/circles
+Version: 0.0.3
+Summary: PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
+Home-page: https://github.com/circles-zone/profile-facebook-selenium-scraper-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: PyMySQL>=1.0.2
-Requires-Dist: pytest>=7.4.0
-Requires-Dist: mysql-connector>=2.2.9
-Requires-Dist: logzio-python-handler>=4.1.0
-Requires-Dist: user-context-remote>=0.0.17
-Requires-Dist: python-sdk-local>=0.0.27
+Requires-Dist: selenium>=4.20.0
+Requires-Dist: logger-local>=0.0.135
+Requires-Dist: profile-local>=0.0.65
+Requires-Dist: language-remote>=0.0.20
 
-PyPI Package for Circles <short-project-name-with-dash> Python
+PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
```

### Comparing `profile-facebook-selenium-scraper-imp-local-0.0.2/README.md` & `profile_facebook_selenium_scraper_imp_local-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 # python-package-template
+
 This repository is designed to help you create local and remote package layers in Python.  
 It focuses on building package layers and does not include GraphQL and REST-API layers.
 
 ## Download Environment
+
 To set up the environment, follow these steps in your terminal:
+
 ```shell
 git clone https://github.com/circles-zone/<your-repo>.git --branch dev  # or other branch
 cd <your-repo>
 git checkout -b BU-<new-branch>  # if a new branch is needed
 python -m venv venv
 pip install -r requirements.txt
 ... <edit your code> ...
 git add .
 git commit -m "Your commit message"
 git push origin BU-<your-branch>
 ```
 
-For more detailed information, refer to the [documentation](https://docs.google.com/document/d/1HKhwlhwLD3S8uJ9LPI7h4Nxu77-DXKZe/edit?usp=sharing&ouid=104468990154530891864&rtpof=true&sd=true).
+For more detailed information, refer to
+the [documentation](https://docs.google.com/document/d/1HKhwlhwLD3S8uJ9LPI7h4Nxu77-DXKZe/edit?usp=sharing&ouid=104468990154530891864&rtpof=true&sd=true).
 
 ## Check List:
 
 ### Directory Structure
 
 Ensure that the root directory has the following structure:
+
 - `.github/`
 - `.vscode/` (optional)
 - `directory_with_same_name_as_the_repo/`
-  - `db/`
-  - `reports/`
-  - `project_name/`
-    - `src/`
-      - `__init__.py`
-      - `example_class.py`
-    - `tests/`
-      - `example_class_test.py`
-    - `__init__.py`
+    - `db/`
+    - `reports/`
+    - `project_name/`
+        - `src/`
+            - `__init__.py`
+            - `example_class.py`
+        - `tests/`
+            - `example_class_test.py`
+        - `__init__.py`
 
 This setup enables easy switching to a mono repo configuration.
 
 ### Database Python Scripts
 
 Place `<table-name>.py` in the `/db` folder if needed.  
 There's no need for a separate file for `_ml` tables.  
@@ -50,32 +55,39 @@
 - Use `/db/<table-name>.py` to create the schema, tables, views (including `_ml_table`).
 - Use `/db/<table-name>_insert.py` to create metadata and test data records.
 
 ### Update `setup.py`
 
 Don't forget to update the `setup.py` file, including the package name and version.  
 Remember to upload the version after every deployment.
+
 ### Working with VS Code
+
 Ensure that you push the `launch.json` file to the repository.  
 This enables running and debugging the code smoothly.
 
 ### Unit Testing
+
 We recommend using `pytest` over the `unittest` package.  
 Create a `pytest.ini` file in the project directory, not the root directory.
 run in termianl: pytest
 
 ## Workflow Completion
-When you've addressed all the TODOs in the repository, using infrastructure classes like Logger, Database, Url, Importer, and others, make sure your Feature Branch GitHub Actions Workflow is green without warnings.  
-All tests should run in GitHub Actions, your code should be well-documented, the `README.md` file should be clear and self-explanatory, test coverage should be above 90%, and all lines of code should be covered by unit tests.
+
+When you've addressed all the TODOs in the repository, using infrastructure classes like Logger, Database, Url,
+Importer, and others, make sure your Feature Branch GitHub Actions Workflow is green without warnings.  
+All tests should run in GitHub Actions, your code should be well-documented, the `README.md` file should be clear and
+self-explanatory, test coverage should be above 90%, and all lines of code should be covered by unit tests.
 
 Once these conditions are met, you can filter and analyze your records in Logz.io.  
 Pull the `dev` branch to your Feature Branch and then create a Pull Request to `dev`.
 
 Good luck :)
 
 ## check your code visibility lint with flake (Mandatory before pusj):
+
 run those command
 python -m pip install flake8 pytest
 flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
 flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
 
 note: you should use autopep8 extension in your code!
```

### Comparing `profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py` & `profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 
 class FacebookLocalConstants:
-
     DEVELOPER_EMAIL = 'neomi.b@circ.zoce'
-
-
     PROFILE_FACEBOOK_SELENIUM_SCRAPER_IMP_LOCAL_COMPONENT_ID = 245
     PROFILE_FACEBOOK_SELENIUM_SCRAPER_IMP_LOCAL_COMPONENT_NAME = 'Profile facebook selenium scraper'
     PROFILE_FACEBOOK_SELENIUM_SCRAPER_IMP_LOCAL__CODE_LOGGER_OBJECT = {
         'component_id': PROFILE_FACEBOOK_SELENIUM_SCRAPER_IMP_LOCAL_COMPONENT_ID,
         'component_name': PROFILE_FACEBOOK_SELENIUM_SCRAPER_IMP_LOCAL_COMPONENT_NAME,
         'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
         'developer_email': DEVELOPER_EMAIL
@@ -19,10 +15,7 @@
         'component_id': PROFILE_FACEBOOK_SELENIUM_SCRAPER_IMP_LOCAL_COMPONENT_ID,
         'component_name': PROFILE_FACEBOOK_SELENIUM_SCRAPER_IMP_LOCAL_COMPONENT_NAME,
         'component_category': LoggerComponentEnum.ComponentCategory.Unit_Test.value,
         'developer_email': DEVELOPER_EMAIL
     }
 
     UNKNOWN_FACEBOOK_ID = 0
-
-
-
```

### Comparing `profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py` & `profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,111 +1,103 @@
 """
 FacebookScraper Class:
 
 This class defines a Facebook scraper to gather
 information about friends on Facebook.
 It uses Selenium for web scraping and provides methods for logging in,
 extracting data about friends."""
-from dotenv import load_dotenv
-load_dotenv()
-import time  # noqa: E402
-import json  # noqa: E402
-# import os
-from datetime import datetime  # noqa: E402
-from language_local import lang_code  # noqa: E402
-from selenium import webdriver  # noqa: E402
-from selenium.webdriver.common.by import By  # noqa: E402
-from selenium.webdriver.support.ui import WebDriverWait  # noqa: E402
-from selenium.webdriver.support import expected_conditions as EC  # noqa: E402
-from selenium.common.exceptions import NoSuchElementException  # noqa: E402
-# from external_user_local.external_user import ExternalUser
-from profile_local.comprehensive_profile import ComprehensiveProfilesLocal  # noqa:E402
-from logger_local.Logger import Logger  # noqa: E402
-from logger_local.LoggerComponentEnum import LoggerComponentEnum  # noqa: E402
+import time
+from datetime import datetime
 
+from language_remote.lang_code import LangCode
+from logger_local.LoggerComponentEnum import LoggerComponentEnum
+from logger_local.LoggerLocal import Logger
+from profile_local.comprehensive_profile import ComprehensiveProfileLocal
+from selenium import webdriver
+from selenium.common.exceptions import NoSuchElementException
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions
+from selenium.webdriver.support.ui import WebDriverWait
 
-LANG_CODE_HE = lang_code.LangCode.HEBREW.value
+LANG_CODE_HE = LangCode.HEBREW.value
 QUEUE_LOCAL_PYTHON_COMPONENT_ID = 245
-QUEUE_LOCAL_PYTHON_COMPONENT_NAME = "\
-    profile_facebook_selenium_scraper_imp_local/\
-    src/facebook_scraper"
+QUEUE_LOCAL_PYTHON_COMPONENT_NAME = "profile_facebook_selenium_scraper_imp_local/src/facebook_scraper"
 DEVELOPER_EMAIL = 'neomi.b@circ.zone'
 DEFAULT_STARS = 0
 DEFAULT_LAST_DIALOG_WORKFLOW_STATE_ID = 0
 SYSTEM_ID = 1
 
+HEADLESS_MODE = True  # You can set to false locally to see the browser & debug
+
 
 class FacebookScraper:
-    """
-    Class for scraping Facebook friends' information."""
+    """Class for scraping Facebook friends' information."""
 
     def __init__(self) -> None:
-        """
-        Initializes the FacebookScraper class."""
+        """Initializes the FacebookScraper class."""
+        self.comprehensive_profile = ComprehensiveProfileLocal()
         self.name = 'name'
-        # self.username = 'username'
         self.gender = 1
         self.job_title = 'job_title'
         self.address = 'address'
 
         self.logger = Logger(
             object={
                 'component_id': QUEUE_LOCAL_PYTHON_COMPONENT_ID,
                 'component_name': QUEUE_LOCAL_PYTHON_COMPONENT_NAME,
-                'component_category':
-                LoggerComponentEnum.ComponentCategory.Code.value,
+                'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
                 'developer_email': DEVELOPER_EMAIL
             }
         )
-        self.driver = webdriver.Firefox()
+        options = webdriver.FirefoxOptions()
+        if HEADLESS_MODE:
+            options.add_argument("--headless")
+        self.driver = webdriver.Firefox(options=options)
         self.wait = WebDriverWait(self.driver, 10)
 
-    def extract_and_cast_to_int(self, input_string: str) -> int:
-        """
-        Extracts and casts the first integer from the given input string."""
-        number = [int(s) for s in input_string.split() if s.isdigit()]
-        return number[0] if number else None
+    @staticmethod
+    def extract_and_cast_to_int(input_string: str) -> int:
+        """Extracts and casts the first integer from the given input string."""
+        for s in input_string.split():
+            if s.isdigit():
+                return int(s)
 
-    def login(self, facebook_user_identifier: str,
-              facebook_password: str) -> None:
+    def login(self, facebook_user_identifier: str, facebook_password: str) -> None:
         """
         Login to the account by given username and facebook_password."""
         try:
             self.logger.start("Logging into Facebook", object={
-                "facebook_user_identifier": facebook_user_identifier
-            })
+                "facebook_user_identifier": facebook_user_identifier})
             self.driver.get('https://www.facebook.com/')
             time.sleep(5)
-            facebook_user_identifier_input = self.driver.find_element(
-                By.ID, 'email')
+            facebook_user_identifier_input = self.driver.find_element(By.ID, 'email')
             facebook_password_input = self.driver.find_element(By.ID, 'pass')
 
             facebook_user_identifier_input.send_keys(facebook_user_identifier)
             facebook_password_input.send_keys(facebook_password)
             facebook_password_input.submit()
 
-            self.wait.until(EC.url_contains('facebook.com'))
+            self.wait.until(expected_conditions.url_contains('facebook.com'))
             time.sleep(10)
             self.logger.end("Login successful")
         except NoSuchElementException:
             self.logger.error("Login failed")
 
-    def get_num_friends(self) -> int:
+    def get_num_friends(self) -> int or None:
         """
         Gets the number of friends from the Facebook friends list."""
         try:
             self.logger.start("Getting the number of friends")
             self.driver.get('https://www.facebook.com/friends/list')
             time.sleep(5)
             num_friends_css_selector = 'div.xu06os2:nth-child(3) > \
                 div:nth-child(1) >div:nth-child(1) > div:nth-child(1) >\
                       div:nth-child(1) > div:nth-child(1) >\
                     h2:nth-child(1) > span:nth-child(1) > span:nth-child(1)'
-            num_of_friends = self.driver.find_element(
-                By.CSS_SELECTOR, num_friends_css_selector).text
+            num_of_friends = self.driver.find_element(By.CSS_SELECTOR, num_friends_css_selector).text
             num_of_friends = self.extract_and_cast_to_int(num_of_friends)
             self.logger.end("Successfully retrieved the number of friends")
             return num_of_friends
         except NoSuchElementException:
             self.logger.error("Error getting the number of friends")
             return None
 
@@ -116,33 +108,29 @@
             self.logger.start(f"Clicking on friend with index {j}")
             friend_css_selector = f'.x135pmgq > div:nth-child({j}) >\
                   a:nth-child(1) >div:nth-child(1) > div:nth-child(2) >\
                       div:nth-child(1) > div:nth-child(1)> div:nth-child(1) >\
                           div:nth-child(1) > span:nth-child(1) >\
                               span:nth-child(1)\
                         > span:nth-child(1)'
-            friend = self.driver.find_element(By.CSS_SELECTOR,
-                                              friend_css_selector)
+            friend = self.driver.find_element(By.CSS_SELECTOR, friend_css_selector)
             friend.click()
             time.sleep(5)
             self.logger.end(f"Clicked on friend with index {j}")
         except NoSuchElementException:
             self.logger.error(f"Error clicking on friend with index {j}")
 
     def get_friend_name(self) -> str:
         """
         Gets the name of the current friend."""
         try:
             self.logger.start("Getting friend's name")
             friend_name_css_selector = '.x14qwyeo > h1:nth-child(1)'
-            friend_name = self.driver.find_element(By.CSS_SELECTOR,
-                                                   friend_name_css_selector
-                                                   ).text
-            self.logger.end(f"Successfully \
-                            retrieved friend's name: {friend_name}")
+            friend_name = self.driver.find_element(By.CSS_SELECTOR, friend_name_css_selector).text
+            self.logger.end(f"Successfully retrieved friend's name: {friend_name}")
             return friend_name
         except NoSuchElementException:
             self.logger.error("Error getting friend's name")
             return ""
 
     def click_about_friend(self) -> None:
         """
@@ -150,79 +138,73 @@
         try:
             self.logger.start("Clicking on the 'About' \
                               section of the current friend's profile")
             about_friend_css_selector = '.x879a55 > div:nth-child(1) >\
                   div:nth-child(1) >div:nth-child(1) > div:nth-child(1) >\
                       div:nth-child(1) > div:nth-child(1) >a:nth-child(3) >\
                           div:nth-child(1) > span:nth-child(1)'
-            about_friend = self.driver.find_element(By.CSS_SELECTOR,
-                                                    about_friend_css_selector)
+            about_friend = self.driver.find_element(By.CSS_SELECTOR, about_friend_css_selector)
             about_friend.click()
             time.sleep(5)
             self.logger.end("Clicked on the 'About' section successfully")
         except NoSuchElementException:
             self.logger.error("Error clicking on the 'About' section")
 
-    def get_job_title(self) -> str:
+    def get_job_title(self) -> str or None:
         """
         Gets the work place information of the current friend."""
         try:
-            self.logger.start(
-                "Getting work place information of the current friend")
+            self.logger.start("Getting work place information of the current friend")
             try:
                 job_title_css_selector = '.xqmdsaz > div:nth-child(1) >\
                       div:nth-child(1) >div:nth-child(2) > div:nth-child(1) >\
                           div:nth-child(1) > div:nth-child(2) >\
                             div:nth-child(1) > span:nth-child(1) > \
                                 a:nth-child(1) > span:nth-child(1) >\
                                     span:nth-child(1)'
-                job_title = self.driver.find_element(
-                    By.CSS_SELECTOR, job_title_css_selector).text
-                self.logger.end(
-                    "Successfully retrieved work place information")
+                job_title = self.driver.find_element(By.CSS_SELECTOR, job_title_css_selector).text
+                self.logger.end("Successfully retrieved work place information")
                 return job_title
             except NoSuchElementException:
                 return None
         except NoSuchElementException:
             self.logger.error("Error getting work place information")
 
-    def get_went_to(self) -> str:
+    def get_went_to(self) -> str or None:
         """
         Gets the 'Went to' information of the current friend.
         """
         try:
             try:
                 self.logger.start(
                     "Getting 'Went to' information of the current friend")
                 went_to_css_selector = 'div.x1hq5gj4:nth-child(3) >\
                       div:nth-child(1) >div:nth-child(1) > div:nth-child(2) >\
                           div:nth-child(1) > span:nth-child(1)'
-                went_to = self.driver.find_element(
-                    By.CSS_SELECTOR, went_to_css_selector).text
+                went_to = self.driver.find_element(By.CSS_SELECTOR, went_to_css_selector).text
                 self.logger.end("Successfully retrieved 'Went to' information")
                 return went_to
             except NoSuchElementException:
                 return None
         except NoSuchElementException:
             self.logger.error("Error getting 'Went to' information")
 
-    def get_address(self) -> str:
+    def get_address(self) -> str or None:
         """
         Gets the residential location information of the current friend."""
         try:
             self.logger.start(
                 "Getting residential location \
                     information of the current friend")
             address_css_selector = 'div.x1hq5gj4:nth-child(4) >\
                   div:nth-child(1) >div:nth-child(1) >\
                       div:nth-child(2) > div:nth-child(1) >\
                           span:nth-child(1) >a:nth-child(1) >\
                               span:nth-child(1) > span:nth-child(1)'
-            address = self.driver.find_element(
-                By.CSS_SELECTOR, address_css_selector).text
+            address = self.driver.find_element(By.CSS_SELECTOR, address_css_selector).text
             self.logger.end(
                 "Successfully retrieved residential location information")
             return address
         except NoSuchElementException:
             self.logger.error("Error getting residential location information")
             return None
 
@@ -233,82 +215,77 @@
         try:
             self.logger.start(
                 "Clicking on 'Basic Info' subsection\
                       of the current friend's profile")
             self.click_about_friend()
 
             basic_info_css_selector = 'div.x1e56ztr:nth-child(5)'
-            basic_info = self.driver.find_element(
-                By.CSS_SELECTOR, basic_info_css_selector)
+            basic_info = self.driver.find_element(By.CSS_SELECTOR, basic_info_css_selector)
             basic_info.click()
             time.sleep(5)
             self.logger.end("Clicked on 'Basic Info' subsection successfully")
         except NoSuchElementException:
             self.logger.error("Error clicking on 'Basic Info' subsection")
 
-    def get_gender_type(self) -> str:
-        """
-        Gets the gender information of the current friend."""
+    def get_gender_type(self) -> int or None:
+        # TODO: use enum
+        """Gets the gender information of the current friend."""
         self.click_about_basic_info_friend()
         try:
             self.logger.start(
                 "Getting gender information of the current friend")
             gender_css_selector = '.xqmdsaz > div:nth-child(3) >\
                   div:nth-child(1) >div:nth-child(2) > div:nth-child(1) >\
                       div:nth-child(1) > div:nth-child(2) >div:nth-child(1) >\
                           div:nth-child(1) > div:nth-child(1) >\
                               div:nth-child(1) >div:nth-child(1) >\
                                   span:nth-child(1)'
-            gender = self.driver.find_element(By.CSS_SELECTOR,
-                                              gender_css_selector).text
+            gender = self.driver.find_element(By.CSS_SELECTOR, gender_css_selector).text
             self.logger.end("Successfully retrieved gender information")
             if gender == 'Female':
                 gender = 1
                 return gender
             if gender == 'Male':
                 gender = 2
                 return gender
         except NoSuchElementException:
             self.logger.error("Error getting gender information")
             return None
 
-    def convert_to_date(self, date_string: str) -> datetime:
+    def convert_to_date(self, date_string: str) -> datetime or None:
         """
         Converts a date string to a datetime object."""
         default_date_format = "%B %d %Y"
         try:
             self.logger.start("Converting date string to datetime object",
-                              object={
-                                       "date_string": date_string})
+                              object={"date_string": date_string})
             date_object = datetime.strptime(date_string, default_date_format)
             self.logger.end("Conversion successful")
             return date_object
         except NoSuchElementException:
             self.logger.error("Error converting date string")
             return None
 
-    def get_birth_date(self) -> datetime:
+    def get_birth_date(self) -> datetime or None:
         """
-        Gets the birth date of the current friend."""
+        Gets the birthdate of the current friend."""
         self.click_about_basic_info_friend()
         try:
             self.logger.start("Getting birth date of the current friend")
             birth_date_css_selector = 'div.xat24cr:nth-child(3) >\
                   div:nth-child(1) >div:nth-child(1) > div:nth-child(2) >\
                       div:nth-child(1) > div:nth-child(1) >div:nth-child(1) >\
                        div:nth-child(1) > div:nth-child(1) > span:nth-child(1)'
-            birth_date = self.driver.find_element(By.CSS_SELECTOR,
-                                                  birth_date_css_selector).text
+            birth_date = self.driver.find_element(By.CSS_SELECTOR, birth_date_css_selector).text
             birth_year_css_selector = 'div.xat24cr:nth-child(3) >\
                   div:nth-child(1) >div:nth-child(1) > div:nth-child(2) >\
                     div:nth-child(2) > div:nth-child(1) >div:nth-child(1) >\
                        div:nth-child(1) > div:nth-child(1) > span:nth-child(1)'
             self.logger.end("Successfully retrieved birth date")
-            birth_year = self.driver.find_element(By.CSS_SELECTOR,
-                                                  birth_year_css_selector).text
+            birth_year = self.driver.find_element(By.CSS_SELECTOR, birth_year_css_selector).text
             birth_date = birth_date + " " + birth_year
             return self.convert_to_date(birth_date)
         except NoSuchElementException:
             self.logger.error("Error getting birth date")
             return None
 
     def scrape_friends(self) -> None:
@@ -339,40 +316,36 @@
             self.logger.end("Scraping completed")
         except NoSuchElementException:
             self.logger.error("Error during scraping")
         finally:
             time.sleep(10)
             self.driver.quit()
 
-    def generate_compatible_json(self, profile_entry: dict):
-        """
-        generate_compatible_json."""
+    @staticmethod
+    def generate_compatible_dict(profile_entry: dict) -> dict:
+        """generate_compatible_dict."""
         profile = {
             'number': profile_entry.get('number', None),
             'profile_name': profile_entry.get('name', None),
             'name': profile_entry.get('name', None),
             'name_approved': True,
-            'lang_code': profile_entry.get('language', LANG_CODE_HE),
+            'lang_code': LangCode(profile_entry.get('language', LANG_CODE_HE)),
             # 'user_id': logger.user_context.get_real_user_id(),
             'person_id': profile_entry.get('person_id', None),
             'is_main': profile_entry.get('is_main', 0),
             'profile_type_id': profile_entry.get('profile_type_id', 1),
             'is_approved': profile_entry.get('is_approved', 0),
-            # 'preferred_lang_code': profile_entry.get('language',
-            # LangCode.ENGLISH.value),
             # 'is_main': profile_entry.get('is_main', None),
-            'preferred_lang_code': profile_entry.get('language', None),
+            'preferred_lang_code': LangCode(profile_entry['language']) if 'language' in profile_entry else None,
             'is_rip': profile_entry.get('rip', 0),
             "main_phone_id": profile_entry.get('main_phone_id', 1),
             "gender_id": profile_entry.get('gender_id', 1),
             "stars": profile_entry.get('stars', 0),
-            'experience_years_min': profile_entry.get(
-                'experience_years_min', None),
-            'last_dialog_workflow_state_id': profile_entry.get(
-                'last_dialog_workflow_state_id', 0),
+            'experience_years_min': profile_entry.get('experience_years_min', None),
+            'last_dialog_workflow_state_id': profile_entry.get('last_dialog_workflow_state_id', 0),
             'visibility_id': profile_entry.get('visibility_id', 0),
         }
         location = {
             'coordinate': {
                 'latitude': profile_entry.get('latitude', 0),
                 'longitude': profile_entry.get('longitude', 0),
             },
@@ -388,44 +361,30 @@
         }
 
         entry = {
             "location": location,
             "profile": profile,
         }
 
-        return json.dumps(entry)
+        return entry
 
     def insert_to_database(self) -> None:
         """insert."""
         self.logger.start()
         profile_json = {
-                'name': self.name,
-                'gender_id': self.gender,
-                'lang_code': LANG_CODE_HE,
-                'visibility_id': True,
-                'is_approved': False,
-                'stars': DEFAULT_STARS,
-                'last_dialog_workflow_state_id':
-                DEFAULT_LAST_DIALOG_WORKFLOW_STATE_ID,
-                'job_title': self.job_title,
-                'address_english': self.address
+            'name': self.name,
+            'gender_id': self.gender,
+            'lang_code': LangCode(LANG_CODE_HE),
+            'visibility_id': True,
+            'is_approved': False,
+            'stars': DEFAULT_STARS,
+            'last_dialog_workflow_state_id': DEFAULT_LAST_DIALOG_WORKFLOW_STATE_ID,
+            'job_title': self.job_title,
+            'address_english': self.address
         }
 
-        profile_str = self.generate_compatible_json(profile_json)
-        ComprehensiveProfilesLocal.insert(profile_str, LANG_CODE_HE)
+        profile_json = self.generate_compatible_dict(profile_json)
+        self.comprehensive_profile.insert(profile_json=profile_json, lang_code=LangCode(LANG_CODE_HE))
         # access_token = os.getenv("FACEBOOK_GRAPH_IMPORT_API_ACCESS_TOKEN")
         # ExternalUser.insert_or_update_external_user_access_token(
         #     self.username, profile_id, SYSTEM_ID, access_token)
         self.logger.end()
-
-
-if __name__ == "__main__":
-    fb_scraper = FacebookScraper()
-
-    FACEBOOK_USER_IDENTIFIER = "neomi.b@circ.zone"
-    FACEBOOK_PASSWORD = "Neo1Bas2Circ3!"
-
-    try:
-        fb_scraper.login(FACEBOOK_USER_IDENTIFIER, FACEBOOK_PASSWORD)
-        fb_scraper.scrape_friends()
-    except NoSuchElementException as e:
-        fb_scraper.logger.error(f"An unexpected error occurred: {str(e)}")
```

### Comparing `profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO` & `profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: profile-facebook-selenium-scraper-imp-local
-Version: 0.0.2
-Summary: PyPI Package for Circles <short-project-name-with-dash> Python
-Home-page: https://github.com/circles
+Version: 0.0.3
+Summary: PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
+Home-page: https://github.com/circles-zone/profile-facebook-selenium-scraper-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: PyMySQL>=1.0.2
-Requires-Dist: pytest>=7.4.0
-Requires-Dist: mysql-connector>=2.2.9
-Requires-Dist: logzio-python-handler>=4.1.0
-Requires-Dist: user-context-remote>=0.0.17
-Requires-Dist: python-sdk-local>=0.0.27
+Requires-Dist: selenium>=4.20.0
+Requires-Dist: logger-local>=0.0.135
+Requires-Dist: profile-local>=0.0.65
+Requires-Dist: language-remote>=0.0.20
 
-PyPI Package for Circles <short-project-name-with-dash> Python
+PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
```

### Comparing `profile-facebook-selenium-scraper-imp-local-0.0.2/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt` & `profile_facebook_selenium_scraper_imp_local-0.0.3/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,10 +3,9 @@
 setup.py
 profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO
 profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt
 profile_facebook_selenium_scraper_imp_local.egg-info/dependency_links.txt
 profile_facebook_selenium_scraper_imp_local.egg-info/requires.txt
 profile_facebook_selenium_scraper_imp_local.egg-info/top_level.txt
 profile_facebook_selenium_scraper_imp_local/src/__init__.py
-profile_facebook_selenium_scraper_imp_local/src/date_time_check.py
 profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py
 profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py
```

### Comparing `profile-facebook-selenium-scraper-imp-local-0.0.2/pyproject.toml` & `profile_facebook_selenium_scraper_imp_local-0.0.3/pyproject.toml`

 * *Files identical despite different names*


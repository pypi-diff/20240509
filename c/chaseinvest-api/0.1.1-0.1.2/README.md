# Comparing `tmp/chaseinvest-api-0.1.1.tar.gz` & `tmp/chaseinvest_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaseinvest-api-0.1.1.tar", last modified: Sun Mar  3 01:41:18 2024, max compression
+gzip compressed data, was "chaseinvest_api-0.1.2.tar", last modified: Thu May  9 10:44:42 2024, max compression
```

## Comparing `chaseinvest-api-0.1.1.tar` & `chaseinvest_api-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:41:18.260122 chaseinvest-api-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-03-03 01:41:18.260122 chaseinvest-api-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:41:18.256122 chaseinvest-api-0.1.1/chase/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/chase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/chase/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/chase/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9170 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/chase/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/chase/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/chase/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:41:18.260122 chaseinvest-api-0.1.1/chaseinvest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-03-03 01:41:18.000000 chaseinvest-api-0.1.1/chaseinvest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-03 01:41:18.000000 chaseinvest-api-0.1.1/chaseinvest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 01:41:18.000000 chaseinvest-api-0.1.1/chaseinvest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-03 01:41:18.000000 chaseinvest-api-0.1.1/chaseinvest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-03 01:41:18.000000 chaseinvest-api-0.1.1/chaseinvest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-03 01:41:18.260122 chaseinvest-api-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 01:41:18.260122 chaseinvest-api-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-03-03 01:41:12.000000 chaseinvest-api-0.1.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:44:42.175531 chaseinvest_api-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-09 10:44:42.175531 chaseinvest_api-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:44:42.171531 chaseinvest_api-0.1.2/chase/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9412 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/chase/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:44:42.171531 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 10:44:42.000000 chaseinvest_api-0.1.2/chaseinvest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:44:42.175531 chaseinvest_api-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:44:42.171531 chaseinvest_api-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-09 10:44:38.000000 chaseinvest_api-0.1.2/tests/test.py
```

### Comparing `chaseinvest-api-0.1.1/LICENSE` & `chaseinvest_api-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chaseinvest-api-0.1.1/PKG-INFO` & `chaseinvest_api-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chaseinvest-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: An unofficial API for Chase Invest
 Home-page: https://github.com/MaxxRK/chaseinvest-api
-Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.2.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: CHASE,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
@@ -23,15 +23,15 @@
 Requires-Dist: playwright-stealth
 
 # chaseinvest-api
  A reverse-engineered python API to interact with the Chase Trading platform.
 
  This is not an official api! This api's functionality may change at any time.
 
- This api provides a means of buying and selling stocks through Chase. It uses selenium-wire to scrape response data and selenium to interact with the website.
+ This api provides a means of buying and selling stocks through Chase. It uses playwright to scrape response data and to interact with the website.
 
  ---
 
 ## Contribution
 I am new to coding and new to open-source. I would love any help and suggestions!
 
 ## Setup
@@ -41,15 +41,15 @@
 ```
 This package requires playwright. After installing chaseinvest-api, you will need to finish the install of playwright. You can do this in most cases by running the command:
 ```
 playwright install
 ```
 If you would like some more information on this, you can find it [here](https://playwright.dev/python/docs/intro).
 
-## Quikstart
+## Quickstart
 The code below will: 
 - Login and print account info. 
 - Get a quote for 'INTC' and print out the information
 - Place a market order for 'INTC' on the first account in the `account_numbers` list
 - Print out the order confirmation
 
 ```
@@ -183,8 +183,9 @@
  - [x] Get placed order status
 
 ## TO DO
  - [ ] Cancel placed orders
  - [ ] Options
  - [ ] Give me some Ideas!
 
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/O5O6PTOYG)  
+## If you would like to support me, you can do so here:
+[![GitHub Sponsors](https://img.shields.io/github/sponsors/maxxrk?style=social)](https://github.com/sponsors/maxxrk)
```

### Comparing `chaseinvest-api-0.1.1/README.md` & `chaseinvest_api-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # chaseinvest-api
  A reverse-engineered python API to interact with the Chase Trading platform.
 
  This is not an official api! This api's functionality may change at any time.
 
- This api provides a means of buying and selling stocks through Chase. It uses selenium-wire to scrape response data and selenium to interact with the website.
+ This api provides a means of buying and selling stocks through Chase. It uses playwright to scrape response data and to interact with the website.
 
  ---
 
 ## Contribution
 I am new to coding and new to open-source. I would love any help and suggestions!
 
 ## Setup
@@ -17,15 +17,15 @@
 ```
 This package requires playwright. After installing chaseinvest-api, you will need to finish the install of playwright. You can do this in most cases by running the command:
 ```
 playwright install
 ```
 If you would like some more information on this, you can find it [here](https://playwright.dev/python/docs/intro).
 
-## Quikstart
+## Quickstart
 The code below will: 
 - Login and print account info. 
 - Get a quote for 'INTC' and print out the information
 - Place a market order for 'INTC' on the first account in the `account_numbers` list
 - Print out the order confirmation
 
 ```
@@ -159,8 +159,9 @@
  - [x] Get placed order status
 
 ## TO DO
  - [ ] Cancel placed orders
  - [ ] Options
  - [ ] Give me some Ideas!
 
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/O5O6PTOYG)  
+## If you would like to support me, you can do so here:
+[![GitHub Sponsors](https://img.shields.io/github/sponsors/maxxrk?style=social)](https://github.com/sponsors/maxxrk)
```

### Comparing `chaseinvest-api-0.1.1/chase/account.py` & `chaseinvest_api-0.1.2/chase/account.py`

 * *Files identical despite different names*

### Comparing `chaseinvest-api-0.1.1/chase/order.py` & `chaseinvest_api-0.1.2/chase/order.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,21 @@
             "AFTER HOURS WARNING": "",
             "ORDER CONFIRMATION": "",
         }
 
         for i in range(0, 4):
             self.session.page.goto(order_page(account_id))
             self.session.page.reload()
+            experience = self.session.page.wait_for_selector(
+                "span > a > span.link__text"
+            )
+            if experience.text_content() == "Switch back to classic trading experience":
+                experience.click()
+                self.session.page.reload()
+                self.session.page.goto(order_page(account_id))
             try:
                 self.session.page.wait_for_selector(
                     "css=label >> text=Buy", timeout=20000
                 )
                 quote_box = self.session.page.query_selector(
                     "#equitySymbolLookup-block-autocomplete-validate-input-field"
                 )
@@ -116,17 +123,17 @@
                     "Enter",
                 )
                 self.session.page.wait_for_selector(".NOTE", timeout=10000)
                 self.session.page.wait_for_selector("#element-id", state="hidden")
                 order_messages["ORDER INVALID"] = "Order page loaded correctly."
                 break
             except PlaywrightTimeoutError:
-                order_messages[
-                    "ORDER INVALID"
-                ] = f"Order page did not load correctly cannot continue. Tried {i + 1} times."
+                order_messages["ORDER INVALID"] = (
+                    f"Order page did not load correctly cannot continue. Tried {i + 1} times."
+                )
                 print(order_messages["ORDER INVALID"])
 
         if order_messages["ORDER INVALID"] != "Order page loaded correctly.":
             return order_messages
 
         if order_type == "BUY":
             buy_btn = self.session.page.wait_for_selector("xpath=//label[text()='Buy']")
@@ -149,37 +156,37 @@
             limit_btn.click()
         elif price_type == "MARKET":
             market_btn = self.session.page.wait_for_selector(
                 "xpath=//label[text()='Market']"
             )
             market_btn.click()
             if duration not in ["DAY", "ON_THE_CLOSE"]:
-                order_messages[
-                    "ORDER INVALID"
-                ] = "Market orders must be DAY or ON THE CLOSE."
+                order_messages["ORDER INVALID"] = (
+                    "Market orders must be DAY or ON THE CLOSE."
+                )
                 return order_messages
         elif price_type == "STOP":
             stop_btn = self.session.page.wait_for_selector(
                 "xpath=//label[text()='Stop']"
             )
             stop_btn.click()
             if duration not in ["DAY", "GOOD_TILL_CANCELLED"]:
-                order_messages[
-                    "ORDER INVALID"
-                ] = "Stop orders must be DAY or GOOD TILL CANCELLED."
+                order_messages["ORDER INVALID"] = (
+                    "Stop orders must be DAY or GOOD TILL CANCELLED."
+                )
                 return order_messages
         elif price_type == "STOP_LIMIT":
             stop_limit_btn = self.session.page.wait_for_selector(
                 "xpath=//label[text()='Stop Limit']"
             )
             stop_limit_btn.click()
             if duration not in ["DAY", "GOOD_TILL_CANCELLED"]:
-                order_messages[
-                    "ORDER INVALID"
-                ] = "Stop orders must be DAY or GOOD TILL CANCELLED."
+                order_messages["ORDER INVALID"] = (
+                    "Stop orders must be DAY or GOOD TILL CANCELLED."
+                )
                 return order_messages
 
         if price_type in ["LIMIT", "STOP_LIMIT"]:
             self.session.page.fill(
                 "#tradeLimitPrice-text-input-field", str(limit_price)
             )
         if price_type in ["STOP", "STOP_LIMIT"]:
@@ -287,17 +294,17 @@
                 order_messages["ORDER CONFIRMATION"] = "Alert Text not found."
                 return order_messages
             order_confirmation = order_handle.text_content()
             order_confirmation = order_confirmation.replace("\n", " ")
             order_messages["ORDER CONFIRMATION"] = order_confirmation
             return order_messages
         except PlaywrightTimeoutError:
-            order_messages[
-                "ORDER CONFIRMATION"
-            ] = "No order confirmation page found. Order Failed."
+            order_messages["ORDER CONFIRMATION"] = (
+                "No order confirmation page found. Order Failed."
+            )
             return order_messages
 
     def get_order_statuses(self, account_id):
         """
         Retrieves the statuses of all recent orders placed.
 
         This method navigates to the order status page and scrapes the status of each order.
```

### Comparing `chaseinvest-api-0.1.1/chase/session.py` & `chaseinvest_api-0.1.2/chase/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         get_browser(): Initializes and returns a WebDriver with the necessary options.
         login(username, password, last_four): Logs into Chase with the provided credentials.
         login_two(code): Logs into Chase with the provided two-factor authentication code.
         save_storage_state(): Saves the storage state of the browser to a file.
         close_browser(): Closes the browser.
     """
 
-    def __init__(self, headless=True, title=None, profile_path="."):
+    def __init__(self, headless=True, title=None, profile_path=".", debug=False):
         """
         Initializes a new instance of the ChaseSession class.
 
         Args:
             title (string): Denotes the name of the profile and if populated will make the session persistent.
             headless (bool, optional): Whether the WebDriver should run in headless mode. Defaults to True.
             docker (bool, optional): Whether the session is running in a Docker container. Defaults to False.
@@ -43,14 +43,15 @@
         """
         self.headless: bool = headless
         self.title: str = title
         self.profile_path: str = profile_path
         self.password: str = ""
         self.context = None
         self.page = None
+        self.debug: bool = debug
         self.playwright = sync_playwright().start()
         self.get_browser()
 
     def __enter__(self):
         """
         Enter the runtime context related to this object.
 
@@ -110,14 +111,18 @@
             self.browser = self.playwright.firefox.launch(headless=True)
         else:
             self.browser = self.playwright.firefox.launch(headless=False)
         self.context = self.browser.new_context(
             viewport={"width": 1920, "height": 1080},
             storage_state=self.profile_path if self.title is not None else None,
         )
+        if self.debug:
+            self.context.tracing.start(
+                name="chase_trace", screenshots=True, snapshots=True
+            )
         self.page = self.context.new_page()
 
     def save_storage_state(self):
         """
         Saves the storage state of the browser to a file.
 
         This method saves the storage state of the browser to a file so that it can be restored later.
@@ -128,14 +133,16 @@
         storage_state = self.page.context.storage_state()
         with open(self.profile_path, "w") as f:
             json.dump(storage_state, f)
 
     def close_browser(self):
         """Closes the browser."""
         self.save_storage_state()
+        if self.debug:
+            self.context.tracing.stop(path="./chase_trace.zip")
         self.browser.close()
         self.playwright.stop()
 
     def login(self, username, password, last_four):
         """
         Logs into the website with the provided username and password.
 
@@ -167,15 +174,14 @@
                 dropdown = self.page.query_selector(
                     "#header-simplerAuth-dropdownoptions-styledselect"
                 )
                 dropdown.click()
                 options_ls = self.page.query_selector_all('li[role="presentation"]')
                 for item in options_ls:
                     item_text = item.text_content()
-                    print(item_text)
                     if str(last_four) in item_text:
                         item.click()
                         break
                 self.page.click('button[type="submit"]')
                 self.page.wait_for_load_state("load", timeout=30000)
                 return True
             except PlaywrightTimeoutError:
```

### Comparing `chaseinvest-api-0.1.1/chase/symbols.py` & `chaseinvest_api-0.1.2/chase/symbols.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 from playwright.sync_api import TimeoutError as PlaywrightTimeoutError
 
 from .session import ChaseSession
-from .urls import account_holdings, holdings_json, order_page, quote_endpoint
+from .urls import account_holdings, holdings_json, order_page
 
 
 class SymbolQuote:
     """
     A class to manage the quote of a specific symbol associated with a ChaseSession.
 
     This class provides methods to retrieve and manage information about the quote of a specific symbol associated with a given session.
@@ -50,66 +50,76 @@
         self.symbol = symbol
         self.ask_price: float = 0
         self.ask_exchange_code: str = ""
         self.ask_quantity: int = 0
         self.bid_price: float = 0
         self.bid_exchange_code: str = ""
         self.bid_quantity: int = 0
-        self.change_amount: float = 0
         self.last_trade_price: float = 0
-        self.last_trade_quantity: int = 0
+        self.last_trade_quantity: float = 0
         self.last_exchange_code: str = ""
-        self.change_percentage: float = 0
         self.as_of_time: datetime = None
         self.security_description: str = ""
-        self.security_symbol: str = ""
-        self.raw_json: dict = {}
         self.get_symbol_quote()
 
     def get_symbol_quote(self):
         """
         Retrieves and sets the quote information of the symbol.
 
         This method navigates to the symbol quote page, waits for the quote information to load, and then retrieves the quote information from the page.
 
         Returns:
             None
         """
-        with self.session.page.expect_request(quote_endpoint(self.symbol)) as first:
+
+        self.session.page.goto(order_page(self.account_id))
+        experience = self.session.page.wait_for_selector("span > a > span.link__text")
+        if experience.text_content() == "Switch back to classic trading experience":
+            experience.click()
+            self.session.page.reload()
             self.session.page.goto(order_page(self.account_id))
-            self.session.page.wait_for_selector("css=label >> text=Buy")
-            self.session.page.wait_for_selector(
-                "#equitySymbolLookup-block-autocomplete-validate-input-field"
-            )
-            self.session.page.fill(
-                "#equitySymbolLookup-block-autocomplete-validate-input-field",
-                self.symbol,
-            )
-            self.session.page.press(
-                "#equitySymbolLookup-block-autocomplete-validate-input-field", "Enter"
-            )
-            first_request = first.value
-            body = first_request.response().json()
-        self.raw_json = body
-        self.ask_price = float(self.raw_json["askPriceAmount"])
-        self.ask_exchange_code = self.raw_json["askExchangeCode"]
-        self.ask_quantity = int(self.raw_json["askQuantity"])
-        self.bid_price = float(self.raw_json["bidPriceAmount"])
-        self.bid_exchange_code = self.raw_json["bidExchangeCode"]
-        self.bid_quantity = int(self.raw_json["bidQuantity"])
-        self.change_amount = float(self.raw_json["changeAmount"])
-        self.last_trade_price = float(self.raw_json["lastTradePriceAmount"])
-        self.last_trade_quantity = int(self.raw_json["lastTradeQuantity"])
-        self.last_exchange_code = self.raw_json["lastTradeExchangeCode"]
-        self.change_percentage = float(self.raw_json["changePercent"])
-        self.as_of_time = datetime.strptime(
-            self.raw_json["asOfTimestamp"], "%Y-%m-%dT%H:%M:%S.%fZ"
+        self.session.page.wait_for_selector("css=label >> text=Buy")
+        self.session.page.wait_for_selector(
+            "#equitySymbolLookup-block-autocomplete-validate-input-field"
+        )
+        self.session.page.fill(
+            "#equitySymbolLookup-block-autocomplete-validate-input-field",
+            self.symbol,
+        )
+        self.session.page.press(
+            "#equitySymbolLookup-block-autocomplete-validate-input-field", "Enter"
         )
-        self.security_description = self.raw_json["securityDescriptionText"]
-        self.security_symbol = self.raw_json["securitySymbolCode"]
+        self.session.page.wait_for_selector("#equityQuoteDetails > section")
+        ask_element = self.session.page.query_selector(
+            "#equityQuoteDetails > section > section > dl > div.askClass.quote-detail-list.col-xs-6.no-padding-right > dd"
+        ).inner_text()
+        ask_string = ask_element.split()
+        bid_element = self.session.page.query_selector(
+            "#equityQuoteDetails > section > section > dl > div.bidClass.quote-detail-list.col-xs-6.no-padding-left > dd"
+        ).inner_text()
+        bid_string = bid_element.split()
+        last_element = self.session.page.query_selector(
+            "#equityQuoteDetails > section > section > dl > div.priceClass.quote-detail-list.list-border.col-xs-6.no-padding-left > dd"
+        ).inner_text()
+        last_string = last_element.split()
+        security_desc = self.session.page.query_selector(
+            "#asset-description"
+        ).inner_text()
+        security_desc_string = security_desc.split("\n", 1)[1].strip()
+        self.ask_price = float(ask_string[0].replace(",", ""))
+        self.ask_exchange_code = ask_string[3].replace("(", "").replace(")", "")
+        self.ask_quantity = int(ask_string[2])
+        self.bid_price = float(bid_string[0].replace(",", ""))
+        self.bid_exchange_code = bid_string[3].replace("(", "").replace(")", "")
+        self.bid_quantity = int(bid_string[2])
+        self.last_trade_price = float(last_string[0].replace(",", ""))
+        self.last_trade_quantity = float(last_string[2].replace(",", ""))
+        self.last_exchange_code = last_string[3].replace("(", "").replace(")", "")
+        self.as_of_time = datetime.now()
+        self.security_description = security_desc_string
 
 
 class SymbolHoldings:
     """
     A class to manage the holdings of a specific account associated with a ChaseSession.
 
     This class provides methods to retrieve and manage information about the holdings of a specific account associated with a given session.
```

### Comparing `chaseinvest-api-0.1.1/chase/urls.py` & `chaseinvest_api-0.1.2/chase/urls.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,30 +52,14 @@
 
     Returns:
         str: The URL for the order page for the specified account.
     """
     return f"https://secure.chase.com/web/auth/dashboard#/dashboard/trade/equity/entry;ai={account_id};sym="
 
 
-def quote_endpoint(ticker):
-    """
-    Generates the URL for the quote endpoint for a specific ticker.
-
-    This function takes a ticker symbol as an argument and returns the URL for the
-    quote endpoint for that ticker on the Chase website.
-
-    Args:
-        ticker (str): The ticker symbol for which to generate the URL.
-
-    Returns:
-        str: The URL for the quote endpoint for the specified ticker.
-    """
-    return f"https://secure.chase.com/svc/wr/dwm/secure/gateway/investments/servicing/inquiry-maintenance/digital-equity-quote/v1/quotes?securitySymbolCode={ticker}&securityValidateIndicator=true"
-
-
 def order_preview_page(account_id):
     """
     Generates the URL for the order preview page for a specific account.
 
     This function takes an account ID as an argument and returns the URL for the
     order preview page for that account on the Chase website.
```

### Comparing `chaseinvest-api-0.1.1/chaseinvest_api.egg-info/PKG-INFO` & `chaseinvest_api-0.1.2/chaseinvest_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chaseinvest-api
-Version: 0.1.1
+Version: 0.1.2
 Summary: An unofficial API for Chase Invest
 Home-page: https://github.com/MaxxRK/chaseinvest-api
-Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.2.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: CHASE,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
@@ -23,15 +23,15 @@
 Requires-Dist: playwright-stealth
 
 # chaseinvest-api
  A reverse-engineered python API to interact with the Chase Trading platform.
 
  This is not an official api! This api's functionality may change at any time.
 
- This api provides a means of buying and selling stocks through Chase. It uses selenium-wire to scrape response data and selenium to interact with the website.
+ This api provides a means of buying and selling stocks through Chase. It uses playwright to scrape response data and to interact with the website.
 
  ---
 
 ## Contribution
 I am new to coding and new to open-source. I would love any help and suggestions!
 
 ## Setup
@@ -41,15 +41,15 @@
 ```
 This package requires playwright. After installing chaseinvest-api, you will need to finish the install of playwright. You can do this in most cases by running the command:
 ```
 playwright install
 ```
 If you would like some more information on this, you can find it [here](https://playwright.dev/python/docs/intro).
 
-## Quikstart
+## Quickstart
 The code below will: 
 - Login and print account info. 
 - Get a quote for 'INTC' and print out the information
 - Place a market order for 'INTC' on the first account in the `account_numbers` list
 - Print out the order confirmation
 
 ```
@@ -183,8 +183,9 @@
  - [x] Get placed order status
 
 ## TO DO
  - [ ] Cancel placed orders
  - [ ] Options
  - [ ] Give me some Ideas!
 
-[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/O5O6PTOYG)  
+## If you would like to support me, you can do so here:
+[![GitHub Sponsors](https://img.shields.io/github/sponsors/maxxrk?style=social)](https://github.com/sponsors/maxxrk)
```

### Comparing `chaseinvest-api-0.1.1/setup.py` & `chaseinvest_api-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="chaseinvest-api",
-    version="0.1.1",
+    version="0.1.2",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Chase Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/chaseinvest-api",
-    download_url="https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.1.tar.gz",
+    download_url="https://github.com/MaxxRK/chaseinvest-api/archive/refs/tags/v0.1.2.tar.gz",
     keywords=["CHASE", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["chase"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `chaseinvest-api-0.1.1/tests/test.py` & `chaseinvest_api-0.1.2/tests/test.py`

 * *Files identical despite different names*


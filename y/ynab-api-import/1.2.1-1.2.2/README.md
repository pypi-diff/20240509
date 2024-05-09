# Comparing `tmp/ynab_api_import-1.2.1.tar.gz` & `tmp/ynab_api_import-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_api_import-1.2.1.tar", max compression
+gzip compressed data, was "ynab_api_import-1.2.2.tar", max compression
```

## Comparing `ynab_api_import-1.2.1.tar` & `ynab_api_import-1.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35148 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/LICENSE
--rw-r--r--   0        0        0     6515 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/README.md
--rw-r--r--   0        0        0      832 2024-04-13 06:36:19.342345 ynab_api_import-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/__init__.py
--rw-r--r--   0        0        0     1373 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/accountclient.py
--rw-r--r--   0        0        0     1465 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/accountfetcher.py
--rw-r--r--   0        0        0      340 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/memocleaner.py
--rw-r--r--   0        0        0      757 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/models/config.py
--rw-r--r--   0        0        0      272 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/models/exceptions.py
--rw-r--r--   0        0        0     1466 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/models/transaction.py
--rw-r--r--   0        0        0     2913 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/requisitionhandler.py
--rw-r--r--   0        0        0     6957 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/ynabapiimport.py
--rw-r--r--   0        0        0     1036 2024-04-13 06:36:05.018419 ynab_api_import-1.2.1/ynabapiimport/ynabclient.py
--rw-r--r--   0        0        0     7324 1970-01-01 00:00:00.000000 ynab_api_import-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/LICENSE
+-rw-r--r--   0        0        0     6588 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/README.md
+-rw-r--r--   0        0        0      832 2024-05-09 05:48:28.113771 ynab_api_import-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/__init__.py
+-rw-r--r--   0        0        0     1373 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/accountclient.py
+-rw-r--r--   0        0        0     1465 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/accountfetcher.py
+-rw-r--r--   0        0        0      340 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/memocleaner.py
+-rw-r--r--   0        0        0      757 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/models/config.py
+-rw-r--r--   0        0        0      272 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/models/exceptions.py
+-rw-r--r--   0        0        0     1466 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/models/transaction.py
+-rw-r--r--   0        0        0     2913 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/requisitionhandler.py
+-rw-r--r--   0        0        0     7240 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/ynabapiimport.py
+-rw-r--r--   0        0        0     1036 2024-05-09 05:48:14.225765 ynab_api_import-1.2.2/ynabapiimport/ynabclient.py
+-rw-r--r--   0        0        0     7397 1970-01-01 00:00:00.000000 ynab_api_import-1.2.2/PKG-INFO
```

### Comparing `ynab_api_import-1.2.1/LICENSE` & `ynab_api_import-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.2.1/README.md` & `ynab_api_import-1.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # ynab-api-import
 
 [![GitHub Release](https://img.shields.io/github/release/dnbasta/ynab-api-import?style=flat)]() 
 [![Github Release](https://img.shields.io/maintenance/yes/2100)]()
+[![Monthly downloads](https://img.shields.io/pypi/dm/ynab-api-import)]()
 
 [!["Buy Me A Coffee"](https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/dnbasta)
 
 This library enables importing YNAB transactions via the 
 [Gocardless Bank Account Data API (formerly Nordigen)](https://gocardless.com/bank-account-data/). 
 It is pretty helpful for cases in which your bank is not covered by YNABs native import functionality.
```

### Comparing `ynab_api_import-1.2.1/pyproject.toml` & `ynab_api_import-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry-core.masonry.api"
 
 [tool.poetry]
 name = "ynab-api-import"
-version = "1.2.1"
+version = "1.2.2"
 authors = ["Daniel Basta <ynab@basta.info>"]
 description = "Library to import bank transactions via API into You Need A Budget (YNAB)"
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabapiimport'}]
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -17,15 +17,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = '>=3.8,<4.0'
 pyyaml = '>=6.0'
 requests = '>=2.28'
 nordigen = '>=1.4'
-pytest = "^8.1.1"
+pytest = "^8.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 
 [poetry.urls]
 "Homepage" = "https://github.com/dnbasta/ynab-api-import"
 "Bug Tracker" = "https://github.com/dnbasta/ynab-api-import/issues"
```

### Comparing `ynab_api_import-1.2.1/ynabapiimport/accountclient.py` & `ynab_api_import-1.2.2/ynabapiimport/accountclient.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.2.1/ynabapiimport/accountfetcher.py` & `ynab_api_import-1.2.2/ynabapiimport/accountfetcher.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.2.1/ynabapiimport/models/config.py` & `ynab_api_import-1.2.2/ynabapiimport/models/config.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.2.1/ynabapiimport/models/transaction.py` & `ynab_api_import-1.2.2/ynabapiimport/models/transaction.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.2.1/ynabapiimport/requisitionhandler.py` & `ynab_api_import-1.2.2/ynabapiimport/requisitionhandler.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.2.1/ynabapiimport/ynabapiimport.py` & `ynab_api_import-1.2.2/ynabapiimport/ynabapiimport.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 		:param secret_id: Secret id from GoCardless
 		:param secret_key: Secret Key from GoCardless
 		:param token: YNAB token
 		:param reference: self chosen reference string to identify connection in GoCardless
 		:param budget_id: YNAB budget id
 		:param account_id: YNAB account id
 		:param resource_id: GoCardless resource id to specify accounts in case multiple are available
-		:raises NoRequisitionError: if GoCardless connection is not valid
-		:raises NoAccountError: if no account is available in authorized GoCardless connection
-		:raises MultipleAccountsError: if multiple accounts are available in authorized GoCardless connection
 		"""
 		self.logger = self._set_up_logger()
 		self.reference = reference
 		self.resource_id = resource_id
 		self._ynab_client = YnabClient(token=token, account_id=account_id, budget_id=budget_id)
 		self._api_client = NordigenClient(secret_id=secret_id, secret_key=secret_key)
 		self._api_client.generate_token()
-		self._account_client = AccountClient.from_api_client(client=self._api_client, reference=self.reference,
-										  resource_id=self.resource_id)
+
+	@property
+	def _account_client(self):
+		return AccountClient.from_api_client(client=self._api_client, reference=self.reference,
+									  resource_id=self.resource_id)
 
 	@classmethod
 	def from_yaml(cls, path: str):
 		"""
 		Creates instance from provided yaml file
 		:param path: path to yaml configuration file
 		:return: instance of YnabApiImport
@@ -68,18 +68,20 @@
 
 	def import_transactions(self, startdate: date = None, memo_regex: str = None) -> int:
 		"""
 		Import bank transactions via GoCardless to YNAB. The method will only import booked transactions and ignore pending ones.
 		:param startdate: date from which to start importing. Will only work for up to max_history_days available for the bank. If not specified will fetch for last 90 days
 		:param memo_regex: regex pattern to parse memos from bank transactions
 		:return: count of processed transactions
+		:raises NoRequisitionError: if GoCardless connection is not valid
+		:raises NoAccountError: if no account is available in authorized GoCardless connection
+		:raises MultipleAccountsError: if multiple accounts are available in authorized GoCardless connection
 		"""
 		if startdate is None:
 			startdate = date.today() - timedelta(days=90)
-
 		transactions = self._account_client.fetch_transactions(startdate=startdate)
 
 		if memo_regex:
 			mc = MemoCleaner(memo_regex=memo_regex)
 			transactions = [mc.clean(t) for t in transactions]
 
 		i = self._ynab_client.insert(transactions)
@@ -87,14 +89,17 @@
 		return i
 
 	def compare_balances(self):
 		"""
 		Compares balance variants for the account (e.g. expected, closingBooked) from API and from YNAB. The method
 		compares the plain balance values as well as the balances minus the sum of still pending transactions.
 		:raises BalancesDontMatchError: if none of the API returned balances for the account match with the one in YNAB
+		:raises NoRequisitionError: if GoCardless connection is not valid
+		:raises NoAccountError: if no account is available in authorized GoCardless connection
+		:raises MultipleAccountsError: if multiple accounts are available in authorized GoCardless connection
 		"""
 		ab, ap = self._account_client.fetch_balances()
 		yb = self._ynab_client.fetch_balance()
 		if yb not in ab.values() and yb not in [b - ap for b in ab.values()]:
 			raise BalancesDontMatchError({'api': ab, 'ynab': yb, 'pending': ap})
 		self.logger.info(f'balances match for {self.reference}')
```

### Comparing `ynab_api_import-1.2.1/ynabapiimport/ynabclient.py` & `ynab_api_import-1.2.2/ynabapiimport/ynabclient.py`

 * *Files identical despite different names*

### Comparing `ynab_api_import-1.2.1/PKG-INFO` & `ynab_api_import-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: ynab-api-import
-Version: 1.2.1
+Version: 1.2.2
 Summary: Library to import bank transactions via API into You Need A Budget (YNAB)
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: nordigen (>=1.4)
-Requires-Dist: pytest (>=8.1.1,<9.0.0)
+Requires-Dist: pytest (>=8.2.0,<9.0.0)
 Requires-Dist: pyyaml (>=6.0)
 Requires-Dist: requests (>=2.28)
 Description-Content-Type: text/markdown
 
 # ynab-api-import
 
 [![GitHub Release](https://img.shields.io/github/release/dnbasta/ynab-api-import?style=flat)]() 
 [![Github Release](https://img.shields.io/maintenance/yes/2100)]()
+[![Monthly downloads](https://img.shields.io/pypi/dm/ynab-api-import)]()
 
 [!["Buy Me A Coffee"](https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/dnbasta)
 
 This library enables importing YNAB transactions via the 
 [Gocardless Bank Account Data API (formerly Nordigen)](https://gocardless.com/bank-account-data/). 
 It is pretty helpful for cases in which your bank is not covered by YNABs native import functionality.
```


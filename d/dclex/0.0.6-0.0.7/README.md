# Comparing `tmp/dclex-0.0.6.tar.gz` & `tmp/dclex-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dclex-0.0.6.tar", last modified: Fri Apr  5 14:10:04 2024, max compression
+gzip compressed data, was "dclex-0.0.7.tar", last modified: Thu May  9 11:53:35 2024, max compression
```

## Comparing `dclex-0.0.6.tar` & `dclex-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.566264 dclex-0.0.6/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     8250 2024-01-31 17:39:20.000000 dclex-0.0.6/LICENSE
--rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-04-05 14:10:04.566264 dclex-0.0.6/PKG-INFO
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      450 2024-04-05 14:00:22.000000 dclex-0.0.6/README.md
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      739 2024-04-05 14:05:35.000000 dclex-0.0.6/pyproject.toml
--rw-rw-r--   0 clouds    (1001) clouds    (1001)       38 2024-04-05 14:10:04.566264 dclex-0.0.6/setup.cfg
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.558265 dclex-0.0.6/src/
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.562265 dclex-0.0.6/src/dclex/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      208 2024-03-04 19:14:07.000000 dclex-0.0.6/src/dclex/__init__.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    11488 2024-04-05 13:54:10.000000 dclex-0.0.6/src/dclex/dclex.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    12964 2024-04-05 13:53:24.000000 dclex-0.0.6/src/dclex/dclex_client.py
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.562265 dclex-0.0.6/src/dclex/resources/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    19297 2024-02-02 17:33:59.000000 dclex-0.0.6/src/dclex/resources/digital_identity_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)    15662 2024-02-02 17:33:59.000000 dclex-0.0.6/src/dclex/resources/factory_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6200 2024-02-02 17:33:59.000000 dclex-0.0.6/src/dclex/resources/usdc_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     9883 2024-02-02 17:33:59.000000 dclex-0.0.6/src/dclex/resources/vault_contract_abi.json
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1188 2024-03-01 16:20:01.000000 dclex-0.0.6/src/dclex/settings.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     2285 2024-03-01 16:30:00.000000 dclex-0.0.6/src/dclex/types.py
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.566264 dclex-0.0.6/src/dclex.egg-info/
--rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/PKG-INFO
--rw-rw-r--   0 clouds    (1001) clouds    (1001)      580 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/SOURCES.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)        1 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/dependency_links.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)       60 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/requires.txt
--rw-rw-r--   0 clouds    (1001) clouds    (1001)        6 2024-04-05 14:10:04.000000 dclex-0.0.6/src/dclex.egg-info/top_level.txt
-drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-04-05 14:10:04.566264 dclex-0.0.6/tests/
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1167 2024-03-04 19:14:07.000000 dclex-0.0.6/tests/test_account.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6062 2024-03-04 19:14:07.000000 dclex-0.0.6/tests/test_orders.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     1534 2024-04-05 13:55:04.000000 dclex-0.0.6/tests/test_stocks.py
--rw-rw-r--   0 clouds    (1001) clouds    (1001)     6753 2024-03-04 19:14:07.000000 dclex-0.0.6/tests/test_transfers.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.567085 dclex-0.0.7/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     8250 2024-01-31 17:39:20.000000 dclex-0.0.7/LICENSE
+-rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-09 11:53:35.567085 dclex-0.0.7/PKG-INFO
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      450 2024-04-05 14:00:22.000000 dclex-0.0.7/README.md
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      739 2024-05-09 11:43:37.000000 dclex-0.0.7/pyproject.toml
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)       38 2024-05-09 11:53:35.567085 dclex-0.0.7/setup.cfg
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.563085 dclex-0.0.7/src/
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.563085 dclex-0.0.7/src/dclex/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      208 2024-05-09 11:47:56.000000 dclex-0.0.7/src/dclex/__init__.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    11676 2024-05-09 11:47:57.000000 dclex-0.0.7/src/dclex/dclex.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    12999 2024-05-09 11:47:57.000000 dclex-0.0.7/src/dclex/dclex_client.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.567085 dclex-0.0.7/src/dclex/resources/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    19297 2024-02-02 17:33:59.000000 dclex-0.0.7/src/dclex/resources/digital_identity_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)    15662 2024-02-02 17:33:59.000000 dclex-0.0.7/src/dclex/resources/factory_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     6200 2024-02-02 17:33:59.000000 dclex-0.0.7/src/dclex/resources/usdc_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     9883 2024-02-02 17:33:59.000000 dclex-0.0.7/src/dclex/resources/vault_contract_abi.json
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1188 2024-03-01 16:20:01.000000 dclex-0.0.7/src/dclex/settings.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     2285 2024-03-01 16:30:00.000000 dclex-0.0.7/src/dclex/types.py
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.567085 dclex-0.0.7/src/dclex.egg-info/
+-rw-r--r--   0 clouds    (1001) clouds    (1001)     9844 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/PKG-INFO
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)      580 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/SOURCES.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)        1 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/dependency_links.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)       60 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/requires.txt
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)        6 2024-05-09 11:53:35.000000 dclex-0.0.7/src/dclex.egg-info/top_level.txt
+drwxrwxr-x   0 clouds    (1001) clouds    (1001)        0 2024-05-09 11:53:35.567085 dclex-0.0.7/tests/
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1167 2024-03-04 19:14:07.000000 dclex-0.0.7/tests/test_account.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     6062 2024-03-04 19:14:07.000000 dclex-0.0.7/tests/test_orders.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     1534 2024-04-05 13:55:04.000000 dclex-0.0.7/tests/test_stocks.py
+-rw-rw-r--   0 clouds    (1001) clouds    (1001)     7028 2024-05-09 11:47:57.000000 dclex-0.0.7/tests/test_transfers.py
```

### Comparing `dclex-0.0.6/LICENSE` & `dclex-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/PKG-INFO` & `dclex-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dclex
-Version: 0.0.6
+Version: 0.0.7
 Summary: DCLEX python library
 License: DCLEX API Non-Commercial License
         
         This DCLEX API Non-Commercial License ("License") is an agreement between DCLEX inc. ("DCLEX") and You, and governs Your use of the API Code. By loging to your DCLEX account programmatically , you acknowledge that You consent to be legally bound by this Agreement.
         
         1. Introduction.
         1.1 DCLEX has developed application program interface ("API") code to permit its customers to use their own internal proprietary software tools in managing their accounts with DCLEX. This License is intended only for users who wish to use the API Code by itself as is, or in connection with or for the development of their own internal proprietary tools to manage their own DCLEX accounts. This License is NOT for anybody who is developing software applications that they wish to: (a) sell to third party users for a fee, or (b) give to third party users to generate an indirect financial benefit (e.g., commissions). If You wish to make a software application for the purposes described in the preceding sentence then please us at info@dclex.com.
```

### Comparing `dclex-0.0.6/pyproject.toml` & `dclex-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dclex"
-version = "0.0.6"
+version = "0.0.7"
 description = "DCLEX python library"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 classifiers = [
     "Intended Audience :: Financial and Insurance Industry",
     "Programming Language :: Python :: 3.7",
```

### Comparing `dclex-0.0.6/src/dclex/dclex.py` & `dclex-0.0.7/src/dclex/dclex.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,24 +123,26 @@
         )
         return self._build_and_send_transaction(
             usdc_contract.functions.transfer(
                 VAULT_CONTRACT_ADDRESS, int(amount * Decimal(10**6))
             )
         )
 
-    def withdraw_usdc(self, amount: Decimal) -> str:
+    def initialize_usdc_withdrawal(self, amount: Decimal):
         account_status = self._dclex_client.get_account_status()
         if account_status not in [AccountStatus.VERIFIED, AccountStatus.DID_MINTED]:
             raise AccountNotVerified()
 
         try:
-            withdrawal_id = self._dclex_client.initialize_usdc_withdrawal(amount=amount)
+            return self._dclex_client.initialize_usdc_withdrawal(amount=amount)
         except APIError as exc:
             if exc.error_code == "INSUFFICIENT_FUNDS":
                 raise NotEnoughFunds()
+
+    def finalize_usdc_withdrawal(self, withdrawal_id: int, amount: Decimal) -> str:
         signature = self._dclex_client.get_withdraw_signature(
             withdrawal_id=withdrawal_id,
         )
 
         vault_contract_address = self._web3.to_checksum_address(VAULT_CONTRACT_ADDRESS)
         vault_contract = self._web3.eth.contract(
             address=vault_contract_address, abi=VAULT_CONTRACT_ABI
@@ -182,27 +184,31 @@
                     "account": self._account.address,
                     "nonce": int.from_bytes(bytes.fromhex(signature.nonce[2:]), "big"),
                 },
                 bytes.fromhex(signature.signature),
             )
         )
 
-    def withdraw_stock_token(self, stock_symbol: str, amount: int) -> str:
+    def initialize_stock_withdrawal(self, stock_symbol: str, amount: int):
         account_status = self._dclex_client.get_account_status()
         if account_status != AccountStatus.DID_MINTED:
             raise AccountNotVerified()
 
         try:
-            withdrawal_id = self._dclex_client.initialize_stock_withdrawal(
+            return self._dclex_client.initialize_stock_withdrawal(
                 amount=amount,
                 asset_type=stock_symbol,
             )
         except APIError as exc:
             if exc.error_code == "INSUFFICIENT_FUNDS":
                 raise NotEnoughFunds()
+
+    def finalize_stock_withdrawal(
+        self, withdrawal_id: int, stock_symbol: str, amount: int
+    ) -> str:
         signature = self._dclex_client.get_withdraw_signature(
             withdrawal_id=withdrawal_id,
         )
 
         factory_contract_address = self._web3.to_checksum_address(
             FACTORY_CONTRACT_ADDRESS
         )
```

### Comparing `dclex-0.0.6/src/dclex/dclex_client.py` & `dclex-0.0.7/src/dclex/dclex_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,18 @@
         }
 
     def prices_stream_access_token(self) -> str:
         response = self._authorized_get("/prices-stream-access-token/")
         return response["pricesStreamAccessToken"]
 
     def prices_stream(self, prices_stream_access_token: str):
-        for sse_message in SSEClient(f"{DCLEX_BASE_URL}/prices-stream/", params={"token": prices_stream_access_token}):
+        for sse_message in SSEClient(
+            f"{DCLEX_BASE_URL}/prices-stream/",
+            params={"token": prices_stream_access_token},
+        ):
             price_data = json.loads(sse_message.data)
             yield Price(
                 symbol=price_data["symbol"],
                 last_price=Decimal(price_data["price"]),
                 timestamp=self._parse_timestamp(price_data["timestamp"]),
                 percentage_change=Decimal(price_data["percentageChange"]),
             )
```

### Comparing `dclex-0.0.6/src/dclex/resources/digital_identity_contract_abi.json` & `dclex-0.0.7/src/dclex/resources/digital_identity_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/src/dclex/resources/factory_contract_abi.json` & `dclex-0.0.7/src/dclex/resources/factory_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/src/dclex/resources/usdc_contract_abi.json` & `dclex-0.0.7/src/dclex/resources/usdc_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/src/dclex/resources/vault_contract_abi.json` & `dclex-0.0.7/src/dclex/resources/vault_contract_abi.json`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/src/dclex/settings.py` & `dclex-0.0.7/src/dclex/settings.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/src/dclex/types.py` & `dclex-0.0.7/src/dclex/types.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/src/dclex.egg-info/PKG-INFO` & `dclex-0.0.7/src/dclex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dclex
-Version: 0.0.6
+Version: 0.0.7
 Summary: DCLEX python library
 License: DCLEX API Non-Commercial License
         
         This DCLEX API Non-Commercial License ("License") is an agreement between DCLEX inc. ("DCLEX") and You, and governs Your use of the API Code. By loging to your DCLEX account programmatically , you acknowledge that You consent to be legally bound by this Agreement.
         
         1. Introduction.
         1.1 DCLEX has developed application program interface ("API") code to permit its customers to use their own internal proprietary software tools in managing their accounts with DCLEX. This License is intended only for users who wish to use the API Code by itself as is, or in connection with or for the development of their own internal proprietary tools to manage their own DCLEX accounts. This License is NOT for anybody who is developing software applications that they wish to: (a) sell to third party users for a fee, or (b) give to third party users to generate an indirect financial benefit (e.g., commissions). If You wish to make a software application for the purposes described in the preceding sentence then please us at info@dclex.com.
```

### Comparing `dclex-0.0.6/src/dclex.egg-info/SOURCES.txt` & `dclex-0.0.7/src/dclex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/tests/test_account.py` & `dclex-0.0.7/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/tests/test_orders.py` & `dclex-0.0.7/tests/test_orders.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/tests/test_stocks.py` & `dclex-0.0.7/tests/test_stocks.py`

 * *Files identical despite different names*

### Comparing `dclex-0.0.6/tests/test_transfers.py` & `dclex-0.0.7/tests/test_transfers.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,41 +20,42 @@
     wait_for_transaction(tx_hash, provider_url)
 
     sleep(3)
 
     assert dclex.get_usdc_ledger_balance() - usdc_ledger_balance_before == 100
     assert dclex.get_usdc_available_balance() - usdc_available_balance_before == 100
 
-    tx_hash = dclex.withdraw_usdc(Decimal(100))
+    withdrawal_id = dclex.initialize_usdc_withdrawal(Decimal(100))
+    tx_hash = dclex.finalize_usdc_withdrawal(withdrawal_id, Decimal(100))
     wait_for_transaction(tx_hash, provider_url)
 
-    sleep(3)
+    sleep(15)
 
-    assert dclex.get_usdc_ledger_balance() == usdc_ledger_balance_before
-    assert dclex.get_usdc_available_balance() == usdc_available_balance_before
+    assert dclex.get_usdc_ledger_balance() == usdc_ledger_balance_before - 100
+    assert dclex.get_usdc_available_balance() == usdc_available_balance_before - 100
 
 
 def test_deposit_usdc_raises_when_user_is_not_verified(dclex_unverified):
     dclex_unverified.login()
     with pytest.raises(AccountNotVerified):
         dclex_unverified.deposit_usdc(Decimal(100))
 
 
-def test_withdraw_usdc_raises_when_user_is_not_verified(dclex_unverified):
+def test_initialize_usdc_withdrawal_raises_when_user_is_not_verified(dclex_unverified):
     dclex_unverified.login()
     with pytest.raises(AccountNotVerified):
-        dclex_unverified.withdraw_usdc(Decimal(100))
+        dclex_unverified.initialize_usdc_withdrawal(Decimal(100))
 
 
-def test_withdraw_usdc_raises_when_not_enough_funds(dclex, provider_url):
+def test_initialize_usdc_withdrawal_raises_when_not_enough_funds(dclex, provider_url):
     dclex.login()
     usdc_available_balance = dclex.get_usdc_available_balance()
 
     with pytest.raises(NotEnoughFunds):
-        dclex.withdraw_usdc(Decimal(usdc_available_balance + 1))
+        dclex.initialize_usdc_withdrawal(Decimal(usdc_available_balance + 1))
 
 
 def test_withdraw_and_deposit_stock(dclex, provider_url):
     dclex.login()
 
     tx_hash = dclex.deposit_usdc(Decimal(200))
     wait_for_transaction(tx_hash, provider_url)
@@ -62,17 +63,18 @@
 
     dclex.create_limit_order(OrderSide.BUY, "AAPL", 1, Decimal(190))
     sleep(30)
 
     aapl_available_balance_before = dclex.get_stock_available_balance("AAPL")
     aapl_ledger_balance_before = dclex.get_stock_ledger_balance("AAPL")
 
-    tx_hash = dclex.withdraw_stock_token("AAPL", 1)
+    withdrawal_id = dclex.initialize_stock_withdrawal("AAPL", 1)
+    tx_hash = dclex.finalize_stock_withdrawal(withdrawal_id, "AAPL", 1)
     wait_for_transaction(tx_hash, provider_url)
-    sleep(3)
+    sleep(20)
 
     assert (
         dclex.get_stock_available_balance("AAPL") - aapl_available_balance_before == -1
     )
     assert dclex.get_stock_ledger_balance("AAPL") - aapl_ledger_balance_before == -1
 
     tx_hash = dclex.deposit_stock_token("AAPL", 1)
@@ -85,26 +87,26 @@
 
 def test_deposit_stock_raises_when_user_is_not_verified(dclex_unverified):
     dclex_unverified.login()
     with pytest.raises(AccountNotVerified):
         dclex_unverified.deposit_stock_token("AAPL", Decimal(1))
 
 
-def test_withdraw_stock_raises_when_user_is_not_verified(dclex_unverified):
+def test_initialize_stock_withdrawal_raises_when_user_is_not_verified(dclex_unverified):
     dclex_unverified.login()
     with pytest.raises(AccountNotVerified):
-        dclex_unverified.withdraw_stock_token("AAPL", Decimal(1))
+        dclex_unverified.initialize_stock_withdrawal("AAPL", Decimal(1))
 
 
-def test_withdraw_stock_raises_when_not_enough_funds(dclex, provider_url):
+def test_initialize_stock_withdrawal_raises_when_not_enough_funds(dclex, provider_url):
     dclex.login()
     available_balance = dclex.get_stock_available_balance("AAPL")
 
     with pytest.raises(NotEnoughFunds):
-        dclex.withdraw_stock_token("AAPL", Decimal(available_balance + 1))
+        dclex.initialize_stock_withdrawal("AAPL", available_balance + 1)
 
 
 def test_usdc_pending_transfers(dclex, provider_url):
     dclex.login()
 
     assert dclex.pending_transfers() == []
```


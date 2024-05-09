# Comparing `tmp/defillama-2.2.1.tar.gz` & `tmp/defillama-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defillama-2.2.1.tar", last modified: Mon May  6 10:09:41 2024, max compression
+gzip compressed data, was "defillama-2.3.0.tar", last modified: Thu May  9 16:47:41 2024, max compression
```

## Comparing `defillama-2.2.1.tar` & `defillama-2.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:41.485442 defillama-2.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:41.481442 defillama-2.2.1/DeFiLlama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 10:09:41.000000 defillama-2.2.1/DeFiLlama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 10:09:33.000000 defillama-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-06 10:09:41.485442 defillama-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-06 10:09:33.000000 defillama-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:41.481442 defillama-2.2.1/defillama/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-06 10:09:33.000000 defillama-2.2.1/defillama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-06 10:09:33.000000 defillama-2.2.1/defillama/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-05-06 10:09:33.000000 defillama-2.2.1/defillama/defillama.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 10:09:41.485442 defillama-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-06 10:09:33.000000 defillama-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 10:09:41.481442 defillama-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-06 10:09:33.000000 defillama-2.2.1/tests/test_defillama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:47:41.653729 defillama-2.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:47:41.653729 defillama-2.3.0/DeFiLlama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-09 16:47:41.000000 defillama-2.3.0/DeFiLlama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-09 16:47:41.000000 defillama-2.3.0/DeFiLlama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:47:41.000000 defillama-2.3.0/DeFiLlama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 16:47:41.000000 defillama-2.3.0/DeFiLlama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 16:47:41.000000 defillama-2.3.0/DeFiLlama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 16:47:33.000000 defillama-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-09 16:47:41.653729 defillama-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-09 16:47:33.000000 defillama-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:47:41.653729 defillama-2.3.0/defillama/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-09 16:47:33.000000 defillama-2.3.0/defillama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-09 16:47:33.000000 defillama-2.3.0/defillama/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12282 2024-05-09 16:47:33.000000 defillama-2.3.0/defillama/defillama.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:47:41.653729 defillama-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-09 16:47:33.000000 defillama-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:47:41.653729 defillama-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-05-09 16:47:33.000000 defillama-2.3.0/tests/test_defillama.py
```

### Comparing `defillama-2.2.1/DeFiLlama.egg-info/PKG-INFO` & `defillama-2.3.0/DeFiLlama.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeFiLlama
-Version: 2.2.1
+Version: 2.3.0
 Summary: Unofficial DeFi Llama API client.
 Home-page: https://github.com/itzmestar/DeFiLlama
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -15,19 +15,20 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.18.4
 
 # DeFiLlama
 
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31014/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3119/)
+[![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-3123/)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Build](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml/badge.svg)](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml)
 
 
 ### Unofficial [DeFi Llama API](https://defillama.com/home) client in python
@@ -61,13 +62,24 @@
 # Get all protocols data
 response = llama.get_all_protocols()
 
 # Get a protocol data
 response = llama.get_protocol(name='uniswap')
 
 ```
+
+Data from stablecoins dashboard
+
+```
+# List all stablecoins along with their circulating amounts
+response = llama.get_stablecoins()
+
+# Get historical mcap sum of all stablecoins in a chain
+response = llama.get_stablecoins_chains_all_historical_mcap_sum(chain='Ethereum', stablecoin_id=1)
+```
+
 -------
 #### Donate & Help maintain the library
 
 [![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
 
 -------
```

### Comparing `defillama-2.2.1/LICENSE` & `defillama-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `defillama-2.2.1/PKG-INFO` & `defillama-2.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeFiLlama
-Version: 2.2.1
+Version: 2.3.0
 Summary: Unofficial DeFi Llama API client.
 Home-page: https://github.com/itzmestar/DeFiLlama
 Author: Tarique Anwer
 Author-email: itzmetariq@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -15,19 +15,20 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.18.4
 
 # DeFiLlama
 
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31014/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3119/)
+[![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-3123/)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Build](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml/badge.svg)](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml)
 
 
 ### Unofficial [DeFi Llama API](https://defillama.com/home) client in python
@@ -61,13 +62,24 @@
 # Get all protocols data
 response = llama.get_all_protocols()
 
 # Get a protocol data
 response = llama.get_protocol(name='uniswap')
 
 ```
+
+Data from stablecoins dashboard
+
+```
+# List all stablecoins along with their circulating amounts
+response = llama.get_stablecoins()
+
+# Get historical mcap sum of all stablecoins in a chain
+response = llama.get_stablecoins_chains_all_historical_mcap_sum(chain='Ethereum', stablecoin_id=1)
+```
+
 -------
 #### Donate & Help maintain the library
 
 [![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
 
 -------
```

### Comparing `defillama-2.2.1/README.md` & `defillama-2.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # DeFiLlama
 
-[![Python 3.6](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310/)
+[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-31014/)
+[![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3119/)
+[![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-3123/)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 [![Build](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml/badge.svg)](https://github.com/itzmestar/DeFiLlama/actions/workflows/python-package.yml)
 
 
 ### Unofficial [DeFi Llama API](https://defillama.com/home) client in python
@@ -42,13 +43,24 @@
 # Get all protocols data
 response = llama.get_all_protocols()
 
 # Get a protocol data
 response = llama.get_protocol(name='uniswap')
 
 ```
+
+Data from stablecoins dashboard
+
+```
+# List all stablecoins along with their circulating amounts
+response = llama.get_stablecoins()
+
+# Get historical mcap sum of all stablecoins in a chain
+response = llama.get_stablecoins_chains_all_historical_mcap_sum(chain='Ethereum', stablecoin_id=1)
+```
+
 -------
 #### Donate & Help maintain the library
 
 [![Paypal](qrcode.png)](https://www.paypal.com/ncp/payment/KLFNJN7SH39EN)
 
 -------
```

### Comparing `defillama-2.2.1/defillama/defillama.py` & `defillama-2.3.0/defillama/defillama.py`

 * *Files 21% similar despite different names*

```diff
@@ -202,14 +202,76 @@
         """
         Get the closest block to a timestamp
         """
         path = f"/block/{chain}/{timestamp}"
 
         return self._get(path)
 
+    # ##### Stablecoins EPs ###### #
+
+    def get_stablecoins(self, include_prices: bool = True):
+        """
+        List all stablecoins along with their circulating amounts
+        """
+        path = "https://stablecoins.llama.fi/stablecoins"
+
+        params = {
+            'includePrices': include_prices
+        }
+
+        return self._get(path, params=params, full_url=True)
+
+    def get_stablecoins_all_historical_mcap_sum(self, stablecoin_id: int):
+        """
+        Get historical mcap sum of all stablecoins
+        """
+        path = "https://stablecoins.llama.fi/stablecoincharts/all"
+
+        params = {
+            'stablecoin': stablecoin_id
+        }
+
+        return self._get(path, params=params, full_url=True)
+
+    def get_stablecoins_chains_all_historical_mcap_sum(self, chain: str, stablecoin_id: int):
+        """
+        Get historical mcap sum of all stablecoins in a chain
+        """
+        path = f"https://stablecoins.llama.fi/stablecoincharts/{chain}"
+
+        params = {
+            'stablecoin': stablecoin_id
+        }
+
+        return self._get(path, params=params, full_url=True)
+
+    def get_stablecoins_historical_mcap_n_chain_distribution(self, stablecoin_id: int):
+        """
+        Get historical mcap & historical chain distribution of a stablecoin
+        """
+        path = f"https://stablecoins.llama.fi/stablecoin/{stablecoin_id}"
+
+        return self._get(path, full_url=True)
+
+    def get_stablecoins_all_current_mcap_sum(self):
+        """
+        Get current mcap sum of all stablecoins on each chain
+        """
+        path = f"https://stablecoins.llama.fi/stablecoinchains"
+
+        return self._get(path, full_url=True)
+
+    def get_stablecoins_historical_prices(self):
+        """
+        Get historical prices of all stablecoins
+        """
+        path = f"https://stablecoins.llama.fi/stablecoinprices"
+
+        return self._get(path, full_url=True)
+
     # ##### Yields EPs ###### #
 
     def get_pools(self):
         """
         Get the latest data for all pools
         """
         path = 'https://yields.llama.fi/pools'
```

### Comparing `defillama-2.2.1/setup.py` & `defillama-2.3.0/setup.py`

 * *Files identical despite different names*


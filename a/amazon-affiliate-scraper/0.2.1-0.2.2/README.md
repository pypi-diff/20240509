# Comparing `tmp/amazon_affiliate_scraper-0.2.1.tar.gz` & `tmp/amazon_affiliate_scraper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_affiliate_scraper-0.2.1.tar", max compression
+gzip compressed data, was "amazon_affiliate_scraper-0.2.2.tar", max compression
```

## Comparing `amazon_affiliate_scraper-0.2.1.tar` & `amazon_affiliate_scraper-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       35 2024-02-16 15:27:07.522571 amazon_affiliate_scraper-0.2.1/amazon_affiliate/__init__.py
--rw-r--r--   0        0        0     1781 2024-05-09 19:25:47.648877 amazon_affiliate_scraper-0.2.1/amazon_affiliate/client.py
--rw-r--r--   0        0        0      521 2024-05-09 19:30:51.147649 amazon_affiliate_scraper-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1071 2024-02-16 15:17:58.313209 amazon_affiliate_scraper-0.2.1/README.md
--rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 amazon_affiliate_scraper-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-02-16 15:27:07.522571 amazon_affiliate_scraper-0.2.2/amazon_affiliate/__init__.py
+-rw-r--r--   0        0        0     1781 2024-05-09 19:25:47.648877 amazon_affiliate_scraper-0.2.2/amazon_affiliate/client.py
+-rw-r--r--   0        0        0      579 2024-05-09 19:34:30.853513 amazon_affiliate_scraper-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      987 2024-05-09 19:34:09.020645 amazon_affiliate_scraper-0.2.2/README.md
+-rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 amazon_affiliate_scraper-0.2.2/PKG-INFO
```

### Comparing `amazon_affiliate_scraper-0.2.1/amazon_affiliate/client.py` & `amazon_affiliate_scraper-0.2.2/amazon_affiliate/client.py`

 * *Files identical despite different names*

### Comparing `amazon_affiliate_scraper-0.2.1/pyproject.toml` & `amazon_affiliate_scraper-0.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 [tool.poetry]
 name = "amazon-affiliate-scraper"
-version = "0.2.1"
+version = "0.2.2"
 description = "\"A simple library to help a developer who is affiliated with Amazon to automate the process."
 authors = ["Marcuth <example@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "amazon_affiliate" }]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 selenium = "^4.20.0"
 pydantic = "^2.7.1"
 webdriver-manager = "^4.0.1"
 
 
+[tool.poetry.group.dev.dependencies]
+twine = "^5.0.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `amazon_affiliate_scraper-0.2.1/PKG-INFO` & `amazon_affiliate_scraper-0.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-affiliate-scraper
-Version: 0.2.1
+Version: 0.2.2
 Summary: "A simple library to help a developer who is affiliated with Amazon to automate the process.
 License: MIT
 Author: Marcuth
 Author-email: example@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,24 +18,28 @@
 
 ## Quickstart
 
 ### Creating Affiliate URL:
 
 ```py
 from amazon_affiliate import AmazonAffiliate
+import json
 
-def main():
+def get_amazon_cookies() -> list[dict]:
+    with open("www.amazon.com.br.cookies (2).json", "r") as file:
+        cookies = json.load(file)
+        return cookies
+
+def main() -> None:
     amazon_affiliate = AmazonAffiliate(
-        cookies_file_path = "path/to/amazon_cookies.json", # Path to Amazon site cookies
-        origin_url = "https://www.amazon.com.br/", # Amazon root URL in your country
-        webdriver_file_path = "path/to/webdriver.exe", # Path to browser webdriver
-        headless = True # If the browser will appear
+        cookies = get_amazon_cookies(),
+        origin_url = "https://www.amazon.com.br/",
+        headless = False
     )
 
-    # Create an affiliate URL like: https://amzn.to/3qAp1rZ
-    affiliate_url = amazon_affiliate.create_affiliate_url("https://www.amazon.com.br/Introdu%C3%A7%C3%A3o-Programa%C3%A7%C3%A3o-com-Python-Algoritmos/dp/8575227181/?_encoding=UTF8&pd_rd_w=cLgOh&content-id=amzn1.sym.142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_p=142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_r=Q5SHBAZH69HSPBRR2MGS&pd_rd_wg=98FtW&pd_rd_r=ffa375c6-01c9-4e9c-9f87-2aef974a89af&ref_=pd_gw_ci_mcx_mr_hp_atf_m") 
+    affiliate_url = amazon_affiliate.create_affiliate_url("https://www.amazon.com.br/Echo-Dot-5%C2%AA-gera%C3%A7%C3%A3o-Cor-Preta/dp/B09B8VGCR8/?_encoding=UTF8&pd_rd_w=z10q4&content-id=amzn1.sym.52e74d21-088e-4a9d-888d-8b14bf95d4ae&pf_rd_p=52e74d21-088e-4a9d-888d-8b14bf95d4ae&pf_rd_r=6360ZE14T1KEYVFYZMBQ&pd_rd_wg=1fQsD&pd_rd_r=58179dcd-f33a-44a6-9b15-0fd56b159876&ref_=pd_gw_crs_zg_bs_16209062011")
 
     print(affiliate_url)
 
 if __name__ == "__main__":
     main()
 ```
```


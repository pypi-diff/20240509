# Comparing `tmp/amazon-affiliate-scraper-0.1.2.tar.gz` & `tmp/amazon-affiliate-scraper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-affiliate-scraper-0.1.2.tar", last modified: Sun Jun 11 14:19:57 2023, max compression
+gzip compressed data, was "amazon-affiliate-scraper-0.2.0.tar", last modified: Fri Feb 16 15:33:55 2024, max compression
```

## Comparing `amazon-affiliate-scraper-0.1.2.tar` & `amazon-affiliate-scraper-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 14:19:57.648396 amazon-affiliate-scraper-0.1.2/
--rw-rw-rw-   0        0        0     1363 2023-06-11 14:19:57.646398 amazon-affiliate-scraper-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1033 2023-06-11 14:18:23.000000 amazon-affiliate-scraper-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 14:19:57.616397 amazon-affiliate-scraper-0.1.2/amazon_affiliate/
--rw-rw-rw-   0        0        0       26 2023-06-11 13:26:35.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate/__init__.py
--rw-rw-rw-   0        0        0     1613 2023-06-11 13:31:37.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate/client.py
-drwxrwxrwx   0        0        0        0 2023-06-11 14:19:57.644402 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/
--rw-rw-rw-   0        0        0     1363 2023-06-11 14:19:57.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-11 14:19:57.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 14:19:57.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-11 14:19:57.000000 amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 14:19:57.648396 amazon-affiliate-scraper-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      636 2023-06-11 14:18:33.000000 amazon-affiliate-scraper-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-16 15:33:55.621345 amazon-affiliate-scraper-0.2.0/
+-rw-rw-rw-   0        0        0     1397 2024-02-16 15:33:55.619338 amazon-affiliate-scraper-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1071 2024-02-16 15:17:58.000000 amazon-affiliate-scraper-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-02-16 15:33:55.583343 amazon-affiliate-scraper-0.2.0/amazon_affiliate/
+-rw-rw-rw-   0        0        0       35 2024-02-16 15:27:07.000000 amazon-affiliate-scraper-0.2.0/amazon_affiliate/__init__.py
+-rw-rw-rw-   0        0        0     1798 2024-02-16 15:31:55.000000 amazon-affiliate-scraper-0.2.0/amazon_affiliate/client.py
+drwxrwxrwx   0        0        0        0 2024-02-16 15:33:55.617340 amazon-affiliate-scraper-0.2.0/amazon_affiliate_scraper.egg-info/
+-rw-rw-rw-   0        0        0     1397 2024-02-16 15:33:55.000000 amazon-affiliate-scraper-0.2.0/amazon_affiliate_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-02-16 15:33:55.000000 amazon-affiliate-scraper-0.2.0/amazon_affiliate_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-16 15:33:55.000000 amazon-affiliate-scraper-0.2.0/amazon_affiliate_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-02-16 15:33:55.000000 amazon-affiliate-scraper-0.2.0/amazon_affiliate_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-16 15:33:55.621345 amazon-affiliate-scraper-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      652 2024-02-16 15:17:02.000000 amazon-affiliate-scraper-0.2.0/setup.py
```

### Comparing `amazon-affiliate-scraper-0.1.2/PKG-INFO` & `amazon-affiliate-scraper-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: amazon-affiliate-scraper
-Version: 0.1.2
+Version: 0.2.0
 Summary: A simple library to help a developer who is affiliated with Amazon to automate the process.
 Author: Marcuth
-Author-email: marcuth2006@gmail.com
+Author-email: example@gmail.com
 License: MIT License
 Keywords: amazon affiliate scraper
 Description-Content-Type: text/markdown
 
 # Amazon Affiliate - Scraper Tool
 
 ## Quickstart
 
 ### Creating Affiliate URL:
 
 ```py
-from amazon_affiliate import Client
+from amazon_affiliate import AmazonAffiliate
 
 def main():
-    client = Client(
+    amazon_affiliate = AmazonAffiliate(
         cookies_file_path = "path/to/amazon_cookies.json", # Path to Amazon site cookies
         origin_url = "https://www.amazon.com.br/", # Amazon root URL in your country
         webdriver_file_path = "path/to/webdriver.exe", # Path to browser webdriver
         headless = True # If the browser will appear
     )
 
-    # Create an affiliate URL like: https://amzn.to/3qAp1rI
-    affiliate_url = client.create_affiliate_url("https://www.amazon.com.br/Introdu%C3%A7%C3%A3o-Programa%C3%A7%C3%A3o-com-Python-Algoritmos/dp/8575227181/?_encoding=UTF8&pd_rd_w=cLgOh&content-id=amzn1.sym.142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_p=142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_r=Q5SHBAZH69HSPBRR2MGS&pd_rd_wg=98FtW&pd_rd_r=ffa375c6-01c9-4e9c-9f87-2aef974a89af&ref_=pd_gw_ci_mcx_mr_hp_atf_m") 
+    # Create an affiliate URL like: https://amzn.to/3qAp1rZ
+    affiliate_url = amazon_affiliate.create_affiliate_url("https://www.amazon.com.br/Introdu%C3%A7%C3%A3o-Programa%C3%A7%C3%A3o-com-Python-Algoritmos/dp/8575227181/?_encoding=UTF8&pd_rd_w=cLgOh&content-id=amzn1.sym.142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_p=142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_r=Q5SHBAZH69HSPBRR2MGS&pd_rd_wg=98FtW&pd_rd_r=ffa375c6-01c9-4e9c-9f87-2aef974a89af&ref_=pd_gw_ci_mcx_mr_hp_atf_m") 
 
     print(affiliate_url)
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `amazon-affiliate-scraper-0.1.2/README.md` & `amazon-affiliate-scraper-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Amazon Affiliate - Scraper Tool
 
 ## Quickstart
 
 ### Creating Affiliate URL:
 
 ```py
-from amazon_affiliate import Client
+from amazon_affiliate import AmazonAffiliate
 
 def main():
-    client = Client(
+    amazon_affiliate = AmazonAffiliate(
         cookies_file_path = "path/to/amazon_cookies.json", # Path to Amazon site cookies
         origin_url = "https://www.amazon.com.br/", # Amazon root URL in your country
         webdriver_file_path = "path/to/webdriver.exe", # Path to browser webdriver
         headless = True # If the browser will appear
     )
 
-    # Create an affiliate URL like: https://amzn.to/3qAp1rI
-    affiliate_url = client.create_affiliate_url("https://www.amazon.com.br/Introdu%C3%A7%C3%A3o-Programa%C3%A7%C3%A3o-com-Python-Algoritmos/dp/8575227181/?_encoding=UTF8&pd_rd_w=cLgOh&content-id=amzn1.sym.142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_p=142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_r=Q5SHBAZH69HSPBRR2MGS&pd_rd_wg=98FtW&pd_rd_r=ffa375c6-01c9-4e9c-9f87-2aef974a89af&ref_=pd_gw_ci_mcx_mr_hp_atf_m") 
+    # Create an affiliate URL like: https://amzn.to/3qAp1rZ
+    affiliate_url = amazon_affiliate.create_affiliate_url("https://www.amazon.com.br/Introdu%C3%A7%C3%A3o-Programa%C3%A7%C3%A3o-com-Python-Algoritmos/dp/8575227181/?_encoding=UTF8&pd_rd_w=cLgOh&content-id=amzn1.sym.142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_p=142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_r=Q5SHBAZH69HSPBRR2MGS&pd_rd_wg=98FtW&pd_rd_r=ffa375c6-01c9-4e9c-9f87-2aef974a89af&ref_=pd_gw_ci_mcx_mr_hp_atf_m") 
 
     print(affiliate_url)
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `amazon-affiliate-scraper-0.1.2/amazon_affiliate/client.py` & `amazon-affiliate-scraper-0.2.0/amazon_affiliate/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,62 @@
+from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
-from pydantic import validate_arguments
+from pydantic import validate_call
 from selenium import webdriver
 from typing import Optional
+import time
 import json
 
 DEFAULT_ORIGIN_URL = "https://amazon.com.br/"
 
-class Client:
+driver_manager = ChromeDriverManager()
+
+class AmazonAffiliate:
+    @validate_call
     def __init__(
         self,
         cookies_file_path: str,
         origin_url: str = DEFAULT_ORIGIN_URL,
-        webdriver_file_path: Optional[str] = None,
+        webdriver_file_path: Optional[str] = driver_manager.install(),
         headless = True
     ) -> None:
         with open(cookies_file_path, "r+") as file:
             cookies = json.load(file)
 
         options = webdriver.ChromeOptions()
 
         if headless:
             options.add_argument("--headless")
 
-        service = Service(webdriver_file_path)
+        service = Service(executable_path = webdriver_file_path)
+
         self._driver = webdriver.Chrome(
             options = options,
             service = service
         )
 
         self._driver.get(origin_url)
 
         self._driver.get_log
 
         for cookie in cookies:
             self._driver.add_cookie(cookie)
 
-    @validate_arguments
+    @validate_call
     def create_affiliate_url(self, original_url: str) -> str:
         self._driver.get(original_url)
 
+        self._driver.implicitly_wait(10)
+
         link_creator_element = self._driver.find_element(By.CSS_SELECTOR, "#amzn-ss-text-link a")
         link_creator_element.click()
 
+        time.sleep(3)
+
         created_link_element = self._driver.find_element(By.CSS_SELECTOR, "#amzn-ss-text-shortlink-textarea")
         created_link = created_link_element.get_attribute("value")
 
         return created_link
 
     def close(self) -> None:
-        self._driver.close()
-
-    def __del__(self) -> None:
-        self.close()
+        self._driver.close()
```

### Comparing `amazon-affiliate-scraper-0.1.2/amazon_affiliate_scraper.egg-info/PKG-INFO` & `amazon-affiliate-scraper-0.2.0/amazon_affiliate_scraper.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: amazon-affiliate-scraper
-Version: 0.1.2
+Version: 0.2.0
 Summary: A simple library to help a developer who is affiliated with Amazon to automate the process.
 Author: Marcuth
-Author-email: marcuth2006@gmail.com
+Author-email: example@gmail.com
 License: MIT License
 Keywords: amazon affiliate scraper
 Description-Content-Type: text/markdown
 
 # Amazon Affiliate - Scraper Tool
 
 ## Quickstart
 
 ### Creating Affiliate URL:
 
 ```py
-from amazon_affiliate import Client
+from amazon_affiliate import AmazonAffiliate
 
 def main():
-    client = Client(
+    amazon_affiliate = AmazonAffiliate(
         cookies_file_path = "path/to/amazon_cookies.json", # Path to Amazon site cookies
         origin_url = "https://www.amazon.com.br/", # Amazon root URL in your country
         webdriver_file_path = "path/to/webdriver.exe", # Path to browser webdriver
         headless = True # If the browser will appear
     )
 
-    # Create an affiliate URL like: https://amzn.to/3qAp1rI
-    affiliate_url = client.create_affiliate_url("https://www.amazon.com.br/Introdu%C3%A7%C3%A3o-Programa%C3%A7%C3%A3o-com-Python-Algoritmos/dp/8575227181/?_encoding=UTF8&pd_rd_w=cLgOh&content-id=amzn1.sym.142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_p=142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_r=Q5SHBAZH69HSPBRR2MGS&pd_rd_wg=98FtW&pd_rd_r=ffa375c6-01c9-4e9c-9f87-2aef974a89af&ref_=pd_gw_ci_mcx_mr_hp_atf_m") 
+    # Create an affiliate URL like: https://amzn.to/3qAp1rZ
+    affiliate_url = amazon_affiliate.create_affiliate_url("https://www.amazon.com.br/Introdu%C3%A7%C3%A3o-Programa%C3%A7%C3%A3o-com-Python-Algoritmos/dp/8575227181/?_encoding=UTF8&pd_rd_w=cLgOh&content-id=amzn1.sym.142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_p=142cf30d-cd8e-4f67-a147-740799e27bf0&pf_rd_r=Q5SHBAZH69HSPBRR2MGS&pd_rd_wg=98FtW&pd_rd_r=ffa375c6-01c9-4e9c-9f87-2aef974a89af&ref_=pd_gw_ci_mcx_mr_hp_atf_m") 
 
     print(affiliate_url)
 
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `amazon-affiliate-scraper-0.1.2/setup.py` & `amazon-affiliate-scraper-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme_content = file.read()
 
 setup(
-    name="amazon-affiliate-scraper",
-    version="0.1.2",
-    license="MIT License",
-    author="Marcuth",
-    long_description=readme_content,
-    long_description_content_type="text/markdown",
-    author_email="marcuth2006@gmail.com",
-    keywords="amazon affiliate scraper",
-    description="A simple library to help a developer who is affiliated with Amazon to automate the process.",
-    packages=["amazon_affiliate"] + [ "amazon_affiliate/" + x for x in find_packages("amazon_affiliate") ]
+    name = "amazon-affiliate-scraper",
+    version = "0.2.0",
+    license = "MIT License",
+    author = "Marcuth",
+    long_description = readme_content,
+    long_description_content_type = "text/markdown",
+    author_email = "example@gmail.com",
+    keywords = "amazon affiliate scraper",
+    description = "A simple library to help a developer who is affiliated with Amazon to automate the process.",
+    packages = ["amazon_affiliate"] + [ "amazon_affiliate/" + x for x in find_packages("amazon_affiliate") ]
 )
```


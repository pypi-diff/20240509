# Comparing `tmp/scrapy-zyte-smartproxy-2.3.3.tar.gz` & `tmp/scrapy_zyte_smartproxy-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-zyte-smartproxy-2.3.3.tar", last modified: Thu Feb 22 20:53:07 2024, max compression
+gzip compressed data, was "scrapy_zyte_smartproxy-2.3.4.tar", last modified: Thu May  9 08:26:37 2024, max compression
```

## Comparing `scrapy-zyte-smartproxy-2.3.3.tar` & `scrapy_zyte_smartproxy-2.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:53:07.539198 scrapy-zyte-smartproxy-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-02-22 20:52:59.000000 scrapy-zyte-smartproxy-2.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-02-22 20:53:07.539198 scrapy-zyte-smartproxy-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-22 20:52:59.000000 scrapy-zyte-smartproxy-2.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:53:07.539198 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-22 20:52:59.000000 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20809 2024-02-22 20:52:59.000000 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-22 20:52:59.000000 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:53:07.539198 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-02-22 20:53:07.000000 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-22 20:53:07.000000 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 20:53:07.000000 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-22 20:53:07.000000 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-22 20:53:07.000000 scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-22 20:53:07.539198 scrapy-zyte-smartproxy-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-02-22 20:52:59.000000 scrapy-zyte-smartproxy-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 20:53:07.539198 scrapy-zyte-smartproxy-2.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    60283 2024-02-22 20:52:59.000000 scrapy-zyte-smartproxy-2.3.3/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:26:37.111930 scrapy_zyte_smartproxy-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-09 08:26:19.000000 scrapy_zyte_smartproxy-2.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-09 08:26:37.111930 scrapy_zyte_smartproxy-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 08:26:19.000000 scrapy_zyte_smartproxy-2.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:26:37.111930 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-09 08:26:19.000000 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21610 2024-05-09 08:26:19.000000 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 08:26:19.000000 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:26:37.111930 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-09 08:26:37.000000 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-09 08:26:37.000000 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:26:37.000000 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 08:26:37.000000 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 08:26:37.000000 scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-09 08:26:37.111930 scrapy_zyte_smartproxy-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-09 08:26:19.000000 scrapy_zyte_smartproxy-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:26:37.111930 scrapy_zyte_smartproxy-2.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    62717 2024-05-09 08:26:19.000000 scrapy_zyte_smartproxy-2.3.4/tests/test_all.py
```

### Comparing `scrapy-zyte-smartproxy-2.3.3/LICENSE.txt` & `scrapy_zyte_smartproxy-2.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-smartproxy-2.3.3/PKG-INFO` & `scrapy_zyte_smartproxy-2.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-zyte-smartproxy
-Version: 2.3.3
+Version: 2.3.4
 Summary: Scrapy middleware for Zyte Smart Proxy Manager
 Home-page: https://github.com/scrapy-plugins/scrapy-zyte-smartproxy
 Author: Zyte
 Author-email: opensource@zyte.com
 Maintainer: Raul Gallegos
 Maintainer-email: raul.ogh@gmail.com
 License: BSD
@@ -46,16 +46,22 @@
    :target: http://travis-ci.org/scrapy-plugins/scrapy-zyte-smartproxy
    :alt: Build Status
 
 .. image:: http://codecov.io/github/scrapy-plugins/scrapy-zyte-smartproxy/coverage.svg?branch=master
    :target: http://codecov.io/github/scrapy-plugins/scrapy-zyte-smartproxy?branch=master
    :alt: Code Coverage
 
-scrapy-zyte-smartproxy provides easy use of `Zyte Smart Proxy Manager
-<https://www.zyte.com/smart-proxy-manager/>`_ (formerly Crawlera) with Scrapy.
+scrapy-zyte-smartproxy is a `Scrapy downloader middleware`_ to use one of
+Zyte’s proxy services: either the `proxy mode`_ of `Zyte API`_ or `Zyte Smart
+Proxy Manager`_ (formerly Crawlera).
+
+.. _Scrapy downloader middleware: https://doc.scrapy.org/en/latest/topics/downloader-middleware.html
+.. _proxy mode: https://docs.zyte.com/zyte-api/usage/proxy-mode.html
+.. _Zyte API: https://docs.zyte.com/zyte-api/get-started.html
+.. _Zyte Smart Proxy Manager: https://www.zyte.com/smart-proxy-manager/
 
 Requirements
 ============
 
 * Python 2.7 or Python 3.4+
 * Scrapy 1.4+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy/middleware.py` & `scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy/middleware.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         return o
 
     def _make_auth_url(self, spider):
         parsed_url = urlparse(self.url)
         auth = self.get_proxyauth(spider)
         if not auth.startswith(b'Basic '):
             raise ValueError(
-                'Zyte Smart Proxy Manager only supports HTTP basic access '
+                'Zyte proxy services only support HTTP basic access '
                 'authentication, but %s.%s.get_proxyauth() returned %r'
                 % (self.__module__, self.__class__.__name__, auth)
             )
         user_and_colon = urlsafe_b64decode(auth[6:].strip()).decode('utf-8')
         netloc = user_and_colon + '@' + parsed_url.netloc.split('@')[-1]
         parsed_url = parsed_url._replace(netloc=netloc)
         return urlunparse(parsed_url)
@@ -107,36 +107,36 @@
         self.exp_backoff = exp_backoff(self.backoff_step, self.backoff_max)
 
         if not self.enabled and not self.force_enable_on_http_codes:
             return
 
         if not self.apikey:
             logger.warning(
-                "Zyte Smart Proxy Manager cannot be used without an API key",
+                "Zyte proxy services cannot be used without an API key",
                 extra={'spider': spider},
             )
             return
 
         self._auth_url = self._make_auth_url(spider)
         self._authless_url = _remove_auth(self._auth_url)
 
         logger.info(
-            "Using Zyte Smart Proxy Manager at %s (apikey: %s)" % (
+            "Using Zyte proxy service %s with an API key ending in %s" % (
                 self.url, self.apikey[:7]
             ),
             extra={'spider': spider},
         )
 
         if not self.preserve_delay:
             # Setting spider download delay to 0 to get maximum crawl rate
             spider.download_delay = 0
             logger.info(
                 "ZyteSmartProxyMiddleware: disabling download delays in "
-                "Scrapy to optimize delays introduced by Zyte Smart Proxy "
-                "Manager. To avoid this behaviour you can use the "
+                "Scrapy to optimize delays introduced by Zyte proxy services. "
+                "To avoid this behaviour you can use the "
                 "ZYTE_SMARTPROXY_PRESERVE_DELAY setting, but keep in mind "
                 "that this may slow down the crawl significantly",
                 extra={'spider': spider},
             )
 
     def _settings_get(self, type_, *a, **kw):
         if type_ is int:
@@ -192,15 +192,17 @@
         )
 
     def get_proxyauth(self, spider):
         """Hook to compute Proxy-Authorization header by custom rules."""
         return basic_auth_header(self.apikey, '')
 
     def _targets_zyte_api(self, request):
-        auth_url = request.meta["proxy"]
+        if self._auth_url is None:
+            return False
+        auth_url = request.meta.get("proxy", self._auth_url)
         targets_zyte_api = self._targets.get(auth_url, None)
         if targets_zyte_api is None:
             targets_zyte_api = urlparse(auth_url).hostname == "api.zyte.com"
             self._targets[auth_url] = targets_zyte_api
         return targets_zyte_api
 
     def _translate_headers(self, request, targets_zyte_api):
@@ -216,14 +218,18 @@
                 "Translating (and dropping) header %r (%r) as %r on request %r",
                 header,
                 value,
                 translation,
                 request,
             )
 
+    def _inc_stat(self, stat, targets_zyte_api, value=1):
+        prefix = "zyte_api_proxy" if targets_zyte_api else "zyte_smartproxy"
+        self.crawler.stats.inc_value("{}/{}".format(prefix, stat), value)
+
     def process_request(self, request, spider):
         if self._is_enabled_for_request(request):
             if 'proxy' not in request.meta:
                 request.meta['proxy'] = self._auth_url
             elif (
                 request.meta['proxy'] == self._authless_url
                 and b"Proxy-Authorization" not in request.headers
@@ -242,16 +248,16 @@
             request.meta['download_timeout'] = self.download_timeout
             if self.job_id:
                 job_header = 'Zyte-JobId' if targets_zyte_api else 'X-Crawlera-JobId'
                 request.headers[job_header] = self.job_id
             user_agent_header = "Zyte-Client" if targets_zyte_api else "X-Crawlera-Client"
             from scrapy_zyte_smartproxy import __version__
             request.headers[user_agent_header] = 'scrapy-zyte-smartproxy/%s' % __version__
-            self.crawler.stats.inc_value('zyte_smartproxy/request')
-            self.crawler.stats.inc_value('zyte_smartproxy/request/method/%s' % request.method)
+            self._inc_stat("request", targets_zyte_api=targets_zyte_api)
+            self._inc_stat("request/method/{}".format(request.method), targets_zyte_api=targets_zyte_api)
             self._translate_headers(request, targets_zyte_api=targets_zyte_api)
             self._clean_zyte_smartproxy_headers(request, targets_zyte_api=targets_zyte_api)
         else:
             self._clean_zyte_smartproxy_headers(request)
 
     def _is_banned(self, response):
         return (
@@ -281,97 +287,102 @@
             response.headers["Zyte-Error"] = value
             return value
         return None
 
     def process_response(self, request, response, spider):
         zyte_smartproxy_error = self._process_error(response)
 
+        targets_zyte_api = self._targets_zyte_api(request)
+
         if not self._is_enabled_for_request(request):
-            return self._handle_not_enabled_response(request, response)
+            return self._handle_not_enabled_response(request, response, targets_zyte_api=targets_zyte_api)
 
         if not self._is_zyte_smartproxy_or_zapi_response(response):
             return response
 
         key = self._get_slot_key(request)
         self._restore_original_delay(request)
 
         if self._is_no_available_proxies(response) or self._is_auth_error(response):
             if self._is_no_available_proxies(response):
                 reason = 'noslaves'
             else:
                 reason = 'autherror'
-            self._set_custom_delay(request, next(self.exp_backoff), reason=reason)
+            self._set_custom_delay(request, next(self.exp_backoff), reason=reason, targets_zyte_api=targets_zyte_api)
         else:
-            self.crawler.stats.inc_value('zyte_smartproxy/delay/reset_backoff')
+            self._inc_stat("delay/reset_backoff", targets_zyte_api=targets_zyte_api)
             self.exp_backoff = exp_backoff(self.backoff_step, self.backoff_max)
 
         if self._is_auth_error(response):
             # When Zyte Smart Proxy Manager has issues it might not be able to
             # authenticate users we must retry
             retries = request.meta.get('zyte_smartproxy_auth_retry_times', 0)
             if retries < self.max_auth_retry_times:
-                return self._retry_auth(response, request, spider)
+                return self._retry_auth(response, request, spider, targets_zyte_api=targets_zyte_api)
             else:
-                self.crawler.stats.inc_value('zyte_smartproxy/retries/auth/max_reached')
+                self._inc_stat("retries/auth/max_reached", targets_zyte_api=targets_zyte_api)
                 logger.warning(
                     "Max retries for authentication issues reached, please check auth"
                     " information settings",
                     extra={'spider': self.spider},
                 )
 
         if self._is_banned(response):
             self._bans[key] += 1
             if self._bans[key] > self.maxbans:
                 self.crawler.engine.close_spider(spider, 'banned')
             else:
                 after = response.headers.get('retry-after')
                 if after:
-                    self._set_custom_delay(request, float(after), reason='banned')
-            self.crawler.stats.inc_value('zyte_smartproxy/response/banned')
+                    self._set_custom_delay(request, float(after), reason='banned', targets_zyte_api=targets_zyte_api)
+            self._inc_stat("response/banned", targets_zyte_api=targets_zyte_api)
         else:
             self._bans[key] = 0
         # If placed behind `RedirectMiddleware`, it would not count 3xx responses
-        self.crawler.stats.inc_value('zyte_smartproxy/response')
-        self.crawler.stats.inc_value('zyte_smartproxy/response/status/%s' % response.status)
+        self._inc_stat("response", targets_zyte_api=targets_zyte_api)
+        self._inc_stat("response/status/{}".format(response.status), targets_zyte_api=targets_zyte_api)
         if zyte_smartproxy_error:
-            self.crawler.stats.inc_value('zyte_smartproxy/response/error')
-            self.crawler.stats.inc_value(
-                'zyte_smartproxy/response/error/%s' % zyte_smartproxy_error.decode('utf8'))
+            self._inc_stat("response/error", targets_zyte_api=targets_zyte_api)
+            error_msg = zyte_smartproxy_error.decode('utf8')
+            self._inc_stat("response/error/{}".format(error_msg), targets_zyte_api=targets_zyte_api)
         return response
 
     def process_exception(self, request, exception, spider):
         if not self._is_enabled_for_request(request):
             return
         if isinstance(exception, (ConnectionRefusedError, ConnectionDone)):
             # Handle Zyte Smart Proxy Manager downtime
             self._clear_dns_cache()
-            self._set_custom_delay(request, self.connection_refused_delay, reason='conn_refused')
+            targets_zyte_api = self._targets_zyte_api(request)
+            self._set_custom_delay(request, self.connection_refused_delay, reason='conn_refused', targets_zyte_api=targets_zyte_api)
 
-    def _handle_not_enabled_response(self, request, response):
+    def _handle_not_enabled_response(self, request, response, targets_zyte_api):
         if self._should_enable_for_response(response):
             domain = self._get_url_domain(request.url)
             self.enabled_for_domain[domain] = True
 
             retryreq = request.copy()
             retryreq.dont_filter = True
-            self.crawler.stats.inc_value('zyte_smartproxy/retries/should_have_been_enabled')
+            self._inc_stat("retries/should_have_been_enabled", targets_zyte_api=targets_zyte_api)
             return retryreq
         return response
 
-    def _retry_auth(self, response, request, spider):
+    def _retry_auth(self, response, request, spider, targets_zyte_api):
         logger.warning(
-            "Retrying a Zyte Smart Proxy Manager request due to an "
-            "authentication issue",
+            (
+                "Retrying a request due to an authentication issue with "
+                "the configured Zyte proxy service"
+            ),
             extra={'spider': self.spider},
         )
         retries = request.meta.get('zyte_smartproxy_auth_retry_times', 0) + 1
         retryreq = request.copy()
         retryreq.meta['zyte_smartproxy_auth_retry_times'] = retries
         retryreq.dont_filter = True
-        self.crawler.stats.inc_value('zyte_smartproxy/retries/auth')
+        self._inc_stat("retries/auth", targets_zyte_api=targets_zyte_api)
         return retryreq
 
     def _clear_dns_cache(self):
         # Scrapy doesn't expire dns records by default, so we force it here,
         # so client can reconnect trough DNS failover.
         dnscache.pop(urlparse(self.url).hostname, None)
 
@@ -398,25 +409,25 @@
     def _get_slot_key(self, request):
         return request.meta.get('download_slot')
 
     def _get_slot(self, request):
         key = self._get_slot_key(request)
         return key, self.crawler.engine.downloader.slots.get(key)
 
-    def _set_custom_delay(self, request, delay, reason=None):
+    def _set_custom_delay(self, request, delay, targets_zyte_api, reason=None):
         """Set custom delay for slot and save original one."""
         key, slot = self._get_slot(request)
         if not slot:
             return
         if self._saved_delays[key] is None:
             self._saved_delays[key] = slot.delay
         slot.delay = delay
         if reason is not None:
-            self.crawler.stats.inc_value('zyte_smartproxy/delay/%s' % reason)
-            self.crawler.stats.inc_value('zyte_smartproxy/delay/%s/total' % reason, delay)
+            self._inc_stat("delay/{}".format(reason), targets_zyte_api=targets_zyte_api)
+            self._inc_stat("delay/{}/total".format(reason), value=delay, targets_zyte_api=targets_zyte_api)
 
     def _restore_original_delay(self, request):
         """Restore original delay for slot if it was changed."""
         key, slot = self._get_slot(request)
         if not slot:
             return
         if self._saved_delays[key] is not None:
```

### Comparing `scrapy-zyte-smartproxy-2.3.3/scrapy_zyte_smartproxy.egg-info/PKG-INFO` & `scrapy_zyte_smartproxy-2.3.4/scrapy_zyte_smartproxy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-zyte-smartproxy
-Version: 2.3.3
+Version: 2.3.4
 Summary: Scrapy middleware for Zyte Smart Proxy Manager
 Home-page: https://github.com/scrapy-plugins/scrapy-zyte-smartproxy
 Author: Zyte
 Author-email: opensource@zyte.com
 Maintainer: Raul Gallegos
 Maintainer-email: raul.ogh@gmail.com
 License: BSD
@@ -46,16 +46,22 @@
    :target: http://travis-ci.org/scrapy-plugins/scrapy-zyte-smartproxy
    :alt: Build Status
 
 .. image:: http://codecov.io/github/scrapy-plugins/scrapy-zyte-smartproxy/coverage.svg?branch=master
    :target: http://codecov.io/github/scrapy-plugins/scrapy-zyte-smartproxy?branch=master
    :alt: Code Coverage
 
-scrapy-zyte-smartproxy provides easy use of `Zyte Smart Proxy Manager
-<https://www.zyte.com/smart-proxy-manager/>`_ (formerly Crawlera) with Scrapy.
+scrapy-zyte-smartproxy is a `Scrapy downloader middleware`_ to use one of
+Zyte’s proxy services: either the `proxy mode`_ of `Zyte API`_ or `Zyte Smart
+Proxy Manager`_ (formerly Crawlera).
+
+.. _Scrapy downloader middleware: https://doc.scrapy.org/en/latest/topics/downloader-middleware.html
+.. _proxy mode: https://docs.zyte.com/zyte-api/usage/proxy-mode.html
+.. _Zyte API: https://docs.zyte.com/zyte-api/get-started.html
+.. _Zyte Smart Proxy Manager: https://www.zyte.com/smart-proxy-manager/
 
 Requirements
 ============
 
 * Python 2.7 or Python 3.4+
 * Scrapy 1.4+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scrapy-zyte-smartproxy-2.3.3/setup.py` & `scrapy_zyte_smartproxy-2.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
-with open("README.rst") as f:
-    readme = f.read()
+with open("README.rst", "rb") as f:
+    readme = f.read().decode("utf-8")
 
 
 setup(
     name='scrapy-zyte-smartproxy',
-    version='2.3.3',
+    version='2.3.4',
     license='BSD',
     description='Scrapy middleware for Zyte Smart Proxy Manager',
     long_description=readme,
     maintainer='Raul Gallegos',
     maintainer_email='raul.ogh@gmail.com',
     author='Zyte',
     author_email='opensource@zyte.com',
```

### Comparing `scrapy-zyte-smartproxy-2.3.3/tests/test_all.py` & `scrapy_zyte_smartproxy-2.3.4/tests/test_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import binascii
 import os
 import pytest
+from copy import copy
 from random import choice
 from unittest import TestCase
 try:
     from unittest.mock import call, patch
 except ImportError:
     from mock import call, patch
 
@@ -401,62 +402,115 @@
                 "proxy": "http://apikey:@api.zyte.com:8011",
             },
         )
         self.assertEqual(mw3.process_request(req3, self.spider), None)
         self.assertEqual(req3.headers.get('X-Crawlera-Jobid'), None)
         self.assertEqual(req3.headers.get('Zyte-JobId'), b'2816')
 
-    def test_stats(self):
+    def _test_stats(self, settings, prefix):
         self.spider.zyte_smartproxy_enabled = True
         spider = self.spider
-        crawler = self._mock_crawler(spider, self.settings)
+        settings = copy(settings)
+        settings["ZYTE_SMARTPROXY_FORCE_ENABLE_ON_HTTP_CODES"] = [555]
+        crawler = self._mock_crawler(spider, settings)
         mw = self.mwcls.from_crawler(crawler)
         mw.open_spider(spider)
         httpproxy = HttpProxyMiddleware.from_crawler(crawler)
 
         req = Request('http://example.com')
         assert mw.process_request(req, spider) is None
         assert httpproxy.process_request(req, spider) is None
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/request'), 1)
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/request/method/GET'), 1)
+        self.assertEqual(crawler.stats.get_value('{}/request'.format(prefix)), 1)
+        self.assertEqual(crawler.stats.get_value('{}/request/method/GET'.format(prefix)), 1)
 
         res = self._mock_zyte_smartproxy_response(req.url)
         assert mw.process_response(req, res, spider) is res
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/response'), 1)
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/response/status/200'), 1)
+        self.assertEqual(crawler.stats.get_value('{}/response'.format(prefix)), 1)
+        self.assertEqual(crawler.stats.get_value('{}/response/status/200'.format(prefix)), 1)
 
         req = Request('http://example.com/other', method='POST')
         assert mw.process_request(req, spider) is None
         assert httpproxy.process_request(req, spider) is None
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/request'), 2)
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/request/method/POST'), 1)
+        self.assertEqual(crawler.stats.get_value('{}/request'.format(prefix)), 2)
+        self.assertEqual(crawler.stats.get_value('{}/request/method/POST'.format(prefix)), 1)
 
         res = self._mock_zyte_smartproxy_response(
             req.url,
             status=mw.ban_code,
             headers={'Zyte-Error': 'somethingbad'}
         )
         assert mw.process_response(req, res, spider) is res
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/response'), 2)
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/response/status/{}'.format(mw.ban_code)), 1)
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/response/error/somethingbad'), 1)
+        self.assertEqual(crawler.stats.get_value('{}/response'.format(prefix)), 2)
+        self.assertEqual(crawler.stats.get_value('{}/response/status/{}'.format(prefix, mw.ban_code)), 1)
+        self.assertEqual(crawler.stats.get_value('{}/response/error'.format(prefix)), 1)
+        self.assertEqual(crawler.stats.get_value('{}/response/error/somethingbad'.format(prefix)), 1)
         self.assertEqual(res.headers["X-Crawlera-Error"], b"somethingbad")
         self.assertEqual(res.headers["Zyte-Error"], b"somethingbad")
+
         res = self._mock_zyte_smartproxy_response(
             req.url,
             status=mw.ban_code,
-            headers={'X-Crawlera-Error': 'banned'}
+            headers={'X-Crawlera-Error': 'banned', "Retry-After": "1"}
         )
         assert mw.process_response(req, res, spider) is res
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/response'), 3)
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/response/status/{}'.format(mw.ban_code)), 2)
-        self.assertEqual(crawler.stats.get_value('zyte_smartproxy/response/banned'), 1)
+        self.assertEqual(crawler.stats.get_value('{}/response'.format(prefix)), 3)
+        self.assertEqual(crawler.stats.get_value('{}/response/status/{}'.format(prefix, mw.ban_code)), 2)
+        self.assertEqual(crawler.stats.get_value('{}/response/banned'.format(prefix)), 1)
         self.assertEqual(res.headers["X-Crawlera-Error"], b"banned")
         self.assertEqual(res.headers["Zyte-Error"], b"banned")
 
+        res = self._mock_zyte_smartproxy_response(
+            req.url,
+            status=mw.ban_code,
+            headers={'X-Crawlera-Error': 'banned', "Retry-After": "1"}
+        )
+        slot_key = "example.com"
+        crawler.engine.downloader.slots[slot_key] = MockedSlot()
+        req.meta["download_slot"] = "example.com"
+        assert mw.process_response(req, res, spider) is res
+        del req.meta["download_slot"]
+        self.assertEqual(crawler.stats.get_value('{}/delay/banned'.format(prefix)), 1)
+        self.assertEqual(crawler.stats.get_value('{}/delay/banned/total'.format(prefix)), 1)
+
+        res = self._mock_zyte_smartproxy_response(
+            req.url,
+            status=407,
+            headers={'X-Crawlera-Error': 'bad_proxy_auth'},
+        )
+        assert isinstance(mw.process_response(req, res, spider), Request)
+        self.assertEqual(crawler.stats.get_value('{}/retries/auth'.format(prefix)), 1)
+
+        res = self._mock_zyte_smartproxy_response(
+            req.url,
+            status=407,
+            headers={'X-Crawlera-Error': 'bad_proxy_auth'},
+        )
+        req.meta["zyte_smartproxy_auth_retry_times"] = 11
+        assert mw.process_response(req, res, spider) is res
+        del req.meta["zyte_smartproxy_auth_retry_times"]
+        self.assertEqual(crawler.stats.get_value('{}/retries/auth'.format(prefix)), 1)
+        self.assertEqual(crawler.stats.get_value('{}/retries/auth/max_reached'.format(prefix)), 1)
+
+        res = self._mock_zyte_smartproxy_response(
+            req.url,
+            status=555,
+        )
+        req.meta["dont_proxy"] = True
+        assert isinstance(mw.process_response(req, res, spider), Request)
+        del req.meta["dont_proxy"]
+        self.assertEqual(crawler.stats.get_value('{}/retries/should_have_been_enabled'.format(prefix)), 1)
+
+    def test_stats_spm(self):
+        self._test_stats(self.settings, "zyte_smartproxy")
+
+    def test_stats_zapi(self):
+        settings = copy(self.settings)
+        settings["ZYTE_SMARTPROXY_URL"] = "http://api.zyte.com:8011"
+        self._test_stats(settings, "zyte_api_proxy")
+
     def _make_fake_request(self, spider, zyte_smartproxy_enabled, **kwargs):
         spider.zyte_smartproxy_enabled = zyte_smartproxy_enabled
         crawler = self._mock_crawler(spider, self.settings)
         mw = self.mwcls.from_crawler(crawler)
         mw.open_spider(spider)
         httpproxy = HttpProxyMiddleware.from_crawler(crawler)
         headers = {
@@ -779,23 +833,23 @@
         spider = self.spider
         self.spider.zyte_smartproxy_enabled = True
         crawler = self._mock_crawler(spider, self.settings)
         mw = self.mwcls.from_crawler(crawler)
         mw.open_spider(spider)
         expected_calls = [
             call(
-                "Using Zyte Smart Proxy Manager at %s (apikey: %s)" % (
+                "Using Zyte proxy service %s with an API key ending in %s" % (
                     self.mwcls.url, 'apikey'
                 ),
                 extra={'spider': spider},
             ),
             call(
                 "ZyteSmartProxyMiddleware: disabling download delays in "
-                "Scrapy to optimize delays introduced by Zyte Smart Proxy "
-                "Manager. To avoid this behaviour you can use the "
+                "Scrapy to optimize delays introduced by Zyte proxy services. "
+                "To avoid this behaviour you can use the "
                 "ZYTE_SMARTPROXY_PRESERVE_DELAY setting, but keep in mind "
                 "that this may slow down the crawl significantly",
                 extra={'spider': spider},
             ),
         ]
         assert mock_logger.info.call_args_list == expected_calls
 
@@ -885,28 +939,28 @@
         self.spider.zyte_smartproxy_enabled = True
         settings = {}
         crawler = self._mock_crawler(self.spider, settings)
         mw = self.mwcls.from_crawler(crawler)
         mw.open_spider(self.spider)
         self.assertTrue(mw.enabled)
         mock_logger.warning.assert_called_with(
-            "Zyte Smart Proxy Manager cannot be used without an API key",
+            "Zyte proxy services cannot be used without an API key",
             extra={'spider': self.spider}
         )
 
     @patch('scrapy_zyte_smartproxy.middleware.logger')
     def test_no_apikey_warning_force_enable(self, mock_logger):
         self.spider.zyte_smartproxy_enabled = False
         settings = {'ZYTE_SMARTPROXY_FORCE_ENABLE_ON_HTTP_CODES': [403]}
         crawler = self._mock_crawler(self.spider, settings)
         mw = self.mwcls.from_crawler(crawler)
         mw.open_spider(self.spider)
         self.assertFalse(mw.enabled)
         mock_logger.warning.assert_called_with(
-            "Zyte Smart Proxy Manager cannot be used without an API key",
+            "Zyte proxy services cannot be used without an API key",
             extra={'spider': self.spider}
         )
 
     @patch('scrapy_zyte_smartproxy.middleware.logger')
     def test_apikey_warning_force_enable(self, mock_logger):
         self.spider.zyte_smartproxy_enabled = False
         settings = {
@@ -967,14 +1021,15 @@
         crawler = self._mock_crawler(self.spider, self.settings)
         mw = self.mwcls.from_crawler(crawler)
         mw.open_spider(self.spider)
 
         # there are no slot named 'example.com'
         noslaves_req = Request(url,
                                meta={'download_slot': 'example.com'})
+        assert mw.process_request(noslaves_req, self.spider) is None
 
         headers = {'X-Crawlera-Error': 'noslaves'}
         noslaves_res = self._mock_zyte_smartproxy_response(
             ban_url,
             status=self.bancode,
             headers=headers,
         )
```


# Comparing `tmp/fastramqpi-7.3.1.tar.gz` & `tmp/fastramqpi-7.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-7.3.1.tar", max compression
+gzip compressed data, was "fastramqpi-7.3.2.tar", max compression
```

## Comparing `fastramqpi-7.3.1.tar` & `fastramqpi-7.3.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0        0        0        0 2024-05-08 11:31:01.926891 fastramqpi-7.3.1/LICENSES/
--rw-r--r--   0        0        0    15177 2024-05-08 11:31:01.926891 fastramqpi-7.3.1/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0    14146 2024-05-08 11:31:01.926891 fastramqpi-7.3.1/README.md
--rw-r--r--   0        0        0       85 2024-05-08 11:31:01.935892 fastramqpi-7.3.1/fastramqpi/__init__.py
--rw-r--r--   0        0        0     7425 2024-05-08 11:31:01.935892 fastramqpi-7.3.1/fastramqpi/app.py
--rw-r--r--   0        0        0     2207 2024-05-08 11:31:01.935892 fastramqpi-7.3.1/fastramqpi/config.py
--rw-r--r--   0        0        0     1620 2024-05-08 11:31:01.935892 fastramqpi-7.3.1/fastramqpi/context.py
--rw-r--r--   0        0        0     1498 2024-05-08 11:31:01.936892 fastramqpi-7.3.1/fastramqpi/depends.py
--rw-r--r--   0        0        0     6738 2024-05-08 11:31:01.936892 fastramqpi-7.3.1/fastramqpi/main.py
--rw-r--r--   0        0        0      477 2024-05-08 11:31:01.936892 fastramqpi-7.3.1/fastramqpi/metrics.py
--rw-r--r--   0        0        0        0 2024-05-08 11:31:02.015900 fastramqpi-7.3.1/fastramqpi/py.typed
--rw-r--r--   0        0        0     5174 2024-05-08 11:31:01.936892 fastramqpi-7.3.1/fastramqpi/pytest_plugin.py
--rw-r--r--   0        0        0      884 2024-05-08 11:31:01.936892 fastramqpi-7.3.1/fastramqpi/pytest_util.py
--rw-r--r--   0        0        0       99 2024-05-08 11:31:01.936892 fastramqpi-7.3.1/fastramqpi/ra_utils/__init__.py
--rw-r--r--   0        0        0     2263 2024-05-08 11:31:01.936892 fastramqpi-7.3.1/fastramqpi/ra_utils/apply.py
--rw-r--r--   0        0        0     1051 2024-05-08 11:31:01.937892 fastramqpi-7.3.1/fastramqpi/ra_utils/async_to_sync.py
--rw-r--r--   0        0        0     2496 2024-05-08 11:31:01.937892 fastramqpi-7.3.1/fastramqpi/ra_utils/asyncio_utils.py
--rw-r--r--   0        0        0      805 2024-05-08 11:31:01.937892 fastramqpi-7.3.1/fastramqpi/ra_utils/attrdict.py
--rw-r--r--   0        0        0     1539 2024-05-08 11:31:01.937892 fastramqpi-7.3.1/fastramqpi/ra_utils/catchtime.py
--rw-r--r--   0        0        0      979 2024-05-08 11:31:01.937892 fastramqpi-7.3.1/fastramqpi/ra_utils/deprecation.py
--rw-r--r--   0        0        0     3961 2024-05-08 11:31:01.937892 fastramqpi-7.3.1/fastramqpi/ra_utils/dict_map.py
--rw-r--r--   0        0        0     2184 2024-05-08 11:31:01.937892 fastramqpi-7.3.1/fastramqpi/ra_utils/ensure_hashable.py
--rw-r--r--   0        0        0     3808 2024-05-08 11:31:01.937892 fastramqpi-7.3.1/fastramqpi/ra_utils/ensure_single_run.py
--rw-r--r--   0        0        0     1723 2024-05-08 11:31:01.938892 fastramqpi-7.3.1/fastramqpi/ra_utils/generate_uuid.py
--rw-r--r--   0        0        0     5633 2024-05-08 11:31:01.938892 fastramqpi-7.3.1/fastramqpi/ra_utils/headers.py
--rw-r--r--   0        0        0     3245 2024-05-08 11:31:01.938892 fastramqpi-7.3.1/fastramqpi/ra_utils/jinja_filter.py
--rw-r--r--   0        0        0     7347 2024-05-08 11:31:01.938892 fastramqpi-7.3.1/fastramqpi/ra_utils/job_settings.py
--rw-r--r--   0        0        0     6027 2024-05-08 11:31:01.938892 fastramqpi-7.3.1/fastramqpi/ra_utils/lazy_dict.py
--rw-r--r--   0        0        0     2929 2024-05-08 11:31:01.938892 fastramqpi-7.3.1/fastramqpi/ra_utils/load_settings.py
--rw-r--r--   0        0        0     2935 2024-05-08 11:31:01.938892 fastramqpi-7.3.1/fastramqpi/ra_utils/multiple_replace.py
--rw-r--r--   0        0        0     2891 2024-05-08 11:31:01.939893 fastramqpi-7.3.1/fastramqpi/ra_utils/semantic_version_type.py
--rw-r--r--   0        0        0     1280 2024-05-08 11:31:01.939893 fastramqpi-7.3.1/fastramqpi/ra_utils/sentry_init.py
--rw-r--r--   0        0        0     1003 2024-05-08 11:31:01.939893 fastramqpi-7.3.1/fastramqpi/ra_utils/strategies.py
--rw-r--r--   0        0        0     3782 2024-05-08 11:31:01.939893 fastramqpi-7.3.1/fastramqpi/ra_utils/structured_url.py
--rw-r--r--   0        0        0     4717 2024-05-08 11:31:01.939893 fastramqpi-7.3.1/fastramqpi/ra_utils/syncable.py
--rw-r--r--   0        0        0      548 2024-05-08 11:31:01.939893 fastramqpi-7.3.1/fastramqpi/ra_utils/tqdm_wrapper.py
--rw-r--r--   0        0        0     1834 2024-05-08 11:31:01.939893 fastramqpi-7.3.1/fastramqpi/ra_utils/transpose_dict.py
--rw-r--r--   0        0        0      300 2024-05-08 11:31:01.939893 fastramqpi-7.3.1/fastramqpi/raclients/__init__.py
--rw-r--r--   0        0        0     6858 2024-05-08 11:31:01.940893 fastramqpi-7.3.1/fastramqpi/raclients/auth.py
--rw-r--r--   0        0        0       99 2024-05-08 11:31:01.940893 fastramqpi-7.3.1/fastramqpi/raclients/graph/__init__.py
--rw-r--r--   0        0        0     7219 2024-05-08 11:31:01.940893 fastramqpi-7.3.1/fastramqpi/raclients/graph/client.py
--rw-r--r--   0        0        0     9303 2024-05-08 11:31:01.940893 fastramqpi-7.3.1/fastramqpi/raclients/graph/transport.py
--rw-r--r--   0        0        0     3482 2024-05-08 11:31:01.940893 fastramqpi-7.3.1/fastramqpi/raclients/graph/util.py
--rw-r--r--   0        0        0       99 2024-05-08 11:31:01.940893 fastramqpi-7.3.1/fastramqpi/raclients/modelclient/__init__.py
--rw-r--r--   0        0        0     4390 2024-05-08 11:31:01.941893 fastramqpi-7.3.1/fastramqpi/raclients/modelclient/base.py
--rw-r--r--   0        0        0     1919 2024-05-08 11:31:01.941893 fastramqpi-7.3.1/fastramqpi/raclients/modelclient/lora.py
--rw-r--r--   0        0        0     5296 2024-05-08 11:31:01.941893 fastramqpi-7.3.1/fastramqpi/raclients/modelclient/mo.py
--rw-r--r--   0        0        0     3459 2024-05-08 11:31:01.941893 fastramqpi-7.3.1/fastramqpi/raclients/upload.py
--rw-r--r--   0        0        0      321 2024-05-08 11:31:01.941893 fastramqpi-7.3.1/fastramqpi/ramqp/__init__.py
--rw-r--r--   0        0        0    18731 2024-05-08 11:31:01.941893 fastramqpi-7.3.1/fastramqpi/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2024-05-08 11:31:01.942893 fastramqpi-7.3.1/fastramqpi/ramqp/amqp.py
--rw-r--r--   0        0        0     2858 2024-05-08 11:31:01.942893 fastramqpi-7.3.1/fastramqpi/ramqp/config.py
--rw-r--r--   0        0        0    11475 2024-05-08 11:31:01.942893 fastramqpi-7.3.1/fastramqpi/ramqp/depends.py
--rw-r--r--   0        0        0     7130 2024-05-08 11:31:01.942893 fastramqpi-7.3.1/fastramqpi/ramqp/metrics.py
--rw-r--r--   0        0        0     8642 2024-05-08 11:31:01.942893 fastramqpi-7.3.1/fastramqpi/ramqp/mo.py
--rw-r--r--   0        0        0     1941 2024-05-08 11:31:01.942893 fastramqpi-7.3.1/fastramqpi/ramqp/utils.py
--rw-r--r--   0        0        0     2173 2024-05-08 11:31:04.129120 fastramqpi-7.3.1/pyproject.toml
--rw-r--r--   0        0        0    15537 1970-01-01 00:00:00.000000 fastramqpi-7.3.1/PKG-INFO
+drwxr-xr-x   0        0        0        0 2024-05-09 06:51:25.166828 fastramqpi-7.3.2/LICENSES/
+-rw-r--r--   0        0        0    15177 2024-05-09 06:51:25.166828 fastramqpi-7.3.2/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0    14146 2024-05-09 06:51:25.166828 fastramqpi-7.3.2/README.md
+-rw-r--r--   0        0        0       85 2024-05-09 06:51:25.178829 fastramqpi-7.3.2/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     7425 2024-05-09 06:51:25.178829 fastramqpi-7.3.2/fastramqpi/app.py
+-rw-r--r--   0        0        0     2207 2024-05-09 06:51:25.178829 fastramqpi-7.3.2/fastramqpi/config.py
+-rw-r--r--   0        0        0     1620 2024-05-09 06:51:25.178829 fastramqpi-7.3.2/fastramqpi/context.py
+-rw-r--r--   0        0        0     1498 2024-05-09 06:51:25.178829 fastramqpi-7.3.2/fastramqpi/depends.py
+-rw-r--r--   0        0        0     6738 2024-05-09 06:51:25.178829 fastramqpi-7.3.2/fastramqpi/main.py
+-rw-r--r--   0        0        0      477 2024-05-09 06:51:25.183829 fastramqpi-7.3.2/fastramqpi/metrics.py
+-rw-r--r--   0        0        0        0 2024-05-09 06:51:25.319843 fastramqpi-7.3.2/fastramqpi/py.typed
+-rw-r--r--   0        0        0     5174 2024-05-09 06:51:25.183829 fastramqpi-7.3.2/fastramqpi/pytest_plugin.py
+-rw-r--r--   0        0        0      884 2024-05-09 06:51:25.183829 fastramqpi-7.3.2/fastramqpi/pytest_util.py
+-rw-r--r--   0        0        0       99 2024-05-09 06:51:25.183829 fastramqpi-7.3.2/fastramqpi/ra_utils/__init__.py
+-rw-r--r--   0        0        0     2263 2024-05-09 06:51:25.183829 fastramqpi-7.3.2/fastramqpi/ra_utils/apply.py
+-rw-r--r--   0        0        0     1051 2024-05-09 06:51:25.183829 fastramqpi-7.3.2/fastramqpi/ra_utils/async_to_sync.py
+-rw-r--r--   0        0        0     2496 2024-05-09 06:51:25.184829 fastramqpi-7.3.2/fastramqpi/ra_utils/asyncio_utils.py
+-rw-r--r--   0        0        0      805 2024-05-09 06:51:25.184829 fastramqpi-7.3.2/fastramqpi/ra_utils/attrdict.py
+-rw-r--r--   0        0        0     1539 2024-05-09 06:51:25.184829 fastramqpi-7.3.2/fastramqpi/ra_utils/catchtime.py
+-rw-r--r--   0        0        0      979 2024-05-09 06:51:25.184829 fastramqpi-7.3.2/fastramqpi/ra_utils/deprecation.py
+-rw-r--r--   0        0        0     3961 2024-05-09 06:51:25.184829 fastramqpi-7.3.2/fastramqpi/ra_utils/dict_map.py
+-rw-r--r--   0        0        0     2184 2024-05-09 06:51:25.184829 fastramqpi-7.3.2/fastramqpi/ra_utils/ensure_hashable.py
+-rw-r--r--   0        0        0     3808 2024-05-09 06:51:25.185829 fastramqpi-7.3.2/fastramqpi/ra_utils/ensure_single_run.py
+-rw-r--r--   0        0        0     1723 2024-05-09 06:51:25.185829 fastramqpi-7.3.2/fastramqpi/ra_utils/generate_uuid.py
+-rw-r--r--   0        0        0     5633 2024-05-09 06:51:25.185829 fastramqpi-7.3.2/fastramqpi/ra_utils/headers.py
+-rw-r--r--   0        0        0     3245 2024-05-09 06:51:25.186829 fastramqpi-7.3.2/fastramqpi/ra_utils/jinja_filter.py
+-rw-r--r--   0        0        0     7347 2024-05-09 06:51:25.186829 fastramqpi-7.3.2/fastramqpi/ra_utils/job_settings.py
+-rw-r--r--   0        0        0     6027 2024-05-09 06:51:25.186829 fastramqpi-7.3.2/fastramqpi/ra_utils/lazy_dict.py
+-rw-r--r--   0        0        0     2929 2024-05-09 06:51:25.186829 fastramqpi-7.3.2/fastramqpi/ra_utils/load_settings.py
+-rw-r--r--   0        0        0     2935 2024-05-09 06:51:25.186829 fastramqpi-7.3.2/fastramqpi/ra_utils/multiple_replace.py
+-rw-r--r--   0        0        0     2891 2024-05-09 06:51:25.186829 fastramqpi-7.3.2/fastramqpi/ra_utils/semantic_version_type.py
+-rw-r--r--   0        0        0     1280 2024-05-09 06:51:25.187830 fastramqpi-7.3.2/fastramqpi/ra_utils/sentry_init.py
+-rw-r--r--   0        0        0     1003 2024-05-09 06:51:25.187830 fastramqpi-7.3.2/fastramqpi/ra_utils/strategies.py
+-rw-r--r--   0        0        0     3782 2024-05-09 06:51:25.187830 fastramqpi-7.3.2/fastramqpi/ra_utils/structured_url.py
+-rw-r--r--   0        0        0     4717 2024-05-09 06:51:25.187830 fastramqpi-7.3.2/fastramqpi/ra_utils/syncable.py
+-rw-r--r--   0        0        0      548 2024-05-09 06:51:25.187830 fastramqpi-7.3.2/fastramqpi/ra_utils/tqdm_wrapper.py
+-rw-r--r--   0        0        0     1834 2024-05-09 06:51:25.187830 fastramqpi-7.3.2/fastramqpi/ra_utils/transpose_dict.py
+-rw-r--r--   0        0        0      300 2024-05-09 06:51:25.188830 fastramqpi-7.3.2/fastramqpi/raclients/__init__.py
+-rw-r--r--   0        0        0     6858 2024-05-09 06:51:25.188830 fastramqpi-7.3.2/fastramqpi/raclients/auth.py
+-rw-r--r--   0        0        0       99 2024-05-09 06:51:25.188830 fastramqpi-7.3.2/fastramqpi/raclients/graph/__init__.py
+-rw-r--r--   0        0        0     7219 2024-05-09 06:51:25.188830 fastramqpi-7.3.2/fastramqpi/raclients/graph/client.py
+-rw-r--r--   0        0        0     9303 2024-05-09 06:51:25.188830 fastramqpi-7.3.2/fastramqpi/raclients/graph/transport.py
+-rw-r--r--   0        0        0     3482 2024-05-09 06:51:25.189830 fastramqpi-7.3.2/fastramqpi/raclients/graph/util.py
+-rw-r--r--   0        0        0       99 2024-05-09 06:51:25.189830 fastramqpi-7.3.2/fastramqpi/raclients/modelclient/__init__.py
+-rw-r--r--   0        0        0     4390 2024-05-09 06:51:25.189830 fastramqpi-7.3.2/fastramqpi/raclients/modelclient/base.py
+-rw-r--r--   0        0        0     1919 2024-05-09 06:51:25.189830 fastramqpi-7.3.2/fastramqpi/raclients/modelclient/lora.py
+-rw-r--r--   0        0        0     5296 2024-05-09 06:51:25.189830 fastramqpi-7.3.2/fastramqpi/raclients/modelclient/mo.py
+-rw-r--r--   0        0        0     3459 2024-05-09 06:51:25.189830 fastramqpi-7.3.2/fastramqpi/raclients/upload.py
+-rw-r--r--   0        0        0      321 2024-05-09 06:51:25.189830 fastramqpi-7.3.2/fastramqpi/ramqp/__init__.py
+-rw-r--r--   0        0        0    18731 2024-05-09 06:51:25.190830 fastramqpi-7.3.2/fastramqpi/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2024-05-09 06:51:25.190830 fastramqpi-7.3.2/fastramqpi/ramqp/amqp.py
+-rw-r--r--   0        0        0     2858 2024-05-09 06:51:25.190830 fastramqpi-7.3.2/fastramqpi/ramqp/config.py
+-rw-r--r--   0        0        0    11475 2024-05-09 06:51:25.190830 fastramqpi-7.3.2/fastramqpi/ramqp/depends.py
+-rw-r--r--   0        0        0     7130 2024-05-09 06:51:25.191830 fastramqpi-7.3.2/fastramqpi/ramqp/metrics.py
+-rw-r--r--   0        0        0     8642 2024-05-09 06:51:25.191830 fastramqpi-7.3.2/fastramqpi/ramqp/mo.py
+-rw-r--r--   0        0        0     1941 2024-05-09 06:51:25.191830 fastramqpi-7.3.2/fastramqpi/ramqp/utils.py
+-rw-r--r--   0        0        0     2173 2024-05-09 06:51:28.719183 fastramqpi-7.3.2/pyproject.toml
+-rw-r--r--   0        0        0    15537 1970-01-01 00:00:00.000000 fastramqpi-7.3.2/PKG-INFO
```

### Comparing `fastramqpi-7.3.1/LICENSES/MPL-2.0.txt` & `fastramqpi-7.3.2/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/README.md` & `fastramqpi-7.3.2/README.md`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/app.py` & `fastramqpi-7.3.2/fastramqpi/app.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/config.py` & `fastramqpi-7.3.2/fastramqpi/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/context.py` & `fastramqpi-7.3.2/fastramqpi/context.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/depends.py` & `fastramqpi-7.3.2/fastramqpi/depends.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/main.py` & `fastramqpi-7.3.2/fastramqpi/main.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/pytest_plugin.py` & `fastramqpi-7.3.2/fastramqpi/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/pytest_util.py` & `fastramqpi-7.3.2/fastramqpi/pytest_util.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/apply.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/apply.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/async_to_sync.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/async_to_sync.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/asyncio_utils.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/asyncio_utils.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/attrdict.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/attrdict.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/catchtime.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/catchtime.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/deprecation.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/dict_map.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/dict_map.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/ensure_hashable.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/ensure_hashable.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/ensure_single_run.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/ensure_single_run.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/generate_uuid.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/generate_uuid.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/headers.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/headers.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/jinja_filter.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/jinja_filter.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/job_settings.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/job_settings.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/lazy_dict.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/lazy_dict.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/load_settings.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/load_settings.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/multiple_replace.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/multiple_replace.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/semantic_version_type.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/semantic_version_type.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/sentry_init.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/sentry_init.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/strategies.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/strategies.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/structured_url.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/structured_url.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/syncable.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/syncable.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/tqdm_wrapper.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/tqdm_wrapper.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ra_utils/transpose_dict.py` & `fastramqpi-7.3.2/fastramqpi/ra_utils/transpose_dict.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/raclients/auth.py` & `fastramqpi-7.3.2/fastramqpi/raclients/auth.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/raclients/graph/client.py` & `fastramqpi-7.3.2/fastramqpi/raclients/graph/client.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/raclients/graph/transport.py` & `fastramqpi-7.3.2/fastramqpi/raclients/graph/transport.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/raclients/graph/util.py` & `fastramqpi-7.3.2/fastramqpi/raclients/graph/util.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/raclients/modelclient/base.py` & `fastramqpi-7.3.2/fastramqpi/raclients/modelclient/base.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/raclients/modelclient/lora.py` & `fastramqpi-7.3.2/fastramqpi/raclients/modelclient/lora.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/raclients/modelclient/mo.py` & `fastramqpi-7.3.2/fastramqpi/raclients/modelclient/mo.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/raclients/upload.py` & `fastramqpi-7.3.2/fastramqpi/raclients/upload.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ramqp/abstract.py` & `fastramqpi-7.3.2/fastramqpi/ramqp/abstract.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ramqp/amqp.py` & `fastramqpi-7.3.2/fastramqpi/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ramqp/config.py` & `fastramqpi-7.3.2/fastramqpi/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ramqp/depends.py` & `fastramqpi-7.3.2/fastramqpi/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ramqp/metrics.py` & `fastramqpi-7.3.2/fastramqpi/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ramqp/mo.py` & `fastramqpi-7.3.2/fastramqpi/ramqp/mo.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/fastramqpi/ramqp/utils.py` & `fastramqpi-7.3.2/fastramqpi/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-7.3.1/pyproject.toml` & `fastramqpi-7.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "7.3.1"
+version = "7.3.2"
 description = "Rammearkitektur integrations framework"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo"]
@@ -15,15 +15,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.11"
 structlog = ">=23.1,<25.0"
 pydantic = "^1.10.5"
 gql = "^3.4.0"
 more-itertools = "^9.1.0"
-prometheus-fastapi-instrumentator = ">=5.9.1,<7.0.0"
+prometheus-fastapi-instrumentator = ">=5.9.1,<8.0.0"
 fastapi = ">=0.108, <1.0"
 httpx = "^0.27.0"
 pytest = "^7.4.3"
 respx = "^0.21.0"
 tenacity = "^8.2.3"
 tqdm = "^4.65.0"
 Authlib = "^1.2.0"
```

### Comparing `fastramqpi-7.3.1/PKG-INFO` & `fastramqpi-7.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastRAMQPI
-Version: 7.3.1
+Version: 7.3.2
 Summary: Rammearkitektur integrations framework
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
@@ -18,15 +18,15 @@
 Requires-Dist: anyio (>=3.6.2,<4.0.0)
 Requires-Dist: fastapi (>=0.108,<1.0)
 Requires-Dist: frozendict (>=2.3.4,<3.0.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: prometheus-client (>=0.16,<0.18)
-Requires-Dist: prometheus-fastapi-instrumentator (>=5.9.1,<7.0.0)
+Requires-Dist: prometheus-fastapi-instrumentator (>=5.9.1,<8.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
 Requires-Dist: ramodels (>=18.5.2,<23.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: respx (>=0.21.0,<0.22.0)
 Requires-Dist: sentry-sdk (>=1.12.1,<2.0.0)
 Requires-Dist: structlog (>=23.1,<25.0)
```


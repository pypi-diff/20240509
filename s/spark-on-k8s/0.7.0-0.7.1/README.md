# Comparing `tmp/spark_on_k8s-0.7.0.tar.gz` & `tmp/spark_on_k8s-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_on_k8s-0.7.0.tar", max compression
+gzip compressed data, was "spark_on_k8s-0.7.1.tar", max compression
```

## Comparing `spark_on_k8s-0.7.0.tar` & `spark_on_k8s-0.7.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0    11357 2024-05-06 12:45:08.017305 spark_on_k8s-0.7.0/LICENSE
--rw-r--r--   0        0        0    12033 2024-05-06 12:45:08.017305 spark_on_k8s-0.7.0/README.md
--rw-r--r--   0        0        0     2574 2024-05-06 12:45:23.505297 spark_on_k8s-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       58 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/airflow/__init__.py
--rw-r--r--   0        0        0     2110 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/airflow/operator_links.py
--rw-r--r--   0        0        0    18482 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/airflow/operators.py
--rw-r--r--   0        0        0     3114 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/airflow/triggers.py
--rw-r--r--   0        0        0     1253 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/__init__.py
--rw-r--r--   0        0        0     1762 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/app.py
--rw-r--r--   0        0        0     1472 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/apps.py
--rw-r--r--   0        0        0      728 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/configuration.py
--rw-r--r--   0        0        0     1305 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/main.py
--rw-r--r--   0        0        0      524 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/utils.py
--rw-r--r--   0        0        0     6750 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/__init__.py
--rw-r--r--   0        0        0      587 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/static/app_logs.css
--rw-r--r--   0        0        0      758 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/static/apps.css
--rw-r--r--   0        0        0     1416 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/app_logs.html
--rw-r--r--   0        0        0     2953 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/apps.html
--rw-r--r--   0        0        0      368 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/error.html
--rw-r--r--   0        0        0      542 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/__init__.py
--rw-r--r--   0        0        0     1621 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/api.py
--rw-r--r--   0        0        0     6601 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/app.py
--rw-r--r--   0        0        0      690 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/apps.py
--rw-r--r--   0        0        0      553 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/namespace.py
--rw-r--r--   0        0        0     8686 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/cli/options.py
--rw-r--r--   0        0        0    27728 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/client.py
--rw-r--r--   0        0        0        0 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/k8s/__init__.py
--rw-r--r--   0        0        0     3135 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/k8s/async_client.py
--rw-r--r--   0        0        0     2849 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/k8s/sync_client.py
--rw-r--r--   0        0        0        0 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/__init__.py
--rw-r--r--   0        0        0    19764 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/app_manager.py
--rw-r--r--   0        0        0     9617 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/async_app_manager.py
--rw-r--r--   0        0        0     4048 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/configuration.py
--rw-r--r--   0        0        0      488 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/logging_mixin.py
--rw-r--r--   0        0        0     3956 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/setup_namespace.py
--rw-r--r--   0        0        0      842 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/spark_app_status.py
--rw-r--r--   0        0        0      141 2024-05-06 12:45:08.021305 spark_on_k8s-0.7.0/spark_on_k8s/utils/types.py
--rw-r--r--   0        0        0    13880 1970-01-01 00:00:00.000000 spark_on_k8s-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 16:45:13.820110 spark_on_k8s-0.7.1/LICENSE
+-rw-r--r--   0        0        0    12033 2024-05-09 16:45:13.820110 spark_on_k8s-0.7.1/README.md
+-rw-r--r--   0        0        0     2694 2024-05-09 16:45:29.456187 spark_on_k8s-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/airflow/__init__.py
+-rw-r--r--   0        0        0     2110 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/airflow/operator_links.py
+-rw-r--r--   0        0        0    18482 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/airflow/operators.py
+-rw-r--r--   0        0        0      377 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/airflow/provider_info.py
+-rw-r--r--   0        0        0     3114 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/airflow/triggers.py
+-rw-r--r--   0        0        0     1253 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/__init__.py
+-rw-r--r--   0        0        0     1762 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/app.py
+-rw-r--r--   0        0        0     1472 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/apps.py
+-rw-r--r--   0        0        0      728 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/configuration.py
+-rw-r--r--   0        0        0     1305 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/main.py
+-rw-r--r--   0        0        0      524 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/utils.py
+-rw-r--r--   0        0        0     6750 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/__init__.py
+-rw-r--r--   0        0        0      587 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/static/app_logs.css
+-rw-r--r--   0        0        0      758 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/static/apps.css
+-rw-r--r--   0        0        0     1416 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/templates/app_logs.html
+-rw-r--r--   0        0        0     2953 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/templates/apps.html
+-rw-r--r--   0        0        0      368 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/templates/error.html
+-rw-r--r--   0        0        0      542 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/cli/__init__.py
+-rw-r--r--   0        0        0     1621 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/cli/api.py
+-rw-r--r--   0        0        0     6601 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/cli/app.py
+-rw-r--r--   0        0        0      690 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/cli/apps.py
+-rw-r--r--   0        0        0      553 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/cli/namespace.py
+-rw-r--r--   0        0        0     8686 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/cli/options.py
+-rw-r--r--   0        0        0    27728 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/client.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/k8s/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/k8s/async_client.py
+-rw-r--r--   0        0        0     2849 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/k8s/sync_client.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/utils/__init__.py
+-rw-r--r--   0        0        0    19764 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/utils/app_manager.py
+-rw-r--r--   0        0        0     9617 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/utils/async_app_manager.py
+-rw-r--r--   0        0        0     4048 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/utils/configuration.py
+-rw-r--r--   0        0        0      488 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/utils/logging_mixin.py
+-rw-r--r--   0        0        0     3956 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/utils/setup_namespace.py
+-rw-r--r--   0        0        0      842 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/utils/spark_app_status.py
+-rw-r--r--   0        0        0      141 2024-05-09 16:45:13.824110 spark_on_k8s-0.7.1/spark_on_k8s/utils/types.py
+-rw-r--r--   0        0        0    13880 1970-01-01 00:00:00.000000 spark_on_k8s-0.7.1/PKG-INFO
```

### Comparing `spark_on_k8s-0.7.0/LICENSE` & `spark_on_k8s-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/README.md` & `spark_on_k8s-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/pyproject.toml` & `spark_on_k8s-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spark-on-k8s"
-version = "0.7.0"
+version = "0.7.1"
 description = "A Python package to submit and manage Apache Spark applications on Kubernetes."
 authors = ["Hussein Awala <hussein@awala.fr>"]
 readme = "README.md"
 repository = "https://github.com/hussein-awala/spark-on-k8s"
 keywords = ["spark", "kubernetes", "k8s", "spark-submit", "spark-on-k8s"]
 license = "Apache-2.0"
 packages = [{include = "spark_on_k8s"}]
@@ -44,14 +44,17 @@
 [tool.poetry.extras]
 api = ["fastapi", "kubernetes-asyncio", "uvicorn", "httpx", "jinja2", "aiohttp", "websockets"]
 airflow = ["kubernetes-asyncio", "apache-airflow", "apache-airflow-providers-cncf-kubernetes", "pendulum"]
 
 [tool.poetry.scripts]
 spark-on-k8s = "spark_on_k8s:cli.main"
 
+[tool.poetry.plugins."apache_airflow_provider"]
+provider_info = "spark_on_k8s.airflow.provider_info:get_provider_info"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 target-version = "py38"
 line-length = 110
```

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/airflow/operator_links.py` & `spark_on_k8s-0.7.1/spark_on_k8s/airflow/operator_links.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/airflow/operators.py` & `spark_on_k8s-0.7.1/spark_on_k8s/airflow/operators.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/airflow/triggers.py` & `spark_on_k8s-0.7.1/spark_on_k8s/airflow/triggers.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/__init__.py` & `spark_on_k8s-0.7.1/spark_on_k8s/api/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/app.py` & `spark_on_k8s-0.7.1/spark_on_k8s/api/app.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/apps.py` & `spark_on_k8s-0.7.1/spark_on_k8s/api/apps.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/configuration.py` & `spark_on_k8s-0.7.1/spark_on_k8s/api/configuration.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/main.py` & `spark_on_k8s-0.7.1/spark_on_k8s/api/main.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/utils.py` & `spark_on_k8s-0.7.1/spark_on_k8s/api/utils.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/__init__.py` & `spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/static/app_logs.css` & `spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/static/app_logs.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/static/apps.css` & `spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/static/apps.css`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/app_logs.html` & `spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/templates/app_logs.html`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/api/webserver/templates/apps.html` & `spark_on_k8s-0.7.1/spark_on_k8s/api/webserver/templates/apps.html`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/cli/__init__.py` & `spark_on_k8s-0.7.1/spark_on_k8s/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/cli/api.py` & `spark_on_k8s-0.7.1/spark_on_k8s/cli/api.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/cli/app.py` & `spark_on_k8s-0.7.1/spark_on_k8s/cli/app.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/cli/apps.py` & `spark_on_k8s-0.7.1/spark_on_k8s/cli/apps.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/cli/namespace.py` & `spark_on_k8s-0.7.1/spark_on_k8s/cli/namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/cli/options.py` & `spark_on_k8s-0.7.1/spark_on_k8s/cli/options.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/client.py` & `spark_on_k8s-0.7.1/spark_on_k8s/client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/k8s/async_client.py` & `spark_on_k8s-0.7.1/spark_on_k8s/k8s/async_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/k8s/sync_client.py` & `spark_on_k8s-0.7.1/spark_on_k8s/k8s/sync_client.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/utils/app_manager.py` & `spark_on_k8s-0.7.1/spark_on_k8s/utils/app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/utils/async_app_manager.py` & `spark_on_k8s-0.7.1/spark_on_k8s/utils/async_app_manager.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/utils/configuration.py` & `spark_on_k8s-0.7.1/spark_on_k8s/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/utils/setup_namespace.py` & `spark_on_k8s-0.7.1/spark_on_k8s/utils/setup_namespace.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/spark_on_k8s/utils/spark_app_status.py` & `spark_on_k8s-0.7.1/spark_on_k8s/utils/spark_app_status.py`

 * *Files identical despite different names*

### Comparing `spark_on_k8s-0.7.0/PKG-INFO` & `spark_on_k8s-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-on-k8s
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python package to submit and manage Apache Spark applications on Kubernetes.
 Home-page: https://github.com/hussein-awala/spark-on-k8s
 License: Apache-2.0
 Keywords: spark,kubernetes,k8s,spark-submit,spark-on-k8s
 Author: Hussein Awala
 Author-email: hussein@awala.fr
 Requires-Python: >=3.8,<4.0
```


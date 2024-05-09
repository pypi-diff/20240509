# Comparing `tmp/airflow_powerbi_plugin-0.0.1.tar.gz` & `tmp/airflow_powerbi_plugin-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_powerbi_plugin-0.0.1.tar", last modified: Mon Apr 29 04:54:43 2024, max compression
+gzip compressed data, was "airflow_powerbi_plugin-0.0.2a1.tar", last modified: Thu May  9 15:45:16 2024, max compression
```

## Comparing `airflow_powerbi_plugin-0.0.1.tar` & `airflow_powerbi_plugin-0.0.2a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-04-29 04:54:43.266601 airflow_powerbi_plugin-0.0.1/
--rw-r--r--   0 ambikagarg   (501) staff       (20)    11356 2024-04-27 14:27:09.000000 airflow_powerbi_plugin-0.0.1/LICENSE
--rw-r--r--   0 ambikagarg   (501) staff       (20)     4283 2024-04-29 04:54:43.265701 airflow_powerbi_plugin-0.0.1/PKG-INFO
--rw-r--r--   0 ambikagarg   (501) staff       (20)     3725 2024-04-27 14:11:40.000000 airflow_powerbi_plugin-0.0.1/README.md
--rw-r--r--   0 ambikagarg   (501) staff       (20)      538 2024-04-29 04:54:27.000000 airflow_powerbi_plugin-0.0.1/pyproject.toml
--rw-r--r--   0 ambikagarg   (501) staff       (20)       38 2024-04-29 04:54:43.266747 airflow_powerbi_plugin-0.0.1/setup.cfg
-drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-04-29 04:54:43.233408 airflow_powerbi_plugin-0.0.1/src/
-drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-04-29 04:54:43.242892 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/
--rw-r--r--   0 ambikagarg   (501) staff       (20)        0 2024-04-29 03:56:28.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/__init__.py
-drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-04-29 04:54:43.254269 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/hooks/
--rw-r--r--   0 ambikagarg   (501) staff       (20)        0 2024-03-04 15:54:39.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/hooks/__init__.py
--rw-r--r--   0 ambikagarg   (501) staff       (20)    11030 2024-04-28 02:40:33.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/hooks/powerbi.py
-drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-04-29 04:54:43.264000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/operators/
--rw-r--r--   0 ambikagarg   (501) staff       (20)        0 2024-03-04 15:48:45.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/operators/__init__.py
--rw-r--r--   0 ambikagarg   (501) staff       (20)     8104 2024-04-29 04:41:16.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/operators/powerbi.py
--rw-r--r--   0 ambikagarg   (501) staff       (20)      441 2024-04-29 04:02:20.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/powerbi_plugin.py
-drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-04-29 04:54:43.264932 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin.egg-info/
--rw-r--r--   0 ambikagarg   (501) staff       (20)     4283 2024-04-29 04:54:43.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin.egg-info/PKG-INFO
--rw-r--r--   0 ambikagarg   (501) staff       (20)      502 2024-04-29 04:54:43.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 ambikagarg   (501) staff       (20)        1 2024-04-29 04:54:43.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 ambikagarg   (501) staff       (20)       23 2024-04-29 04:54:43.000000 airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-05-09 15:45:16.604118 airflow_powerbi_plugin-0.0.2a1/
+-rw-r--r--   0 ambikagarg   (501) staff       (20)    11356 2024-04-27 14:27:09.000000 airflow_powerbi_plugin-0.0.2a1/LICENSE
+-rw-r--r--   0 ambikagarg   (501) staff       (20)     4285 2024-05-09 15:45:16.603387 airflow_powerbi_plugin-0.0.2a1/PKG-INFO
+-rw-r--r--   0 ambikagarg   (501) staff       (20)     3725 2024-05-09 15:01:42.000000 airflow_powerbi_plugin-0.0.2a1/README.md
+-rw-r--r--   0 ambikagarg   (501) staff       (20)      540 2024-05-09 15:44:28.000000 airflow_powerbi_plugin-0.0.2a1/pyproject.toml
+-rw-r--r--   0 ambikagarg   (501) staff       (20)       38 2024-05-09 15:45:16.604209 airflow_powerbi_plugin-0.0.2a1/setup.cfg
+drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-05-09 15:45:16.576031 airflow_powerbi_plugin-0.0.2a1/src/
+drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-05-09 15:45:16.586721 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/
+-rw-r--r--   0 ambikagarg   (501) staff       (20)        0 2024-04-29 03:56:28.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/__init__.py
+drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-05-09 15:45:16.595932 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/hooks/
+-rw-r--r--   0 ambikagarg   (501) staff       (20)        0 2024-03-04 15:54:39.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/hooks/__init__.py
+-rw-r--r--   0 ambikagarg   (501) staff       (20)    11030 2024-04-28 02:40:33.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/hooks/powerbi.py
+drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-05-09 15:45:16.601950 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/operators/
+-rw-r--r--   0 ambikagarg   (501) staff       (20)        0 2024-03-04 15:48:45.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/operators/__init__.py
+-rw-r--r--   0 ambikagarg   (501) staff       (20)     8142 2024-05-09 14:56:57.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/operators/powerbi.py
+-rw-r--r--   0 ambikagarg   (501) staff       (20)      441 2024-04-29 04:02:20.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/powerbi_plugin.py
+drwxr-xr-x   0 ambikagarg   (501) staff       (20)        0 2024-05-09 15:45:16.602768 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin.egg-info/
+-rw-r--r--   0 ambikagarg   (501) staff       (20)     4285 2024-05-09 15:45:16.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 ambikagarg   (501) staff       (20)      502 2024-05-09 15:45:16.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 ambikagarg   (501) staff       (20)        1 2024-05-09 15:45:16.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 ambikagarg   (501) staff       (20)       23 2024-05-09 15:45:16.000000 airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin.egg-info/top_level.txt
```

### Comparing `airflow_powerbi_plugin-0.0.1/LICENSE` & `airflow_powerbi_plugin-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_powerbi_plugin-0.0.1/PKG-INFO` & `airflow_powerbi_plugin-0.0.2a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_powerbi_plugin
-Version: 0.0.1
+Version: 0.0.2a1
 Summary: Airflow PowerBI plugin
 Author-email: Ambika Garg <ambikagarg1101@gmail.com>
 Project-URL: Homepage, https://github.com/ambika-garg/PowerBI_Airflow_Plugin
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
@@ -23,40 +23,44 @@
 To utilize this operator, simply fork the repository locally and you're ready to roll.
 
 ### Authentication
 Before diving in,
 * You must have <strong>Admin account of Power BI</strong>.
 * The plugin supports the <strong>SPN (Service Principal) authentication</strong> with the Power BI. You need to add your service prinicpal as the <strong>Contributor</strong> in your Power BI workspace.
 
-Since custom connection forms aren't feasible in Apache Airflow plugins, credentials must be stored in the secret backend. Here's what you need to store:
-1. `client_id`: The Client ID of your service principal.
-2. `client_secret`: The Client Secret of your service principal.
-3. `tenant_id`: The Tenant Id of your service principal.
+Since custom connection forms aren't feasible in Apache Airflow plugins, use can use `Generic` connection type. Here's what you need to store:
+1. `Connection Id`: Name of the connection Id
+2. `Connection Type`: Generic
+3. `Login`: The Client ID of your service principal.
+4. `Password`: The Client Secret of your service principal.
+3. `Extra`: {
+    "tenantId": The Tenant Id of your service principal.
+}
 
 ## Operators
 ### PowerBIDatasetRefreshOperator
 This operator composes the logic for this plugin. It triggers the Power BI dataset refresh and pushes the details in Xcom. It can accept the following parameters:
 
 * `dataset_id`: The dataset Id.
 * `group_id`: The workspace Id.
 * `wait_for_termination`: (Default value: True) Wait until the pre-existing or current triggered refresh completes before exiting.
 * `force_refresh`: When enabled, it will force refresh the dataset again, after pre-existing ongoing refresh request is terminated.
 * `timeout`: Time in seconds to wait for a dataset to reach a terminal status for non-asynchronous waits. Used only if ``wait_for_termination`` is True.
 * `check_interval`: Number of seconds to wait before rechecking the refresh status.
 
 ## Features
 * #### Xcom Integration: The Power BI Dataset refresh operator enriches the Xcom with essential fields for downstream tasks:
-1. `powerbi_dataset_refresh_id`: Request Id of the Dataset Refresh.
-2. `powerbi_dataset_refresh_status`: Refresh Status.
+1. `refresh_id`: Request Id of the  semantic model refresh.
+2. `refresh_status`: Refresh Status.
     * `Unknown`: Refresh state is unknown or a refresh is in progress.
     * `Completed`: Refresh successfully completed.
-    * `Failed`: Refresh failed (details in `powerbi_dataset_refresh_error`).
+    * `Failed`: Refresh failed (details in `refresh_error`).
     * `Disabled`: Refresh is disabled by a selective refresh.
-3. `powerbi_dataset_refresh_end_time`: The end date and time of the refresh (may be None if a refresh is in progress)
-4. `powerbi_dataset_refresh_error`: Failure error code in JSON format (None if no error)
+3. `refresh_end_time`: The end date and time of the refresh (may be None if a refresh is in progress)
+4. `refresh_error`: Failure error code in JSON format (None if no error)
 
 * #### External Monitoring link: The operator conveniently provides a redirect link to the Power BI UI for monitoring refreshes.
 
 ## Sample DAG to use the plugin.
 
 Ready to give it a spin? Check out the sample DAG code below:
```

### Comparing `airflow_powerbi_plugin-0.0.1/README.md` & `airflow_powerbi_plugin-0.0.2a1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,40 +8,44 @@
 To utilize this operator, simply fork the repository locally and you're ready to roll.
 
 ### Authentication
 Before diving in,
 * You must have <strong>Admin account of Power BI</strong>.
 * The plugin supports the <strong>SPN (Service Principal) authentication</strong> with the Power BI. You need to add your service prinicpal as the <strong>Contributor</strong> in your Power BI workspace.
 
-Since custom connection forms aren't feasible in Apache Airflow plugins, credentials must be stored in the secret backend. Here's what you need to store:
-1. `client_id`: The Client ID of your service principal.
-2. `client_secret`: The Client Secret of your service principal.
-3. `tenant_id`: The Tenant Id of your service principal.
+Since custom connection forms aren't feasible in Apache Airflow plugins, use can use `Generic` connection type. Here's what you need to store:
+1. `Connection Id`: Name of the connection Id
+2. `Connection Type`: Generic
+3. `Login`: The Client ID of your service principal.
+4. `Password`: The Client Secret of your service principal.
+3. `Extra`: {
+    "tenantId": The Tenant Id of your service principal.
+}
 
 ## Operators
 ### PowerBIDatasetRefreshOperator
 This operator composes the logic for this plugin. It triggers the Power BI dataset refresh and pushes the details in Xcom. It can accept the following parameters:
 
 * `dataset_id`: The dataset Id.
 * `group_id`: The workspace Id.
 * `wait_for_termination`: (Default value: True) Wait until the pre-existing or current triggered refresh completes before exiting.
 * `force_refresh`: When enabled, it will force refresh the dataset again, after pre-existing ongoing refresh request is terminated.
 * `timeout`: Time in seconds to wait for a dataset to reach a terminal status for non-asynchronous waits. Used only if ``wait_for_termination`` is True.
 * `check_interval`: Number of seconds to wait before rechecking the refresh status.
 
 ## Features
 * #### Xcom Integration: The Power BI Dataset refresh operator enriches the Xcom with essential fields for downstream tasks:
-1. `powerbi_dataset_refresh_id`: Request Id of the Dataset Refresh.
-2. `powerbi_dataset_refresh_status`: Refresh Status.
+1. `refresh_id`: Request Id of the  semantic model refresh.
+2. `refresh_status`: Refresh Status.
     * `Unknown`: Refresh state is unknown or a refresh is in progress.
     * `Completed`: Refresh successfully completed.
-    * `Failed`: Refresh failed (details in `powerbi_dataset_refresh_error`).
+    * `Failed`: Refresh failed (details in `refresh_error`).
     * `Disabled`: Refresh is disabled by a selective refresh.
-3. `powerbi_dataset_refresh_end_time`: The end date and time of the refresh (may be None if a refresh is in progress)
-4. `powerbi_dataset_refresh_error`: Failure error code in JSON format (None if no error)
+3. `refresh_end_time`: The end date and time of the refresh (may be None if a refresh is in progress)
+4. `refresh_error`: Failure error code in JSON format (None if no error)
 
 * #### External Monitoring link: The operator conveniently provides a redirect link to the Power BI UI for monitoring refreshes.
 
 ## Sample DAG to use the plugin.
 
 Ready to give it a spin? Check out the sample DAG code below:
```

### Comparing `airflow_powerbi_plugin-0.0.1/pyproject.toml` & `airflow_powerbi_plugin-0.0.2a1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "airflow_powerbi_plugin"
-version = "0.0.1"
+version = "0.0.2a1"
 authors = [
   { name="Ambika Garg", email="ambikagarg1101@gmail.com" },
 ]
 description = "Airflow PowerBI plugin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/hooks/powerbi.py` & `airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/hooks/powerbi.py`

 * *Files identical despite different names*

### Comparing `airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin/operators/powerbi.py` & `airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin/operators/powerbi.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 from airflow.models.taskinstancekey import TaskInstanceKey
 from airflow.models import BaseOperatorLink  # type: ignore
 from airflow.utils.context import Context
 
 from airflow_powerbi_plugin.hooks.powerbi import PowerBIDatasetRefreshException, PowerBIDatasetRefreshFields, PowerBIDatasetRefreshStatus, PowerBIHook
 
 
-
-
 class PowerBILink(BaseOperatorLink):
     """Construct a link to monitor a dataset in Power BI."""
 
     name = "Monitor PowerBI Dataset"
 
     def get_link(self, operator: BaseOperator, *, ti_key: TaskInstanceKey):
         url = (
@@ -85,15 +83,15 @@
     def execute(self, context: Context):
         """Refresh the Power BI Dataset."""
         self.log.info("Check if a refresh is already in progress.")
         refresh_details = self.hook.get_latest_refresh_details(
             dataset_id=self.dataset_id, group_id=self.group_id
         )
 
-        if(
+        if (
             refresh_details is None
             or refresh_details.get(PowerBIDatasetRefreshFields.STATUS.value)
             in PowerBIDatasetRefreshStatus.TERMINAL_STATUSES
         ):
             self.log.info("No pre-existing refresh found.")
             request_id = self.hook.trigger_dataset_refresh(
                 dataset_id=self.dataset_id,
@@ -108,15 +106,16 @@
                     group_id=self.group_id,
                     expected_status=PowerBIDatasetRefreshStatus.COMPLETED,
                 ):
                     self.log.info(
                         "Dataset refresh %s has completed successfully.", request_id)
                 else:
                     raise PowerBIDatasetRefreshException(
-                        f"Dataset refresh {request_id} has failed or has been cancelled."
+                        f"Dataset refresh {
+                            request_id} has failed or has been cancelled."
                     )
         else:
             if (
                 refresh_details.get(PowerBIDatasetRefreshFields.STATUS.value)
                 == PowerBIDatasetRefreshStatus.IN_PROGRESS
             ):
                 request_id = str(refresh_details.get(
@@ -134,15 +133,16 @@
                         expected_status=PowerBIDatasetRefreshStatus.COMPLETED,
                     ):
                         self.log.info(
                             "Pre-existing dataset refresh %s has completed successfully.", request_id
                         )
                     else:
                         raise PowerBIDatasetRefreshException(
-                            f"Pre-exisintg dataset refresh {request_id} has failed or has been cancelled."
+                            f"Pre-exisintg dataset refresh {
+                                request_id} has failed or has been cancelled."
                         )
 
                     if self.force_refresh:
                         self.log.info("Starting forced refresh.")
                         request_id = self.hook.trigger_dataset_refresh(
                             dataset_id=self.dataset_id,
                             group_id=self.group_id,
@@ -157,15 +157,16 @@
                                 group_id=self.group_id,
                                 expected_status=PowerBIDatasetRefreshStatus.COMPLETED,
                             ):
                                 self.log.info(
                                     "Dataset refresh %s has completed successfully.", request_id)
                             else:
                                 raise PowerBIDatasetRefreshException(
-                                    f"Dataset refresh {request_id} has failed or has been cancelled."
+                                    f"Dataset refresh {
+                                        request_id} has failed or has been cancelled."
                                 )
 
         # Retrieve refresh details after triggering refresh
         refresh_details = self.hook.get_refresh_details_by_request_id(
             dataset_id=self.dataset_id, group_id=self.group_id, request_id=request_id
         )
 
@@ -176,14 +177,14 @@
         end_time = str(refresh_details.get(
             PowerBIDatasetRefreshFields.END_TIME.value))
         error = str(refresh_details.get(
             PowerBIDatasetRefreshFields.ERROR.value))
 
         # Xcom Integration
         context["ti"].xcom_push(
-            key="powerbi_dataset_refresh_id", value=request_id)
+            key="refresh_id", value=request_id)
         context["ti"].xcom_push(
-            key="powerbi_dataset_refresh_status", value=status)
+            key="refresh_status", value=status)
         context["ti"].xcom_push(
-            key="powerbi_dataset_refresh_end_time", value=end_time)
+            key="refresh_end_time", value=end_time)
         context["ti"].xcom_push(
-            key="powerbi_dataset_refresh_error", value=error)
+            key="refresh_error", value=error)
```

### Comparing `airflow_powerbi_plugin-0.0.1/src/airflow_powerbi_plugin.egg-info/PKG-INFO` & `airflow_powerbi_plugin-0.0.2a1/src/airflow_powerbi_plugin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow_powerbi_plugin
-Version: 0.0.1
+Version: 0.0.2a1
 Summary: Airflow PowerBI plugin
 Author-email: Ambika Garg <ambikagarg1101@gmail.com>
 Project-URL: Homepage, https://github.com/ambika-garg/PowerBI_Airflow_Plugin
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
@@ -23,40 +23,44 @@
 To utilize this operator, simply fork the repository locally and you're ready to roll.
 
 ### Authentication
 Before diving in,
 * You must have <strong>Admin account of Power BI</strong>.
 * The plugin supports the <strong>SPN (Service Principal) authentication</strong> with the Power BI. You need to add your service prinicpal as the <strong>Contributor</strong> in your Power BI workspace.
 
-Since custom connection forms aren't feasible in Apache Airflow plugins, credentials must be stored in the secret backend. Here's what you need to store:
-1. `client_id`: The Client ID of your service principal.
-2. `client_secret`: The Client Secret of your service principal.
-3. `tenant_id`: The Tenant Id of your service principal.
+Since custom connection forms aren't feasible in Apache Airflow plugins, use can use `Generic` connection type. Here's what you need to store:
+1. `Connection Id`: Name of the connection Id
+2. `Connection Type`: Generic
+3. `Login`: The Client ID of your service principal.
+4. `Password`: The Client Secret of your service principal.
+3. `Extra`: {
+    "tenantId": The Tenant Id of your service principal.
+}
 
 ## Operators
 ### PowerBIDatasetRefreshOperator
 This operator composes the logic for this plugin. It triggers the Power BI dataset refresh and pushes the details in Xcom. It can accept the following parameters:
 
 * `dataset_id`: The dataset Id.
 * `group_id`: The workspace Id.
 * `wait_for_termination`: (Default value: True) Wait until the pre-existing or current triggered refresh completes before exiting.
 * `force_refresh`: When enabled, it will force refresh the dataset again, after pre-existing ongoing refresh request is terminated.
 * `timeout`: Time in seconds to wait for a dataset to reach a terminal status for non-asynchronous waits. Used only if ``wait_for_termination`` is True.
 * `check_interval`: Number of seconds to wait before rechecking the refresh status.
 
 ## Features
 * #### Xcom Integration: The Power BI Dataset refresh operator enriches the Xcom with essential fields for downstream tasks:
-1. `powerbi_dataset_refresh_id`: Request Id of the Dataset Refresh.
-2. `powerbi_dataset_refresh_status`: Refresh Status.
+1. `refresh_id`: Request Id of the  semantic model refresh.
+2. `refresh_status`: Refresh Status.
     * `Unknown`: Refresh state is unknown or a refresh is in progress.
     * `Completed`: Refresh successfully completed.
-    * `Failed`: Refresh failed (details in `powerbi_dataset_refresh_error`).
+    * `Failed`: Refresh failed (details in `refresh_error`).
     * `Disabled`: Refresh is disabled by a selective refresh.
-3. `powerbi_dataset_refresh_end_time`: The end date and time of the refresh (may be None if a refresh is in progress)
-4. `powerbi_dataset_refresh_error`: Failure error code in JSON format (None if no error)
+3. `refresh_end_time`: The end date and time of the refresh (may be None if a refresh is in progress)
+4. `refresh_error`: Failure error code in JSON format (None if no error)
 
 * #### External Monitoring link: The operator conveniently provides a redirect link to the Power BI UI for monitoring refreshes.
 
 ## Sample DAG to use the plugin.
 
 Ready to give it a spin? Check out the sample DAG code below:
```


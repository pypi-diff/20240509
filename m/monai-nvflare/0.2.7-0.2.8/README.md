# Comparing `tmp/monai_nvflare-0.2.7-py3-none-any.whl.zip` & `tmp/monai_nvflare-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15048 bytes, number of entries: 11
--rw-rw-r--  2.0 unx      842 b- defN 24-Jan-19 02:23 monai_nvflare/__init__.py
--rw-rw-r--  2.0 unx    10507 b- defN 24-Feb-20 18:07 monai_nvflare/client_algo_executor.py
--rw-rw-r--  2.0 unx     7394 b- defN 24-Jan-19 02:23 monai_nvflare/client_algo_statistics.py
--rw-rw-r--  2.0 unx     4800 b- defN 24-Jan-30 21:34 monai_nvflare/monai_bundle_persistor.py
--rw-rw-r--  2.0 unx     2145 b- defN 24-Jan-19 02:23 monai_nvflare/monai_data_stats_persistor.py
--rw-rw-r--  2.0 unx    10869 b- defN 24-Feb-20 18:07 monai_nvflare/nvflare_stats_handler.py
--rw-rw-r--  2.0 unx      747 b- defN 24-Jan-19 02:23 monai_nvflare/utils.py
--rw-rw-r--  2.0 unx     2385 b- defN 24-Apr-04 19:25 monai_nvflare-0.2.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-04 19:25 monai_nvflare-0.2.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 24-Apr-04 19:25 monai_nvflare-0.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      964 b- defN 24-Apr-04 19:25 monai_nvflare-0.2.7.dist-info/RECORD
-11 files, 40759 bytes uncompressed, 13400 bytes compressed:  67.1%
+Zip file size: 15067 bytes, number of entries: 11
+-rw-rw-r--  2.0 unx      842 b- defN 24-May-09 17:13 monai_nvflare/__init__.py
+-rw-rw-r--  2.0 unx    10559 b- defN 24-May-09 17:13 monai_nvflare/client_algo_executor.py
+-rw-rw-r--  2.0 unx     7394 b- defN 24-May-09 17:13 monai_nvflare/client_algo_statistics.py
+-rw-rw-r--  2.0 unx     4800 b- defN 24-May-09 17:13 monai_nvflare/monai_bundle_persistor.py
+-rw-rw-r--  2.0 unx     2145 b- defN 24-May-09 17:13 monai_nvflare/monai_data_stats_persistor.py
+-rw-rw-r--  2.0 unx    10869 b- defN 24-May-09 17:13 monai_nvflare/nvflare_stats_handler.py
+-rw-rw-r--  2.0 unx      747 b- defN 24-May-09 17:13 monai_nvflare/utils.py
+-rw-rw-r--  2.0 unx     2385 b- defN 24-May-09 17:25 monai_nvflare-0.2.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-09 17:25 monai_nvflare-0.2.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 24-May-09 17:25 monai_nvflare-0.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      964 b- defN 24-May-09 17:25 monai_nvflare-0.2.8.dist-info/RECORD
+11 files, 40811 bytes uncompressed, 13419 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: monai_nvflare/nvflare_stats_handler.py
 Comment: 
 
 Filename: monai_nvflare/utils.py
 Comment: 
 
-Filename: monai_nvflare-0.2.7.dist-info/METADATA
+Filename: monai_nvflare-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: monai_nvflare-0.2.7.dist-info/WHEEL
+Filename: monai_nvflare-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: monai_nvflare-0.2.7.dist-info/top_level.txt
+Filename: monai_nvflare-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: monai_nvflare-0.2.7.dist-info/RECORD
+Filename: monai_nvflare-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monai_nvflare/client_algo_executor.py

```diff
@@ -96,14 +96,15 @@
             if not isinstance(self.client_algo, ClientAlgo):
                 raise TypeError(f"client_algo must be client_algo type. Got: {type(self.client_algo)}")
             self.client_algo.initialize(
                 extra={
                     ExtraItems.CLIENT_NAME: fl_ctx.get_identity_name(),
                     ExtraItems.APP_ROOT: fl_ctx.get_prop(FLContextKey.APP_ROOT),
                     ExtraItems.STATS_SENDER: stats_sender,
+                    ExtraItems.LOGGING_FILE: False,
                 }
             )
         except Exception as e:
             self.log_exception(fl_ctx, f"client_algo initialize exception: {e}")
 
     def execute(self, task_name: str, shareable: Shareable, fl_ctx: FLContext, abort_signal: Signal) -> Shareable:
         self.log_info(fl_ctx, f"Client trainer got task: {task_name}")
```

## Comparing `monai_nvflare-0.2.7.dist-info/METADATA` & `monai_nvflare-0.2.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: monai-nvflare
-Version: 0.2.7
+Version: 0.2.8
 Summary: MONAI NVIDIA FLARE integration
 Home-page: https://github.com/NVIDIA/NVFlare
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
 Requires-Dist: monai >=1.3.0
-Requires-Dist: nvflare ~=2.4.1rc3
+Requires-Dist: nvflare ~=2.4.1rc8
 
 # MONAI Integration
 
 ## Objective
 Integration with [MONAI](https://monai.io/)'s federated learning capabilities.
 
 Add `ClientAlgoExecutor` class to allow using MONAI's `ClientAlgo` class in federated scenarios.
```


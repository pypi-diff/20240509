# Comparing `tmp/db_contrib_tool-0.7.3.tar.gz` & `tmp/db_contrib_tool-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_contrib_tool-0.7.3.tar", max compression
+gzip compressed data, was "db_contrib_tool-0.7.4.tar", max compression
```

## Comparing `db_contrib_tool-0.7.3.tar` & `db_contrib_tool-0.7.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     6286 2024-04-23 16:49:45.454339 db_contrib_tool-0.7.3/README.md
--rw-r--r--   0        0        0     2184 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/pyproject.toml
--rw-r--r--   0        0        0       13 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/__init__.py
--rw-r--r--   0        0        0      989 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/cli.py
--rw-r--r--   0        0        0        0 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/clients/__init__.py
--rw-r--r--   0        0        0     7143 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/clients/download_client.py
--rw-r--r--   0        0        0     1701 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/clients/file_service.py
--rw-r--r--   0        0        0     2636 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/clients/git_client.py
--rw-r--r--   0        0        0      305 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/clients/io_client.py
--rw-r--r--   0        0        0      984 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/clients/platform_details.py
--rw-r--r--   0        0        0     2737 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/clients/resmoke_proxy.py
--rw-r--r--   0        0        0    10275 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/config/setup_repro_env_config.yml
--rw-r--r--   0        0        0     5999 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/config.py
--rw-r--r--   0        0        0      445 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/evg_aware_bisect/README.md
--rw-r--r--   0        0        0     8844 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/evg_aware_bisect/__init__.py
--rw-r--r--   0        0        0     4639 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/evg_aware_bisect/cli.py
--rw-r--r--   0        0        0      110 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
--rw-r--r--   0        0        0      418 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
--rw-r--r--   0        0        0       52 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
--rw-r--r--   0        0        0        0 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/services/__init__.py
--rw-r--r--   0        0        0     9277 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/services/evergreen_service.py
--rw-r--r--   0        0        0     2404 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/services/git_service.py
--rw-r--r--   0        0        0     2029 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/services/platform_service.py
--rw-r--r--   0        0        0       13 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_mongot_repro_env/__init__.py
--rw-r--r--   0        0        0     3990 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_mongot_repro_env/cli.py
--rw-r--r--   0        0        0    13806 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/README.md
--rw-r--r--   0        0        0       13 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/__init__.py
--rw-r--r--   0        0        0    18510 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
--rw-r--r--   0        0        0     9874 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/cli.py
--rw-r--r--   0        0        0    10159 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/download_service.py
--rw-r--r--   0        0        0     4796 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
--rw-r--r--   0        0        0     5586 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/release_models.py
--rw-r--r--   0        0        0     4167 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/request_models.py
--rw-r--r--   0        0        0    10698 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
--rw-r--r--   0        0        0      615 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/symbolizer/README.md
--rw-r--r--   0        0        0        0 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/symbolizer/__init__.py
--rw-r--r--   0        0        0     4190 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/symbolizer/cli.py
--rw-r--r--   0        0        0     4798 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
--rw-r--r--   0        0        0    24229 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/symbolizer/mongosymb.py
--rw-r--r--   0        0        0     2269 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/usage_analytics.py
--rw-r--r--   0        0        0      235 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/utils/__init__.py
--rw-r--r--   0        0        0     1855 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/utils/build_system_options.py
--rw-r--r--   0        0        0     2108 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/utils/evergreen_conn.py
--rw-r--r--   0        0        0     1085 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/utils/filesystem.py
--rw-r--r--   0        0        0    10608 2024-04-23 16:49:45.458339 db_contrib_tool-0.7.3/src/db_contrib_tool/utils/oauth.py
--rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.3/setup.py
--rw-r--r--   0        0        0     7542 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     6286 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/README.md
+-rw-r--r--   0        0        0     2184 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/__init__.py
+-rw-r--r--   0        0        0      989 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/cli.py
+-rw-r--r--   0        0        0        0 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/__init__.py
+-rw-r--r--   0        0        0     7143 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/download_client.py
+-rw-r--r--   0        0        0     1733 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/file_service.py
+-rw-r--r--   0        0        0     2636 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/git_client.py
+-rw-r--r--   0        0        0      305 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/io_client.py
+-rw-r--r--   0        0        0      984 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/platform_details.py
+-rw-r--r--   0        0        0     2737 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/clients/resmoke_proxy.py
+-rw-r--r--   0        0        0    10275 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/config/setup_repro_env_config.yml
+-rw-r--r--   0        0        0     5999 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/config.py
+-rw-r--r--   0        0        0      445 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/README.md
+-rw-r--r--   0        0        0     8844 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/__init__.py
+-rw-r--r--   0        0        0     4639 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/cli.py
+-rw-r--r--   0        0        0      110 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/run_user_script.sh
+-rw-r--r--   0        0        0      418 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/setup_test_env.sh
+-rw-r--r--   0        0        0       52 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/teardown_test_env.sh
+-rw-r--r--   0        0        0        0 2024-05-09 17:07:33.482360 db_contrib_tool-0.7.4/src/db_contrib_tool/services/__init__.py
+-rw-r--r--   0        0        0     9277 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/services/evergreen_service.py
+-rw-r--r--   0        0        0     2404 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/services/git_service.py
+-rw-r--r--   0        0        0     2029 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/services/platform_service.py
+-rw-r--r--   0        0        0       13 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_mongot_repro_env/__init__.py
+-rw-r--r--   0        0        0     3990 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_mongot_repro_env/cli.py
+-rw-r--r--   0        0        0    13806 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/README.md
+-rw-r--r--   0        0        0       13 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/__init__.py
+-rw-r--r--   0        0        0    18510 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py
+-rw-r--r--   0        0        0     9894 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/cli.py
+-rw-r--r--   0        0        0    10159 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/download_service.py
+-rw-r--r--   0        0        0     4796 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/release_discovery_service.py
+-rw-r--r--   0        0        0     5586 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/release_models.py
+-rw-r--r--   0        0        0     4167 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/request_models.py
+-rw-r--r--   0        0        0    10710 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/setup_repro_env.py
+-rw-r--r--   0        0        0      615 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/__init__.py
+-rw-r--r--   0        0        0     4190 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/cli.py
+-rw-r--r--   0        0        0     4798 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py
+-rw-r--r--   0        0        0    24229 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/mongosymb.py
+-rw-r--r--   0        0        0     2269 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/usage_analytics.py
+-rw-r--r--   0        0        0      235 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/__init__.py
+-rw-r--r--   0        0        0     1855 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/build_system_options.py
+-rw-r--r--   0        0        0     2108 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/evergreen_conn.py
+-rw-r--r--   0        0        0     1085 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/filesystem.py
+-rw-r--r--   0        0        0    10608 2024-05-09 17:07:33.486360 db_contrib_tool-0.7.4/src/db_contrib_tool/utils/oauth.py
+-rw-r--r--   0        0        0     7972 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.4/setup.py
+-rw-r--r--   0        0        0     7542 1970-01-01 00:00:00.000000 db_contrib_tool-0.7.4/PKG-INFO
```

### Comparing `db_contrib_tool-0.7.3/README.md` & `db_contrib_tool-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/pyproject.toml` & `db_contrib_tool-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "db-contrib-tool"
-version = "0.7.3"
+version = "0.7.4"
 description = "The `db-contrib-tool` - MongoDB's tool for contributors."
 authors = ["DAG team <dev-prod-dag@mongodb.com>"]
 readme = "README.md"
 repository = "https://github.com/10gen/db-contrib-tool"
 include = [
     "src/db_contrib_tool/bisect/*.sh",
     "src/db_contrib_tool/config/*.yml",
```

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/cli.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/clients/download_client.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/download_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/clients/file_service.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/file_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,36 +24,37 @@
             if os.stat(target_file).st_size > 0:
                 out.write(os.pathsep)
             out.write(os.pathsep.join(paths))
 
         LOGGER.info(f"Finished writing binary paths on Windows to {target_file}")
 
     @staticmethod
-    def append_lines_to_file(file_name: str, content: List[str]) -> None:
-        """
-        Append the given content to the specified file.
-
-        :param file_name: File to write to.
-        :param content: Content to write to file.
-        """
-        with open(file_name, "a") as out:
-            out.write("\n".join(content))
-
-    @staticmethod
     def delete_file(file_name: str) -> None:
         """
         Delete the given file from the filesystem.
 
         :param file_name: File to delete.
         """
         os.remove(file_name)
 
     @staticmethod
-    def write_dict_to_json(file_name: str, content: dict) -> None:
+    def append_dict_to_json_file(file_name: str, content_to_append: dict) -> None:
         """
-        Write the given dict to the specified file in json format.
+        Append the given dict to the specified file in json format.
 
-        :param file_name: File to write to.
-        :param content: Content to write to file.
+        :param file_name: File to append to.
+        :param content_to_append: Content to append to file.
         """
-        with open(file_name, "w") as out:
-            json.dump(content, out, indent=2)
+        try:
+            with open(file_name, "r") as file:
+                content_json = json.load(file)
+        except Exception:
+            content_json = None
+
+        try:
+            content_dict = dict(content_json)
+            content_dict.update(content_to_append)
+        except Exception:
+            content_dict = content_to_append
+
+        with open(file_name, "w") as file:
+            json.dump(content_dict, file, indent=2)
```

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/clients/git_client.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/clients/platform_details.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/platform_details.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/clients/resmoke_proxy.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/clients/resmoke_proxy.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/config/setup_repro_env_config.yml` & `db_contrib_tool-0.7.4/src/db_contrib_tool/config/setup_repro_env_config.yml`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/config.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/config.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/evg_aware_bisect/__init__.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/__init__.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/evg_aware_bisect/cli.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/evg_aware_bisect/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/services/evergreen_service.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/services/evergreen_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/services/git_service.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/services/git_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/services/platform_service.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/services/platform_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/setup_mongot_repro_env/cli.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_mongot_repro_env/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/README.md` & `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/artifact_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/cli.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,20 @@
 @click.option(
     "--fallbackToMaster",
     "fallback_to_master",
     is_flag=True,
     help="Fallback to downloading the latest binaries from master if the requested"
     " version is not found (Only application for mongo versions).",
 )
-@click.option("--evgVersionsFile", "evg_versions_file", type=click.Path(), hidden=True)
+@click.option(
+    "--evgVersionsFile",
+    "evg_versions_file",
+    type=click.Path(),
+    hidden=True,
+)
 @click.option(
     "-ed",
     "--extractDownloads",
     "extract_downloads",
     default=True,
     hidden=True,
 )
@@ -285,15 +290,15 @@
         platform=_platform.lower() if _platform else None,
         architecture=architecture.lower(),
         variant=variant.lower() if variant else None,
         versions=massage_versions(install_last_continuous, install_last_lts, versions),
         ignore_failed_push=(not require_push),
         fallback_to_master=fallback_to_master,
         download_options=download_options,
-        evg_version_file=evg_versions_file,
+        evg_versions_file=evg_versions_file,
     )
     evg_api = get_evergreen_api(evergreen_config)
 
     def dependencies(binder: inject.Binder) -> None:
         """Define dependencies for execution."""
         binder.bind(SetupReproEnvConfig, SETUP_REPRO_ENV_CONFIG)
         binder.bind(EvergreenApi, evg_api)
```

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/download_service.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/download_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/release_discovery_service.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/release_discovery_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/release_models.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/release_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/request_models.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/request_models.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/setup_repro_env/setup_repro_env.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/setup_repro_env/setup_repro_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,29 +58,29 @@
     * architecture: Target architecture to download.
     * variant: Build Variant to download from.
 
     * versions: List of items to download.
     * ignore_failed_push: Download version even if the push task failed.
     * fallback_to_master: Should the latest master be downloaded if the version doesn't exist.
 
-    * evg_version_file: Write which evergreen version were downloaded from to this file.
+    * evg_versions_file: Write which evergreen versions were downloaded from to this file.
 
     * download_options: Options specifying how downloads should occur.
     """
 
     edition: str
     platform: Optional[str]
     architecture: str
     variant: Optional[str]
 
     versions: List[str]
     ignore_failed_push: bool
     fallback_to_master: bool
 
-    evg_version_file: Optional[str]
+    evg_versions_file: Optional[str]
 
     download_options: DownloadOptions
 
     def get_download_target(self, platform: Optional[str] = None) -> DownloadTarget:
         """
         Get the download target to use based on these parameters.
 
@@ -265,21 +265,21 @@
                     request=download_request.discovery_request,
                     exc_info=True,
                 )
 
         if is_windows():
             self.file_service.write_windows_install_paths(WINDOWS_BIN_PATHS_FILE, link_directories)
 
-        if setup_repro_params.evg_version_file is not None:
-            self.file_service.write_dict_to_json(
-                setup_repro_params.evg_version_file, downloaded_versions
+        if setup_repro_params.evg_versions_file is not None:
+            self.file_service.append_dict_to_json_file(
+                setup_repro_params.evg_versions_file, downloaded_versions
             )
             LOGGER.info(
                 "Finished writing downloaded Evergreen versions",
-                target_file=os.path.abspath(setup_repro_params.evg_version_file),
+                target_file=os.path.abspath(setup_repro_params.evg_versions_file),
             )
 
         if failed_requests:
             LOGGER.error("Some requests were not able to setup.", failed_requests=failed_requests)
             return False
 
         LOGGER.info("Downloaded versions", request_list=discovery_request_list)
```

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/symbolizer/README.md` & `db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/README.md`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/symbolizer/cli.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/cli.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/mongo_log_parser_service.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/symbolizer/mongosymb.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/symbolizer/mongosymb.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/usage_analytics.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/usage_analytics.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/utils/build_system_options.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/utils/build_system_options.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/utils/evergreen_conn.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/utils/evergreen_conn.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/utils/filesystem.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/src/db_contrib_tool/utils/oauth.py` & `db_contrib_tool-0.7.4/src/db_contrib_tool/utils/oauth.py`

 * *Files identical despite different names*

### Comparing `db_contrib_tool-0.7.3/setup.py` & `db_contrib_tool-0.7.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
  'tenacity>=8.0.1,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['db-contrib-tool = db_contrib_tool.cli:cli']}
 
 setup_kwargs = {
     'name': 'db-contrib-tool',
-    'version': '0.7.3',
+    'version': '0.7.4',
     'description': "The `db-contrib-tool` - MongoDB's tool for contributors.",
     'long_description': '# db-contrib-tool\n\nThe `db-contrib-tool` - MongoDB\'s tools for contributors.\n\n## Table of contents\n\n- [db-contrib-tool](#db-contrib-tool)\n  - [Table of contents](#table-of-contents)\n  - [Description](#description)\n  - [Dependencies](#dependencies)\n  - [Installation](#installation)\n  - [Usage](#usage)\n  - [Contributor\'s Guide (local development)](#contributors-guide-local-development)\n    - [Install project dependencies](#install-project-dependencies)\n    - [Run command line tool (local development)](#run-command-line-tool-local-development)\n    - [Run linters](#run-linters)\n    - [Run tests](#run-tests)\n    - [Pre-commit](#pre-commit)\n    - [Testing changes in mongo](#testing-changes-in-mongo)\n    - [Testing changes locally](#testing-changes-locally)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThe command line tool with various subcommands:\n- `bisect`\n  - [README.md](src/db_contrib_tool/evg_aware_bisect/README.md)\n  - performs an evergreen-aware git-bisect to find the \'last passing version\' and \'first failing version\' of mongo\n- `setup-repro-env`\n  - [README.md](src/db_contrib_tool/setup_repro_env/README.md)\n  - downloads and installs:\n    - particular MongoDB versions\n    - debug symbols\n    - artifacts (including resmoke, python scripts etc)\n    - python venv for resmoke, python scripts etc\n- `symbolize`\n  - [README.md](src/db_contrib_tool/symbolizer/README.md)\n  - Symbolizes stacktraces from recent `mongod` and `mongos` binaries compiled in Evergreen, including patch builds, mainline builds, and release/production builds.\n  - Requires authenticating to an internal MongoDB symbol mapping service.\n\n## Dependencies\n\n- Python 3.9 or later (python3 from the [MongoDB Toolchain](https://github.com/10gen/toolchain-builder/blob/master/INSTALL.md) is highly recommended)\n\n## Installation\n\nMake sure [dependencies](#dependencies) are installed.\nUse [pipx](https://pypa.github.io/pipx/) to install db-contrib-tool that will be available globally on your machine:\n\n```bash\npython3 -m pip install pipx\npython3 -m pipx ensurepath\n```\n\nInstalling db-contrib-tool:\n\n```bash\npython3 -m pipx install db-contrib-tool\n```\n\nUpgrading db-contrib-tool:\n\n```bash\npython3 -m pipx upgrade db-contrib-tool\n```\n\nIn case of installation errors, some of them may be related to pipx and could be fixed by re-installing pipx.\n\nRemoving pipx completely (WARNING! This will delete everything that is installed and managed by pipx):\n\n```bash\npython3 -m pip uninstall pipx\nrm -rf ~/.local/pipx  # in case you\'re using the default pipx home directory\n```\n\nNow you can try to install again from scratch.\n\n## Usage\n\nPrint out help message:\n\n```bash\ndb-contrib-tool --help\n```\n\nFor more information see [description](#description) section.\n\n## Contributor\'s Guide (local development)\n\n### Install project dependencies\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management.\n\n```bash\npoetry install\n```\n\n### Run command line tool (local development)\n\nSome subcommands like `bisect` and `symbolize` could be tested from the db-contrib-tool repo root:\n\n```bash\npoetry run db-contrib-tool --help\n```\n\nFor `setup-repro-env` some features can also be tested from the db-contrib-tool repo root,\nbut full features are available when running from mongo repo root.\nSee [testing changes locally](#testing-changes-locally) section.\n\n### Run linters\n\n```bash\npoetry run isort src tests\npoetry run black src tests\n```\n\n### Run tests\n\n```bash\npoetry run pytest\n```\n\n### Pre-commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time.<br>\nTo enable pre-commit on your local repository run:\n```bash\npoetry run pre-commit install\n```\n\nTo run pre-commit manually:\n```bash\npoetry run pre-commit run\n```\n\n### Testing changes in mongo\n\nThis tool is used to help run tests in the mongodb/mongo repository. On occasion, it may be\ndesirable to run a mongodb-mongo-* patch build with in-flight changes to this repository. The\nfollowing steps can be taken to accomplish that.\n\n- Create a branch with the changes you wish to test.\n- Push the branch to the origin repository: `git push -u origin <branch_name>`.\n- In the "mongo" repository, edit the [evergreen/prelude_db_contrib_tool.sh](https://github.com/10gen/mongo/blob/bbdc1347cdf2533f81b6fd05715c4ef1a092f5a6/evergreen/prelude_db_contrib_tool.sh#L12)\n  to install from the git repository instead of from pypi:\n\n  ```bash\n  pipx install "git+ssh://git@github.com/<user_name>/db-contrib-tool.git@<branch_name>" || exit 1\n  ```\n\n- Create a patch build.\n\nThe patch build should now pull down the changes from your branch instead of using the published\ndb-contrib-tool.\n\n**Note**: Since the db-contrib-tool is pulled from your branch, if you need to make additional\nchanges to the tool, you can just push to the branch and then restart the desired tasks. There is\nno need to create an additional patch build unless you also need to make updates to the mongo\nrepository.\n\n### Testing changes locally\n\nPipx installation recommendations can be found in [installation](#installation) section.\n\nThe tool can be installed via pipx from your local repo:\n\n```bash\npython3 -m pipx install /path/to/db-contrib-tool/repo/root/dir\n```\n\nIf the tool is already installed you can force install an updated version using --force flag:\n\n```bash\npython3 -m pipx install --force /path/to/db-contrib-tool/repo/root/dir\n```\n\nAfter these steps you can run in-development version of db-contrib-tool from any directory:\n\n```bash\ndb-contrib-tool --help\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a GitHub Pull Request for code review.\nThis project uses the [Evergreen Commit Queue](https://docs.devprod.prod.corp.mongodb.com/evergreen/Project-Configuration/Commit-Queue).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to pypi is done by [deploy](https://spruce.mongodb.com/commits/db-contrib-tool?taskNames=deploy)\ntask of `db-contrib-tool` project in Evergreen.\nA new version in Evergreen is created on merges to `main` branch.\n',
     'author': 'DAG team',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/10gen/db-contrib-tool',
```

### Comparing `db_contrib_tool-0.7.3/PKG-INFO` & `db_contrib_tool-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-contrib-tool
-Version: 0.7.3
+Version: 0.7.4
 Summary: The `db-contrib-tool` - MongoDB's tool for contributors.
 Home-page: https://github.com/10gen/db-contrib-tool
 Author: DAG team
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

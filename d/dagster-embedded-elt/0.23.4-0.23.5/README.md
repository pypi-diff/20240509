# Comparing `tmp/dagster-embedded-elt-0.23.4.tar.gz` & `tmp/dagster-embedded-elt-0.23.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.23.4.tar", last modified: Thu May  2 20:38:04 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.5.tar", last modified: Thu May  9 17:55:27 2024, max compression
```

## Comparing `dagster-embedded-elt-0.23.4.tar` & `dagster-embedded-elt-0.23.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.845964 dagster-embedded-elt-0.23.4/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-02 20:38:04.845964 dagster-embedded-elt-0.23.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.837964 dagster-embedded-elt-0.23.4/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.841964 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3875 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/constants.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/resource.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.845964 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4954 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8087 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    17560 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:38:04.837964 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-02 20:38:04.000000 dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-05-02 20:38:04.849964 dagster-embedded-elt-0.23.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2024-05-02 20:31:41.000000 dagster-embedded-elt-0.23.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:27.004084 dagster-embedded-elt-0.23.5/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-09 17:55:27.004084 dagster-embedded-elt-0.23.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:26.992084 dagster-embedded-elt-0.23.5/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:26.996084 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7033 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:27.004084 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5804 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    20594 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:26.992084 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-09 17:55:26.000000 dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-05-09 17:55:27.004084 dagster-embedded-elt-0.23.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-09 17:47:35.000000 dagster-embedded-elt-0.23.5/setup.py
```

### Comparing `dagster-embedded-elt-0.23.4/LICENSE` & `dagster-embedded-elt-0.23.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.4/PKG-INFO` & `dagster-embedded-elt-0.23.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/asset_decorator.py` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/resource.py` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt/dlt/translator.py` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt/dlt/translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     AssetsDefinition,
     AssetSpec,
     BackfillPolicy,
     PartitionsDefinition,
     _check as check,
     multi_asset,
 )
+from dagster._utils.merger import deep_merge_dicts
 from dagster._utils.security import non_secure_md5_hash_str
 
 from dagster_embedded_elt.sling.dagster_sling_translator import DagsterSlingTranslator
 from dagster_embedded_elt.sling.sling_replication import SlingReplicationParam, validate_replication
 
 METADATA_KEY_TRANSLATOR = "dagster_embedded_elt/dagster_sling_translator"
 METADATA_KEY_REPLICATION_CONFIG = "dagster_embedded_elt/sling_replication_config"
@@ -23,14 +24,31 @@
     """Returns a list of streams and their configs from a Sling replication config."""
     for stream, config in replication_config.get("streams", {}).items():
         if config and config.get("disabled", False):
             continue
         yield {"name": stream, "config": config}
 
 
+def streams_with_default_dagster_meta(
+    streams: Iterable[Mapping[str, Any]], replication_config: Mapping[str, Any]
+) -> Iterable[Mapping[str, Any]]:
+    """Ensures dagster meta configs in the `defaults` block of the replication_config are passed to
+    the assets definition object.
+    """
+    default_dagster_meta = replication_config.get("defaults", {}).get("meta", {}).get("dagster", {})
+    if not default_dagster_meta:
+        yield from streams
+    else:
+        for stream in streams:
+            name = stream["name"]
+            config = vars(stream["config"])
+            config["meta"] = deep_merge_dicts(default_dagster_meta, config["meta"])
+            yield {"name": name, "config": config}
+
+
 def sling_assets(
     *,
     replication_config: SlingReplicationParam,
     dagster_sling_translator: Optional[DagsterSlingTranslator] = None,
     name: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     backfill_policy: Optional[BackfillPolicy] = None,
@@ -74,29 +92,33 @@
 
             config_path = "/path/to/replication.yaml"
             @sling_assets(replication_config=config_path)
             def my_assets(context, sling: SlingResource):
                 yield from sling.replicate(context=context)
     """
     replication_config = validate_replication(replication_config)
-    streams = get_streams_from_replication(replication_config)
+
+    raw_streams = get_streams_from_replication(replication_config)
+
+    streams = streams_with_default_dagster_meta(raw_streams, replication_config)
+
     code_version = non_secure_md5_hash_str(str(replication_config).encode())
 
     dagster_sling_translator = (
         check.opt_inst_param(
             dagster_sling_translator, "dagster_sling_translator", DagsterSlingTranslator
         )
         or DagsterSlingTranslator()
     )
 
     return multi_asset(
         name=name,
         compute_kind="sling",
         partitions_def=partitions_def,
-        can_subset=False,
+        can_subset=True,
         op_tags=op_tags,
         backfill_policy=backfill_policy,
         specs=[
             AssetSpec(
                 key=dagster_sling_translator.get_asset_key(stream),
                 deps=dagster_sling_translator.get_deps_asset_key(stream),
                 description=dagster_sling_translator.get_description(stream),
```

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from dagster._utils.warnings import deprecation_warning
 from pydantic import Field
 
 from dagster_embedded_elt.sling.asset_decorator import (
     METADATA_KEY_REPLICATION_CONFIG,
     METADATA_KEY_TRANSLATOR,
     get_streams_from_replication,
+    streams_with_default_dagster_meta,
 )
 from dagster_embedded_elt.sling.dagster_sling_translator import DagsterSlingTranslator
 from dagster_embedded_elt.sling.sling_replication import SlingReplicationParam, validate_replication
 
 logger = get_dagster_logger()
 
 ANSI_ESCAPE = re.compile(r"\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])")
@@ -224,14 +225,69 @@
     """
 
     source_connection: Optional[SlingSourceConnection] = None
     target_connection: Optional[SlingTargetConnection] = None
     connections: List[SlingConnectionResource] = []
     _stdout: List[str] = []
 
+    @staticmethod
+    def _get_replication_streams_for_context(
+        context: Union[OpExecutionContext, AssetExecutionContext],
+    ) -> Dict[str, Any]:
+        """Computes the sling replication streams config for a given execution context with an
+        assets def, possibly involving a subset selection of sling assets.
+        """
+        if not context.has_assets_def:
+            no_assets_def_message = """
+            The current execution context has no backing AssetsDefinition object. Therefore,  no
+            sling assets subsetting will be performed...
+            """
+            logger.warn(no_assets_def_message)
+            return {}
+        context_streams = {}
+        assets_def = context.assets_def
+        run_config = context.run_config
+        if run_config:  # triggered via sensor
+            run_config_ops = run_config.get("ops", {})
+            if isinstance(run_config_ops, dict):
+                assets_op_config = run_config_ops.get(assets_def.op.name, {}).get("config", {})
+            else:
+                assets_op_config = {}
+            context_streams = assets_op_config.get("context_streams", {})
+            if not context_streams:
+                no_context_streams_config_message = f"""
+                It was expected that your `run_config` would provide a `context_streams` config for
+                the op {assets_def.op.name}. Instead, the received value for this op config was
+                {assets_op_config}.
+
+                NO ASSET SUBSETTING WILL BE PERFORMED!
+
+                If that was your intention, you can safely ignore this message. Otherwise, provide
+                the mentioned `context_streams` config for executing only your desired asset subset.
+                """
+                logger.warn(no_context_streams_config_message)
+        else:
+            metadata_by_key = assets_def.metadata_by_key
+            first_asset_metadata = next(iter(metadata_by_key.values()))
+            replication_config: dict[str, Any] = first_asset_metadata.get(
+                METADATA_KEY_REPLICATION_CONFIG, {}
+            )
+            dagster_sling_translator: DagsterSlingTranslator = first_asset_metadata.get(
+                METADATA_KEY_TRANSLATOR, DagsterSlingTranslator()
+            )
+            raw_streams = get_streams_from_replication(replication_config)
+            streams = streams_with_default_dagster_meta(raw_streams, replication_config)
+            selected_asset_keys = context.selected_asset_keys
+            for stream in streams:
+                asset_key = dagster_sling_translator.get_asset_key(stream)
+                if asset_key in selected_asset_keys:
+                    context_streams.update({stream["name"]: stream["config"]})
+
+        return context_streams
+
     @classmethod
     def _is_dagster_maintained(cls) -> bool:
         return True
 
     def _clean_connection_dict(self, d: Dict[str, Any]) -> Dict[str, Any]:
         d = _process_env_vars(d)
         if d["connection_string"]:
@@ -391,15 +447,19 @@
             first_asset_metadata = next(iter(metadata_by_key.values()))
             dagster_sling_translator = first_asset_metadata.get(METADATA_KEY_TRANSLATOR)
             replication_config = first_asset_metadata.get(METADATA_KEY_REPLICATION_CONFIG)
 
         # if translator has not been defined on metadata _or_ through param, then use the default constructor
         dagster_sling_translator = dagster_sling_translator or DagsterSlingTranslator()
 
-        replication_config = validate_replication(replication_config)
+        # convert to dict to enable updating the index
+        replication_config = dict(validate_replication(replication_config))
+        context_streams = self._get_replication_streams_for_context(context)
+        if context_streams:
+            replication_config.update({"streams": context_streams})
         stream_definition = get_streams_from_replication(replication_config)
 
         with self._setup_config():
             uid = uuid.uuid4()
             temp_dir = tempfile.gettempdir()
             temp_file = os.path.join(temp_dir, f"sling-replication-{uid}.json")
             env = os.environ.copy()
```

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt/sling/sling_replication.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/PKG-INFO` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.4
+Version: 0.23.5
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.4/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.5/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.4/setup.py` & `dagster-embedded-elt-0.23.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.4", "sling>=1.1.5", "dlt>=0.4"],
+    install_requires=["dagster==1.7.5", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
     extras_require={
         "test": [
             "duckdb",
         ]
     },
 )
```


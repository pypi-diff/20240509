# Comparing `tmp/stactask-0.4.2.tar.gz` & `tmp/stactask-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactask-0.4.2.tar", last modified: Fri Mar  8 14:18:22 2024, max compression
+gzip compressed data, was "stactask-0.5.0rc1.tar", last modified: Thu May  9 13:55:11 2024, max compression
```

## Comparing `stactask-0.4.2.tar` & `stactask-0.5.0rc1.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:18:22.369993 stactask-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-03-08 14:18:12.000000 stactask-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-08 14:18:12.000000 stactask-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-03-08 14:18:22.369993 stactask-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-03-08 14:18:12.000000 stactask-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-08 14:18:12.000000 stactask-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 14:18:22.369993 stactask-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:18:22.369993 stactask-0.4.2/stactask/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-08 14:18:12.000000 stactask-0.4.2/stactask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-03-08 14:18:12.000000 stactask-0.4.2/stactask/asset_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-08 14:18:12.000000 stactask-0.4.2/stactask/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 14:18:12.000000 stactask-0.4.2/stactask/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-03-08 14:18:12.000000 stactask-0.4.2/stactask/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-08 14:18:12.000000 stactask-0.4.2/stactask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:18:22.369993 stactask-0.4.2/stactask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-03-08 14:18:22.000000 stactask-0.4.2/stactask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-08 14:18:22.000000 stactask-0.4.2/stactask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 14:18:22.000000 stactask-0.4.2/stactask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-08 14:18:22.000000 stactask-0.4.2/stactask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-08 14:18:22.000000 stactask-0.4.2/stactask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 14:18:22.369993 stactask-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-03-08 14:18:12.000000 stactask-0.4.2/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-03-08 14:18:12.000000 stactask-0.4.2/tests/test_task_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:11.562483 stactask-0.5.0rc1/stactask/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/asset_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20417 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/stactask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/tests/test_task_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/tests/test_utils.py
```

### Comparing `stactask-0.4.2/LICENSE` & `stactask-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `stactask-0.4.2/pyproject.toml` & `stactask-0.5.0rc1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,54 @@
 [project]
 name = "stactask"
-version = "0.4.2"
+version = "0.5.0-pre1"
 authors = [{ name = "Matthew Hanson", email = "matt.a.hanson@gmail.com" }]
 maintainers = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 description = "Class interface for running custom algorithms and workflows on STAC Items"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 keywords = ["pystac", "imagery", "raster", "catalog", "STAC"]
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "pystac>=1.6",
     "python-dateutil>=2.7.0",
     "boto3-utils>=0.3.2",
     "fsspec>=2022.8.2",
+    "stac-asset>=0.3.0",
     "jsonpath_ng>=1.5.3",
     "requests>=2.28.1",
     "s3fs>=2022.8.2",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black~=24.0",
     "codespell~=2.2.5",
-    "mypy~=1.8.0",
-    "pre-commit~=3.5.0",
-    "pytest-cov~=4.1.0",
-    "pytest~=8.0",
-    "ruff~=0.3.1",
+    "mypy~=1.9",
+    "pre-commit~=3.7",
+    "ruff~=0.4.1",
     "types-setuptools~=69.0",
+    "boto3-stubs",
+]
+test = [
+    "pytest~=8.0",
+    "pytest-cov~=5.0",
+    "pytest-env~=1.1",
+    "moto~=5.0.5",
 ]
 
 [project.urls]
 Issues = "https://github.com/stac-utils/stactask/issues"
 Github = "https://github.com/stac-utils/stac-task"
 Changelog = "https://github.com/stac-utils/stac-task/blob/main/CHANGELOG.md"
 
@@ -51,7 +57,22 @@
 
 [[tool.mypy.overrides]]
 module = ["boto3utils", "jsonpath_ng.ext", "fsspec"]
 ignore_missing_imports = true
 
 [tool.ruff.lint]
 select = ["F", "E", "W", "I", "ERA", "RUF"]
+
+[tool.pytest.ini_options]
+addopts = "-rx -q -s -vvv"
+log_cli_level = "INFO"
+log_cli = true
+markers = ["system", "unit"]
+env = [
+    "AWS_DEFAULT_REGION=us-west-2",
+    "AWS_ACCESS_KEY_ID=foo",
+    "AWS_SECRET_ACCESS_KEY=bar",
+    "AWS_SESSION_TOKEN=baz",
+]
+filterwarnings = [
+    "ignore::UserWarning:stactask.*:",
+]
```

### Comparing `stactask-0.4.2/stactask/task.py` & `stactask-0.5.0rc1/stactask/task.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import argparse
 import asyncio
-import itertools
 import json
 import logging
 import os
 import sys
 import warnings
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from os import makedirs
 from pathlib import Path
 from shutil import rmtree
 from tempfile import mkdtemp
-from typing import Any, Callable, Dict, Iterable, List, Optional, Union
+from typing import Any, Callable, Iterable, Optional, Union
 
 import fsspec
 from boto3utils import s3
-from pystac import Item, ItemCollection
+from pystac import Asset, Item, ItemCollection
 
 from .asset_io import (
     download_item_assets,
     download_items_assets,
     upload_item_assets_to_s3,
 )
+from .config import DownloadConfig
 from .exceptions import FailedValidation
-from .utils import stac_jsonpath_match
+from .logging import TaskLoggerAdapter
+from .utils import find_collection as utils_find_collection
 
 # types
 PathLike = Union[str, Path]
 
 
+class DeprecatedStoreTrueAction(argparse._StoreTrueAction):
+    def __call__(self, parser, namespace, values, option_string=None) -> None:  # type: ignore
+        warnings.warn("Argument %s is deprecated." % self.option_strings)
+        super().__call__(parser, namespace, values, option_string)
+
+
 class Task(ABC):
     """
     Tasks can use parameters provided in a `process` Dictionary that is supplied in
     the ItemCollection JSON under the "process" field. An example process
     definition:
 
     ```
@@ -56,131 +63,149 @@
 
     name = "task"
     description = "A task for doing things"
     version = "0.1.0"
 
     def __init__(
         self: "Task",
-        payload: Dict[str, Any],
+        payload: dict[str, Any],
         workdir: Optional[PathLike] = None,
         save_workdir: Optional[bool] = None,
-        skip_upload: bool = False,
-        skip_validation: bool = False,
+        skip_upload: bool = False,  # deprecated
+        skip_validation: bool = False,  # deprecated
+        upload: bool = True,
+        validate: bool = True,
     ):
-        self.logger = logging.getLogger(self.name)
 
-        # validate input payload... or not
-        if not skip_validation:
+        if not skip_validation and validate:
             if not self.validate(payload):
                 raise FailedValidation()
 
         # set instance variables
-        self._skip_upload = skip_upload
+        if skip_upload:
+            self._upload = False
+        else:
+            self._upload = upload
+
+        self._skip_upload = not upload  # deprecated
         self._payload = payload
 
         # create temporary work directory if workdir is None
         if workdir is None:
             self._workdir = Path(mkdtemp())
             # if we are using a temp workdir we want to rm by default
             self._save_workdir = save_workdir if save_workdir is not None else False
         else:
             self._workdir = Path(workdir).absolute()
             makedirs(self._workdir, exist_ok=True)
             # if a workdir was specified we don't want to rm by default
             self._save_workdir = save_workdir if save_workdir is not None else True
 
+        self.logger = TaskLoggerAdapter(
+            logging.getLogger(self.name),
+            self._payload.get("id"),
+        )
+
     @property
-    def process_definition(self) -> Dict[str, Any]:
+    def process_definition(self) -> dict[str, Any]:
         process = self._payload.get("process", {})
         if isinstance(process, dict):
             return process
         else:
             raise ValueError(f"process is not a dict: {type(process)}")
 
     @property
-    def parameters(self) -> Dict[str, Any]:
+    def parameters(self) -> dict[str, Any]:
         task_configs = self.process_definition.get("tasks", [])
-        if isinstance(task_configs, List):
+        if isinstance(task_configs, list):
             warnings.warn(
                 "task configs is list, use a dictionary instead",
                 DeprecationWarning,
                 stacklevel=2,
             )
             task_config_list = [cfg for cfg in task_configs if cfg["name"] == self.name]
             if len(task_config_list) == 0:
                 return {}
             else:
-                task_config: Dict[str, Any] = task_config_list[0]
+                task_config: dict[str, Any] = task_config_list[0]
                 parameters = task_config.get("parameters", {})
                 if isinstance(parameters, dict):
                     return parameters
                 else:
                     raise ValueError(f"parameters is not a dict: {type(parameters)}")
-        elif isinstance(task_configs, Dict):
+        elif isinstance(task_configs, dict):
             config = task_configs.get(self.name, {})
             if isinstance(config, dict):
                 return config
             else:
                 raise ValueError(
                     f"task config for {self.name} is not a dict: {type(config)}"
                 )
         else:
             raise ValueError(f"unexpected value for 'tasks': {task_configs}")
 
     @property
-    def upload_options(self) -> Dict[str, Any]:
+    def upload_options(self) -> dict[str, Any]:
         upload_options = self.process_definition.get("upload_options", {})
         if isinstance(upload_options, dict):
             return upload_options
         else:
             raise ValueError(f"upload_options is not a dict: {type(upload_options)}")
 
     @property
-    def items_as_dicts(self) -> List[Dict[str, Any]]:
+    def collection_mapping(self) -> dict[str, str]:
+        collection_mapping = self.upload_options.get("collections", {})
+        if isinstance(collection_mapping, dict):
+            return collection_mapping
+        else:
+            raise ValueError(f"collections is not a dict: {type(collection_mapping)}")
+
+    @property
+    def items_as_dicts(self) -> list[dict[str, Any]]:
         features = self._payload.get("features", [])
         if isinstance(features, list):
             return features
         else:
             raise ValueError(f"features is not a list: {type(features)}")
 
     @property
     def items(self) -> ItemCollection:
         items_dict = {"type": "FeatureCollection", "features": self.items_as_dicts}
         return ItemCollection.from_dict(items_dict, preserve_dict=True)
 
     @classmethod
-    def validate(cls, payload: Dict[str, Any]) -> bool:
+    def validate(cls, payload: dict[str, Any]) -> bool:
         """Validates the payload and returns True if valid. If invalid, raises
         ``stactask.exceptions.FailedValidation`` or returns False."""
         # put validation logic on input Items and process definition here
         return True
 
     @classmethod
-    def add_software_version(cls, items: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+    def add_software_version(cls, items: list[dict[str, Any]]) -> list[dict[str, Any]]:
         warnings.warn(
             "add_software_version is deprecated, "
             "use add_software_version_to_item instead",
             DeprecationWarning,
         )
         modified_items = list()
         for item in items:
             modified_items.append(cls.add_software_version_to_item(item))
         return modified_items
 
     @classmethod
-    def add_software_version_to_item(cls, item: Dict[str, Any]) -> Dict[str, Any]:
+    def add_software_version_to_item(cls, item: dict[str, Any]) -> dict[str, Any]:
         """Adds software version information to a single item.
 
         Uses the processing extension.
 
         Args:
             item: A single STAC item
 
         Returns:
-            Dict[str, Any]: The same item with processing information applied.
+            dict[str, Any]: The same item with processing information applied.
         """
         processing_ext = (
             "https://stac-extensions.github.io/processing/v1.1.0/schema.json"
         )
         if "stac_extensions" not in item:
             item["stac_extensions"] = []
         item["stac_extensions"].append(processing_ext)
@@ -202,104 +227,118 @@
                 rmtree(self._workdir)
         except Exception as e:
             self.logger.warning(
                 "Failed removing work directory %s: %s", self._workdir, e
             )
 
     def assign_collections(self) -> None:
-        """Assigns new collection names based on"""
-        for i, (coll, expr) in itertools.product(
-            self._payload["features"],
-            self.upload_options.get("collections", dict()).items(),
-        ):
-            if stac_jsonpath_match(i, expr):
-                i["collection"] = coll
+        """Assigns new collection names based on upload_options collections attribute
+        according to the first matching expression in the order they are defined."""
+        for item in self._payload["features"]:
+            if coll := utils_find_collection(self.collection_mapping, item):
+                item["collection"] = coll
 
     def download_item_assets(
         self,
         item: Item,
         path_template: str = "${collection}/${id}",
-        keep_original_filenames: bool = False,
-        **kwargs: Any,
+        config: Optional[DownloadConfig] = None,
+        keep_non_downloaded: bool = True,
     ) -> Item:
         """Download provided asset keys for the given item. Assets are
         saved in workdir in a directory (as specified by path_template), and
         the items are updated with the new asset hrefs.
 
         Args:
             item (pystac.Item): STAC Item for which assets need be downloaded.
-            assets (Optional[List[str]]): List of asset keys to download.
+            assets (Optional[list[str]]): List of asset keys to download.
                 Defaults to all assets.
             path_template (Optional[str]): String to be interpolated to specify
                 where to store downloaded files.
             keep_original_filenames (Optional[bool]): Controls whether original
                 file names should be used, or asset key + extension.
         """
-        outdir = str(self._workdir / path_template)
-        loop = asyncio.get_event_loop()
-        item = loop.run_until_complete(
+        return asyncio.get_event_loop().run_until_complete(
             download_item_assets(
                 item,
-                path_template=outdir,
-                keep_original_filenames=keep_original_filenames,
-                **kwargs,
+                path_template=str(self._workdir / path_template),
+                config=config,
+                keep_non_downloaded=keep_non_downloaded,
             )
         )
-        return item
 
     def download_items_assets(
         self,
         items: Iterable[Item],
         path_template: str = "${collection}/${id}",
-        keep_original_filenames: bool = False,
-        **kwargs: Any,
-    ) -> List[Item]:
+        config: Optional[DownloadConfig] = None,
+        keep_non_downloaded: bool = True,
+    ) -> list[Item]:
         """Download provided asset keys for the given items. Assets are
         saved in workdir in a directory (as specified by path_template), and
         the items are updated with the new asset hrefs.
 
         Args:
-            items (List[pystac.Item]): List of STAC Items for which assets need
+            items (list[pystac.Item]): List of STAC Items for which assets need
                 be downloaded.
-            assets (Optional[List[str]]): List of asset keys to download.
+            assets (Optional[list[str]]): List of asset keys to download.
                 Defaults to all assets.
             path_template (Optional[str]): String to be interpolated to specify
                 where to store downloaded files.
             keep_original_filenames (Optional[bool]): Controls whether original
                 file names should be used, or asset key + extension.
         """
-        outdir = str(self._workdir / path_template)
-        loop = asyncio.get_event_loop()
-        items = loop.run_until_complete(
-            download_items_assets(
-                items,
-                path_template=outdir,
-                keep_original_filenames=keep_original_filenames,
-                **kwargs,
+        return list(
+            asyncio.get_event_loop().run_until_complete(
+                download_items_assets(
+                    items,
+                    path_template=str(self._workdir / path_template),
+                    config=config,
+                    keep_non_downloaded=keep_non_downloaded,
+                )
             )
         )
-        return list(items)
 
     def upload_item_assets_to_s3(
         self,
         item: Item,
-        assets: Optional[List[str]] = None,
+        assets: Optional[list[str]] = None,
         s3_client: Optional[s3] = None,
     ) -> Item:
-        if self._skip_upload:
+        if self._upload:
+            item = upload_item_assets_to_s3(
+                item=item, assets=assets, s3_client=s3_client, **self.upload_options
+            )
+        else:
             self.logger.warning("Skipping upload of new and modified assets")
-            return item
-        item = upload_item_assets_to_s3(
-            item=item, assets=assets, s3_client=s3_client, **self.upload_options
-        )
+
         return item
 
+    def _is_local_asset(self, asset: Asset) -> bool:
+        return bool(asset.href.startswith(str(self._workdir)))
+
+    def _get_local_asset_keys(self, item: Item) -> list[str]:
+        return [
+            key for key, asset in item.assets.items() if self._is_local_asset(asset)
+        ]
+
+    def upload_local_item_assets_to_s3(
+        self,
+        item: Item,
+        s3_client: Optional[s3] = None,
+    ) -> Item:
+        return self.upload_item_assets_to_s3(
+            item=item,
+            assets=self._get_local_asset_keys(item),
+            s3_client=s3_client,
+        )
+
     # this should be in PySTAC
     @staticmethod
-    def create_item_from_item(item: Dict[str, Any]) -> Dict[str, Any]:
+    def create_item_from_item(item: dict[str, Any]) -> dict[str, Any]:
         new_item = deepcopy(item)
         # create a derived output item
         links = [
             link["href"] for link in item.get("links", []) if link["rel"] == "self"
         ]
         if len(links) == 1:
             # add derived from link
@@ -310,48 +349,47 @@
                     "href": links[0],
                     "type": "application/json",
                 }
             )
         return new_item
 
     @abstractmethod
-    def process(self, **kwargs: Any) -> List[Dict[str, Any]]:
+    def process(self, **kwargs: Any) -> list[dict[str, Any]]:
         """Main task logic - virtual
 
         Returns:
             [type]: [description]
         """
         # download assets of interest, this will update self.items
         # do some stuff
         pass
 
-    def post_process_item(self, item: Dict[str, Any]) -> Dict[str, Any]:
+    def post_process_item(self, item: dict[str, Any]) -> dict[str, Any]:
         """Perform post-processing operations on an item.
 
         E.g. add software version information.
 
         Most tasks should prefer to not override this method, as logic should be
         kept in :py:meth:`Task.process`. If you do override this method, make
         sure to call ``super().post_process_item()`` AFTER doing any custom
         post-processing, so any regular behavior can take your changes into account.
 
         Args:
             item: An item produced by :py:meth:`Task.process`
 
         Returns:
-            Dict[str, Any]: The item with any additional attributes applied.
+            dict[str, Any]: The item with any additional attributes applied.
         """
-        item = self.add_software_version_to_item(item)
         assert "stac_extensions" in item
         assert isinstance(item["stac_extensions"], list)
         item["stac_extensions"].sort()
         return item
 
     @classmethod
-    def handler(cls, payload: Dict[str, Any], **kwargs: Any) -> Dict[str, Any]:
+    def handler(cls, payload: dict[str, Any], **kwargs: Any) -> dict[str, Any]:
         task = None
         try:
             if "href" in payload or "url" in payload:
                 # read input
                 with fsspec.open(payload.get("href", payload.get("url"))) as f:
                     payload = json.loads(f.read())
 
@@ -369,15 +407,15 @@
                 task.logger.error(err, exc_info=True)
                 raise err
         finally:
             if task:
                 task.cleanup_workdir()
 
     @classmethod
-    def parse_args(cls, args: List[str]) -> Dict[str, Any]:
+    def parse_args(cls, args: list[str]) -> dict[str, Any]:
         dhf = argparse.ArgumentDefaultsHelpFormatter
         parser0 = argparse.ArgumentParser(description=cls.description)
         parser0.add_argument(
             "--version",
             help="Print version and exit",
             action="version",
             version=cls.version,
@@ -387,57 +425,113 @@
         pparser.add_argument(
             "--logging", default="INFO", help="DEBUG, INFO, WARN, ERROR, CRITICAL"
         )
 
         subparsers = parser0.add_subparsers(dest="command")
 
         # run
-        h = "Process STAC Item Collection"
         parser = subparsers.add_parser(
-            "run", parents=[pparser], help=h, formatter_class=dhf
+            "run",
+            parents=[pparser],
+            formatter_class=dhf,
+            help="Process STAC Item Collection",
         )
         parser.add_argument(
-            "input", help="Full path of item collection to process (s3 or local)"
+            "input",
+            nargs="?",
+            help="Full path of item collection to process (s3 or local)",
         )
 
-        h = "Write output payload to this URL"
-        parser.add_argument("--output", help=h, default=None)
+        parser.add_argument(
+            "--output",
+            default=None,
+            help="Write output payload to this URL",
+        )
 
         # additional options
-        h = "Use this as work directory. Will be created."
-        parser.add_argument("--workdir", help=h, default=None, type=Path)
-        h = "Save workdir after completion"
         parser.add_argument(
-            "--save-workdir", dest="save_workdir", action="store_true", default=False
+            "--workdir",
+            default=None,
+            type=Path,
+            help="Use this as work directory. Will be created.",
         )
-        h = "Skip uploading of any generated assets and resulting STAC Items"
+
         parser.add_argument(
-            "--skip-upload", dest="skip_upload", action="store_true", default=False
+            "--save-workdir",
+            dest="save_workdir",
+            action="store_true",
+            default=False,
+            help="Save workdir after completion",
+        )
+
+        # skips are deprecated in favor of boolean optionals
+        parser.add_argument(
+            "--skip-upload",
+            dest="skip_upload",
+            action=DeprecatedStoreTrueAction,
+            default=False,
+            help="DEPRECATED: Skip uploading of generated assets and STAC Items",
         )
-        h = "Skip validation of input payload"
         parser.add_argument(
             "--skip-validation",
             dest="skip_validation",
+            action=DeprecatedStoreTrueAction,
+            default=False,
+            help="DEPRECATED: Skip validation of input payload",
+        )
+
+        parser.add_argument(
+            "--upload",
+            dest="upload",
+            action="store_true",
+            default=True,
+            help="Upload generated assets and resulting STAC Items",
+        )
+        parser.add_argument(
+            "--no-upload",
+            dest="upload",
+            action="store_false",
+            help="Don't upload generated assets and resulting STAC Items",
+        )
+        parser.add_argument(
+            "--validate",
+            dest="validate",
+            action="store_true",
+            default=True,
+            help="Validate input payload",
+        )
+        parser.add_argument(
+            "--no-validate",
+            dest="validate",
+            action="store_false",
+            help="Don't validate input payload",
+        )
+
+        parser.add_argument(
+            "--local",
             action="store_true",
             default=False,
+            help=""" Run local mode
+(save-workdir = True, upload = False,
+workdir = 'local-output', output = 'local-output/output-payload.json') """,
         )
-        h = """ Run local mode
-(save-workdir = True, skip-upload = True, skip-validation = True,
-workdir = 'local-output', output = 'local-output/output-payload.json') """
-        parser.add_argument("--local", help=h, action="store_true", default=False)
 
         # turn Namespace into dictionary
         pargs = vars(parser0.parse_args(args))
         # only keep keys that are not None
         pargs = {k: v for k, v in pargs.items() if v is not None}
 
+        if pargs.pop("skip_validation", False):
+            pargs["validate"] = False
+        if pargs.pop("skip_upload", False):
+            pargs["upload"] = False
+
         if pargs.pop("local", False):
-            # local mode sets all of
-            for k in ["save_workdir", "skip_upload", "skip_validation"]:
-                pargs[k] = True
+            pargs["save_workdir"] = True
+            pargs["upload"] = False
             if pargs.get("workdir") is None:
                 pargs["workdir"] = "local-output"
             if pargs.get("output") is None:
                 pargs["output"] = Path(pargs["workdir"]) / "output-payload.json"
 
         if pargs.get("command", None) is None:
             parser.print_help()
@@ -462,26 +556,31 @@
             "fsspec",
             "asyncio",
             "aiobotocore",
         ]:
             logging.getLogger(ql).propagate = False
 
         if cmd == "run":
-            href = args.pop("input")
+            href = args.pop("input", None)
             href_out = args.pop("output", None)
 
             # read input
-            with fsspec.open(href) as f:
-                payload = json.loads(f.read())
+            if href is None:
+                payload = json.load(sys.stdin)
+            else:
+                with fsspec.open(href) as f:
+                    payload = json.loads(f.read())
 
             # run task handler
             payload_out = cls.handler(payload, **args)
 
             # write output
-            if href_out is not None:
+            if href_out is None:
+                json.dump(payload_out, sys.stdout)
+            else:
                 with fsspec.open(href_out, "w") as f:
                     f.write(json.dumps(payload_out))
 
 
 # from https://pythonalgos.com/runtimeerror-event-loop-is-closed-asyncio-fix/
 """fix yelling at me error"""
 from asyncio.proactor_events import _ProactorBasePipeTransport  # noqa
```

### Comparing `stactask-0.4.2/tests/test_task_download.py` & `stactask-0.5.0rc1/tests/test_task_download.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,115 +1,153 @@
 import json
+import os
 from pathlib import Path
-from typing import Any, Dict
+from typing import Any
 
 import pytest
+import stac_asset
+
+from stactask.config import DownloadConfig
 
 from .tasks import NothingTask
 
 
 @pytest.fixture
-def item_collection() -> Dict[str, Any]:
+def item_collection() -> dict[str, Any]:
     name = "sentinel2-l2a-j2k-payload"
     filename = Path(__file__).parent / "fixtures" / f"{name}.json"
     with open(filename) as f:
         items = json.loads(f.read())
     assert isinstance(items, dict)
     return items
 
 
-def test_download_nosuch_asset(item_collection: Dict[str, Any]) -> None:
+def test_download_nosuch_asset(tmp_path: Path, item_collection: dict[str, Any]) -> None:
+    t = NothingTask(
+        item_collection,
+        workdir=tmp_path / "test-task-download-nosuch-asset",
+        save_workdir=True,
+    )
+    item = t.download_item_assets(
+        t.items[0], config=DownloadConfig(include=["nosuch_asset"])
+    )
+
+    # new item has same assets hrefs as old item
+    assert [x.href for x in item.assets.values()] == [
+        x.href for x in t.items[0].assets.values()
+    ]
+
+
+def test_download_asset_dont_keep_existing(
+    tmp_path: Path, item_collection: dict[str, Any]
+) -> None:
     t = NothingTask(
         item_collection,
+        workdir=tmp_path / "test-task-download-nosuch-asset",
+        save_workdir=True,
+    )
+    item = t.download_item_assets(
+        t.items[0],
+        config=DownloadConfig(include=["nosuch_asset"]),
+        keep_non_downloaded=False,
     )
-    item = t.download_item_assets(t.items[0], assets=["nosuch_asset"]).to_dict()
-    # new item same as old item
-    assert item["assets"] == t.items[0].to_dict()["assets"]
+
+    # new item has no assets
+    assert item.assets == {}
 
 
 # @vcr.use_cassette(str(cassettepath / 'download_assets'))
-def test_download_item_asset(tmp_path: Path, item_collection: Dict[str, Any]) -> None:
+def test_download_item_asset(tmp_path: Path, item_collection: dict[str, Any]) -> None:
     t = NothingTask(item_collection, workdir=tmp_path / "test-task-download-item-asset")
-    item = t.download_item_assets(t.items[0], assets=["tileinfo_metadata"]).to_dict()
-    fname = item["assets"]["tileinfo_metadata"]["href"]
-    filename = Path(fname)
-    assert filename.is_file() is True
+    item = t.download_item_assets(
+        t.items[0], config=DownloadConfig(include=["tileinfo_metadata"])
+    )
+    assert Path(item.assets["tileinfo_metadata"].get_absolute_href()).is_file()
 
 
 def test_download_keep_original_filenames(
-    tmp_path: Path, item_collection: Dict[str, Any]
+    tmp_path: Path, item_collection: dict[str, Any]
 ) -> None:
     t = NothingTask(
         item_collection,
         workdir=tmp_path / "test-task-download-item-asset",
     )
     item = t.download_item_assets(
-        t.items[0], assets=["tileinfo_metadata"], keep_original_filenames=True
+        t.items[0],
+        config=DownloadConfig(
+            include=["tileinfo_metadata"],
+            file_name_strategy=stac_asset.FileNameStrategy.FILE_NAME,
+        ),
     ).to_dict()
     fname = item["assets"]["tileinfo_metadata"]["href"]
     filename = Path(fname)
     assert filename.name == "tileInfo.json"
 
 
 def test_download_item_asset_local(
-    tmp_path: Path, item_collection: Dict[str, Any]
+    tmp_path: Path, item_collection: dict[str, Any]
 ) -> None:
     t = NothingTask(item_collection, workdir=tmp_path / "test-task-download-item-asset")
-    item = t.download_item_assets(t.items[0], assets=["tileinfo_metadata"])
-    fname = item.assets["tileinfo_metadata"].href
-    filename = Path(fname)
-    assert filename.is_file() is True
+    item = t.download_item_assets(
+        t.items[0], config=DownloadConfig(include=["tileinfo_metadata"])
+    )
+
+    assert (
+        Path(os.path.dirname(item.self_href)) / item.assets["tileinfo_metadata"].href
+    ).is_file()
+
     # Downloaded to local, as in prev test.
     # With the asset hrefs updated by the prev download, we "download" again to subdir
     item = t.download_item_assets(
-        item, assets=["tileinfo_metadata"], path_template="again/${collection}/${id}"
+        item=item,
+        config=DownloadConfig(include=["tileinfo_metadata"]),
+        path_template="again/${collection}/${id}",
     )
-    href = item.assets["tileinfo_metadata"].href
+    assert "again" in item.self_href
+    href = item.assets["tileinfo_metadata"].get_absolute_href()
     assert "again" in href
-    filename = Path(href)
-    assert filename.is_file() is True
+    assert Path(href).is_file()
 
 
 # @vcr.use_cassette(str(cassettepath / 'download_assets'))
-def test_download_item_assets(tmp_path: Path, item_collection: Dict[str, Any]) -> None:
+def test_download_item_assets(tmp_path: Path, item_collection: dict[str, Any]) -> None:
     t = NothingTask(
         item_collection,
         workdir=tmp_path / "test-task-download-item-assets",
         save_workdir=True,
     )
     item = t.download_item_assets(
-        t.items[0], assets=["tileinfo_metadata", "granule_metadata"]
-    ).to_dict()
-    filename = Path(item["assets"]["tileinfo_metadata"]["href"])
-    assert filename.is_file() is True
-    filename = Path(item["assets"]["granule_metadata"]["href"])
-    assert filename.is_file() is True
+        t.items[0],
+        config=DownloadConfig(include=["tileinfo_metadata", "granule_metadata"]),
+    )
 
+    assert Path(item.assets["tileinfo_metadata"].get_absolute_href()).is_file()
+    assert Path(item.assets["granule_metadata"].get_absolute_href()).is_file()
 
-def test_download_items_assets(tmp_path: Path, item_collection: Dict[str, Any]) -> None:
+
+def test_download_items_assets(tmp_path: Path, item_collection: dict[str, Any]) -> None:
     asset_key = "tileinfo_metadata"
     t = NothingTask(
         item_collection,
         workdir=tmp_path / "test-task-download-items-assets",
         save_workdir=True,
     )
-    items = [i.to_dict() for i in t.download_items_assets(t.items, assets=[asset_key])]
-    filename = Path(items[0]["assets"][asset_key]["href"])
-    assert filename.is_file() is True
-    filename = Path(items[1]["assets"][asset_key]["href"])
-    assert filename.is_file() is True
+    items = t.download_items_assets(t.items, config=DownloadConfig(include=[asset_key]))
+
+    assert len(items) == 2
+    for item in items:
+        assert Path(item.assets[asset_key].get_absolute_href()).is_file()
 
 
 # @vcr.use_cassette(str(cassettepath / 'download_assets'))
 @pytest.mark.s3_requester_pays
-def test_download_large_asset(tmp_path: Path, item_collection: Dict[str, Any]) -> None:
+def test_download_large_asset(tmp_path: Path, item_collection: dict[str, Any]) -> None:
     t = NothingTask(
         item_collection,
         workdir=tmp_path / "test-task-download-assets",
         save_workdir=True,
     )
     item = t.download_item_assets(
-        t.items[0], assets=["red"], requester_pays=True
-    ).to_dict()
-    filename = Path(item["assets"]["red"]["href"])
-    assert filename.is_file() is True
-    del t
+        t.items[0], config=DownloadConfig(s3_requester_pays=True, include=["red"])
+    )
+
+    assert Path(item.assets["red"].get_absolute_href()).is_file()
```


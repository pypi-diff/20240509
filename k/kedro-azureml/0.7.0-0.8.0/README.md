# Comparing `tmp/kedro_azureml-0.7.0.tar.gz` & `tmp/kedro_azureml-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_azureml-0.7.0.tar", max compression
+gzip compressed data, was "kedro_azureml-0.8.0.tar", max compression
```

## Comparing `kedro_azureml-0.7.0.tar` & `kedro_azureml-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11338 2023-11-15 14:12:47.078241 kedro_azureml-0.7.0/LICENSE
--rw-r--r--   0        0        0     2441 2023-11-15 14:12:47.078241 kedro_azureml-0.7.0/README.md
--rw-r--r--   0        0        0       96 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/__init__.py
--rw-r--r--   0        0        0        0 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/auth/__init__.py
--rw-r--r--   0        0        0      879 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/auth/utils.py
--rw-r--r--   0        0        0    12998 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/cli.py
--rw-r--r--   0        0        0     7407 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/cli_functions.py
--rw-r--r--   0        0        0     2551 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/client.py
--rw-r--r--   0        0        0     4613 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/config.py
--rw-r--r--   0        0        0      323 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/constants.py
--rw-r--r--   0        0        0      604 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/datasets/__init__.py
--rw-r--r--   0        0        0     9019 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/datasets/asset_dataset.py
--rw-r--r--   0        0        0      130 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/datasets/file_dataset.py
--rw-r--r--   0        0        0      430 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/datasets/pandas_dataset.py
--rw-r--r--   0        0        0     4948 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/datasets/pipeline_dataset.py
--rw-r--r--   0        0        0     2653 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/datasets/runner_dataset.py
--rw-r--r--   0        0        0      301 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/datasets/v1_datasets.py
--rw-r--r--   0        0        0      149 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/distributed/__init__.py
--rw-r--r--   0        0        0      541 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/distributed/config.py
--rw-r--r--   0        0        0      701 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/distributed/decorators.py
--rw-r--r--   0        0        0     1220 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/distributed/utils.py
--rw-r--r--   0        0        0    14861 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/generator.py
--rw-r--r--   0        0        0     2290 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/hooks.py
--rw-r--r--   0        0        0     2784 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/manager.py
--rw-r--r--   0        0        0     3838 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/runner.py
--rw-r--r--   0        0        0      695 2023-11-15 14:12:47.090242 kedro_azureml-0.7.0/kedro_azureml/utils.py
--rw-r--r--   0        0        0     1776 2023-11-15 14:12:47.094241 kedro_azureml-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3815 1970-01-01 00:00:00.000000 kedro_azureml-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-05-09 19:07:11.118582 kedro_azureml-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2441 2024-05-09 19:07:11.118582 kedro_azureml-0.8.0/README.md
+-rw-r--r--   0        0        0       96 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/auth/__init__.py
+-rw-r--r--   0        0        0      879 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/auth/utils.py
+-rw-r--r--   0        0        0    12998 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/cli.py
+-rw-r--r--   0        0        0     7407 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/cli_functions.py
+-rw-r--r--   0        0        0     2551 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/client.py
+-rw-r--r--   0        0        0     4766 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/config.py
+-rw-r--r--   0        0        0      323 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/constants.py
+-rw-r--r--   0        0        0      604 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/datasets/__init__.py
+-rw-r--r--   0        0        0     9266 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/datasets/asset_dataset.py
+-rw-r--r--   0        0        0      130 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/datasets/file_dataset.py
+-rw-r--r--   0        0        0      430 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/datasets/pandas_dataset.py
+-rw-r--r--   0        0        0     5160 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/datasets/pipeline_dataset.py
+-rw-r--r--   0        0        0     2653 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/datasets/runner_dataset.py
+-rw-r--r--   0        0        0      301 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/datasets/v1_datasets.py
+-rw-r--r--   0        0        0      149 2024-05-09 19:07:11.126582 kedro_azureml-0.8.0/kedro_azureml/distributed/__init__.py
+-rw-r--r--   0        0        0      541 2024-05-09 19:07:11.130582 kedro_azureml-0.8.0/kedro_azureml/distributed/config.py
+-rw-r--r--   0        0        0      701 2024-05-09 19:07:11.130582 kedro_azureml-0.8.0/kedro_azureml/distributed/decorators.py
+-rw-r--r--   0        0        0     1220 2024-05-09 19:07:11.130582 kedro_azureml-0.8.0/kedro_azureml/distributed/utils.py
+-rw-r--r--   0        0        0    14861 2024-05-09 19:07:11.130582 kedro_azureml-0.8.0/kedro_azureml/generator.py
+-rw-r--r--   0        0        0     2290 2024-05-09 19:07:11.130582 kedro_azureml-0.8.0/kedro_azureml/hooks.py
+-rw-r--r--   0        0        0     2784 2024-05-09 19:07:11.130582 kedro_azureml-0.8.0/kedro_azureml/manager.py
+-rw-r--r--   0        0        0     3838 2024-05-09 19:07:11.130582 kedro_azureml-0.8.0/kedro_azureml/runner.py
+-rw-r--r--   0        0        0      695 2024-05-09 19:07:11.130582 kedro_azureml-0.8.0/kedro_azureml/utils.py
+-rw-r--r--   0        0        0     1777 2024-05-09 19:07:11.130582 kedro_azureml-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3865 1970-01-01 00:00:00.000000 kedro_azureml-0.8.0/PKG-INFO
```

### Comparing `kedro_azureml-0.7.0/LICENSE` & `kedro_azureml-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/README.md` & `kedro_azureml-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/auth/utils.py` & `kedro_azureml-0.8.0/kedro_azureml/auth/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/cli.py` & `kedro_azureml-0.8.0/kedro_azureml/cli.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/cli_functions.py` & `kedro_azureml-0.8.0/kedro_azureml/cli_functions.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/client.py` & `kedro_azureml-0.8.0/kedro_azureml/client.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/config.py` & `kedro_azureml-0.8.0/kedro_azureml/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 from typing import Dict, Optional, Type
 
 import yaml
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, Field, field_validator
+from typing_extensions import Annotated
 
 from kedro_azureml.utils import update_dict
 
 
 class DefaultConfigDict(defaultdict):
     def __getitem__(self, key):
         defaults: BaseModel = super().__getitem__("__default__")
@@ -35,29 +36,32 @@
     @staticmethod
     def _create_default_dict_with(
         value: dict, default, dict_cls: Type = DefaultConfigDict
     ):
         default_value = (value := value or {}).get("__default__", default)
         return dict_cls(lambda: default_value, value)
 
-    @validator("compute", always=True)
+    @field_validator("compute")
+    @classmethod
     def _validate_compute(cls, value):
         return AzureMLConfig._create_default_dict_with(
             value, ComputeConfig(cluster_name="{cluster_name}")
         )
 
     subscription_id: str
     resource_group: str
     workspace_name: str
     experiment_name: str
-    compute: Optional[Dict[str, ComputeConfig]]
-    temporary_storage: Optional[AzureTempStorageConfig]
-    environment_name: Optional[str]
-    code_directory: Optional[str]
-    working_directory: Optional[str]
+    compute: Annotated[
+        Optional[Dict[str, ComputeConfig]], Field(validate_default=True)
+    ] = None
+    temporary_storage: Optional[AzureTempStorageConfig] = None
+    environment_name: Optional[str] = None
+    code_directory: Optional[str] = None
+    working_directory: Optional[str] = None
     pipeline_data_passing: Optional[PipelineDataPassingConfig] = None
 
 
 class KedroAzureMLConfig(BaseModel):
     azure: AzureMLConfig
     docker: Optional[DockerConfig] = None
```

### Comparing `kedro_azureml-0.7.0/kedro_azureml/datasets/__init__.py` & `kedro_azureml-0.8.0/kedro_azureml/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/datasets/asset_dataset.py` & `kedro_azureml-0.8.0/kedro_azureml/datasets/asset_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,25 +77,33 @@
         self,
         azureml_dataset: str,
         dataset: Union[str, Type[AbstractDataset], Dict[str, Any]],
         root_dir: str = "data",
         filepath_arg: str = "filepath",
         azureml_type: AzureMLDataAssetType = "uri_folder",
         version: Optional[Version] = None,
+        metadata: Dict[str, Any] = None,
     ):
         """
         azureml_dataset: Name of the AzureML file azureml_dataset.
         dataset: Type of the underlying dataset that is saved on AzureML e.g. Parquet, Csv etc.
         root_dir: The local folder where the dataset should be saved during local runs.
                 Relevant only for local execution via `kedro run`.
         filepath_arg: Filepath arg on the wrapped dataset, defaults to `filepath`
         azureml_type: Either `uri_folder` or `uri_file`
         version: Version of the AzureML dataset to be used in kedro format.
+        metadata: Any arbitrary metadata.
+            This is ignored by Kedro, but may be consumed by users or external plugins.
         """
-        super().__init__(dataset=dataset, root_dir=root_dir, filepath_arg=filepath_arg)
+        super().__init__(
+            dataset=dataset,
+            root_dir=root_dir,
+            filepath_arg=filepath_arg,
+            metadata=metadata,
+        )
 
         self._azureml_dataset = azureml_dataset
         self._version = version
         # 1 entry for load version, 1 for save version
         self._version_cache = Cache(maxsize=2)  # type: Cache
         self._download = True
         self._local_run = True
@@ -183,18 +191,18 @@
                     f"Did not find version {self.resolve_load_version()} for {self}"
                 )
             fs = AzureMachineLearningFileSystem(azureml_ds.path)
             if azureml_ds.type == "uri_file":
                 # relative (to storage account root) path of the file dataset on azure
                 # Note that path is converted to str for compatibility reasons with
                 # fsspec AbstractFileSystem expand_path function
-                path_on_azure = str(fs._infer_storage_options(azureml_ds.path)[-1])
+                path_on_azure = str(fs._infer_storage_options(azureml_ds.path)[1])
             elif azureml_ds.type == "uri_folder":
                 # relative (to storage account root) path of the folder dataset on azure
-                dataset_root_on_azure = fs._infer_storage_options(azureml_ds.path)[-1]
+                dataset_root_on_azure = fs._infer_storage_options(azureml_ds.path)[1]
                 # relative (to storage account root) path of the dataset in the folder on azure
                 path_on_azure = str(
                     Path(dataset_root_on_azure)
                     / self._dataset_config[self._filepath_arg]
                 )
             else:
                 raise ValueError("Unsupported AzureMLDataset type")
```

### Comparing `kedro_azureml-0.7.0/kedro_azureml/datasets/pipeline_dataset.py` & `kedro_azureml-0.8.0/kedro_azureml/datasets/pipeline_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,37 +56,41 @@
     """
 
     def __init__(
         self,
         dataset: Union[str, Type[AbstractDataset], Dict[str, Any]],
         root_dir: str = "data",
         filepath_arg: str = "filepath",
+        metadata: Dict[str, Any] = None,
     ):
         """Creates a new instance of ``AzureMLPipelineDataset``.
 
         Args:
             dataset: Underlying dataset definition.
                 Accepted formats are:
                 a) object of a class that inherits from ``AbstractDataset``
                 b) a string representing a fully qualified class name to such class
                 c) a dictionary with ``type`` key pointing to a string from b),
                 other keys are passed to the Dataset initializer.
             filepath_arg: Underlying dataset initializer argument that will
                 set the filepath.
                 If unspecified, defaults to "filepath".
+            metadata: Any arbitrary metadata.
+                This is ignored by Kedro, but may be consumed by users or external plugins.
 
         Raises:
             DatasetError: If versioning is enabled for the underlying dataset.
         """
 
         dataset = dataset if isinstance(dataset, dict) else {"type": dataset}
         self._dataset_type, self._dataset_config = parse_dataset_definition(dataset)
 
         self.root_dir = root_dir
         self._filepath_arg = filepath_arg
+        self.metadata = metadata
         try:
             # Convert filepath to relative path
             self._dataset_config[self._filepath_arg] = str(
                 Path(self._dataset_config[self._filepath_arg]).relative_to(Path.cwd())
             )
         except ValueError:
             # If the path is not relative to the current working directory, do not modify it
```

### Comparing `kedro_azureml-0.7.0/kedro_azureml/datasets/runner_dataset.py` & `kedro_azureml-0.8.0/kedro_azureml/datasets/runner_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/distributed/config.py` & `kedro_azureml-0.8.0/kedro_azureml/distributed/config.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/distributed/decorators.py` & `kedro_azureml-0.8.0/kedro_azureml/distributed/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/distributed/utils.py` & `kedro_azureml-0.8.0/kedro_azureml/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/generator.py` & `kedro_azureml-0.8.0/kedro_azureml/generator.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/hooks.py` & `kedro_azureml-0.8.0/kedro_azureml/hooks.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/manager.py` & `kedro_azureml-0.8.0/kedro_azureml/manager.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/runner.py` & `kedro_azureml-0.8.0/kedro_azureml/runner.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/kedro_azureml/utils.py` & `kedro_azureml-0.8.0/kedro_azureml/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.7.0/pyproject.toml` & `kedro_azureml-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kedro-azureml"
-version = "0.7.0"
+version = "0.8.0"
 description = "Kedro plugin with Azure ML Pipelines support"
 readme = "README.md"
 authors = ['marcin.zablocki <marcin.zablocki@getindata.com>']
 maintainers = ['GetInData MLOPS <mlops@getindata.com>']
 homepage = "https://github.com/getindata/kedro-azureml"
 repository = "https://github.com/getindata/kedro-azureml"
 documentation = "https://kedro-azureml.readthedocs.io/"
@@ -28,25 +28,25 @@
     "raise NotImplementedError"
 ]
 
 [tool.isort]
 known_third_party = ["azure", "tabulate", "pydantic","semver","setuptools"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-kedro = ">=0.18.11,<0.19"
+python = ">=3.8,<3.12"
+kedro = ">=0.18.13,<0.19"
 cloudpickle = "^2.1.0"
 adlfs = ">=2022.2.0"
 azure-ai-ml = ">=1.2.0"
 azureml-mlflow = { version = ">=1.42.0", optional = true}
-pydantic = "~=1.9.1"
+pydantic = "~=2.6.4"
 mlflow = {version = ">2.0.0,<3.0.0", optional = true}
 backoff = "^2.2.1"
 kedro-datasets = ">=1.0.0"
-azureml-fsspec = "^1.1.1"
+azureml-fsspec = "~=1.3.1"
 pyarrow = ">=11.0.0"
 
 [tool.poetry.extras]
 mlflow = ["azureml-mlflow", "mlflow"]
 
 [tool.poetry.dev-dependencies]
 pytest = "<7"
```

### Comparing `kedro_azureml-0.7.0/PKG-INFO` & `kedro_azureml-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: kedro-azureml
-Version: 0.7.0
+Version: 0.8.0
 Summary: Kedro plugin with Azure ML Pipelines support
 Home-page: https://github.com/getindata/kedro-azureml
 License: Apache-2.0
 Keywords: kedro,mlops,azureml,machinelearning
 Author: marcin.zablocki
 Author-email: marcin.zablocki@getindata.com
 Maintainer: GetInData MLOPS
 Maintainer-email: mlops@getindata.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mlflow
 Requires-Dist: adlfs (>=2022.2.0)
 Requires-Dist: azure-ai-ml (>=1.2.0)
-Requires-Dist: azureml-fsspec (>=1.1.1,<2.0.0)
+Requires-Dist: azureml-fsspec (>=1.3.1,<1.4.0)
 Requires-Dist: azureml-mlflow (>=1.42.0) ; extra == "mlflow"
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cloudpickle (>=2.1.0,<3.0.0)
-Requires-Dist: kedro (>=0.18.11,<0.19)
+Requires-Dist: kedro (>=0.18.13,<0.19)
 Requires-Dist: kedro-datasets (>=1.0.0)
 Requires-Dist: mlflow (>2.0.0,<3.0.0) ; extra == "mlflow"
 Requires-Dist: pyarrow (>=11.0.0)
-Requires-Dist: pydantic (>=1.9.1,<1.10.0)
+Requires-Dist: pydantic (>=2.6.4,<2.7.0)
 Project-URL: Documentation, https://kedro-azureml.readthedocs.io/
 Project-URL: Repository, https://github.com/getindata/kedro-azureml
 Description-Content-Type: text/markdown
 
 # Kedro Azure ML Pipelines plugin
 
 [![Python Version](https://img.shields.io/pypi/pyversions/kedro-azureml)](https://github.com/getindata/kedro-azureml)
```

#### html2text {}

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1 Name: kedro-azureml Version: 0.7.0 Summary: Kedro plugin
+Metadata-Version: 2.1 Name: kedro-azureml Version: 0.8.0 Summary: Kedro plugin
 with Azure ML Pipelines support Home-page: https://github.com/getindata/kedro-
 azureml License: Apache-2.0 Keywords: kedro,mlops,azureml,machinelearning
 Author: marcin.zablocki Author-email: marcin.zablocki@getindata.com Maintainer:
 GetInData MLOPS Maintainer-email: mlops@getindata.com Requires-Python:
->=3.8,<3.11 Classifier: Development Status :: 4 - Beta Classifier: License ::
+>=3.8,<3.12 Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Provides-Extra: mlflow Requires-Dist: adlfs (>=2022.2.0)
-Requires-Dist: azure-ai-ml (>=1.2.0) Requires-Dist: azureml-fsspec
-(>=1.1.1,<2.0.0) Requires-Dist: azureml-mlflow (>=1.42.0) ; extra == "mlflow"
-Requires-Dist: backoff (>=2.2.1,<3.0.0) Requires-Dist: cloudpickle
-(>=2.1.0,<3.0.0) Requires-Dist: kedro (>=0.18.11,<0.19) Requires-Dist: kedro-
-datasets (>=1.0.0) Requires-Dist: mlflow (>2.0.0,<3.0.0) ; extra == "mlflow"
-Requires-Dist: pyarrow (>=11.0.0) Requires-Dist: pydantic (>=1.9.1,<1.10.0)
-Project-URL: Documentation, https://kedro-azureml.readthedocs.io/ Project-URL:
-Repository, https://github.com/getindata/kedro-azureml Description-Content-
-Type: text/markdown # Kedro Azure ML Pipelines plugin [![Python Version](https:
-//img.shields.io/pypi/pyversions/kedro-azureml)](https://github.com/getindata/
-kedro-azureml) [![License](https://img.shields.io/badge/license-Apache%202.0-
-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![SemVer](https://
-img.shields.io/badge/semver-2.0.0-green)](https://semver.org/) [![PyPI version]
-(https://badge.fury.io/py/kedro-azureml.svg)](https://pypi.org/project/kedro-
-azureml/) [![Downloads](https://pepy.tech/badge/kedro-azureml)](https://
-pepy.tech/project/kedro-azureml) [![Maintainability Rating](https://
-sonarcloud.io/api/project_badges/measure?project=getindata_kedro-
-azureml&metric=sqale_rating)](https://sonarcloud.io/summary/
-new_code?id=getindata_kedro-azureml) [![Coverage](https://sonarcloud.io/api/
-project_badges/measure?project=getindata_kedro-azureml&metric=coverage)](https:
-//sonarcloud.io/summary/new_code?id=getindata_kedro-azureml) [![Documentation
-Status](https://readthedocs.org/projects/kedro-vertexai/badge/?version=latest)]
-(https://kedro-azureml.readthedocs.io/en/latest/?badge=latest)
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
+Extra: mlflow Requires-Dist: adlfs (>=2022.2.0) Requires-Dist: azure-ai-ml
+(>=1.2.0) Requires-Dist: azureml-fsspec (>=1.3.1,<1.4.0) Requires-Dist:
+azureml-mlflow (>=1.42.0) ; extra == "mlflow" Requires-Dist: backoff
+(>=2.2.1,<3.0.0) Requires-Dist: cloudpickle (>=2.1.0,<3.0.0) Requires-Dist:
+kedro (>=0.18.13,<0.19) Requires-Dist: kedro-datasets (>=1.0.0) Requires-Dist:
+mlflow (>2.0.0,<3.0.0) ; extra == "mlflow" Requires-Dist: pyarrow (>=11.0.0)
+Requires-Dist: pydantic (>=2.6.4,<2.7.0) Project-URL: Documentation, https://
+kedro-azureml.readthedocs.io/ Project-URL: Repository, https://github.com/
+getindata/kedro-azureml Description-Content-Type: text/markdown # Kedro Azure
+ML Pipelines plugin [![Python Version](https://img.shields.io/pypi/pyversions/
+kedro-azureml)](https://github.com/getindata/kedro-azureml) [![License](https:/
+/img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/
+licenses/Apache-2.0) [![SemVer](https://img.shields.io/badge/semver-2.0.0-
+green)](https://semver.org/) [![PyPI version](https://badge.fury.io/py/kedro-
+azureml.svg)](https://pypi.org/project/kedro-azureml/) [![Downloads](https://
+pepy.tech/badge/kedro-azureml)](https://pepy.tech/project/kedro-azureml) [!
+[Maintainability Rating](https://sonarcloud.io/api/project_badges/
+measure?project=getindata_kedro-azureml&metric=sqale_rating)](https://
+sonarcloud.io/summary/new_code?id=getindata_kedro-azureml) [![Coverage](https:/
+/sonarcloud.io/api/project_badges/measure?project=getindata_kedro-
+azureml&metric=coverage)](https://sonarcloud.io/summary/
+new_code?id=getindata_kedro-azureml) [![Documentation Status](https://
+readthedocs.org/projects/kedro-vertexai/badge/?version=latest)](https://kedro-
+azureml.readthedocs.io/en/latest/?badge=latest)
                      _[_h_t_t_p_s_:_/_/_g_e_t_i_n_d_a_t_a_._c_o_m_/_i_m_g_/_l_o_g_o_._s_v_g_]
             ******** WWee hheellpp ccoommppaanniieess ttuurrnn tthheeiirr ddaattaa iinnttoo aasssseettss ********
 ## About Following plugin enables running Kedro pipelines on Azure ML Pipelines
 service. We support 2 native Azure Machine Learning types of workflows: * For
 Data Scientists: fast, iterative development with code upload * For MLOps:
 stable, repeatable workflows with Docker ## Documentation For detailed
 documentation refer to https://kedro-azureml.readthedocs.io/ ## Usage guide ```
```


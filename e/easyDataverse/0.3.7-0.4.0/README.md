# Comparing `tmp/easyDataverse-0.3.7.tar.gz` & `tmp/easydataverse-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyDataverse-0.3.7.tar", last modified: Tue Oct 18 13:20:38 2022, max compression
+gzip compressed data, was "easydataverse-0.4.0.tar", max compression
```

## Comparing `easyDataverse-0.3.7.tar` & `easydataverse-0.4.0.tar`

### file list

```diff
@@ -1,62 +1,13 @@
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.285271 easyDataverse-0.3.7/
--rw-r--r--   0 jara1991   (501) staff       (20)     1066 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/LICENSE
--rw-r--r--   0 jara1991   (501) staff       (20)       39 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/MANIFEST.in
--rw-r--r--   0 jara1991   (501) staff       (20)      188 2022-10-18 13:20:38.285133 easyDataverse-0.3.7/PKG-INFO
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.278262 easyDataverse-0.3.7/easyDataverse/
--rw-r--r--   0 jara1991   (501) staff       (20)      114 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/__init__.py
--rw-r--r--   0 jara1991   (501) staff       (20)     3026 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/cli.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.279978 easyDataverse-0.3.7/easyDataverse/core/
--rw-r--r--   0 jara1991   (501) staff       (20)       84 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/core/__init__.py
--rw-r--r--   0 jara1991   (501) staff       (20)     4708 2022-09-20 22:58:00.000000 easyDataverse-0.3.7/easyDataverse/core/base.py
--rw-r--r--   0 jara1991   (501) staff       (20)    23125 2022-10-18 10:26:35.000000 easyDataverse-0.3.7/easyDataverse/core/dataset.py
--rw-r--r--   0 jara1991   (501) staff       (20)     1557 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/core/exceptions.py
--rw-r--r--   0 jara1991   (501) staff       (20)      473 2022-10-10 10:27:45.000000 easyDataverse-0.3.7/easyDataverse/core/file.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.280447 easyDataverse-0.3.7/easyDataverse/tools/
--rw-r--r--   0 jara1991   (501) staff       (20)       83 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/__init__.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.281622 easyDataverse-0.3.7/easyDataverse/tools/codegen/
--rw-r--r--   0 jara1991   (501) staff       (20)       43 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/codegen/__init__.py
--rw-r--r--   0 jara1991   (501) staff       (20)     5959 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/codegen/clsmod.py
--rw-r--r--   0 jara1991   (501) staff       (20)     3210 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/codegen/filehandling.py
--rw-r--r--   0 jara1991   (501) staff       (20)     5392 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/codegen/generator.py
--rw-r--r--   0 jara1991   (501) staff       (20)     2025 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/codegen/restmod.py
--rw-r--r--   0 jara1991   (501) staff       (20)     5803 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/codegen/schema.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.281761 easyDataverse-0.3.7/easyDataverse/tools/codegen/templates/
--rw-r--r--   0 jara1991   (501) staff       (20)        0 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/codegen/templates/__init__.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.282490 easyDataverse-0.3.7/easyDataverse/tools/downloader/
--rw-r--r--   0 jara1991   (501) staff       (20)        0 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/downloader/__init__.py
--rw-r--r--   0 jara1991   (501) staff       (20)     4313 2022-10-18 11:24:13.000000 easyDataverse-0.3.7/easyDataverse/tools/downloader/downloader.py
--rw-r--r--   0 jara1991   (501) staff       (20)     3865 2022-10-18 11:27:37.000000 easyDataverse-0.3.7/easyDataverse/tools/downloader/libutils.py
--rw-r--r--   0 jara1991   (501) staff       (20)     9940 2022-10-18 11:24:10.000000 easyDataverse-0.3.7/easyDataverse/tools/downloader/nolibutils.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.283219 easyDataverse-0.3.7/easyDataverse/tools/software/
--rw-r--r--   0 jara1991   (501) staff       (20)       46 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/software/__init__.py
--rw-r--r--   0 jara1991   (501) staff       (20)     3934 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/software/pythonparser.py
--rw-r--r--   0 jara1991   (501) staff       (20)      700 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/software/softwareinfo.py
--rw-r--r--   0 jara1991   (501) staff       (20)     2052 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/software/softwaretools.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.283544 easyDataverse-0.3.7/easyDataverse/tools/uploader/
--rw-r--r--   0 jara1991   (501) staff       (20)        0 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/uploader/__init__.py
--rw-r--r--   0 jara1991   (501) staff       (20)     7537 2022-10-10 12:51:16.000000 easyDataverse-0.3.7/easyDataverse/tools/uploader/uploader.py
--rw-r--r--   0 jara1991   (501) staff       (20)        0 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/uploader/utils.py
--rw-r--r--   0 jara1991   (501) staff       (20)      769 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/utils.py
--rw-r--r--   0 jara1991   (501) staff       (20)     2811 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/easyDataverse/tools/xmltools.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.279101 easyDataverse-0.3.7/easyDataverse.egg-info/
--rw-r--r--   0 jara1991   (501) staff       (20)      188 2022-10-18 13:20:38.000000 easyDataverse-0.3.7/easyDataverse.egg-info/PKG-INFO
--rw-r--r--   0 jara1991   (501) staff       (20)     1561 2022-10-18 13:20:38.000000 easyDataverse-0.3.7/easyDataverse.egg-info/SOURCES.txt
--rw-r--r--   0 jara1991   (501) staff       (20)        1 2022-10-18 13:20:38.000000 easyDataverse-0.3.7/easyDataverse.egg-info/dependency_links.txt
--rw-r--r--   0 jara1991   (501) staff       (20)       53 2022-10-18 13:20:38.000000 easyDataverse-0.3.7/easyDataverse.egg-info/entry_points.txt
--rw-r--r--   0 jara1991   (501) staff       (20)      152 2022-10-18 13:20:38.000000 easyDataverse-0.3.7/easyDataverse.egg-info/requires.txt
--rw-r--r--   0 jara1991   (501) staff       (20)       20 2022-10-18 13:20:38.000000 easyDataverse-0.3.7/easyDataverse.egg-info/top_level.txt
--rw-r--r--   0 jara1991   (501) staff       (20)       38 2022-10-18 13:20:38.285314 easyDataverse-0.3.7/setup.cfg
--rw-r--r--   0 jara1991   (501) staff       (20)      736 2022-10-18 13:15:50.000000 easyDataverse-0.3.7/setup.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.283716 easyDataverse-0.3.7/tests/
--rw-r--r--   0 jara1991   (501) staff       (20)        0 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/tests/__init__.py
--rw-r--r--   0 jara1991   (501) staff       (20)     1494 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/tests/conftest.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.284323 easyDataverse-0.3.7/tests/core/
--rw-r--r--   0 jara1991   (501) staff       (20)        0 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/tests/core/__init__.py
--rw-r--r--   0 jara1991   (501) staff       (20)    12549 2022-10-10 10:35:22.000000 easyDataverse-0.3.7/tests/core/test_dataset.py
--rw-r--r--   0 jara1991   (501) staff       (20)     1988 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/tests/core/test_dataverse_base.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.284458 easyDataverse-0.3.7/tests/fixtures/
--rw-r--r--   0 jara1991   (501) staff       (20)        0 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/tests/fixtures/__init__.py
-drwxr-xr-x   0 jara1991   (501) staff       (20)        0 2022-10-18 13:20:38.284894 easyDataverse-0.3.7/tests/fixtures/dataset/
--rw-r--r--   0 jara1991   (501) staff       (20)        0 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/tests/fixtures/dataset/__init__.py
--rw-r--r--   0 jara1991   (501) staff       (20)     1130 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/tests/fixtures/dataset/invalidclass.py
--rw-r--r--   0 jara1991   (501) staff       (20)     1150 2022-08-22 13:15:30.000000 easyDataverse-0.3.7/tests/fixtures/dataset/toydataset.py
+-rw-r--r--   0        0        0     1066 2024-05-09 20:41:59.766842 easydataverse-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3771 2024-05-09 20:41:59.766842 easydataverse-0.4.0/Readme.md
+-rw-r--r--   0        0        0      155 2024-05-09 20:41:59.766842 easydataverse-0.4.0/easyDataverse/__init__.py
+-rw-r--r--   0        0        0    13437 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/base.py
+-rw-r--r--   0        0        0    11339 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/classgen.py
+-rw-r--r--   0        0        0     1867 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/connect.py
+-rw-r--r--   0        0        0    12760 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/dataset.py
+-rw-r--r--   0        0        0    18696 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/dataverse.py
+-rw-r--r--   0        0        0     5958 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/downloader.py
+-rw-r--r--   0        0        0     4402 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/uploader.py
+-rw-r--r--   0        0        0      174 2024-05-09 20:41:59.770842 easydataverse-0.4.0/easyDataverse/utils.py
+-rw-r--r--   0        0        0      867 2024-05-09 20:41:59.770842 easydataverse-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5027 1970-01-01 00:00:00.000000 easydataverse-0.4.0/PKG-INFO
```

### Comparing `easyDataverse-0.3.7/LICENSE` & `easydataverse-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyDataverse-0.3.7/easyDataverse/tools/downloader/nolibutils.py` & `easydataverse-0.4.0/easyDataverse/classgen.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,316 +1,447 @@
-import copy
+from datetime import date
 import forge
+import types
 import re
-import requests
 
-from pyDataverse.api import NativeApi
-from pydantic import Field, create_model
-from typing import Optional, List, Dict, List
-
-from easyDataverse.core.base import DataverseBase
-
-
-class Types:
-    """Enumeration used to infer type annotations for PyDantic"""
-
-    STR = str
-    FLOAT = float
-    INT = int
-
-    LIST_STR = List[str]
-    LIST_FLOAT = List[float]
-    LIST_INT = List[int]
-
-    OPTIONAL_STR = Optional[str]
-    OPTIONAL_FLOAT = Optional[float]
-    OPTIONAL_INT = Optional[int]
-
-    @classmethod
-    def get_mixed_type(
-        cls, dtype: str, multiple: bool = False, required: bool = False, pre: str = ""
-    ):
-        STRING_TYPES = ["text", "textbox", "url", "date"]
-        FLOAT_TYPES = ["float"]
-        INTEGER_TYPES = ["integer"]
-
-        if not required:
-            pre = "OPTIONAL_"
-        if multiple:
-            pre = "LIST_"
-
-        if dtype.lower() in STRING_TYPES:
-            return cls.__dict__[f"{pre}STR"]
-        elif dtype.lower() in FLOAT_TYPES:
-            return cls.__dict__[f"{pre}FLOAT"]
-        elif dtype.lower() in INTEGER_TYPES:
-            return cls.__dict__[f"{pre}INT"]
-        else:
-            return cls.__dict__[f"{pre}STR"]
+from enum import Enum
+from pydantic import AnyHttpUrl, EmailStr, create_model, Field
+from pydantic.fields import FieldInfo
+from typing import List, Tuple, Union, Type, Optional, Dict, Callable
+
+from easyDataverse.base import DataverseBase
+
+TYPE_MAPPING = {
+    "text": str,
+    "url": AnyHttpUrl,
+    "float": float,
+    "integer": int,
+    "int": int,
+    "textbox": str,
+    "date": date,
+    "email": EmailStr,
+}
+
+
+def create_dataverse_class(
+    name: str,
+    primitives: List[Dict],
+    compounds: Optional[List] = None,
+    common_part="",
+) -> Callable:
+    """Parses the parameters given by a dataverse metadatablock definition
+    and dynamically creates a class that can be used to report data
+    to a dataset.
+
+    Args:
+        name (str): Name of the metadatablock/field
+        primitives (List[Dict]): List of primitive fields to parse.
+        compounds (List, optional): List of compound fields to parse. Defaults to None.
+
+    Returns:
+        Callable: DataverseBase class that can be used within the Dataset/DataverseBase class
+    """
 
+    if compounds is None:
+        compounds = []
 
-# ! STEP 1 UTILS: Fetching of the raw Dataverse JSON data
-def fetch_dataset(p_id: str, dataverse_url: str, api_token: Optional[str] = None):
-    """Fetches a dataset from a given Dataverse installation and persistent identifier.
+    cls_name = construct_class_name(name)
+
+    # Cosmetics :-P
+    common_part = find_common_name_part(
+        [camel_to_snake(field["name"]) for field in primitives]
+        + [camel_to_snake(field["name"]) for field in compounds]
+    )
+
+    # Get all primitive attributes
+    attributes = {
+        process_name(field["name"], common_part): (
+            get_field_type(field),
+            prepare_field_meta(field),
+        )
+        for field in primitives
+    }
+
+    # Get all compounds and collect add function
+    add_functions = {}
+    attributes.update(
+        {
+            process_name(compound["name"], common_part): create_compound(
+                compound, add_functions, common_part
+            )
+            for compound in compounds
+        }
+    )
+
+    # Create the class and add utilities
+    dv_class = create_model(
+        cls_name,
+        __base__=(DataverseBase,),
+        **attributes,
+    )
+
+    for name, fun in add_functions.items():
+        setattr(dv_class, name, fun)
+
+    return dv_class
+
+
+def create_compound(
+    compound: Dict,
+    add_functions: Dict,
+    common_part: str = "",
+) -> Tuple[Callable, FieldInfo]:
+    """Takes a compound definition, creates a corresponding data type and an add_function
 
     Args:
-        p_id (str): Persistent Identifier of the dataset
-        dataverse_url (str): URL to the dataverse installation to fetch the dataset from.
+        compound (Dict): Dictionary containing the compound configuration
+        add_functions (Dict): Add function registry which will be added to the parent class.
+        common_part (str, optional): Common part of the compound name. Defaults to "".
 
     Returns:
-        Dict: Dataverse JSON as a dictionary representation
+        Tuple[Callable, FieldInfo]: Class as a type and Field meta for PyDantic
     """
-    if dataverse_url.endswith("/"):
-        dataverse_url = dataverse_url[0:-1]
 
-    if api_token:
-        api = NativeApi(dataverse_url, api_token)
+    # Get all the names
+    attribute_name = process_name(
+        compound["name"],
+        common_part,
+    )
+
+    sub_cls = create_dataverse_class(
+        compound["title"],
+        compound["childFields"].values(),
+    )
+
+    if compound["multiple"] is True:
+        dtype = list_type(sub_cls)
+    else:
+        dtype = optional_type(sub_cls)
+
+    field_meta = prepare_field_meta(compound)
+
+    if compound["multiple"] is False:
+        # Set non-multiple compounds directly as default
+        field_meta.default = None
+        field_meta.default_factory = sub_cls
+
+    # Create add function
+    fun_name = f"add_{attribute_name}"
+    add_functions[fun_name] = generate_add_function(sub_cls, attribute_name, fun_name)
+
+    return (dtype, field_meta)
+
+
+def get_field_type(field: Dict) -> Type:
+    """Retrieves the type hint of a field
+
+    Args:
+        field (Dict): The field dictionary containing information about the field
+
+    Returns:
+        Type: The type hint of the field
+
+    """
+    if field["isControlledVocabulary"]:
+        dtype = Enum(
+            field["name"],
+            {
+                spaced_to_snake(value).upper(): value
+                for value in field["controlledVocabularyValues"]
+            },
+        )
     else:
-        api = NativeApi(dataverse_url)
+        dtype = TYPE_MAPPING[field["type"].lower()]
 
-    # Download the dataset and retrieve the field data
-    return api.get_dataset(p_id).json()
+    if field["multiple"]:
+        return list_type(dtype)
+    else:
+        return optional_type(dtype)
 
 
-# ! STEP 2 UTILS: Creation of an on-the-fly object model
-def create_block_definitions(block_name, block, dataverse_url):
-    """Generates an object model based on the definition of a block.
+def prepare_field_meta(field: Dict) -> FieldInfo:
+    """
+    Extracts metadata from the field definition to compose a PyDantic Field instance.
 
     Args:
-        block_name (str): Internal name of the metadatablock. This is not always the display name.
-        block (Dict): Metadatablock definition from the Dataverse JSON dataset.
-        dataverse_url (str): URL to the dataverse installation to fetch the block definition.
+        field (Dict): The field definition.
 
     Returns:
-        DataverseBase: Empty object representation of the metadatablock.
+        FieldInfo: The PyDantic Field instance.
     """
-    # Get a lookup from the metadata config of the target DV
-    lookup = _fetch_lookup(dataverse_url, block_name)
 
-    # Initialize both definitions and add function dicts
-    cls_def = {}
-    add_funs = {}
+    is_multiple = field["multiple"]
 
-    # Turn raw definitions into classes
-    for field in block["fields"]:
-        _process_field(field, lookup, cls_def, add_funs)
+    if field["type"].lower() == "none":
+        type_class = "compound"
+    elif field["isControlledVocabulary"]:
+        type_class = "controlledVocabulary"
+    else:
+        type_class = "primitive"
+
+    field_parameters = {
+        "alias": field["name"],
+        "description": field["description"],
+    }
 
-    # Now, create the class
-    block_cls = create_model(
-        block_name.capitalize(), __base__=(DataverseBase,), **cls_def
-    )()
+    json_schema_extra = {
+        "multiple": is_multiple,
+        "typeClass": type_class,
+        "typeName": field["name"],
+    }
 
-    # Add metadatablock_name
-    block_cls.__dict__["_metadatablock_name"] = block_name
+    if is_multiple:
+        field_parameters["default_factory"] = list
+    else:
+        field_parameters["default"] = None
 
-    # TODO: Fix recursion problem with add_funs
-    # Finally, add all add-functions
-    # for name, function in add_funs.items():
-    #    function = types.MethodType( function, block_cls )
-    #    block_cls.__dict__[name] = function
-    #    break
+    return Field(
+        **field_parameters,
+        json_schema_extra=json_schema_extra,
+    )
 
-    return block_cls
 
+def generate_add_function(subclass, attribute, name):
+    """Generates an add function for a subclass.
 
-def _fetch_lookup(dataverse_url: str, block_name: str):
-    """Fetches the metadatablock definition from the Dataverse API
+    Args:
+        subclass (class): The subclass to be added.
+        attribute (str): The attribute name to append the subclass instance to.
+        name (str): The name of the generated add function.
 
-    This resulting definition is used to infer the correct names for
-    the resulting fields. All other metadata for the fields such as
-    'typeClass' etc. are drawn from the datasets Dataverse JSON.
+    Returns:
+        function: The generated add function.
     """
-    url = f"{dataverse_url}/api/metadatablocks/{block_name}"
-    response = requests.get(url)
-    block_data = response.json()["data"]
-    return block_data["fields"]
 
+    def add_fun_template(self, **kwargs):
+        getattr(self, attribute).append(subclass(**kwargs))
 
-def _process_field(field, lookup, cls_def, add_funs):
-    """Processes a field according to its 'typeClass'."""
+    signature = create_function_signature(subclass)
+    new_func = forge.sign(forge.self, *signature)(
+        types.FunctionType(
+            add_fun_template.__code__,
+            add_fun_template.__globals__,
+            name,
+            add_fun_template.__defaults__,
+            add_fun_template.__closure__,
+        )
+    )
 
-    PROCESS_MAPPING = {
-        "primitive": _process_primitive,
-        "controlledVocabulary": _process_primitive,
-        "compound": _process_compound,
-    }
+    new_func.__annotations__ = dict(subclass.__annotations__)
+    new_func.__doc__ = str(forge.repr_callable(new_func))
 
-    fun = PROCESS_MAPPING[field["typeClass"]]
-    fun(field, lookup, cls_def, add_funs)
+    return new_func
 
 
-def _process_compound(field, lookup, cls_def, add_funs):
-    """Processes a compound field and creates a new class from it."""
+def create_function_signature(subclass) -> List:
+    """
+    Forges a signature for an add function
 
-    _, description, cls = _create_compound_class(field, lookup)
+    Args:
+        subclass: The subclass for which the signature is being forged
+
+    Returns:
+        signature: The forged signature as a list of keyword arguments
+    """
+    signature = []
+    for name, dtype in subclass.__annotations__.items():
+        sig_params = {"name": name, "type": dtype, "interface_name": name}
 
-    field_meta = copy.deepcopy(field)
-    field_meta["description"] = description
-    field_meta.pop("value")
+        default = subclass.model_fields[name].default
 
-    if field["multiple"]:
-        dtype = List[cls]
-        field_meta["default_factory"] = list
-    else:
-        dtype = Optional[cls]
-        field_meta["default"] = None
+        if default is None:
+            sig_params["default"] = None
+
+        signature.append(forge.kwarg(**sig_params))
+
+    return signature
+
+
+def clean_name(name):
+    """
+    Removes anything that is not a valid variable name.
 
-    field_name = lookup[field["typeName"]]["title"]
-    field_name = "".join([name.capitalize() for name in field_name.split(" ")])
-    field_name = _camel_to_snake(field_name)
+    Parameters:
+        name (str): The name to be cleaned.
 
-    # Generate add method
-    add_funs[f"add_{field_name}"] = _generate_add_method(cls, field_name)
+    Returns:
+        str: The cleaned name.
+    """
+    return re.sub(r"[^\w\s_]", " ", name).strip()
 
-    cls_def[field_name] = (dtype, Field(**field_meta))
 
+def camel_to_snake(name):
+    """
+    Converts a camel case string to snake case.
 
-def _process_primitive(field, lookup, cls_def, add_funs):
-    """Processes a primitive field and adds it to the metadatablock class definition"""
+    Args:
+        name (str): The camel case string to be converted.
 
-    name, primitive = _parse_primitive(field, lookup)
-    cls_def[name] = primitive
+    Returns:
+        str: The snake case representation of the input string.
+    """
 
+    name = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", clean_name(name))
+    return re.sub("([a-z0-9])([A-Z])", r"\1_\2", name).lower()
 
-def _create_compound_class(field, lookup):
-    """Creates a compound class based on the primitives that it is made up from."""
 
-    # Get metadata from lookup
-    field_meta = lookup[field["typeName"]]
-    name = field_meta["title"]
-    cls_name = _snake_to_camel(name.replace(" ", "_"))
-    description = field_meta["description"]
+def spaced_to_snake(name: str) -> str:
+    """Turns names that contain a space into snake case
 
-    # Get all fields
-    fields = _parse_compound_fields(field["value"], lookup)
+    Args:
+        name (str): The name to be converted to snake case.
 
-    # Create the resulting class
-    cls = create_model(cls_name, __base__=(DataverseBase,), **fields)
+    Returns:
+        str: The name converted to snake case.
 
-    cls.__name__ = cls_name
+    """
+    name = clean_name(name).strip("_").strip()
 
-    # Create a new type from this
-    return name, description, cls
+    if name == "":
+        raise ValueError(f"Class name cannot be empty. Got '{name}'")
 
+    return "_".join([word.lower() for word in name.replace("-", " ").split(" ")])
 
-def _parse_compound_fields(data: List, lookup):
-    """Parses primitive fields found in a compound definition."""
 
-    parsed_fields = {}
+def construct_class_name(name: str) -> str:
+    """Converts a display name to a class name.
 
-    for member in data:
-        for primitive in member.values():
-            name, field = _parse_primitive(primitive, lookup)
-            parsed_fields[name] = field
+    Args:
+        name (str): The display name to be converted.
 
-    return parsed_fields
+    Returns:
+        str: The converted class name.
 
+    Raises:
+        ValueError: If the name is empty.
 
-def _parse_primitive(data: Dict, lookup: Dict):
-    """Parses a primitive field. Returns name and field definition"""
+    """
+    name = spaced_to_snake(name)
 
-    data = copy.deepcopy(data)
-    data.pop("value")
+    if name == "":
+        raise ValueError(f"Class name cannot be empty. Got '{name}'")
 
-    # Get metadata from lookup
-    name = _camel_to_snake(lookup[data["typeName"]]["title"])
-    name = "".join([n.capitalize() for n in name.split(" ")])
-    name = _camel_to_snake(name)
+    return "".join([part.capitalize() for part in name.split("_")])
 
-    data["description"] = lookup[data["typeName"]]["description"]
 
-    return name, _create_primitive_field(lookup=lookup, **data)
+def list_type(dtype: Type):
+    """Encapsulates given types within a List typing
 
+    Args:
+        dtype (Type): The type to be encapsulated
 
-def _create_primitive_field(lookup: Dict, **kwargs):
-    """Creates a primtive PyDantic field used to assign to a class."""
+    Returns:
+        List[dtype]: The encapsulated type as a List
 
-    # Get type from lookup
-    field_def = lookup[kwargs["typeName"]]
-    dtype = field_def["type"]
-    dtype = Types.get_mixed_type(dtype=dtype, multiple=kwargs["multiple"])
+    """
+    return List[dtype]
 
-    if kwargs["multiple"]:
-        kwargs["default_factory"] = list
-    else:
-        kwargs["default"] = None
 
-    return (dtype, Field(**kwargs))
+def optional_type(dtype: Type):
+    """Encapsulates given types within an Optional typing
 
+    Args:
+        dtype (Type): The type to be encapsulated
 
-def _generate_add_method(target_cls, field):
-    """Generates an add method that later on can be added to a target class to facilitate compound addition."""
-    add_fun = copy.deepcopy(_generic_add_function)
-    add_fun.__name__ = f"add_{field}"
+    Returns:
+        Optional[Type]: The encapsulated type wrapped in Optional
 
-    return forge.sign(
-        forge.self,
-        *[
-            forge.kwarg(name, type=dtype, default=forge.empty)
-            for name, dtype in target_cls.__annotations__.items()
-        ],
-        forge.kwarg("_target_cls", default=target_cls, bound=True),
-        forge.kwarg("_field", default=field, bound=True),
-    )(add_fun)
+    """
+    return Optional[dtype]
 
 
-def _generic_add_function(self, **kwargs):
-    """This is a generic function used as a template for add-funs"""
-    target_cls = kwargs["_target_cls"]
-    field = kwargs["_field"]
-    kwargs.pop("_target_cls")
-    kwargs.pop("_field")
+def union_type(dtypes: Tuple):
+    """Encapsulates given types within a Union typing
 
-    self.__dict__[field].append(target_cls(**kwargs))
+    Args:
+        dtypes (Tuple): A tuple of types to be encapsulated within a Union typing
 
+    Raises:
+        ValueError: If only a single type is provided
 
-def _camel_to_snake(name):
-    """Turns 'CamelCase' to 'camel_case'"""
-    name = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
-    return re.sub("([a-z0-9])([A-Z])", r"\1_\2", name).lower()
+    Returns:
+        Union: A Union typing encapsulating the given types
+    """
+
+    if not isinstance(dtypes, tuple):
+        raise TypeError(f"Expected a tuple of types, got {type(dtypes)}")
 
+    if len(dtypes) < 2:
+        raise ValueError("Union type requires more than a single type")
 
-def _snake_to_camel(name):
-    """Turns 'snake_case' to 'SnakeCase'"""
-    return "".join(x.capitalize() or "_" for x in name.split("_"))
+    return Union[dtypes]  # type: ignore
 
 
-# ! STEP 3 UTILS: Assignment of the values to the generated data model
-def populate_block_values(block_cls: DataverseBase, block_json: Dict):
-    """Parses the given Dataverse JSON and assigns all values to the generated metadatablock object model.
+def remove_child_fields_from_global(fields: Dict) -> Dict:
+    """
+    Removes fields that belong to a compound from the global scope.
 
     Args:
-        block_cls (DataverseBase): Object representation of the block.
-        block_json (Dict): JSON representation of the dataset's metadatablock.
+        fields (Dict): A dictionary containing the fields.
+
+    Returns:
+        Dict: The updated dictionary with the removed fields.
     """
 
-    for field in block_json:
-        field_type = field["typeClass"]
-        attr_name = _find_attribute(block_cls, field["typeName"])
+    compounds = list(filter(lambda field: "childFields" in field, fields.values()))
+    for compound in compounds:
+        for child_name in compound["childFields"].keys():
+            if child_name in fields:
+                fields.pop(child_name)
+
+    return fields
 
-        if field_type == "compound":
 
-            for entry in field["value"]:
-                sub_class = _get_sub_class(block_cls, attr_name)
-                kwargs = {
-                    _find_attribute(sub_class, name): compound["value"]
-                    for name, compound in entry.items()
-                }
+def process_name(attr_name, common_part):
+    """
+    Process the attribute name by converting it from camel case to snake case and removing the common part.
 
-                block_cls.__dict__[attr_name].append(sub_class(**kwargs))
+    Args:
+        attr_name (str): The attribute name to be processed.
+        common_part (str): The common part to be removed from the attribute name.
 
-        else:
-            block_cls.__dict__[attr_name] = field["value"]
+    Returns:
+        str: The processed attribute name.
+    """
+    return camel_to_snake(attr_name).replace(common_part, "", 1).replace(" ", "")
 
 
-def _find_attribute(block, typeName):
-    """Finds the corresponding attribute name of the Dataverse field"""
-    for name, field in block.__fields__.items():
-        if typeName == field.field_info.extra["typeName"]:
-            return name
+def find_common_name_part(names: List[str]):
+    """
+    Finds a common name part to remove this across primitives and compounds
 
-    raise AttributeError(f"Cant locate attribute with 'typeName = {typeName}'.")
+    Args:
+        names (List[str]): A list of names to find the common part from.
+
+    Returns:
+        str: The common name part found.
+
+    Raises:
+        None
+
+    Examples:
+        >>> names = ["apple", "banana", "apricot"]
+        >>> find_common_name_part(names)
+        'a_'
+    """
+
+    if len(names) <= 1:
+        return ""
+
+    diff = False
+    common_start = []
+
+    while diff is False:
+        try:
+            current_char_set = {name.split("_")[len(common_start)] for name in names}
+        except IndexError:
+            return "_".join(common_start) + "_"
+
+        if len(current_char_set) == 1:
+            common_start += list(current_char_set)
+        else:
+            diff = True
 
+    if len(common_start) == 0:
+        return ""
 
-def _get_sub_class(block, field_name):
-    """Returns the sub class of a compound field in order to add data."""
-    return block.__fields__[field_name].type_
+    return "_".join(common_start) + "_"
```


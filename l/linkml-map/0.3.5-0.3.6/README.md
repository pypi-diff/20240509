# Comparing `tmp/linkml_map-0.3.5.tar.gz` & `tmp/linkml_map-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_map-0.3.5.tar", max compression
+gzip compressed data, was "linkml_map-0.3.6.tar", max compression
```

## Comparing `linkml_map-0.3.5.tar` & `linkml_map-0.3.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1474 2024-05-02 03:03:24.839000 linkml_map-0.3.5/README.md
--rw-r--r--   0        0        0     1516 2024-05-02 03:03:56.466852 linkml_map-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      127 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/cli/__init__.py
--rw-r--r--   0        0        0     6182 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/cli/cli.py
--rw-r--r--   0        0        0       61 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/__init__.py
--rw-r--r--   0        0        0      447 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/awk_compiler.py
--rw-r--r--   0        0        0     2793 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/compiler.py
--rw-r--r--   0        0        0     3853 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/graphviz_compiler.py
--rw-r--r--   0        0        0     1266 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/j2_based_compiler.py
--rw-r--r--   0        0        0      268 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/markdown_compiler.py
--rw-r--r--   0        0        0     3523 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/python_compiler.py
--rw-r--r--   0        0        0      383 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/r2rml_compiler.py
--rw-r--r--   0        0        0      395 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/sparql_compiler.py
--rw-r--r--   0        0        0     4410 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/sql_compiler.py
--rw-r--r--   0        0        0      460 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/sssom_compiler.py
--rw-r--r--   0        0        0       63 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/templates/__init__.py
--rw-r--r--   0        0        0      717 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/templates/markdown.j2
--rw-r--r--   0        0        0      173 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/tr/__init__.py
--rw-r--r--   0        0        0      756 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/compiler/tr/transformer_to_mapping_tables.tr.yaml
--rw-r--r--   0        0        0      111 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/datamodel/__init__.py
--rw-r--r--   0        0        0      161 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/datamodel/sssom.map.yaml
--rw-r--r--   0        0        0    18689 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/datamodel/transformer_model.py
--rw-r--r--   0        0        0    10658 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/datamodel/transformer_model.yaml
--rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/functions/__init__.py
--rw-r--r--   0        0        0     4448 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/functions/unit_conversion.py
--rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/importer/__init__.py
--rw-r--r--   0        0        0      866 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/importer/importer.py
--rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/inference/__init__.py
--rw-r--r--   0        0        0     1565 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/inference/inference.py
--rw-r--r--   0        0        0     7414 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/inference/inverter.py
--rw-r--r--   0        0        0    10117 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/inference/schema_mapper.py
--rw-r--r--   0        0        0     6602 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/session.py
--rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/transformer/__init__.py
--rw-r--r--   0        0        0     2226 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/transformer/duckdb_transformer.py
--rw-r--r--   0        0        0    16600 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/transformer/object_transformer.py
--rw-r--r--   0        0        0     9812 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/transformer/transformer.py
--rw-r--r--   0        0        0        0 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/__init__.py
--rw-r--r--   0        0        0     1306 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/dynamic_object.py
--rw-r--r--   0        0        0     6824 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/eval_utils.py
--rw-r--r--   0        0        0      767 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/loaders.py
--rw-r--r--   0        0        0     9496 2024-05-02 03:03:24.843000 linkml_map-0.3.5/src/linkml_map/utils/multi_file_transformer.py
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 linkml_map-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1474 2024-05-08 23:06:17.118384 linkml_map-0.3.6/README.md
+-rw-r--r--   0        0        0     1516 2024-05-08 23:06:45.126567 linkml_map-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      127 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/cli/__init__.py
+-rw-r--r--   0        0        0     6182 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/cli/cli.py
+-rw-r--r--   0        0        0       61 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/__init__.py
+-rw-r--r--   0        0        0      447 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/awk_compiler.py
+-rw-r--r--   0        0        0     2793 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/compiler.py
+-rw-r--r--   0        0        0     3853 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/graphviz_compiler.py
+-rw-r--r--   0        0        0     1266 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/j2_based_compiler.py
+-rw-r--r--   0        0        0      268 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/markdown_compiler.py
+-rw-r--r--   0        0        0     3523 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/python_compiler.py
+-rw-r--r--   0        0        0      383 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/r2rml_compiler.py
+-rw-r--r--   0        0        0      395 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/sparql_compiler.py
+-rw-r--r--   0        0        0     4410 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/sql_compiler.py
+-rw-r--r--   0        0        0      460 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/sssom_compiler.py
+-rw-r--r--   0        0        0       63 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/templates/__init__.py
+-rw-r--r--   0        0        0      717 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/templates/markdown.j2
+-rw-r--r--   0        0        0      173 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/tr/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/compiler/tr/transformer_to_mapping_tables.tr.yaml
+-rw-r--r--   0        0        0      111 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/datamodel/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/datamodel/sssom.map.yaml
+-rw-r--r--   0        0        0    18689 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/datamodel/transformer_model.py
+-rw-r--r--   0        0        0    10658 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/datamodel/transformer_model.yaml
+-rw-r--r--   0        0        0        0 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/functions/__init__.py
+-rw-r--r--   0        0        0     4448 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/functions/unit_conversion.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/importer/__init__.py
+-rw-r--r--   0        0        0      866 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/importer/importer.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/inference/__init__.py
+-rw-r--r--   0        0        0     1565 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/inference/inference.py
+-rw-r--r--   0        0        0     7414 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/inference/inverter.py
+-rw-r--r--   0        0        0    10117 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/inference/schema_mapper.py
+-rw-r--r--   0        0        0     6602 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/session.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/transformer/__init__.py
+-rw-r--r--   0        0        0     2226 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/transformer/duckdb_transformer.py
+-rw-r--r--   0        0        0    19674 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/transformer/object_transformer.py
+-rw-r--r--   0        0        0     9812 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/transformer/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/utils/__init__.py
+-rw-r--r--   0        0        0     1306 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/utils/dynamic_object.py
+-rw-r--r--   0        0        0     7136 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/utils/eval_utils.py
+-rw-r--r--   0        0        0      767 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/utils/loaders.py
+-rw-r--r--   0        0        0     9496 2024-05-08 23:06:17.122384 linkml_map-0.3.6/src/linkml_map/utils/multi_file_transformer.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 linkml_map-0.3.6/PKG-INFO
```

### Comparing `linkml_map-0.3.5/README.md` & `linkml_map-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/pyproject.toml` & `linkml_map-0.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml-map"
-version = "0.3.5"
+version = "0.3.6"
 description = "a framework for specifying and executing mappings between data models"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 linkml-runtime = ">=1.7.2"
```

### Comparing `linkml_map-0.3.5/src/linkml_map/cli/cli.py` & `linkml_map-0.3.6/src/linkml_map/cli/cli.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/compiler/compiler.py` & `linkml_map-0.3.6/src/linkml_map/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/compiler/graphviz_compiler.py` & `linkml_map-0.3.6/src/linkml_map/compiler/graphviz_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/compiler/j2_based_compiler.py` & `linkml_map-0.3.6/src/linkml_map/compiler/j2_based_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/compiler/python_compiler.py` & `linkml_map-0.3.6/src/linkml_map/compiler/python_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/compiler/sql_compiler.py` & `linkml_map-0.3.6/src/linkml_map/compiler/sql_compiler.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/compiler/templates/markdown.j2` & `linkml_map-0.3.6/src/linkml_map/compiler/templates/markdown.j2`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/compiler/tr/transformer_to_mapping_tables.tr.yaml` & `linkml_map-0.3.6/src/linkml_map/compiler/tr/transformer_to_mapping_tables.tr.yaml`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/datamodel/transformer_model.py` & `linkml_map-0.3.6/src/linkml_map/datamodel/transformer_model.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/datamodel/transformer_model.yaml` & `linkml_map-0.3.6/src/linkml_map/datamodel/transformer_model.yaml`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/functions/unit_conversion.py` & `linkml_map-0.3.6/src/linkml_map/functions/unit_conversion.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/importer/importer.py` & `linkml_map-0.3.6/src/linkml_map/importer/importer.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/inference/inference.py` & `linkml_map-0.3.6/src/linkml_map/inference/inference.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/inference/inverter.py` & `linkml_map-0.3.6/src/linkml_map/inference/inverter.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/inference/schema_mapper.py` & `linkml_map-0.3.6/src/linkml_map/inference/schema_mapper.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/session.py` & `linkml_map-0.3.6/src/linkml_map/session.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/transformer/duckdb_transformer.py` & `linkml_map-0.3.6/src/linkml_map/transformer/duckdb_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/transformer/object_transformer.py` & `linkml_map-0.3.6/src/linkml_map/transformer/object_transformer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
+from collections.abc import Mapping
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Type, Union
+from typing import Any, Dict, Iterator, List, Optional, Tuple, Type, Union
 
 import yaml
 from asteval import Interpreter
 from linkml_runtime import SchemaView
 from linkml_runtime.index.object_index import ObjectIndex
 from linkml_runtime.utils.yamlutils import YAMLRoot
 from pydantic import BaseModel
@@ -13,23 +14,105 @@
 from linkml_map.datamodel.transformer_model import (
     CollectionType,
     SerializationSyntaxType,
     SlotDerivation,
 )
 from linkml_map.functions.unit_conversion import UnitSystem, convert_units
 from linkml_map.transformer.transformer import OBJECT_TYPE, Transformer
-from linkml_map.utils.dynamic_object import dynamic_object
-from linkml_map.utils.eval_utils import eval_expr
+from linkml_map.utils.dynamic_object import DynObj, dynamic_object
+from linkml_map.utils.eval_utils import eval_expr, eval_expr_with_mapping
 
 DICT_OBJ = Dict[str, Any]
 
 
 logger = logging.getLogger(__name__)
 
 
+class Bindings(Mapping):
+    """
+    Efficiently access source object attributes.
+    """
+
+    def __init__(
+        self,
+        object_transformer: "ObjectTransformer",
+        source_obj: OBJECT_TYPE,
+        source_obj_typed: OBJECT_TYPE,
+        source_type: str,
+        sv: SchemaView,
+        bindings: Dict,
+    ):
+        self.object_transformer: "ObjectTransformer" = object_transformer
+        self.source_obj: OBJECT_TYPE = source_obj
+        self.source_obj_typed: OBJECT_TYPE = source_obj_typed
+        self.source_type: str = source_type
+        self.sv: SchemaView = sv
+        self.bindings: Dict = {}
+        if bindings:
+            self.bindings.update(bindings)
+
+    def get_ctxt_obj_and_dict(self, source_obj: OBJECT_TYPE = None) -> Tuple[DynObj, OBJECT_TYPE]:
+        """
+        Transform a source object into a typed context object and dictionary, and cache results.
+
+        :param source_obj: Source data. Should be a subset of source_obj provided in the constructor.
+        If None the full source_obj from constructor is used.
+        :return: Tuple of typed context object and context dictionary. The object is the dictionary
+        with keys converted to member variables.
+        """
+        if source_obj is None:
+            source_obj = self.source_obj
+
+        if self.object_transformer.object_index:
+            if not self.source_obj_typed:
+                source_obj_dyn = dynamic_object(source_obj, self.sv, self.source_type)
+            else:
+                source_obj_dyn = self.source_obj_typed
+            # Clear cache: Cache doesn't work since the cache key is the same when source_obj has only a subset
+            # of its keys. eg. {"age": self.source_obj["age"]} and {"name": self.source_obj["name"]}
+            # (with optionally the identifier key included) will have the same cache key, and so `bless` will
+            # incorrectly return the same cached values.
+            self.object_transformer.object_index.clear_proxy_object_cache()
+
+            ctxt_obj = self.object_transformer.object_index.bless(source_obj_dyn)
+            ctxt_dict = {
+                k: getattr(ctxt_obj, k) for k in ctxt_obj._attributes() if not k.startswith("_")
+            }
+        else:
+            do = dynamic_object(source_obj, self.sv, self.source_type)
+            ctxt_obj = do
+            ctxt_dict = vars(do)
+
+        self.bindings.update(ctxt_dict)
+
+        return ctxt_obj, ctxt_dict
+
+    def _all_keys(self) -> List[Any]:
+        keys = list(self.source_obj.keys()) + list(self.bindings.keys())
+        # Remove duplicate keys (ie. found in both source_obj and bindings), and retain original order
+        keys = list(dict.fromkeys(keys).keys())
+        return keys
+
+    def __len__(self) -> int:
+        return len(self._all_keys())
+
+    def __iter__(self) -> Iterator:
+        return iter(self._all_keys())
+
+    def __getitem__(self, name: Any) -> Any:
+        if name not in self.bindings:
+            _ = self.get_ctxt_obj_and_dict({name: self.source_obj[name]})
+
+        return self.bindings.get(name)
+
+    def __setitem__(self, name: Any, value: Any):
+        del name, value
+        raise RuntimeError(f"__setitem__ not allowed on class {self.__class__.__name__}")
+
+
 @dataclass
 class ObjectTransformer(Transformer):
     """
     A Transformer that works on in-memory dict objects.
 
     This works recursively
     """
@@ -108,42 +191,38 @@
             source_obj_typed = source_obj
             source_obj = vars(source_obj)
         if not isinstance(source_obj, dict):
             logger.warning(f"Unexpected: {source_obj} for type {source_type}")
             return source_obj
         class_deriv = self._get_class_derivation(source_type)
         tgt_attrs = {}
+        bindings = None
         # map each slot assignment in source_obj, if there is a slot_derivation
         for slot_derivation in class_deriv.slot_derivations.values():
             v = None
             source_class_slot = None
             if slot_derivation.unit_conversion:
                 v = self._perform_unit_conversion(slot_derivation, source_obj, sv, source_type)
             elif slot_derivation.expr:
-                if self.object_index:
-                    if not source_obj_typed:
-                        source_obj_dyn = dynamic_object(source_obj, sv, source_type)
-                    else:
-                        source_obj_dyn = source_obj_typed
-                    ctxt_obj = self.object_index.bless(source_obj_dyn)
-                    ctxt_dict = {
-                        k: getattr(ctxt_obj, k)
-                        for k in ctxt_obj._attributes()
-                        if not k.startswith("_")
-                    }
-                else:
-                    do = dynamic_object(source_obj, sv, source_type)
-                    ctxt_obj = do
-                    ctxt_dict = vars(do)
+                if bindings is None:
+                    bindings = Bindings(
+                        self,
+                        source_obj=source_obj,
+                        source_obj_typed=source_obj_typed,
+                        source_type=source_type,
+                        sv=sv,
+                        bindings={"NULL": None},
+                    )
 
                 try:
-                    v = eval_expr(slot_derivation.expr, **ctxt_dict, NULL=None)
+                    v = eval_expr_with_mapping(slot_derivation.expr, bindings)
                 except Exception:
                     if not self.unrestricted_eval:
                         raise RuntimeError(f"Expression not in safe subset: {slot_derivation.expr}")
+                    ctxt_obj, _ = bindings.get_ctxt_obj_and_dict()
                     aeval = Interpreter(usersyms={"src": ctxt_obj, "target": None})
                     aeval(slot_derivation.expr)
                     v = aeval.symtable["target"]
             elif slot_derivation.populated_from:
                 v = source_obj.get(slot_derivation.populated_from, None)
                 source_class_slot = sv.induced_slot(slot_derivation.populated_from, source_type)
                 logger.debug(
```

### Comparing `linkml_map-0.3.5/src/linkml_map/transformer/transformer.py` & `linkml_map-0.3.6/src/linkml_map/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/utils/dynamic_object.py` & `linkml_map-0.3.6/src/linkml_map/utils/dynamic_object.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/utils/eval_utils.py` & `linkml_map-0.3.6/src/linkml_map/utils/eval_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
  - See `<https://stackoverflow.com/questions/2371436/evaluating-a-mathematical-expression-in-a-string>`_
 
 TODO: move to core
 """
 
 import ast
 import operator as op
+from collections.abc import Mapping
 
 # supported operators
 from typing import Any, List, Tuple
 
 operators = {
     ast.Add: op.add,
     ast.Sub: op.sub,
@@ -48,14 +49,29 @@
 }
 
 
 class UnsetValueError(Exception):
     pass
 
 
+def eval_expr_with_mapping(expr: str, mapping: Mapping) -> Any:
+    """
+    Evaluates a given expression, with restricted syntax.
+    This function is equivalent to eval_expr where **kwargs has been switched to a Mapping (eg. a dictionary).
+    See eval_expr for details.
+    """
+    if expr == "None":
+        # TODO: do this as part of parsing
+        return None
+    try:
+        return eval_(ast.parse(expr, mode="eval").body, mapping)
+    except UnsetValueError:
+        return None
+
+
 def eval_expr(expr: str, **kwargs) -> Any:
     """
     Evaluates a given expression, with restricted syntax
 
     >>> eval_expr('2^6')
     4
     >>> eval_expr('2**6')
@@ -90,23 +106,15 @@
     - Expressions such as `person.name` can be used on objects to lookup by attribute/slot
     - Paths can be chained, e.g. `person.address.street`
     - Operations on lists are distributed, e.g `container.persons.name` will return a list of names
     - Similarly `strlen(container.persons.name)` will return a list whose members are the lengths of all names
 
     :param expr: expression to evaluate
     """
-    # if kwargs:
-    #    expr = expr.format(**kwargs)
-    if expr == "None":
-        # TODO: do this as part of parsing
-        return None
-    try:
-        return eval_(ast.parse(expr, mode="eval").body, kwargs)
-    except UnsetValueError:
-        return None
+    return eval_expr_with_mapping(expr, kwargs)
 
 
 def eval_(node, bindings=None):
     if isinstance(node, ast.Num):
         return node.n
     elif isinstance(node, ast.Str):
         if "s" in vars(node):
```

### Comparing `linkml_map-0.3.5/src/linkml_map/utils/loaders.py` & `linkml_map-0.3.6/src/linkml_map/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/src/linkml_map/utils/multi_file_transformer.py` & `linkml_map-0.3.6/src/linkml_map/utils/multi_file_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml_map-0.3.5/PKG-INFO` & `linkml_map-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml-map
-Version: 0.3.5
+Version: 0.3.6
 Summary: a framework for specifying and executing mappings between data models
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


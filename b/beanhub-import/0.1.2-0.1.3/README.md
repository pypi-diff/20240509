# Comparing `tmp/beanhub_import-0.1.2.tar.gz` & `tmp/beanhub_import-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.1.2.tar", max compression
+gzip compressed data, was "beanhub_import-0.1.3.tar", max compression
```

## Comparing `beanhub_import-0.1.2.tar` & `beanhub_import-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/LICENSE
--rw-r--r--   0        0        0      174 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/__init__.py
--rw-r--r--   0        0        0       58 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/constants.py
--rw-r--r--   0        0        0     4339 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/data_types.py
--rw-r--r--   0        0        0     7979 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/post_processor.py
--rw-r--r--   0        0        0    10412 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/processor.py
--rw-r--r--   0        0        0      725 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-09 19:08:49.072095 beanhub_import-0.1.3/LICENSE
+-rw-r--r--   0        0        0    22266 2024-05-09 19:08:49.072095 beanhub_import-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/__init__.py
+-rw-r--r--   0        0        0      231 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/constants.py
+-rw-r--r--   0        0        0     4617 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     7962 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0    10490 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/processor.py
+-rw-r--r--   0        0        0      276 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/beanhub_import/templates.py
+-rw-r--r--   0        0        0      757 2024-05-09 19:08:49.076095 beanhub_import-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    23189 1970-01-01 00:00:00.000000 beanhub_import-0.1.3/PKG-INFO
```

### Comparing `beanhub_import-0.1.2/LICENSE` & `beanhub_import-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.2/beanhub_import/data_types.py` & `beanhub_import-0.1.3/beanhub_import/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,22 +58,26 @@
     status: StrMatch | None = None
     type: StrMatch | None = None
     source_account: StrMatch | None = None
     dest_account: StrMatch | None = None
     note: StrMatch | None = None
     reference: StrMatch | None = None
     payee: StrMatch | None = None
+    gl_code: StrMatch | None = None
+    name_on_card: StrMatch | None = None
+    last_four_digits: StrMatch | None = None
 
 
 TxnMatchRule = SimpleTxnMatchRule
 
 
 @enum.unique
 class ActionType(str, enum.Enum):
     add_txn = "add_txn"
+    ignore = "ignore"
 
 
 class AmountTemplate(ImportBaseModel):
     number: str | None = None
     currency: str | None = None
 
 
@@ -138,15 +142,19 @@
 
 class ActionAddTxn(ImportBaseModel):
     type: typing.Literal[ActionType.add_txn] = pydantic.Field(ActionType.add_txn)
     file: str | None = None
     txn: TransactionTemplate
 
 
-Action = ActionAddTxn
+class ActionIgnore(ImportBaseModel):
+    type: typing.Literal[ActionType.ignore] = pydantic.Field(ActionType.ignore)
+
+
+Action = ActionAddTxn | ActionIgnore
 
 
 SimpleFileMatch = str | StrExactMatch | StrRegexMatch
 
 
 class InputConfigDetails(ImportBaseModel):
     extractor: str | None = None
```

### Comparing `beanhub_import-0.1.2/beanhub_import/post_processor.py` & `beanhub_import-0.1.3/beanhub_import/post_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import collections
 import copy
-import itertools
 import json
 import pathlib
 import typing
 
 from beancount_parser.data_types import Entry
 from beancount_parser.data_types import EntryType
 from beancount_parser.helpers import collect_entries
```

### Comparing `beanhub_import-0.1.2/beanhub_import/processor.py` & `beanhub_import-0.1.3/beanhub_import/processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import typing
 
 from beanhub_extract.data_types import Transaction
 from beanhub_extract.extractors import ALL_EXTRACTORS
 from beanhub_extract.utils import strip_txn_base_path
 from jinja2.sandbox import SandboxedEnvironment
 
+from . import constants
 from .data_types import ActionType
 from .data_types import Amount
 from .data_types import GeneratedPosting
 from .data_types import GeneratedTransaction
 from .data_types import ImportDoc
 from .data_types import ImportRule
 from .data_types import InputConfigDetails
@@ -24,22 +25,15 @@
 from .data_types import StrContainsMatch
 from .data_types import StrExactMatch
 from .data_types import StrMatch
 from .data_types import StrOneOfMatch
 from .data_types import StrPrefixMatch
 from .data_types import StrRegexMatch
 from .data_types import StrSuffixMatch
-
-
-DEFAULT_TXN_TEMPLATE = dict(
-    id="{{ file }}:{{ lineno }}",
-    date="{{ date }}",
-    flag="*",
-    narration="{{ desc | default(bank_desc, true) }}",
-)
+from .templates import make_environment
 
 
 def walk_dir_files(
     target_dir: pathlib.Path,
 ) -> typing.Generator[pathlib.Path, None, None]:
     for root, dirs, files in os.walk(target_dir):
         for file in files:
@@ -115,31 +109,34 @@
             return
         return result
 
     for import_rule in import_rules:
         if not match_transaction(txn, import_rule.match):
             continue
         for action in import_rule.actions:
+            if action.type == ActionType.ignore:
+                logger.debug("Ignored transaction %s:%s", txn.file, txn.lineno)
+                return True
             if action.type != ActionType.add_txn:
                 # we only support add txn for now
                 raise ValueError(f"Unsupported action type {action.type}")
 
             template_values = {
                 key: first_non_none(
                     getattr(action.txn, key),
                     getattr(default_txn, key) if default_txn is not None else None,
-                    DEFAULT_TXN_TEMPLATE.get(key),
+                    constants.DEFAULT_TXN_TEMPLATE.get(key),
                 )
                 for key in ("date", "flag", "narration", "payee")
             }
             template_values["id"] = first_non_none(
                 getattr(action.txn, "id"),
                 getattr(default_txn, "id") if default_txn is not None else None,
                 default_import_id,
-                DEFAULT_TXN_TEMPLATE["id"],
+                constants.DEFAULT_TXN_TEMPLATE["id"],
             )
 
             posting_templates: list[PostingTemplate] = []
             if input_config.prepend_postings is not None:
                 posting_templates.extend(input_config.prepend_postings)
             if action.txn.postings is not None:
                 posting_templates.extend(action.txn.postings)
@@ -221,15 +218,15 @@
 
 
 def process_imports(
     import_doc: ImportDoc,
     input_dir: pathlib.Path,
 ) -> typing.Generator[GeneratedTransaction | Transaction, None, None]:
     logger = logging.getLogger(__name__)
-    template_env = SandboxedEnvironment()
+    template_env = make_environment()
     if import_doc.context is not None:
         template_env.globals.update(import_doc.context)
     for filepath in walk_dir_files(input_dir):
         for input_config in import_doc.inputs:
             if not match_file(input_config.match, filepath):
                 continue
             rel_filepath = filepath.relative_to(input_dir)
```

### Comparing `beanhub_import-0.1.2/pyproject.toml` & `beanhub_import-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.1.2"
+version = "0.1.3"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytz = "^2024.1"
-beanhub-extract = "^0.0.5"
 pydantic = "^2.7.1"
 pyyaml = "^6.0.1"
 jinja2 = "^3.1.3"
-beancount-black = "^1.0.2"
-beancount-parser = "^1.1.0"
+beanhub-extract = ">= 0.0.7, <0.1.0"
+beancount-black = ">= 1.0.2, < 1.1.0"
+beancount-parser = ">= 1.2.3, < 1.3.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.1"
 pytest-mock = "^3.11.1"
```


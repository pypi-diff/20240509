# Comparing `tmp/beanhub_import-0.1.1.tar.gz` & `tmp/beanhub_import-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_import-0.1.1.tar", max compression
+gzip compressed data, was "beanhub_import-0.1.2.tar", max compression
```

## Comparing `beanhub_import-0.1.1.tar` & `beanhub_import-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/LICENSE
--rw-r--r--   0        0        0      174 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/__init__.py
--rw-r--r--   0        0        0       58 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/constants.py
--rw-r--r--   0        0        0     3771 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/data_types.py
--rw-r--r--   0        0        0     6928 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/post_processor.py
--rw-r--r--   0        0        0     9218 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/beanhub_import/processor.py
--rw-r--r--   0        0        0      725 2024-05-08 17:54:23.508348 beanhub_import-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/LICENSE
+-rw-r--r--   0        0        0      174 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/__init__.py
+-rw-r--r--   0        0        0       58 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/constants.py
+-rw-r--r--   0        0        0     4339 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/data_types.py
+-rw-r--r--   0        0        0     7979 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/post_processor.py
+-rw-r--r--   0        0        0    10412 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/beanhub_import/processor.py
+-rw-r--r--   0        0        0      725 2024-05-08 23:13:22.980289 beanhub_import-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 beanhub_import-0.1.2/PKG-INFO
```

### Comparing `beanhub_import-0.1.1/LICENSE` & `beanhub_import-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_import-0.1.1/beanhub_import/data_types.py` & `beanhub_import-0.1.2/beanhub_import/data_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,27 +15,38 @@
     regex: str
 
 
 class StrExactMatch(ImportBaseModel):
     equals: str
 
 
+class StrOneOfMatch(ImportBaseModel):
+    one_of: list[str]
+
+
 class StrPrefixMatch(ImportBaseModel):
     prefix: str
 
 
 class StrSuffixMatch(ImportBaseModel):
     suffix: str
 
 
 class StrContainsMatch(ImportBaseModel):
     contains: str
 
 
-StrMatch = str | StrPrefixMatch | StrSuffixMatch | StrExactMatch | StrContainsMatch
+StrMatch = (
+    str
+    | StrPrefixMatch
+    | StrSuffixMatch
+    | StrExactMatch
+    | StrContainsMatch
+    | StrOneOfMatch
+)
 
 
 class SimpleTxnMatchRule(ImportBaseModel):
     extractor: StrMatch | None = None
     file: StrMatch | None = None
     date: StrMatch | None = None
     post_date: StrMatch | None = None
@@ -70,21 +81,29 @@
     # account of the posting
     account: str | None = None
     amount: AmountTemplate | None = None
     price: AmountTemplate | None = None
     cost: str | None = None
 
 
+class MetadataItemTemplate(ImportBaseModel):
+    name: str
+    value: str
+
+
 class TransactionTemplate(ImportBaseModel):
     # the import-id for de-duplication
     id: str | None = None
     date: str | None = None
     flag: str | None = None
     narration: str | None = None
     payee: str | None = None
+    tags: list[str] | None = None
+    links: list[str] | None = None
+    metadata: list[MetadataItemTemplate] | None = None
     postings: list[PostingTemplate] | None = None
 
 
 class Amount(ImportBaseModel):
     number: str
     currency: str
 
@@ -92,24 +111,32 @@
 class GeneratedPosting(ImportBaseModel):
     account: str
     amount: Amount | None = None
     price: Amount | None = None
     cost: str | None = None
 
 
+class MetadataItem(ImportBaseModel):
+    name: str
+    value: str
+
+
 class GeneratedTransaction(ImportBaseModel):
     file: str
     # the `import-id` metadata field for de-duplication
     id: str
     # the `import-src` metadata field for annotating the source file(s)
     sources: list[str] | None = None
     date: str
     flag: str
     narration: str
     payee: str | None = None
+    tags: list[str] | None = None
+    links: list[str] | None = None
+    metadata: list[MetadataItem] | None = None
     postings: list[GeneratedPosting]
 
 
 class ActionAddTxn(ImportBaseModel):
     type: typing.Literal[ActionType.add_txn] = pydantic.Field(ActionType.add_txn)
     file: str | None = None
     txn: TransactionTemplate
@@ -135,14 +162,16 @@
 
 
 class OutputConfig(ImportBaseModel):
     match: SimpleFileMatch
 
 
 class ImportRule(ImportBaseModel):
+    # Name of import rule, for users to read only
+    name: str | None = None
     match: TxnMatchRule
     actions: list[Action]
 
 
 class ImportDoc(ImportBaseModel):
     context: dict | None = None
     inputs: list[InputConfig]
```

### Comparing `beanhub_import-0.1.1/beanhub_import/post_processor.py` & `beanhub_import-0.1.2/beanhub_import/post_processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,18 +17,22 @@
 from .data_types import BeancountTransaction
 from .data_types import ChangeSet
 from .data_types import GeneratedPosting
 from .data_types import GeneratedTransaction
 
 
 def extract_existing_transactions(
-    parser: Lark, bean_file: pathlib.Path, import_id_key: str = constants.IMPORT_ID_KEY
+    parser: Lark,
+    bean_file: pathlib.Path,
+    root_dir: pathlib.Path | None = None,
 ) -> typing.Generator[BeancountTransaction, None, None]:
     last_txn = None
-    for bean_path, tree in traverse(parser=parser, bean_file=bean_file):
+    for bean_path, tree in traverse(
+        parser=parser, bean_file=bean_file, root_dir=root_dir
+    ):
         if tree.data != "start":
             raise ValueError("Expected start")
         for child in tree.children:
             if child is None:
                 continue
             if child.data != "statement":
                 raise ValueError("Expected statement")
@@ -41,15 +45,15 @@
                 if directive_type != "txn":
                     continue
                 last_txn = date_directive
             elif first_child.data == "metadata_item":
                 metadata_key = first_child.children[0].value
                 metadata_value = first_child.children[1]
                 if (
-                    metadata_key == import_id_key
+                    metadata_key == constants.IMPORT_ID_KEY
                     and metadata_value.type == "ESCAPED_STRING"
                 ):
                     yield BeancountTransaction(
                         file=bean_path,
                         lineno=last_txn.meta.line,
                         id=json.loads(metadata_value.value),
                     )
@@ -62,17 +66,16 @@
 ) -> dict[pathlib.Path, ChangeSet]:
     generated_id_txns = {txn.id: txn for txn in generated_txns}
     imported_id_txns = {txn.id: txn for txn in imported_txns}
 
     to_remove = collections.defaultdict(list)
     for txn in imported_txns:
         generated_txn = generated_id_txns.get(txn.id)
-        if generated_txn is not None and txn.file.resolve() != (
-            work_dir / generated_txn.file
-        ):
+        generated_file = (work_dir / generated_txn.file).resolve()
+        if generated_txn is not None and txn.file.resolve() != generated_file:
             # it appears that the generated txn's file is different from the old one, let's remove it
             to_remove[txn.file].append(txn)
 
     to_add = collections.defaultdict(list)
     to_update = collections.defaultdict(dict)
     for txn in generated_txns:
         imported_txn = imported_id_txns.get(txn.id)
@@ -119,27 +122,43 @@
 ) -> str:
     columns = [
         txn.date,
         txn.flag,
         *((json.dumps(txn.payee),) if txn.payee is not None else ()),
         json.dumps(txn.narration),
     ]
+    if txn.tags is not None:
+        columns.extend(map(lambda t: "#" + t, txn.tags))
+    if txn.links is not None:
+        columns.extend(map(lambda t: "^" + t, txn.links))
     line = " ".join(columns)
     import_src = None
     if txn.sources is not None:
         import_src = ":".join(txn.sources)
+    extra_metadata = []
+    if txn.metadata is not None:
+        for item in txn.metadata:
+            if item.name in frozenset(
+                [constants.IMPORT_ID_KEY, constants.IMPORT_SRC_KEY]
+            ):
+                raise ValueError(
+                    f"Metadata item name {item.name} is reserved for beanhub-import usage"
+                )
+            extra_metadata.append(f"  {item.name}: {json.dumps(item.value)}")
+
     return "\n".join(
         [
             line,
             f"  {constants.IMPORT_ID_KEY}: {json.dumps(txn.id)}",
             *(
                 (f"  {constants.IMPORT_SRC_KEY}: {json.dumps(import_src)}",)
                 if import_src is not None
                 else ()
             ),
+            *extra_metadata,
             *(map(posting_to_text, txn.postings)),
         ]
     )
 
 
 def apply_change_set(
     tree: Lark,
@@ -168,33 +187,46 @@
             comments=tail_comments,
             statement=None,
             metadata=[],
             postings=[],
         )
 
     new_children = []
-    for entry in itertools.chain(entries, entries_to_add):
+
+    def _expand_entry(entry: Entry):
+        new_children.append(entry.statement)
+        for metadata in entry.metadata:
+            new_children.extend(metadata.comments)
+            new_children.append(metadata.statement)
+        for posting in entry.postings:
+            new_children.extend(posting.comments)
+            new_children.append(posting.statement)
+            for metadata in posting.metadata:
+                new_children.extend(metadata.comments)
+                new_children.append(metadata.statement)
+
+    # Expand existing entries and look up update replacements if there's one
+    for entry in entries:
         if entry.type == EntryType.COMMENTS:
             new_children.extend(entry.comments)
             continue
         if entry.statement.meta.line in lines_to_remove:
             # We also drop the comments
             continue
         actual_entry = line_to_entries.get(entry.statement.meta.line, entry)
         # use comments from existing entry regardless
         new_children.extend(entry.comments)
-        new_children.append(actual_entry.statement)
-        for metadata in actual_entry.metadata:
-            new_children.extend(metadata.comments)
-            new_children.append(metadata.statement)
-        for posting in actual_entry.postings:
-            new_children.extend(posting.comments)
-            new_children.append(posting.statement)
-            for metadata in posting.metadata:
-                new_children.extend(metadata.comments)
-                new_children.append(metadata.statement)
+        _expand_entry(actual_entry)
+
+    # Add new entries
+    for entry in entries_to_add:
+        if entry.type == EntryType.COMMENTS:
+            new_children.extend(entry.comments)
+            continue
+        new_children.extend(entry.comments)
+        _expand_entry(entry)
 
     if tailing_comments_entry is not None:
         new_children.extend(tailing_comments_entry.comments)
 
     new_tree.children = new_children
     return new_tree
```

### Comparing `beanhub_import-0.1.1/beanhub_import/processor.py` & `beanhub_import-0.1.2/beanhub_import/processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 from .data_types import ActionType
 from .data_types import Amount
 from .data_types import GeneratedPosting
 from .data_types import GeneratedTransaction
 from .data_types import ImportDoc
 from .data_types import ImportRule
 from .data_types import InputConfigDetails
+from .data_types import MetadataItem
 from .data_types import PostingTemplate
 from .data_types import SimpleFileMatch
 from .data_types import SimpleTxnMatchRule
 from .data_types import StrContainsMatch
 from .data_types import StrExactMatch
 from .data_types import StrMatch
+from .data_types import StrOneOfMatch
 from .data_types import StrPrefixMatch
 from .data_types import StrRegexMatch
 from .data_types import StrSuffixMatch
 
 
 DEFAULT_TXN_TEMPLATE = dict(
     id="{{ file }}:{{ lineno }}",
@@ -66,14 +68,16 @@
         return value == pattern.equals
     elif isinstance(pattern, StrPrefixMatch):
         return value.startswith(pattern.prefix)
     elif isinstance(pattern, StrSuffixMatch):
         return value.endswith(pattern.suffix)
     elif isinstance(pattern, StrContainsMatch):
         return pattern.contains in value
+    elif isinstance(pattern, StrOneOfMatch):
+        return value in pattern.one_of
     else:
         raise ValueError(f"Unexpected str match type {type(pattern)}")
 
 
 def match_transaction(txn: Transaction, rule: SimpleTxnMatchRule) -> bool:
     return all(
         match_str(getattr(rule, key), getattr(txn, key))
@@ -99,14 +103,22 @@
     processed = False
 
     def render_str(value: str | None) -> str | None:
         if value is None:
             return None
         return template_env.from_string(value).render(**txn_ctx)
 
+    def process_links_or_tags(links_or_tags: list[str] | None) -> list[str] | None:
+        if links_or_tags is None:
+            return
+        result = list(filter(lambda x: x, [render_str(item) for item in links_or_tags]))
+        if not result:
+            return
+        return result
+
     for import_rule in import_rules:
         if not match_transaction(txn, import_rule.match):
             continue
         for action in import_rule.actions:
             if action.type != ActionType.add_txn:
                 # we only support add txn for now
                 raise ValueError(f"Unsupported action type {action.type}")
@@ -132,14 +144,28 @@
             if action.txn.postings is not None:
                 posting_templates.extend(action.txn.postings)
             elif default_txn is not None and default_txn.postings is not None:
                 posting_templates.extend(default_txn.postings)
             if input_config.appending_postings is not None:
                 posting_templates.extend(input_config.appending_postings)
 
+            generated_tags = process_links_or_tags(action.txn.tags)
+            generated_links = process_links_or_tags(action.txn.links)
+
+            generated_metadata = []
+            if action.txn.metadata is not None:
+                for item in action.txn.metadata:
+                    name = render_str(item.name)
+                    value = render_str(item.value)
+                    if not name or not value:
+                        continue
+                    generated_metadata.append(MetadataItem(name=name, value=value))
+            if not generated_metadata:
+                generated_metadata = None
+
             generated_postings = []
             for posting_template in posting_templates:
                 amount = None
                 if posting_template.amount is not None:
                     amount = Amount(
                         number=render_str(posting_template.amount.number),
                         currency=render_str(posting_template.amount.currency),
@@ -167,21 +193,25 @@
                 logger.error(
                     "Output file not defined when generating transaction with rule %s",
                     import_rule,
                 )
                 raise ValueError(
                     f"Output file not defined when generating transaction with rule {import_rule}"
                 )
+
             processed = True
             yield GeneratedTransaction(
                 # We don't add line number here because sources it is going to be added as `import-src` metadata field.
-                # Otherwise provided CSV's lineno may change every time we run import if the date order is desc and
+                # Otherwise, the provided CSV's lineno may change every time we run import if the date order is desc and
                 # there are new transactions added since then.
                 sources=[txn.file],
                 file=render_str(output_file),
+                tags=generated_tags,
+                links=generated_links,
+                metadata=generated_metadata,
                 postings=generated_postings,
                 **{key: render_str(value) for key, value in template_values.items()},
             )
             # TODO: make it possible to generate multiple transaction by changing rule config if there's
             #       a valid use case
         break
     logger.debug(
```

### Comparing `beanhub_import-0.1.1/pyproject.toml` & `beanhub_import-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-import"
-version = "0.1.1"
+version = "0.1.2"
 description = "The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `beanhub_import-0.1.1/PKG-INFO` & `beanhub_import-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beanhub-import
-Version: 0.1.1
+Version: 0.1.2
 Summary: The simple library for import extracted transactions provided by beanhub-extract and generate corresponding Beancount transactions based on predefined rules
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


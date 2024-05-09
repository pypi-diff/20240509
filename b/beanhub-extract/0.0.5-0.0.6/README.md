# Comparing `tmp/beanhub_extract-0.0.5.tar.gz` & `tmp/beanhub_extract-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanhub_extract-0.0.5.tar", max compression
+gzip compressed data, was "beanhub_extract-0.0.6.tar", max compression
```

## Comparing `beanhub_extract-0.0.5.tar` & `beanhub_extract-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-05 19:15:13.060071 beanhub_extract-0.0.5/LICENSE
--rw-r--r--   0        0        0      165 2024-05-05 19:15:13.060071 beanhub_extract-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-05-05 19:15:13.060071 beanhub_extract-0.0.5/beanhub_extract/__init__.py
--rw-r--r--   0        0        0     1655 2024-05-05 19:15:13.060071 beanhub_extract-0.0.5/beanhub_extract/data_types.py
--rw-r--r--   0        0        0      115 2024-05-05 19:15:13.060071 beanhub_extract-0.0.5/beanhub_extract/extractors/__init__.py
--rw-r--r--   0        0        0     2008 2024-05-05 19:15:13.060071 beanhub_extract-0.0.5/beanhub_extract/extractors/mercury.py
--rw-r--r--   0        0        0      977 2024-05-05 19:15:13.060071 beanhub_extract-0.0.5/beanhub_extract/utils.py
--rw-r--r--   0        0        0      578 2024-05-05 19:15:13.060071 beanhub_extract-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 beanhub_extract-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-09 01:19:39.484397 beanhub_extract-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2636 2024-05-09 01:19:39.484397 beanhub_extract-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 01:19:39.484397 beanhub_extract-0.0.6/beanhub_extract/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-09 01:19:39.484397 beanhub_extract-0.0.6/beanhub_extract/data_types.py
+-rw-r--r--   0        0        0      115 2024-05-09 01:19:39.484397 beanhub_extract-0.0.6/beanhub_extract/extractors/__init__.py
+-rw-r--r--   0        0        0     2423 2024-05-09 01:19:39.484397 beanhub_extract-0.0.6/beanhub_extract/extractors/mercury.py
+-rw-r--r--   0        0        0      977 2024-05-09 01:19:39.484397 beanhub_extract-0.0.6/beanhub_extract/utils.py
+-rw-r--r--   0        0        0      578 2024-05-09 01:19:39.484397 beanhub_extract-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3286 1970-01-01 00:00:00.000000 beanhub_extract-0.0.6/PKG-INFO
```

### Comparing `beanhub_extract-0.0.5/LICENSE` & `beanhub_extract-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.5/beanhub_extract/data_types.py` & `beanhub_extract-0.0.6/beanhub_extract/data_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,7 +40,15 @@
     dest_account: str | None = None
     # note or memo for the transaction
     note: str | None = None
     # Reference value
     reference: str | None = None
     # Payee of the transaction
     payee: str | None = None
+    # General Ledger Code
+    gl_code: str | None = None
+    # Name on the credit/debit card
+    name_on_card: str | None = None
+    # Last 4 digits of credit/debit card
+    last_four_digits: str | None = None
+    # All the columns not handled and put into `Transaction`'s attributes by the extractor goes here
+    extra: dict | None = None
```

### Comparing `beanhub_extract-0.0.5/beanhub_extract/extractors/mercury.py` & `beanhub_extract-0.0.6/beanhub_extract/extractors/mercury.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import csv
 import datetime
 import decimal
+import os
 import typing
 
 import pytz
 
 from ..data_types import Transaction
 
 
@@ -23,39 +24,51 @@
     date = parse_date(parts[0])
     time = parse_time(parts[1])
     return datetime.datetime.combine(date, time)
 
 
 class MercuryExtractor:
     EXTRACTOR_NAME = "mercury"
-    DEFAULT_IMPORT_ID = "{{ file }}:{{ reversed_lineno }}"
+    DEFAULT_IMPORT_ID = "{{ file | as_posix_path }}:{{ reversed_lineno }}"
 
     def __init__(self, input_file: typing.TextIO):
         self.input_file = input_file
 
     def __call__(self) -> typing.Generator[Transaction, None, None]:
         filename = None
         if hasattr(self.input_file, "name"):
             filename = self.input_file.name
+        row_count_reader = csv.DictReader(self.input_file)
+        row_count = 0
+        for _ in row_count_reader:
+            row_count += 1
+        self.input_file.seek(os.SEEK_SET, 0)
         reader = csv.DictReader(self.input_file)
-        # this consumes quite some memory, but it should be fine assume most csv dump files are small
-        rows = list(reader)
         timezone = pytz.UTC
-        for i, row in enumerate(rows):
+        for i, row in enumerate(reader):
+            kwargs = dict(
+                date=parse_date(row.pop("Date (UTC)")),
+                desc=row.pop("Description"),
+                amount=decimal.Decimal(row.pop("Amount")),
+                status=row.pop("Status"),
+                source_account=row.pop("Source Account"),
+                bank_desc=row.pop("Bank Description"),
+                reference=row.pop("Reference"),
+                note=row.pop("Note"),
+                category=row.pop("Category"),
+                currency=row.pop("Original Currency"),
+                name_on_card=row.pop("Name On Card"),
+                last_four_digits=row.pop("Last Four Digits"),
+                gl_code=row.pop("GL Code"),
+                timestamp=parse_datetime(row.pop("Timestamp")).replace(tzinfo=timezone),
+            )
+            if row:
+                kwargs["extra"] = row
+
             yield Transaction(
                 extractor=self.EXTRACTOR_NAME,
                 file=filename,
                 lineno=i + 1,
-                reversed_lineno=i - len(rows),
-                date=parse_date(row["Date (UTC)"]),
-                desc=row["Description"],
-                amount=decimal.Decimal(row["Amount"]),
-                status=row["Status"],
-                source_account=row["Source Account"],
-                bank_desc=row["Bank Description"],
-                reference=row["Reference"],
-                note=row["Note"],
-                category=row["Category"],
-                currency=row["Original Currency"],
-                timestamp=parse_datetime(row["Timestamp"]).replace(tzinfo=timezone),
+                reversed_lineno=i - row_count,
                 timezone="UTC",
+                **kwargs
             )
```

### Comparing `beanhub_extract-0.0.5/beanhub_extract/utils.py` & `beanhub_extract-0.0.6/beanhub_extract/utils.py`

 * *Files identical despite different names*

### Comparing `beanhub_extract-0.0.5/pyproject.toml` & `beanhub_extract-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beanhub-extract"
-version = "0.0.5"
+version = "0.0.6"
 description = "The simple library for extracting all kind of bank account transaction export files, mostly for beanhub-import to inject and generate transactions"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```


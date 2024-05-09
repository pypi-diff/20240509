# Comparing `tmp/biblelib-0.3.5.tar.gz` & `tmp/biblelib-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblelib-0.3.5.tar", max compression
+gzip compressed data, was "biblelib-0.3.6.tar", max compression
```

## Comparing `biblelib-0.3.5.tar` & `biblelib-0.3.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.5/LICENSE.md
--rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.5/LICENSE.md~
--rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.5/README.md
--rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.5/biblelib/__init__.py
--rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.5/biblelib/book/ReadMe.md
--rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.5/biblelib/book/__init__.py
--rw-r--r--   0        0        0    15533 2024-03-24 20:04:43.564328 biblelib-0.3.5/biblelib/book/book.py
--rw-r--r--   0        0        0     5178 2024-04-18 23:10:23.491912 biblelib-0.3.5/biblelib/book/books.tsv
--rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.5/biblelib/sources.py
--rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.5/biblelib/unit/__init__.py
--rw-r--r--   0        0        0     5936 2024-04-23 02:01:59.233109 biblelib-0.3.5/biblelib/unit/book.py
--rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.5/biblelib/unit/bookchapters.tsv
--rw-r--r--   0        0        0     7217 2024-04-23 02:09:13.463233 biblelib-0.3.5/biblelib/unit/chapter.py
--rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.5/biblelib/unit/chapters.tsv
--rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.5/biblelib/unit/chapterverses.tsv
--rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.5/biblelib/unit/pericope.py
--rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.5/biblelib/unit/tempchapter.py
--rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.5/biblelib/unit/unit.py
--rw-r--r--   0        0        0     6339 2024-04-23 02:09:29.760805 biblelib-0.3.5/biblelib/unit/unitrange.py
--rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.5/biblelib/unit/verse.py
--rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.5/biblelib/versification/Enumerator.py
--rw-r--r--   0        0        0     2108 2024-03-19 16:38:12.467449 biblelib-0.3.5/biblelib/versification/Mapper.py
--rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.5/biblelib/versification/ReadMe.md
--rw-r--r--   0        0        0     1871 2024-03-15 00:46:57.917308 biblelib-0.3.5/biblelib/versification/VrefReader.py
--rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.5/biblelib/versification/__init__.py
--rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.5/biblelib/versification/eng-nt-vref.txt
--rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.5/biblelib/versification/eng-ot-vref.txt
--rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.5/biblelib/versification/eng-protestant-vref.txt
--rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.5/biblelib/versification/org-nt-vref.txt
--rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.5/biblelib/versification/org-ot-vref.txt
--rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.5/biblelib/versification/org-protestant-vref.txt
--rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.5/biblelib/versification/rso-nt-vref.txt
--rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.5/biblelib/versification/rso-ot-vref.txt
--rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.5/biblelib/versification/rso-protestant-vref.txt
--rw-r--r--   0        0        0      910 2024-05-06 23:25:56.736634 biblelib-0.3.5/biblelib/word/__init__.py
--rw-r--r--   0        0        0    25126 2024-05-07 00:20:10.294458 biblelib-0.3.5/biblelib/word/bcvwpid.py
--rw-r--r--   0        0        0      356 2024-05-06 23:17:32.231962 biblelib-0.3.5/biblelib/word/mappings/__init__.py
--rw-r--r--   0        0        0     5513 2024-05-06 22:42:51.746991 biblelib-0.3.5/biblelib/word/mappings/gnt.py
--rw-r--r--   0        0        0     1189 2024-05-07 00:20:11.048356 biblelib-0.3.5/biblelib/word/mappings/marble.py
--rw-r--r--   0        0        0     3671 2024-05-06 21:44:17.650867 biblelib-0.3.5/biblelib/word/mappings/wlcm.py
--rw-r--r--   0        0        0     1324 2024-05-07 00:36:40.536806 biblelib-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.6/LICENSE.md
+-rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.6/LICENSE.md~
+-rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.6/README.md
+-rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.6/biblelib/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.6/biblelib/book/ReadMe.md
+-rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.6/biblelib/book/__init__.py
+-rw-r--r--   0        0        0    15533 2024-03-24 20:04:43.564328 biblelib-0.3.6/biblelib/book/book.py
+-rw-r--r--   0        0        0     5178 2024-04-18 23:10:23.491912 biblelib-0.3.6/biblelib/book/books.tsv
+-rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.6/biblelib/sources.py
+-rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.6/biblelib/unit/__init__.py
+-rw-r--r--   0        0        0     5936 2024-04-23 02:01:59.233109 biblelib-0.3.6/biblelib/unit/book.py
+-rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.6/biblelib/unit/bookchapters.tsv
+-rw-r--r--   0        0        0     7217 2024-04-23 02:09:13.463233 biblelib-0.3.6/biblelib/unit/chapter.py
+-rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.6/biblelib/unit/chapters.tsv
+-rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.6/biblelib/unit/chapterverses.tsv
+-rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.6/biblelib/unit/pericope.py
+-rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.6/biblelib/unit/tempchapter.py
+-rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.6/biblelib/unit/unit.py
+-rw-r--r--   0        0        0     6339 2024-04-23 02:09:29.760805 biblelib-0.3.6/biblelib/unit/unitrange.py
+-rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.6/biblelib/unit/verse.py
+-rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.6/biblelib/versification/Enumerator.py
+-rw-r--r--   0        0        0     2108 2024-03-19 16:38:12.467449 biblelib-0.3.6/biblelib/versification/Mapper.py
+-rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.6/biblelib/versification/ReadMe.md
+-rw-r--r--   0        0        0     1871 2024-03-15 00:46:57.917308 biblelib-0.3.6/biblelib/versification/VrefReader.py
+-rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.6/biblelib/versification/__init__.py
+-rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.6/biblelib/versification/eng-nt-vref.txt
+-rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.6/biblelib/versification/eng-ot-vref.txt
+-rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.6/biblelib/versification/eng-protestant-vref.txt
+-rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.6/biblelib/versification/org-nt-vref.txt
+-rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.6/biblelib/versification/org-ot-vref.txt
+-rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.6/biblelib/versification/org-protestant-vref.txt
+-rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.6/biblelib/versification/rso-nt-vref.txt
+-rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.6/biblelib/versification/rso-ot-vref.txt
+-rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.6/biblelib/versification/rso-protestant-vref.txt
+-rw-r--r--   0        0        0      910 2024-05-06 23:25:56.736634 biblelib-0.3.6/biblelib/word/__init__.py
+-rw-r--r--   0        0        0    25630 2024-05-09 21:24:01.299209 biblelib-0.3.6/biblelib/word/bcvwpid.py
+-rw-r--r--   0        0        0      356 2024-05-06 23:17:32.231962 biblelib-0.3.6/biblelib/word/mappings/__init__.py
+-rw-r--r--   0        0        0     5513 2024-05-06 22:42:51.746991 biblelib-0.3.6/biblelib/word/mappings/gnt.py
+-rw-r--r--   0        0        0     1189 2024-05-07 00:20:11.048356 biblelib-0.3.6/biblelib/word/mappings/marble.py
+-rw-r--r--   0        0        0     3671 2024-05-06 21:44:17.650867 biblelib-0.3.6/biblelib/word/mappings/wlcm.py
+-rw-r--r--   0        0        0     1324 2024-05-09 21:35:48.550711 biblelib-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.6/PKG-INFO
```

### Comparing `biblelib-0.3.5/LICENSE.md` & `biblelib-0.3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/LICENSE.md~` & `biblelib-0.3.6/LICENSE.md~`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/README.md` & `biblelib-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/book/ReadMe.md` & `biblelib-0.3.6/biblelib/book/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/book/book.py` & `biblelib-0.3.6/biblelib/book/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/book/books.tsv` & `biblelib-0.3.6/biblelib/book/books.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/sources.py` & `biblelib-0.3.6/biblelib/sources.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/__init__.py` & `biblelib-0.3.6/biblelib/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/book.py` & `biblelib-0.3.6/biblelib/unit/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/bookchapters.tsv` & `biblelib-0.3.6/biblelib/unit/bookchapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/chapter.py` & `biblelib-0.3.6/biblelib/unit/chapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/chapters.tsv` & `biblelib-0.3.6/biblelib/unit/chapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/chapterverses.tsv` & `biblelib-0.3.6/biblelib/unit/chapterverses.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/pericope.py` & `biblelib-0.3.6/biblelib/unit/pericope.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/tempchapter.py` & `biblelib-0.3.6/biblelib/unit/tempchapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/unit.py` & `biblelib-0.3.6/biblelib/unit/unit.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/unitrange.py` & `biblelib-0.3.6/biblelib/unit/unitrange.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/unit/verse.py` & `biblelib-0.3.6/biblelib/unit/verse.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/Enumerator.py` & `biblelib-0.3.6/biblelib/versification/Enumerator.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/Mapper.py` & `biblelib-0.3.6/biblelib/versification/Mapper.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/ReadMe.md` & `biblelib-0.3.6/biblelib/versification/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/VrefReader.py` & `biblelib-0.3.6/biblelib/versification/VrefReader.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/eng-nt-vref.txt` & `biblelib-0.3.6/biblelib/versification/eng-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/eng-ot-vref.txt` & `biblelib-0.3.6/biblelib/versification/eng-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/eng-protestant-vref.txt` & `biblelib-0.3.6/biblelib/versification/eng-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/org-nt-vref.txt` & `biblelib-0.3.6/biblelib/versification/org-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/org-ot-vref.txt` & `biblelib-0.3.6/biblelib/versification/org-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/org-protestant-vref.txt` & `biblelib-0.3.6/biblelib/versification/org-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/rso-nt-vref.txt` & `biblelib-0.3.6/biblelib/versification/rso-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/rso-ot-vref.txt` & `biblelib-0.3.6/biblelib/versification/rso-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/versification/rso-protestant-vref.txt` & `biblelib-0.3.6/biblelib/versification/rso-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/word/__init__.py` & `biblelib-0.3.6/biblelib/word/__init__.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/word/bcvwpid.py` & `biblelib-0.3.6/biblelib/word/bcvwpid.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,15 +357,16 @@
     - BB identifies a book
     - CCC identifies a chapter number
     - VVV identifies a verse number
     - WWW identifies a word number
     - P optionally identifies a word part: this is optional for NT
       books, where it defaults to 1 if output.
 
-    Identifiers may have an optional corpus prefix.
+    Identifiers may have an optional corpus prefix. This is removed
+    from the ID but retained as self.corpus_prefix.
 
     This dataclass does not validate whether any identifiers are in
     the correct range: it only records the data. Validation is planned
     for a future version.
 
     All sequence indices are one-based, not zero-based, and derived
     from the tokenization of the input text (which should be specified
@@ -387,14 +388,16 @@
     to other Book identifiers.
 
     """
 
     # book mapping data
     word_ID: str = field(init=False)
     part_ID: str = ""
+    # this is not part of the overall ID, and is computed based on
+    # book
     canon_prefix: str = ""
     # the longth of the bcvwp ID
     _idlen = 11
 
     def __post_init__(self) -> None:
         """Compute other values on initialization.
 
@@ -417,49 +420,54 @@
         # cannot call super because allows either 11 or 12 length
         # super()__post_init__()
         idpat = re.compile(r"^[no]?\d{11,12}$")
         assert idpat.match(self.ID), f"Invalid identifier: {self.ID}"
         # assert 13 >= len(self.ID) >= 11, f"Invalid length: {self.ID}"
         if self.ID.startswith("o") or self.ID.startswith("n"):
             self.canon_prefix = self.ID[0]
-            restid = self.ID[1:]
+            restid = self.ID = self.ID[1:]
         else:
             restid = self.ID
             # set canon_prefix and prepend to ID
             self.canon_prefix = _get_canon_prefix(restid[0:2])
-            self.ID = self.canon_prefix + self.ID
+            # don't include canon prefix in the ID: decide that at
+            # output time with get_id().
+            # self.ID = self.canon_prefix + self.ID
         self.book_ID = restid[0:2]
         # TODO: add tests, presumably a closed set of values
         assert self.canon_prefix == _get_canon_prefix(self.book_ID), f"Canon prefix must match book ID: {self.ID}"
         self.chapter_ID = restid[2:5]
         self.verse_ID = restid[5:8]
         self.word_ID = restid[8:11]
         if len(restid) == 12:
             self.part_ID = restid[11]
         else:
             self.part_ID = "1"
             self.ID += self.part_ID
 
-    def get_id(self, prefix: bool = True, nt_part: bool = False) -> str:
+    def get_id(self, prefix: bool = False, part_index: bool = True) -> str:
         """Return a string identifier for the instance.
 
-        With prefix (default=True), prefix OT references with 'o' and
-        NT references with 'n'.
-
-        With nt_part=True (default=False), if an NT token, include a
-        part ID'. This makes the identifier 12 characters, same as for
-        Hebrew.
+        With prefix (default=False), prefix OT references with 'o' and
+        NT references with 'n'. This is only typcal for Macula source
+        references.
+
+        With part_index (default=True), include a part ID, making the
+        identifier 12 characters. This is typical for Hebrew, but not
+        for Greek or target tokens. Raise ValueError if this would
+        drop a non-default part ID.
 
         """
         strid = self.ID
-        if not prefix:
+        if prefix:
             # drop the prefix
-            strid = self.ID[1:]
-        if self.canon_prefix == "n" and not nt_part:
-            # drop the part
+            strid = f"{self.canon_prefix}{strid}"
+        if not part_index:
+            if self.part_ID not in {"", "1"}:
+                raise ValueError(f"Unsafe to drop non-default part index: {self}")
             strid = strid[:-1]
         return strid
 
     def includes(self, other: Any) -> bool:
         """Return True if other is included in the scope of self.
 
         Simply based on substring matching. Any instance includes
```

### Comparing `biblelib-0.3.5/biblelib/word/mappings/gnt.py` & `biblelib-0.3.6/biblelib/word/mappings/gnt.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/word/mappings/marble.py` & `biblelib-0.3.6/biblelib/word/mappings/marble.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/biblelib/word/mappings/wlcm.py` & `biblelib-0.3.6/biblelib/word/mappings/wlcm.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.5/pyproject.toml` & `biblelib-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biblelib"
-version = "0.3.5"
+version = "0.3.6"
 description = "Utilities for working with metadata for Bible books, references, pericopes, and other units."
 authors = ["Sean Boisen <sean.boisen@gmail.com>"]
 repository = "https://github.com/Clear-Bible/Biblelib/"
 # documentation = "https://sboisen.github.io/Biblelib/"
 readme = "README.md"
 # apparently text files are also shipped?
 # include = [
```

### Comparing `biblelib-0.3.5/PKG-INFO` & `biblelib-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblelib
-Version: 0.3.5
+Version: 0.3.6
 Summary: Utilities for working with metadata for Bible books, references, pericopes, and other units.
 Home-page: https://github.com/Clear-Bible/Biblelib/
 Author: Sean Boisen
 Author-email: sean.boisen@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


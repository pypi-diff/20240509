# Comparing `tmp/feezfuzz-0.1.4.4.tar.gz` & `tmp/feezfuzz-0.1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feezfuzz-0.1.4.4.tar", last modified: Thu May  9 11:59:09 2024, max compression
+gzip compressed data, was "feezfuzz-0.1.4.5.tar", last modified: Thu May  9 12:08:22 2024, max compression
```

## Comparing `feezfuzz-0.1.4.4.tar` & `feezfuzz-0.1.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1073 2023-04-23 04:29:22.226756 feezfuzz-0.1.4.4/LICENSE
--rw-r--r--   0        0        0      687 2024-03-21 05:39:38.563881 feezfuzz-0.1.4.4/README.md
--rw-r--r--   0        0        0      509 2024-05-09 11:59:09.827593 feezfuzz-0.1.4.4/pyproject.toml
--rw-r--r--   0        0        0        2 2024-03-21 05:35:28.830530 feezfuzz-0.1.4.4/src/feezfuzz/__init__.py
--rw-r--r--   0        0        0     1201 2024-03-21 10:55:08.017170 feezfuzz-0.1.4.4/src/feezfuzz/__main__.py
--rw-r--r--   0        0        0     3584 2024-04-02 14:21:52.378981 feezfuzz-0.1.4.4/src/feezfuzz/build.py
--rw-r--r--   0        0        0      209 2024-04-02 14:21:52.378981 feezfuzz-0.1.4.4/src/feezfuzz/enums/__init__.py
--rw-r--r--   0        0        0       64 2023-04-28 04:25:53.170095 feezfuzz-0.1.4.4/src/feezfuzz/enums/cardtypes.py
--rw-r--r--   0        0        0      806 2024-03-31 17:08:30.780185 feezfuzz-0.1.4.4/src/feezfuzz/enums/columnnames.py
--rw-r--r--   0        0        0       99 2023-04-28 04:26:09.233429 feezfuzz-0.1.4.4/src/feezfuzz/enums/datatypes.py
--rw-r--r--   0        0        0     5396 2024-03-21 06:57:30.047535 feezfuzz-0.1.4.4/src/feezfuzz/enums/instructions.py
--rw-r--r--   0        0        0       85 2023-04-28 04:25:23.303426 feezfuzz-0.1.4.4/src/feezfuzz/enums/slotnames.py
--rw-r--r--   0        0        0      281 2023-04-28 04:43:00.356832 feezfuzz-0.1.4.4/src/feezfuzz/enums/spellclasses.py
--rw-r--r--   0        0        0      390 2023-04-28 04:26:59.500099 feezfuzz-0.1.4.4/src/feezfuzz/enums/uuidgroups.py
--rw-r--r--   0        0        0      687 2023-04-28 04:26:43.510098 feezfuzz-0.1.4.4/src/feezfuzz/enums/uuidtypes.py
--rw-r--r--   0        0        0      247 2024-03-31 14:17:11.631258 feezfuzz-0.1.4.4/src/feezfuzz/io_utils.py
--rw-r--r--   0        0        0      485 2024-03-11 15:22:30.446984 feezfuzz-0.1.4.4/src/feezfuzz/nodes/byte.py
--rw-r--r--   0        0        0      548 2024-03-11 15:31:02.597020 feezfuzz-0.1.4.4/src/feezfuzz/nodes/cardid.py
--rw-r--r--   0        0        0     2561 2024-03-31 17:49:47.283688 feezfuzz-0.1.4.4/src/feezfuzz/nodes/cell.py
--rw-r--r--   0        0        0      453 2024-03-11 15:25:44.483664 feezfuzz-0.1.4.4/src/feezfuzz/nodes/column.py
--rw-r--r--   0        0        0     4073 2024-04-02 14:19:31.168971 feezfuzz-0.1.4.4/src/feezfuzz/nodes/command.py
--rw-r--r--   0        0        0      502 2024-03-11 15:24:57.510328 feezfuzz-0.1.4.4/src/feezfuzz/nodes/indextable.py
--rw-r--r--   0        0        0     1101 2024-03-11 15:24:31.110326 feezfuzz-0.1.4.4/src/feezfuzz/nodes/level.py
--rw-r--r--   0        0        0     2377 2024-03-31 14:17:49.184594 feezfuzz-0.1.4.4/src/feezfuzz/nodes/row.py
--rw-r--r--   0        0        0     1357 2024-05-09 11:58:11.642139 feezfuzz-0.1.4.4/src/feezfuzz/nodes/script.py
--rw-r--r--   0        0        0      922 2024-03-15 14:24:52.210273 feezfuzz-0.1.4.4/src/feezfuzz/nodes/string.py
--rw-r--r--   0        0        0     2077 2024-04-02 14:21:52.378981 feezfuzz-0.1.4.4/src/feezfuzz/nodes/table.py
--rw-r--r--   0        0        0      769 2024-03-11 21:33:23.503417 feezfuzz-0.1.4.4/src/feezfuzz/nodes/uint.py
--rw-r--r--   0        0        0      333 2024-03-11 15:22:57.090320 feezfuzz-0.1.4.4/src/feezfuzz/nodes/ushort.py
--rw-r--r--   0        0        0      734 2024-03-15 14:26:32.626947 feezfuzz-0.1.4.4/src/feezfuzz/nodes/uuid.py
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 feezfuzz-0.1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-23 04:29:22.226756 feezfuzz-0.1.4.5/LICENSE
+-rw-r--r--   0        0        0      687 2024-03-21 05:39:38.563881 feezfuzz-0.1.4.5/README.md
+-rw-r--r--   0        0        0      509 2024-05-09 12:08:22.778169 feezfuzz-0.1.4.5/pyproject.toml
+-rw-r--r--   0        0        0        2 2024-03-21 05:35:28.830530 feezfuzz-0.1.4.5/src/feezfuzz/__init__.py
+-rw-r--r--   0        0        0     1201 2024-03-21 10:55:08.017170 feezfuzz-0.1.4.5/src/feezfuzz/__main__.py
+-rw-r--r--   0        0        0     3584 2024-04-02 14:21:52.378981 feezfuzz-0.1.4.5/src/feezfuzz/build.py
+-rw-r--r--   0        0        0      209 2024-04-02 14:21:52.378981 feezfuzz-0.1.4.5/src/feezfuzz/enums/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-28 04:25:53.170095 feezfuzz-0.1.4.5/src/feezfuzz/enums/cardtypes.py
+-rw-r--r--   0        0        0      806 2024-03-31 17:08:30.780185 feezfuzz-0.1.4.5/src/feezfuzz/enums/columnnames.py
+-rw-r--r--   0        0        0       99 2023-04-28 04:26:09.233429 feezfuzz-0.1.4.5/src/feezfuzz/enums/datatypes.py
+-rw-r--r--   0        0        0     5396 2024-03-21 06:57:30.047535 feezfuzz-0.1.4.5/src/feezfuzz/enums/instructions.py
+-rw-r--r--   0        0        0       85 2023-04-28 04:25:23.303426 feezfuzz-0.1.4.5/src/feezfuzz/enums/slotnames.py
+-rw-r--r--   0        0        0      281 2023-04-28 04:43:00.356832 feezfuzz-0.1.4.5/src/feezfuzz/enums/spellclasses.py
+-rw-r--r--   0        0        0      390 2023-04-28 04:26:59.500099 feezfuzz-0.1.4.5/src/feezfuzz/enums/uuidgroups.py
+-rw-r--r--   0        0        0      687 2023-04-28 04:26:43.510098 feezfuzz-0.1.4.5/src/feezfuzz/enums/uuidtypes.py
+-rw-r--r--   0        0        0      247 2024-03-31 14:17:11.631258 feezfuzz-0.1.4.5/src/feezfuzz/io_utils.py
+-rw-r--r--   0        0        0      485 2024-03-11 15:22:30.446984 feezfuzz-0.1.4.5/src/feezfuzz/nodes/byte.py
+-rw-r--r--   0        0        0      548 2024-03-11 15:31:02.597020 feezfuzz-0.1.4.5/src/feezfuzz/nodes/cardid.py
+-rw-r--r--   0        0        0     2561 2024-03-31 17:49:47.283688 feezfuzz-0.1.4.5/src/feezfuzz/nodes/cell.py
+-rw-r--r--   0        0        0      453 2024-03-11 15:25:44.483664 feezfuzz-0.1.4.5/src/feezfuzz/nodes/column.py
+-rw-r--r--   0        0        0     4073 2024-04-02 14:19:31.168971 feezfuzz-0.1.4.5/src/feezfuzz/nodes/command.py
+-rw-r--r--   0        0        0      502 2024-03-11 15:24:57.510328 feezfuzz-0.1.4.5/src/feezfuzz/nodes/indextable.py
+-rw-r--r--   0        0        0     1101 2024-03-11 15:24:31.110326 feezfuzz-0.1.4.5/src/feezfuzz/nodes/level.py
+-rw-r--r--   0        0        0     2377 2024-03-31 14:17:49.184594 feezfuzz-0.1.4.5/src/feezfuzz/nodes/row.py
+-rw-r--r--   0        0        0     1378 2024-05-09 12:07:44.083673 feezfuzz-0.1.4.5/src/feezfuzz/nodes/script.py
+-rw-r--r--   0        0        0      922 2024-03-15 14:24:52.210273 feezfuzz-0.1.4.5/src/feezfuzz/nodes/string.py
+-rw-r--r--   0        0        0     2077 2024-04-02 14:21:52.378981 feezfuzz-0.1.4.5/src/feezfuzz/nodes/table.py
+-rw-r--r--   0        0        0      769 2024-03-11 21:33:23.503417 feezfuzz-0.1.4.5/src/feezfuzz/nodes/uint.py
+-rw-r--r--   0        0        0      333 2024-03-11 15:22:57.090320 feezfuzz-0.1.4.5/src/feezfuzz/nodes/ushort.py
+-rw-r--r--   0        0        0      734 2024-03-15 14:26:32.626947 feezfuzz-0.1.4.5/src/feezfuzz/nodes/uuid.py
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 feezfuzz-0.1.4.5/PKG-INFO
```

### Comparing `feezfuzz-0.1.4.4/LICENSE` & `feezfuzz-0.1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/README.md` & `feezfuzz-0.1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/__main__.py` & `feezfuzz-0.1.4.5/src/feezfuzz/__main__.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/build.py` & `feezfuzz-0.1.4.5/src/feezfuzz/build.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/enums/columnnames.py` & `feezfuzz-0.1.4.5/src/feezfuzz/enums/columnnames.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/enums/instructions.py` & `feezfuzz-0.1.4.5/src/feezfuzz/enums/instructions.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/enums/uuidtypes.py` & `feezfuzz-0.1.4.5/src/feezfuzz/enums/uuidtypes.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/cardid.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/cardid.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/cell.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/cell.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/command.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/command.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/level.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/level.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/row.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/row.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/script.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/script.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 from .uint import Uint
 from .uuid import Uuid
 from ..enums import INSTRUCTIONS
 
 
 class Script:
     def __init__(self, script: str, longform: bool = False):
-        self.script = script.replace("\r", "\n").replace("\t", "    ")
+        self.script = script.replace("\r", "\n")
         self.commands = [
             Command(string, longform)
             for string in self.script.strip().split("\n")
         ]
 
     @classmethod
     def from_toml(cls, script: str, locale: "Table", npc_id: str):
+        script = script.replace("\t", " ")
         while text := re.search("<.*?>", script, flags=re.DOTALL):
             text = text.group(0)
             uuid = locale.register_text(format_text(text), Uuid(npc_id).uid.value)
             script = re.sub(re.escape(text), uuid.hex(), script)
         return cls(script, longform=True)
 
     def xml(self):
```

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/string.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/string.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/table.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/table.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/uint.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/uint.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/src/feezfuzz/nodes/uuid.py` & `feezfuzz-0.1.4.5/src/feezfuzz/nodes/uuid.py`

 * *Files identical despite different names*

### Comparing `feezfuzz-0.1.4.4/PKG-INFO` & `feezfuzz-0.1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feezfuzz
-Version: 0.1.4.4
+Version: 0.1.4.5
 Summary: A WIP parser for Zanzarah's Data files.
 Author-Email: AcipenserSturio <AcipenserSturio@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: tomli>=2.0.1
 Requires-Dist: tomli-w>=1.0.0
 Description-Content-Type: text/markdown
```


# Comparing `tmp/btrview-0.6.3.tar.gz` & `tmp/btrview-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btrview-0.6.3.tar", last modified: Sun May  5 15:28:05 2024, max compression
+gzip compressed data, was "btrview-0.7.0.tar", last modified: Thu May  9 03:49:43 2024, max compression
```

## Comparing `btrview-0.6.3.tar` & `btrview-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 15:28:05.678496 btrview-0.6.3/
--rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.6.3/LICENSE.md
--rw-r--r--   0 chris     (1000) chris     (1000)     6296 2024-05-05 15:28:05.675163 btrview-0.6.3/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)     4284 2024-05-03 19:16:33.000000 btrview-0.6.3/README.md
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 15:28:05.675163 btrview-0.6.3/btrview/
--rw-r--r--   0 chris     (1000) chris     (1000)       86 2024-05-05 15:27:53.000000 btrview-0.6.3/btrview/__init__.py
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.6.3/btrview/__main__.py
--rw-r--r--   0 chris     (1000) chris     (1000)     3665 2024-05-05 15:16:06.000000 btrview-0.6.3/btrview/btr_dict.py
--rw-r--r--   0 chris     (1000) chris     (1000)     7362 2024-04-18 03:01:25.000000 btrview-0.6.3/btrview/btrfs.py
--rw-r--r--   0 chris     (1000) chris     (1000)     6906 2024-05-05 15:24:51.000000 btrview-0.6.3/btrview/rich_output.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 15:28:05.675163 btrview-0.6.3/btrview/scripts/
--rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.6.3/btrview/scripts/btrview.py
--rw-r--r--   0 chris     (1000) chris     (1000)     5914 2024-05-05 13:39:59.000000 btrview-0.6.3/btrview/subvolume.py
--rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-04-10 13:31:52.000000 btrview-0.6.3/btrview/utils.py
-drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-05 15:28:05.675163 btrview-0.6.3/btrview.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     6296 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) chris     (1000)      388 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/entry_points.txt
--rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/requires.txt
--rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-05 15:28:05.000000 btrview-0.6.3/btrview.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) chris     (1000)     1215 2024-05-05 15:27:53.000000 btrview-0.6.3/pyproject.toml
--rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-05 15:28:05.678496 btrview-0.6.3/setup.cfg
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-09 03:49:43.176333 btrview-0.7.0/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1069 2024-04-18 05:35:32.000000 btrview-0.7.0/LICENSE.md
+-rw-r--r--   0 chris     (1000) chris     (1000)     6364 2024-05-09 03:49:43.176333 btrview-0.7.0/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)     4352 2024-05-09 03:44:40.000000 btrview-0.7.0/README.md
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-09 03:49:43.173000 btrview-0.7.0/btrview/
+-rw-r--r--   0 chris     (1000) chris     (1000)       88 2024-05-09 03:49:20.000000 btrview-0.7.0/btrview/__init__.py
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.7.0/btrview/__main__.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     7839 2024-05-09 03:38:00.000000 btrview-0.7.0/btrview/btrfs.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     6906 2024-05-09 03:00:04.000000 btrview-0.7.0/btrview/rich_output.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-09 03:49:43.176333 btrview-0.7.0/btrview/scripts/
+-rwxr-xr-x   0 chris     (1000) chris     (1000)     2172 2024-04-18 03:01:25.000000 btrview-0.7.0/btrview/scripts/btrview.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     4534 2024-05-09 03:38:00.000000 btrview-0.7.0/btrview/subvolume.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     3217 2024-05-09 03:38:00.000000 btrview-0.7.0/btrview/typed_info.py
+-rw-r--r--   0 chris     (1000) chris     (1000)     1254 2024-05-07 01:01:20.000000 btrview-0.7.0/btrview/utils.py
+drwxr-xr-x   0 chris     (1000) chris     (1000)        0 2024-05-09 03:49:43.176333 btrview-0.7.0/btrview.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     6364 2024-05-09 03:49:43.000000 btrview-0.7.0/btrview.egg-info/PKG-INFO
+-rw-r--r--   0 chris     (1000) chris     (1000)      390 2024-05-09 03:49:43.000000 btrview-0.7.0/btrview.egg-info/SOURCES.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        1 2024-05-09 03:49:43.000000 btrview-0.7.0/btrview.egg-info/dependency_links.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       57 2024-05-09 03:49:43.000000 btrview-0.7.0/btrview.egg-info/entry_points.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)       64 2024-05-09 03:49:43.000000 btrview-0.7.0/btrview.egg-info/requires.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)        8 2024-05-09 03:49:43.000000 btrview-0.7.0/btrview.egg-info/top_level.txt
+-rw-r--r--   0 chris     (1000) chris     (1000)     1215 2024-05-09 03:49:20.000000 btrview-0.7.0/pyproject.toml
+-rw-r--r--   0 chris     (1000) chris     (1000)       38 2024-05-09 03:49:43.176333 btrview-0.7.0/setup.cfg
```

### Comparing `btrview-0.6.3/LICENSE.md` & `btrview-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `btrview-0.6.3/PKG-INFO` & `btrview-0.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.6.3
+Version: 0.7.0
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,17 +63,17 @@
 
 Btrview relies on the following dependencies:
 * python 3.11 or greater
 * btrfs-progs
 * python-treelib
 * python-rich
 
-If you have pip installed you can grab btrview from the python package index with `pip install btrview`. Using pip to install btrview will also install the required python dependencies. In addition installing via pip will add the `btrview` command to your path allowing you to run the command from anywhere on the system. 
+The easiest way to download btrview is to use [pipx](https://pipx.pypa.io/stable/installation/) to download it from the python package index. Use the command `pipx --system-site-packages install btrview`. Using pipx to install btrview will also install the required python dependencies and add the `btrview` command to your path allowing you to run the command from anywhere on the system.
 
-If you don't feel like installing via pip you can download it via `git clone https://github.com/CopOnTheRun/btrview` then `cd btrview`. From within the btrview directory you can run the script with `python -m btrview`. Note that if you clone the repository you'll need to make sure you have all the dependencies installed already.
+If you don't feel like installing via pipx you can download it via `git clone https://github.com/CopOnTheRun/btrview` then `cd btrview`. From within the btrview directory you can run the script with `python -m btrview`. Note that if you clone the repository you'll need to make sure you have all the dependencies installed already.
 
 ## Some Qs and As:
 
 ### Q: What is btrfs?
 
 In short, it's a copy on write (COW) filesystem. If you're not already using btrfs, then check out the [documentation](https://btrfs.readthedocs.io/en/latest/) to see if it's something you'd be interested in.
```

### Comparing `btrview-0.6.3/README.md` & `btrview-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 Btrview relies on the following dependencies:
 * python 3.11 or greater
 * btrfs-progs
 * python-treelib
 * python-rich
 
-If you have pip installed you can grab btrview from the python package index with `pip install btrview`. Using pip to install btrview will also install the required python dependencies. In addition installing via pip will add the `btrview` command to your path allowing you to run the command from anywhere on the system. 
+The easiest way to download btrview is to use [pipx](https://pipx.pypa.io/stable/installation/) to download it from the python package index. Use the command `pipx --system-site-packages install btrview`. Using pipx to install btrview will also install the required python dependencies and add the `btrview` command to your path allowing you to run the command from anywhere on the system.
 
-If you don't feel like installing via pip you can download it via `git clone https://github.com/CopOnTheRun/btrview` then `cd btrview`. From within the btrview directory you can run the script with `python -m btrview`. Note that if you clone the repository you'll need to make sure you have all the dependencies installed already.
+If you don't feel like installing via pipx you can download it via `git clone https://github.com/CopOnTheRun/btrview` then `cd btrview`. From within the btrview directory you can run the script with `python -m btrview`. Note that if you clone the repository you'll need to make sure you have all the dependencies installed already.
 
 ## Some Qs and As:
 
 ### Q: What is btrfs?
 
 In short, it's a copy on write (COW) filesystem. If you're not already using btrfs, then check out the [documentation](https://btrfs.readthedocs.io/en/latest/) to see if it's something you'd be interested in.
```

### Comparing `btrview-0.6.3/btrview/__main__.py` & `btrview-0.7.0/btrview/__main__.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.3/btrview/btr_dict.py` & `btrview-0.7.0/btrview/typed_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,114 @@
-"""Classes and functions to parse output from btrfs-progs commands."""
-import re
-from pathlib import Path, PurePath
-from typing import Self,TypedDict,Required
+"""Classes and constants to aid in casting SubvolumeInfo objects."""
+from pathlib import PurePath
+from typing import Self
 from datetime import datetime
 from uuid import UUID
 from dataclasses import dataclass
 
+from btrfsutil import SubvolumeInfo
+
+UUIDS = {"uuid": "UUID",
+         "parent_uuid": "Parent UUID",
+         "received_uuid": "Received UUID"}
+
+TIMES = {"otime": "Creation time",
+         "rtime": "Receieve time",
+         "stime": "Send time",
+         "ctime": None}
+
+GENS = {"generation": "Generation",
+        "otransid": "Gen at creation",
+        "rtransid": "Receive transid",
+        "stransid": "Send transid",
+        "ctransid": None}
+
+INTS = {"id": "Subvolume ID",
+        "parent_id": "Parent ID",
+        "dir_id": None,
+        "flags": "Flags"}
+
+OTHER = {"name": "Name",
+         "path": "Path"}
+
+BTRDICT = {v:k for k,v in (UUIDS | TIMES | GENS | INTS | OTHER).items() if v}
+BASE = {k:v for k,v in BTRDICT.items() if v in ("name","id","uuid")}
+
 @dataclass
 class Generation:
     """A class representing a btrfs generation"""
     generation: int
 
     def __lt__(self, other: Self):
         return self.generation < other.generation
 
-BtrDict = TypedDict("BtrDict", {
-    "btrfs Path": PurePath,
-    "Name": Required[str],
-    "Subvolume ID": Required[str],
-    "UUID": Required[UUID],
-    "Parent UUID": UUID | None,
-    "Received UUID": UUID | None,
-    "Creation time": datetime,
-    "Send time": datetime,
-    "Receive time":datetime | None,
-    "Generation": Generation,
-    "Gen at creation": Generation,
-    "Parent ID": str,
-    "Top level ID": str,
-    "Flags": str,
-    "Send transid": str,
-    "Receive transid": str,
-    }, total = False)
-
-class BtrfsDict:
-    """Class to cast a btrfs dictionary to the correct python types"""
-    def __init__(self, str_dict: dict[str, str]):
-        self._str_dict = str_dict
-        self.btr_dict = self.cast_dict(str_dict)
+@dataclass(frozen=True)
+class BaseInfo:
+    name: str
+    id: int
+    uuid: UUID
 
-    @staticmethod
-    def cast(dict_key: str, dict_value: str):
-        """Cast a string to its proper python type"""
-        if dict_value == "-":
+    @classmethod
+    def from_deleted(cls, suuid: str) -> "BaseInfo":
+        uuid = UUID(suuid)
+        bi = BaseInfo(suuid, uuid.int, uuid)
+        return bi
+
+    def __getitem__(self, key):
+        if key in BASE:
+            return getattr(self, BTRDICT[key])
+        else:
             return None
-        match dict_key:
-            case "Creation Time"|"Send Time"|"Receive Time":
-                return datetime.fromisoformat(dict_value)
-            case "UUID"|"Received UUID"| "Parent UUID":
-                return UUID(dict_value)
-            case "Generation"|"Gen at Creation":
-                return Generation(int(dict_value))
-            case "btrfs Path":
-                return PurePath(dict_value)
-            case _:
-                return dict_value
 
-    @classmethod
-    def cast_dict(cls, str_dict: dict[str,str]):
-        """Casts the inputed dictionary into a properly typed btrfs dictionary"""
-        new_dict = {}
-        for key,val in str_dict.items():
-            new_dict[key] = cls.cast(key,val)
-        return new_dict
+@dataclass(frozen=True)
+class TypedInfo(BaseInfo):
+    """A wrapper around SubvolumeInfo that adds type hints and convenience methods"""
+    name: str
+    path: PurePath
+    id: int
+    parent_id: int
+    dir_id: int
+    flags: int
+    uuid: UUID
+    parent_uuid: UUID
+    received_uuid: UUID
+    generation: Generation
+    ctransid: Generation
+    otransid: Generation
+    stransid: Generation
+    rtransid: Generation
+    ctime: datetime
+    otime: datetime
 
     @classmethod
-    def from_list(cls, list_str: str) -> Self:
-        """Turns output from `btrfs subvolume list` command into a list of subvolumes"""
-        keys = "ID,gen,cgen,parent,parent_uuid,received_uuid,uuid".split(",")
-        vals = "Subvolume ID,Generation,Gen at creation,Parent ID,Parent UUID,Received UUID,UUID".split(",")
-        key_dict = {key:val for key,val in zip(keys,vals)}
-        str_dict = {}
-        for key,val in key_dict.items():
-            match = re.search(f"\\b{key}\\s+(\\S+)", list_str)
-            if match :
-                str_dict[val] = match.group(1)
-        path_match = re.search(r"path\s*(.*)",list_str).group(1).removeprefix("<FS_TREE>/")
-        str_dict["btrfs Path"] = Path(f"/{path_match}")
-        str_dict["Name"] = str_dict["btrfs Path"].name
-        return cls(str_dict)
+    def from_info(cls, path: str, info: SubvolumeInfo):
+        kw_args = {}
+        kw_args["path"] = PurePath("/" + path)
+        kw_args["name"] = kw_args["path"].name or "<FS_TREE>"
+        for attr in info.__match_args__:
+            val = getattr(info, attr)
+            kw_args[attr] = cls._cast(attr, val)
+        return cls(**kw_args)
 
     @classmethod
-    def from_show(cls, show_text: str) -> Self:
-        """Creates btrfs prop dict based on the output of btrfs subvolume show."""
-        str_dict: dict[str,str] = {}
-        lines = show_text.splitlines()
-        str_dict["btrfs Path"] = ("/" + lines[0]).replace("//","/")
-        for line in lines[1:]:
-            if re.search(r":\s+",line):
-                k,v = line.split(":",maxsplit=1)
-                k = k.strip()
-                v = v.strip()
-                str_dict[k] = v
-        return cls(str_dict)
+    def _cast(cls, key: str, value: str|int|bytes) -> None | datetime | UUID | Generation | str:
+        """Cast a string to its proper python type"""
+        if key in TIMES:
+            return datetime.fromtimestamp(value) if value else None
+        elif key in UUIDS:
+            value = value.hex()
+            return UUID(value) if value != "0"*32 else None
+        elif key in GENS:
+            return Generation(value) if value else None
+        elif key in INTS:
+            return int(value)
+        else:
+            raise KeyError(f"{key = } can't be cast")
+
+    def __getitem__(self, key: str):
+        if key in BTRDICT:
+            return getattr(self, BTRDICT[key])
+        else:
+            #returns None instead of raising an error
+            #makes it slightly easier to use with Subvolume
+            return None 
 
-    @classmethod
-    def from_deleted(cls, uuid: str) -> Self:
-        """Creates a btrfs prop dict from a UUID"""
-        str_dict = {"UUID":uuid,"Name":uuid,"Subvolume ID":uuid}
-        return cls(str_dict)
```

### Comparing `btrview-0.6.3/btrview/btrfs.py` & `btrview-0.7.0/btrview/btrfs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Classes and functions to interact with a btrfs filesystem."""
 import json
 from collections import defaultdict
 from pathlib import Path, PurePath
 from typing import Self, Callable, TypeAlias, Iterable
 
 from treelib import Tree
+import btrfsutil
 
 from btrview.utils import run
 from btrview.subvolume import Subvolume, Mount
 
 Sieve: TypeAlias = Callable[[Subvolume], bool]
 
 class SubvolumeSieve:
@@ -79,17 +80,16 @@
         #preventing direct access to the set object
         return tuple(self._all_mounts[self.uuid])
 
     @property
     def default_subvolume(self) -> str:
         """Return the default subvolume for the filesystem"""
         mount = self.mounts[0]
-        out = run(f"btrfs subvolume get-default {mount.target}")
-        subvol_id = out.stdout.split()[1]
-        return subvol_id
+        default = btrfsutil.get_default_subvolume(mount.target)
+        return str(default)
 
     @classmethod
     def get_filesystems(cls, labels:list[str] | None = None) -> list[Self]:
         """Returns a list of each filesystem on the system."""
         #had to be here in case nothing gets initialized
         if not cls._UUIDs:
             cls._get_mounts() 
@@ -100,44 +100,60 @@
                 filesystems.append(fs)
         return filesystems
 
     @classmethod
     def _get_deleted_subvols(cls, subvols: list[Subvolume]) -> list[Subvolume]:
         """Returns a list of deleted subvolumes"""
         uuids: set[str] = {s.id("snap") for s in subvols}
-        puuids: set[str] = {s.parent("snap") for s in subvols if s.parent("snap")}
+        puuids: set[str | None] = {s.parent("snap") for s in subvols if s.parent("snap")}
         deleted_puuids = puuids - uuids
         deleted_subvols = [Subvolume.from_deleted(puuid) for puuid in deleted_puuids]
         return deleted_subvols
 
-    def _parse_subvol_list(self, list_str: str) -> list[Subvolume]:
-        """Turns output from `btrfs subvolume list` command into a list of subvolumes"""
-        list_lines = list_str.splitlines()
-        return [Subvolume.from_list(line, self.mounts) for line in list_lines]
+    def _subvol_info_iter(self,) -> list[Subvolume]:
+        """Returns a list of subvolume from a SubvolumeIterator"""
+        subvol_iter = btrfsutil.SubvolumeIterator(self.mounts[0].target,info = True, top=5)
+        subvols = []
+        for path, info in subvol_iter:
+            subvol = Subvolume.from_info(path, info, self.mounts)
+            subvols.append(subvol)
+        return subvols
 
     def subvolumes(self, remove: tuple[str, ...]) -> list[Subvolume]:
         """Return a list of subvolumes on the file system"""
         mount_point = self.mounts[0].target 
-        subvols = [] if "root" in remove else [Subvolume.from_ID("5",mount_point, self.mounts)]
-        out = run(f"sudo btrfs subvolume list -apcguqR {mount_point}")
-        subvols.extend(self._parse_subvol_list(out.stdout))
+        subvols = [] if "root" in remove else [Subvolume.from_ID(mount_point,5, self.mounts)]
+        subvols.extend(self._subvol_info_iter())
         subvols.extend(self._get_deleted_subvols(subvols))
         sieve = SubvolumeSieve(subvols)
 
         return sieve.sieve_str(remove)
 
     def forest(self, snapshots: bool, remove: tuple[str, ...]) -> list[Tree]:
         """Returns a forest of subvolumes with parent/child relationships
         being based on subvolume layout or snapshots."""
         kind = "snap" if snapshots else "subvol"
         return get_forest(self.subvolumes(remove), kind)
         
     def __str__(self) -> str:
         return f"{self.label or self.uuid}"
 
+    @staticmethod
+    def is_btrfs(path: Path | str) -> bool:
+        """Returns true if path is part of a btrfs filesystem."""
+        path = Path(path)
+        if not path.exists():
+            raise FileNotFoundError(f"{path} doesn't exist.")
+        try:
+            btrfsutil.subvolume_info(path)
+        except btrfsutil.BtrfsUtilError as e:
+            if e.btrfsutilerror == btrfsutil.ERROR_NOT_BTRFS:
+                return False
+        return True
+
 def subvol_in_list(ID: str, subvolumes: list[Subvolume], kind = "subvol") -> Subvolume | None:
     """Returns a subvolume from a list if there, else returns None."""
     for subvolume in subvolumes:
         if subvolume.id(kind) == ID:
             return subvolume
     return None
```

### Comparing `btrview-0.6.3/btrview/rich_output.py` & `btrview-0.7.0/btrview/rich_output.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.3/btrview/scripts/btrview.py` & `btrview-0.7.0/btrview/scripts/btrview.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.3/btrview/subvolume.py` & `btrview-0.7.0/btrview/subvolume.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 """Subvolume Classes and errors."""
 from pathlib import Path, PurePath
 from typing import Self
 from dataclasses import dataclass
 
-from btrview.utils import run
-from btrview.btr_dict import BtrDict, BtrfsDict
+from btrfsutil import SubvolumeInfo, subvolume_info, subvolume_path
+from btrview.typed_info import BaseInfo, TypedInfo, BTRDICT, BASE
 
 class NotASubvolumeError(NotADirectoryError):
     """Throw when a directory isn't a subvolume"""
 
 @dataclass(frozen=True)
 class Mount:
     """Basic class for working with mounted subvolumes."""
     fsroot: PurePath
     target: Path
 
-    def resolve(self, path: Path) -> Path:
+    def resolve(self, path: PurePath) -> Path:
         """Returns the resolved path of another path"""
         fsroot_str = str(self.fsroot)
         target_str = str(self.target)
         if fsroot_str == "/":
             target_str = target_str + "/"
         path_str = str(path)
         new_path = path_str.replace(fsroot_str,target_str,1).replace("//","/",1)
         return Path(new_path)
 
     def __str__(self) -> str:
         return f"{self.fsroot} on {self.target}"
 
 class Subvolume:
     """Class representing a btrfs subvolume"""
-    def __init__(self, props: BtrDict, mounts: tuple[Mount, ...],
-                 deleted: bool = False, show: bool = False) -> None:
-        self.props = props
+    def __init__(self, 
+                 info: BaseInfo, 
+                 mounts: tuple[Mount, ...],
+                 deleted = False) -> None:
+        self.info = info
         self.mounts = mounts
         self.deleted = deleted
-        self._show = show
 
     @property
-    def paths(self) -> list[Path]:
+    def fs_paths(self) -> list[Path]:
         """Returns all the reachable paths of the Subvolume"""
-        if self["btrfs Path"] is None:
+        if self["Path"] is None:
             return []
-        btr_path = Path(self["btrfs Path"])
+        btr_path = self["Path"]
         paths = [mount.resolve(btr_path) for mount in self.mounts if btr_path.is_relative_to(mount.fsroot)]
         paths = [path for path in paths if path.exists()]
         return paths
 
     @property
     def mounted(self) -> bool:
         """Returns whether the subvolume is reachable via the filesystem"""
-        return bool(self.paths)
+        return bool(self.fs_paths)
 
     @property
     def root_subvolume(self) -> bool:
         """Returns whether the subvolume is the root_subvolume"""
         return self["Subvolume ID"] == "5"
 
     @property
@@ -62,21 +63,21 @@
         """Returns whether the subvolume is a snapshot"""
         return bool(self["Parent UUID"])
 
     @property
     def mount_points(self) -> tuple[Path, ...]:
         """Returns mount points of Subvolume"""
         targets = [mount.target for mount in self.mounts]
-        return tuple(path for path in self.paths if path in targets)
+        return tuple(path for path in self.fs_paths if path in targets)
 
     def parent(self, p_type: str) -> str | None:
         """Returns parent UUID or ID string"""
         match p_type:
             case "snap":
-                parent = self["Received UUID"] or self["Parent UUID"]
+                parent = self["Parent UUID"]
             case "subvol":
                 parent = self["Parent ID"]
             case _:
                 parent = None
         return parent
 
     def id(self, p_type: str) -> str:
@@ -87,82 +88,50 @@
             case "subvol":
                 ID = self["Subvolume ID"]
             case _:
                 ID = self["UUID"]
         return ID
 
     @classmethod
-    def from_UUID(cls, uuid: str, path: str | Path, mounts: tuple[Mount, ...]) -> Self:
-        """Creates subvolume from the subvolumes UUID and any path on the filesystem"""
-        cmd = f"btrfs subvolume show -u {uuid} {path}"
-        props = cls._run_cmd(cmd)
-        return cls(props, mounts, show = True)
+    def from_info(cls, path: str, info: SubvolumeInfo, mounts: tuple[Mount, ...]) -> Self:
+        t_info = TypedInfo.from_info(path, info)
+        return cls(t_info, mounts)
 
     @classmethod
-    def from_ID(cls, ID: str, path: str | Path, mounts: tuple[Mount, ...]) -> Self:
+    def from_ID(cls, path: str | Path, subvol_id: int, mounts: tuple[Mount, ...]) -> Self:
         """Creates subvolume from subvolume's ID and any path on the filesystem"""
-        cmd = f"btrfs subvolume show -r {ID} {path}"
-        props = cls._run_cmd(cmd)
-        return cls(props, mounts, show = True)
+        info = subvolume_info(path, subvol_id)
+        btrfs_path = subvolume_path(path, subvol_id)
+        return cls.from_info(btrfs_path, info, mounts)
 
     @classmethod
-    def from_list(cls, list_str: str, mounts: tuple[Mount, ...]) -> Self:
-        props = BtrfsDict.from_list(list_str).btr_dict
-        return cls(props, mounts)
-
-    @classmethod
-    def from_deleted(cls, UUID: str) -> Self:
-        """Creates subvolume from subvolume's ID and any path on the filesystem"""
-        props: BtrDict = {"UUID":UUID,"Subvolume ID":UUID, "Name":UUID}
-        return cls(props, tuple(), deleted=True)
-
-    @classmethod
-    def _run_cmd(cls, cmd: str) -> BtrDict:
-        """Runs the shell command and returns the prop dictionary
-        if the command doesn't error"""
-        out = run(cmd)
-        if out.returncode != 0:
-            raise NotASubvolumeError
-        props = BtrfsDict.from_show(out.stdout).btr_dict
-        return props
-
-    @staticmethod
-    def is_btrfs(path: Path) -> bool:
-        """Returns true if path is part of a btrfs filesystem."""
-        response = run(f"btrfs filesystem usage '{path}'")
-        return response.returncode == 0
+    def from_deleted(cls, uuid: str):
+        info = TypedInfo.from_deleted(str(uuid))
+        return cls(info, (), True)
 
     def __getitem__(self, key: str) -> str | None:
-        """Returns the item from the props dictionary, but instead
-        of throwing a key error, returns None"""
-        if key in self.props:
-            return self.props[key]
-        elif self.deleted:
-            #just assume it's None for deleted subvols. #could cause problems
-            #in that deleted Subvolumes won't throw KeyError
-            return None
-        elif not self._show:
-            cmd = f"btrfs subvolume show -u {self['UUID']} {self.mounts[0].target}"
-            props = self._run_cmd(cmd)
-            self.props |= props
-            self._show = True
-        try:
-            return self.props[key]
-        except KeyError:
-            pass
-        try:
-            return getattr(self, key)
-        except AttributeError:
-            raise KeyError(f"Subvolume has no attribute or key '{key}'")
+        """Returns the item from TypedInfo object."""
+        if key in BTRDICT:
+            if not self.deleted:
+                return self.info[key]
+            else:
+                return self.info[key] if key in BASE else None
+        else:
+            try:
+                return getattr(self, key)
+            except AttributeError:
+                raise KeyError(f"Subvolume has no attribute or key '{key}'")
 
     def __str__(self) -> str:
         string = self["Name"]
         if mps := self.mount_points:
             mp_string = ", ".join(str(mp) for mp in mps)
             string = f"{string} on: {mp_string}"
         return str(string)
 
     def __hash__(self) -> int:
         return hash(self["UUID"])
 
     def __eq__(self, other) -> bool:
         return self["UUID"] == other["UUID"]
+
+
```

### Comparing `btrview-0.6.3/btrview/utils.py` & `btrview-0.7.0/btrview/utils.py`

 * *Files identical despite different names*

### Comparing `btrview-0.6.3/btrview.egg-info/PKG-INFO` & `btrview-0.7.0/btrview.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btrview
-Version: 0.6.3
+Version: 0.7.0
 Summary: View btrfs snapshot trees
 Author: Chris Copley
 License: MIT License
         
         Copyright (c) 2024 Chris Copley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -63,17 +63,17 @@
 
 Btrview relies on the following dependencies:
 * python 3.11 or greater
 * btrfs-progs
 * python-treelib
 * python-rich
 
-If you have pip installed you can grab btrview from the python package index with `pip install btrview`. Using pip to install btrview will also install the required python dependencies. In addition installing via pip will add the `btrview` command to your path allowing you to run the command from anywhere on the system. 
+The easiest way to download btrview is to use [pipx](https://pipx.pypa.io/stable/installation/) to download it from the python package index. Use the command `pipx --system-site-packages install btrview`. Using pipx to install btrview will also install the required python dependencies and add the `btrview` command to your path allowing you to run the command from anywhere on the system.
 
-If you don't feel like installing via pip you can download it via `git clone https://github.com/CopOnTheRun/btrview` then `cd btrview`. From within the btrview directory you can run the script with `python -m btrview`. Note that if you clone the repository you'll need to make sure you have all the dependencies installed already.
+If you don't feel like installing via pipx you can download it via `git clone https://github.com/CopOnTheRun/btrview` then `cd btrview`. From within the btrview directory you can run the script with `python -m btrview`. Note that if you clone the repository you'll need to make sure you have all the dependencies installed already.
 
 ## Some Qs and As:
 
 ### Q: What is btrfs?
 
 In short, it's a copy on write (COW) filesystem. If you're not already using btrfs, then check out the [documentation](https://btrfs.readthedocs.io/en/latest/) to see if it's something you'd be interested in.
```

### Comparing `btrview-0.6.3/pyproject.toml` & `btrview-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "btrview"
-version = "0.6.3"
+version = "0.7.0"
 description = "View btrfs snapshot trees"
 readme = "README.md"
 authors = [{name = "Chris Copley"}]
 license = {file = "LICENSE.md"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 Issues = "https://github.com/CopOnTheRun/btrview/issues"
 
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.bumpver]
-current_version = "0.6.3"
+current_version = "0.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```


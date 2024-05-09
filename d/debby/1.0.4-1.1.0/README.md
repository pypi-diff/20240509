# Comparing `tmp/debby-1.0.4.tar.gz` & `tmp/debby-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debby-1.0.4.tar", max compression
+gzip compressed data, was "debby-1.1.0.tar", max compression
```

## Comparing `debby-1.0.4.tar` & `debby-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2024-05-07 16:48:05.045505 debby-1.0.4/LICENSE
--rw-r--r--   0        0        0     4859 2024-05-07 16:48:05.045505 debby-1.0.4/README.md
--rw-r--r--   0        0        0      301 2024-05-07 16:48:05.045505 debby-1.0.4/debby/__init__.py
--rw-r--r--   0        0        0      739 2024-05-07 16:48:05.045505 debby-1.0.4/debby/__main__.py
--rw-r--r--   0        0        0     6592 2024-05-07 16:48:05.045505 debby-1.0.4/debby/args.py
--rw-r--r--   0        0        0     2263 2024-05-07 16:48:05.045505 debby-1.0.4/debby/control_file.py
--rw-r--r--   0        0        0      383 2024-05-07 16:48:05.045505 debby-1.0.4/debby/exceptions.py
--rw-r--r--   0        0        0     1781 2024-05-07 16:48:05.045505 debby-1.0.4/debby/files.py
--rw-r--r--   0        0        0      165 2024-05-07 16:48:05.045505 debby-1.0.4/debby/meta/__init__.py
--rw-r--r--   0        0        0     1218 2024-05-07 16:48:05.045505 debby-1.0.4/debby/meta/meta.py
--rw-r--r--   0        0        0     2543 2024-05-07 16:48:05.045505 debby-1.0.4/debby/meta/meta_loader.py
--rw-r--r--   0        0        0      702 2024-05-07 16:48:05.045505 debby-1.0.4/debby/meta/meta_loader_factory.py
--rw-r--r--   0        0        0      883 2024-05-07 16:48:05.045505 debby-1.0.4/debby/meta/poetry_meta_loader.py
--rw-r--r--   0        0        0     1992 2024-05-07 16:48:05.045505 debby-1.0.4/debby/meta/pyproject_meta_loader.py
--rw-r--r--   0        0        0      986 2024-05-07 16:48:05.045505 debby-1.0.4/debby/package.py
--rw-r--r--   0        0        0        1 2024-05-07 16:48:05.045505 debby-1.0.4/debby/py.typed
--rw-r--r--   0        0        0      784 2024-05-07 16:48:13.917478 debby-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     5753 1970-01-01 00:00:00.000000 debby-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-09 09:23:41.666567 debby-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4859 2024-05-09 09:23:41.666567 debby-1.1.0/README.md
+-rw-r--r--   0        0        0      301 2024-05-09 09:23:41.666567 debby-1.1.0/debby/__init__.py
+-rw-r--r--   0        0        0      739 2024-05-09 09:23:41.666567 debby-1.1.0/debby/__main__.py
+-rw-r--r--   0        0        0     7792 2024-05-09 09:23:41.666567 debby-1.1.0/debby/args.py
+-rw-r--r--   0        0        0     2263 2024-05-09 09:23:41.666567 debby-1.1.0/debby/control_file.py
+-rw-r--r--   0        0        0      383 2024-05-09 09:23:41.666567 debby-1.1.0/debby/exceptions.py
+-rw-r--r--   0        0        0     2449 2024-05-09 09:23:41.666567 debby-1.1.0/debby/files.py
+-rw-r--r--   0        0        0      165 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/__init__.py
+-rw-r--r--   0        0        0     1210 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/meta.py
+-rw-r--r--   0        0        0     2543 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/meta_loader.py
+-rw-r--r--   0        0        0      702 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/meta_loader_factory.py
+-rw-r--r--   0        0        0      883 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/poetry_meta_loader.py
+-rw-r--r--   0        0        0     1992 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/pyproject_meta_loader.py
+-rw-r--r--   0        0        0      986 2024-05-09 09:23:41.666567 debby-1.1.0/debby/package.py
+-rw-r--r--   0        0        0        1 2024-05-09 09:23:41.666567 debby-1.1.0/debby/py.typed
+-rw-r--r--   0        0        0      784 2024-05-09 09:23:50.546504 debby-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5753 1970-01-01 00:00:00.000000 debby-1.1.0/PKG-INFO
```

### Comparing `debby-1.0.4/LICENSE` & `debby-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `debby-1.0.4/README.md` & `debby-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `debby-1.0.4/debby/__main__.py` & `debby-1.1.0/debby/__main__.py`

 * *Files identical despite different names*

### Comparing `debby-1.0.4/debby/args.py` & `debby-1.1.0/debby/args.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from argparse import ArgumentParser
 from dataclasses import dataclass
+from importlib import metadata
 from pathlib import Path
 from typing import Any, Literal, Optional, Sequence, Tuple, Union
 
 from typing_extensions import Self
 
 
 @dataclass
@@ -36,156 +37,167 @@
     @classmethod
     def parse(cls, argv: Optional[Sequence[str]] = None) -> Self:
         parser = ArgumentParser()
         parser.add_argument(
             "-f",
             "--file",
             dest="files",
-            help="Path to the files to package. Can be passed multiple times. E.g. --file SOURCE1 DESTINATION1 --file SOURCE2 DESTINATION2. Sources must point to existing files or directories and destinations will be treated as relative to the package root.",
+            help="Path to the files/directories to package. Can be passed multiple times. E.g. --file SOURCE1 DESTINATION1 --file SOURCE2 DESTINATION2. Sources must point to existing files or directories and destinations will be treated as relative to the package root. You may also choose to not use this flag and copy the files manually to the output directory.",
             type=Path,
             nargs=2,
             action="append",
             default=[],
+            metavar=("SOURCE", "DESTINATION"),
         )
         parser.add_argument(
             "-t",
             "--template",
-            help="Path to the control file template",
+            help="Path to a control file template to use instead of generating one from scratch. This file may contain placeholders such as {meta.name} and {meta.version}. See the documentation for more information. https://abrahammurciano.github.io/debby",
             type=Path,
         )
         parser.add_argument(
             "-o",
             "--out-dir",
-            help="Path to the output directory",
+            help="Path to the output directory. Defaults to debian/build.",
             type=Path,
             default=Path("debian/build"),
         )
         parser.add_argument(
             "--no-size",
-            help="Do not include the total size of the package in the control file",
+            help="Do not include the total size of the package in the control file.",
             action="store_true",
         )
         cls._add_meta_source_group(parser)
         cls._add_meta_override_args(parser)
+        parser.add_argument(
+            "-V",
+            action="version",
+            help="Print the version and exit.",
+            version=metadata.version((__package__ or "debby").split(".", 1)[0]),
+        )
         return cls(**vars(parser.parse_args(argv)))
 
     @classmethod
     def _add_meta_source_group(cls, parser: ArgumentParser) -> None:
-        meta_source_group = parser.add_mutually_exclusive_group(required=True)
+        meta_source_group = parser.add_mutually_exclusive_group()
         meta_source_group.add_argument(
             "--pyproject",
-            help="Read metadata according to PEP 621 from the given pyproject.toml file",
+            help="Read metadata according to PEP 621 from ./pyproject.toml, or the given file if specified.",
             type=Path,
-            metavar="pyproject.toml",
+            metavar="PYPROJECT_FILE",
+            nargs="?",
+            const=Path("pyproject.toml"),
         )
         meta_source_group.add_argument(
             "--poetry",
-            help="Read poetry metadata from the given pyproject.toml file",
+            help="Read poetry metadata from the ./pyproject.toml file, or the given file if specified.",
             type=Path,
-            metavar="pyproject.toml",
+            metavar="PYPROJECT_FILE",
+            nargs="?",
+            const=Path("pyproject.toml"),
         )
 
     @classmethod
     def _add_meta_override_args(cls, parser: ArgumentParser) -> None:
         meta_overrides_group = parser.add_argument_group(
             "Metadata Overrides",
             "Override metadata fields. Environment variables such as DEBBY_META_VERSION can be used to set these fields.",
         )
         meta_overrides_group.add_argument(
             "-n",
             "--name",
-            help="Specify the package name",
+            help="Specify the package name.",
             default=os.environ.get("DEBBY_META_NAME"),
         )
         meta_overrides_group.add_argument(
             "-s",
             "--source",
-            help="Specify the package source",
+            help="Specify the package source.",
             default=os.environ.get("DEBBY_META_SOURCE"),
         )
         meta_overrides_group.add_argument(
             "-v",
             "--version",
-            help="Specify the package version",
+            help="Specify the package version.",
             default=os.environ.get("DEBBY_META_VERSION"),
         )
         meta_overrides_group.add_argument(
             "--section",
-            help="Specify the package section",
+            help="Specify the package section. For example, 'misc' or 'python'.",
             default=os.environ.get("DEBBY_META_SECTION"),
         )
         meta_overrides_group.add_argument(
             "-p",
             "--priority",
-            help="Specify the package priority",
+            help="Specify the package priority. Usually 'optional'.",
             default=os.environ.get("DEBBY_META_PRIORITY"),
         )
         meta_overrides_group.add_argument(
             "-a",
             "--architecture",
-            help="Specify the package architecture",
-            default=os.environ.get("DEBBY_META_ARCHITECTURE"),
+            help="Specify the package architecture. Defaults to 'all'.",
+            default=os.environ.get("DEBBY_META_ARCHITECTURE", "all"),
         )
         meta_overrides_group.add_argument(
             "-e",
             "--essential",
             choices=["yes", "no"],
-            help="Specify whether the package is essential",
+            help="Specify whether the package is essential.",
             default=os.environ.get("DEBBY_META_ESSENTIAL"),
         )
         meta_overrides_group.add_argument(
             "-m",
             "--maintainer",
-            help="Specify the package maintainer",
+            help="Specify the package maintainer. For example, 'John Doe <john.doe@example.com>'.",
             default=os.environ.get("DEBBY_META_MAINTAINER"),
         )
         meta_overrides_group.add_argument(
             "-d",
             "--description",
-            help="Specify the package description",
+            help="Specify the package description.",
             default=os.environ.get("DEBBY_META_DESCRIPTION"),
         )
         meta_overrides_group.add_argument(
             "--homepage",
-            help="Specify the package homepage",
+            help="Specify the package homepage.",
             default=os.environ.get("DEBBY_META_HOMEPAGE"),
         )
         cls._add_dependencies_args(meta_overrides_group)
 
     @classmethod
     def _add_dependencies_args(cls, parser: Union[ArgumentParser, Any]) -> None:
         parser.add_argument_group("Dependencies", "Specify package dependencies")
         parser.add_argument(
             "--depends",
-            help="Specify package dependencies",
+            help="Specify packages that your package depends on. For example, 'python3, python3-requests (>= 2.24)'.",
             default=os.environ.get("DEBBY_META_DEPENDS"),
         )
         parser.add_argument(
             "--pre-depends",
-            help="Specify package pre-dependencies",
+            help="Specify packages that must be installed before your package is installed.",
             default=os.environ.get("DEBBY_META_PRE_DEPENDS"),
         )
         parser.add_argument(
             "--recommends",
-            help="Specify package recommendations",
+            help="Specify packages that are recommended but not strictly required for your package.",
             default=os.environ.get("DEBBY_META_RECOMMENDS"),
         )
         parser.add_argument(
             "--suggests",
-            help="Specify package suggestions",
+            help="Specify packages that are suggested but not required for your package.",
             default=os.environ.get("DEBBY_META_SUGGESTS"),
         )
         parser.add_argument(
             "--enhances",
-            help="Specify package enhancements",
+            help="Specify packages that your package enhances.",
             default=os.environ.get("DEBBY_META_ENHANCES"),
         )
         parser.add_argument(
             "--breaks",
-            help="Specify package breaks",
+            help="Specify packages that your package breaks.",
             default=os.environ.get("DEBBY_META_BREAKS"),
         )
         parser.add_argument(
             "--conflicts",
-            help="Specify package conflicts",
+            help="Specify packages that your package conflicts with.",
             default=os.environ.get("DEBBY_META_CONFLICTS"),
         )
```

### Comparing `debby-1.0.4/debby/control_file.py` & `debby-1.1.0/debby/control_file.py`

 * *Files identical despite different names*

### Comparing `debby-1.0.4/debby/files.py` & `debby-1.1.0/debby/files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import shutil
 from functools import cached_property
 from pathlib import Path
 from typing import Iterable, Iterator, Mapping, Tuple
 
 
 class Files(Mapping[Path, Path]):
     """A mapping of target paths in the package to source paths on the filesystem.
@@ -21,40 +22,55 @@
                 "source files must all exist and destination paths must all be relative"
             )
 
     def package(self, path: Path) -> None:
         for dst, src in self.items():
             target = path / dst
             target.parent.mkdir(parents=True, exist_ok=True)
-            target.symlink_to(src)
-
-    @classmethod
-    def _normalize_files(
-        cls, files: Iterable[Tuple[Path, Path]]
-    ) -> Mapping[Path, Path]:
-        return {
-            dst.relative_to(dst.anchor) if dst.is_absolute() else dst: src
-            for src, dst in files
-        }
+            if src.is_dir():
+                shutil.copytree(src, target)
+            else:
+                shutil.copy2(src, target)
 
     @property
     def sources(self) -> Iterable[Path]:
         return self._files.values()
 
     @property
     def destinations(self) -> Iterable[Path]:
         return self._files.keys()
 
     @cached_property
     def total_size(self) -> int:
         return sum(
-            (max(f.resolve().stat().st_size, 1024) // 1024) * 1024 for f in self.sources
+            self._size_of(path) for source in self.sources for path in source.rglob("*")
         )
 
     def __getitem__(self, key: Path) -> Path:
         return self._files[key]
 
     def __iter__(self) -> Iterator[Path]:
         return iter(self._files)
 
     def __len__(self) -> int:
         return len(self._files)
+
+    @classmethod
+    def _normalize_files(
+        cls, files: Iterable[Tuple[Path, Path]]
+    ) -> Mapping[Path, Path]:
+        return {
+            dst.relative_to(dst.anchor) if dst.is_absolute() else dst: src
+            for src, dst in files
+        }
+
+    @classmethod
+    def _size_of(cls, path: Path) -> int:
+        """Get the size of a filesystem object for the Installed-Size field in the control file.
+
+        The disk space is given as the accumulated size of each regular file and symlink rounded to 1 KiB used units, and a baseline of 1 KiB for any other filesystem object type.
+
+        https://www.debian.org/doc/debian-policy/ch-controlfields.html#s-f-installed-size
+        """
+        if path.is_file():
+            return max(1024, (path.stat().st_size // 1024) * 1024)
+        return 1024
```

### Comparing `debby-1.0.4/debby/meta/meta.py` & `debby-1.1.0/debby/meta/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class Meta:
     """Metadata for a Debian package."""
 
     name: str
     version: str
     maintainer: str
     description: str
-    architecture: str = "all"
+    architecture: str
     source: Optional[str] = None
     section: Optional[str] = None
     priority: Optional[str] = None
     essential: Optional[Literal["yes", "no"]] = None
     homepage: Optional[str] = None
     depends: Optional[str] = None
     pre_depends: Optional[str] = None
```

### Comparing `debby-1.0.4/debby/meta/meta_loader.py` & `debby-1.1.0/debby/meta/meta_loader.py`

 * *Files identical despite different names*

### Comparing `debby-1.0.4/debby/meta/meta_loader_factory.py` & `debby-1.1.0/debby/meta/meta_loader_factory.py`

 * *Files identical despite different names*

### Comparing `debby-1.0.4/debby/meta/poetry_meta_loader.py` & `debby-1.1.0/debby/meta/poetry_meta_loader.py`

 * *Files identical despite different names*

### Comparing `debby-1.0.4/debby/meta/pyproject_meta_loader.py` & `debby-1.1.0/debby/meta/pyproject_meta_loader.py`

 * *Files identical despite different names*

### Comparing `debby-1.0.4/debby/package.py` & `debby-1.1.0/debby/package.py`

 * *Files identical despite different names*

### Comparing `debby-1.0.4/pyproject.toml` & `debby-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "debby"
 # Version is overwritten at build time by CI based on git tag
-version = "1.0.4"
+version = "1.1.0"
 description = "Create .deb files easily using python package metadata"
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/debby"
 documentation = "https://abrahammurciano.github.io/debby/debby"
 keywords = []
```

### Comparing `debby-1.0.4/PKG-INFO` & `debby-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debby
-Version: 1.0.4
+Version: 1.1.0
 Summary: Create .deb files easily using python package metadata
 Home-page: https://github.com/abrahammurciano/debby
 License: GPLv3
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```


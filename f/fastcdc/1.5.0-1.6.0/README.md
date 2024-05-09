# Comparing `tmp/fastcdc-1.5.0.tar.gz` & `tmp/fastcdc-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastcdc-1.5.0.tar", max compression
+gzip compressed data, was "fastcdc-1.6.0.tar", max compression
```

## Comparing `fastcdc-1.5.0.tar` & `fastcdc-1.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1824 2020-06-27 15:59:31.291723 fastcdc-1.5.0/build.py
--rw-r--r--   0        0        0       18 2020-05-23 20:10:03.765326 fastcdc-1.5.0/fastcdc/.gitignore
--rw-r--r--   0        0        0      277 2023-03-13 16:39:52.421869 fastcdc-1.5.0/fastcdc/__init__.py
--rw-r--r--   0        0        0     2210 2020-06-27 15:59:31.293723 fastcdc-1.5.0/fastcdc/benchmark.py
--rw-r--r--   0        0        0     1841 2020-06-27 15:59:31.293723 fastcdc-1.5.0/fastcdc/chunkify.py
--rw-r--r--   0        0        0      533 2020-06-27 15:59:31.294725 fastcdc-1.5.0/fastcdc/cli.py
--rw-r--r--   0        0        0     5159 2020-05-09 21:30:49.474779 fastcdc-1.5.0/fastcdc/const.py
--rw-r--r--   0        0        0     7364 2020-09-30 08:03:13.670476 fastcdc-1.5.0/fastcdc/fastcdc_cy.pyx
--rw-r--r--   0        0        0     7558 2020-08-08 17:36:46.435239 fastcdc-1.5.0/fastcdc/fastcdc_py.py
--rw-r--r--   0        0        0     3457 2020-05-24 10:11:17.155062 fastcdc-1.5.0/fastcdc/original.py
--rw-r--r--   0        0        0     3055 2020-09-30 07:42:31.654173 fastcdc-1.5.0/fastcdc/scan.py
--rw-r--r--   0        0        0     2235 2020-06-27 15:59:31.296723 fastcdc-1.5.0/fastcdc/utils.py
--rw-r--r--   0        0        0     1077 2020-11-25 18:01:43.048143 fastcdc-1.5.0/LICENSE
--rw-r--r--   0        0        0     1506 2023-03-13 16:39:52.421869 fastcdc-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     6357 2023-03-13 16:40:45.327759 fastcdc-1.5.0/README.md
--rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 fastcdc-1.5.0/setup.py
--rw-r--r--   0        0        0     7959 1970-01-01 00:00:00.000000 fastcdc-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1777 2023-03-14 08:39:13.371095 fastcdc-1.6.0/build.py
+-rw-r--r--   0        0        0       18 2020-05-23 20:10:03.765326 fastcdc-1.6.0/fastcdc/.gitignore
+-rw-r--r--   0        0        0      289 2024-05-09 19:08:19.455276 fastcdc-1.6.0/fastcdc/__init__.py
+-rw-r--r--   0        0        0     2136 2023-03-14 08:39:13.372095 fastcdc-1.6.0/fastcdc/benchmark.py
+-rw-r--r--   0        0        0     1790 2023-03-14 08:39:13.372095 fastcdc-1.6.0/fastcdc/chunkify.py
+-rw-r--r--   0        0        0      512 2023-03-14 08:39:13.373094 fastcdc-1.6.0/fastcdc/cli.py
+-rw-r--r--   0        0        0     4886 2023-03-14 08:39:13.373094 fastcdc-1.6.0/fastcdc/const.py
+-rw-r--r--   0        0        0     7364 2020-09-30 08:03:13.670476 fastcdc-1.6.0/fastcdc/fastcdc_cy.pyx
+-rw-r--r--   0        0        0     7558 2023-03-14 08:39:13.374094 fastcdc-1.6.0/fastcdc/fastcdc_py.py
+-rw-r--r--   0        0        0     3348 2023-03-14 08:39:13.374094 fastcdc-1.6.0/fastcdc/original.py
+-rw-r--r--   0        0        0     2966 2023-03-14 08:39:13.375094 fastcdc-1.6.0/fastcdc/scan.py
+-rw-r--r--   0        0        0     2154 2023-03-14 08:39:13.376094 fastcdc-1.6.0/fastcdc/utils.py
+-rw-r--r--   0        0        0     1077 2020-11-25 18:01:43.048143 fastcdc-1.6.0/LICENSE
+-rw-r--r--   0        0        0     1564 2024-05-09 19:08:19.456276 fastcdc-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6646 2024-05-09 19:08:39.120461 fastcdc-1.6.0/README.md
+-rw-r--r--   0        0        0     7659 1970-01-01 00:00:00.000000 fastcdc-1.6.0/setup.py
+-rw-r--r--   0        0        0     8014 1970-01-01 00:00:00.000000 fastcdc-1.6.0/PKG-INFO
```

### Comparing `fastcdc-1.5.0/build.py` & `fastcdc-1.6.0/build.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-# -*- coding: utf-8 -*-
-"""
-The shared library can also be built manually using the command:
-$ cythonize -X language_level=3 -a -i ./fastcdc/fastcdc_cy.pyx
-"""
-from distutils.command.build_ext import build_ext
-
-
-class BuildExt(build_ext):
-    def run(self):
-        try:
-            print("Trying to compile C accelerator module")
-            build_ext.run(self)
-            print("Successfully comiled C accelerator module")
-        except Exception as e:
-            print(e)
-            print("************************************************************")
-            print("Cannot compile C accelerator module, use pure python version")
-            print("************************************************************")
-
-    def build_extensions(self):
-        try:
-            print("Trying to compile C accelerator module")
-            super().build_extensions()
-            print("Successfully comiled C accelerator module")
-        except Exception as e:
-            print(e)
-            print("************************************************************")
-            print("Cannot compile C accelerator module, use pure python version")
-            print("************************************************************")
-
-
-def build(setup_kwargs):
-    try:
-        from Cython.Build import cythonize
-
-        setup_kwargs.update(
-            dict(
-                ext_modules=cythonize(["fastcdc/fastcdc_cy.pyx"]),
-                cmdclass=dict(build_ext=BuildExt),
-            )
-        )
-    except Exception as e:
-        print(e)
-        print("************************************************************")
-        print("Cannot compile C accelerator module, use pure python version")
-        print("************************************************************")
+# -*- coding: utf-8 -*-
+"""
+The shared library can also be built manually using the command:
+$ cythonize -X language_level=3 -a -i ./fastcdc/fastcdc_cy.pyx
+"""
+from distutils.command.build_ext import build_ext
+
+
+class BuildExt(build_ext):
+    def run(self):
+        try:
+            print("Trying to compile C accelerator module")
+            build_ext.run(self)
+            print("Successfully comiled C accelerator module")
+        except Exception as e:
+            print(e)
+            print("************************************************************")
+            print("Cannot compile C accelerator module, use pure python version")
+            print("************************************************************")
+
+    def build_extensions(self):
+        try:
+            print("Trying to compile C accelerator module")
+            super().build_extensions()
+            print("Successfully comiled C accelerator module")
+        except Exception as e:
+            print(e)
+            print("************************************************************")
+            print("Cannot compile C accelerator module, use pure python version")
+            print("************************************************************")
+
+
+def build(setup_kwargs):
+    try:
+        from Cython.Build import cythonize
+
+        setup_kwargs.update(
+            dict(
+                ext_modules=cythonize(["fastcdc/fastcdc_cy.pyx"]),
+                cmdclass=dict(build_ext=BuildExt),
+            )
+        )
+    except Exception as e:
+        print(e)
+        print("************************************************************")
+        print("Cannot compile C accelerator module, use pure python version")
+        print("************************************************************")
```

### Comparing `fastcdc-1.5.0/fastcdc/chunkify.py` & `fastcdc-1.6.0/fastcdc/chunkify.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-# -*- coding: utf-8 -*-
-import click
-from fastcdc import __version__, fastcdc
-import hashlib
-from fastcdc.utils import DefaultHelp, supported_hashes
-
-
-@click.command(cls=DefaultHelp)
-@click.version_option(version=__version__, message="fastcdc - %(version)s")
-@click.argument("file", type=click.File("rb"))
-@click.option(
-    "-s",
-    "--size",
-    type=click.INT,
-    default=16384,
-    help="The desired average size of the chunks.",
-    show_default=True,
-)
-@click.option(
-    "-mi", "--min-size", type=click.INT, help="Minimum chunk size (default size/4)"
-)
-@click.option(
-    "-ma", "--max-size", type=click.INT, help="Maximum chunk size (default size*8)"
-)
-@click.option(
-    "-hf", "--hash-function", type=click.STRING, default="sha256", show_default=True
-)
-def chunkify(file, size, min_size, max_size, hash_function):
-    """Find variable sized chunks for FILE and compute hashes."""
-    supported = supported_hashes()
-    if hash_function not in supported:
-        msg = "'{}' is not a supported hash.\nTry one of these:\n{}".format(
-            hash_function, ", ".join(supported)
-        )
-        raise click.BadOptionUsage("hf", msg)
-
-    hf = getattr(hashlib, hash_function)
-    chunker = fastcdc(file, min_size, size, max_size, hf=hf)
-
-    num_chunks = 0
-    for chunk in chunker:
-        click.secho("hash", fg="bright_magenta", nl=False)
-        click.secho("=", nl=False)
-        click.secho(chunk.hash, fg="bright_cyan", nl=False)
-        click.secho(" offset", fg="bright_magenta", nl=False)
-        click.secho("=", nl=False)
-        click.secho(str(chunk.offset), fg="bright_cyan", nl=False)
-        click.secho(" size", fg="bright_magenta", nl=False)
-        click.secho("=", nl=False)
-        click.secho(str(chunk.length), fg="bright_cyan")
-        num_chunks += 1
+# -*- coding: utf-8 -*-
+import click
+from fastcdc import __version__, fastcdc
+import hashlib
+from fastcdc.utils import DefaultHelp, supported_hashes
+
+
+@click.command(cls=DefaultHelp)
+@click.version_option(version=__version__, message="fastcdc - %(version)s")
+@click.argument("file", type=click.File("rb"))
+@click.option(
+    "-s",
+    "--size",
+    type=click.INT,
+    default=16384,
+    help="The desired average size of the chunks.",
+    show_default=True,
+)
+@click.option(
+    "-mi", "--min-size", type=click.INT, help="Minimum chunk size (default size/4)"
+)
+@click.option(
+    "-ma", "--max-size", type=click.INT, help="Maximum chunk size (default size*8)"
+)
+@click.option(
+    "-hf", "--hash-function", type=click.STRING, default="sha256", show_default=True
+)
+def chunkify(file, size, min_size, max_size, hash_function):
+    """Find variable sized chunks for FILE and compute hashes."""
+    supported = supported_hashes()
+    if hash_function not in supported:
+        msg = "'{}' is not a supported hash.\nTry one of these:\n{}".format(
+            hash_function, ", ".join(supported)
+        )
+        raise click.BadOptionUsage("hf", msg)
+
+    hf = getattr(hashlib, hash_function)
+    chunker = fastcdc(file, min_size, size, max_size, hf=hf)
+
+    num_chunks = 0
+    for chunk in chunker:
+        click.secho("hash", fg="bright_magenta", nl=False)
+        click.secho("=", nl=False)
+        click.secho(chunk.hash, fg="bright_cyan", nl=False)
+        click.secho(" offset", fg="bright_magenta", nl=False)
+        click.secho("=", nl=False)
+        click.secho(str(chunk.offset), fg="bright_cyan", nl=False)
+        click.secho(" size", fg="bright_magenta", nl=False)
+        click.secho("=", nl=False)
+        click.secho(str(chunk.length), fg="bright_cyan")
+        num_chunks += 1
```

### Comparing `fastcdc-1.5.0/fastcdc/fastcdc_cy.pyx` & `fastcdc-1.6.0/fastcdc/fastcdc_cy.pyx`

 * *Files identical despite different names*

### Comparing `fastcdc-1.5.0/fastcdc/fastcdc_py.py` & `fastcdc-1.6.0/fastcdc/fastcdc_py.py`

 * *Files identical despite different names*

### Comparing `fastcdc-1.5.0/fastcdc/original.py` & `fastcdc-1.6.0/fastcdc/original.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-# -*- coding: utf-8 -*-
-"""
-True to the original port of https://github.com/nlfiedler/fastcdc-rs
-"""
-import os
-from dataclasses import dataclass
-from mmap import mmap, ACCESS_READ
-from typing import Optional, ByteString, BinaryIO, Text, Union
-from fastcdc.const import (
-    TABLE,
-    MINIMUM_MIN,
-    MINIMUM_MAX,
-    AVERAGE_MIN,
-    AVERAGE_MAX,
-    MAXIMUM_MIN,
-    MAXIMUM_MAX,
-)
-from fastcdc.utils import center_size, logarithm2, mask
-
-
-@dataclass
-class Chunk:
-    offset: int
-    length: int
-
-
-@dataclass
-class FastCDC:
-
-    source: Union[ByteString, BinaryIO, Text]
-    bytes_processed: int
-    bytes_remaining: int
-    min_size: int
-    avg_size: int
-    max_size: int
-    mask_s: int
-    mask_l: int
-
-    @classmethod
-    def new(
-        cls,
-        source: Union[ByteString, BinaryIO, Text],
-        min_size: int,
-        avg_size: int,
-        max_size: int,
-    ):
-        assert min_size >= MINIMUM_MIN
-        assert min_size <= MINIMUM_MAX
-        assert avg_size >= AVERAGE_MIN
-        assert avg_size <= AVERAGE_MAX
-        assert max_size >= MAXIMUM_MIN
-        assert max_size <= MAXIMUM_MAX
-        bits = logarithm2(avg_size)
-        mask_s = mask(bits + 1)
-        mask_l = mask(bits - 1)
-        if isinstance(source, BinaryIO):
-            source = mmap(source.fileno(), 0, access=ACCESS_READ)
-            source.seek(0)
-        if isinstance(source, Text):
-            infile = os.open(source, os.O_RDONLY)
-            source = mmap(infile, 0, access=ACCESS_READ)
-        return cls(source, 0, len(source), min_size, avg_size, max_size, mask_s, mask_l)
-
-    def cut(self, source_offset: int, source_size: int) -> int:
-        if source_size <= self.min_size:
-            return source_size
-        else:
-            if source_size > self.max_size:
-                source_size = self.max_size
-            source_start = source_offset
-            source_len1 = source_offset + center_size(
-                self.avg_size, self.min_size, source_size
-            )
-            source_len2 = source_offset + source_size
-            hash_ = 0
-            source_offset += self.min_size
-            while source_offset < source_len1:
-                index = self.source[source_offset]
-                source_offset += 1
-                hash_ = (hash_ >> 1) + TABLE[index]
-                if hash_ & self.mask_s == 0:
-                    return source_offset - source_start
-
-            while source_offset < source_len2:
-                index = self.source[source_offset]
-                source_offset += 1
-                hash_ = (hash_ >> 1) + TABLE[index]
-                if hash_ & self.mask_l == 0:
-                    return source_offset - source_start
-            return source_size
-
-    def __iter__(self):
-        self.bytes_processed = 0
-        self.bytes_remaining = len(self.source)
-        return self
-
-    def __next__(self) -> Optional[Chunk]:
-        if self.bytes_remaining == 0:
-            raise StopIteration
-        else:
-            chunk_size = self.cut(self.bytes_processed, self.bytes_remaining)
-            chunk_start = self.bytes_processed
-            self.bytes_processed += chunk_size
-            self.bytes_remaining -= chunk_size
-            return Chunk(offset=chunk_start, length=chunk_size)
-
-    def __del__(self):
-        if hasattr(self.source, "close"):
-            self.source.close()
+# -*- coding: utf-8 -*-
+"""
+True to the original port of https://github.com/nlfiedler/fastcdc-rs
+"""
+import os
+from dataclasses import dataclass
+from mmap import mmap, ACCESS_READ
+from typing import Optional, ByteString, BinaryIO, Text, Union
+from fastcdc.const import (
+    TABLE,
+    MINIMUM_MIN,
+    MINIMUM_MAX,
+    AVERAGE_MIN,
+    AVERAGE_MAX,
+    MAXIMUM_MIN,
+    MAXIMUM_MAX,
+)
+from fastcdc.utils import center_size, logarithm2, mask
+
+
+@dataclass
+class Chunk:
+    offset: int
+    length: int
+
+
+@dataclass
+class FastCDC:
+
+    source: Union[ByteString, BinaryIO, Text]
+    bytes_processed: int
+    bytes_remaining: int
+    min_size: int
+    avg_size: int
+    max_size: int
+    mask_s: int
+    mask_l: int
+
+    @classmethod
+    def new(
+        cls,
+        source: Union[ByteString, BinaryIO, Text],
+        min_size: int,
+        avg_size: int,
+        max_size: int,
+    ):
+        assert min_size >= MINIMUM_MIN
+        assert min_size <= MINIMUM_MAX
+        assert avg_size >= AVERAGE_MIN
+        assert avg_size <= AVERAGE_MAX
+        assert max_size >= MAXIMUM_MIN
+        assert max_size <= MAXIMUM_MAX
+        bits = logarithm2(avg_size)
+        mask_s = mask(bits + 1)
+        mask_l = mask(bits - 1)
+        if isinstance(source, BinaryIO):
+            source = mmap(source.fileno(), 0, access=ACCESS_READ)
+            source.seek(0)
+        if isinstance(source, Text):
+            infile = os.open(source, os.O_RDONLY)
+            source = mmap(infile, 0, access=ACCESS_READ)
+        return cls(source, 0, len(source), min_size, avg_size, max_size, mask_s, mask_l)
+
+    def cut(self, source_offset: int, source_size: int) -> int:
+        if source_size <= self.min_size:
+            return source_size
+        else:
+            if source_size > self.max_size:
+                source_size = self.max_size
+            source_start = source_offset
+            source_len1 = source_offset + center_size(
+                self.avg_size, self.min_size, source_size
+            )
+            source_len2 = source_offset + source_size
+            hash_ = 0
+            source_offset += self.min_size
+            while source_offset < source_len1:
+                index = self.source[source_offset]
+                source_offset += 1
+                hash_ = (hash_ >> 1) + TABLE[index]
+                if hash_ & self.mask_s == 0:
+                    return source_offset - source_start
+
+            while source_offset < source_len2:
+                index = self.source[source_offset]
+                source_offset += 1
+                hash_ = (hash_ >> 1) + TABLE[index]
+                if hash_ & self.mask_l == 0:
+                    return source_offset - source_start
+            return source_size
+
+    def __iter__(self):
+        self.bytes_processed = 0
+        self.bytes_remaining = len(self.source)
+        return self
+
+    def __next__(self) -> Optional[Chunk]:
+        if self.bytes_remaining == 0:
+            raise StopIteration
+        else:
+            chunk_size = self.cut(self.bytes_processed, self.bytes_remaining)
+            chunk_start = self.bytes_processed
+            self.bytes_processed += chunk_size
+            self.bytes_remaining -= chunk_size
+            return Chunk(offset=chunk_start, length=chunk_size)
+
+    def __del__(self):
+        if hasattr(self.source, "close"):
+            self.source.close()
```

### Comparing `fastcdc-1.5.0/fastcdc/scan.py` & `fastcdc-1.6.0/fastcdc/scan.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-# -*- coding: utf-8 -*-
-import hashlib
-from humanize import intcomma, naturalsize
-import click
-from codetiming import Timer
-
-import fastcdc
-from fastcdc.utils import DefaultHelp, iter_files, supported_hashes
-
-
-@click.command(cls=DefaultHelp)
-@click.argument(
-    "paths", type=click.Path(exists=True, file_okay=False, resolve_path=True), nargs=-1,
-)
-@click.option(
-    "-r", "--recursive", help="Scan directory tree recursively.", is_flag=True,
-)
-@click.option(
-    "-s",
-    "--size",
-    type=click.INT,
-    default=16384,
-    help="The desired average size of the chunks.",
-    show_default=True,
-)
-@click.option(
-    "-mi", "--min-size", type=click.INT, help="Minimum chunk size (default size/4)"
-)
-@click.option(
-    "-ma", "--max-size", type=click.INT, help="Maximum chunk size (default size*8)"
-)
-@click.option(
-    "-hf", "--hash-function", type=click.STRING, default="sha256", show_default=True
-)
-def scan(paths, recursive, size, min_size, max_size, hash_function):
-    """Scan files in directories and report duplication."""
-    if min_size is None:
-        min_size = size // 4
-    if max_size is None:
-        max_size = size * 8
-
-    bytes_total = 0
-    bytes_dupe = 0
-    fingerprints = set()
-    supported = supported_hashes()
-    if hash_function not in supported:
-        msg = "'{}' is not a supported hash.\nTry one of these:\n{}".format(
-            hash_function, ", ".join(supported)
-        )
-        raise click.BadOptionUsage("hf", msg)
-
-    hf = getattr(hashlib, hash_function)
-    files = []
-    for path in paths:
-        files += list(iter_files(path, recursive))
-    t = Timer("scan", logger=None)
-    t.start()
-    with click.progressbar(files) as pgbar:
-        for entry in pgbar:
-            try:
-                chunker = fastcdc.fastcdc(entry.path, min_size, size, max_size, hf=hf)
-            except Exception as e:
-                click.echo("\n for {}".format(entry.path))
-                click.echo(repr(e))
-                continue
-            for chunk in chunker:
-                bytes_total += chunk.length
-                if chunk.hash in fingerprints:
-                    bytes_dupe += chunk.length
-                fingerprints.add(chunk.hash)
-    t.stop()
-    if bytes_total:
-        data_per_s = bytes_total / Timer.timers.mean("scan")
-        dd_ratio = bytes_dupe / bytes_total * 100
-        click.echo("Files:          {}".format(intcomma(len(files))))
-        click.echo(
-            "Chunk Sizes:    min {} - avg {} - max {}".format(min_size, size, max_size)
-        )
-        click.echo("Unique Chunks:  {}".format(intcomma(len(fingerprints))))
-        click.echo("Total Data:     {}".format(naturalsize(bytes_total)))
-        click.echo("Dupe Data:      {}".format(naturalsize(bytes_dupe)))
-        click.echo("DeDupe Ratio:   {:.2f} %".format(dd_ratio))
-        click.echo("Throughput:     {}/s".format(naturalsize(data_per_s)))
-    else:
-        click.echo("No data.")
-
-
-if __name__ == "__main__":
-    scan()
+# -*- coding: utf-8 -*-
+import hashlib
+from humanize import intcomma, naturalsize
+import click
+from codetiming import Timer
+
+import fastcdc
+from fastcdc.utils import DefaultHelp, iter_files, supported_hashes
+
+
+@click.command(cls=DefaultHelp)
+@click.argument(
+    "paths", type=click.Path(exists=True, file_okay=False, resolve_path=True), nargs=-1,
+)
+@click.option(
+    "-r", "--recursive", help="Scan directory tree recursively.", is_flag=True,
+)
+@click.option(
+    "-s",
+    "--size",
+    type=click.INT,
+    default=16384,
+    help="The desired average size of the chunks.",
+    show_default=True,
+)
+@click.option(
+    "-mi", "--min-size", type=click.INT, help="Minimum chunk size (default size/4)"
+)
+@click.option(
+    "-ma", "--max-size", type=click.INT, help="Maximum chunk size (default size*8)"
+)
+@click.option(
+    "-hf", "--hash-function", type=click.STRING, default="sha256", show_default=True
+)
+def scan(paths, recursive, size, min_size, max_size, hash_function):
+    """Scan files in directories and report duplication."""
+    if min_size is None:
+        min_size = size // 4
+    if max_size is None:
+        max_size = size * 8
+
+    bytes_total = 0
+    bytes_dupe = 0
+    fingerprints = set()
+    supported = supported_hashes()
+    if hash_function not in supported:
+        msg = "'{}' is not a supported hash.\nTry one of these:\n{}".format(
+            hash_function, ", ".join(supported)
+        )
+        raise click.BadOptionUsage("hf", msg)
+
+    hf = getattr(hashlib, hash_function)
+    files = []
+    for path in paths:
+        files += list(iter_files(path, recursive))
+    t = Timer("scan", logger=None)
+    t.start()
+    with click.progressbar(files) as pgbar:
+        for entry in pgbar:
+            try:
+                chunker = fastcdc.fastcdc(entry.path, min_size, size, max_size, hf=hf)
+            except Exception as e:
+                click.echo("\n for {}".format(entry.path))
+                click.echo(repr(e))
+                continue
+            for chunk in chunker:
+                bytes_total += chunk.length
+                if chunk.hash in fingerprints:
+                    bytes_dupe += chunk.length
+                fingerprints.add(chunk.hash)
+    t.stop()
+    if bytes_total:
+        data_per_s = bytes_total / Timer.timers.mean("scan")
+        dd_ratio = bytes_dupe / bytes_total * 100
+        click.echo("Files:          {}".format(intcomma(len(files))))
+        click.echo(
+            "Chunk Sizes:    min {} - avg {} - max {}".format(min_size, size, max_size)
+        )
+        click.echo("Unique Chunks:  {}".format(intcomma(len(fingerprints))))
+        click.echo("Total Data:     {}".format(naturalsize(bytes_total)))
+        click.echo("Dupe Data:      {}".format(naturalsize(bytes_dupe)))
+        click.echo("DeDupe Ratio:   {:.2f} %".format(dd_ratio))
+        click.echo("Throughput:     {}/s".format(naturalsize(data_per_s)))
+    else:
+        click.echo("No data.")
+
+
+if __name__ == "__main__":
+    scan()
```

### Comparing `fastcdc-1.5.0/LICENSE` & `fastcdc-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastcdc-1.5.0/pyproject.toml` & `fastcdc-1.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-[tool.poetry]
-name = "fastcdc"
-version = "1.5.0"
-description = "FastCDC (content defined chunking) in pure Python."
-authors = ["Titusz Pan <tp@py7.de>"]
-license = "MIT"
-readme = "README.md"
-repository = "https://github.com/iscc/fastcdc-py"
-keywords = ["cdc", "chunking"]
-
-classifiers = [
-    "Intended Audience :: Developers",
-    "Intended Audience :: Information Technology",
-    "Environment :: Console",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: Unix",
-    "Operating System :: POSIX",
-    "Operating System :: Microsoft :: Windows",
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-    "Topic :: Multimedia",
-    "Topic :: System :: Archiving",
-    "Topic :: Utilities",
-    "Topic :: Software Development",
-]
-
-[tool.poetry.scripts]
-fastcdc = 'fastcdc.cli:cli'
-
-[tool.poetry.dependencies]
-python = ">=3.7.2,<4.0"
-click = "^8.1"
-humanize = "^4.0"
-codetiming = "^1.2"
-click-default-group = "^1.2"
-py-cpuinfo = "^9.0"
-
-xxhash = { version = "^3.0", optional = true }
-blake3 = { version = "^0.3", optional = true }
-
-[tool.poetry.extras]
-hashes = ["xxhash", "blake3"]
-
-[tool.poetry.dev-dependencies]
-pytest = "*"
-black = "*"
-cython = "*"
-pytest-benchmark = "*"
-
-[tool.poetry.build]
-generate-setup-file = true
-script = "build.py"
-
-[build-system]
-requires = ["poetry-core>=1.0.0", "setuptools", "wheel", "cython"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "fastcdc"
+version = "1.6.0"
+description = "FastCDC (content defined chunking) in pure Python."
+authors = ["Titusz Pan <tp@py7.de>"]
+license = "MIT"
+readme = "README.md"
+repository = "https://github.com/iscc/fastcdc-py"
+keywords = ["cdc", "chunking"]
+
+classifiers = [
+    "Intended Audience :: Developers",
+    "Intended Audience :: Information Technology",
+    "Environment :: Console",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: Unix",
+    "Operating System :: POSIX",
+    "Operating System :: Microsoft :: Windows",
+    'Programming Language :: Python',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    "Topic :: Multimedia",
+    "Topic :: System :: Archiving",
+    "Topic :: Utilities",
+    "Topic :: Software Development",
+]
+
+[tool.poetry.scripts]
+fastcdc = 'fastcdc.cli:cli'
+
+[tool.poetry.dependencies]
+python = ">=3.7.2,<4.0"
+click = "^8.1"
+humanize = "^4.0"
+codetiming = "^1.2"
+click-default-group = "^1.2"
+py-cpuinfo = "^9.0"
+
+xxhash = { version = "^3.0", optional = true }
+blake3 = { version = "^0.3", optional = true }
+
+[tool.poetry.extras]
+hashes = ["xxhash", "blake3"]
+
+[tool.poetry.dev-dependencies]
+pytest = "*"
+black = "*"
+cython = "*"
+pytest-benchmark = "*"
+
+[tool.poetry.build]
+generate-setup-file = true
+script = "build.py"
+
+[build-system]
+requires = ["poetry-core>=1.0.0", "setuptools", "wheel", "cython"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `fastcdc-1.5.0/README.md` & `fastcdc-1.6.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,179 +1,43 @@
-# FastCDC
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-[![Tests](https://github.com/titusz/fastcdc-py/workflows/Tests/badge.svg)](https://github.com/titusz/fastcdc-py/actions?query=workflow%3ATests)
-[![Version](https://img.shields.io/pypi/v/fastcdc.svg)](https://pypi.python.org/pypi/fastcdc/)
-[![Downloads](https://pepy.tech/badge/fastcdc)](https://pepy.tech/project/fastcdc)
-
-This package implements the "FastCDC" content defined chunking algorithm in
-Python with optional cython support. To learn more about content
-defined chunking and its applications, see the reference material linked below.
-
-
-## Requirements
-
-* [Python](https://www.python.org/) Version 3.7 and later. Tested on Linux, Mac and
-Windows
-
-## Installing
-
-```shell
-$ pip install fastcdc
-```
-
-To enable add additional support for the hash algorithms
-([xxhash](https://github.com/Cyan4973/xxHash) and
-[blake3](https://github.com/BLAKE3-team/BLAKE3/)) use
-
-```shell
-$ pip install fastcdc[hashes]
-```
-
-## Usage
-
-### Calculate chunks with default settings:
-```shell
-$ fastcdc tests/SekienAkashita.jpg
-hash=103159aa68bb1ea98f64248c647b8fe9a303365d80cb63974a73bba8bc3167d7 offset=0 size=22366
-hash=3f2b58dc77982e763e75db76c4205aaab4e18ff8929e298ca5c58500fee5530d offset=22366 size=10491
-hash=fcfb2f49ccb2640887a74fad1fb8a32368b5461a9dccc28f29ddb896b489b913 offset=32857 size=14094
-hash=bd1198535cdb87c5571378db08b6e886daf810873f5d77000a54795409464138 offset=46951 size=18696
-hash=d6347a2e5bf586d42f2d80559d4f4a2bf160dce8f77eede023ad2314856f3086 offset=65647 size=43819
-```
-
-### Customize min-size, avg-size, max-size, and hash function
-```shell
-$ fastcdc -mi 16384 -s 32768 -ma 65536 -hf sha256 tests/SekienAkashita.jpg
-hash=5a80871bad4588c7278d39707fe68b8b174b1aa54c59169d3c2c72f1e16ef46d offset=0 size=32857
-hash=13f6a4c6d42df2b76c138c13e86e1379c203445055c2b5f043a5f6c291fa520d offset=32857 size=16408
-hash=0fe7305ba21a5a5ca9f89962c5a6f3e29cd3e2b36f00e565858e0012e5f8df36 offset=49265 size=60201
-```
-
-###  Scan files in directory and report duplication.
-```shell
-$ fastcdc scan ~/Downloads
-[####################################]  100%
-Files:          1,332
-Chunk Sizes:    min 4096 - avg 16384 - max 131072
-Unique Chunks:  506,077
-Total Data:     9.3 GB
-Dupe Data:      873.8 MB
-DeDupe Ratio:   9.36 %
-Throughput:     135.2 MB/s
-```
-
-### Show help
-
-```shell
-$ fastcdc
-Usage: fastcdc [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --version  Show the version and exit.
-  --help     Show this message and exit.
-
-Commands:
-  chunkify*  Find variable sized chunks for FILE and compute hashes.
-  benchmark  Benchmark chunking performance.
-  scan       Scan files in directory and report duplication.
-```
-
-### Use from your python code
-The  tests also have some short examples of using the chunker, of which this
-code snippet is an example:
-
-```python
-from fastcdc import fastcdc
-
-results = list(fastcdc("tests/SekienAkashita.jpg", 16384, 32768, 65536))
-assert len(results) == 3
-assert results[0].offset == 0
-assert results[0].length == 32857
-assert results[1].offset == 32857
-assert results[1].length == 16408
-assert results[2].offset == 49265
-assert results[2].length == 60201
-```
-
-## Reference Material
-
-The algorithm is as described in "FastCDC: a Fast and Efficient Content-Defined
-Chunking Approach for Data Deduplication"; see the
-[paper](https://www.usenix.org/system/files/conference/atc16/atc16-paper-xia.pdf),
-and
-[presentation](https://www.usenix.org/sites/default/files/conference/protected-files/atc16_slides_xia.pdf)
-for details. There are some minor differences, as described below.
-
-### Differences with the FastCDC paper
-
-The explanation below is copied from
-[ronomon/deduplication](https://github.com/ronomon/deduplication) since this
-codebase is little more than a translation of that implementation:
-
-> The following optimizations and variations on FastCDC are involved in the chunking algorithm:
-> * 31 bit integers to avoid 64 bit integers for the sake of the Javascript reference implementation.
-> * A right shift instead of a left shift to remove the need for an additional modulus operator, which would otherwise have been necessary to prevent overflow.
-> * Masks are no longer zero-padded since a right shift is used instead of a left shift.
-> * A more adaptive threshold based on a combination of average and minimum chunk size (rather than just average chunk size) to decide the pivot point at which to switch masks. A larger minimum chunk size now switches from the strict mask to the eager mask earlier.
-> * Masks use 1 bit of chunk size normalization instead of 2 bits of chunk size normalization.
-
-The primary objective of this codebase was to have a Python implementation with a
-permissive license, which could be used for new projects, without concern for
-data parity with existing implementations.
-
-## Prior Art
-
-This package started as Python port of the implementation by Nathan Fiedler (see the
-nlfiedler link below).
-
-* [nlfiedler/fastcdc-rs](https://github.com/nlfiedler/fastcdc-rs)
-    + Rust implementation on which this code is based.
-* [ronomon/deduplication](https://github.com/ronomon/deduplication)
-    + C++ and JavaScript implementation on which the rust implementation is based.
-* [rdedup_cdc at docs.rs](https://docs.rs/crate/rdedup-cdc/0.1.0/source/src/fastcdc.rs)
-    + An alternative implementation of FastCDC to the one in this crate.
-* [jrobhoward/quickcdc](https://github.com/jrobhoward/quickcdc)
-    + Similar but slightly earlier algorithm by some of the same researchers.
-
-## Change Log
-
-## [1.5.0] - 2023-03-13
-- added python 3.10/3.11 support
-- removed python 3.6 support
-- update dependencies
-
-## [1.4.2] - 2020-11-25
-- add binary releases to PyPI (Xie Yanbo)
-- update dependencies
-
-## [1.4.1] - 2020-09-30
-- fix issue with fat option in cython version
-- updated dependencies
-
-## [1.4.0] - 2020-08-08
-- add support for multiple path with scan command
-- fix issue with building cython extension
-- fix issue with fat option
-- fix zero-devision error
-
-## [1.3.0] - 2020-06-26
-- add new `scan` command to calculate deduplication ratio for directories
-
-## [1.2.0] - 2020-05-23
-
-### Added
-- faster optional cython implementation
-- benchmark command
-
-## [1.1.0] - 2020-05-09
-
-### Added
-- high-level API
-- support for streams
-- support for custom hash functions
+packages = \
+['fastcdc']
 
+package_data = \
+{'': ['*']}
 
-## [1.0.0] - 2020-05-07
-
-### Added
-- Initial release (port of [nlfiedler/fastcdc-rs](https://github.com/nlfiedler/fastcdc-rs)).
+install_requires = \
+['click-default-group>=1.2,<2.0',
+ 'click>=8.1,<9.0',
+ 'codetiming>=1.2,<2.0',
+ 'humanize>=4.0,<5.0',
+ 'py-cpuinfo>=9.0,<10.0']
+
+extras_require = \
+{'hashes': ['xxhash>=3.0,<4.0', 'blake3>=0.3,<0.4']}
+
+entry_points = \
+{'console_scripts': ['fastcdc = fastcdc.cli:cli']}
+
+setup_kwargs = {
+    'name': 'fastcdc',
+    'version': '1.6.0',
+    'description': 'FastCDC (content defined chunking) in pure Python.',
+    'long_description': '# FastCDC\n\n[![Tests](https://github.com/titusz/fastcdc-py/workflows/Tests/badge.svg)](https://github.com/titusz/fastcdc-py/actions?query=workflow%3ATests)\n[![Version](https://img.shields.io/pypi/v/fastcdc.svg)](https://pypi.python.org/pypi/fastcdc/)\n[![Downloads](https://pepy.tech/badge/fastcdc)](https://pepy.tech/project/fastcdc)\n\nThis package implements the "FastCDC" content defined chunking algorithm in\nPython with optional cython support. To learn more about content\ndefined chunking and its applications, see the reference material linked below.\n\n\n## Requirements\n\n* [Python](https://www.python.org/) Version 3.7 and later. Tested on Linux, Mac and\nWindows\n\n## Installing\n\n```shell\n$ pip install fastcdc\n```\n\nTo enable add additional support for the hash algorithms\n([xxhash](https://github.com/Cyan4973/xxHash) and\n[blake3](https://github.com/BLAKE3-team/BLAKE3/)) use\n\n```shell\n$ pip install fastcdc[hashes]\n```\n\n## Usage\n\n### Calculate chunks with default settings:\n```shell\n$ fastcdc tests/SekienAkashita.jpg\nhash=103159aa68bb1ea98f64248c647b8fe9a303365d80cb63974a73bba8bc3167d7 offset=0 size=22366\nhash=3f2b58dc77982e763e75db76c4205aaab4e18ff8929e298ca5c58500fee5530d offset=22366 size=10491\nhash=fcfb2f49ccb2640887a74fad1fb8a32368b5461a9dccc28f29ddb896b489b913 offset=32857 size=14094\nhash=bd1198535cdb87c5571378db08b6e886daf810873f5d77000a54795409464138 offset=46951 size=18696\nhash=d6347a2e5bf586d42f2d80559d4f4a2bf160dce8f77eede023ad2314856f3086 offset=65647 size=43819\n```\n\n### Customize min-size, avg-size, max-size, and hash function\n```shell\n$ fastcdc -mi 16384 -s 32768 -ma 65536 -hf sha256 tests/SekienAkashita.jpg\nhash=5a80871bad4588c7278d39707fe68b8b174b1aa54c59169d3c2c72f1e16ef46d offset=0 size=32857\nhash=13f6a4c6d42df2b76c138c13e86e1379c203445055c2b5f043a5f6c291fa520d offset=32857 size=16408\nhash=0fe7305ba21a5a5ca9f89962c5a6f3e29cd3e2b36f00e565858e0012e5f8df36 offset=49265 size=60201\n```\n\n###  Scan files in directory and report duplication.\n```shell\n$ fastcdc scan ~/Downloads\n[####################################]  100%\nFiles:          1,332\nChunk Sizes:    min 4096 - avg 16384 - max 131072\nUnique Chunks:  506,077\nTotal Data:     9.3 GB\nDupe Data:      873.8 MB\nDeDupe Ratio:   9.36 %\nThroughput:     135.2 MB/s\n```\n\n### Show help\n\n```shell\n$ fastcdc\nUsage: fastcdc [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --version  Show the version and exit.\n  --help     Show this message and exit.\n\nCommands:\n  chunkify*  Find variable sized chunks for FILE and compute hashes.\n  benchmark  Benchmark chunking performance.\n  scan       Scan files in directory and report duplication.\n```\n\n### Use from your python code\nThe  tests also have some short examples of using the chunker, of which this\ncode snippet is an example:\n\n```python\nfrom fastcdc import fastcdc\n\nresults = list(fastcdc("tests/SekienAkashita.jpg", 16384, 32768, 65536))\nassert len(results) == 3\nassert results[0].offset == 0\nassert results[0].length == 32857\nassert results[1].offset == 32857\nassert results[1].length == 16408\nassert results[2].offset == 49265\nassert results[2].length == 60201\n```\n\n## Reference Material\n\nThe algorithm is as described in "FastCDC: a Fast and Efficient Content-Defined\nChunking Approach for Data Deduplication"; see the\n[paper](https://www.usenix.org/system/files/conference/atc16/atc16-paper-xia.pdf),\nand\n[presentation](https://www.usenix.org/sites/default/files/conference/protected-files/atc16_slides_xia.pdf)\nfor details. There are some minor differences, as described below.\n\n### Differences with the FastCDC paper\n\nThe explanation below is copied from\n[ronomon/deduplication](https://github.com/ronomon/deduplication) since this\ncodebase is little more than a translation of that implementation:\n\n> The following optimizations and variations on FastCDC are involved in the chunking algorithm:\n> * 31 bit integers to avoid 64 bit integers for the sake of the Javascript reference implementation.\n> * A right shift instead of a left shift to remove the need for an additional modulus operator, which would otherwise have been necessary to prevent overflow.\n> * Masks are no longer zero-padded since a right shift is used instead of a left shift.\n> * A more adaptive threshold based on a combination of average and minimum chunk size (rather than just average chunk size) to decide the pivot point at which to switch masks. A larger minimum chunk size now switches from the strict mask to the eager mask earlier.\n> * Masks use 1 bit of chunk size normalization instead of 2 bits of chunk size normalization.\n\nThe primary objective of this codebase was to have a Python implementation with a\npermissive license, which could be used for new projects, without concern for\ndata parity with existing implementations.\n\n## Prior Art\n\nThis package started as Python port of the implementation by Nathan Fiedler (see the\nnlfiedler link below).\n\n* [nlfiedler/fastcdc-rs](https://github.com/nlfiedler/fastcdc-rs)\n    + Rust implementation on which this code is based.\n* [ronomon/deduplication](https://github.com/ronomon/deduplication)\n    + C++ and JavaScript implementation on which the rust implementation is based.\n* [rdedup_cdc at docs.rs](https://docs.rs/crate/rdedup-cdc/0.1.0/source/src/fastcdc.rs)\n    + An alternative implementation of FastCDC to the one in this crate.\n* [jrobhoward/quickcdc](https://github.com/jrobhoward/quickcdc)\n    + Similar but slightly earlier algorithm by some of the same researchers.\n\n## Change Log\n\n## [1.6.0] - 2024-05-09\n- added python 3.12 support\n- removed python 3.7 support\n- updated dependencies\n\n## [1.5.0] - 2023-03-13\n- added python 3.10/3.11 support\n- removed python 3.6 support\n- update dependencies\n\n## [1.4.2] - 2020-11-25\n- add binary releases to PyPI (Xie Yanbo)\n- update dependencies\n\n## [1.4.1] - 2020-09-30\n- fix issue with fat option in cython version\n- updated dependencies\n\n## [1.4.0] - 2020-08-08\n- add support for multiple path with scan command\n- fix issue with building cython extension\n- fix issue with fat option\n- fix zero-devision error\n\n## [1.3.0] - 2020-06-26\n- add new `scan` command to calculate deduplication ratio for directories\n\n## [1.2.0] - 2020-05-23\n\n### Added\n- faster optional cython implementation\n- benchmark command\n\n## [1.1.0] - 2020-05-09\n\n### Added\n- high-level API\n- support for streams\n- support for custom hash functions\n\n\n## [1.0.0] - 2020-05-07\n\n### Added\n- Initial release (port of [nlfiedler/fastcdc-rs](https://github.com/nlfiedler/fastcdc-rs)).\n\n',
+    'author': 'Titusz Pan',
+    'author_email': 'tp@py7.de',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://github.com/iscc/fastcdc-py',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'extras_require': extras_require,
+    'entry_points': entry_points,
+    'python_requires': '>=3.7.2,<4.0',
+}
+from build import *
+build(setup_kwargs)
 
+setup(**setup_kwargs)
```

### Comparing `fastcdc-1.5.0/setup.py` & `fastcdc-1.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,225 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fastcdc
+Version: 1.6.0
+Summary: FastCDC (content defined chunking) in pure Python.
+Home-page: https://github.com/iscc/fastcdc-py
+License: MIT
+Keywords: cdc,chunking
+Author: Titusz Pan
+Author-email: tp@py7.de
+Requires-Python: >=3.7.2,<4.0
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Multimedia
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: Utilities
+Provides-Extra: hashes
+Requires-Dist: blake3 (>=0.3,<0.4) ; extra == "hashes"
+Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: click-default-group (>=1.2,<2.0)
+Requires-Dist: codetiming (>=1.2,<2.0)
+Requires-Dist: humanize (>=4.0,<5.0)
+Requires-Dist: py-cpuinfo (>=9.0,<10.0)
+Requires-Dist: xxhash (>=3.0,<4.0) ; extra == "hashes"
+Project-URL: Repository, https://github.com/iscc/fastcdc-py
+Description-Content-Type: text/markdown
+
+# FastCDC
+
+[![Tests](https://github.com/titusz/fastcdc-py/workflows/Tests/badge.svg)](https://github.com/titusz/fastcdc-py/actions?query=workflow%3ATests)
+[![Version](https://img.shields.io/pypi/v/fastcdc.svg)](https://pypi.python.org/pypi/fastcdc/)
+[![Downloads](https://pepy.tech/badge/fastcdc)](https://pepy.tech/project/fastcdc)
+
+This package implements the "FastCDC" content defined chunking algorithm in
+Python with optional cython support. To learn more about content
+defined chunking and its applications, see the reference material linked below.
+
+
+## Requirements
+
+* [Python](https://www.python.org/) Version 3.7 and later. Tested on Linux, Mac and
+Windows
+
+## Installing
+
+```shell
+$ pip install fastcdc
+```
+
+To enable add additional support for the hash algorithms
+([xxhash](https://github.com/Cyan4973/xxHash) and
+[blake3](https://github.com/BLAKE3-team/BLAKE3/)) use
+
+```shell
+$ pip install fastcdc[hashes]
+```
+
+## Usage
+
+### Calculate chunks with default settings:
+```shell
+$ fastcdc tests/SekienAkashita.jpg
+hash=103159aa68bb1ea98f64248c647b8fe9a303365d80cb63974a73bba8bc3167d7 offset=0 size=22366
+hash=3f2b58dc77982e763e75db76c4205aaab4e18ff8929e298ca5c58500fee5530d offset=22366 size=10491
+hash=fcfb2f49ccb2640887a74fad1fb8a32368b5461a9dccc28f29ddb896b489b913 offset=32857 size=14094
+hash=bd1198535cdb87c5571378db08b6e886daf810873f5d77000a54795409464138 offset=46951 size=18696
+hash=d6347a2e5bf586d42f2d80559d4f4a2bf160dce8f77eede023ad2314856f3086 offset=65647 size=43819
+```
+
+### Customize min-size, avg-size, max-size, and hash function
+```shell
+$ fastcdc -mi 16384 -s 32768 -ma 65536 -hf sha256 tests/SekienAkashita.jpg
+hash=5a80871bad4588c7278d39707fe68b8b174b1aa54c59169d3c2c72f1e16ef46d offset=0 size=32857
+hash=13f6a4c6d42df2b76c138c13e86e1379c203445055c2b5f043a5f6c291fa520d offset=32857 size=16408
+hash=0fe7305ba21a5a5ca9f89962c5a6f3e29cd3e2b36f00e565858e0012e5f8df36 offset=49265 size=60201
+```
+
+###  Scan files in directory and report duplication.
+```shell
+$ fastcdc scan ~/Downloads
+[####################################]  100%
+Files:          1,332
+Chunk Sizes:    min 4096 - avg 16384 - max 131072
+Unique Chunks:  506,077
+Total Data:     9.3 GB
+Dupe Data:      873.8 MB
+DeDupe Ratio:   9.36 %
+Throughput:     135.2 MB/s
+```
+
+### Show help
+
+```shell
+$ fastcdc
+Usage: fastcdc [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --version  Show the version and exit.
+  --help     Show this message and exit.
+
+Commands:
+  chunkify*  Find variable sized chunks for FILE and compute hashes.
+  benchmark  Benchmark chunking performance.
+  scan       Scan files in directory and report duplication.
+```
+
+### Use from your python code
+The  tests also have some short examples of using the chunker, of which this
+code snippet is an example:
+
+```python
+from fastcdc import fastcdc
+
+results = list(fastcdc("tests/SekienAkashita.jpg", 16384, 32768, 65536))
+assert len(results) == 3
+assert results[0].offset == 0
+assert results[0].length == 32857
+assert results[1].offset == 32857
+assert results[1].length == 16408
+assert results[2].offset == 49265
+assert results[2].length == 60201
+```
+
+## Reference Material
+
+The algorithm is as described in "FastCDC: a Fast and Efficient Content-Defined
+Chunking Approach for Data Deduplication"; see the
+[paper](https://www.usenix.org/system/files/conference/atc16/atc16-paper-xia.pdf),
+and
+[presentation](https://www.usenix.org/sites/default/files/conference/protected-files/atc16_slides_xia.pdf)
+for details. There are some minor differences, as described below.
+
+### Differences with the FastCDC paper
+
+The explanation below is copied from
+[ronomon/deduplication](https://github.com/ronomon/deduplication) since this
+codebase is little more than a translation of that implementation:
+
+> The following optimizations and variations on FastCDC are involved in the chunking algorithm:
+> * 31 bit integers to avoid 64 bit integers for the sake of the Javascript reference implementation.
+> * A right shift instead of a left shift to remove the need for an additional modulus operator, which would otherwise have been necessary to prevent overflow.
+> * Masks are no longer zero-padded since a right shift is used instead of a left shift.
+> * A more adaptive threshold based on a combination of average and minimum chunk size (rather than just average chunk size) to decide the pivot point at which to switch masks. A larger minimum chunk size now switches from the strict mask to the eager mask earlier.
+> * Masks use 1 bit of chunk size normalization instead of 2 bits of chunk size normalization.
+
+The primary objective of this codebase was to have a Python implementation with a
+permissive license, which could be used for new projects, without concern for
+data parity with existing implementations.
+
+## Prior Art
+
+This package started as Python port of the implementation by Nathan Fiedler (see the
+nlfiedler link below).
+
+* [nlfiedler/fastcdc-rs](https://github.com/nlfiedler/fastcdc-rs)
+    + Rust implementation on which this code is based.
+* [ronomon/deduplication](https://github.com/ronomon/deduplication)
+    + C++ and JavaScript implementation on which the rust implementation is based.
+* [rdedup_cdc at docs.rs](https://docs.rs/crate/rdedup-cdc/0.1.0/source/src/fastcdc.rs)
+    + An alternative implementation of FastCDC to the one in this crate.
+* [jrobhoward/quickcdc](https://github.com/jrobhoward/quickcdc)
+    + Similar but slightly earlier algorithm by some of the same researchers.
+
+## Change Log
+
+## [1.6.0] - 2024-05-09
+- added python 3.12 support
+- removed python 3.7 support
+- updated dependencies
+
+## [1.5.0] - 2023-03-13
+- added python 3.10/3.11 support
+- removed python 3.6 support
+- update dependencies
+
+## [1.4.2] - 2020-11-25
+- add binary releases to PyPI (Xie Yanbo)
+- update dependencies
+
+## [1.4.1] - 2020-09-30
+- fix issue with fat option in cython version
+- updated dependencies
+
+## [1.4.0] - 2020-08-08
+- add support for multiple path with scan command
+- fix issue with building cython extension
+- fix issue with fat option
+- fix zero-devision error
+
+## [1.3.0] - 2020-06-26
+- add new `scan` command to calculate deduplication ratio for directories
+
+## [1.2.0] - 2020-05-23
+
+### Added
+- faster optional cython implementation
+- benchmark command
+
+## [1.1.0] - 2020-05-09
+
+### Added
+- high-level API
+- support for streams
+- support for custom hash functions
 
-packages = \
-['fastcdc']
 
-package_data = \
-{'': ['*']}
+## [1.0.0] - 2020-05-07
+
+### Added
+- Initial release (port of [nlfiedler/fastcdc-rs](https://github.com/nlfiedler/fastcdc-rs)).
 
-install_requires = \
-['click-default-group>=1.2,<2.0',
- 'click>=8.1,<9.0',
- 'codetiming>=1.2,<2.0',
- 'humanize>=4.0,<5.0',
- 'py-cpuinfo>=9.0,<10.0']
-
-extras_require = \
-{'hashes': ['xxhash>=3.0,<4.0', 'blake3>=0.3,<0.4']}
-
-entry_points = \
-{'console_scripts': ['fastcdc = fastcdc.cli:cli']}
-
-setup_kwargs = {
-    'name': 'fastcdc',
-    'version': '1.5.0',
-    'description': 'FastCDC (content defined chunking) in pure Python.',
-    'long_description': '# FastCDC\n\n[![Tests](https://github.com/titusz/fastcdc-py/workflows/Tests/badge.svg)](https://github.com/titusz/fastcdc-py/actions?query=workflow%3ATests)\n[![Version](https://img.shields.io/pypi/v/fastcdc.svg)](https://pypi.python.org/pypi/fastcdc/)\n[![Downloads](https://pepy.tech/badge/fastcdc)](https://pepy.tech/project/fastcdc)\n\nThis package implements the "FastCDC" content defined chunking algorithm in\nPython with optional cython support. To learn more about content\ndefined chunking and its applications, see the reference material linked below.\n\n\n## Requirements\n\n* [Python](https://www.python.org/) Version 3.7 and later. Tested on Linux, Mac and\nWindows\n\n## Installing\n\n```shell\n$ pip install fastcdc\n```\n\nTo enable add additional support for the hash algorithms\n([xxhash](https://github.com/Cyan4973/xxHash) and\n[blake3](https://github.com/BLAKE3-team/BLAKE3/)) use\n\n```shell\n$ pip install fastcdc[hashes]\n```\n\n## Usage\n\n### Calculate chunks with default settings:\n```shell\n$ fastcdc tests/SekienAkashita.jpg\nhash=103159aa68bb1ea98f64248c647b8fe9a303365d80cb63974a73bba8bc3167d7 offset=0 size=22366\nhash=3f2b58dc77982e763e75db76c4205aaab4e18ff8929e298ca5c58500fee5530d offset=22366 size=10491\nhash=fcfb2f49ccb2640887a74fad1fb8a32368b5461a9dccc28f29ddb896b489b913 offset=32857 size=14094\nhash=bd1198535cdb87c5571378db08b6e886daf810873f5d77000a54795409464138 offset=46951 size=18696\nhash=d6347a2e5bf586d42f2d80559d4f4a2bf160dce8f77eede023ad2314856f3086 offset=65647 size=43819\n```\n\n### Customize min-size, avg-size, max-size, and hash function\n```shell\n$ fastcdc -mi 16384 -s 32768 -ma 65536 -hf sha256 tests/SekienAkashita.jpg\nhash=5a80871bad4588c7278d39707fe68b8b174b1aa54c59169d3c2c72f1e16ef46d offset=0 size=32857\nhash=13f6a4c6d42df2b76c138c13e86e1379c203445055c2b5f043a5f6c291fa520d offset=32857 size=16408\nhash=0fe7305ba21a5a5ca9f89962c5a6f3e29cd3e2b36f00e565858e0012e5f8df36 offset=49265 size=60201\n```\n\n###  Scan files in directory and report duplication.\n```shell\n$ fastcdc scan ~/Downloads\n[####################################]  100%\nFiles:          1,332\nChunk Sizes:    min 4096 - avg 16384 - max 131072\nUnique Chunks:  506,077\nTotal Data:     9.3 GB\nDupe Data:      873.8 MB\nDeDupe Ratio:   9.36 %\nThroughput:     135.2 MB/s\n```\n\n### Show help\n\n```shell\n$ fastcdc\nUsage: fastcdc [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --version  Show the version and exit.\n  --help     Show this message and exit.\n\nCommands:\n  chunkify*  Find variable sized chunks for FILE and compute hashes.\n  benchmark  Benchmark chunking performance.\n  scan       Scan files in directory and report duplication.\n```\n\n### Use from your python code\nThe  tests also have some short examples of using the chunker, of which this\ncode snippet is an example:\n\n```python\nfrom fastcdc import fastcdc\n\nresults = list(fastcdc("tests/SekienAkashita.jpg", 16384, 32768, 65536))\nassert len(results) == 3\nassert results[0].offset == 0\nassert results[0].length == 32857\nassert results[1].offset == 32857\nassert results[1].length == 16408\nassert results[2].offset == 49265\nassert results[2].length == 60201\n```\n\n## Reference Material\n\nThe algorithm is as described in "FastCDC: a Fast and Efficient Content-Defined\nChunking Approach for Data Deduplication"; see the\n[paper](https://www.usenix.org/system/files/conference/atc16/atc16-paper-xia.pdf),\nand\n[presentation](https://www.usenix.org/sites/default/files/conference/protected-files/atc16_slides_xia.pdf)\nfor details. There are some minor differences, as described below.\n\n### Differences with the FastCDC paper\n\nThe explanation below is copied from\n[ronomon/deduplication](https://github.com/ronomon/deduplication) since this\ncodebase is little more than a translation of that implementation:\n\n> The following optimizations and variations on FastCDC are involved in the chunking algorithm:\n> * 31 bit integers to avoid 64 bit integers for the sake of the Javascript reference implementation.\n> * A right shift instead of a left shift to remove the need for an additional modulus operator, which would otherwise have been necessary to prevent overflow.\n> * Masks are no longer zero-padded since a right shift is used instead of a left shift.\n> * A more adaptive threshold based on a combination of average and minimum chunk size (rather than just average chunk size) to decide the pivot point at which to switch masks. A larger minimum chunk size now switches from the strict mask to the eager mask earlier.\n> * Masks use 1 bit of chunk size normalization instead of 2 bits of chunk size normalization.\n\nThe primary objective of this codebase was to have a Python implementation with a\npermissive license, which could be used for new projects, without concern for\ndata parity with existing implementations.\n\n## Prior Art\n\nThis package started as Python port of the implementation by Nathan Fiedler (see the\nnlfiedler link below).\n\n* [nlfiedler/fastcdc-rs](https://github.com/nlfiedler/fastcdc-rs)\n    + Rust implementation on which this code is based.\n* [ronomon/deduplication](https://github.com/ronomon/deduplication)\n    + C++ and JavaScript implementation on which the rust implementation is based.\n* [rdedup_cdc at docs.rs](https://docs.rs/crate/rdedup-cdc/0.1.0/source/src/fastcdc.rs)\n    + An alternative implementation of FastCDC to the one in this crate.\n* [jrobhoward/quickcdc](https://github.com/jrobhoward/quickcdc)\n    + Similar but slightly earlier algorithm by some of the same researchers.\n\n## Change Log\n\n## [1.5.0] - 2023-03-13\n- added python 3.10/3.11 support\n- removed python 3.6 support\n- update dependencies\n\n## [1.4.2] - 2020-11-25\n- add binary releases to PyPI (Xie Yanbo)\n- update dependencies\n\n## [1.4.1] - 2020-09-30\n- fix issue with fat option in cython version\n- updated dependencies\n\n## [1.4.0] - 2020-08-08\n- add support for multiple path with scan command\n- fix issue with building cython extension\n- fix issue with fat option\n- fix zero-devision error\n\n## [1.3.0] - 2020-06-26\n- add new `scan` command to calculate deduplication ratio for directories\n\n## [1.2.0] - 2020-05-23\n\n### Added\n- faster optional cython implementation\n- benchmark command\n\n## [1.1.0] - 2020-05-09\n\n### Added\n- high-level API\n- support for streams\n- support for custom hash functions\n\n\n## [1.0.0] - 2020-05-07\n\n### Added\n- Initial release (port of [nlfiedler/fastcdc-rs](https://github.com/nlfiedler/fastcdc-rs)).\n\n',
-    'author': 'Titusz Pan',
-    'author_email': 'tp@py7.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/iscc/fastcdc-py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.2,<4.0',
-}
-from build import *
-build(setup_kwargs)
 
-setup(**setup_kwargs)
```


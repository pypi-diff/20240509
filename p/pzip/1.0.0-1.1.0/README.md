# Comparing `tmp/pzip-1.0.0.tar.gz` & `tmp/pzip-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pzip-1.0.0.tar", last modified: Thu Mar  9 14:30:15 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pzip-1.0.0.tar` & `pzip-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2023-03-09 14:30:15.776406 pzip-1.0.0/
--rw-r--r--   0 dcwatson   (501) staff       (20)     1094 2022-08-26 01:13:55.000000 pzip-1.0.0/LICENSE
--rw-r--r--   0 dcwatson   (501) staff       (20)     3931 2023-03-09 14:30:15.776482 pzip-1.0.0/PKG-INFO
--rw-r--r--   0 dcwatson   (501) staff       (20)     3269 2022-08-26 01:13:55.000000 pzip-1.0.0/README.md
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2023-03-09 14:30:15.775521 pzip-1.0.0/pzip/
--rw-r--r--   0 dcwatson   (501) staff       (20)      881 2023-03-09 14:27:37.000000 pzip-1.0.0/pzip/__init__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)       61 2022-08-26 01:13:55.000000 pzip-1.0.0/pzip/__main__.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     8013 2023-03-09 14:13:28.000000 pzip-1.0.0/pzip/base.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     9632 2023-03-09 14:20:28.000000 pzip-1.0.0/pzip/cli.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     8903 2022-08-26 01:13:55.000000 pzip-1.0.0/pzip/reader.py
--rw-r--r--   0 dcwatson   (501) staff       (20)     4671 2023-03-09 14:13:28.000000 pzip-1.0.0/pzip/writer.py
-drwxr-xr-x   0 dcwatson   (501) staff       (20)        0 2023-03-09 14:30:15.776286 pzip-1.0.0/pzip.egg-info/
--rw-r--r--   0 dcwatson   (501) staff       (20)     3931 2023-03-09 14:30:15.000000 pzip-1.0.0/pzip.egg-info/PKG-INFO
--rw-r--r--   0 dcwatson   (501) staff       (20)      295 2023-03-09 14:30:15.000000 pzip-1.0.0/pzip.egg-info/SOURCES.txt
--rw-r--r--   0 dcwatson   (501) staff       (20)        1 2023-03-09 14:30:15.000000 pzip-1.0.0/pzip.egg-info/dependency_links.txt
--rw-r--r--   0 dcwatson   (501) staff       (20)       39 2023-03-09 14:30:15.000000 pzip-1.0.0/pzip.egg-info/entry_points.txt
--rw-r--r--   0 dcwatson   (501) staff       (20)       65 2023-03-09 14:30:15.000000 pzip-1.0.0/pzip.egg-info/requires.txt
--rw-r--r--   0 dcwatson   (501) staff       (20)        5 2023-03-09 14:30:15.000000 pzip-1.0.0/pzip.egg-info/top_level.txt
--rw-r--r--   0 dcwatson   (501) staff       (20)       94 2023-03-09 14:30:15.776697 pzip-1.0.0/setup.cfg
--rw-r--r--   0 dcwatson   (501) staff       (20)     1204 2023-03-09 14:22:34.000000 pzip-1.0.0/setup.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pzip-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pzip-1.1.0/.python-version
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pzip-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pzip-1.1.0/mkdocs.yml
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 pzip-1.1.0/requirements-dev.lock
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pzip-1.1.0/requirements.lock
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 pzip-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 pzip-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 pzip-1.1.0/docs/encryption.md
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 pzip-1.1.0/docs/format.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 pzip-1.1.0/docs/index.md
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 pzip-1.1.0/src/pzip/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pzip-1.1.0/src/pzip/__main__.py
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 pzip-1.1.0/src/pzip/base.py
+-rw-r--r--   0        0        0     9216 2020-02-02 00:00:00.000000 pzip-1.1.0/src/pzip/cli.py
+-rw-r--r--   0        0        0     8903 2020-02-02 00:00:00.000000 pzip-1.1.0/src/pzip/reader.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 pzip-1.1.0/src/pzip/writer.py
+-rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 pzip-1.1.0/tests/test_pzip.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pzip-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pzip-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 pzip-1.1.0/README.md
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 pzip-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 pzip-1.1.0/PKG-INFO
```

### Comparing `pzip-1.0.0/LICENSE` & `pzip-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pzip-1.0.0/PKG-INFO` & `pzip-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pzip
-Version: 1.0.0
+Version: 1.1.0
 Summary: Crytographically secure file compression.
-Home-page: https://github.com/imsweb/pzip
-Author: Dan Watson
-Author-email: watsond@imsweb.com
+Project-URL: Homepage, https://github.com/imsweb/pzip
+Author-email: Dan Watson <watsond@imsweb.com>
 License: MIT
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Archiving :: Compression
-Description-Content-Type: text/markdown
+Requires-Python: >=3.8
+Requires-Dist: cryptography
 Provides-Extra: deflate
-Provides-Extra: tqdm
-Provides-Extra: all
-License-File: LICENSE
+Requires-Dist: deflate; extra == 'deflate'
+Description-Content-Type: text/markdown
 
 ![CI](https://github.com/imsweb/pzip/workflows/CI/badge.svg?branch=master)
 
 # PZip
 
 PZip is an encrypted file format (with optional compression), a command-line tool, and a Python file-like interface.
```

### Comparing `pzip-1.0.0/README.md` & `pzip-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pzip-1.0.0/pzip/__init__.py` & `pzip-1.1.0/src/pzip/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     PZip,
     RawKey,
     Tag,
 )
 from .reader import PZipReader
 from .writer import PZipWriter
 
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 __version_info__ = tuple(int(num) for num in __version__.split("."))
 
 
 def open(fileobj, mode="rb", *, key=None, **kwargs):
     if isinstance(fileobj, (str, int)):
         fileobj = builtins.open(fileobj, mode)
     if "r" in mode:
```

### Comparing `pzip-1.0.0/pzip/base.py` & `pzip-1.1.0/src/pzip/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 from cryptography.hazmat.primitives.kdf.hkdf import HKDF
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 
 try:
-    import deflate
+    import deflate  # pyright: ignore[reportMissingImports]
 
     gzip_compress = deflate.gzip_compress
     gzip_decompress = deflate.gzip_decompress
 except ImportError:
     gzip_compress = gzip.compress
     gzip_decompress = gzip.decompress
 
@@ -38,15 +38,15 @@
 
 
 class InvalidFile(Exception):
     pass
 
 
 # Number of PBKDF2 iterations to use by default. May increase over time.
-DEFAULT_ITERATIONS = 200000
+DEFAULT_ITERATIONS = 600_000
 
 
 class Flag(enum.IntFlag):
     APPEND_LENGTH = 1 << 0
 
 
 class BlockFlag(enum.IntFlag):
@@ -231,26 +231,26 @@
 
 class Password(KeyMaterial):
     kdf = KeyDerivation.PBKDF2_SHA256
 
 
 class PZip(io.RawIOBase):
     # First two bytes of any PZIP file.
-    MAGIC = b"\xB6\x9E"  # ¶ž
+    MAGIC = b"\xb6\x9e"  # ¶ž
 
     # PZip header format (for struct):
     # magic, version, flags, algorithm, kdf, compression, #tags
     HEADER_FORMAT = "!2s6B"
 
     # PZip header size.
     HEADER_SIZE = struct.calcsize(HEADER_FORMAT)
 
     # Default plaintext block size when encrypting.
-    # Benchmarking suggests that block sizes in the 256k-1MB range perform best.
-    DEFAULT_BLOCK_SIZE = 2**18  # 256k
+    # Benchmarking suggests that block sizes in the 128k-1MB range perform best.
+    DEFAULT_BLOCK_SIZE = 2**17  # 128k
 
     def __init__(
         self,
         fileobj,
         name=None,
         close=Close.AUTOMATIC,
     ):
```

### Comparing `pzip-1.0.0/pzip/cli.py` & `pzip-1.1.0/src/pzip/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 import argparse
 import getpass
 import io
 import os
 import secrets
 import sys
 
-try:
-    import tqdm
-
-    has_tqdm = True
-except ImportError:
-    has_tqdm = False
-
 from .base import InvalidFile, PZip
 from .reader import PZipReader
 from .writer import PZipWriter
 
 
 def log(msg, *args):
     print(msg.format(*args), file=sys.stderr, flush=True)
@@ -261,25 +254,14 @@
         key = getpass.getpass("Password: ")
         if mode == "wb":
             verify = getpass.getpass("Verify: ")
             if verify != key:
                 die("passwords did not match")
     for filename in files:
         infile, outfile, total = get_files(filename, mode, key, options)
-        progress = (
-            tqdm.tqdm(
-                desc=filename,
-                total=total,
-                unit="B",
-                unit_scale=True,
-                unit_divisor=1024,
-            )
-            if has_tqdm and filename and total and not options.quiet
-            else None
-        )
-        copy(infile, outfile, progress=progress)
+        copy(infile, outfile)
         if filename and not options.keep:
             os.remove(filename)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pzip-1.0.0/pzip/reader.py` & `pzip-1.1.0/src/pzip/reader.py`

 * *Files identical despite different names*

### Comparing `pzip-1.0.0/pzip/writer.py` & `pzip-1.1.0/src/pzip/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self,
         fileobj,
         key,
         nonce=None,
         block_size=None,
         append_length=True,
         compress=None,
-        **kwargs
+        **kwargs,
     ):
         key = KeyMaterial.resolve(key)
         super().__init__(fileobj, **kwargs)
         # Set the KDF that was used, if any.
         self.kdf = key.kdf
         # Set the compression algorithm and level, if any.
         self.compression, self.compresslevel = Compression.resolve(compress)
```


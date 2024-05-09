# Comparing `tmp/ig_trading_lib-0.3.0.tar.gz` & `tmp/ig_trading_lib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ig_trading_lib-0.3.0.tar", max compression
+gzip compressed data, was "ig_trading_lib-0.4.0.tar", max compression
```

## Comparing `ig_trading_lib-0.3.0.tar` & `ig_trading_lib-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1071 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/LICENSE
--rw-r--r--   0        0        0     1310 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/README.md
--rw-r--r--   0        0        0      278 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/__init__.py
--rw-r--r--   0        0        0      136 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__init__.py
--rw-r--r--   0        0        0      296 2024-04-07 21:42:39.687569 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5065 2024-04-07 21:42:39.863568 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/cache.cpython-39.pyc
--rw-r--r--   0        0        0     1927 2024-04-07 21:42:39.879568 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     4752 2024-04-07 21:42:39.691569 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/service.cpython-39.pyc
--rw-r--r--   0        0        0     4636 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/authentication/cache.py
--rw-r--r--   0        0        0     1117 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/authentication/models.py
--rw-r--r--   0        0        0     4578 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/authentication/service.py
--rw-r--r--   0        0        0        0 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/markets/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/__init__.py
--rw-r--r--   0        0        0      173 2024-04-07 21:42:40.215566 ig_trading_lib-0.3.0/ig_trading_lib/trading/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      850 2024-04-07 21:42:40.223566 ig_trading_lib-0.3.0/ig_trading_lib/trading/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0      643 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/models.py
--rw-r--r--   0        0        0      134 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__init__.py
--rw-r--r--   0        0        0      345 2024-04-07 21:42:40.215566 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5424 2024-04-07 21:42:40.215566 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     2732 2024-04-07 21:42:40.247566 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/service.cpython-39.pyc
--rw-r--r--   0        0        0     5097 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/models.py
--rw-r--r--   0        0        0     2531 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/service.py
--rw-r--r--   0        0        0      315 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__init__.py
--rw-r--r--   0        0        0      452 2024-04-07 21:42:40.295566 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    10549 2024-04-07 21:42:40.299566 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     5566 2024-04-07 21:42:40.327566 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/service.cpython-39.pyc
--rw-r--r--   0        0        0    11119 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/models.py
--rw-r--r--   0        0        0     5901 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/service.py
--rw-r--r--   0        0        0      547 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 ig_trading_lib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-09 20:22:51.269169 ig_trading_lib-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1310 2024-05-09 20:22:51.269169 ig_trading_lib-0.4.0/README.md
+-rw-r--r--   0        0        0      278 2024-05-09 20:22:51.269169 ig_trading_lib-0.4.0/ig_trading_lib/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:22:51.269169 ig_trading_lib-0.4.0/ig_trading_lib/account/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-09 20:22:51.269169 ig_trading_lib-0.4.0/ig_trading_lib/authentication/__init__.py
+-rw-r--r--   0        0        0      296 2024-05-09 20:23:08.969148 ig_trading_lib-0.4.0/ig_trading_lib/authentication/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5065 2024-05-09 20:23:09.149147 ig_trading_lib-0.4.0/ig_trading_lib/authentication/__pycache__/cache.cpython-39.pyc
+-rw-r--r--   0        0        0     1927 2024-05-09 20:23:09.169147 ig_trading_lib-0.4.0/ig_trading_lib/authentication/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     4752 2024-05-09 20:23:08.969148 ig_trading_lib-0.4.0/ig_trading_lib/authentication/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0        0        0     4636 2024-05-09 20:22:51.269169 ig_trading_lib-0.4.0/ig_trading_lib/authentication/cache.py
+-rw-r--r--   0        0        0     1117 2024-05-09 20:22:51.269169 ig_trading_lib-0.4.0/ig_trading_lib/authentication/models.py
+-rw-r--r--   0        0        0     4578 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/authentication/service.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/markets/__init__.py
+-rw-r--r--   0        0        0      145 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/trading/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-09 20:23:09.393147 ig_trading_lib-0.4.0/ig_trading_lib/trading/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      850 2024-05-09 20:23:09.401147 ig_trading_lib-0.4.0/ig_trading_lib/trading/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0      643 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/trading/models.py
+-rw-r--r--   0        0        0      134 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/__init__.py
+-rw-r--r--   0        0        0      345 2024-05-09 20:23:09.433147 ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5424 2024-05-09 20:23:09.437147 ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     3578 2024-05-09 20:23:09.457147 ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0        0        0     5097 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/models.py
+-rw-r--r--   0        0        0     3539 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/service.py
+-rw-r--r--   0        0        0      315 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/__init__.py
+-rw-r--r--   0        0        0      452 2024-05-09 20:23:09.393147 ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    10628 2024-05-09 20:23:09.393147 ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     5721 2024-05-09 20:23:09.433147 ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0        0        0    11195 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/models.py
+-rw-r--r--   0        0        0     6041 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/service.py
+-rw-r--r--   0        0        0      547 2024-05-09 20:22:51.273169 ig_trading_lib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 ig_trading_lib-0.4.0/PKG-INFO
```

### Comparing `ig_trading_lib-0.3.0/LICENSE` & `ig_trading_lib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.3.0/README.md` & `ig_trading_lib-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/cache.cpython-39.pyc` & `ig_trading_lib-0.4.0/ig_trading_lib/authentication/__pycache__/cache.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  7 21:42:19 2024 UTC, .py size: 4636 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3b13 1366 1c12 0000  a.......;..f....
+00000000: 610d 0d0a 0000 0000 9b30 3d66 1c12 0000  a........0=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6406 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -34,16 +34,16 @@
 00000210: 0074 0064 0183 0182 0164 0053 0029 024e  .t.d.....d.S.).N
 00000220: 7a29 496d 706c 656d 656e 7420 4175 7468  z)Implement Auth
 00000230: 6f72 697a 6174 696f 6e20 7265 7370 6f6e  orization respon
 00000240: 7365 2063 6163 6869 6e67 21a9 01da 134e  se caching!....N
 00000250: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
 00000260: 6f72 a901 720c 0000 00a9 0072 1100 0000  or..r......r....
 00000270: fa56 2f68 6f6d 652f 7275 6e6e 6572 2f77  .V/home/runner/w
-00000280: 6f72 6b2f 6967 5f74 7261 6469 6e67 5f6c  ork/ig_trading_l
-00000290: 6962 2f69 675f 7472 6164 696e 675f 6c69  ib/ig_trading_li
+00000280: 6f72 6b2f 6967 2d74 7261 6469 6e67 2d6c  ork/ig-trading-l
+00000290: 6962 2f69 672d 7472 6164 696e 672d 6c69  ib/ig-trading-li
 000002a0: 622f 6967 5f74 7261 6469 6e67 5f6c 6962  b/ig_trading_lib
 000002b0: 2f61 7574 6865 6e74 6963 6174 696f 6e2f  /authentication/
 000002c0: 6361 6368 652e 7079 da1c 7361 7665 5f61  cache.py..save_a
 000002d0: 7574 6865 6e74 6963 6174 696f 6e5f 7265  uthentication_re
 000002e0: 7370 6f6e 7365 1200 0000 7302 0000 0000  sponse....s.....
 000002f0: 037a 3341 7574 6865 6e74 6963 6174 696f  .z3Authenticatio
 00000300: 6e43 6163 6865 4142 432e 7361 7665 5f61  nCacheABC.save_a
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/models.cpython-39.pyc` & `ig_trading_lib-0.4.0/ig_trading_lib/authentication/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  7 21:42:19 2024 UTC, .py size: 1117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3b13 1366 5d04 0000  a.......;..f]...
+00000000: 610d 0d0a 0000 0000 9b30 3d66 5d04 0000  a........0=f]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6501 6404 6405 6406 6702  m.Z...e.d.d.d.g.
 00000060: 8302 5a07 4700 6407 6408 8400 6408 6506  ..Z.G.d.d...d.e.
 00000070: 8303 5a08 4700 6409 640a 8400 640a 6506  ..Z.G.d.d...d.e.
@@ -24,17 +24,17 @@
 00000170: 6f73 6974 5a0a 7072 6f66 6974 4c6f 7373  ositZ.profitLoss
 00000180: da09 6176 6169 6c61 626c 654e 2905 da08  ..availableN)...
 00000190: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
 000001a0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 000001b0: 5f5f da05 666c 6f61 74da 0f5f 5f61 6e6e  __..float..__ann
 000001c0: 6f74 6174 696f 6e73 5f5f a900 7210 0000  otations__..r...
 000001d0: 0072 1000 0000 fa57 2f68 6f6d 652f 7275  .r.....W/home/ru
-000001e0: 6e6e 6572 2f77 6f72 6b2f 6967 5f74 7261  nner/work/ig_tra
-000001f0: 6469 6e67 5f6c 6962 2f69 675f 7472 6164  ding_lib/ig_trad
-00000200: 696e 675f 6c69 622f 6967 5f74 7261 6469  ing_lib/ig_tradi
+000001e0: 6e6e 6572 2f77 6f72 6b2f 6967 2d74 7261  nner/work/ig-tra
+000001f0: 6469 6e67 2d6c 6962 2f69 672d 7472 6164  ding-lib/ig-trad
+00000200: 696e 672d 6c69 622f 6967 5f74 7261 6469  ing-lib/ig_tradi
 00000210: 6e67 5f6c 6962 2f61 7574 6865 6e74 6963  ng_lib/authentic
 00000220: 6174 696f 6e2f 6d6f 6465 6c73 2e70 7972  ation/models.pyr
 00000230: 0900 0000 0a00 0000 7308 0000 000a 0108  ........s.......
 00000240: 0108 0108 0172 0900 0000 6300 0000 0000  .....r....c.....
 00000250: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
 00000260: 0000 0073 2e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
 00000270: 5500 6503 6504 6401 3c00 6503 6504 6402  U.e.e.d.<.e.e.d.
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/service.cpython-39.pyc` & `ig_trading_lib-0.4.0/ig_trading_lib/authentication/__pycache__/service.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  7 21:42:19 2024 UTC, .py size: 4578 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3b13 1366 e211 0000  a.......;..f....
+00000000: 610d 0d0a 0000 0000 9b30 3d66 e211 0000  a........0=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6401 6c04 5a04 6400 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6405 6406 6c07 6d08 5a08 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6407 6c09 6d0a 5a0a 0100 6500 a00b 650c  d.l.m.Z...e...e.
@@ -24,16 +24,16 @@
 00000170: 726f 7273 2069 6e20 7468 6520 6175 7468  rors in the auth
 00000180: 656e 7469 6361 7469 6f6e 2070 726f 6365  entication proce
 00000190: 7373 2e4e 2904 da08 5f5f 6e61 6d65 5f5f  ss.N)...__name__
 000001a0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 000001b0: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
 000001c0: 635f 5fa9 0072 0d00 0000 720d 0000 00fa  c__..r....r.....
 000001d0: 582f 686f 6d65 2f72 756e 6e65 722f 776f  X/home/runner/wo
-000001e0: 726b 2f69 675f 7472 6164 696e 675f 6c69  rk/ig_trading_li
-000001f0: 622f 6967 5f74 7261 6469 6e67 5f6c 6962  b/ig_trading_lib
+000001e0: 726b 2f69 672d 7472 6164 696e 672d 6c69  rk/ig-trading-li
+000001f0: 622f 6967 2d74 7261 6469 6e67 2d6c 6962  b/ig-trading-lib
 00000200: 2f69 675f 7472 6164 696e 675f 6c69 622f  /ig_trading_lib/
 00000210: 6175 7468 656e 7469 6361 7469 6f6e 2f73  authentication/s
 00000220: 6572 7669 6365 2e70 7972 0800 0000 0f00  ervice.pyr......
 00000230: 0000 7302 0000 0008 0172 0800 0000 6300  ..s......r....c.
 00000240: 0000 0000 0000 0000 0000 0000 0000 0007  ................
 00000250: 0000 0040 0000 0073 ae00 0000 6500 5a01  ...@...s....e.Z.
 00000260: 6400 5a02 6401 5a03 6418 6504 6504 6504  d.Z.d.Z.d.e.e.e.
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/authentication/cache.py` & `ig_trading_lib-0.4.0/ig_trading_lib/authentication/cache.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/authentication/models.py` & `ig_trading_lib-0.4.0/ig_trading_lib/authentication/models.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/authentication/service.py` & `ig_trading_lib-0.4.0/ig_trading_lib/authentication/service.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/__pycache__/models.cpython-39.pyc` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  7 21:42:19 2024 UTC, .py size: 643 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3b13 1366 8302 0000  a.......;..f....
+00000000: 610d 0d0a 0000 0000 9b30 3d66 8302 0000  a........0=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6503 8303 5a04 6501 6405 1900 5a05 6501  e...Z.e.d...Z.e.
 00000060: 6406 1900 5a06 6407 5300 2908 e900 0000  d...Z.d.S.).....
 00000070: 0029 01da 074c 6974 6572 616c 2901 da09  .)...Literal)...
@@ -13,17 +13,17 @@
 000000c0: 0d44 6561 6c52 6566 6572 656e 6365 da0d  .DealReference..
 000000d0: 6465 616c 5265 6665 7265 6e63 654e 2905  dealReferenceN).
 000000e0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 000000f0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 00000100: 6d65 5f5f da03 7374 72da 0f5f 5f61 6e6e  me__..str..__ann
 00000110: 6f74 6174 696f 6e73 5f5f a900 720b 0000  otations__..r...
 00000120: 0072 0b00 0000 fa50 2f68 6f6d 652f 7275  .r.....P/home/ru
-00000130: 6e6e 6572 2f77 6f72 6b2f 6967 5f74 7261  nner/work/ig_tra
-00000140: 6469 6e67 5f6c 6962 2f69 675f 7472 6164  ding_lib/ig_trad
-00000150: 696e 675f 6c69 622f 6967 5f74 7261 6469  ing_lib/ig_tradi
+00000130: 6e6e 6572 2f77 6f72 6b2f 6967 2d74 7261  nner/work/ig-tra
+00000140: 6469 6e67 2d6c 6962 2f69 672d 7472 6164  ding-lib/ig-trad
+00000150: 696e 672d 6c69 622f 6967 5f74 7261 6469  ing-lib/ig_tradi
 00000160: 6e67 5f6c 6962 2f74 7261 6469 6e67 2f6d  ng_lib/trading/m
 00000170: 6f64 656c 732e 7079 7204 0000 0005 0000  odels.pyr.......
 00000180: 0073 0200 0000 0a01 7204 0000 0029 175a  .s......r....).Z
 00000190: 0653 4841 5245 535a 0642 494e 4152 595a  .SHARESZ.BINARYZ
 000001a0: 0d42 554e 4745 455f 4341 5050 4544 5a12  .BUNGEE_CAPPEDZ.
 000001b0: 4255 4e47 4545 5f43 4f4d 4d4f 4449 5449  BUNGEE_COMMODITI
 000001c0: 4553 5a11 4255 4e47 4545 5f43 5552 5245  ESZ.BUNGEE_CURRE
@@ -39,15 +39,15 @@
 00000260: 4f4d 4d4f 4449 5449 4553 5a0e 4f50 545f  OMMODITIESZ.OPT_
 00000270: 4355 5252 454e 4349 4553 5a0b 4f50 545f  CURRENCIESZ.OPT_
 00000280: 494e 4449 4345 535a 094f 5054 5f52 4154  INDICESZ.OPT_RAT
 00000290: 4553 5a0a 4f50 545f 5348 4152 4553 5a05  ESZ.OPT_SHARESZ.
 000002a0: 5241 5445 535a 0753 4543 544f 5253 5a0d  RATESZ.SECTORSZ.
 000002b0: 5350 5249 4e54 5f4d 4152 4b45 545a 0b54  SPRINT_MARKETZ.T
 000002c0: 4553 545f 4d41 524b 4554 da07 554e 4b4e  EST_MARKET..UNKN
-000002d0: 4f57 4e29 025a 0342 5559 da04 5345 4c4c  OWN).Z.BUY..SELL
+000002d0: 4f57 4e29 02da 0342 5559 da04 5345 4c4c  OWN)...BUY..SELL
 000002e0: 4e29 07da 0674 7970 696e 6772 0200 0000  N)...typingr....
 000002f0: da08 7079 6461 6e74 6963 7203 0000 0072  ..pydanticr....r
 00000300: 0400 0000 da0e 496e 7374 7275 6d65 6e74  ......Instrument
 00000310: 5479 7065 da09 4469 7265 6374 696f 6e72  Type..Directionr
 00000320: 0b00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
 00000330: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
 00000340: 0073 0c00 0000 0c01 0c03 1004 0201 02ff  .s..............
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/models.py` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/models.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/models.cpython-39.pyc` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  7 21:42:19 2024 UTC, .py size: 5097 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3b13 1366 e913 0000  a.......;..f....
+00000000: 610d 0d0a 0000 0000 9b30 3d66 e913 0000  a........0=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6405  m.Z.m.Z.m.Z...d.
@@ -24,19 +24,19 @@
 00000170: 6c5f 7661 6c69 6461 746f 72da 1066 6965  l_validator..fie
 00000180: 6c64 5f73 6572 6961 6c69 7a65 72e9 0200  ld_serializer...
 00000190: 0000 2902 da0e 496e 7374 7275 6d65 6e74  ..)...Instrument
 000001a0: 5479 7065 da09 4469 7265 6374 696f 6e29  Type..Direction)
 000001b0: 02da 054c 494d 4954 5a04 5354 4f50 2902  ...LIMITZ.STOP).
 000001c0: da13 474f 4f44 5f54 494c 4c5f 4341 4e43  ..GOOD_TILL_CANC
 000001d0: 454c 4c45 44da 0e47 4f4f 445f 5449 4c4c  ELLED..GOOD_TILL
-000001e0: 5f44 4154 4529 075a 0643 4c4f 5345 445a  _DATE).Z.CLOSEDZ
-000001f0: 0a45 4449 5453 5f4f 4e4c 595a 074f 4646  .EDITS_ONLYZ.OFF
-00000200: 4c49 4e45 5a0a 4f4e 5f41 5543 5449 4f4e  LINEZ.ON_AUCTION
-00000210: 5a13 4f4e 5f41 5543 5449 4f4e 5f4e 4f5f  Z.ON_AUCTION_NO_
-00000220: 4544 4954 535a 0953 5553 5045 4e44 4544  EDITSZ.SUSPENDED
+000001e0: 5f44 4154 4529 07da 0643 4c4f 5345 44da  _DATE)...CLOSED.
+000001f0: 0a45 4449 5453 5f4f 4e4c 59da 074f 4646  .EDITS_ONLY..OFF
+00000200: 4c49 4e45 da0a 4f4e 5f41 5543 5449 4f4e  LINE..ON_AUCTION
+00000210: da13 4f4e 5f41 5543 5449 4f4e 5f4e 4f5f  ..ON_AUCTION_NO_
+00000220: 4544 4954 53da 0953 5553 5045 4e44 4544  EDITS..SUSPENDED
 00000230: da09 5452 4144 4541 424c 4563 0000 0000  ..TRADEABLEc....
 00000240: 0000 0000 0000 0000 0000 0000 0300 0000  ................
 00000250: 4000 0000 73c8 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
 00000260: 0255 0065 0365 0464 013c 0065 0365 0464  .U.e.e.d.<.e.e.d
 00000270: 023c 0065 0365 0464 033c 0065 0565 0464  .<.e.e.d.<.e.e.d
 00000280: 043c 0065 0365 0464 053c 0065 0665 0464  .<.e.e.d.<.e.e.d
 00000290: 063c 0065 0764 0764 088d 0165 0464 093c  .<.e.d.d...e.d.<
@@ -65,25 +65,25 @@
 00000400: 6573 4176 6169 6c61 626c 65da 0d73 6361  esAvailable..sca
 00000410: 6c69 6e67 4661 6374 6f72 4e29 0ada 085f  lingFactorN)..._
 00000420: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000430: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
 00000440: 5fda 0373 7472 da0f 5f5f 616e 6e6f 7461  _..str..__annota
 00000450: 7469 6f6e 735f 5fda 0c4d 6172 6b65 7453  tions__..MarketS
 00000460: 7461 7475 7372 0f00 0000 7209 0000 00da  tatusr....r.....
-00000470: 0369 6e74 da04 626f 6f6c a900 7232 0000  .int..bool..r2..
-00000480: 0072 3200 0000 fa57 2f68 6f6d 652f 7275  .r2....W/home/ru
-00000490: 6e6e 6572 2f77 6f72 6b2f 6967 5f74 7261  nner/work/ig_tra
-000004a0: 6469 6e67 5f6c 6962 2f69 675f 7472 6164  ding_lib/ig_trad
-000004b0: 696e 675f 6c69 622f 6967 5f74 7261 6469  ing_lib/ig_tradi
+00000470: 0369 6e74 da04 626f 6f6c a900 7238 0000  .int..bool..r8..
+00000480: 0072 3800 0000 fa57 2f68 6f6d 652f 7275  .r8....W/home/ru
+00000490: 6e6e 6572 2f77 6f72 6b2f 6967 2d74 7261  nner/work/ig-tra
+000004a0: 6469 6e67 2d6c 6962 2f69 672d 7472 6164  ding-lib/ig-trad
+000004b0: 696e 672d 6c69 622f 6967 5f74 7261 6469  ing-lib/ig_tradi
 000004c0: 6e67 5f6c 6962 2f74 7261 6469 6e67 2f6f  ng_lib/trading/o
 000004d0: 7264 6572 732f 6d6f 6465 6c73 2e70 7972  rders/models.pyr
-000004e0: 1500 0000 2100 0000 7324 0000 000a 0108  ....!...s$......
+000004e0: 1b00 0000 2100 0000 7324 0000 000a 0108  ....!...s$......
 000004f0: 0108 0108 0108 0108 0108 010e 010e 010e  ................
 00000500: 010e 010e 010e 010e 0108 0108 0108 0108  ................
-00000510: 0172 1500 0000 6300 0000 0000 0000 0000  .r....c.........
+00000510: 0172 1b00 0000 6300 0000 0000 0000 0000  .r....c.........
 00000520: 0000 0000 0000 0005 0000 0040 0000 0073  ...........@...s
 00000530: 3401 0000 6500 5a01 6400 5a02 5500 6503  4...e.Z.d.Z.U.e.
 00000540: 6504 6401 3c00 6505 6504 6402 3c00 6503  e.d.<.e.e.d.<.e.
 00000550: 6504 6403 3c00 6506 6404 6405 8d01 6504  e.d.<.e.d.d...e.
 00000560: 6406 3c00 6506 6404 6405 8d01 6504 6407  d.<.e.d.d...e.d.
 00000570: 3c00 6507 6504 6408 3c00 6409 5a08 6509  <.e.e.d.<.d.Z.e.
 00000580: 650a 1900 6504 640a 3c00 6409 5a0b 6509  e...e.d.<.d.Z.e.
@@ -99,15 +99,15 @@
 00000620: 6509 6503 1900 6509 650a 1900 6417 9c02  e.e...e.e...d...
 00000630: 6418 6419 8404 8301 8301 5a14 6512 640c  d.d.......Z.e.d.
 00000640: 6415 6416 8d02 6513 6509 6503 1900 6509  d.d...e.e.e...e.
 00000650: 650a 1900 6417 9c02 641a 641b 8404 8301  e...d...d.d.....
 00000660: 8301 5a15 6409 5300 291c da10 576f 726b  ..Z.d.S.)...Work
 00000670: 696e 674f 7264 6572 4461 7461 da06 6465  ingOrderData..de
 00000680: 616c 4964 da09 6469 7265 6374 696f 6e72  alId..directionr
-00000690: 1a00 0000 720e 0000 0072 1c00 0000 da09  ....r....r......
+00000690: 2000 0000 720e 0000 0072 2200 0000 da09   ...r....r".....
 000006a0: 6f72 6465 7253 697a 65da 0a6f 7264 6572  orderSize..order
 000006b0: 4c65 7665 6cda 0b74 696d 6549 6e46 6f72  Level..timeInFor
 000006c0: 6365 4eda 0c67 6f6f 6454 696c 6c44 6174  ceN..goodTillDat
 000006d0: 65da 0f67 6f6f 6454 696c 6c44 6174 6549  e..goodTillDateI
 000006e0: 534f da0b 6372 6561 7465 6444 6174 65da  SO..createdDate.
 000006f0: 0e63 7265 6174 6564 4461 7465 5554 43da  .createdDateUTC.
 00000700: 0e67 7561 7261 6e74 6565 6453 746f 70da  .guaranteedStop.
@@ -125,72 +125,72 @@
 000007c0: 027c 019b 009d 0283 0182 0159 006e 0230  .|.........Y.n.0
 000007d0: 0064 0053 0029 034e 7a0e 2559 2f25 6d2f  .d.S.).Nz.%Y/%m/
 000007e0: 2564 2025 483a 254d 7a2f 496e 7661 6c69  %d %H:%Mz/Invali
 000007f0: 6420 6461 7465 7469 6d65 2066 6f72 6d61  d datetime forma
 00000800: 7420 666f 7220 676f 6f64 5469 6c6c 4461  t for goodTillDa
 00000810: 7465 2076 616c 7565 20a9 0372 0200 0000  te value ..r....
 00000820: da08 7374 7270 7469 6d65 da0a 5661 6c75  ..strptime..Valu
-00000830: 6545 7272 6f72 a902 da03 636c 7372 4900  eError....clsrI.
-00000840: 0000 7232 0000 0072 3200 0000 7233 0000  ..r2...r2...r3..
+00000830: 6545 7272 6f72 a902 da03 636c 7372 4f00  eError....clsrO.
+00000840: 0000 7238 0000 0072 3800 0000 7239 0000  ..r8...r8...r9..
 00000850: 00da 1470 6172 7365 5f67 6f6f 645f 7469  ...parse_good_ti
 00000860: 6c6c 5f64 6174 6549 0000 0073 0a00 0000  ll_dateI...s....
 00000870: 0003 0801 0201 0e01 0c01 7a25 576f 726b  ..........z%Work
 00000880: 696e 674f 7264 6572 4461 7461 2e70 6172  ingOrderData.par
 00000890: 7365 5f67 6f6f 645f 7469 6c6c 5f64 6174  se_good_till_dat
 000008a0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
 000008b0: 0000 0800 0000 4300 0000 7334 0000 007a  ......C...s4...z
 000008c0: 0e74 00a0 017c 0164 01a1 0257 0053 0004  .t...|.d...W.S..
 000008d0: 0074 0279 2e01 0001 0001 0074 0264 027c  .t.y.......t.d.|
 000008e0: 019b 009d 0283 0182 0159 006e 0230 0064  .........Y.n.0.d
 000008f0: 0053 0029 034e 7a14 2559 2f25 6d2f 2564  .S.).Nz.%Y/%m/%d
 00000900: 2025 483a 254d 3a25 533a 2566 7a2e 496e   %H:%M:%S:%fz.In
 00000910: 7661 6c69 6420 6461 7465 7469 6d65 2066  valid datetime f
 00000920: 6f72 6d61 7420 666f 7220 6372 6561 7465  ormat for create
-00000930: 6444 6174 6520 7661 6c75 6520 724b 0000  dDate value rK..
-00000940: 0072 4e00 0000 7232 0000 0072 3200 0000  .rN...r2...r2...
-00000950: 7233 0000 00da 1270 6172 7365 5f63 7265  r3.....parse_cre
+00000930: 6444 6174 6520 7661 6c75 6520 7251 0000  dDate value rQ..
+00000940: 0072 5400 0000 7238 0000 0072 3800 0000  .rT...r8...r8...
+00000950: 7239 0000 00da 1270 6172 7365 5f63 7265  r9.....parse_cre
 00000960: 6174 6564 5f64 6174 6552 0000 0073 0800  ated_dateR...s..
 00000970: 0000 0003 0201 0e01 0c01 7a23 576f 726b  ..........z#Work
 00000980: 696e 674f 7264 6572 4461 7461 2e70 6172  ingOrderData.par
 00000990: 7365 5f63 7265 6174 6564 5f64 6174 6529  se_created_date)
-000009a0: 1672 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
-000009b0: 722d 0000 0072 2e00 0000 7210 0000 0072  r-...r....r....r
+000009a0: 1672 3000 0000 7231 0000 0072 3200 0000  .r0...r1...r2...
+000009b0: 7233 0000 0072 3400 0000 7210 0000 0072  r3...r4...r....r
 000009c0: 0900 0000 da0b 5469 6d65 496e 466f 7263  ......TimeInForc
-000009d0: 6572 3a00 0000 7204 0000 0072 0200 0000  er:...r....r....
-000009e0: 723b 0000 0072 3100 0000 da09 4f72 6465  r;...r1.....Orde
-000009f0: 7254 7970 6572 4000 0000 7241 0000 0072  rTyper@...rA...r
-00000a00: 4300 0000 7244 0000 0072 0a00 0000 da0b  C...rD...r......
-00000a10: 636c 6173 736d 6574 686f 6472 5000 0000  classmethodrP...
-00000a20: 7251 0000 0072 3200 0000 7232 0000 0072  rQ...r2...r2...r
-00000a30: 3200 0000 7233 0000 0072 3400 0000 3600  2...r3...r4...6.
+000009d0: 6572 4000 0000 7204 0000 0072 0200 0000  er@...r....r....
+000009e0: 7241 0000 0072 3700 0000 da09 4f72 6465  rA...r7.....Orde
+000009f0: 7254 7970 6572 4600 0000 7247 0000 0072  rTyperF...rG...r
+00000a00: 4900 0000 724a 0000 0072 0a00 0000 da0b  I...rJ...r......
+00000a10: 636c 6173 736d 6574 686f 6472 5600 0000  classmethodrV...
+00000a20: 7257 0000 0072 3800 0000 7238 0000 0072  rW...r8...r8...r
+00000a30: 3800 0000 7239 0000 0072 3a00 0000 3600  8...r9...r:...6.
 00000a40: 0000 732e 0000 000a 0108 0108 0108 010e  ..s.............
 00000a50: 010e 0108 0110 0110 0108 0108 0108 0108  ................
 00000a60: 0116 0116 0108 0110 0116 020a 0102 011c  ................
-00000a70: 070a 0102 0172 3400 0000 6300 0000 0000  .....r4...c.....
+00000a70: 070a 0102 0172 3a00 0000 6300 0000 0000  .....r:...c.....
 00000a80: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
 00000a90: 0000 0073 1e00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
 00000aa0: 5500 6503 6504 6401 3c00 6505 6504 6402  U.e.e.d.<.e.e.d.
 00000ab0: 3c00 6403 5300 2904 da0c 576f 726b 696e  <.d.S.)...Workin
 00000ac0: 674f 7264 6572 da10 776f 726b 696e 674f  gOrder..workingO
 00000ad0: 7264 6572 4461 7461 da0a 6d61 726b 6574  rderData..market
-00000ae0: 4461 7461 4e29 0672 2a00 0000 722b 0000  DataN).r*...r+..
-00000af0: 0072 2c00 0000 7234 0000 0072 2e00 0000  .r,...r4...r....
-00000b00: 7215 0000 0072 3200 0000 7232 0000 0072  r....r2...r2...r
-00000b10: 3200 0000 7233 0000 0072 5500 0000 5b00  2...r3...rU...[.
-00000b20: 0000 7304 0000 000a 0108 0172 5500 0000  ..s........rU...
+00000ae0: 4461 7461 4e29 0672 3000 0000 7231 0000  DataN).r0...r1..
+00000af0: 0072 3200 0000 723a 0000 0072 3400 0000  .r2...r:...r4...
+00000b00: 721b 0000 0072 3800 0000 7238 0000 0072  r....r8...r8...r
+00000b10: 3800 0000 7239 0000 0072 5b00 0000 5b00  8...r9...r[...[.
+00000b20: 0000 7304 0000 000a 0108 0172 5b00 0000  ..s........r[...
 00000b30: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000b40: 0003 0000 0040 0000 0073 1a00 0000 6500  .....@...s....e.
 00000b50: 5a01 6400 5a02 5500 6503 6504 1900 6505  Z.d.Z.U.e.e...e.
 00000b60: 6401 3c00 6402 5300 2903 da0d 576f 726b  d.<.d.S.)...Work
 00000b70: 696e 674f 7264 6572 73da 0d77 6f72 6b69  ingOrders..worki
-00000b80: 6e67 4f72 6465 7273 4e29 0672 2a00 0000  ngOrdersN).r*...
-00000b90: 722b 0000 0072 2c00 0000 7205 0000 0072  r+...r,...r....r
-00000ba0: 5500 0000 722e 0000 0072 3200 0000 7232  U...r....r2...r2
-00000bb0: 0000 0072 3200 0000 7233 0000 0072 5800  ...r2...r3...rX.
-00000bc0: 0000 6000 0000 7302 0000 000a 0172 5800  ..`...s......rX.
+00000b80: 6e67 4f72 6465 7273 4e29 0672 3000 0000  ngOrdersN).r0...
+00000b90: 7231 0000 0072 3200 0000 7205 0000 0072  r1...r2...r....r
+00000ba0: 5b00 0000 7234 0000 0072 3800 0000 7238  [...r4...r8...r8
+00000bb0: 0000 0072 3800 0000 7239 0000 0072 5e00  ...r8...r9...r^.
+00000bc0: 0000 6000 0000 7302 0000 000a 0172 5e00  ..`...s......r^.
 00000bd0: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
 00000be0: 0000 0009 0000 0040 0000 0073 7601 0000  .......@...sv...
 00000bf0: 6500 5a01 6400 5a02 5500 6503 6401 6402  e.Z.d.Z.U.e.d.d.
 00000c00: 8d01 6504 6403 3c00 6505 6504 6404 3c00  ..e.d.<.e.e.d.<.
 00000c10: 6506 6504 6405 3c00 6503 6406 6402 8d01  e.e.d.<.e.d.d...
 00000c20: 6504 6407 3c00 6408 5a07 6508 6504 6409  e.d.<.d.Z.e.e.d.
 00000c30: 3c00 6503 640a 6402 8d01 6504 640b 3c00  <.e.d.d...e.d.<.
@@ -211,129 +211,129 @@
 00000d20: 6423 8404 8301 8301 5a1b 6518 6420 641c  d#......Z.e.d d.
 00000d30: 8d01 6519 651a 6421 9c01 6424 6425 8404  ..e.e.d!..d$d%..
 00000d40: 8301 8301 5a1c 6518 6420 641c 8d01 6519  ....Z.e.d d...e.
 00000d50: 651a 6421 9c01 6426 6427 8404 8301 8301  e.d!..d&d'......
 00000d60: 5a1d 6415 5300 2928 da12 4372 6561 7465  Z.d.S.)(..Create
 00000d70: 576f 726b 696e 674f 7264 6572 7a08 5b41  WorkingOrderz.[A
 00000d80: 2d5a 5d7b 337d 2901 da07 7061 7474 6572  -Z]{3})...patter
-00000d90: 6e72 4200 0000 7236 0000 0072 1a00 0000  nrB...r6...r....
+00000d90: 6e72 4800 0000 723c 0000 0072 2000 0000  nrH...r<...r ...
 00000da0: 7a1d 285c 647b 327d 2d29 3f5b 412d 5a5d  z.(\d{2}-)?[A-Z]
 00000db0: 7b33 7d2d 5c64 7b32 7d7c 2d7c 4446 4272  {3}-\d{2}|-|DFBr
-00000dc0: 1800 0000 46da 0966 6f72 6365 4f70 656e  ....F..forceOpen
+00000dc0: 1e00 0000 46da 0966 6f72 6365 4f70 656e  ....F..forceOpen
 00000dd0: 7a29 285c 647b 347d 2f5c 647b 327d 2f5c  z)(\d{4}/\d{2}/\
 00000de0: 647b 327d 205c 647b 327d 3a5c 647b 327d  d{2} \d{2}:\d{2}
-00000df0: 3a5c 647b 327d 7c5c 642a 2972 3a00 0000  :\d{2}|\d*)r:...
-00000e00: 720e 0000 0072 1c00 0000 da05 6c65 7665  r....r......leve
+00000df0: 3a5c 647b 327d 7c5c 642a 2972 4000 0000  :\d{2}|\d*)r@...
+00000e00: 720e 0000 0072 2200 0000 da05 6c65 7665  r....r".....leve
 00000e10: 6ce9 0c00 0000 da04 7369 7a65 da04 7479  l.......size..ty
-00000e20: 7065 723e 0000 0072 1200 0000 7239 0000  per>...r....r9..
+00000e20: 7065 7244 0000 0072 1200 0000 723f 0000  perD...r....r?..
 00000e30: 004e da0d 6465 616c 5265 6665 7265 6e63  .N..dealReferenc
-00000e40: 6572 4100 0000 da0a 6c69 6d69 744c 6576  erA.....limitLev
-00000e50: 656c 7240 0000 00da 0973 746f 704c 6576  elr@.....stopLev
-00000e60: 656c da05 706c 6169 6e72 4600 0000 7248  el..plainrF...rH
+00000e40: 6572 4700 0000 da0a 6c69 6d69 744c 6576  erG.....limitLev
+00000e50: 656c 7246 0000 00da 0973 746f 704c 6576  elrF.....stopLev
+00000e60: 656c da05 706c 6169 6e72 4c00 0000 724e  el..plainrL...rN
 00000e70: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
 00000e80: 0300 0000 0200 0000 4300 0000 7314 0000  ........C...s...
 00000e90: 007c 0164 0075 0172 1074 007c 0183 0153  .|.d.u.r.t.|...S
 00000ea0: 0064 0053 0029 014e 2901 da05 666c 6f61  .d.S.).N)...floa
-00000eb0: 7429 03da 0473 656c 6672 4900 0000 da05  t)...selfrI.....
-00000ec0: 5f69 6e66 6f72 3200 0000 7232 0000 0072  _infor2...r2...r
-00000ed0: 3300 0000 da11 7365 7269 616c 697a 655f  3.....serialize_
+00000eb0: 7429 03da 0473 656c 6672 4f00 0000 da05  t)...selfrO.....
+00000ec0: 5f69 6e66 6f72 3800 0000 7238 0000 0072  _infor8...r8...r
+00000ed0: 3900 0000 da11 7365 7269 616c 697a 655f  9.....serialize_
 00000ee0: 6465 6369 6d61 6c76 0000 0073 0400 0000  decimalv...s....
 00000ef0: 000a 0801 7a24 4372 6561 7465 576f 726b  ....z$CreateWork
 00000f00: 696e 674f 7264 6572 2e73 6572 6961 6c69  ingOrder.seriali
-00000f10: 7a65 5f64 6563 696d 616c 7245 0000 0029  ze_decimalrE...)
+00000f10: 7a65 5f64 6563 696d 616c 724b 0000 0029  ze_decimalrK...)
 00000f20: 01da 0464 6174 6163 0200 0000 0000 0000  ...datac........
 00000f30: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
 00000f40: 734c 0000 007c 01a0 0064 01a1 0164 0275  sL...|...d...d.u
 00000f50: 0172 247c 01a0 0064 03a1 0164 0275 0172  .r$|...d...d.u.r
 00000f60: 2474 0164 0483 0182 017c 01a0 0064 05a1  $t.d.....|...d..
 00000f70: 0164 0275 0172 487c 01a0 0064 06a1 0164  .d.u.rH|...d...d
 00000f80: 0275 0172 4874 0164 0783 0182 017c 0153  .u.rHt.d.....|.S
 00000f90: 0029 087a 775b 436f 6e73 7472 6169 6e74  .).zw[Constraint
 00000fa0: 3a20 5365 7420 6f6e 6c79 206f 6e65 206f  : Set only one o
 00000fb0: 6620 7b6c 696d 6974 4c65 7665 6c2c 6c69  f {limitLevel,li
 00000fc0: 6d69 7444 6973 7461 6e63 657d 5d0a 2020  mitDistance}].  
 00000fd0: 2020 2020 2020 5b43 6f6e 7374 7261 696e        [Constrain
 00000fe0: 743a 2053 6574 206f 6e6c 7920 6f6e 6520  t: Set only one 
 00000ff0: 6f66 207b 7374 6f70 4c65 7665 6c2c 7374  of {stopLevel,st
-00001000: 6f70 4469 7374 616e 6365 7d5d 7262 0000  opDistance}]rb..
-00001010: 004e 7241 0000 007a 2c53 6574 206f 6e6c  .NrA...z,Set onl
+00001000: 6f70 4469 7374 616e 6365 7d5d 7268 0000  opDistance}]rh..
+00001010: 004e 7247 0000 007a 2c53 6574 206f 6e6c  .NrG...z,Set onl
 00001020: 7920 6f6e 6520 6f66 206c 696d 6974 4c65  y one of limitLe
 00001030: 7665 6c20 6f72 206c 696d 6974 4469 7374  vel or limitDist
-00001040: 616e 6365 2e72 6300 0000 7240 0000 007a  ance.rc...r@...z
+00001040: 616e 6365 2e72 6900 0000 7246 0000 007a  ance.ri...rF...z
 00001050: 2a53 6574 206f 6e6c 7920 6f6e 6520 6f66  *Set only one of
 00001060: 2073 746f 704c 6576 656c 206f 7220 7374   stopLevel or st
 00001070: 6f70 4469 7374 616e 6365 2ea9 02da 0367  opDistance.....g
-00001080: 6574 724d 0000 00a9 0272 4f00 0000 7269  etrM.....rO...ri
-00001090: 0000 0072 3200 0000 7232 0000 0072 3300  ...r2...r2...r3.
+00001080: 6574 7253 0000 00a9 0272 5500 0000 726f  etrS.....rU...ro
+00001090: 0000 0072 3800 0000 7238 0000 0072 3900  ...r8...r8...r9.
 000010a0: 0000 da18 6368 6563 6b5f 756e 6971 7565  ....check_unique
 000010b0: 5f63 6f6e 7374 7261 696e 7473 8300 0000  _constraints....
 000010c0: 730a 0000 0000 051c 0108 011c 0108 017a  s..............z
 000010d0: 2b43 7265 6174 6557 6f72 6b69 6e67 4f72  +CreateWorkingOr
 000010e0: 6465 722e 6368 6563 6b5f 756e 6971 7565  der.check_unique
 000010f0: 5f63 6f6e 7374 7261 696e 7473 6302 0000  _constraintsc...
 00001100: 0000 0000 0000 0000 0002 0000 0003 0000  ................
 00001110: 0043 0000 0073 2800 0000 7c01 a000 6401  .C...s(...|...d.
 00001120: a101 6402 6b02 7224 7c01 a000 6403 a101  ..d.k.r$|...d...
 00001130: 6400 7500 7224 7401 6404 8301 8201 7c01  d.u.r$t.d.....|.
-00001140: 5300 2905 4e72 3900 0000 7213 0000 0072  S.).Nr9...r....r
-00001150: 3a00 0000 7a39 7469 6d65 496e 466f 7263  :...z9timeInForc
+00001140: 5300 2905 4e72 3f00 0000 7213 0000 0072  S.).Nr?...r....r
+00001150: 4000 0000 7a39 7469 6d65 496e 466f 7263  @...z9timeInForc
 00001160: 6520 474f 4f44 5f54 494c 4c5f 4441 5445  e GOOD_TILL_DATE
 00001170: 2072 6571 7569 7265 7320 6120 676f 6f64   requires a good
 00001180: 5469 6c6c 4461 7465 2076 616c 7565 2e72  TillDate value.r
-00001190: 6a00 0000 2902 7266 0000 0072 6900 0000  j...).rf...ri...
-000011a0: 7232 0000 0072 3200 0000 7233 0000 00da  r2...r2...r3....
+00001190: 7000 0000 2902 726c 0000 0072 6f00 0000  p...).rl...ro...
+000011a0: 7238 0000 0072 3800 0000 7239 0000 00da  r8...r8...r9....
 000011b0: 1776 616c 6964 6174 655f 676f 6f64 5f74  .validate_good_t
 000011c0: 696c 6c5f 6461 7465 8e00 0000 7310 0000  ill_date....s...
 000011d0: 0000 040c ff02 020c fe02 0402 0102 ff04  ................
 000011e0: 037a 2a43 7265 6174 6557 6f72 6b69 6e67  .z*CreateWorking
 000011f0: 4f72 6465 722e 7661 6c69 6461 7465 5f67  Order.validate_g
 00001200: 6f6f 645f 7469 6c6c 5f64 6174 6563 0200  ood_till_datec..
 00001210: 0000 0000 0000 0000 0000 0200 0000 0500  ................
 00001220: 0000 4300 0000 7332 0000 007c 01a0 0064  ..C...s2...|...d
 00001230: 01a1 0172 2e74 017c 01a0 0064 02a1 0183  ...r.t.|...d....
 00001240: 0174 017c 01a0 0064 03a1 0183 0141 0073  .t.|...d.....A.s
 00001250: 2e74 0264 0483 0182 017c 0153 0029 054e  .t.d.....|.S.).N
-00001260: 723e 0000 0072 6300 0000 7240 0000 007a  r>...rc...r@...z
+00001260: 7244 0000 0072 6900 0000 7246 0000 007a  rD...ri...rF...z
 00001270: 4e57 6865 6e20 6775 6172 616e 7465 6564  NWhen guaranteed
 00001280: 5374 6f70 2069 7320 7472 7565 2c20 7370  Stop is true, sp
 00001290: 6563 6966 7920 6578 6163 746c 7920 6f6e  ecify exactly on
 000012a0: 6520 6f66 2073 746f 704c 6576 656c 206f  e of stopLevel o
 000012b0: 7220 7374 6f70 4469 7374 616e 6365 2e29  r stopDistance.)
-000012c0: 0372 6b00 0000 7231 0000 0072 4d00 0000  .rk...r1...rM...
-000012d0: 726c 0000 0072 3200 0000 7232 0000 0072  rl...r2...r2...r
-000012e0: 3300 0000 da21 6368 6563 6b5f 6775 6172  3....!check_guar
+000012c0: 0372 7100 0000 7237 0000 0072 5300 0000  .rq...r7...rS...
+000012d0: 7272 0000 0072 3800 0000 7238 0000 0072  rr...r8...r8...r
+000012e0: 3900 0000 da21 6368 6563 6b5f 6775 6172  9....!check_guar
 000012f0: 616e 7465 6564 5f73 746f 705f 636f 6e73  anteed_stop_cons
 00001300: 7472 6169 6e74 739a 0000 0073 0e00 0000  traints....s....
 00001310: 0003 0a01 1aff 0203 0201 02ff 0403 7a34  ..............z4
 00001320: 4372 6561 7465 576f 726b 696e 674f 7264  CreateWorkingOrd
 00001330: 6572 2e63 6865 636b 5f67 7561 7261 6e74  er.check_guarant
 00001340: 6565 645f 7374 6f70 5f63 6f6e 7374 7261  eed_stop_constra
-00001350: 696e 7473 291e 722a 0000 0072 2b00 0000  ints).r*...r+...
-00001360: 722c 0000 0072 0b00 0000 722e 0000 0072  r,...r....r....r
-00001370: 1000 0000 722d 0000 0072 5c00 0000 7231  ....r-...r\...r1
-00001380: 0000 0072 0900 0000 7253 0000 0072 3e00  ...r....rS...r>.
-00001390: 0000 7239 0000 0072 5200 0000 7261 0000  ..r9...rR...ra..
-000013a0: 0072 0400 0000 7241 0000 0072 6200 0000  .r....rA...rb...
-000013b0: 7240 0000 0072 6300 0000 720d 0000 0072  r@...rc...r....r
-000013c0: 0300 0000 7265 0000 0072 6800 0000 720c  ....re...rh...r.
-000013d0: 0000 0072 5400 0000 7207 0000 0072 6d00  ...rT...r....rm.
-000013e0: 0000 726e 0000 0072 6f00 0000 7232 0000  ..rn...ro...r2..
-000013f0: 0072 3200 0000 7232 0000 0072 3300 0000  .r2...r2...r3...
-00001400: 725a 0000 0064 0000 0073 4600 0000 0a01  rZ...d...sF.....
+00001350: 696e 7473 291e 7230 0000 0072 3100 0000  ints).r0...r1...
+00001360: 7232 0000 0072 0b00 0000 7234 0000 0072  r2...r....r4...r
+00001370: 1000 0000 7233 0000 0072 6200 0000 7237  ....r3...rb...r7
+00001380: 0000 0072 0900 0000 7259 0000 0072 4400  ...r....rY...rD.
+00001390: 0000 723f 0000 0072 5800 0000 7267 0000  ..r?...rX...rg..
+000013a0: 0072 0400 0000 7247 0000 0072 6800 0000  .r....rG...rh...
+000013b0: 7246 0000 0072 6900 0000 720d 0000 0072  rF...ri...r....r
+000013c0: 0300 0000 726b 0000 0072 6e00 0000 720c  ....rk...rn...r.
+000013d0: 0000 0072 5a00 0000 7207 0000 0072 7300  ...rZ...r....rs.
+000013e0: 0000 7274 0000 0072 7500 0000 7238 0000  ..rt...ru...r8..
+000013f0: 0072 3800 0000 7238 0000 0072 3900 0000  .r8...r8...r9...
+00001400: 7260 0000 0064 0000 0073 4600 0000 0a01  r`...d...sF.....
 00001410: 0e01 0801 0801 0e01 0c01 0e01 0e01 0e01  ................
 00001420: 0801 0c01 0c01 1001 1601 1601 1601 1602  ................
 00001430: 0201 0201 0201 0201 0201 0201 0201 02f9  ................
 00001440: 0409 1604 0801 0201 1209 0801 0201 120a  ................
-00001450: 0801 0201 725a 0000 004e 291a 7202 0000  ....rZ...N).r...
+00001450: 0801 0201 7260 0000 004e 291a 7202 0000  ....r`...N).r...
 00001460: 00da 0764 6563 696d 616c 7203 0000 00da  ...decimalr.....
 00001470: 0674 7970 696e 6772 0400 0000 7205 0000  .typingr....r...
 00001480: 0072 0600 0000 7207 0000 00da 0870 7964  .r....r......pyd
 00001490: 616e 7469 6372 0800 0000 7209 0000 0072  anticr....r....r
 000014a0: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
 000014b0: 0000 00da 066d 6f64 656c 7372 0f00 0000  .....modelsr....
-000014c0: 7210 0000 0072 5300 0000 7252 0000 0072  r....rS...rR...r
-000014d0: 2f00 0000 7215 0000 0072 3400 0000 7255  /...r....r4...rU
-000014e0: 0000 0072 5800 0000 725a 0000 0072 3200  ...rX...rZ...r2.
-000014f0: 0000 7232 0000 0072 3200 0000 7233 0000  ..r2...r2...r3..
+000014c0: 7210 0000 0072 5900 0000 7258 0000 0072  r....rY...rX...r
+000014d0: 3500 0000 721b 0000 0072 3a00 0000 725b  5...r....r:...r[
+000014e0: 0000 0072 5e00 0000 7260 0000 0072 3800  ...r^...r`...r8.
+000014f0: 0000 7238 0000 0072 3800 0000 7239 0000  ..r8...r8...r9..
 00001500: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
 00001510: 1c00 0000 0c01 0c01 1802 2008 1003 0803  .......... .....
 00001520: 0803 0201 02ff 040b 1015 1025 1005 1004  ...........%....
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/service.cpython-39.pyc` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/__pycache__/service.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  7 21:42:19 2024 UTC, .py size: 2531 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3b13 1366 e309 0000  a.......;..f....
+00000000: 610d 0d0a 0000 0000 9b30 3d66 d30d 0000  a........0=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6406 6407 6c06 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6500 a00a 650b a101 5a0c 4700 6408  ..e...e...Z.G.d.
@@ -22,150 +22,203 @@
 00000150: 6169 7365 6420 666f 7220 6572 726f 7273  aised for errors
 00000160: 2069 6e20 7468 6520 6f72 6465 7220 7072   in the order pr
 00000170: 6f63 6573 732e 4e29 04da 085f 5f6e 616d  ocess.N)...__nam
 00000180: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
 00000190: 0c5f 5f71 7561 6c6e 616d 655f 5fda 075f  .__qualname__.._
 000001a0: 5f64 6f63 5f5f a900 720e 0000 0072 0e00  _doc__..r....r..
 000001b0: 0000 fa58 2f68 6f6d 652f 7275 6e6e 6572  ...X/home/runner
-000001c0: 2f77 6f72 6b2f 6967 5f74 7261 6469 6e67  /work/ig_trading
-000001d0: 5f6c 6962 2f69 675f 7472 6164 696e 675f  _lib/ig_trading_
+000001c0: 2f77 6f72 6b2f 6967 2d74 7261 6469 6e67  /work/ig-trading
+000001d0: 2d6c 6962 2f69 672d 7472 6164 696e 672d  -lib/ig-trading-
 000001e0: 6c69 622f 6967 5f74 7261 6469 6e67 5f6c  lib/ig_trading_l
 000001f0: 6962 2f74 7261 6469 6e67 2f6f 7264 6572  ib/trading/order
 00000200: 732f 7365 7276 6963 652e 7079 7209 0000  s/service.pyr...
 00000210: 000e 0000 0073 0400 0000 0801 0401 7209  .....s........r.
 00000220: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000230: 0000 0000 0400 0000 4000 0000 734e 0000  ........@...sN..
+00000230: 0000 0000 0400 0000 4000 0000 735e 0000  ........@...s^..
 00000240: 0065 005a 0164 005a 0265 0365 0465 0364  .e.Z.d.Z.e.e.e.d
 00000250: 019c 0364 0264 0384 045a 0565 0665 0764  ...d.d...Z.e.e.d
 00000260: 049c 0164 0564 0684 0483 015a 0865 0964  ...d.d.....Z.e.d
 00000270: 049c 0164 0764 0884 045a 0a65 0b65 0c64  ...d.d...Z.e.e.d
-00000280: 099c 0264 0a64 0b84 045a 0d64 0c53 0029  ...d.d...Z.d.S.)
-00000290: 0dda 0c4f 7264 6572 5365 7276 6963 65a9  ...OrderService.
-000002a0: 03da 0761 7069 5f6b 6579 da06 746f 6b65  ...api_key..toke
-000002b0: 6e73 da08 6261 7365 5f75 726c 6304 0000  ns..base_urlc...
-000002c0: 0000 0000 0000 0000 0004 0000 0002 0000  ................
-000002d0: 0043 0000 0073 1600 0000 7c01 7c00 5f00  .C...s....|.|._.
-000002e0: 7c02 7c00 5f01 7c03 7c00 5f02 6400 5300  |.|._.|.|._.d.S.
-000002f0: 2901 4e72 1100 0000 2904 da04 7365 6c66  ).Nr....)...self
-00000300: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000310: 0e00 0000 720e 0000 0072 0f00 0000 da08  ....r....r......
-00000320: 5f5f 696e 6974 5f5f 1400 0000 7306 0000  __init__....s...
-00000330: 0000 0106 0106 017a 154f 7264 6572 5365  .......z.OrderSe
-00000340: 7276 6963 652e 5f5f 696e 6974 5f5f 2901  rvice.__init__).
-00000350: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-00000360: 0000 0000 0001 0000 0007 0000 0043 0000  .............C..
-00000370: 0073 1c00 0000 6401 6401 6402 7c00 6a00  .s....d.d.d.|.j.
-00000380: 7c00 6a01 6a02 7c00 6a01 6a03 6403 9c06  |.j.j.|.j.j.d...
-00000390: 5300 2904 4e7a 1f61 7070 6c69 6361 7469  S.).Nz.applicati
-000003a0: 6f6e 2f6a 736f 6e3b 2063 6861 7273 6574  on/json; charset
-000003b0: 3d75 7466 2d38 da01 3229 067a 0c43 6f6e  =utf-8..2).z.Con
-000003c0: 7465 6e74 2d54 7970 65da 0641 6363 6570  tent-Type..Accep
-000003d0: 74da 0756 6572 7369 6f6e 7a0c 582d 4947  t..Versionz.X-IG
-000003e0: 2d41 5049 2d4b 4559 7a10 582d 5345 4355  -API-KEYz.X-SECU
-000003f0: 5249 5459 2d54 4f4b 454e da03 4353 5429  RITY-TOKEN..CST)
-00000400: 0472 1200 0000 7213 0000 00da 1078 5f73  .r....r......x_s
-00000410: 6563 7572 6974 795f 746f 6b65 6eda 0963  ecurity_token..c
-00000420: 7374 5f74 6f6b 656e 2901 7215 0000 0072  st_token).r....r
-00000430: 0e00 0000 720e 0000 0072 0f00 0000 da07  ....r....r......
-00000440: 6865 6164 6572 7319 0000 0073 0e00 0000  headers....s....
-00000450: 0003 0201 0201 0201 0401 0601 06fa 7a14  ..............z.
-00000460: 4f72 6465 7253 6572 7669 6365 2e68 6561  OrderService.hea
-00000470: 6465 7273 6301 0000 0000 0000 0000 0000  dersc...........
-00000480: 0004 0000 000a 0000 0043 0000 0073 b400  .........C...s..
-00000490: 0000 7c00 6a00 9b00 6401 9d02 7d01 7a42  ..|.j...d...}.zB
-000004a0: 7401 6a02 7c01 7c00 6a03 6402 8d02 7d02  t.j.|.|.j.d...}.
-000004b0: 7c02 6a04 6403 6b02 7238 7405 a006 7c02  |.j.d.k.r8t...|.
-000004c0: a007 a100 a101 5700 5300 7408 6404 7c02  ......W.S.t.d.|.
-000004d0: 6a04 7c02 6a09 6602 1600 8301 8201 5700  j.|.j.f.......W.
-000004e0: 6e60 0400 740a 797e 0100 7d03 0100 7a18  n`..t.y~..}...z.
-000004f0: 7408 6405 7c03 1600 8301 8201 5700 5900  t.d.|.......W.Y.
-00000500: 6406 7d03 7e03 6e3a 6406 7d03 7e03 3000  d.}.~.n:d.}.~.0.
-00000510: 0400 7401 6a0b 79ae 0100 7d03 0100 7a18  ..t.j.y...}...z.
-00000520: 7408 6407 7c03 1600 8301 8201 5700 5900  t.d.|.......W.Y.
-00000530: 6406 7d03 7e03 6e0a 6406 7d03 7e03 3000  d.}.~.n.d.}.~.0.
-00000540: 3000 6406 5300 2908 7a17 4765 7420 776f  0.d.S.).z.Get wo
-00000550: 726b 696e 6720 6f72 6465 7273 206c 6973  rking orders lis
-00000560: 747a 1b2f 6761 7465 7761 792f 6465 616c  tz./gateway/deal
-00000570: 2f77 6f72 6b69 6e67 6f72 6465 7273 2901  /workingorders).
-00000580: 721e 0000 00e9 c800 0000 7a2d 576f 726b  r.........z-Work
-00000590: 696e 6720 6f72 6465 7273 2066 6169 6c65  ing orders faile
-000005a0: 6420 7769 7468 2073 7461 7475 7320 636f  d with status co
-000005b0: 6465 2025 733a 2025 737a 2349 6e76 616c  de %s: %sz#Inval
-000005c0: 6964 2077 6f72 6b69 6e67 206f 7264 6572  id working order
-000005d0: 7320 7265 7370 6f6e 7365 3a20 2573 4e7a  s response: %sNz
-000005e0: 2157 6f72 6b69 6e67 206f 7264 6572 7320  !Working orders 
-000005f0: 7265 7175 6573 7420 6661 696c 6564 3a20  request failed: 
-00000600: 2573 290c 7214 0000 00da 0872 6571 7565  %s).r......reque
-00000610: 7374 73da 0367 6574 721e 0000 00da 0b73  sts..getr......s
-00000620: 7461 7475 735f 636f 6465 7205 0000 00da  tatus_coder.....
-00000630: 0e6d 6f64 656c 5f76 616c 6964 6174 65da  .model_validate.
-00000640: 046a 736f 6e72 0900 0000 da04 7465 7874  .jsonr......text
-00000650: 7202 0000 00da 1052 6571 7565 7374 4578  r......RequestEx
-00000660: 6365 7074 696f 6e29 0472 1500 0000 da03  ception).r......
-00000670: 7572 6cda 0872 6573 706f 6e73 65da 0165  url..response..e
-00000680: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
-00000690: 1267 6574 5f77 6f72 6b69 6e67 5f6f 7264  .get_working_ord
-000006a0: 6572 7325 0000 0073 1c00 0000 0002 0c01  ers%...s........
-000006b0: 0201 1001 0a01 1002 0201 0201 0aff 02ff  ................
-000006c0: 0804 0e01 2001 1001 7a1f 4f72 6465 7253  .... ...z.OrderS
-000006d0: 6572 7669 6365 2e67 6574 5f77 6f72 6b69  ervice.get_worki
-000006e0: 6e67 5f6f 7264 6572 7329 02da 0d77 6f72  ng_orders)...wor
-000006f0: 6b69 6e67 5f6f 7264 6572 7217 0000 0063  king_orderr....c
-00000700: 0200 0000 0000 0000 0000 0000 0500 0000  ................
-00000710: 0a00 0000 4300 0000 73ba 0000 007c 006a  ....C...s....|.j
-00000720: 009b 0064 019d 027d 027a 4874 016a 027c  ...d...}.zHt.j.|
-00000730: 027c 006a 037c 01a0 04a1 0064 028d 037d  .|.j.|.....d...}
-00000740: 037c 036a 0564 036b 0272 3e74 06a0 077c  .|.j.d.k.r>t...|
-00000750: 03a0 08a1 00a1 0157 0053 0074 0964 047c  .......W.S.t.d.|
-00000760: 036a 057c 036a 0a66 0216 0083 0182 0157  .j.|.j.f.......W
-00000770: 006e 6004 0074 0b79 8401 007d 0401 007a  .n`..t.y...}...z
-00000780: 1874 0964 057c 0416 0083 0182 0157 0059  .t.d.|.......W.Y
-00000790: 0064 067d 047e 046e 3a64 067d 047e 0430  .d.}.~.n:d.}.~.0
-000007a0: 0004 0074 016a 0c79 b401 007d 0401 007a  ...t.j.y...}...z
-000007b0: 1874 0964 077c 0416 0083 0182 0157 0059  .t.d.|.......W.Y
-000007c0: 0064 067d 047e 046e 0a64 067d 047e 0430  .d.}.~.n.d.}.~.0
-000007d0: 0030 0064 0653 0029 087a 1a43 7265 6174  .0.d.S.).z.Creat
-000007e0: 6520 6120 6e65 7720 776f 726b 696e 6720  e a new working 
-000007f0: 6f72 6465 727a 1f2f 6761 7465 7761 792f  orderz./gateway/
-00000800: 6465 616c 2f77 6f72 6b69 6e67 6f72 6465  deal/workingorde
-00000810: 7273 2f6f 7463 2902 721e 0000 0072 2400  rs/otc).r....r$.
-00000820: 0000 721f 0000 007a 3343 7265 6174 6520  ..r....z3Create 
-00000830: 776f 726b 696e 6720 6f72 6465 7220 6661  working order fa
-00000840: 696c 6564 2077 6974 6820 7374 6174 7573  iled with status
-00000850: 2063 6f64 6520 2573 3a20 2573 7a29 496e   code %s: %sz)In
-00000860: 7661 6c69 6420 6372 6561 7465 2077 6f72  valid create wor
-00000870: 6b69 6e67 206f 7264 6572 2072 6573 706f  king order respo
-00000880: 6e73 653a 2025 734e 7a27 4372 6561 7465  nse: %sNz'Create
-00000890: 2077 6f72 6b69 6e67 206f 7264 6572 2072   working order r
-000008a0: 6571 7565 7374 2066 6169 6c65 643a 2025  equest failed: %
-000008b0: 7329 0d72 1400 0000 7220 0000 00da 0470  s).r....r .....p
-000008c0: 6f73 7472 1e00 0000 da04 6469 6374 7222  ostr......dictr"
-000008d0: 0000 0072 0800 0000 7223 0000 0072 2400  ...r....r#...r$.
-000008e0: 0000 7209 0000 0072 2500 0000 7202 0000  ..r....r%...r...
-000008f0: 0072 2600 0000 2905 7215 0000 0072 2b00  .r&...).r....r+.
-00000900: 0000 7227 0000 0072 2800 0000 7229 0000  ..r'...r(...r)..
-00000910: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-00000920: da14 6372 6561 7465 5f77 6f72 6b69 6e67  ..create_working
-00000930: 5f6f 7264 6572 3700 0000 731c 0000 0000  _order7...s.....
-00000940: 020c 0102 0116 010a 0110 0202 0102 010a  ................
-00000950: ff02 ff08 040e 0120 0110 017a 214f 7264  ....... ...z!Ord
-00000960: 6572 5365 7276 6963 652e 6372 6561 7465  erService.create
-00000970: 5f77 6f72 6b69 6e67 5f6f 7264 6572 4e29  _working_orderN)
-00000980: 0e72 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000990: da03 7374 7272 0300 0000 7216 0000 00da  ..strr....r.....
-000009a0: 0870 726f 7065 7274 7972 2d00 0000 721e  .propertyr-...r.
-000009b0: 0000 0072 0500 0000 722a 0000 0072 0600  ...r....r*...r..
-000009c0: 0000 7208 0000 0072 2e00 0000 720e 0000  ..r....r....r...
-000009d0: 0072 0e00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-000009e0: 7210 0000 0013 0000 0073 0a00 0000 0801  r........s......
-000009f0: 1205 0201 100b 0e12 7210 0000 0029 10da  ........r....)..
-00000a00: 076c 6f67 6769 6e67 7220 0000 00da 0870  .loggingr .....p
-00000a10: 7964 616e 7469 6372 0200 0000 da0e 6967  ydanticr......ig
-00000a20: 5f74 7261 6469 6e67 5f6c 6962 7203 0000  _trading_libr...
-00000a30: 00da 066d 6f64 656c 7372 0500 0000 7206  ...modelsr....r.
-00000a40: 0000 0072 0800 0000 da09 6765 744c 6f67  ...r......getLog
-00000a50: 6765 7272 0a00 0000 da06 6c6f 6767 6572  gerr......logger
-00000a60: da09 4578 6365 7074 696f 6e72 0900 0000  ..Exceptionr....
-00000a70: 7210 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00000a80: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
-00000a90: 6c65 3e01 0000 0073 1000 0000 0802 0801  le>....s........
-00000aa0: 0c02 0c01 1001 0c03 0a03 1005            ............
+00000280: 099c 0264 0a64 0b84 045a 0d65 0365 0c64  ...d.d...Z.e.e.d
+00000290: 0c9c 0264 0d64 0e84 045a 0e64 0f53 0029  ...d.d...Z.d.S.)
+000002a0: 10da 0c4f 7264 6572 5365 7276 6963 65a9  ...OrderService.
+000002b0: 03da 0761 7069 5f6b 6579 da06 746f 6b65  ...api_key..toke
+000002c0: 6e73 da08 6261 7365 5f75 726c 6304 0000  ns..base_urlc...
+000002d0: 0000 0000 0000 0000 0004 0000 0002 0000  ................
+000002e0: 0043 0000 0073 1600 0000 7c01 7c00 5f00  .C...s....|.|._.
+000002f0: 7c02 7c00 5f01 7c03 7c00 5f02 6400 5300  |.|._.|.|._.d.S.
+00000300: 2901 4e72 1100 0000 2904 da04 7365 6c66  ).Nr....)...self
+00000310: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+00000320: 0e00 0000 720e 0000 0072 0f00 0000 da08  ....r....r......
+00000330: 5f5f 696e 6974 5f5f 1400 0000 7306 0000  __init__....s...
+00000340: 0000 0106 0106 017a 154f 7264 6572 5365  .......z.OrderSe
+00000350: 7276 6963 652e 5f5f 696e 6974 5f5f 2901  rvice.__init__).
+00000360: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
+00000370: 0000 0000 0001 0000 0007 0000 0043 0000  .............C..
+00000380: 0073 1c00 0000 6401 6401 6402 7c00 6a00  .s....d.d.d.|.j.
+00000390: 7c00 6a01 6a02 7c00 6a01 6a03 6403 9c06  |.j.j.|.j.j.d...
+000003a0: 5300 2904 4e7a 1f61 7070 6c69 6361 7469  S.).Nz.applicati
+000003b0: 6f6e 2f6a 736f 6e3b 2063 6861 7273 6574  on/json; charset
+000003c0: 3d75 7466 2d38 da01 3229 067a 0c43 6f6e  =utf-8..2).z.Con
+000003d0: 7465 6e74 2d54 7970 65da 0641 6363 6570  tent-Type..Accep
+000003e0: 74da 0756 6572 7369 6f6e 7a0c 582d 4947  t..Versionz.X-IG
+000003f0: 2d41 5049 2d4b 4559 7a10 582d 5345 4355  -API-KEYz.X-SECU
+00000400: 5249 5459 2d54 4f4b 454e da03 4353 5429  RITY-TOKEN..CST)
+00000410: 0472 1200 0000 7213 0000 00da 1078 5f73  .r....r......x_s
+00000420: 6563 7572 6974 795f 746f 6b65 6eda 0963  ecurity_token..c
+00000430: 7374 5f74 6f6b 656e 2901 7215 0000 0072  st_token).r....r
+00000440: 0e00 0000 720e 0000 0072 0f00 0000 da07  ....r....r......
+00000450: 6865 6164 6572 7319 0000 0073 0e00 0000  headers....s....
+00000460: 0003 0201 0201 0201 0401 0601 06fa 7a14  ..............z.
+00000470: 4f72 6465 7253 6572 7669 6365 2e68 6561  OrderService.hea
+00000480: 6465 7273 6301 0000 0000 0000 0000 0000  dersc...........
+00000490: 0004 0000 000a 0000 0043 0000 0073 b400  .........C...s..
+000004a0: 0000 7c00 6a00 9b00 6401 9d02 7d01 7a42  ..|.j...d...}.zB
+000004b0: 7401 6a02 7c01 7c00 6a03 6402 8d02 7d02  t.j.|.|.j.d...}.
+000004c0: 7c02 6a04 6403 6b02 7238 7405 a006 7c02  |.j.d.k.r8t...|.
+000004d0: a007 a100 a101 5700 5300 7408 6404 7c02  ......W.S.t.d.|.
+000004e0: 6a04 7c02 6a09 6602 1600 8301 8201 5700  j.|.j.f.......W.
+000004f0: 6e60 0400 740a 797e 0100 7d03 0100 7a18  n`..t.y~..}...z.
+00000500: 7408 6405 7c03 1600 8301 8201 5700 5900  t.d.|.......W.Y.
+00000510: 6406 7d03 7e03 6e3a 6406 7d03 7e03 3000  d.}.~.n:d.}.~.0.
+00000520: 0400 7401 6a0b 79ae 0100 7d03 0100 7a18  ..t.j.y...}...z.
+00000530: 7408 6407 7c03 1600 8301 8201 5700 5900  t.d.|.......W.Y.
+00000540: 6406 7d03 7e03 6e0a 6406 7d03 7e03 3000  d.}.~.n.d.}.~.0.
+00000550: 3000 6406 5300 2908 7a17 4765 7420 776f  0.d.S.).z.Get wo
+00000560: 726b 696e 6720 6f72 6465 7273 206c 6973  rking orders lis
+00000570: 747a 1b2f 6761 7465 7761 792f 6465 616c  tz./gateway/deal
+00000580: 2f77 6f72 6b69 6e67 6f72 6465 7273 a901  /workingorders..
+00000590: 721e 0000 00e9 c800 0000 7a2d 576f 726b  r.........z-Work
+000005a0: 696e 6720 6f72 6465 7273 2066 6169 6c65  ing orders faile
+000005b0: 6420 7769 7468 2073 7461 7475 7320 636f  d with status co
+000005c0: 6465 2025 733a 2025 737a 2349 6e76 616c  de %s: %sz#Inval
+000005d0: 6964 2077 6f72 6b69 6e67 206f 7264 6572  id working order
+000005e0: 7320 7265 7370 6f6e 7365 3a20 2573 4e7a  s response: %sNz
+000005f0: 2157 6f72 6b69 6e67 206f 7264 6572 7320  !Working orders 
+00000600: 7265 7175 6573 7420 6661 696c 6564 3a20  request failed: 
+00000610: 2573 290c 7214 0000 00da 0872 6571 7565  %s).r......reque
+00000620: 7374 73da 0367 6574 721e 0000 00da 0b73  sts..getr......s
+00000630: 7461 7475 735f 636f 6465 7205 0000 00da  tatus_coder.....
+00000640: 0e6d 6f64 656c 5f76 616c 6964 6174 65da  .model_validate.
+00000650: 046a 736f 6e72 0900 0000 da04 7465 7874  .jsonr......text
+00000660: 7202 0000 00da 1052 6571 7565 7374 4578  r......RequestEx
+00000670: 6365 7074 696f 6e29 0472 1500 0000 da03  ception).r......
+00000680: 7572 6cda 0872 6573 706f 6e73 65da 0165  url..response..e
+00000690: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+000006a0: 1267 6574 5f77 6f72 6b69 6e67 5f6f 7264  .get_working_ord
+000006b0: 6572 7325 0000 0073 1c00 0000 0002 0c01  ers%...s........
+000006c0: 0201 1001 0a01 1002 0201 0201 0aff 02ff  ................
+000006d0: 0804 0e01 2001 1001 7a1f 4f72 6465 7253  .... ...z.OrderS
+000006e0: 6572 7669 6365 2e67 6574 5f77 6f72 6b69  ervice.get_worki
+000006f0: 6e67 5f6f 7264 6572 7329 02da 0d77 6f72  ng_orders)...wor
+00000700: 6b69 6e67 5f6f 7264 6572 7217 0000 0063  king_orderr....c
+00000710: 0200 0000 0000 0000 0000 0000 0500 0000  ................
+00000720: 0a00 0000 4300 0000 73ba 0000 007c 006a  ....C...s....|.j
+00000730: 009b 0064 019d 027d 027a 4874 016a 027c  ...d...}.zHt.j.|
+00000740: 027c 006a 037c 01a0 04a1 0064 028d 037d  .|.j.|.....d...}
+00000750: 037c 036a 0564 036b 0272 3e74 06a0 077c  .|.j.d.k.r>t...|
+00000760: 03a0 08a1 00a1 0157 0053 0074 0964 047c  .......W.S.t.d.|
+00000770: 036a 057c 036a 0a66 0216 0083 0182 0157  .j.|.j.f.......W
+00000780: 006e 6004 0074 0b79 8401 007d 0401 007a  .n`..t.y...}...z
+00000790: 1874 0964 057c 0416 0083 0182 0157 0059  .t.d.|.......W.Y
+000007a0: 0064 067d 047e 046e 3a64 067d 047e 0430  .d.}.~.n:d.}.~.0
+000007b0: 0004 0074 016a 0c79 b401 007d 0401 007a  ...t.j.y...}...z
+000007c0: 1874 0964 077c 0416 0083 0182 0157 0059  .t.d.|.......W.Y
+000007d0: 0064 067d 047e 046e 0a64 067d 047e 0430  .d.}.~.n.d.}.~.0
+000007e0: 0030 0064 0653 0029 087a 8543 7265 6174  .0.d.S.).z.Creat
+000007f0: 6520 6120 6e65 7720 776f 726b 696e 6720  e a new working 
+00000800: 6f72 6465 720a 2020 2020 2020 2020 3a70  order.        :p
+00000810: 6172 616d 2077 6f72 6b69 6e67 5f6f 7264  aram working_ord
+00000820: 6572 3a20 4372 6561 7465 576f 726b 696e  er: CreateWorkin
+00000830: 674f 7264 6572 2069 6e73 7461 6e63 650a  gOrder instance.
+00000840: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00000850: 2044 6561 6c52 6566 6572 656e 6365 2069   DealReference i
+00000860: 6e73 7461 6e63 650a 2020 2020 2020 2020  nstance.        
+00000870: 7a1f 2f67 6174 6577 6179 2f64 6561 6c2f  z./gateway/deal/
+00000880: 776f 726b 696e 676f 7264 6572 732f 6f74  workingorders/ot
+00000890: 6329 0272 1e00 0000 7225 0000 0072 2000  c).r....r%...r .
+000008a0: 0000 7a33 4372 6561 7465 2077 6f72 6b69  ..z3Create worki
+000008b0: 6e67 206f 7264 6572 2066 6169 6c65 6420  ng order failed 
+000008c0: 7769 7468 2073 7461 7475 7320 636f 6465  with status code
+000008d0: 2025 733a 2025 737a 2949 6e76 616c 6964   %s: %sz)Invalid
+000008e0: 2063 7265 6174 6520 776f 726b 696e 6720   create working 
+000008f0: 6f72 6465 7220 7265 7370 6f6e 7365 3a20  order response: 
+00000900: 2573 4e7a 2743 7265 6174 6520 776f 726b  %sNz'Create work
+00000910: 696e 6720 6f72 6465 7220 7265 7175 6573  ing order reques
+00000920: 7420 6661 696c 6564 3a20 2573 290d 7214  t failed: %s).r.
+00000930: 0000 0072 2100 0000 da04 706f 7374 721e  ...r!.....postr.
+00000940: 0000 00da 0464 6963 7472 2300 0000 7208  .....dictr#...r.
+00000950: 0000 0072 2400 0000 7225 0000 0072 0900  ...r$...r%...r..
+00000960: 0000 7226 0000 0072 0200 0000 7227 0000  ..r&...r....r'..
+00000970: 0029 0572 1500 0000 722c 0000 0072 2800  .).r....r,...r(.
+00000980: 0000 7229 0000 0072 2a00 0000 720e 0000  ..r)...r*...r...
+00000990: 0072 0e00 0000 720f 0000 00da 1463 7265  .r....r......cre
+000009a0: 6174 655f 776f 726b 696e 675f 6f72 6465  ate_working_orde
+000009b0: 7237 0000 0073 1c00 0000 0005 0c01 0201  r7...s..........
+000009c0: 1601 0a01 1002 0201 0201 0aff 02ff 0804  ................
+000009d0: 0e01 2001 1001 7a21 4f72 6465 7253 6572  .. ...z!OrderSer
+000009e0: 7669 6365 2e63 7265 6174 655f 776f 726b  vice.create_work
+000009f0: 696e 675f 6f72 6465 7229 02da 0764 6561  ing_order)...dea
+00000a00: 6c5f 6964 7217 0000 0063 0200 0000 0000  l_idr....c......
+00000a10: 0000 0000 0000 0500 0000 0a00 0000 4300  ..............C.
+00000a20: 0000 73b8 0000 007c 006a 009b 0064 017c  ..s....|.j...d.|
+00000a30: 019b 009d 037d 027a 4274 016a 027c 027c  .....}.zBt.j.|.|
+00000a40: 006a 0364 028d 027d 037c 036a 0464 036b  .j.d...}.|.j.d.k
+00000a50: 0272 3c74 05a0 067c 03a0 07a1 00a1 0157  .r<t...|.......W
+00000a60: 0053 0074 0864 047c 036a 047c 036a 0966  .S.t.d.|.j.|.j.f
+00000a70: 0216 0083 0182 0157 006e 6004 0074 0a79  .......W.n`..t.y
+00000a80: 8201 007d 0401 007a 1874 0864 057c 0416  ...}...z.t.d.|..
+00000a90: 0083 0182 0157 0059 0064 067d 047e 046e  .....W.Y.d.}.~.n
+00000aa0: 3a64 067d 047e 0430 0004 0074 016a 0b79  :d.}.~.0...t.j.y
+00000ab0: b201 007d 0401 007a 1874 0864 077c 0416  ...}...z.t.d.|..
+00000ac0: 0083 0182 0157 0059 0064 067d 047e 046e  .....W.Y.d.}.~.n
+00000ad0: 0a64 067d 047e 0430 0030 0064 0653 0029  .d.}.~.0.0.d.S.)
+00000ae0: 087a 6344 656c 6574 6520 6120 776f 726b  .zcDelete a work
+00000af0: 696e 6720 6f72 6465 720a 2020 2020 2020  ing order.      
+00000b00: 2020 3a70 6172 616d 2064 6561 6c5f 6964    :param deal_id
+00000b10: 3a20 7374 720a 2020 2020 2020 2020 3a72  : str.        :r
+00000b20: 6574 7572 6e3a 2044 6561 6c52 6566 6572  eturn: DealRefer
+00000b30: 656e 6365 2069 6e73 7461 6e63 650a 2020  ence instance.  
+00000b40: 2020 2020 2020 7a20 2f67 6174 6577 6179        z /gateway
+00000b50: 2f64 6561 6c2f 776f 726b 696e 676f 7264  /deal/workingord
+00000b60: 6572 732f 6f74 632f 721f 0000 0072 2000  ers/otc/r....r .
+00000b70: 0000 7a33 4465 6c65 7465 2077 6f72 6b69  ..z3Delete worki
+00000b80: 6e67 206f 7264 6572 2066 6169 6c65 6420  ng order failed 
+00000b90: 7769 7468 2073 7461 7475 7320 636f 6465  with status code
+00000ba0: 2025 733a 2025 737a 2949 6e76 616c 6964   %s: %sz)Invalid
+00000bb0: 2064 656c 6574 6520 776f 726b 696e 6720   delete working 
+00000bc0: 6f72 6465 7220 7265 7370 6f6e 7365 3a20  order response: 
+00000bd0: 2573 4e7a 2744 656c 6574 6520 776f 726b  %sNz'Delete work
+00000be0: 696e 6720 6f72 6465 7220 7265 7175 6573  ing order reques
+00000bf0: 7420 6661 696c 6564 3a20 2573 290c 7214  t failed: %s).r.
+00000c00: 0000 0072 2100 0000 da06 6465 6c65 7465  ...r!.....delete
+00000c10: 721e 0000 0072 2300 0000 7208 0000 0072  r....r#...r....r
+00000c20: 2400 0000 7225 0000 0072 0900 0000 7226  $...r%...r....r&
+00000c30: 0000 0072 0200 0000 7227 0000 0029 0572  ...r....r'...).r
+00000c40: 1500 0000 7230 0000 0072 2800 0000 7229  ....r0...r(...r)
+00000c50: 0000 0072 2a00 0000 720e 0000 0072 0e00  ...r*...r....r..
+00000c60: 0000 720f 0000 00da 1464 656c 6574 655f  ..r......delete_
+00000c70: 776f 726b 696e 675f 6f72 6465 724c 0000  working_orderL..
+00000c80: 0073 1c00 0000 0005 1001 0201 1001 0a01  .s..............
+00000c90: 1002 0201 0201 0aff 02ff 0804 0e01 2001  .............. .
+00000ca0: 1001 7a21 4f72 6465 7253 6572 7669 6365  ..z!OrderService
+00000cb0: 2e64 656c 6574 655f 776f 726b 696e 675f  .delete_working_
+00000cc0: 6f72 6465 724e 290f 720a 0000 0072 0b00  orderN).r....r..
+00000cd0: 0000 720c 0000 00da 0373 7472 7203 0000  ..r......strr...
+00000ce0: 0072 1600 0000 da08 7072 6f70 6572 7479  .r......property
+00000cf0: 722e 0000 0072 1e00 0000 7205 0000 0072  r....r....r....r
+00000d00: 2b00 0000 7206 0000 0072 0800 0000 722f  +...r....r....r/
+00000d10: 0000 0072 3200 0000 720e 0000 0072 0e00  ...r2...r....r..
+00000d20: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000d30: 0013 0000 0073 0c00 0000 0801 1205 0201  .....s..........
+00000d40: 100b 0e12 1015 7210 0000 0029 10da 076c  ......r....)...l
+00000d50: 6f67 6769 6e67 7221 0000 00da 0870 7964  oggingr!.....pyd
+00000d60: 616e 7469 6372 0200 0000 da0e 6967 5f74  anticr......ig_t
+00000d70: 7261 6469 6e67 5f6c 6962 7203 0000 00da  rading_libr.....
+00000d80: 066d 6f64 656c 7372 0500 0000 7206 0000  .modelsr....r...
+00000d90: 0072 0800 0000 da09 6765 744c 6f67 6765  .r......getLogge
+00000da0: 7272 0a00 0000 da06 6c6f 6767 6572 da09  rr......logger..
+00000db0: 4578 6365 7074 696f 6e72 0900 0000 7210  Exceptionr....r.
+00000dc0: 0000 0072 0e00 0000 720e 0000 0072 0e00  ...r....r....r..
+00000dd0: 0000 720f 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000de0: 3e01 0000 0073 1000 0000 0802 0801 0c02  >....s..........
+00000df0: 0c01 1001 0c03 0a03 1005                 ..........
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/models.py` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/models.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/service.py` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/orders/service.py`

 * *Files 26% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         except ValidationError as e:
             raise OrderException("Invalid working orders response: %s" % e)
         except requests.RequestException as e:
             raise OrderException("Working orders request failed: %s" % e)
 
 
     def create_working_order(self, working_order: CreateWorkingOrder) -> DealReference:
-        """Create a new working order"""
+        """Create a new working order
+        :param working_order: CreateWorkingOrder instance
+        :return: DealReference instance
+        """
         url = f"{self.base_url}/gateway/deal/workingorders/otc"
         try:
             response = requests.post(url, headers=self.headers, json=working_order.dict())
             if response.status_code == 200:
                 return DealReference.model_validate(response.json())
             else:
                 raise OrderException(
@@ -66,7 +69,26 @@
                 )
         except ValidationError as e:
             raise OrderException("Invalid create working order response: %s" % e)
         except requests.RequestException as e:
             raise OrderException("Create working order request failed: %s" % e)
 
 
+    def delete_working_order(self, deal_id: str) -> DealReference:
+        """Delete a working order
+        :param deal_id: str
+        :return: DealReference instance
+        """
+        url = f"{self.base_url}/gateway/deal/workingorders/otc/{deal_id}"
+        try:
+            response = requests.delete(url, headers=self.headers)
+            if response.status_code == 200:
+                return DealReference.model_validate(response.json())
+            else:
+                raise OrderException(
+                    "Delete working order failed with status code %s: %s"
+                    % (response.status_code, response.text)
+                )
+        except ValidationError as e:
+            raise OrderException("Invalid delete working order response: %s" % e)
+        except requests.RequestException as e:
+            raise OrderException("Delete working order request failed: %s" % e)
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/models.cpython-39.pyc` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  7 21:42:19 2024 UTC, .py size: 11119 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3b13 1366 6f2b 0000  a.......;..fo+..
+00000000: 610d 0d0a 0000 0000 9b30 3d66 bb2b 0000  a........0=f.+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6404 6405 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
@@ -21,21 +21,21 @@
 00000140: 2906 da09 4261 7365 4d6f 6465 6cda 0663  )...BaseModel..c
 00000150: 6f6e 7374 72da 0a63 6f6e 6465 6369 6d61  onstr..condecima
 00000160: 6cda 0663 6f6e 696e 74da 0f6d 6f64 656c  l..conint..model
 00000170: 5f76 616c 6964 6174 6f72 da10 6669 656c  _validator..fiel
 00000180: 645f 7365 7269 616c 697a 6572 e902 0000  d_serializer....
 00000190: 0029 02da 0e49 6e73 7472 756d 656e 7454  .)...InstrumentT
 000001a0: 7970 65da 0944 6972 6563 7469 6f6e 2907  ype..Direction).
-000001b0: da09 5452 4144 4541 424c 45da 0643 4c4f  ..TRADEABLE..CLO
-000001c0: 5345 44da 0a45 4449 5453 5f4f 4e4c 59da  SED..EDITS_ONLY.
-000001d0: 074f 4646 4c49 4e45 da0a 4f4e 5f41 5543  .OFFLINE..ON_AUC
-000001e0: 5449 4f4e da13 4f4e 5f41 5543 5449 4f4e  TION..ON_AUCTION
-000001f0: 5f4e 4f5f 4544 4954 53da 0953 5553 5045  _NO_EDITS..SUSPE
+000001b0: da09 5452 4144 4541 424c 455a 0643 4c4f  ..TRADEABLEZ.CLO
+000001c0: 5345 445a 0a45 4449 5453 5f4f 4e4c 595a  SEDZ.EDITS_ONLYZ
+000001d0: 074f 4646 4c49 4e45 5a0a 4f4e 5f41 5543  .OFFLINEZ.ON_AUC
+000001e0: 5449 4f4e 5a13 4f4e 5f41 5543 5449 4f4e  TIONZ.ON_AUCTION
+000001f0: 5f4e 4f5f 4544 4954 535a 0953 5553 5045  _NO_EDITSZ.SUSPE
 00000200: 4e44 4544 2903 da05 4c49 4d49 54da 064d  NDED)...LIMIT..M
-00000210: 4152 4b45 54da 0551 554f 5445 2902 5a15  ARKET..QUOTE).Z.
+00000210: 4152 4b45 54da 0551 554f 5445 2902 da15  ARKET..QUOTE)...
 00000220: 4558 4543 5554 455f 414e 445f 454c 494d  EXECUTE_AND_ELIM
 00000230: 494e 4154 455a 0c46 494c 4c5f 4f52 5f4b  INATEZ.FILL_OR_K
 00000240: 494c 4c63 0000 0000 0000 0000 0000 0000  ILLc............
 00000250: 0000 0000 0300 0000 4000 0000 7396 0000  ........@...s...
 00000260: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
 00000270: 013c 0065 0365 0464 023c 0065 0365 0464  .<.e.e.d.<.e.e.d
 00000280: 033c 0065 0565 0464 043c 0065 0665 0464  .<.e.e.d.<.e.e.d
@@ -61,24 +61,24 @@
 000003c0: 696e 6746 6163 746f 724e 290a da08 5f5f  ingFactorN)...__
 000003d0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 000003e0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 000003f0: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
 00000400: 696f 6e73 5f5f 720e 0000 00da 0566 6c6f  ions__r......flo
 00000410: 6174 da03 696e 74da 0462 6f6f 6cda 104d  at..int..bool..M
 00000420: 6172 6b65 7453 7461 7475 7354 7970 65a9  arketStatusType.
-00000430: 0072 3500 0000 7235 0000 00fa 5a2f 686f  .r5...r5....Z/ho
+00000430: 0072 3000 0000 7230 0000 00fa 5a2f 686f  .r0...r0....Z/ho
 00000440: 6d65 2f72 756e 6e65 722f 776f 726b 2f69  me/runner/work/i
-00000450: 675f 7472 6164 696e 675f 6c69 622f 6967  g_trading_lib/ig
-00000460: 5f74 7261 6469 6e67 5f6c 6962 2f69 675f  _trading_lib/ig_
+00000450: 672d 7472 6164 696e 672d 6c69 622f 6967  g-trading-lib/ig
+00000460: 2d74 7261 6469 6e67 2d6c 6962 2f69 675f  -trading-lib/ig_
 00000470: 7472 6164 696e 675f 6c69 622f 7472 6164  trading_lib/trad
 00000480: 696e 672f 706f 7369 7469 6f6e 732f 6d6f  ing/positions/mo
-00000490: 6465 6c73 2e70 7972 1a00 0000 1e00 0000  dels.pyr........
+00000490: 6465 6c73 2e70 7972 1500 0000 1e00 0000  dels.pyr........
 000004a0: 7322 0000 000a 0108 0108 0108 0108 0108  s"..............
 000004b0: 0108 0108 0108 0108 0108 0108 0108 0108  ................
-000004c0: 0108 0108 0108 0172 1a00 0000 6300 0000  .......r....c...
+000004c0: 0108 0108 0108 0172 1500 0000 6300 0000  .......r....c...
 000004d0: 0000 0000 0000 0000 0000 0000 0004 0000  ................
 000004e0: 0040 0000 0073 de00 0000 6500 5a01 6400  .@...s....e.Z.d.
 000004f0: 5a02 5500 6503 6401 6402 8d01 6504 6403  Z.U.e.d.d...e.d.
 00000500: 3c00 6505 6504 6404 3c00 6506 6504 6405  <.e.e.d.<.e.e.d.
 00000510: 3c00 6506 6504 6406 3c00 6506 6504 6407  <.e.e.d.<.e.e.d.
 00000520: 3c00 6506 6504 6408 3c00 6506 6504 6409  <.e.e.d.<.e.e.d.
 00000530: 3c00 6507 6504 640a 3c00 6503 6401 6402  <.e.e.d.<.e.d.d.
@@ -88,573 +88,578 @@
 00000570: 640e 3c00 6503 6401 6402 8d01 6504 640f  d.<.e.d.d...e.d.
 00000580: 3c00 640c 5a0b 6509 6503 6401 6402 8d01  <.d.Z.e.e.d.d...
 00000590: 1900 6504 6410 3c00 640c 5a0c 6509 650d  ..e.d.<.d.Z.e.e.
 000005a0: 6411 6412 8d01 1900 6504 6413 3c00 640c  d.d.....e.d.<.d.
 000005b0: 5a0e 6509 6503 6401 6402 8d01 1900 6504  Z.e.e.d.d.....e.
 000005c0: 6414 3c00 640c 5300 2915 da08 506f 7369  d.<.d.S.)...Posi
 000005d0: 7469 6f6e 720d 0000 00a9 01da 0e64 6563  tionr........dec
-000005e0: 696d 616c 5f70 6c61 6365 73da 0c63 6f6e  imal_places..con
-000005f0: 7472 6163 7453 697a 65da 0e63 6f6e 7472  tractSize..contr
+000005e0: 696d 616c 5f70 6c61 6365 735a 0c63 6f6e  imal_placesZ.con
+000005f0: 7472 6163 7453 697a 655a 0e63 6f6e 7472  tractSizeZ.contr
 00000600: 6f6c 6c65 6452 6973 6bda 0b63 7265 6174  olledRisk..creat
 00000610: 6564 4461 7465 da0e 6372 6561 7465 6444  edDate..createdD
 00000620: 6174 6555 5443 da08 6375 7272 656e 6379  ateUTC..currency
 00000630: da06 6465 616c 4964 da0d 6465 616c 5265  ..dealId..dealRe
 00000640: 6665 7265 6e63 65da 0964 6972 6563 7469  ference..directi
 00000650: 6f6e da05 6c65 7665 6c4e da0a 6c69 6d69  on..levelN..limi
 00000660: 744c 6576 656c da12 6c69 6d69 7465 6452  tLevel..limitedR
 00000670: 6973 6b50 7265 6d69 756d da04 7369 7a65  iskPremium..size
 00000680: da09 7374 6f70 4c65 7665 6c72 0100 0000  ..stopLevelr....
 00000690: 2901 da02 6765 da0c 7472 6169 6c69 6e67  )...ge..trailing
 000006a0: 5374 6570 da14 7472 6169 6c69 6e67 5374  Step..trailingSt
-000006b0: 6f70 4469 7374 616e 6365 290f 722c 0000  opDistance).r,..
-000006c0: 0072 2d00 0000 722e 0000 0072 0900 0000  .r-...r....r....
-000006d0: 7230 0000 0072 3300 0000 722f 0000 0072  r0...r3...r/...r
-000006e0: 0f00 0000 7243 0000 0072 0600 0000 7244  ....rC...r....rD
-000006f0: 0000 0072 4600 0000 7248 0000 0072 0a00  ...rF...rH...r..
-00000700: 0000 7249 0000 0072 3500 0000 7235 0000  ..rI...r5...r5..
-00000710: 0072 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
+000006b0: 6f70 4469 7374 616e 6365 290f 7227 0000  opDistance).r'..
+000006c0: 0072 2800 0000 7229 0000 0072 0900 0000  .r(...r)...r....
+000006d0: 722b 0000 0072 2e00 0000 722a 0000 0072  r+...r....r*...r
+000006e0: 0f00 0000 723c 0000 0072 0600 0000 723d  ....r<...r....r=
+000006f0: 0000 0072 3f00 0000 7241 0000 0072 0a00  ...r?...rA...r..
+00000700: 0000 7242 0000 0072 3000 0000 7230 0000  ..rB...r0...r0..
+00000710: 0072 3000 0000 7231 0000 0072 3200 0000  .r0...r1...r2...
 00000720: 3200 0000 731e 0000 000a 010e 0108 0108  2...s...........
 00000730: 0108 0108 0108 0108 0108 010e 0116 0116  ................
-00000740: 010e 0116 0116 0172 3700 0000 6300 0000  .......r7...c...
+00000740: 010e 0116 0116 0172 3200 0000 6300 0000  .......r2...c...
 00000750: 0000 0000 0000 0000 0000 0000 0003 0000  ................
 00000760: 0040 0000 0073 1e00 0000 6500 5a01 6400  .@...s....e.Z.d.
 00000770: 5a02 5500 6503 6504 6401 3c00 6505 6504  Z.U.e.e.d.<.e.e.
 00000780: 6402 3c00 6403 5300 2904 da0c 4f70 656e  d.<.d.S.)...Open
 00000790: 506f 7369 7469 6f6e da08 706f 7369 7469  Position..positi
-000007a0: 6f6e da06 6d61 726b 6574 4e29 0672 2c00  on..marketN).r,.
-000007b0: 0000 722d 0000 0072 2e00 0000 7237 0000  ..r-...r....r7..
-000007c0: 0072 3000 0000 721a 0000 0072 3500 0000  .r0...r....r5...
-000007d0: 7235 0000 0072 3500 0000 7236 0000 0072  r5...r5...r6...r
-000007e0: 4a00 0000 4400 0000 7304 0000 000a 0108  J...D...s.......
-000007f0: 0172 4a00 0000 6300 0000 0000 0000 0000  .rJ...c.........
+000007a0: 6f6e 5a06 6d61 726b 6574 4e29 0672 2700  onZ.marketN).r'.
+000007b0: 0000 7228 0000 0072 2900 0000 7232 0000  ..r(...r)...r2..
+000007c0: 0072 2b00 0000 7215 0000 0072 3000 0000  .r+...r....r0...
+000007d0: 7230 0000 0072 3000 0000 7231 0000 0072  r0...r0...r1...r
+000007e0: 4300 0000 4400 0000 7304 0000 000a 0108  C...D...s.......
+000007f0: 0172 4300 0000 6300 0000 0000 0000 0000  .rC...c.........
 00000800: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
 00000810: 1a00 0000 6500 5a01 6400 5a02 5500 6503  ....e.Z.d.Z.U.e.
 00000820: 6504 1900 6505 6401 3c00 6402 5300 2903  e...e.d.<.d.S.).
-00000830: da0d 4f70 656e 506f 7369 7469 6f6e 73da  ..OpenPositions.
-00000840: 0970 6f73 6974 696f 6e73 4e29 0672 2c00  .positionsN).r,.
-00000850: 0000 722d 0000 0072 2e00 0000 7203 0000  ..r-...r....r...
-00000860: 0072 4a00 0000 7230 0000 0072 3500 0000  .rJ...r0...r5...
-00000870: 7235 0000 0072 3500 0000 7236 0000 0072  r5...r5...r6...r
-00000880: 4d00 0000 4900 0000 7302 0000 000a 0172  M...I...s......r
-00000890: 4d00 0000 6300 0000 0000 0000 0000 0000  M...c...........
-000008a0: 0000 0000 000a 0000 0040 0000 0073 e001  .........@...s..
+00000830: da0d 4f70 656e 506f 7369 7469 6f6e 735a  ..OpenPositionsZ
+00000840: 0970 6f73 6974 696f 6e73 4e29 0672 2700  .positionsN).r'.
+00000850: 0000 7228 0000 0072 2900 0000 7203 0000  ..r(...r)...r...
+00000860: 0072 4300 0000 722b 0000 0072 3000 0000  .rC...r+...r0...
+00000870: 7230 0000 0072 3000 0000 7231 0000 0072  r0...r0...r1...r
+00000880: 4500 0000 4900 0000 7302 0000 000a 0172  E...I...s......r
+00000890: 4500 0000 6300 0000 0000 0000 0000 0000  E...c...........
+000008a0: 0000 0000 000a 0000 0040 0000 0073 f801  .........@...s..
 000008b0: 0000 6500 5a01 6400 5a02 5500 6503 6401  ..e.Z.d.Z.U.e.d.
 000008c0: 6402 8d01 6504 6403 3c00 6505 6504 6404  d...e.d.<.e.e.d.
 000008d0: 3c00 6503 6405 6402 8d01 6504 6406 3c00  <.e.d.d...e.d.<.
-000008e0: 6503 6407 6402 8d01 6504 6408 3c00 6506  e.d.d...e.d.<.e.
-000008f0: 6504 6409 3c00 6506 6504 640a 3c00 6507  e.d.<.e.e.d.<.e.
-00000900: 6504 640b 3c00 6508 6504 640c 3c00 6506  e.d.<.e.e.d.<.e.
-00000910: 6504 640d 3c00 640e 5a09 650a 6503 640f  e.d.<.d.Z.e.e.d.
-00000920: 6402 8d01 1900 6504 6410 3c00 640e 5a0b  d.....e.d.<.d.Z.
-00000930: 650a 650c 6411 6412 8d01 1900 6504 6413  e.e.d.d.....e.d.
-00000940: 3c00 640e 5a0d 650a 650c 6414 6412 8d01  <.d.Z.e.e.d.d...
-00000950: 1900 6504 6415 3c00 640e 5a0e 650a 650c  ..e.d.<.d.Z.e.e.
-00000960: 6414 6412 8d01 1900 6504 6416 3c00 640e  d.d.....e.d.<.d.
-00000970: 5a0f 650a 6503 6417 6402 8d01 1900 6504  Z.e.e.d.d.....e.
-00000980: 6418 3c00 650c 6414 6419 641a 8d02 6504  d.<.e.d.d.d...e.
-00000990: 641b 3c00 640e 5a10 650a 650c 6414 6412  d.<.d.Z.e.e.d.d.
-000009a0: 8d01 1900 6504 641c 3c00 640e 5a11 650a  ....e.d.<.d.Z.e.
-000009b0: 650c 6414 6412 8d01 1900 6504 641d 3c00  e.d.d.....e.d.<.
-000009c0: 640e 5a12 650a 650c 6414 6412 8d01 1900  d.Z.e.e.d.d.....
-000009d0: 6504 641e 3c00 6513 6413 6415 6416 641b  e.d.<.e.d.d.d.d.
-000009e0: 641c 641d 641e 641f 6420 8d08 650a 6514  d.d.d.d.d ..e.e.
-000009f0: 1900 6515 6421 9c02 6422 6423 8404 8301  ..e.d!..d"d#....
-00000a00: 5a16 6517 6424 6420 8d01 6518 6519 6425  Z.e.d$d ..e.e.d%
-00000a10: 9c01 6426 6427 8404 8301 8301 5a1a 6517  ..d&d'......Z.e.
-00000a20: 6424 6420 8d01 6518 6519 6425 9c01 6428  d$d ..e.e.d%..d(
-00000a30: 6429 8404 8301 8301 5a1b 6517 6424 6420  d)......Z.e.d$d 
-00000a40: 8d01 6518 6519 6425 9c01 642a 642b 8404  ..e.e.d%..d*d+..
-00000a50: 8301 8301 5a1c 6517 6424 6420 8d01 6518  ....Z.e.d$d ..e.
-00000a60: 6519 6425 9c01 642c 642d 8404 8301 8301  e.d%..d,d-......
-00000a70: 5a1d 6517 6424 6420 8d01 6518 6519 6425  Z.e.d$d ..e.e.d%
-00000a80: 9c01 642e 642f 8404 8301 8301 5a1e 640e  ..d.d/......Z.d.
-00000a90: 5300 2930 da0e 4372 6561 7465 506f 7369  S.)0..CreatePosi
-00000aa0: 7469 6f6e 7a0a 5e5b 412d 5a5d 7b33 7d24  tionz.^[A-Z]{3}$
-00000ab0: a901 da07 7061 7474 6572 6eda 0c63 7572  ....pattern..cur
-00000ac0: 7265 6e63 7943 6f64 6572 4100 0000 7a15  rencyCoderA...z.
-00000ad0: 5e5b 412d 5a61 2d7a 302d 392e 5f5d 7b36  ^[A-Za-z0-9._]{6
-00000ae0: 2c33 307d 2472 1d00 0000 7a1f 5e28 5c64  ,30}$r....z.^(\d
-00000af0: 7b32 7d2d 293f 5b41 2d5a 5d7b 337d 2d5c  {2}-)?[A-Z]{3}-\
-00000b00: 647b 327d 7c2d 7c44 4642 2472 1c00 0000  d{2}|-|DFB$r....
-00000b10: da09 666f 7263 654f 7065 6eda 0e67 7561  ..forceOpen..gua
-00000b20: 7261 6e74 6565 6453 746f 70da 096f 7264  ranteedStop..ord
-00000b30: 6572 5479 7065 da0b 7469 6d65 496e 466f  erType..timeInFo
-00000b40: 7263 65da 0c74 7261 696c 696e 6753 746f  rce..trailingSto
-00000b50: 704e 7a17 5e5b 412d 5a61 2d7a 302d 395f  pNz.^[A-Za-z0-9_
-00000b60: 5c2d 2e5d 7b31 2c33 307d 2472 4000 0000  \-.]{1,30}$r@...
-00000b70: e90c 0000 0072 3800 0000 7242 0000 0072  .....r8...rB...r
-00000b80: 0d00 0000 da0d 6c69 6d69 7444 6973 7461  ......limitDista
-00000b90: 6e63 6572 4300 0000 7a0e 5e5b 412d 5a61  ncerC...z.^[A-Za
-00000ba0: 2d7a 302d 395d 2b24 da07 7175 6f74 6549  -z0-9]+$..quoteI
-00000bb0: 6472 0100 0000 2902 7239 0000 00da 0267  dr....).r9.....g
-00000bc0: 7472 4500 0000 da0c 7374 6f70 4469 7374  trE.....stopDist
-00000bd0: 616e 6365 7246 0000 00da 1574 7261 696c  ancerF.....trail
-00000be0: 696e 6753 746f 7049 6e63 7265 6d65 6e74  ingStopIncrement
-00000bf0: da05 706c 6169 6ea9 01da 046d 6f64 65a9  ..plain....mode.
-00000c00: 02da 0176 da06 7265 7475 726e 6303 0000  ...v..returnc...
-00000c10: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-00000c20: 0043 0000 0073 1400 0000 7c01 6400 7501  .C...s....|.d.u.
-00000c30: 7210 7400 7c01 8301 5300 6400 5300 a901  r.t.|...S.d.S...
-00000c40: 4ea9 0172 3100 0000 a903 da04 7365 6c66  N..r1.......self
-00000c50: 7262 0000 00da 055f 696e 666f 7235 0000  rb....._infor5..
-00000c60: 0072 3500 0000 7236 0000 00da 1173 6572  .r5...r6.....ser
-00000c70: 6961 6c69 7a65 5f64 6563 696d 616c 6100  ialize_decimala.
-00000c80: 0000 7304 0000 0000 0b08 017a 2043 7265  ..s........z Cre
-00000c90: 6174 6550 6f73 6974 696f 6e2e 7365 7269  atePosition.seri
-00000ca0: 616c 697a 655f 6465 6369 6d61 6cda 0662  alize_decimal..b
-00000cb0: 6566 6f72 65a9 01da 0464 6174 6163 0200  efore....datac..
-00000cc0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00000cd0: 0000 4300 0000 734c 0000 007c 01a0 0064  ..C...sL...|...d
-00000ce0: 01a1 0164 0075 0172 247c 01a0 0064 02a1  ...d.u.r$|...d..
-00000cf0: 0164 0075 0172 2474 0164 0383 0182 017c  .d.u.r$t.d.....|
-00000d00: 01a0 0064 04a1 0164 0075 0172 487c 01a0  ...d...d.u.rH|..
-00000d10: 0064 05a1 0164 0075 0172 4874 0164 0683  .d...d.u.rHt.d..
-00000d20: 0182 017c 0153 0029 074e 7243 0000 0072  ...|.S.).NrC...r
-00000d30: 5900 0000 7a2c 5365 7420 6f6e 6c79 206f  Y...z,Set only o
-00000d40: 6e65 206f 6620 6c69 6d69 744c 6576 656c  ne of limitLevel
-00000d50: 206f 7220 6c69 6d69 7444 6973 7461 6e63   or limitDistanc
-00000d60: 652e 7246 0000 0072 5c00 0000 7a2a 5365  e.rF...r\...z*Se
-00000d70: 7420 6f6e 6c79 206f 6e65 206f 6620 7374  t only one of st
-00000d80: 6f70 4c65 7665 6c20 6f72 2073 746f 7044  opLevel or stopD
-00000d90: 6973 7461 6e63 652e a902 da03 6765 74da  istance.....get.
-00000da0: 0a56 616c 7565 4572 726f 72a9 02da 0363  .ValueError....c
-00000db0: 6c73 726c 0000 0072 3500 0000 7235 0000  lsrl...r5...r5..
-00000dc0: 0072 3600 0000 da18 6368 6563 6b5f 756e  .r6.....check_un
-00000dd0: 6971 7565 5f63 6f6e 7374 7261 696e 7473  ique_constraints
-00000de0: 6f00 0000 730a 0000 0000 031c 0108 011c  o...s...........
-00000df0: 0108 017a 2743 7265 6174 6550 6f73 6974  ...z'CreatePosit
-00000e00: 696f 6e2e 6368 6563 6b5f 756e 6971 7565  ion.check_unique
-00000e10: 5f63 6f6e 7374 7261 696e 7473 6302 0000  _constraintsc...
-00000e20: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-00000e30: 0043 0000 0073 4e00 0000 7c01 a000 6401  .C...sN...|...d.
-00000e40: a101 734a 7401 7c01 a000 6402 a101 6400  ..sJt.|...d...d.
-00000e50: 7501 7c01 a000 6403 a101 6400 7501 7c01  u.|...d...d.u.|.
-00000e60: a000 6404 a101 6400 7501 7c01 a000 6405  ..d...d.u.|...d.
-00000e70: a101 6400 7501 6704 8301 724a 7402 6406  ..d.u.g...rJt.d.
-00000e80: 8301 8201 7c01 5300 2907 4e72 5300 0000  ....|.S.).NrS...
-00000e90: 7259 0000 0072 4300 0000 725c 0000 0072  rY...rC...r\...r
-00000ea0: 4600 0000 7a3c 666f 7263 654f 7065 6e20  F...z<forceOpen 
-00000eb0: 6d75 7374 2062 6520 7472 7565 2069 6620  must be true if 
-00000ec0: 6c69 6d69 7420 6f72 2073 746f 7020 636f  limit or stop co
-00000ed0: 6e73 7472 6169 6e74 7320 6172 6520 7365  nstraints are se
-00000ee0: 742e 2903 726e 0000 00da 0361 6e79 726f  t.).rn.....anyro
-00000ef0: 0000 0072 7000 0000 7235 0000 0072 3500  ...rp...r5...r5.
-00000f00: 0000 7236 0000 00da 1c63 6865 636b 5f66  ..r6.....check_f
-00000f10: 6f72 6365 5f6f 7065 6e5f 636f 6e73 7472  orce_open_constr
-00000f20: 6169 6e74 7378 0000 0073 1600 0000 0003  aintsx...s......
-00000f30: 0c02 0c01 0c01 0c01 0cfc 02ff 0408 0201  ................
-00000f40: 02ff 0403 7a2b 4372 6561 7465 506f 7369  ....z+CreatePosi
-00000f50: 7469 6f6e 2e63 6865 636b 5f66 6f72 6365  tion.check_force
-00000f60: 5f6f 7065 6e5f 636f 6e73 7472 6169 6e74  _open_constraint
-00000f70: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
-00000f80: 0000 0500 0000 4300 0000 7332 0000 007c  ......C...s2...|
-00000f90: 01a0 0064 01a1 0172 2e74 017c 01a0 0064  ...d...r.t.|...d
-00000fa0: 02a1 0183 0174 017c 01a0 0064 03a1 0183  .....t.|...d....
-00000fb0: 0141 0073 2e74 0264 0483 0182 017c 0153  .A.s.t.d.....|.S
-00000fc0: 0029 054e 7254 0000 0072 4600 0000 725c  .).NrT...rF...r\
-00000fd0: 0000 007a 4e57 6865 6e20 6775 6172 616e  ...zNWhen guaran
-00000fe0: 7465 6564 5374 6f70 2069 7320 7472 7565  teedStop is true
-00000ff0: 2c20 7370 6563 6966 7920 6578 6163 746c  , specify exactl
-00001000: 7920 6f6e 6520 6f66 2073 746f 704c 6576  y one of stopLev
-00001010: 656c 206f 7220 7374 6f70 4469 7374 616e  el or stopDistan
-00001020: 6365 2e29 0372 6e00 0000 7233 0000 0072  ce.).rn...r3...r
-00001030: 6f00 0000 7270 0000 0072 3500 0000 7235  o...rp...r5...r5
-00001040: 0000 0072 3600 0000 da21 6368 6563 6b5f  ...r6....!check_
-00001050: 6775 6172 616e 7465 6564 5f73 746f 705f  guaranteed_stop_
-00001060: 636f 6e73 7472 6169 6e74 7388 0000 0073  constraints....s
-00001070: 0e00 0000 0003 0a01 1aff 0203 0201 02ff  ................
-00001080: 0403 7a30 4372 6561 7465 506f 7369 7469  ..z0CreatePositi
-00001090: 6f6e 2e63 6865 636b 5f67 7561 7261 6e74  on.check_guarant
-000010a0: 6565 645f 7374 6f70 5f63 6f6e 7374 7261  eed_stop_constra
-000010b0: 696e 7473 6302 0000 0000 0000 0000 0000  intsc...........
-000010c0: 0003 0000 0005 0000 0043 0000 0073 a600  .........C...s..
-000010d0: 0000 7c01 a000 6401 a101 7d02 7c02 6402  ..|...d...}.|.d.
-000010e0: 6b02 7240 7c01 a000 6403 a101 6400 7501  k.r@|...d...d.u.
-000010f0: 7228 7401 6404 8301 8201 7c01 a000 6405  r(t.d.....|...d.
-00001100: a101 6400 7500 72a2 7401 6406 8301 8201  ..d.u.r.t.d.....
-00001110: 6e62 7c02 6407 6b02 7272 7402 7c01 a000  nb|.d.k.rrt.|...
-00001120: 6405 a101 6400 7501 7c01 a000 6403 a101  d...d.u.|...d...
-00001130: 6400 7501 6702 8301 72a2 7401 6408 8301  d.u.g...r.t.d...
-00001140: 8201 6e30 7c02 6409 6b02 72a2 7403 7c01  ..n0|.d.k.r.t.|.
-00001150: a000 6405 a101 6400 7501 7c01 a000 6403  ..d...d.u.|...d.
-00001160: a101 6400 7501 6702 8301 73a2 7401 640a  ..d.u.g...s.t.d.
-00001170: 8301 8201 7c01 5300 290b 4e72 5500 0000  ....|.S.).NrU...
-00001180: 7217 0000 0072 5a00 0000 7a2b 446f 206e  r....rZ...z+Do n
-00001190: 6f74 2073 6574 2071 756f 7465 4964 2077  ot set quoteId w
-000011a0: 6865 6e20 6f72 6465 7254 7970 6520 6973  hen orderType is
-000011b0: 204c 494d 4954 2e72 4200 0000 7a22 5365   LIMIT.rB...z"Se
-000011c0: 7420 6c65 7665 6c20 7768 656e 206f 7264  t level when ord
-000011d0: 6572 5479 7065 2069 7320 4c49 4d49 542e  erType is LIMIT.
-000011e0: 7218 0000 007a 3544 6f20 6e6f 7420 7365  r....z5Do not se
-000011f0: 7420 6c65 7665 6c20 6f72 2071 756f 7465  t level or quote
-00001200: 4964 2077 6865 6e20 6f72 6465 7254 7970  Id when orderTyp
-00001210: 6520 6973 204d 4152 4b45 542e 7219 0000  e is MARKET.r...
-00001220: 007a 3353 6574 2062 6f74 6820 6c65 7665  .z3Set both leve
-00001230: 6c20 616e 6420 7175 6f74 6549 6420 7768  l and quoteId wh
-00001240: 656e 206f 7264 6572 5479 7065 2069 7320  en orderType is 
-00001250: 5155 4f54 452e 2904 726e 0000 0072 6f00  QUOTE.).rn...ro.
-00001260: 0000 7273 0000 00da 0361 6c6c 2903 7271  ..rs.....all).rq
-00001270: 0000 0072 6c00 0000 5a0a 6f72 6465 725f  ...rl...Z.order_
-00001280: 7479 7065 7235 0000 0072 3500 0000 7236  typer5...r5...r6
-00001290: 0000 00da 1c63 6865 636b 5f6f 7264 6572  .....check_order
-000012a0: 5f74 7970 655f 636f 6e73 7472 6169 6e74  _type_constraint
-000012b0: 7393 0000 0073 2200 0000 0003 0a01 0801  s....s".........
-000012c0: 0e01 0801 0e01 0a01 0801 2001 0201 02ff  .......... .....
-000012d0: 0603 0801 0201 1aff 0403 0801 7a2b 4372  ............z+Cr
-000012e0: 6561 7465 506f 7369 7469 6f6e 2e63 6865  eatePosition.che
-000012f0: 636b 5f6f 7264 6572 5f74 7970 655f 636f  ck_order_type_co
-00001300: 6e73 7472 6169 6e74 7363 0200 0000 0000  nstraintsc......
-00001310: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
-00001320: 0000 735e 0000 007c 01a0 0064 01a1 0172  ..s^...|...d...r
-00001330: 5a7c 01a0 0064 02a1 0164 0075 0172 2074  Z|...d...d.u.r t
-00001340: 0164 0383 0182 017c 01a0 0064 04a1 0172  .d.....|...d...r
-00001350: 3274 0164 0583 0182 0174 027c 01a0 0064  2t.d.....t.|...d
-00001360: 06a1 0164 0075 017c 01a0 0064 07a1 0164  ...d.u.|...d...d
-00001370: 0075 0167 0283 0173 5a74 0164 0883 0182  .u.g...sZt.d....
-00001380: 017c 0153 0029 094e 7257 0000 0072 4600  .|.S.).NrW...rF.
-00001390: 0000 7a2f 446f 206e 6f74 2073 6574 2073  ..z/Do not set s
-000013a0: 746f 704c 6576 656c 2077 6865 6e20 7472  topLevel when tr
-000013b0: 6169 6c69 6e67 5374 6f70 2069 7320 7472  ailingStop is tr
-000013c0: 7565 2e72 5400 0000 7a37 6775 6172 616e  ue.rT...z7guaran
-000013d0: 7465 6564 5374 6f70 206d 7573 7420 6265  teedStop must be
-000013e0: 2066 616c 7365 2077 6865 6e20 7472 6169   false when trai
-000013f0: 6c69 6e67 5374 6f70 2069 7320 7472 7565  lingStop is true
-00001400: 2e72 5c00 0000 725d 0000 007a 4a53 6574  .r\...r]...zJSet
-00001410: 2062 6f74 6820 7374 6f70 4469 7374 616e   both stopDistan
-00001420: 6365 2061 6e64 2074 7261 696c 696e 6753  ce and trailingS
-00001430: 746f 7049 6e63 7265 6d65 6e74 2077 6865  topIncrement whe
-00001440: 6e20 7472 6169 6c69 6e67 5374 6f70 2069  n trailingStop i
-00001450: 7320 7472 7565 2e29 0372 6e00 0000 726f  s true.).rn...ro
-00001460: 0000 0072 7600 0000 7270 0000 0072 3500  ...rv...rp...r5.
-00001470: 0000 7235 0000 0072 3600 0000 da1f 6368  ..r5...r6.....ch
-00001480: 6563 6b5f 7472 6169 6c69 6e67 5f73 746f  eck_trailing_sto
-00001490: 705f 636f 6e73 7472 6169 6e74 73a8 0000  p_constraints...
-000014a0: 0073 2000 0000 0003 0a01 0e01 0801 0a01  .s .............
-000014b0: 0201 02ff 0403 0202 0c01 0cfe 02ff 0406  ................
-000014c0: 0201 02ff 0403 7a2e 4372 6561 7465 506f  ......z.CreatePo
-000014d0: 7369 7469 6f6e 2e63 6865 636b 5f74 7261  sition.check_tra
-000014e0: 696c 696e 675f 7374 6f70 5f63 6f6e 7374  iling_stop_const
-000014f0: 7261 696e 7473 291f 722c 0000 0072 2d00  raints).r,...r-.
-00001500: 0000 722e 0000 0072 0800 0000 7230 0000  ..r....r....r0..
-00001510: 0072 0f00 0000 7233 0000 00da 094f 7264  .r....r3.....Ord
-00001520: 6572 5479 7065 da0b 5469 6d65 496e 466f  erType..TimeInFo
-00001530: 7263 6572 4000 0000 7206 0000 0072 4200  rcer@...r....rB.
-00001540: 0000 7209 0000 0072 5900 0000 7243 0000  ..r....rY...rC..
-00001550: 0072 5a00 0000 725c 0000 0072 4600 0000  .rZ...r\...rF...
-00001560: 725d 0000 0072 0c00 0000 7202 0000 0072  r]...r....r....r
-00001570: 3100 0000 7269 0000 0072 0b00 0000 da0b  1...ri...r......
-00001580: 636c 6173 736d 6574 686f 6472 0400 0000  classmethodr....
-00001590: 7272 0000 0072 7400 0000 7275 0000 0072  rr...rt...ru...r
-000015a0: 7700 0000 7278 0000 0072 3500 0000 7235  w...rx...r5...r5
-000015b0: 0000 0072 3500 0000 7236 0000 0072 4f00  ...r5...r6...rO.
-000015c0: 0000 4d00 0000 7358 0000 000a 010e 0108  ..M...sX........
-000015d0: 010e 010e 0108 0108 0108 0108 0108 0116  ................
-000015e0: 0116 0116 0116 0116 0110 0116 0116 0116  ................
-000015f0: 0202 0102 0102 0102 0102 0102 0102 0102  ................
-00001600: 0102 f804 0a16 0408 0102 0112 0708 0102  ................
-00001610: 0112 0e08 0102 0112 0908 0102 0112 1308  ................
-00001620: 0102 0172 4f00 0000 6300 0000 0000 0000  ...rO...c.......
-00001630: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-00001640: 0073 0e01 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-00001650: 6503 6504 6401 3c00 6505 6504 6402 3c00  e.e.d.<.e.e.d.<.
-00001660: 6506 6403 6404 6405 8d02 6504 6406 3c00  e.d.d.d...e.d.<.
-00001670: 6507 6504 6407 3c00 6408 5a08 6509 650a  e.e.d.<.d.Z.e.e.
-00001680: 1900 6504 6409 3c00 6408 5a0b 6509 650c  ..e.d.<.d.Z.e.e.
-00001690: 640a 640b 8d01 1900 6504 640c 3c00 6408  d.d.....e.d.<.d.
-000016a0: 5a0d 6509 650c 640d 640b 8d01 1900 6504  Z.e.e.d.d.....e.
-000016b0: 640e 3c00 6408 5a0e 6509 650c 640f 640b  d.<.d.Z.e.e.d.d.
-000016c0: 8d01 1900 6504 6410 3c00 6408 5a0f 6509  ....e.d.<.d.Z.e.
-000016d0: 6506 6411 6412 8d01 1900 6504 6413 3c00  e.d.d.....e.d.<.
-000016e0: 6510 6413 6406 6414 6415 8d03 6509 6511  e.d.d.d.d...e.e.
-000016f0: 1900 6509 6512 1900 6416 9c02 6417 6418  ..e.e...d...d.d.
-00001700: 8404 8301 5a13 6514 6419 6415 8d01 6515  ....Z.e.d.d...e.
-00001710: 6516 641a 9c01 641b 641c 8404 8301 8301  e.d...d.d.......
-00001720: 5a17 6514 6419 6415 8d01 6515 6516 641a  Z.e.d.d...e.e.d.
-00001730: 9c01 641d 641e 8404 8301 8301 5a18 6515  ..d.d.......Z.e.
-00001740: 6519 641f 9c01 6420 6421 8404 8301 5a1a  e.d...d d!....Z.
-00001750: 6408 5300 2922 da0d 436c 6f73 6550 6f73  d.S.)"..ClosePos
-00001760: 6974 696f 6e72 4100 0000 7255 0000 0072  itionrA...rU...r
-00001770: 0100 0000 720d 0000 0029 0272 5b00 0000  ....r....).r[...
-00001780: 7239 0000 0072 4500 0000 7256 0000 004e  r9...rE...rV...N
-00001790: 725a 0000 007a 072e 7b31 2c33 307d 7250  rZ...z..{1,30}rP
-000017a0: 0000 0072 3f00 0000 7a13 5b41 2d5a 612d  ...r?...z.[A-Za-
-000017b0: 7a30 2d39 2e5f 5d7b 362c 3330 7d72 1d00  z0-9._]{6,30}r..
-000017c0: 0000 7a1d 285c 647b 327d 2d29 3f5b 412d  ..z.(\d{2}-)?[A-
-000017d0: 5a5d 7b33 7d2d 5c64 7b32 7d7c 2d7c 4446  Z]{3}-\d{2}|-|DF
-000017e0: 4272 1c00 0000 7258 0000 0072 3800 0000  Br....rX...r8...
-000017f0: 7242 0000 0072 5e00 0000 725f 0000 0072  rB...r^...r_...r
-00001800: 6100 0000 6303 0000 0000 0000 0000 0000  a...c...........
-00001810: 0003 0000 0002 0000 0043 0000 0073 1400  .........C...s..
-00001820: 0000 7c01 6400 7501 7210 7400 7c01 8301  ..|.d.u.r.t.|...
-00001830: 5300 6400 5300 7264 0000 0072 6500 0000  S.d.S.rd...re...
-00001840: 7266 0000 0072 3500 0000 7235 0000 0072  rf...r5...r5...r
-00001850: 3600 0000 7269 0000 00c9 0000 0073 0400  6...ri.......s..
-00001860: 0000 0002 0801 7a1f 436c 6f73 6550 6f73  ......z.ClosePos
-00001870: 6974 696f 6e2e 7365 7269 616c 697a 655f  ition.serialize_
-00001880: 6465 6369 6d61 6c72 6a00 0000 726b 0000  decimalrj...rk..
-00001890: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-000018a0: 0000 0300 0000 4300 0000 73b0 0000 007c  ......C...s....|
-000018b0: 01a0 0064 01a1 0164 026b 0272 327c 01a0  ...d...d.k.r2|..
-000018c0: 0064 03a1 0164 0075 0073 2a7c 01a0 0064  .d...d.u.s*|...d
-000018d0: 04a1 0164 0075 0072 3274 0164 0583 0182  ...d.u.r2t.d....
-000018e0: 017c 01a0 0064 01a1 0164 066b 0272 647c  .|...d...d.k.rd|
-000018f0: 01a0 0064 04a1 0164 0075 0170 567c 01a0  ...d...d.u.pV|..
-00001900: 0064 03a1 0164 0075 0172 6474 0164 0783  .d...d.u.rdt.d..
-00001910: 0182 017c 01a0 0064 01a1 0164 086b 0272  ...|...d...d.k.r
-00001920: 887c 01a0 0064 03a1 0164 0075 0172 8874  .|...d...d.u.r.t
-00001930: 0164 0983 0182 017c 01a0 0064 01a1 0164  .d.....|...d...d
-00001940: 086b 0272 ac7c 01a0 0064 04a1 0164 0075  .k.r.|...d...d.u
-00001950: 0072 ac74 0164 0a83 0182 017c 0153 0029  .r.t.d.....|.S.)
-00001960: 0b4e 7255 0000 0072 1900 0000 725a 0000  .NrU...r....rZ..
-00001970: 0072 4200 0000 7a2c 7175 6f74 6549 6420  .rB...z,quoteId 
-00001980: 6973 2072 6571 7569 7265 6420 7768 656e  is required when
-00001990: 206f 7264 6572 5479 7065 2069 7320 5155   orderType is QU
-000019a0: 4f54 452e 7218 0000 007a 3b6c 6576 656c  OTE.r....z;level
-000019b0: 2061 6e64 2071 756f 7465 4964 2061 7265   and quoteId are
-000019c0: 206e 6f74 2061 6c6c 6f77 6564 2077 6865   not allowed whe
-000019d0: 6e20 6f72 6465 7254 7970 6520 6973 204d  n orderType is M
-000019e0: 4152 4b45 542e 7217 0000 007a 2f71 756f  ARKET.r....z/quo
-000019f0: 7465 4964 2069 7320 6e6f 7420 616c 6c6f  teId is not allo
-00001a00: 7765 6420 7768 656e 206f 7264 6572 5479  wed when orderTy
-00001a10: 7065 2069 7320 4c49 4d49 542e 7a2a 6c65  pe is LIMIT.z*le
-00001a20: 7665 6c20 6973 2072 6571 7569 7265 6420  vel is required 
-00001a30: 7768 656e 206f 7264 6572 5479 7065 2069  when orderType i
-00001a40: 7320 4c49 4d49 542e 726d 0000 0072 7000  s LIMIT.rm...rp.
-00001a50: 0000 7235 0000 0072 3500 0000 7236 0000  ..r5...r5...r6..
-00001a60: 00da 1063 6865 636b 5f6f 7264 6572 5f74  ...check_order_t
-00001a70: 7970 65ce 0000 0073 2400 0000 0003 0e01  ype....s$.......
-00001a80: 0cff 0201 0cff 0203 0803 0cff 0202 1afe  ................
-00001a90: 0204 0201 02ff 0404 1c01 0802 1c01 0802  ................
-00001aa0: 7a1e 436c 6f73 6550 6f73 6974 696f 6e2e  z.ClosePosition.
-00001ab0: 6368 6563 6b5f 6f72 6465 725f 7479 7065  check_order_type
-00001ac0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001ad0: 0003 0000 0043 0000 0073 4c00 0000 7c01  .....C...sL...|.
-00001ae0: a000 6401 a101 6400 7501 7224 7c01 a000  ..d...d.u.r$|...
-00001af0: 6402 a101 6400 7501 7224 7401 6403 8301  d...d.u.r$t.d...
-00001b00: 8201 7c01 a000 6401 a101 6400 7500 7248  ..|...d...d.u.rH
-00001b10: 7c01 a000 6402 a101 6400 7500 7248 7401  |...d...d.u.rHt.
-00001b20: 6404 8301 8201 7c01 5300 2905 4e72 3f00  d.....|.S.).Nr?.
-00001b30: 0000 721d 0000 007a 1f53 6574 206f 6e6c  ..r....z.Set onl
-00001b40: 7920 6f6e 6520 6f66 2064 6561 6c49 6420  y one of dealId 
-00001b50: 6f72 2065 7069 632e 7a1a 5365 7420 6f6e  or epic.z.Set on
-00001b60: 6520 6f66 2064 6561 6c49 6420 6f72 2065  e of dealId or e
-00001b70: 7069 632e 726d 0000 0072 7000 0000 7235  pic.rm...rp...r5
-00001b80: 0000 0072 3500 0000 7236 0000 0072 7200  ...r5...r6...rr.
-00001b90: 0000 e600 0000 730a 0000 0000 031c 0108  ......s.........
-00001ba0: 011c 0108 017a 2643 6c6f 7365 506f 7369  .....z&ClosePosi
-00001bb0: 7469 6f6e 2e63 6865 636b 5f75 6e69 7175  tion.check_uniqu
-00001bc0: 655f 636f 6e73 7472 6169 6e74 7329 0172  e_constraints).r
-00001bd0: 4b00 0000 6302 0000 0000 0000 0000 0000  K...c...........
-00001be0: 0002 0000 0009 0000 0043 0000 0073 3000  .........C...s0.
-00001bf0: 0000 7c00 7c01 6a00 6401 6b02 7210 6402  ..|.|.j.d.k.r.d.
-00001c00: 6e02 6401 7c01 6a01 7c01 6a02 7c01 6a03  n.d.|.j.|.j.|.j.
-00001c10: 7c01 6a04 7c01 6a05 7c01 6a06 6403 8d07  |.j.|.j.|.j.d...
-00001c20: 5300 2904 7aad 4372 6561 7465 2061 2043  S.).z.Create a C
-00001c30: 6c6f 7365 506f 7369 7469 6f6e 2066 726f  losePosition fro
-00001c40: 6d20 6120 4372 6561 7465 506f 7369 7469  m a CreatePositi
-00001c50: 6f6e 2e0a 2020 2020 2020 2020 3a70 6172  on..        :par
-00001c60: 616d 2070 6f73 6974 696f 6e3a 2043 7265  am position: Cre
-00001c70: 6174 6550 6f73 6974 696f 6e2e 2054 6865  atePosition. The
-00001c80: 2070 6f73 6974 696f 6e20 746f 2063 6c6f   position to clo
-00001c90: 7365 2e0a 2020 2020 2020 2020 3a72 6574  se..        :ret
-00001ca0: 7572 6e3a 2043 6c6f 7365 506f 7369 7469  urn: ClosePositi
-00001cb0: 6f6e 2e20 5468 6520 706f 7369 7469 6f6e  on. The position
-00001cc0: 2074 6f20 636c 6f73 652e 0a20 2020 2020   to close..     
-00001cd0: 2020 20da 0453 454c 4cda 0342 5559 a907     ..SELL..BUY..
-00001ce0: 7241 0000 0072 5500 0000 7245 0000 0072  rA...rU...rE...r
-00001cf0: 5600 0000 721d 0000 0072 1c00 0000 7242  V...r....r....rB
-00001d00: 0000 0072 8000 0000 2902 7271 0000 0072  ...r....).rq...r
-00001d10: 4b00 0000 7235 0000 0072 3500 0000 7236  K...r5...r5...r6
-00001d20: 0000 00da 0b66 726f 6d5f 6372 6561 7465  .....from_create
-00001d30: ef00 0000 7312 0000 0000 0602 0110 0104  ....s...........
-00001d40: 0104 0104 0104 0104 0104 f97a 1943 6c6f  ...........z.Clo
-00001d50: 7365 506f 7369 7469 6f6e 2e66 726f 6d5f  sePosition.from_
-00001d60: 6372 6561 7465 291b 722c 0000 0072 2d00  create).r,...r-.
-00001d70: 0000 722e 0000 0072 0f00 0000 7230 0000  ..r....r....r0..
-00001d80: 0072 7900 0000 7209 0000 0072 7a00 0000  .ry...r....rz...
-00001d90: 725a 0000 0072 0600 0000 722f 0000 0072  rZ...r....r/...r
-00001da0: 3f00 0000 7208 0000 0072 1d00 0000 721c  ?...r....r....r.
-00001db0: 0000 0072 4200 0000 720c 0000 0072 0200  ...rB...r....r..
-00001dc0: 0000 7231 0000 0072 6900 0000 720b 0000  ..r1...ri...r...
-00001dd0: 0072 7b00 0000 7204 0000 0072 7d00 0000  .r{...r....r}...
-00001de0: 7272 0000 0072 4f00 0000 7281 0000 0072  rr...rO...r....r
-00001df0: 3500 0000 7235 0000 0072 3500 0000 7236  5...r5...r5...r6
-00001e00: 0000 0072 7c00 0000 be00 0000 7326 0000  ...r|.......s&..
-00001e10: 000a 0108 0108 0110 0108 0110 0116 0116  ................
-00001e20: 0116 0116 020c 011a 0408 0102 0112 1608  ................
-00001e30: 0102 0112 0702 0172 7c00 0000 6300 0000  .......r|...c...
-00001e40: 0000 0000 0000 0000 0000 0000 0007 0000  ................
-00001e50: 0040 0000 0073 2201 0000 6500 5a01 6400  .@...s"...e.Z.d.
-00001e60: 5a02 5500 6401 5a03 6504 6505 1900 6506  Z.U.d.Z.e.e...e.
-00001e70: 6402 3c00 6401 5a07 6504 6508 6403 6404  d.<.d.Z.e.e.d.d.
-00001e80: 8d01 1900 6506 6405 3c00 6401 5a09 6504  ....e.d.<.d.Z.e.
-00001e90: 6508 6403 6404 8d01 1900 6506 6406 3c00  e.d.d.....e.d.<.
-00001ea0: 6401 5a0a 6504 6505 1900 6506 6407 3c00  d.Z.e.e...e.d.<.
-00001eb0: 6401 5a0b 6504 6508 6403 6404 8d01 1900  d.Z.e.e.d.d.....
-00001ec0: 6506 6408 3c00 6401 5a0c 6504 6508 6403  e.d.<.d.Z.e.e.d.
-00001ed0: 6404 8d01 1900 6506 6409 3c00 650d 6405  d.....e.d.<.e.d.
-00001ee0: 6406 6408 6409 640a 640b 8d05 650e 6504  d.d.d.d.d...e.e.
-00001ef0: 650f 1900 6504 6510 1900 640c 9c02 640d  e...e.e...d...d.
-00001f00: 640e 8404 8301 8301 5a11 6512 640f 640b  d.......Z.e.d.d.
-00001f10: 8d01 650e 6513 6410 9c01 6411 6412 8404  ..e.e.d...d.d...
-00001f20: 8301 8301 5a14 6512 640f 640b 8d01 650e  ....Z.e.d.d...e.
-00001f30: 6513 6410 9c01 6413 6414 8404 8301 8301  e.d...d.d.......
-00001f40: 5a15 650e 6513 6410 9c01 6415 6416 8404  Z.e.e.d...d.d...
-00001f50: 8301 5a16 650e 6513 6410 9c01 6417 6418  ..Z.e.e.d...d.d.
-00001f60: 8404 8301 5a17 650e 6513 6410 9c01 6419  ....Z.e.e.d...d.
-00001f70: 641a 8404 8301 5a18 6401 5300 291b da0e  d.....Z.d.S.)...
-00001f80: 5570 6461 7465 506f 7369 7469 6f6e 4e72  UpdatePositionNr
-00001f90: 5400 0000 720d 0000 0072 3800 0000 7243  T...r....r8...rC
-00001fa0: 0000 0072 4600 0000 7257 0000 0072 4900  ...rF...rW...rI.
-00001fb0: 0000 725d 0000 0072 5e00 0000 725f 0000  ..r]...r^...r_..
-00001fc0: 0072 6100 0000 6303 0000 0000 0000 0000  .ra...c.........
-00001fd0: 0000 0003 0000 0002 0000 0043 0000 0073  ...........C...s
-00001fe0: 1400 0000 7c01 6400 7501 7210 7400 7c01  ....|.d.u.r.t.|.
-00001ff0: 8301 5300 6400 5300 7264 0000 0072 6500  ..S.d.S.rd...re.
-00002000: 0000 2903 7271 0000 0072 6200 0000 7268  ..).rq...rb...rh
-00002010: 0000 0072 3500 0000 7235 0000 0072 3600  ...r5...r5...r6.
-00002020: 0000 7269 0000 0008 0100 0073 0400 0000  ..ri.......s....
-00002030: 0009 0801 7a20 5570 6461 7465 506f 7369  ....z UpdatePosi
-00002040: 7469 6f6e 2e73 6572 6961 6c69 7a65 5f64  tion.serialize_d
-00002050: 6563 696d 616c 726a 0000 0072 6b00 0000  ecimalrj...rk...
-00002060: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00002070: 0003 0000 0043 0000 0073 3200 0000 7c01  .....C...s2...|.
-00002080: a000 6401 a101 7216 7c00 a001 7c01 a101  ..d...r.|...|...
-00002090: 0100 6e18 7c01 a000 6401 a101 6402 6b02  ..n.|...d...d.k.
-000020a0: 722e 7c00 a002 7c01 a101 0100 7c01 5300  r.|...|.....|.S.
-000020b0: 2903 4e72 5700 0000 4629 0372 6e00 0000  ).NrW...F).rn...
-000020c0: da1c 5f76 616c 6964 6174 655f 7472 6169  .._validate_trai
-000020d0: 6c69 6e67 5f73 746f 705f 7472 7565 da1d  ling_stop_true..
-000020e0: 5f76 616c 6964 6174 655f 7472 6169 6c69  _validate_traili
-000020f0: 6e67 5f73 746f 705f 6661 6c73 6572 7000  ng_stop_falserp.
-00002100: 0000 7235 0000 0072 3500 0000 7236 0000  ..r5...r5...r6..
-00002110: 00da 2276 616c 6964 6174 655f 7472 6169  .."validate_trai
-00002120: 6c69 6e67 5f73 746f 705f 636f 6e73 7472  ling_stop_constr
-00002130: 6169 6e74 7314 0100 0073 0a00 0000 0003  aints....s......
-00002140: 0a01 0c01 0e01 0a01 7a31 5570 6461 7465  ........z1Update
-00002150: 506f 7369 7469 6f6e 2e76 616c 6964 6174  Position.validat
-00002160: 655f 7472 6169 6c69 6e67 5f73 746f 705f  e_trailing_stop_
-00002170: 636f 6e73 7472 6169 6e74 7363 0200 0000  constraintsc....
-00002180: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00002190: 4300 0000 7318 0000 007c 01a0 0064 01a1  C...s....|...d..
-000021a0: 0172 147c 00a0 017c 01a1 0101 007c 0153  .r.|...|.....|.S
-000021b0: 0029 024e 7254 0000 0029 0272 6e00 0000  .).NrT...).rn...
-000021c0: da1e 5f76 616c 6964 6174 655f 6775 6172  .._validate_guar
-000021d0: 616e 7465 6564 5f73 746f 705f 7472 7565  anteed_stop_true
-000021e0: 7270 0000 0072 3500 0000 7235 0000 0072  rp...r5...r5...r
-000021f0: 3600 0000 da24 7661 6c69 6461 7465 5f67  6....$validate_g
-00002200: 7561 7261 6e74 6565 645f 7374 6f70 5f63  uaranteed_stop_c
-00002210: 6f6e 7374 7261 696e 7473 1d01 0000 7306  onstraints....s.
-00002220: 0000 0000 030a 010a 017a 3355 7064 6174  .........z3Updat
-00002230: 6550 6f73 6974 696f 6e2e 7661 6c69 6461  ePosition.valida
-00002240: 7465 5f67 7561 7261 6e74 6565 645f 7374  te_guaranteed_st
-00002250: 6f70 5f63 6f6e 7374 7261 696e 7473 6302  op_constraintsc.
-00002260: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00002270: 0000 0003 0000 0073 3400 0000 8800 a000  .......s4.......
-00002280: 6401 a101 7212 7401 6402 8301 8201 7402  d...r.t.d.....t.
-00002290: 8700 6601 6403 6404 8408 6405 4400 8301  ..f.d.d...d.D...
-000022a0: 8301 7230 7401 6406 8301 8201 6400 5300  ..r0t.d.....d.S.
-000022b0: 2907 4e72 5400 0000 7a3b 4966 2074 7261  ).NrT...z;If tra
-000022c0: 696c 696e 6753 746f 7020 6973 2074 7275  ilingStop is tru
-000022d0: 652c 2074 6865 6e20 6775 6172 616e 7465  e, then guarante
-000022e0: 6564 5374 6f70 206d 7573 7420 6265 2066  edStop must be f
-000022f0: 616c 7365 2e63 0100 0000 0000 0000 0000  alse.c..........
-00002300: 0000 0200 0000 0400 0000 3300 0000 731c  ..........3...s.
-00002310: 0000 007c 005d 147d 0188 00a0 007c 01a1  ...|.].}.....|..
-00002320: 0164 0075 0056 0001 0071 0264 0053 0072  .d.u.V...q.d.S.r
-00002330: 6400 0000 a901 726e 0000 00a9 02da 022e  d.....rn........
-00002340: 30da 0566 6965 6c64 726b 0000 0072 3500  0..fieldrk...r5.
-00002350: 0000 7236 0000 00da 093c 6765 6e65 7870  ..r6.....<genexp
-00002360: 723e 2a01 0000 7304 0000 0004 0202 ff7a  r>*...s........z
-00002370: 3e55 7064 6174 6550 6f73 6974 696f 6e2e  >UpdatePosition.
-00002380: 5f76 616c 6964 6174 655f 7472 6169 6c69  _validate_traili
-00002390: 6e67 5f73 746f 705f 7472 7565 2e3c 6c6f  ng_stop_true.<lo
-000023a0: 6361 6c73 3e2e 3c67 656e 6578 7072 3e29  cals>.<genexpr>)
-000023b0: 0372 4900 0000 725d 0000 0072 4600 0000  .rI...r]...rF...
-000023c0: 7a65 4966 2074 7261 696c 696e 6753 746f  zeIf trailingSto
-000023d0: 7020 6973 2074 7275 652c 2074 6865 6e20  p is true, then 
-000023e0: 7472 6169 6c69 6e67 5374 6f70 4469 7374  trailingStopDist
-000023f0: 616e 6365 2c20 7472 6169 6c69 6e67 5374  ance, trailingSt
-00002400: 6f70 496e 6372 656d 656e 742c 2061 6e64  opIncrement, and
-00002410: 2073 746f 704c 6576 656c 206d 7573 7420   stopLevel must 
-00002420: 6265 2073 6574 2e29 0372 6e00 0000 726f  be set.).rn...ro
-00002430: 0000 0072 7300 0000 7270 0000 0072 3500  ...rs...rp...r5.
-00002440: 0000 726b 0000 0072 3600 0000 7283 0000  ..rk...r6...r...
-00002450: 0024 0100 0073 1400 0000 0002 0a01 0201  .$...s..........
-00002460: 02ff 0403 0c02 02fe 0804 0201 02ff 7a2b  ..............z+
-00002470: 5570 6461 7465 506f 7369 7469 6f6e 2e5f  UpdatePosition._
-00002480: 7661 6c69 6461 7465 5f74 7261 696c 696e  validate_trailin
-00002490: 675f 7374 6f70 5f74 7275 6563 0200 0000  g_stop_truec....
-000024a0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000024b0: 0300 0000 7322 0000 0074 0087 0066 0164  ....s"...t...f.d
-000024c0: 0164 0284 0864 0344 0083 0183 0172 1e74  .d...d.D.....r.t
-000024d0: 0164 0483 0182 0164 0053 0029 054e 6301  .d.....d.S.).Nc.
-000024e0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-000024f0: 0000 0033 0000 0073 1c00 0000 7c00 5d14  ...3...s....|.].
-00002500: 7d01 8800 a000 7c01 a101 6400 7501 5600  }.....|...d.u.V.
-00002510: 0100 7102 6400 5300 7264 0000 0072 8800  ..q.d.S.rd...r..
-00002520: 0000 7289 0000 0072 6b00 0000 7235 0000  ..r....rk...r5..
-00002530: 0072 3600 0000 728c 0000 0034 0100 0073  .r6...r....4...s
-00002540: 0400 0000 0402 02ff 7a3f 5570 6461 7465  ........z?Update
-00002550: 506f 7369 7469 6f6e 2e5f 7661 6c69 6461  Position._valida
-00002560: 7465 5f74 7261 696c 696e 675f 7374 6f70  te_trailing_stop
-00002570: 5f66 616c 7365 2e3c 6c6f 6361 6c73 3e2e  _false.<locals>.
-00002580: 3c67 656e 6578 7072 3e29 0272 4900 0000  <genexpr>).rI...
-00002590: 725d 0000 007a 5849 6620 7472 6169 6c69  r]...zXIf traili
-000025a0: 6e67 5374 6f70 2069 7320 6661 6c73 652c  ngStop is false,
-000025b0: 2074 6865 6e20 444f 204e 4f54 2073 6574   then DO NOT set
-000025c0: 2074 7261 696c 696e 6753 746f 7044 6973   trailingStopDis
-000025d0: 7461 6e63 6520 6f72 2074 7261 696c 696e  tance or trailin
-000025e0: 6753 746f 7049 6e63 7265 6d65 6e74 2e29  gStopIncrement.)
-000025f0: 0272 7300 0000 726f 0000 0072 7000 0000  .rs...ro...rp...
-00002600: 7235 0000 0072 6b00 0000 7236 0000 0072  r5...rk...r6...r
-00002610: 8400 0000 3201 0000 730c 0000 0000 020c  ....2...s.......
-00002620: 0202 fe08 0402 0102 ff7a 2c55 7064 6174  .........z,Updat
-00002630: 6550 6f73 6974 696f 6e2e 5f76 616c 6964  ePosition._valid
-00002640: 6174 655f 7472 6169 6c69 6e67 5f73 746f  ate_trailing_sto
-00002650: 705f 6661 6c73 6563 0200 0000 0000 0000  p_falsec........
-00002660: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00002670: 732c 0000 007c 01a0 0064 01a1 0164 0075  s,...|...d...d.u
-00002680: 0072 1674 0164 0283 0182 017c 01a0 0064  .r.t.d.....|...d
-00002690: 03a1 0172 2874 0164 0483 0182 0164 0053  ...r(t.d.....d.S
-000026a0: 0029 054e 7246 0000 007a 3649 6620 6775  .).NrF...z6If gu
-000026b0: 6172 616e 7465 6564 5374 6f70 2069 7320  aranteedStop is 
-000026c0: 7472 7565 2c20 7468 656e 2073 746f 704c  true, then stopL
-000026d0: 6576 656c 206d 7573 7420 6265 2073 6574  evel must be set
-000026e0: 2e72 5700 0000 7a34 6775 6172 616e 7465  .rW...z4guarante
-000026f0: 6564 5374 6f70 2061 6e64 2074 7261 696c  edStop and trail
-00002700: 696e 6753 746f 7020 6361 6e6e 6f74 2062  ingStop cannot b
-00002710: 6f74 6820 6265 2074 7275 652e 726d 0000  oth be true.rm..
-00002720: 0072 7000 0000 7235 0000 0072 3500 0000  .rp...r5...r5...
-00002730: 7236 0000 0072 8600 0000 3c01 0000 7308  r6...r....<...s.
-00002740: 0000 0000 020e 0108 010a 017a 2d55 7064  ...........z-Upd
-00002750: 6174 6550 6f73 6974 696f 6e2e 5f76 616c  atePosition._val
-00002760: 6964 6174 655f 6775 6172 616e 7465 6564  idate_guaranteed
-00002770: 5f73 746f 705f 7472 7565 2919 722c 0000  _stop_true).r,..
-00002780: 0072 2d00 0000 722e 0000 0072 5400 0000  .r-...r....rT...
-00002790: 7206 0000 0072 3300 0000 7230 0000 0072  r....r3...r0...r
-000027a0: 4300 0000 7209 0000 0072 4600 0000 7257  C...r....rF...rW
-000027b0: 0000 0072 4900 0000 725d 0000 0072 0c00  ...rI...r]...r..
-000027c0: 0000 727b 0000 0072 0200 0000 7231 0000  ..r{...r....r1..
-000027d0: 0072 6900 0000 720b 0000 00da 0464 6963  .ri...r......dic
-000027e0: 7472 8500 0000 7287 0000 0072 8300 0000  tr....r....r....
-000027f0: 7284 0000 0072 8600 0000 7235 0000 0072  r....r....r5...r
-00002800: 3500 0000 7235 0000 0072 3600 0000 7282  5...r5...r6...r.
-00002810: 0000 0000 0100 0073 3600 0000 0a01 1001  .......s6.......
-00002820: 1601 1601 1001 1601 1602 0201 0201 0201  ................
-00002830: 0201 0201 02fb 0407 0201 1c04 0801 0201  ................
-00002840: 1207 0801 0201 1205 0201 100d 0201 1009  ................
-00002850: 0201 7282 0000 004e 291b da07 6465 6369  ..r....N)...deci
-00002860: 6d61 6c72 0200 0000 da06 7479 7069 6e67  malr......typing
-00002870: 7203 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
-00002880: 0600 0000 da08 7079 6461 6e74 6963 7207  ......pydanticr.
-00002890: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-000028a0: 0000 720b 0000 0072 0c00 0000 da06 6d6f  ..r....r......mo
-000028b0: 6465 6c73 720e 0000 0072 0f00 0000 7234  delsr....r....r4
-000028c0: 0000 0072 7900 0000 727a 0000 0072 1a00  ...ry...rz...r..
-000028d0: 0000 7237 0000 0072 4a00 0000 724d 0000  ..r7...rJ...rM..
-000028e0: 0072 4f00 0000 727c 0000 0072 8200 0000  .rO...r|...r....
-000028f0: 7235 0000 0072 3500 0000 7235 0000 0072  r5...r5...r5...r
-00002900: 3600 0000 da08 3c6d 6f64 756c 653e 0100  6.....<module>..
-00002910: 0000 731e 0000 000c 0118 0220 0810 0302  ..s........ ....
-00002920: 0102 ff04 0a08 0208 0310 1410 1210 0510  ................
-00002930: 0410 7110 42                             ..q.B
+000008e0: 6407 5a06 6503 6408 6402 8d01 6504 6409  d.Z.e.d.d...e.d.
+000008f0: 3c00 640a 5a07 6508 6504 640b 3c00 640a  <.d.Z.e.e.d.<.d.
+00000900: 5a09 6508 6504 640c 3c00 640d 5a0a 650b  Z.e.e.d.<.d.Z.e.
+00000910: 6504 640e 3c00 640f 5a0c 650d 6504 6410  e.d.<.d.Z.e.e.d.
+00000920: 3c00 640a 5a0e 6508 6504 6411 3c00 6412  <.d.Z.e.e.d.<.d.
+00000930: 5a0f 6510 6503 6413 6402 8d01 1900 6504  Z.e.e.d.d.....e.
+00000940: 6414 3c00 6412 5a11 6510 6512 6415 6416  d.<.d.Z.e.e.d.d.
+00000950: 8d01 1900 6504 6417 3c00 6412 5a13 6510  ....e.d.<.d.Z.e.
+00000960: 6512 6418 6416 8d01 1900 6504 6419 3c00  e.d.d.....e.d.<.
+00000970: 6412 5a14 6510 6512 6418 6416 8d01 1900  d.Z.e.e.d.d.....
+00000980: 6504 641a 3c00 6412 5a15 6510 6503 641b  e.d.<.d.Z.e.e.d.
+00000990: 6402 8d01 1900 6504 641c 3c00 6512 6418  d.....e.d.<.e.d.
+000009a0: 641d 641e 8d02 6504 641f 3c00 6412 5a16  d.d...e.d.<.d.Z.
+000009b0: 6510 6512 6418 6416 8d01 1900 6504 6420  e.e.d.d.....e.d 
+000009c0: 3c00 6412 5a17 6510 6512 6418 6416 8d01  <.d.Z.e.e.d.d...
+000009d0: 1900 6504 6421 3c00 6412 5a18 6510 6512  ..e.d!<.d.Z.e.e.
+000009e0: 6418 6416 8d01 1900 6504 6422 3c00 6519  d.d.....e.d"<.e.
+000009f0: 6417 6419 641a 641f 6420 6421 6422 6423  d.d.d.d.d d!d"d#
+00000a00: 6424 8d08 6510 651a 1900 651b 6425 9c02  d$..e.e...e.d%..
+00000a10: 6426 6427 8404 8301 5a1c 651d 6428 6424  d&d'....Z.e.d(d$
+00000a20: 8d01 651e 651f 6429 9c01 642a 642b 8404  ..e.e.d)..d*d+..
+00000a30: 8301 8301 5a20 651d 6428 6424 8d01 651e  ....Z e.d(d$..e.
+00000a40: 651f 6429 9c01 642c 642d 8404 8301 8301  e.d)..d,d-......
+00000a50: 5a21 651d 6428 6424 8d01 651e 651f 6429  Z!e.d(d$..e.e.d)
+00000a60: 9c01 642e 642f 8404 8301 8301 5a22 651d  ..d.d/......Z"e.
+00000a70: 6428 6424 8d01 651e 651f 6429 9c01 6430  d(d$..e.e.d)..d0
+00000a80: 6431 8404 8301 8301 5a23 651d 6428 6424  d1......Z#e.d(d$
+00000a90: 8d01 651e 651f 6429 9c01 6432 6433 8404  ..e.e.d)..d2d3..
+00000aa0: 8301 8301 5a24 6412 5300 2934 da0e 4372  ....Z$d.S.)4..Cr
+00000ab0: 6561 7465 506f 7369 7469 6f6e 7a0a 5e5b  eatePositionz.^[
+00000ac0: 412d 5a5d 7b33 7d24 a901 da07 7061 7474  A-Z]{3}$....patt
+00000ad0: 6572 6eda 0c63 7572 7265 6e63 7943 6f64  ern..currencyCod
+00000ae0: 6572 3a00 0000 7a15 5e5b 412d 5a61 2d7a  er:...z.^[A-Za-z
+00000af0: 302d 392e 5f5d 7b36 2c33 307d 2472 1800  0-9._]{6,30}$r..
+00000b00: 0000 da03 4446 427a 1f5e 285c 647b 327d  ....DFBz.^(\d{2}
+00000b10: 2d29 3f5b 412d 5a5d 7b33 7d2d 5c64 7b32  -)?[A-Z]{3}-\d{2
+00000b20: 7d7c 2d7c 4446 4224 7217 0000 0046 da09  }|-|DFB$r....F..
+00000b30: 666f 7263 654f 7065 6eda 0e67 7561 7261  forceOpen..guara
+00000b40: 6e74 6565 6453 746f 7072 1200 0000 da09  nteedStopr......
+00000b50: 6f72 6465 7254 7970 6572 1400 0000 da0b  orderTyper......
+00000b60: 7469 6d65 496e 466f 7263 65da 0c74 7261  timeInForce..tra
+00000b70: 696c 696e 6753 746f 704e 7a17 5e5b 412d  ilingStopNz.^[A-
+00000b80: 5a61 2d7a 302d 395f 5c2d 2e5d 7b31 2c33  Za-z0-9_\-.]{1,3
+00000b90: 307d 2472 3900 0000 e90c 0000 0072 3300  0}$r9........r3.
+00000ba0: 0000 723b 0000 0072 0d00 0000 da0d 6c69  ..r;...r......li
+00000bb0: 6d69 7444 6973 7461 6e63 6572 3c00 0000  mitDistancer<...
+00000bc0: 7a0e 5e5b 412d 5a61 2d7a 302d 395d 2b24  z.^[A-Za-z0-9]+$
+00000bd0: da07 7175 6f74 6549 6472 0100 0000 2902  ..quoteIdr....).
+00000be0: 7234 0000 00da 0267 7472 3e00 0000 da0c  r4.....gtr>.....
+00000bf0: 7374 6f70 4469 7374 616e 6365 723f 0000  stopDistancer?..
+00000c00: 00da 1574 7261 696c 696e 6753 746f 7049  ...trailingStopI
+00000c10: 6e63 7265 6d65 6e74 da05 706c 6169 6ea9  ncrement..plain.
+00000c20: 01da 046d 6f64 65a9 02da 0176 da06 7265  ...mode....v..re
+00000c30: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
+00000c40: 0003 0000 0002 0000 0043 0000 0073 1400  .........C...s..
+00000c50: 0000 7c01 6400 7501 7210 7400 7c01 8301  ..|.d.u.r.t.|...
+00000c60: 5300 6400 5300 a901 4ea9 0172 2c00 0000  S.d.S...N..r,...
+00000c70: a903 da04 7365 6c66 725a 0000 00da 055f  ....selfrZ....._
+00000c80: 696e 666f 7230 0000 0072 3000 0000 7231  infor0...r0...r1
+00000c90: 0000 00da 1173 6572 6961 6c69 7a65 5f64  .....serialize_d
+00000ca0: 6563 696d 616c 6100 0000 7304 0000 0000  ecimala...s.....
+00000cb0: 0b08 017a 2043 7265 6174 6550 6f73 6974  ...z CreatePosit
+00000cc0: 696f 6e2e 7365 7269 616c 697a 655f 6465  ion.serialize_de
+00000cd0: 6369 6d61 6cda 0662 6566 6f72 65a9 01da  cimal..before...
+00000ce0: 0464 6174 6163 0200 0000 0000 0000 0000  .datac..........
+00000cf0: 0000 0200 0000 0300 0000 4300 0000 734c  ..........C...sL
+00000d00: 0000 007c 01a0 0064 01a1 0164 0075 0172  ...|...d...d.u.r
+00000d10: 247c 01a0 0064 02a1 0164 0075 0172 2474  $|...d...d.u.r$t
+00000d20: 0164 0383 0182 017c 01a0 0064 04a1 0164  .d.....|...d...d
+00000d30: 0075 0172 487c 01a0 0064 05a1 0164 0075  .u.rH|...d...d.u
+00000d40: 0172 4874 0164 0683 0182 017c 0153 0029  .rHt.d.....|.S.)
+00000d50: 074e 723c 0000 0072 5100 0000 7a2c 5365  .Nr<...rQ...z,Se
+00000d60: 7420 6f6e 6c79 206f 6e65 206f 6620 6c69  t only one of li
+00000d70: 6d69 744c 6576 656c 206f 7220 6c69 6d69  mitLevel or limi
+00000d80: 7444 6973 7461 6e63 652e 723f 0000 0072  tDistance.r?...r
+00000d90: 5400 0000 7a2a 5365 7420 6f6e 6c79 206f  T...z*Set only o
+00000da0: 6e65 206f 6620 7374 6f70 4c65 7665 6c20  ne of stopLevel 
+00000db0: 6f72 2073 746f 7044 6973 7461 6e63 652e  or stopDistance.
+00000dc0: a902 da03 6765 74da 0a56 616c 7565 4572  ....get..ValueEr
+00000dd0: 726f 72a9 02da 0363 6c73 7264 0000 0072  ror....clsrd...r
+00000de0: 3000 0000 7230 0000 0072 3100 0000 da18  0...r0...r1.....
+00000df0: 6368 6563 6b5f 756e 6971 7565 5f63 6f6e  check_unique_con
+00000e00: 7374 7261 696e 7473 6f00 0000 730a 0000  straintso...s...
+00000e10: 0000 031c 0108 011c 0108 017a 2743 7265  ...........z'Cre
+00000e20: 6174 6550 6f73 6974 696f 6e2e 6368 6563  atePosition.chec
+00000e30: 6b5f 756e 6971 7565 5f63 6f6e 7374 7261  k_unique_constra
+00000e40: 696e 7473 6302 0000 0000 0000 0000 0000  intsc...........
+00000e50: 0002 0000 0007 0000 0043 0000 0073 4e00  .........C...sN.
+00000e60: 0000 7c01 a000 6401 a101 734a 7401 7c01  ..|...d...sJt.|.
+00000e70: a000 6402 a101 6400 7501 7c01 a000 6403  ..d...d.u.|...d.
+00000e80: a101 6400 7501 7c01 a000 6404 a101 6400  ..d.u.|...d...d.
+00000e90: 7501 7c01 a000 6405 a101 6400 7501 6704  u.|...d...d.u.g.
+00000ea0: 8301 724a 7402 6406 8301 8201 7c01 5300  ..rJt.d.....|.S.
+00000eb0: 2907 4e72 4b00 0000 7251 0000 0072 3c00  ).NrK...rQ...r<.
+00000ec0: 0000 7254 0000 0072 3f00 0000 7a3c 666f  ..rT...r?...z<fo
+00000ed0: 7263 654f 7065 6e20 6d75 7374 2062 6520  rceOpen must be 
+00000ee0: 7472 7565 2069 6620 6c69 6d69 7420 6f72  true if limit or
+00000ef0: 2073 746f 7020 636f 6e73 7472 6169 6e74   stop constraint
+00000f00: 7320 6172 6520 7365 742e 2903 7266 0000  s are set.).rf..
+00000f10: 00da 0361 6e79 7267 0000 0072 6800 0000  ...anyrg...rh...
+00000f20: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
+00000f30: 1c63 6865 636b 5f66 6f72 6365 5f6f 7065  .check_force_ope
+00000f40: 6e5f 636f 6e73 7472 6169 6e74 7378 0000  n_constraintsx..
+00000f50: 0073 1600 0000 0003 0c02 0c01 0c01 0c01  .s..............
+00000f60: 0cfc 02ff 0408 0201 02ff 0403 7a2b 4372  ............z+Cr
+00000f70: 6561 7465 506f 7369 7469 6f6e 2e63 6865  eatePosition.che
+00000f80: 636b 5f66 6f72 6365 5f6f 7065 6e5f 636f  ck_force_open_co
+00000f90: 6e73 7472 6169 6e74 7363 0200 0000 0000  nstraintsc......
+00000fa0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
+00000fb0: 0000 7332 0000 007c 01a0 0064 01a1 0172  ..s2...|...d...r
+00000fc0: 2e74 017c 01a0 0064 02a1 0183 0174 017c  .t.|...d.....t.|
+00000fd0: 01a0 0064 03a1 0183 0141 0073 2e74 0264  ...d.....A.s.t.d
+00000fe0: 0483 0182 017c 0153 0029 054e 724c 0000  .....|.S.).NrL..
+00000ff0: 0072 3f00 0000 7254 0000 007a 4e57 6865  .r?...rT...zNWhe
+00001000: 6e20 6775 6172 616e 7465 6564 5374 6f70  n guaranteedStop
+00001010: 2069 7320 7472 7565 2c20 7370 6563 6966   is true, specif
+00001020: 7920 6578 6163 746c 7920 6f6e 6520 6f66  y exactly one of
+00001030: 2073 746f 704c 6576 656c 206f 7220 7374   stopLevel or st
+00001040: 6f70 4469 7374 616e 6365 2e29 0372 6600  opDistance.).rf.
+00001050: 0000 722e 0000 0072 6700 0000 7268 0000  ..r....rg...rh..
+00001060: 0072 3000 0000 7230 0000 0072 3100 0000  .r0...r0...r1...
+00001070: da21 6368 6563 6b5f 6775 6172 616e 7465  .!check_guarante
+00001080: 6564 5f73 746f 705f 636f 6e73 7472 6169  ed_stop_constrai
+00001090: 6e74 7388 0000 0073 0e00 0000 0003 0a01  nts....s........
+000010a0: 1aff 0203 0201 02ff 0403 7a30 4372 6561  ..........z0Crea
+000010b0: 7465 506f 7369 7469 6f6e 2e63 6865 636b  tePosition.check
+000010c0: 5f67 7561 7261 6e74 6565 645f 7374 6f70  _guaranteed_stop
+000010d0: 5f63 6f6e 7374 7261 696e 7473 6302 0000  _constraintsc...
+000010e0: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+000010f0: 0043 0000 0073 a600 0000 7c01 a000 6401  .C...s....|...d.
+00001100: a101 7d02 7c02 6402 6b02 7240 7c01 a000  ..}.|.d.k.r@|...
+00001110: 6403 a101 6400 7501 7228 7401 6404 8301  d...d.u.r(t.d...
+00001120: 8201 7c01 a000 6405 a101 6400 7500 72a2  ..|...d...d.u.r.
+00001130: 7401 6406 8301 8201 6e62 7c02 6407 6b02  t.d.....nb|.d.k.
+00001140: 7272 7402 7c01 a000 6405 a101 6400 7501  rrt.|...d...d.u.
+00001150: 7c01 a000 6403 a101 6400 7501 6702 8301  |...d...d.u.g...
+00001160: 72a2 7401 6408 8301 8201 6e30 7c02 6409  r.t.d.....n0|.d.
+00001170: 6b02 72a2 7403 7c01 a000 6405 a101 6400  k.r.t.|...d...d.
+00001180: 7501 7c01 a000 6403 a101 6400 7501 6702  u.|...d...d.u.g.
+00001190: 8301 73a2 7401 640a 8301 8201 7c01 5300  ..s.t.d.....|.S.
+000011a0: 290b 4e72 4d00 0000 7211 0000 0072 5200  ).NrM...r....rR.
+000011b0: 0000 7a2b 446f 206e 6f74 2073 6574 2071  ..z+Do not set q
+000011c0: 756f 7465 4964 2077 6865 6e20 6f72 6465  uoteId when orde
+000011d0: 7254 7970 6520 6973 204c 494d 4954 2e72  rType is LIMIT.r
+000011e0: 3b00 0000 7a22 5365 7420 6c65 7665 6c20  ;...z"Set level 
+000011f0: 7768 656e 206f 7264 6572 5479 7065 2069  when orderType i
+00001200: 7320 4c49 4d49 542e 7212 0000 007a 3544  s LIMIT.r....z5D
+00001210: 6f20 6e6f 7420 7365 7420 6c65 7665 6c20  o not set level 
+00001220: 6f72 2071 756f 7465 4964 2077 6865 6e20  or quoteId when 
+00001230: 6f72 6465 7254 7970 6520 6973 204d 4152  orderType is MAR
+00001240: 4b45 542e 7213 0000 007a 3353 6574 2062  KET.r....z3Set b
+00001250: 6f74 6820 6c65 7665 6c20 616e 6420 7175  oth level and qu
+00001260: 6f74 6549 6420 7768 656e 206f 7264 6572  oteId when order
+00001270: 5479 7065 2069 7320 5155 4f54 452e 2904  Type is QUOTE.).
+00001280: 7266 0000 0072 6700 0000 726b 0000 00da  rf...rg...rk....
+00001290: 0361 6c6c 2903 7269 0000 0072 6400 0000  .all).ri...rd...
+000012a0: 5a0a 6f72 6465 725f 7479 7065 7230 0000  Z.order_typer0..
+000012b0: 0072 3000 0000 7231 0000 00da 1c63 6865  .r0...r1.....che
+000012c0: 636b 5f6f 7264 6572 5f74 7970 655f 636f  ck_order_type_co
+000012d0: 6e73 7472 6169 6e74 7393 0000 0073 2200  nstraints....s".
+000012e0: 0000 0003 0a01 0801 0e01 0801 0e01 0a01  ................
+000012f0: 0801 2001 0201 02ff 0603 0801 0201 1aff  .. .............
+00001300: 0403 0801 7a2b 4372 6561 7465 506f 7369  ....z+CreatePosi
+00001310: 7469 6f6e 2e63 6865 636b 5f6f 7264 6572  tion.check_order
+00001320: 5f74 7970 655f 636f 6e73 7472 6169 6e74  _type_constraint
+00001330: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
+00001340: 0000 0500 0000 4300 0000 735e 0000 007c  ......C...s^...|
+00001350: 01a0 0064 01a1 0172 5a7c 01a0 0064 02a1  ...d...rZ|...d..
+00001360: 0164 0075 0172 2074 0164 0383 0182 017c  .d.u.r t.d.....|
+00001370: 01a0 0064 04a1 0172 3274 0164 0583 0182  ...d...r2t.d....
+00001380: 0174 027c 01a0 0064 06a1 0164 0075 017c  .t.|...d...d.u.|
+00001390: 01a0 0064 07a1 0164 0075 0167 0283 0173  ...d...d.u.g...s
+000013a0: 5a74 0164 0883 0182 017c 0153 0029 094e  Zt.d.....|.S.).N
+000013b0: 724f 0000 0072 3f00 0000 7a2f 446f 206e  rO...r?...z/Do n
+000013c0: 6f74 2073 6574 2073 746f 704c 6576 656c  ot set stopLevel
+000013d0: 2077 6865 6e20 7472 6169 6c69 6e67 5374   when trailingSt
+000013e0: 6f70 2069 7320 7472 7565 2e72 4c00 0000  op is true.rL...
+000013f0: 7a37 6775 6172 616e 7465 6564 5374 6f70  z7guaranteedStop
+00001400: 206d 7573 7420 6265 2066 616c 7365 2077   must be false w
+00001410: 6865 6e20 7472 6169 6c69 6e67 5374 6f70  hen trailingStop
+00001420: 2069 7320 7472 7565 2e72 5400 0000 7255   is true.rT...rU
+00001430: 0000 007a 4a53 6574 2062 6f74 6820 7374  ...zJSet both st
+00001440: 6f70 4469 7374 616e 6365 2061 6e64 2074  opDistance and t
+00001450: 7261 696c 696e 6753 746f 7049 6e63 7265  railingStopIncre
+00001460: 6d65 6e74 2077 6865 6e20 7472 6169 6c69  ment when traili
+00001470: 6e67 5374 6f70 2069 7320 7472 7565 2e29  ngStop is true.)
+00001480: 0372 6600 0000 7267 0000 0072 6e00 0000  .rf...rg...rn...
+00001490: 7268 0000 0072 3000 0000 7230 0000 0072  rh...r0...r0...r
+000014a0: 3100 0000 da1f 6368 6563 6b5f 7472 6169  1.....check_trai
+000014b0: 6c69 6e67 5f73 746f 705f 636f 6e73 7472  ling_stop_constr
+000014c0: 6169 6e74 73a8 0000 0073 2000 0000 0003  aints....s .....
+000014d0: 0a01 0e01 0801 0a01 0201 02ff 0403 0202  ................
+000014e0: 0c01 0cfe 02ff 0406 0201 02ff 0403 7a2e  ..............z.
+000014f0: 4372 6561 7465 506f 7369 7469 6f6e 2e63  CreatePosition.c
+00001500: 6865 636b 5f74 7261 696c 696e 675f 7374  heck_trailing_st
+00001510: 6f70 5f63 6f6e 7374 7261 696e 7473 2925  op_constraints)%
+00001520: 7227 0000 0072 2800 0000 7229 0000 0072  r'...r(...r)...r
+00001530: 0800 0000 722b 0000 0072 0f00 0000 7217  ....r+...r....r.
+00001540: 0000 0072 4b00 0000 722e 0000 0072 4c00  ...rK...r....rL.
+00001550: 0000 724d 0000 00da 094f 7264 6572 5479  ..rM.....OrderTy
+00001560: 7065 724e 0000 00da 0b54 696d 6549 6e46  perN.....TimeInF
+00001570: 6f72 6365 724f 0000 0072 3900 0000 7206  orcerO...r9...r.
+00001580: 0000 0072 3b00 0000 7209 0000 0072 5100  ...r;...r....rQ.
+00001590: 0000 723c 0000 0072 5200 0000 7254 0000  ..r<...rR...rT..
+000015a0: 0072 3f00 0000 7255 0000 0072 0c00 0000  .r?...rU...r....
+000015b0: 7202 0000 0072 2c00 0000 7261 0000 0072  r....r,...ra...r
+000015c0: 0b00 0000 da0b 636c 6173 736d 6574 686f  ......classmetho
+000015d0: 6472 0400 0000 726a 0000 0072 6c00 0000  dr....rj...rl...
+000015e0: 726d 0000 0072 6f00 0000 7270 0000 0072  rm...ro...rp...r
+000015f0: 3000 0000 7230 0000 0072 3000 0000 7231  0...r0...r0...r1
+00001600: 0000 0072 4600 0000 4d00 0000 7358 0000  ...rF...M...sX..
+00001610: 000a 010e 0108 010e 0112 010c 010c 010c  ................
+00001620: 010c 010c 0116 0116 0116 0116 0116 0110  ................
+00001630: 0116 0116 0116 0202 0102 0102 0102 0102  ................
+00001640: 0102 0102 0102 0102 f804 0a16 0408 0102  ................
+00001650: 0112 0708 0102 0112 0e08 0102 0112 0908  ................
+00001660: 0102 0112 1308 0102 0172 4600 0000 6300  .........rF...c.
+00001670: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+00001680: 0000 0040 0000 0073 1201 0000 6500 5a01  ...@...s....e.Z.
+00001690: 6400 5a02 5500 6503 6504 6401 3c00 6505  d.Z.U.e.e.d.<.e.
+000016a0: 6504 6402 3c00 6506 6403 6404 6405 8d02  e.d.<.e.d.d.d...
+000016b0: 6504 6406 3c00 6407 5a07 6508 6504 6408  e.d.<.d.Z.e.e.d.
+000016c0: 3c00 6407 5a09 650a 650b 1900 6504 6409  <.d.Z.e.e...e.d.
+000016d0: 3c00 6407 5a0c 650a 650d 640a 640b 8d01  <.d.Z.e.e.d.d...
+000016e0: 1900 6504 640c 3c00 6407 5a0e 650a 650d  ..e.d.<.d.Z.e.e.
+000016f0: 640d 640b 8d01 1900 6504 640e 3c00 6407  d.d.....e.d.<.d.
+00001700: 5a0f 650a 650d 640f 640b 8d01 1900 6504  Z.e.e.d.d.....e.
+00001710: 6410 3c00 6407 5a10 650a 6506 6411 6412  d.<.d.Z.e.e.d.d.
+00001720: 8d01 1900 6504 6413 3c00 6511 6413 6406  ....e.d.<.e.d.d.
+00001730: 6414 6415 8d03 650a 6512 1900 650a 6513  d.d...e.e...e.e.
+00001740: 1900 6416 9c02 6417 6418 8404 8301 5a14  ..d...d.d.....Z.
+00001750: 6515 6419 6415 8d01 6516 6517 641a 9c01  e.d.d...e.e.d...
+00001760: 641b 641c 8404 8301 8301 5a18 6515 6419  d.d.......Z.e.d.
+00001770: 6415 8d01 6516 6517 641a 9c01 641d 641e  d...e.e.d...d.d.
+00001780: 8404 8301 8301 5a19 6516 651a 641f 9c01  ......Z.e.e.d...
+00001790: 6420 6421 8404 8301 5a1b 6407 5300 2922  d d!....Z.d.S.)"
+000017a0: da0d 436c 6f73 6550 6f73 6974 696f 6e72  ..ClosePositionr
+000017b0: 3a00 0000 724d 0000 0072 0100 0000 720d  :...rM...r....r.
+000017c0: 0000 0029 0272 5300 0000 7234 0000 0072  ...).rS...r4...r
+000017d0: 3e00 0000 4e72 4e00 0000 7252 0000 007a  >...NrN...rR...z
+000017e0: 072e 7b31 2c33 307d 7247 0000 0072 3800  ..{1,30}rG...r8.
+000017f0: 0000 7a13 5b41 2d5a 612d 7a30 2d39 2e5f  ..z.[A-Za-z0-9._
+00001800: 5d7b 362c 3330 7d72 1800 0000 7a1d 285c  ]{6,30}r....z.(\
+00001810: 647b 327d 2d29 3f5b 412d 5a5d 7b33 7d2d  d{2}-)?[A-Z]{3}-
+00001820: 5c64 7b32 7d7c 2d7c 4446 4272 1700 0000  \d{2}|-|DFBr....
+00001830: 7250 0000 0072 3300 0000 723b 0000 0072  rP...r3...r;...r
+00001840: 5600 0000 7257 0000 0072 5900 0000 6303  V...rW...rY...c.
+00001850: 0000 0000 0000 0000 0000 0003 0000 0002  ................
+00001860: 0000 0043 0000 0073 1400 0000 7c01 6400  ...C...s....|.d.
+00001870: 7501 7210 7400 7c01 8301 5300 6400 5300  u.r.t.|...S.d.S.
+00001880: 725c 0000 0072 5d00 0000 725e 0000 0072  r\...r]...r^...r
+00001890: 3000 0000 7230 0000 0072 3100 0000 7261  0...r0...r1...ra
+000018a0: 0000 00c9 0000 0073 0400 0000 0002 0801  .......s........
+000018b0: 7a1f 436c 6f73 6550 6f73 6974 696f 6e2e  z.ClosePosition.
+000018c0: 7365 7269 616c 697a 655f 6465 6369 6d61  serialize_decima
+000018d0: 6c72 6200 0000 7263 0000 0063 0200 0000  lrb...rc...c....
+000018e0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000018f0: 4300 0000 73b0 0000 007c 01a0 0064 01a1  C...s....|...d..
+00001900: 0164 026b 0272 327c 01a0 0064 03a1 0164  .d.k.r2|...d...d
+00001910: 0075 0073 2a7c 01a0 0064 04a1 0164 0075  .u.s*|...d...d.u
+00001920: 0072 3274 0164 0583 0182 017c 01a0 0064  .r2t.d.....|...d
+00001930: 01a1 0164 066b 0272 647c 01a0 0064 04a1  ...d.k.rd|...d..
+00001940: 0164 0075 0170 567c 01a0 0064 03a1 0164  .d.u.pV|...d...d
+00001950: 0075 0172 6474 0164 0783 0182 017c 01a0  .u.rdt.d.....|..
+00001960: 0064 01a1 0164 086b 0272 887c 01a0 0064  .d...d.k.r.|...d
+00001970: 03a1 0164 0075 0172 8874 0164 0983 0182  ...d.u.r.t.d....
+00001980: 017c 01a0 0064 01a1 0164 086b 0272 ac7c  .|...d...d.k.r.|
+00001990: 01a0 0064 04a1 0164 0075 0072 ac74 0164  ...d...d.u.r.t.d
+000019a0: 0a83 0182 017c 0153 0029 0b4e 724d 0000  .....|.S.).NrM..
+000019b0: 0072 1300 0000 7252 0000 0072 3b00 0000  .r....rR...r;...
+000019c0: 7a2c 7175 6f74 6549 6420 6973 2072 6571  z,quoteId is req
+000019d0: 7569 7265 6420 7768 656e 206f 7264 6572  uired when order
+000019e0: 5479 7065 2069 7320 5155 4f54 452e 7212  Type is QUOTE.r.
+000019f0: 0000 007a 3b6c 6576 656c 2061 6e64 2071  ...z;level and q
+00001a00: 756f 7465 4964 2061 7265 206e 6f74 2061  uoteId are not a
+00001a10: 6c6c 6f77 6564 2077 6865 6e20 6f72 6465  llowed when orde
+00001a20: 7254 7970 6520 6973 204d 4152 4b45 542e  rType is MARKET.
+00001a30: 7211 0000 007a 2f71 756f 7465 4964 2069  r....z/quoteId i
+00001a40: 7320 6e6f 7420 616c 6c6f 7765 6420 7768  s not allowed wh
+00001a50: 656e 206f 7264 6572 5479 7065 2069 7320  en orderType is 
+00001a60: 4c49 4d49 542e 7a2a 6c65 7665 6c20 6973  LIMIT.z*level is
+00001a70: 2072 6571 7569 7265 6420 7768 656e 206f   required when o
+00001a80: 7264 6572 5479 7065 2069 7320 4c49 4d49  rderType is LIMI
+00001a90: 542e 7265 0000 0072 6800 0000 7230 0000  T.re...rh...r0..
+00001aa0: 0072 3000 0000 7231 0000 00da 1063 6865  .r0...r1.....che
+00001ab0: 636b 5f6f 7264 6572 5f74 7970 65ce 0000  ck_order_type...
+00001ac0: 0073 2400 0000 0003 0e01 0cff 0201 0cff  .s$.............
+00001ad0: 0203 0803 0cff 0202 1afe 0204 0201 02ff  ................
+00001ae0: 0404 1c01 0802 1c01 0802 7a1e 436c 6f73  ..........z.Clos
+00001af0: 6550 6f73 6974 696f 6e2e 6368 6563 6b5f  ePosition.check_
+00001b00: 6f72 6465 725f 7479 7065 6302 0000 0000  order_typec.....
+00001b10: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00001b20: 0000 0073 4c00 0000 7c01 a000 6401 a101  ...sL...|...d...
+00001b30: 6400 7501 7224 7c01 a000 6402 a101 6400  d.u.r$|...d...d.
+00001b40: 7501 7224 7401 6403 8301 8201 7c01 a000  u.r$t.d.....|...
+00001b50: 6401 a101 6400 7500 7248 7c01 a000 6402  d...d.u.rH|...d.
+00001b60: a101 6400 7500 7248 7401 6404 8301 8201  ..d.u.rHt.d.....
+00001b70: 7c01 5300 2905 4e72 3800 0000 7218 0000  |.S.).Nr8...r...
+00001b80: 007a 1f53 6574 206f 6e6c 7920 6f6e 6520  .z.Set only one 
+00001b90: 6f66 2064 6561 6c49 6420 6f72 2065 7069  of dealId or epi
+00001ba0: 632e 7a1a 5365 7420 6f6e 6520 6f66 2064  c.z.Set one of d
+00001bb0: 6561 6c49 6420 6f72 2065 7069 632e 7265  ealId or epic.re
+00001bc0: 0000 0072 6800 0000 7230 0000 0072 3000  ...rh...r0...r0.
+00001bd0: 0000 7231 0000 0072 6a00 0000 e600 0000  ..r1...rj.......
+00001be0: 730a 0000 0000 031c 0108 011c 0108 017a  s..............z
+00001bf0: 2643 6c6f 7365 506f 7369 7469 6f6e 2e63  &ClosePosition.c
+00001c00: 6865 636b 5f75 6e69 7175 655f 636f 6e73  heck_unique_cons
+00001c10: 7472 6169 6e74 7329 0172 4400 0000 6302  traints).rD...c.
+00001c20: 0000 0000 0000 0000 0000 0002 0000 0009  ................
+00001c30: 0000 0043 0000 0073 3000 0000 7c00 7c01  ...C...s0...|.|.
+00001c40: 6a00 6401 6b02 7210 6402 6e02 6401 7c01  j.d.k.r.d.n.d.|.
+00001c50: 6a01 7c01 6a02 7c01 6a03 7c01 6a04 7c01  j.|.j.|.j.|.j.|.
+00001c60: 6a05 7c01 6a06 6403 8d07 5300 2904 7aad  j.|.j.d...S.).z.
+00001c70: 4372 6561 7465 2061 2043 6c6f 7365 506f  Create a ClosePo
+00001c80: 7369 7469 6f6e 2066 726f 6d20 6120 4372  sition from a Cr
+00001c90: 6561 7465 506f 7369 7469 6f6e 2e0a 2020  eatePosition..  
+00001ca0: 2020 2020 2020 3a70 6172 616d 2070 6f73        :param pos
+00001cb0: 6974 696f 6e3a 2043 7265 6174 6550 6f73  ition: CreatePos
+00001cc0: 6974 696f 6e2e 2054 6865 2070 6f73 6974  ition. The posit
+00001cd0: 696f 6e20 746f 2063 6c6f 7365 2e0a 2020  ion to close..  
+00001ce0: 2020 2020 2020 3a72 6574 7572 6e3a 2043        :return: C
+00001cf0: 6c6f 7365 506f 7369 7469 6f6e 2e20 5468  losePosition. Th
+00001d00: 6520 706f 7369 7469 6f6e 2074 6f20 636c  e position to cl
+00001d10: 6f73 652e 0a20 2020 2020 2020 20da 0453  ose..        ..S
+00001d20: 454c 4c5a 0342 5559 a907 723a 0000 0072  ELLZ.BUY..r:...r
+00001d30: 4d00 0000 723e 0000 0072 4e00 0000 7218  M...r>...rN...r.
+00001d40: 0000 0072 1700 0000 723b 0000 0072 7700  ...r....r;...rw.
+00001d50: 0000 2902 7269 0000 0072 4400 0000 7230  ..).ri...rD...r0
+00001d60: 0000 0072 3000 0000 7231 0000 00da 0b66  ...r0...r1.....f
+00001d70: 726f 6d5f 6372 6561 7465 ef00 0000 7312  rom_create....s.
+00001d80: 0000 0000 0602 0110 0104 0104 0104 0104  ................
+00001d90: 0104 0104 f97a 1943 6c6f 7365 506f 7369  .....z.ClosePosi
+00001da0: 7469 6f6e 2e66 726f 6d5f 6372 6561 7465  tion.from_create
+00001db0: 291c 7227 0000 0072 2800 0000 7229 0000  ).r'...r(...r)..
+00001dc0: 0072 0f00 0000 722b 0000 0072 7100 0000  .r....r+...rq...
+00001dd0: 7209 0000 0072 4e00 0000 7272 0000 0072  r....rN...rr...r
+00001de0: 5200 0000 7206 0000 0072 2a00 0000 7238  R...r....r*...r8
+00001df0: 0000 0072 0800 0000 7218 0000 0072 1700  ...r....r....r..
+00001e00: 0000 723b 0000 0072 0c00 0000 7202 0000  ..r;...r....r...
+00001e10: 0072 2c00 0000 7261 0000 0072 0b00 0000  .r,...ra...r....
+00001e20: 7273 0000 0072 0400 0000 7275 0000 0072  rs...r....ru...r
+00001e30: 6a00 0000 7246 0000 0072 7800 0000 7230  j...rF...rx...r0
+00001e40: 0000 0072 3000 0000 7230 0000 0072 3100  ...r0...r0...r1.
+00001e50: 0000 7274 0000 00be 0000 0073 2600 0000  ..rt.......s&...
+00001e60: 0a01 0801 0801 1001 0c01 1001 1601 1601  ................
+00001e70: 1601 1602 0c01 1a04 0801 0201 1216 0801  ................
+00001e80: 0201 1207 0201 7274 0000 0063 0000 0000  ......rt...c....
+00001e90: 0000 0000 0000 0000 0000 0000 0700 0000  ................
+00001ea0: 4000 0000 7322 0100 0065 005a 0164 005a  @...s"...e.Z.d.Z
+00001eb0: 0255 0064 015a 0365 0465 0519 0065 0664  .U.d.Z.e.e...e.d
+00001ec0: 023c 0064 015a 0765 0465 0864 0364 048d  .<.d.Z.e.e.d.d..
+00001ed0: 0119 0065 0664 053c 0064 015a 0965 0465  ...e.d.<.d.Z.e.e
+00001ee0: 0864 0364 048d 0119 0065 0664 063c 0064  .d.d.....e.d.<.d
+00001ef0: 015a 0a65 0465 0519 0065 0664 073c 0064  .Z.e.e...e.d.<.d
+00001f00: 015a 0b65 0465 0864 0364 048d 0119 0065  .Z.e.e.d.d.....e
+00001f10: 0664 083c 0064 015a 0c65 0465 0864 0364  .d.<.d.Z.e.e.d.d
+00001f20: 048d 0119 0065 0664 093c 0065 0d64 0564  .....e.d.<.e.d.d
+00001f30: 0664 0864 0964 0a64 0b8d 0565 0e65 0465  .d.d.d.d...e.e.e
+00001f40: 0f19 0065 0465 1019 0064 0c9c 0264 0d64  ...e.e...d...d.d
+00001f50: 0e84 0483 0183 015a 1165 1264 0f64 0b8d  .......Z.e.d.d..
+00001f60: 0165 0e65 1364 109c 0164 1164 1284 0483  .e.e.d...d.d....
+00001f70: 0183 015a 1465 1264 0f64 0b8d 0165 0e65  ...Z.e.d.d...e.e
+00001f80: 1364 109c 0164 1364 1484 0483 0183 015a  .d...d.d.......Z
+00001f90: 1565 0e65 1364 109c 0164 1564 1684 0483  .e.e.d...d.d....
+00001fa0: 015a 1665 0e65 1364 109c 0164 1764 1884  .Z.e.e.d...d.d..
+00001fb0: 0483 015a 1765 0e65 1364 109c 0164 1964  ...Z.e.e.d...d.d
+00001fc0: 1a84 0483 015a 1864 0153 0029 1bda 0e55  .....Z.d.S.)...U
+00001fd0: 7064 6174 6550 6f73 6974 696f 6e4e 724c  pdatePositionNrL
+00001fe0: 0000 0072 0d00 0000 7233 0000 0072 3c00  ...r....r3...r<.
+00001ff0: 0000 723f 0000 0072 4f00 0000 7242 0000  ..r?...rO...rB..
+00002000: 0072 5500 0000 7256 0000 0072 5700 0000  .rU...rV...rW...
+00002010: 7259 0000 0063 0300 0000 0000 0000 0000  rY...c..........
+00002020: 0000 0300 0000 0200 0000 4300 0000 7314  ..........C...s.
+00002030: 0000 007c 0164 0075 0172 1074 007c 0183  ...|.d.u.r.t.|..
+00002040: 0153 0064 0053 0072 5c00 0000 725d 0000  .S.d.S.r\...r]..
+00002050: 0029 0372 6900 0000 725a 0000 0072 6000  .).ri...rZ...r`.
+00002060: 0000 7230 0000 0072 3000 0000 7231 0000  ..r0...r0...r1..
+00002070: 0072 6100 0000 0801 0000 7304 0000 0000  .ra.......s.....
+00002080: 0908 017a 2055 7064 6174 6550 6f73 6974  ...z UpdatePosit
+00002090: 696f 6e2e 7365 7269 616c 697a 655f 6465  ion.serialize_de
+000020a0: 6369 6d61 6c72 6200 0000 7263 0000 0063  cimalrb...rc...c
+000020b0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000020c0: 0300 0000 4300 0000 7332 0000 007c 01a0  ....C...s2...|..
+000020d0: 0064 01a1 0172 167c 00a0 017c 01a1 0101  .d...r.|...|....
+000020e0: 006e 187c 01a0 0064 01a1 0164 026b 0272  .n.|...d...d.k.r
+000020f0: 2e7c 00a0 027c 01a1 0101 007c 0153 0029  .|...|.....|.S.)
+00002100: 034e 724f 0000 0046 2903 7266 0000 00da  .NrO...F).rf....
+00002110: 1c5f 7661 6c69 6461 7465 5f74 7261 696c  ._validate_trail
+00002120: 696e 675f 7374 6f70 5f74 7275 65da 1d5f  ing_stop_true.._
+00002130: 7661 6c69 6461 7465 5f74 7261 696c 696e  validate_trailin
+00002140: 675f 7374 6f70 5f66 616c 7365 7268 0000  g_stop_falserh..
+00002150: 0072 3000 0000 7230 0000 0072 3100 0000  .r0...r0...r1...
+00002160: da22 7661 6c69 6461 7465 5f74 7261 696c  ."validate_trail
+00002170: 696e 675f 7374 6f70 5f63 6f6e 7374 7261  ing_stop_constra
+00002180: 696e 7473 1401 0000 730a 0000 0000 030a  ints....s.......
+00002190: 010c 010e 010a 017a 3155 7064 6174 6550  .......z1UpdateP
+000021a0: 6f73 6974 696f 6e2e 7661 6c69 6461 7465  osition.validate
+000021b0: 5f74 7261 696c 696e 675f 7374 6f70 5f63  _trailing_stop_c
+000021c0: 6f6e 7374 7261 696e 7473 6302 0000 0000  onstraintsc.....
+000021d0: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+000021e0: 0000 0073 1800 0000 7c01 a000 6401 a101  ...s....|...d...
+000021f0: 7214 7c00 a001 7c01 a101 0100 7c01 5300  r.|...|.....|.S.
+00002200: 2902 4e72 4c00 0000 2902 7266 0000 00da  ).NrL...).rf....
+00002210: 1e5f 7661 6c69 6461 7465 5f67 7561 7261  ._validate_guara
+00002220: 6e74 6565 645f 7374 6f70 5f74 7275 6572  nteed_stop_truer
+00002230: 6800 0000 7230 0000 0072 3000 0000 7231  h...r0...r0...r1
+00002240: 0000 00da 2476 616c 6964 6174 655f 6775  ....$validate_gu
+00002250: 6172 616e 7465 6564 5f73 746f 705f 636f  aranteed_stop_co
+00002260: 6e73 7472 6169 6e74 731d 0100 0073 0600  nstraints....s..
+00002270: 0000 0003 0a01 0a01 7a33 5570 6461 7465  ........z3Update
+00002280: 506f 7369 7469 6f6e 2e76 616c 6964 6174  Position.validat
+00002290: 655f 6775 6172 616e 7465 6564 5f73 746f  e_guaranteed_sto
+000022a0: 705f 636f 6e73 7472 6169 6e74 7363 0200  p_constraintsc..
+000022b0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000022c0: 0000 0300 0000 7334 0000 0088 00a0 0064  ......s4.......d
+000022d0: 01a1 0172 1274 0164 0283 0182 0174 0287  ...r.t.d.....t..
+000022e0: 0066 0164 0364 0484 0864 0544 0083 0183  .f.d.d...d.D....
+000022f0: 0172 3074 0164 0683 0182 0164 0053 0029  .r0t.d.....d.S.)
+00002300: 074e 724c 0000 007a 3b49 6620 7472 6169  .NrL...z;If trai
+00002310: 6c69 6e67 5374 6f70 2069 7320 7472 7565  lingStop is true
+00002320: 2c20 7468 656e 2067 7561 7261 6e74 6565  , then guarantee
+00002330: 6453 746f 7020 6d75 7374 2062 6520 6661  dStop must be fa
+00002340: 6c73 652e 6301 0000 0000 0000 0000 0000  lse.c...........
+00002350: 0002 0000 0004 0000 0033 0000 0073 1c00  .........3...s..
+00002360: 0000 7c00 5d14 7d01 8800 a000 7c01 a101  ..|.].}.....|...
+00002370: 6400 7500 5600 0100 7102 6400 5300 725c  d.u.V...q.d.S.r\
+00002380: 0000 00a9 0172 6600 0000 a902 da02 2e30  .....rf........0
+00002390: da05 6669 656c 6472 6300 0000 7230 0000  ..fieldrc...r0..
+000023a0: 0072 3100 0000 da09 3c67 656e 6578 7072  .r1.....<genexpr
+000023b0: 3e2a 0100 0073 0400 0000 0402 02ff 7a3e  >*...s........z>
+000023c0: 5570 6461 7465 506f 7369 7469 6f6e 2e5f  UpdatePosition._
+000023d0: 7661 6c69 6461 7465 5f74 7261 696c 696e  validate_trailin
+000023e0: 675f 7374 6f70 5f74 7275 652e 3c6c 6f63  g_stop_true.<loc
+000023f0: 616c 733e 2e3c 6765 6e65 7870 723e 2903  als>.<genexpr>).
+00002400: 7242 0000 0072 5500 0000 723f 0000 007a  rB...rU...r?...z
+00002410: 6549 6620 7472 6169 6c69 6e67 5374 6f70  eIf trailingStop
+00002420: 2069 7320 7472 7565 2c20 7468 656e 2074   is true, then t
+00002430: 7261 696c 696e 6753 746f 7044 6973 7461  railingStopDista
+00002440: 6e63 652c 2074 7261 696c 696e 6753 746f  nce, trailingSto
+00002450: 7049 6e63 7265 6d65 6e74 2c20 616e 6420  pIncrement, and 
+00002460: 7374 6f70 4c65 7665 6c20 6d75 7374 2062  stopLevel must b
+00002470: 6520 7365 742e 2903 7266 0000 0072 6700  e set.).rf...rg.
+00002480: 0000 726b 0000 0072 6800 0000 7230 0000  ..rk...rh...r0..
+00002490: 0072 6300 0000 7231 0000 0072 7a00 0000  .rc...r1...rz...
+000024a0: 2401 0000 7314 0000 0000 020a 0102 0102  $...s...........
+000024b0: ff04 030c 0202 fe08 0402 0102 ff7a 2b55  .............z+U
+000024c0: 7064 6174 6550 6f73 6974 696f 6e2e 5f76  pdatePosition._v
+000024d0: 616c 6964 6174 655f 7472 6169 6c69 6e67  alidate_trailing
+000024e0: 5f73 746f 705f 7472 7565 6302 0000 0000  _stop_truec.....
+000024f0: 0000 0000 0000 0002 0000 0004 0000 0003  ................
+00002500: 0000 0073 2200 0000 7400 8700 6601 6401  ...s"...t...f.d.
+00002510: 6402 8408 6403 4400 8301 8301 721e 7401  d...d.D.....r.t.
+00002520: 6404 8301 8201 6400 5300 2905 4e63 0100  d.....d.S.).Nc..
+00002530: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00002540: 0000 3300 0000 731c 0000 007c 005d 147d  ..3...s....|.].}
+00002550: 0188 00a0 007c 01a1 0164 0075 0156 0001  .....|...d.u.V..
+00002560: 0071 0264 0053 0072 5c00 0000 727f 0000  .q.d.S.r\...r...
+00002570: 0072 8000 0000 7263 0000 0072 3000 0000  .r....rc...r0...
+00002580: 7231 0000 0072 8300 0000 3401 0000 7304  r1...r....4...s.
+00002590: 0000 0004 0202 ff7a 3f55 7064 6174 6550  .......z?UpdateP
+000025a0: 6f73 6974 696f 6e2e 5f76 616c 6964 6174  osition._validat
+000025b0: 655f 7472 6169 6c69 6e67 5f73 746f 705f  e_trailing_stop_
+000025c0: 6661 6c73 652e 3c6c 6f63 616c 733e 2e3c  false.<locals>.<
+000025d0: 6765 6e65 7870 723e 2902 7242 0000 0072  genexpr>).rB...r
+000025e0: 5500 0000 7a58 4966 2074 7261 696c 696e  U...zXIf trailin
+000025f0: 6753 746f 7020 6973 2066 616c 7365 2c20  gStop is false, 
+00002600: 7468 656e 2044 4f20 4e4f 5420 7365 7420  then DO NOT set 
+00002610: 7472 6169 6c69 6e67 5374 6f70 4469 7374  trailingStopDist
+00002620: 616e 6365 206f 7220 7472 6169 6c69 6e67  ance or trailing
+00002630: 5374 6f70 496e 6372 656d 656e 742e 2902  StopIncrement.).
+00002640: 726b 0000 0072 6700 0000 7268 0000 0072  rk...rg...rh...r
+00002650: 3000 0000 7263 0000 0072 3100 0000 727b  0...rc...r1...r{
+00002660: 0000 0032 0100 0073 0c00 0000 0002 0c02  ...2...s........
+00002670: 02fe 0804 0201 02ff 7a2c 5570 6461 7465  ........z,Update
+00002680: 506f 7369 7469 6f6e 2e5f 7661 6c69 6461  Position._valida
+00002690: 7465 5f74 7261 696c 696e 675f 7374 6f70  te_trailing_stop
+000026a0: 5f66 616c 7365 6302 0000 0000 0000 0000  _falsec.........
+000026b0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+000026c0: 2c00 0000 7c01 a000 6401 a101 6400 7500  ,...|...d...d.u.
+000026d0: 7216 7401 6402 8301 8201 7c01 a000 6403  r.t.d.....|...d.
+000026e0: a101 7228 7401 6404 8301 8201 6400 5300  ..r(t.d.....d.S.
+000026f0: 2905 4e72 3f00 0000 7a36 4966 2067 7561  ).Nr?...z6If gua
+00002700: 7261 6e74 6565 6453 746f 7020 6973 2074  ranteedStop is t
+00002710: 7275 652c 2074 6865 6e20 7374 6f70 4c65  rue, then stopLe
+00002720: 7665 6c20 6d75 7374 2062 6520 7365 742e  vel must be set.
+00002730: 724f 0000 007a 3467 7561 7261 6e74 6565  rO...z4guarantee
+00002740: 6453 746f 7020 616e 6420 7472 6169 6c69  dStop and traili
+00002750: 6e67 5374 6f70 2063 616e 6e6f 7420 626f  ngStop cannot bo
+00002760: 7468 2062 6520 7472 7565 2e72 6500 0000  th be true.re...
+00002770: 7268 0000 0072 3000 0000 7230 0000 0072  rh...r0...r0...r
+00002780: 3100 0000 727d 0000 003c 0100 0073 0800  1...r}...<...s..
+00002790: 0000 0002 0e01 0801 0a01 7a2d 5570 6461  ..........z-Upda
+000027a0: 7465 506f 7369 7469 6f6e 2e5f 7661 6c69  tePosition._vali
+000027b0: 6461 7465 5f67 7561 7261 6e74 6565 645f  date_guaranteed_
+000027c0: 7374 6f70 5f74 7275 6529 1972 2700 0000  stop_true).r'...
+000027d0: 7228 0000 0072 2900 0000 724c 0000 0072  r(...r)...rL...r
+000027e0: 0600 0000 722e 0000 0072 2b00 0000 723c  ....r....r+...r<
+000027f0: 0000 0072 0900 0000 723f 0000 0072 4f00  ...r....r?...rO.
+00002800: 0000 7242 0000 0072 5500 0000 720c 0000  ..rB...rU...r...
+00002810: 0072 7300 0000 7202 0000 0072 2c00 0000  .rs...r....r,...
+00002820: 7261 0000 0072 0b00 0000 da04 6469 6374  ra...r......dict
+00002830: 727c 0000 0072 7e00 0000 727a 0000 0072  r|...r~...rz...r
+00002840: 7b00 0000 727d 0000 0072 3000 0000 7230  {...r}...r0...r0
+00002850: 0000 0072 3000 0000 7231 0000 0072 7900  ...r0...r1...ry.
+00002860: 0000 0001 0000 7336 0000 000a 0110 0116  ......s6........
+00002870: 0116 0110 0116 0116 0202 0102 0102 0102  ................
+00002880: 0102 0102 fb04 0702 011c 0408 0102 0112  ................
+00002890: 0708 0102 0112 0502 0110 0d02 0110 0902  ................
+000028a0: 0172 7900 0000 4e29 1bda 0764 6563 696d  .ry...N)...decim
+000028b0: 616c 7202 0000 00da 0674 7970 696e 6772  alr......typingr
+000028c0: 0300 0000 7204 0000 0072 0500 0000 7206  ....r....r....r.
+000028d0: 0000 00da 0870 7964 616e 7469 6372 0700  .....pydanticr..
+000028e0: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
+000028f0: 0072 0b00 0000 720c 0000 00da 066d 6f64  .r....r......mod
+00002900: 656c 7372 0e00 0000 720f 0000 0072 2f00  elsr....r....r/.
+00002910: 0000 7271 0000 0072 7200 0000 7215 0000  ..rq...rr...r...
+00002920: 0072 3200 0000 7243 0000 0072 4500 0000  .r2...rC...rE...
+00002930: 7246 0000 0072 7400 0000 7279 0000 0072  rF...rt...ry...r
+00002940: 3000 0000 7230 0000 0072 3000 0000 7231  0...r0...r0...r1
+00002950: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00002960: 0073 1e00 0000 0c01 1802 2008 1003 0201  .s........ .....
+00002970: 02ff 040a 0802 0803 1014 1012 1005 1004  ................
+00002980: 1071 1042                                .q.B
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/service.cpython-39.pyc` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/__pycache__/service.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  7 21:42:19 2024 UTC, .py size: 5901 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3b13 1366 0d17 0000  a.......;..f....
+00000000: 610d 0d0a 0000 0000 9b30 3d66 9917 0000  a........0=f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6406 6407 6c06 6d0c 5a0c 0100 6500  ..d.d.l.m.Z...e.
@@ -26,29 +26,29 @@
 00000190: 7272 6f72 7320 696e 2074 6865 2070 6f73  rrors in the pos
 000001a0: 6974 696f 6e73 2070 726f 6365 7373 2e4e  itions process.N
 000001b0: 2904 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000001c0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 000001d0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5fa9  name__..__doc__.
 000001e0: 0072 1100 0000 7211 0000 00fa 5b2f 686f  .r....r.....[/ho
 000001f0: 6d65 2f72 756e 6e65 722f 776f 726b 2f69  me/runner/work/i
-00000200: 675f 7472 6164 696e 675f 6c69 622f 6967  g_trading_lib/ig
-00000210: 5f74 7261 6469 6e67 5f6c 6962 2f69 675f  _trading_lib/ig_
+00000200: 672d 7472 6164 696e 672d 6c69 622f 6967  g-trading-lib/ig
+00000210: 2d74 7261 6469 6e67 2d6c 6962 2f69 675f  -trading-lib/ig_
 00000220: 7472 6164 696e 675f 6c69 622f 7472 6164  trading_lib/trad
 00000230: 696e 672f 706f 7369 7469 6f6e 732f 7365  ing/positions/se
 00000240: 7276 6963 652e 7079 720c 0000 0014 0000  rvice.pyr.......
 00000250: 0073 0200 0000 0801 720c 0000 0063 0000  .s......r....c..
 00000260: 0000 0000 0000 0000 0000 0000 0000 0400  ................
 00000270: 0000 4000 0000 7380 0000 0065 005a 0164  ..@...s....e.Z.d
 00000280: 005a 0265 0365 0465 0364 019c 0364 0264  .Z.e.e.e.d...d.d
 00000290: 0384 045a 0565 0665 0764 049c 0164 0564  ...Z.e.e.d...d.d
 000002a0: 0684 0483 015a 0865 0365 0964 079c 0264  .....Z.e.e.d...d
 000002b0: 0864 0984 045a 0a65 0b64 049c 0164 0a64  .d...Z.e.d...d.d
 000002c0: 0b84 045a 0c65 0d65 0e64 0c9c 0264 0d64  ...Z.e.e.d...d.d
-000002d0: 0e84 045a 0f65 1065 0e64 0f9c 0264 1064  ...Z.e.e.d...d.d
-000002e0: 1184 045a 1165 0365 1265 0e64 129c 0364  ...Z.e.e.e.d...d
+000002d0: 0e84 045a 0f65 0365 1065 0e64 0f9c 0364  ...Z.e.e.e.d...d
+000002e0: 1064 1184 045a 1165 1265 0e64 129c 0264  .d...Z.e.e.d...d
 000002f0: 1364 1484 045a 1364 1553 0029 16da 0f50  .d...Z.d.S.)...P
 00000300: 6f73 6974 696f 6e53 6572 7669 6365 a903  ositionService..
 00000310: da07 6170 695f 6b65 79da 0674 6f6b 656e  ..api_key..token
 00000320: 73da 0862 6173 655f 7572 6c63 0400 0000  s..base_urlc....
 00000330: 0000 0000 0000 0000 0400 0000 0200 0000  ................
 00000340: 4300 0000 7316 0000 007c 017c 005f 007c  C...s....|.|._.|
 00000350: 027c 005f 017c 037c 005f 0264 0153 0029  .|._.|.|._.d.S.)
@@ -219,130 +219,140 @@
 00000da0: 616c 2f70 6f73 6974 696f 6e73 2f6f 7463  al/positions/otc
 00000db0: a902 7221 0000 0072 2900 0000 7224 0000  ..r!...r)...r$..
 00000dc0: 007a 3643 7265 6174 6520 706f 7369 7469  .z6Create positi
 00000dd0: 6f6e 2072 6571 7565 7374 2066 6169 6c65  on request faile
 00000de0: 6420 7769 7468 2073 7461 7475 7320 636f  d with status co
 00000df0: 6465 2025 733a 2025 737a 2243 7265 6174  de %s: %sz"Creat
 00000e00: 6520 706f 7369 7469 6f6e 2072 6571 7565  e position reque
-00000e10: 7374 2066 6169 6c65 643a 2025 734e a90c  st failed: %sN..
+00000e10: 7374 2066 6169 6c65 643a 2025 734e 290c  st failed: %sN).
 00000e20: 7217 0000 0072 2500 0000 da04 706f 7374  r....r%.....post
 00000e30: 7221 0000 00da 0a6d 6f64 656c 5f64 756d  r!.....model_dum
 00000e40: 7072 2700 0000 720b 0000 0072 2800 0000  pr'...r....r(...
 00000e50: 7229 0000 0072 0c00 0000 722a 0000 0072  r)...r....r*...r
 00000e60: 2b00 0000 2905 7218 0000 0072 3100 0000  +...).r....r1...
 00000e70: 722c 0000 0072 2d00 0000 722e 0000 0072  r,...r-...r....r
 00000e80: 1100 0000 7211 0000 0072 1200 0000 da0f  ....r....r......
 00000e90: 6372 6561 7465 5f70 6f73 6974 696f 6e55  create_positionU
 00000ea0: 0000 0073 1c00 0000 0006 0c01 0201 0401  ...s............
 00000eb0: 0cff 0603 0a01 1002 0201 0201 0aff 02ff  ................
 00000ec0: 0804 1001 7a1f 506f 7369 7469 6f6e 5365  ....z.PositionSe
 00000ed0: 7276 6963 652e 6372 6561 7465 5f70 6f73  rvice.create_pos
-00000ee0: 6974 696f 6e29 02da 0563 6c6f 7365 721a  ition)...closer.
-00000ef0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00000f00: 0500 0000 0a00 0000 4300 0000 738c 0000  ........C...s...
-00000f10: 007c 006a 009b 0064 019d 027d 027a 4874  .|.j...d...}.zHt
-00000f20: 016a 027c 027c 006a 037c 01a0 04a1 0064  .j.|.|.j.|.....d
-00000f30: 028d 037d 037c 036a 0564 036b 0272 3e74  ...}.|.j.d.k.r>t
-00000f40: 06a0 077c 03a0 08a1 00a1 0157 0053 0074  ...|.......W.S.t
-00000f50: 0964 047c 036a 057c 036a 0a66 0216 0083  .d.|.j.|.j.f....
-00000f60: 0182 0157 006e 3204 0074 016a 0b79 8601  ...W.n2..t.j.y..
-00000f70: 007d 0401 007a 1874 0964 057c 0416 0083  .}...z.t.d.|....
-00000f80: 0182 0157 0059 0064 067d 047e 046e 0a64  ...W.Y.d.}.~.n.d
-00000f90: 067d 047e 0430 0030 0064 0653 0029 077a  .}.~.0.0.d.S.).z
-00000fa0: bd43 6c6f 7365 2061 2070 6f73 6974 696f  .Close a positio
-00000fb0: 6e20 666f 7220 7468 6520 6175 7468 656e  n for the authen
-00000fc0: 7469 6361 7465 6420 6163 636f 756e 742e  ticated account.
-00000fd0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000fe0: 636c 6f73 653a 2043 6c6f 7365 506f 7369  close: ClosePosi
-00000ff0: 7469 6f6e 2e20 5468 6520 706f 7369 7469  tion. The positi
-00001000: 6f6e 2074 6f20 636c 6f73 652e 0a20 2020  on to close..   
-00001010: 2020 2020 203a 7265 7475 726e 3a20 4465       :return: De
-00001020: 616c 5265 6665 7265 6e63 6520 652e 673a  alReference e.g:
-00001030: 207b 2764 6561 6c52 6566 6572 656e 6365   {'dealReference
-00001040: 273a 2027 4449 4141 4141 4242 4243 4343  ': 'DIAAAABBBCCC
-00001050: 3132 3327 7d0a 2020 2020 2020 2020 7232  123'}.        r2
-00001060: 0000 0072 3300 0000 7224 0000 007a 3543  ...r3...r$...z5C
-00001070: 6c6f 7365 2070 6f73 6974 696f 6e20 7265  lose position re
-00001080: 7175 6573 7420 6661 696c 6564 2077 6974  quest failed wit
-00001090: 6820 7374 6174 7573 2063 6f64 6520 2573  h status code %s
-000010a0: 3a20 2573 7a21 436c 6f73 6520 706f 7369  : %sz!Close posi
-000010b0: 7469 6f6e 2072 6571 7565 7374 2066 6169  tion request fai
-000010c0: 6c65 643a 2025 734e 7234 0000 0029 0572  led: %sNr4...).r
-000010d0: 1800 0000 7238 0000 0072 2c00 0000 722d  ....r8...r,...r-
-000010e0: 0000 0072 2e00 0000 7211 0000 0072 1100  ...r....r....r..
-000010f0: 0000 7212 0000 00da 0e63 6c6f 7365 5f70  ..r......close_p
-00001100: 6f73 6974 696f 6e6a 0000 0073 1800 0000  ositionj...s....
-00001110: 0006 0c01 0201 1601 0a01 1002 0201 0201  ................
-00001120: 0aff 02ff 0804 1001 7a1e 506f 7369 7469  ........z.Positi
-00001130: 6f6e 5365 7276 6963 652e 636c 6f73 655f  onService.close_
-00001140: 706f 7369 7469 6f6e 2903 7222 0000 00da  position).r"....
-00001150: 0675 7064 6174 6572 1a00 0000 6303 0000  .updater....c...
-00001160: 0000 0000 0000 0000 0006 0000 000a 0000  ................
-00001170: 0043 0000 0073 9000 0000 7c00 6a00 9b00  .C...s....|.j...
-00001180: 6401 7c01 9b00 9d03 7d03 7a48 7401 6a02  d.|.....}.zHt.j.
-00001190: 7c03 7c00 6a03 7c02 a004 a100 6402 8d03  |.|.j.|.....d...
-000011a0: 7d04 7c04 6a05 6403 6b02 7242 7406 a007  }.|.j.d.k.rBt...
-000011b0: 7c04 a008 a100 a101 5700 5300 7409 6404  |.......W.S.t.d.
-000011c0: 7c04 6a05 7c04 6a0a 6602 1600 8301 8201  |.j.|.j.f.......
-000011d0: 5700 6e32 0400 7401 6a0b 798a 0100 7d05  W.n2..t.j.y...}.
-000011e0: 0100 7a18 7409 6405 7c05 1600 8301 8201  ..z.t.d.|.......
-000011f0: 5700 5900 6406 7d05 7e05 6e0a 6406 7d05  W.Y.d.}.~.n.d.}.
-00001200: 7e05 3000 3000 6406 5300 2907 6106 0100  ~.0.0.d.S.).a...
-00001210: 0055 7064 6174 6520 6120 706f 7369 7469  .Update a positi
-00001220: 6f6e 2066 6f72 2074 6865 2061 7574 6865  on for the authe
-00001230: 6e74 6963 6174 6564 2061 6363 6f75 6e74  nticated account
-00001240: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00001250: 2064 6561 6c5f 6964 3a20 7374 722e 2054   deal_id: str. T
-00001260: 6865 2064 6561 6c20 4944 206f 6620 7468  he deal ID of th
-00001270: 6520 706f 7369 7469 6f6e 2074 6f20 7570  e position to up
-00001280: 6461 7465 2e0a 2020 2020 2020 2020 3a70  date..        :p
-00001290: 6172 616d 2075 7064 6174 653a 2055 7064  aram update: Upd
-000012a0: 6174 6550 6f73 6974 696f 6e2e 2050 6f73  atePosition. Pos
-000012b0: 6974 696f 6e20 7570 6461 7465 2064 6574  ition update det
-000012c0: 6169 6c73 2e0a 2020 2020 2020 2020 3a72  ails..        :r
-000012d0: 6574 7572 6e3a 2044 6561 6c52 6566 6572  eturn: DealRefer
-000012e0: 656e 6365 2065 2e67 3a20 7b27 6465 616c  ence e.g: {'deal
-000012f0: 5265 6665 7265 6e63 6527 3a20 2744 4941  Reference': 'DIA
-00001300: 4141 4142 4242 4343 4331 3233 277d 0a20  AAABBBCCC123'}. 
-00001310: 2020 2020 2020 207a 1c2f 6761 7465 7761         z./gatewa
-00001320: 792f 6465 616c 2f70 6f73 6974 696f 6e73  y/deal/positions
-00001330: 2f6f 7463 2f72 3300 0000 7224 0000 007a  /otc/r3...r$...z
-00001340: 3655 7064 6174 6520 706f 7369 7469 6f6e  6Update position
-00001350: 2072 6571 7565 7374 2066 6169 6c65 6420   request failed 
-00001360: 7769 7468 2073 7461 7475 7320 636f 6465  with status code
-00001370: 2025 733a 2025 737a 2255 7064 6174 6520   %s: %sz"Update 
-00001380: 706f 7369 7469 6f6e 2072 6571 7565 7374  position request
-00001390: 2066 6169 6c65 643a 2025 734e 290c 7217   failed: %sN).r.
-000013a0: 0000 0072 2500 0000 da03 7075 7472 2100  ...r%.....putr!.
-000013b0: 0000 7236 0000 0072 2700 0000 720b 0000  ..r6...r'...r...
-000013c0: 0072 2800 0000 7229 0000 0072 0c00 0000  .r(...r)...r....
-000013d0: 722a 0000 0072 2b00 0000 2906 7218 0000  r*...r+...).r...
-000013e0: 0072 2200 0000 723a 0000 0072 2c00 0000  .r"...r:...r,...
-000013f0: 722d 0000 0072 2e00 0000 7211 0000 0072  r-...r....r....r
-00001400: 1100 0000 7212 0000 00da 0f75 7064 6174  ....r......updat
-00001410: 655f 706f 7369 7469 6f6e 7d00 0000 7318  e_position}...s.
-00001420: 0000 0000 0710 0102 0116 010a 0110 0202  ................
-00001430: 0102 010a ff02 ff08 0410 017a 1f50 6f73  ...........z.Pos
-00001440: 6974 696f 6e53 6572 7669 6365 2e75 7064  itionService.upd
-00001450: 6174 655f 706f 7369 7469 6f6e 4e29 1472  ate_positionN).r
-00001460: 0d00 0000 720e 0000 0072 0f00 0000 da03  ....r....r......
-00001470: 7374 7272 0300 0000 7219 0000 00da 0870  strr....r......p
-00001480: 726f 7065 7274 79da 0464 6963 7472 2100  roperty..dictr!.
-00001490: 0000 7206 0000 0072 2f00 0000 7205 0000  ..r....r/...r...
-000014a0: 0072 3000 0000 7207 0000 0072 0b00 0000  .r0...r....r....
-000014b0: 7237 0000 0072 0800 0000 7239 0000 0072  r7...r....r9...r
-000014c0: 0900 0000 723c 0000 0072 1100 0000 7211  ....r<...r....r.
-000014d0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-000014e0: 0000 1800 0000 7310 0000 0008 0112 0a02  ......s.........
-000014f0: 0110 0a10 140e 1310 1510 1372 1300 0000  ...........r....
-00001500: 2913 da07 6c6f 6767 696e 6772 2500 0000  )...loggingr%...
-00001510: da08 7079 6461 6e74 6963 7202 0000 00da  ..pydanticr.....
-00001520: 0e69 675f 7472 6164 696e 675f 6c69 6272  .ig_trading_libr
-00001530: 0300 0000 da06 6d6f 6465 6c73 7205 0000  ......modelsr...
-00001540: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
-00001550: 7209 0000 0072 0b00 0000 da09 6765 744c  r....r......getL
-00001560: 6f67 6765 7272 0d00 0000 da06 6c6f 6767  oggerr......logg
-00001570: 6572 da09 4578 6365 7074 696f 6e72 0c00  er..Exceptionr..
-00001580: 0000 7213 0000 0072 1100 0000 7211 0000  ..r....r....r...
-00001590: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
-000015a0: 6475 6c65 3e01 0000 0073 1000 0000 0802  dule>....s......
-000015b0: 0801 0c02 0c01 1c07 0c03 0a03 1004       ..............
+00000ee0: 6974 696f 6e29 0372 2200 0000 da06 7570  ition).r".....up
+00000ef0: 6461 7465 721a 0000 0063 0300 0000 0000  dater....c......
+00000f00: 0000 0000 0000 0600 0000 0a00 0000 4300  ..............C.
+00000f10: 0000 7390 0000 007c 006a 009b 0064 017c  ..s....|.j...d.|
+00000f20: 019b 009d 037d 037a 4874 016a 027c 037c  .....}.zHt.j.|.|
+00000f30: 006a 037c 02a0 04a1 0064 028d 037d 047c  .j.|.....d...}.|
+00000f40: 046a 0564 036b 0272 4274 06a0 077c 04a0  .j.d.k.rBt...|..
+00000f50: 08a1 00a1 0157 0053 0074 0964 047c 046a  .....W.S.t.d.|.j
+00000f60: 057c 046a 0a66 0216 0083 0182 0157 006e  .|.j.f.......W.n
+00000f70: 3204 0074 016a 0b79 8a01 007d 0501 007a  2..t.j.y...}...z
+00000f80: 1874 0964 057c 0516 0083 0182 0157 0059  .t.d.|.......W.Y
+00000f90: 0064 067d 057e 056e 0a64 067d 057e 0530  .d.}.~.n.d.}.~.0
+00000fa0: 0030 0064 0653 0029 0761 0601 0000 5570  .0.d.S.).a....Up
+00000fb0: 6461 7465 2061 2070 6f73 6974 696f 6e20  date a position 
+00000fc0: 666f 7220 7468 6520 6175 7468 656e 7469  for the authenti
+00000fd0: 6361 7465 6420 6163 636f 756e 742e 0a20  cated account.. 
+00000fe0: 2020 2020 2020 203a 7061 7261 6d20 6465         :param de
+00000ff0: 616c 5f69 643a 2073 7472 2e20 5468 6520  al_id: str. The 
+00001000: 6465 616c 2049 4420 6f66 2074 6865 2070  deal ID of the p
+00001010: 6f73 6974 696f 6e20 746f 2075 7064 6174  osition to updat
+00001020: 652e 0a20 2020 2020 2020 203a 7061 7261  e..        :para
+00001030: 6d20 7570 6461 7465 3a20 5570 6461 7465  m update: Update
+00001040: 506f 7369 7469 6f6e 2e20 506f 7369 7469  Position. Positi
+00001050: 6f6e 2075 7064 6174 6520 6465 7461 696c  on update detail
+00001060: 732e 0a20 2020 2020 2020 203a 7265 7475  s..        :retu
+00001070: 726e 3a20 4465 616c 5265 6665 7265 6e63  rn: DealReferenc
+00001080: 6520 652e 673a 207b 2764 6561 6c52 6566  e e.g: {'dealRef
+00001090: 6572 656e 6365 273a 2027 4449 4141 4141  erence': 'DIAAAA
+000010a0: 4242 4243 4343 3132 3327 7d0a 2020 2020  BBBCCC123'}.    
+000010b0: 2020 2020 7a1c 2f67 6174 6577 6179 2f64      z./gateway/d
+000010c0: 6561 6c2f 706f 7369 7469 6f6e 732f 6f74  eal/positions/ot
+000010d0: 632f 7233 0000 0072 2400 0000 7a36 5570  c/r3...r$...z6Up
+000010e0: 6461 7465 2070 6f73 6974 696f 6e20 7265  date position re
+000010f0: 7175 6573 7420 6661 696c 6564 2077 6974  quest failed wit
+00001100: 6820 7374 6174 7573 2063 6f64 6520 2573  h status code %s
+00001110: 3a20 2573 7a22 5570 6461 7465 2070 6f73  : %sz"Update pos
+00001120: 6974 696f 6e20 7265 7175 6573 7420 6661  ition request fa
+00001130: 696c 6564 3a20 2573 4e29 0c72 1700 0000  iled: %sN).r....
+00001140: 7225 0000 00da 0370 7574 7221 0000 0072  r%.....putr!...r
+00001150: 3500 0000 7227 0000 0072 0b00 0000 7228  5...r'...r....r(
+00001160: 0000 0072 2900 0000 720c 0000 0072 2a00  ...r)...r....r*.
+00001170: 0000 722b 0000 0029 0672 1800 0000 7222  ..r+...).r....r"
+00001180: 0000 0072 3700 0000 722c 0000 0072 2d00  ...r7...r,...r-.
+00001190: 0000 722e 0000 0072 1100 0000 7211 0000  ..r....r....r...
+000011a0: 0072 1200 0000 da0f 7570 6461 7465 5f70  .r......update_p
+000011b0: 6f73 6974 696f 6e6a 0000 0073 1800 0000  ositionj...s....
+000011c0: 0007 1001 0201 1601 0a01 1002 0201 0201  ................
+000011d0: 0aff 02ff 0804 1001 7a1f 506f 7369 7469  ........z.Positi
+000011e0: 6f6e 5365 7276 6963 652e 7570 6461 7465  onService.update
+000011f0: 5f70 6f73 6974 696f 6e29 02da 0563 6c6f  _position)...clo
+00001200: 7365 721a 0000 0063 0200 0000 0000 0000  ser....c........
+00001210: 0000 0000 0700 0000 0a00 0000 4300 0000  ............C...
+00001220: 73ac 0000 007c 006a 009b 0064 019d 027d  s....|.j...d...}
+00001230: 027c 006a 01a0 02a1 007d 0364 027c 0364  .|.j.....}.d.|.d
+00001240: 033c 0064 047c 0364 053c 007c 016a 0364  .<.d.|.d.<.|.j.d
+00001250: 0664 078d 017d 047a 4274 046a 057c 027c  .d...}.zBt.j.|.|
+00001260: 037c 0464 088d 037d 057c 056a 0664 096b  .|.d...}.|.j.d.k
+00001270: 0272 5e74 07a0 087c 05a0 09a1 00a1 0157  .r^t...|.......W
+00001280: 0053 0074 0a64 0a7c 056a 067c 056a 0b66  .S.t.d.|.j.|.j.f
+00001290: 0216 0083 0182 0157 006e 3204 0074 046a  .......W.n2..t.j
+000012a0: 0c79 a601 007d 0601 007a 1874 0a64 0b7c  .y...}...z.t.d.|
+000012b0: 0616 0083 0182 0157 0059 0064 0c7d 067e  .......W.Y.d.}.~
+000012c0: 066e 0a64 0c7d 067e 0630 0030 0064 0c53  .n.d.}.~.0.0.d.S
+000012d0: 0029 0d7a bd43 6c6f 7365 2061 2070 6f73  .).z.Close a pos
+000012e0: 6974 696f 6e20 666f 7220 7468 6520 6175  ition for the au
+000012f0: 7468 656e 7469 6361 7465 6420 6163 636f  thenticated acco
+00001300: 756e 742e 0a20 2020 2020 2020 203a 7061  unt..        :pa
+00001310: 7261 6d20 636c 6f73 653a 2043 6c6f 7365  ram close: Close
+00001320: 506f 7369 7469 6f6e 2e20 5468 6520 706f  Position. The po
+00001330: 7369 7469 6f6e 2074 6f20 636c 6f73 652e  sition to close.
+00001340: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00001350: 3a20 4465 616c 5265 6665 7265 6e63 6520  : DealReference 
+00001360: 652e 673a 207b 2764 6561 6c52 6566 6572  e.g: {'dealRefer
+00001370: 656e 6365 273a 2027 4449 4141 4141 4242  ence': 'DIAAAABB
+00001380: 4243 4343 3132 3327 7d0a 2020 2020 2020  BCCC123'}.      
+00001390: 2020 7232 0000 00da 0131 721d 0000 00da    r2.....1r.....
+000013a0: 0644 454c 4554 45da 075f 6d65 7468 6f64  .DELETE.._method
+000013b0: 5429 01da 0c65 7863 6c75 6465 5f6e 6f6e  T)...exclude_non
+000013c0: 6572 3300 0000 7224 0000 007a 3543 6c6f  er3...r$...z5Clo
+000013d0: 7365 2070 6f73 6974 696f 6e20 7265 7175  se position requ
+000013e0: 6573 7420 6661 696c 6564 2077 6974 6820  est failed with 
+000013f0: 7374 6174 7573 2063 6f64 6520 2573 3a20  status code %s: 
+00001400: 2573 7a21 436c 6f73 6520 706f 7369 7469  %sz!Close positi
+00001410: 6f6e 2072 6571 7565 7374 2066 6169 6c65  on request faile
+00001420: 643a 2025 734e 290d 7217 0000 0072 2100  d: %sN).r....r!.
+00001430: 0000 da04 636f 7079 7235 0000 0072 2500  ....copyr5...r%.
+00001440: 0000 7234 0000 0072 2700 0000 720b 0000  ..r4...r'...r...
+00001450: 0072 2800 0000 7229 0000 0072 0c00 0000  .r(...r)...r....
+00001460: 722a 0000 0072 2b00 0000 2907 7218 0000  r*...r+...).r...
+00001470: 0072 3a00 0000 722c 0000 0072 2100 0000  .r:...r,...r!...
+00001480: 7229 0000 0072 2d00 0000 722e 0000 0072  r)...r-...r....r
+00001490: 1100 0000 7211 0000 0072 1200 0000 da0e  ....r....r......
+000014a0: 636c 6f73 655f 706f 7369 7469 6f6e 7e00  close_position~.
+000014b0: 0000 7320 0000 0000 060c 010a 0108 0108  ..s ............
+000014c0: 010c 0102 0110 010a 0110 0202 0102 010a  ................
+000014d0: ff02 ff08 0410 017a 1e50 6f73 6974 696f  .......z.Positio
+000014e0: 6e53 6572 7669 6365 2e63 6c6f 7365 5f70  nService.close_p
+000014f0: 6f73 6974 696f 6e4e 2914 720d 0000 0072  ositionN).r....r
+00001500: 0e00 0000 720f 0000 00da 0373 7472 7203  ....r......strr.
+00001510: 0000 0072 1900 0000 da08 7072 6f70 6572  ...r......proper
+00001520: 7479 da04 6469 6374 7221 0000 0072 0600  ty..dictr!...r..
+00001530: 0000 722f 0000 0072 0500 0000 7230 0000  ..r/...r....r0..
+00001540: 0072 0700 0000 720b 0000 0072 3600 0000  .r....r....r6...
+00001550: 7209 0000 0072 3900 0000 7208 0000 0072  r....r9...r....r
+00001560: 4000 0000 7211 0000 0072 1100 0000 7211  @...r....r....r.
+00001570: 0000 0072 1200 0000 7213 0000 0018 0000  ...r....r.......
+00001580: 0073 1000 0000 0801 120a 0201 100a 1014  .s..............
+00001590: 0e13 1015 1214 7213 0000 0029 13da 076c  ......r....)...l
+000015a0: 6f67 6769 6e67 7225 0000 00da 0870 7964  oggingr%.....pyd
+000015b0: 616e 7469 6372 0200 0000 da0e 6967 5f74  anticr......ig_t
+000015c0: 7261 6469 6e67 5f6c 6962 7203 0000 00da  rading_libr.....
+000015d0: 066d 6f64 656c 7372 0500 0000 7206 0000  .modelsr....r...
+000015e0: 0072 0700 0000 7208 0000 0072 0900 0000  .r....r....r....
+000015f0: 720b 0000 00da 0967 6574 4c6f 6767 6572  r......getLogger
+00001600: 720d 0000 00da 066c 6f67 6765 72da 0945  r......logger..E
+00001610: 7863 6570 7469 6f6e 720c 0000 0072 1300  xceptionr....r..
+00001620: 0000 7211 0000 0072 1100 0000 7211 0000  ..r....r....r...
+00001630: 0072 1200 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+00001640: 0100 0000 7310 0000 0008 0208 010c 020c  ....s...........
+00001650: 011c 070c 030a 0310 04                   .........
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/models.py` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,20 @@
     positions: List[OpenPosition]
 
 
 class CreatePosition(BaseModel):
     currencyCode: constr(pattern=r"^[A-Z]{3}$")
     direction: Direction
     epic: constr(pattern=r"^[A-Za-z0-9._]{6,30}$")
-    expiry: constr(pattern=r"^(\d{2}-)?[A-Z]{3}-\d{2}|-|DFB$")
-    forceOpen: bool
-    guaranteedStop: bool
-    orderType: OrderType
-    timeInForce: TimeInForce
-    trailingStop: bool
+    expiry: constr(pattern=r"^(\d{2}-)?[A-Z]{3}-\d{2}|-|DFB$") = "DFB"
+    forceOpen: bool = False
+    guaranteedStop: bool = False
+    orderType: OrderType = "MARKET"
+    timeInForce: TimeInForce = "EXECUTE_AND_ELIMINATE"
+    trailingStop: bool = False
     dealReference: Optional[constr(pattern=r"^[A-Za-z0-9_\-.]{1,30}$")] = None
     level: Optional[condecimal(decimal_places=12)] = None
     limitDistance: Optional[condecimal(decimal_places=2)] = None
     limitLevel: Optional[condecimal(decimal_places=2)] = None
     quoteId: Optional[constr(pattern=r"^[A-Za-z0-9]+$")] = None
     size: condecimal(decimal_places=2, gt=0)
     stopDistance: Optional[condecimal(decimal_places=2)] = None
@@ -187,15 +187,15 @@
         return data
 
 
 class ClosePosition(BaseModel):
     direction: Direction
     orderType: OrderType
     size: condecimal(gt=0, decimal_places=2)
-    timeInForce: TimeInForce
+    timeInForce: TimeInForce = None
     quoteId: Optional[str] = None
     dealId: Optional[constr(pattern=".{1,30}")] = None
     epic: Optional[constr(pattern="[A-Za-z0-9._]{6,30}")] = None
     expiry: Optional[constr(pattern="(\\d{2}-)?[A-Z]{3}-\\d{2}|-|DFB")] = None
     level: Optional[condecimal(decimal_places=12)] = None
 
     @field_serializer("level", "size", mode="plain")
```

### Comparing `ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/service.py` & `ig_trading_lib-0.4.0/ig_trading_lib/trading/positions/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,45 +99,49 @@
                 raise PositionsError(
                     "Create position request failed with status code %s: %s"
                     % (response.status_code, response.text)
                 )
         except requests.RequestException as e:
             raise PositionsError("Create position request failed: %s" % e)
 
-    def close_position(self, close: ClosePosition) -> DealReference:
-        """Close a position for the authenticated account.
-        :param close: ClosePosition. The position to close.
+    def update_position(self, deal_id: str, update: UpdatePosition) -> DealReference:
+        """Update a position for the authenticated account.
+        :param deal_id: str. The deal ID of the position to update.
+        :param update: UpdatePosition. Position update details.
         :return: DealReference e.g: {'dealReference': 'DIAAAABBBCCC123'}
         """
 
-        url = f"{self.base_url}/gateway/deal/positions/otc"
+        url = f"{self.base_url}/gateway/deal/positions/otc/{deal_id}"
         try:
-            response = requests.post(url, headers=self.headers, json=close.model_dump())
+            response = requests.put(url, headers=self.headers, json=update.model_dump())
             if response.status_code == 200:
                 return DealReference.model_validate(response.json())
             else:
                 raise PositionsError(
-                    "Close position request failed with status code %s: %s"
+                    "Update position request failed with status code %s: %s"
                     % (response.status_code, response.text)
                 )
         except requests.RequestException as e:
-            raise PositionsError("Close position request failed: %s" % e)
+            raise PositionsError("Update position request failed: %s" % e)
 
-    def update_position(self, deal_id: str, update: UpdatePosition) -> DealReference:
-        """Update a position for the authenticated account.
-        :param deal_id: str. The deal ID of the position to update.
-        :param update: UpdatePosition. Position update details.
+    def close_position(self, close: ClosePosition) -> DealReference:
+        """Close a position for the authenticated account.
+        :param close: ClosePosition. The position to close.
         :return: DealReference e.g: {'dealReference': 'DIAAAABBBCCC123'}
         """
 
-        url = f"{self.base_url}/gateway/deal/positions/otc/{deal_id}"
+        url = f"{self.base_url}/gateway/deal/positions/otc"
+        headers = self.headers.copy()
+        headers["Version"] = "1"
+        headers["_method"] = "DELETE"
+        json = close.model_dump(exclude_none=True)
         try:
-            response = requests.put(url, headers=self.headers, json=update.model_dump())
+            response = requests.post(url, headers=headers, json=json)
             if response.status_code == 200:
                 return DealReference.model_validate(response.json())
             else:
                 raise PositionsError(
-                    "Update position request failed with status code %s: %s"
+                    "Close position request failed with status code %s: %s"
                     % (response.status_code, response.text)
                 )
         except requests.RequestException as e:
-            raise PositionsError("Update position request failed: %s" % e)
+            raise PositionsError("Close position request failed: %s" % e)
```

### Comparing `ig_trading_lib-0.3.0/pyproject.toml` & `ig_trading_lib-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ig-trading-lib"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Python library for IG Trading."
 authors = ["Evgeny Aleshin"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `ig_trading_lib-0.3.0/PKG-INFO` & `ig_trading_lib-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ig-trading-lib
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Python library for IG Trading.
 License: MIT
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


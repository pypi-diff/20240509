# Comparing `tmp/pyav-12.1.0rc1.tar.gz` & `tmp/pyav-12.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyav-12.1.0rc1.tar", last modified: Wed May  8 00:42:33 2024, max compression
+gzip compressed data, was "pyav-12.1.0rc2.tar", last modified: Thu May  9 08:53:06 2024, max compression
```

## Comparing `pyav-12.1.0rc1.tar` & `pyav-12.1.0rc2.tar`

### file list

```diff
@@ -1,307 +1,307 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.092471 pyav-12.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-08 00:42:33.088471 pyav-12.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.032470 pyav-12.1.0rc1/av/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/_core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/_core.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/about.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.036470 pyav-12.1.0rc1/av/audio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/codeccontext.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/codeccontext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/codeccontext.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/fifo.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/fifo.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/format.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/format.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/frame.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/frame.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/layout.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/layout.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/layout.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/plane.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/plane.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/plane.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/resampler.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/resampler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/resampler.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/audio/stream.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/bitstream.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/bitstream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/bitstream.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/buffer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/buffer.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/bytesource.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/bytesource.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.036470 pyav-12.1.0rc1/av/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/codec/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/codec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/codec/codec.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/codec/codec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/codec/codec.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/codec/context.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/codec/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/codec/context.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.036470 pyav-12.1.0rc1/av/container/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/core.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/core.pyi
--rwxr-xr-x   0 runner    (1001) docker     (127)    15242 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/core.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/input.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/input.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/input.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/output.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/output.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/output.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/pyio.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/pyio.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/streams.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/streams.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/container/streams.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.040470 pyav-12.1.0rc1/av/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/data/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/data/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/data/stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/data/stream.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/descriptor.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/descriptor.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/dictionary.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/dictionary.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/dictionary.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/enum.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/enum.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/enum.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/error.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/error.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.040470 pyav-12.1.0rc1/av/filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/context.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/context.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/context.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/filter.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/filter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/filter.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/graph.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/graph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/graph.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/link.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/link.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/link.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/pad.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/pad.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/filter/pad.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/format.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/format.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/frame.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/frame.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/logging.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/logging.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/logging.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/option.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/option.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/option.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/packet.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/packet.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/packet.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/plane.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/plane.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/plane.pyx
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.040470 pyav-12.1.0rc1/av/sidedata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/sidedata/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/sidedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/sidedata/motionvectors.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/sidedata/motionvectors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/sidedata/motionvectors.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/sidedata/sidedata.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/sidedata/sidedata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/sidedata/sidedata.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/stream.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.044470 pyav-12.1.0rc1/av/subtitles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/codeccontext.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/codeccontext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/codeccontext.pyx
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/stream.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/subtitle.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/subtitle.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/subtitles/subtitle.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.044470 pyav-12.1.0rc1/av/video/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/codeccontext.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/codeccontext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/codeccontext.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/format.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/format.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/frame.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/frame.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/plane.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/plane.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/plane.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/reformatter.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/reformatter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/reformatter.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/av/video/stream.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.044470 pyav-12.1.0rc1/include/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libav.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.048470 pyav-12.1.0rc1/include/libavcodec/
--rw-r--r--   0 runner    (1001) docker     (127)    13444 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavcodec/avcodec.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavcodec/bsf.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.048470 pyav-12.1.0rc1/include/libavdevice/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavdevice/avdevice.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.048470 pyav-12.1.0rc1/include/libavfilter/
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavfilter/avfilter.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavfilter/avfiltergraph.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavfilter/buffersink.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavfilter/buffersrc.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.048470 pyav-12.1.0rc1/include/libavformat/
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavformat/avformat.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.048470 pyav-12.1.0rc1/include/libavutil/
--rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavutil/avutil.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavutil/channel_layout.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavutil/dict.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavutil/error.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavutil/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavutil/motion_vector.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libavutil/samplefmt.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.048470 pyav-12.1.0rc1/include/libswresample/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libswresample/swresample.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.048470 pyav-12.1.0rc1/include/libswscale/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/include/libswscale/swscale.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.048470 pyav-12.1.0rc1/pyav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-08 00:42:32.000000 pyav-12.1.0rc1/pyav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-08 00:42:33.000000 pyav-12.1.0rc1/pyav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:42:32.000000 pyav-12.1.0rc1/pyav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 00:42:32.000000 pyav-12.1.0rc1/pyav.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 00:42:32.000000 pyav-12.1.0rc1/pyav.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-08 00:42:32.000000 pyav-12.1.0rc1/pyav.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 00:42:33.092471 pyav-12.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.020469 pyav-12.1.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.060470 pyav-12.1.0rc1/src/av/
--rw-r--r--   0 runner    (1001) docker     (127)   228698 2024-05-08 00:42:25.000000 pyav-12.1.0rc1/src/av/_core.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.064470 pyav-12.1.0rc1/src/av/audio/
--rw-r--r--   0 runner    (1001) docker     (127)   429089 2024-05-08 00:42:30.000000 pyav-12.1.0rc1/src/av/audio/codeccontext.c
--rw-r--r--   0 runner    (1001) docker     (127)   490647 2024-05-08 00:42:29.000000 pyav-12.1.0rc1/src/av/audio/fifo.c
--rw-r--r--   0 runner    (1001) docker     (127)   387525 2024-05-08 00:42:29.000000 pyav-12.1.0rc1/src/av/audio/format.c
--rw-r--r--   0 runner    (1001) docker     (127)   572417 2024-05-08 00:42:29.000000 pyav-12.1.0rc1/src/av/audio/frame.c
--rw-r--r--   0 runner    (1001) docker     (127)   569637 2024-05-08 00:42:30.000000 pyav-12.1.0rc1/src/av/audio/layout.c
--rw-r--r--   0 runner    (1001) docker     (127)   357622 2024-05-08 00:42:29.000000 pyav-12.1.0rc1/src/av/audio/plane.c
--rw-r--r--   0 runner    (1001) docker     (127)   505097 2024-05-08 00:42:30.000000 pyav-12.1.0rc1/src/av/audio/resampler.c
--rw-r--r--   0 runner    (1001) docker     (127)   406373 2024-05-08 00:42:30.000000 pyav-12.1.0rc1/src/av/audio/stream.c
--rw-r--r--   0 runner    (1001) docker     (127)   398227 2024-05-08 00:42:23.000000 pyav-12.1.0rc1/src/av/bitstream.c
--rw-r--r--   0 runner    (1001) docker     (127)   411731 2024-05-08 00:42:23.000000 pyav-12.1.0rc1/src/av/buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)   315061 2024-05-08 00:42:23.000000 pyav-12.1.0rc1/src/av/bytesource.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.068470 pyav-12.1.0rc1/src/av/codec/
--rw-r--r--   0 runner    (1001) docker     (127)   641826 2024-05-08 00:42:28.000000 pyav-12.1.0rc1/src/av/codec/codec.c
--rw-r--r--   0 runner    (1001) docker     (127)  1057195 2024-05-08 00:42:28.000000 pyav-12.1.0rc1/src/av/codec/context.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.072470 pyav-12.1.0rc1/src/av/container/
--rw-r--r--   0 runner    (1001) docker     (127)   786872 2024-05-08 00:42:26.000000 pyav-12.1.0rc1/src/av/container/core.c
--rw-r--r--   0 runner    (1001) docker     (127)   636779 2024-05-08 00:42:26.000000 pyav-12.1.0rc1/src/av/container/input.c
--rw-r--r--   0 runner    (1001) docker     (127)   570542 2024-05-08 00:42:26.000000 pyav-12.1.0rc1/src/av/container/output.c
--rw-r--r--   0 runner    (1001) docker     (127)   428774 2024-05-08 00:42:25.000000 pyav-12.1.0rc1/src/av/container/pyio.c
--rw-r--r--   0 runner    (1001) docker     (127)   506624 2024-05-08 00:42:25.000000 pyav-12.1.0rc1/src/av/container/streams.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.072470 pyav-12.1.0rc1/src/av/data/
--rw-r--r--   0 runner    (1001) docker     (127)   357940 2024-05-08 00:42:30.000000 pyav-12.1.0rc1/src/av/data/stream.c
--rw-r--r--   0 runner    (1001) docker     (127)   353528 2024-05-08 00:42:22.000000 pyav-12.1.0rc1/src/av/descriptor.c
--rw-r--r--   0 runner    (1001) docker     (127)   444866 2024-05-08 00:42:24.000000 pyav-12.1.0rc1/src/av/dictionary.c
--rw-r--r--   0 runner    (1001) docker     (127)   867500 2024-05-08 00:42:23.000000 pyav-12.1.0rc1/src/av/enum.c
--rw-r--r--   0 runner    (1001) docker     (127)   686509 2024-05-08 00:42:22.000000 pyav-12.1.0rc1/src/av/error.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.076470 pyav-12.1.0rc1/src/av/filter/
--rw-r--r--   0 runner    (1001) docker     (127)   523994 2024-05-08 00:42:31.000000 pyav-12.1.0rc1/src/av/filter/context.c
--rw-r--r--   0 runner    (1001) docker     (127)   611535 2024-05-08 00:42:31.000000 pyav-12.1.0rc1/src/av/filter/filter.c
--rw-r--r--   0 runner    (1001) docker     (127)   614694 2024-05-08 00:42:31.000000 pyav-12.1.0rc1/src/av/filter/graph.c
--rw-r--r--   0 runner    (1001) docker     (127)   379619 2024-05-08 00:42:32.000000 pyav-12.1.0rc1/src/av/filter/link.c
--rw-r--r--   0 runner    (1001) docker     (127)   414805 2024-05-08 00:42:31.000000 pyav-12.1.0rc1/src/av/filter/pad.c
--rw-r--r--   0 runner    (1001) docker     (127)   479599 2024-05-08 00:42:24.000000 pyav-12.1.0rc1/src/av/format.c
--rw-r--r--   0 runner    (1001) docker     (127)   435749 2024-05-08 00:42:24.000000 pyav-12.1.0rc1/src/av/frame.c
--rw-r--r--   0 runner    (1001) docker     (127)   563016 2024-05-08 00:42:23.000000 pyav-12.1.0rc1/src/av/logging.c
--rw-r--r--   0 runner    (1001) docker     (127)   504998 2024-05-08 00:42:24.000000 pyav-12.1.0rc1/src/av/option.c
--rw-r--r--   0 runner    (1001) docker     (127)   489209 2024-05-08 00:42:24.000000 pyav-12.1.0rc1/src/av/packet.c
--rw-r--r--   0 runner    (1001) docker     (127)   362713 2024-05-08 00:42:23.000000 pyav-12.1.0rc1/src/av/plane.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.076470 pyav-12.1.0rc1/src/av/sidedata/
--rw-r--r--   0 runner    (1001) docker     (127)   540636 2024-05-08 00:42:25.000000 pyav-12.1.0rc1/src/av/sidedata/motionvectors.c
--rw-r--r--   0 runner    (1001) docker     (127)   556413 2024-05-08 00:42:25.000000 pyav-12.1.0rc1/src/av/sidedata/sidedata.c
--rw-r--r--   0 runner    (1001) docker     (127)   494980 2024-05-08 00:42:24.000000 pyav-12.1.0rc1/src/av/stream.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.080470 pyav-12.1.0rc1/src/av/subtitles/
--rw-r--r--   0 runner    (1001) docker     (127)   356129 2024-05-08 00:42:32.000000 pyav-12.1.0rc1/src/av/subtitles/codeccontext.c
--rw-r--r--   0 runner    (1001) docker     (127)   341775 2024-05-08 00:42:32.000000 pyav-12.1.0rc1/src/av/subtitles/stream.c
--rw-r--r--   0 runner    (1001) docker     (127)   821623 2024-05-08 00:42:32.000000 pyav-12.1.0rc1/src/av/subtitles/subtitle.c
--rw-r--r--   0 runner    (1001) docker     (127)   265628 2024-05-08 00:42:25.000000 pyav-12.1.0rc1/src/av/utils.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.084470 pyav-12.1.0rc1/src/av/video/
--rw-r--r--   0 runner    (1001) docker     (127)   595328 2024-05-08 00:42:28.000000 pyav-12.1.0rc1/src/av/video/codeccontext.c
--rw-r--r--   0 runner    (1001) docker     (127)   613578 2024-05-08 00:42:27.000000 pyav-12.1.0rc1/src/av/video/format.c
--rw-r--r--   0 runner    (1001) docker     (127)  1757212 2024-05-08 00:42:27.000000 pyav-12.1.0rc1/src/av/video/frame.c
--rw-r--r--   0 runner    (1001) docker     (127)   430748 2024-05-08 00:42:26.000000 pyav-12.1.0rc1/src/av/video/plane.c
--rw-r--r--   0 runner    (1001) docker     (127)   480479 2024-05-08 00:42:28.000000 pyav-12.1.0rc1/src/av/video/reformatter.c
--rw-r--r--   0 runner    (1001) docker     (127)   424135 2024-05-08 00:42:27.000000 pyav-12.1.0rc1/src/av/video/stream.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:33.088471 pyav-12.1.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_audiofifo.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_audioformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_audioframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_audiolayout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_audioresampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_bitstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)    17838 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_codec_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_colorspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_containerformat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_doctests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_file_probing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_packet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_python_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_seek.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_videoformat.py
--rw-r--r--   0 runner    (1001) docker     (127)    28349 2024-05-08 00:42:18.000000 pyav-12.1.0rc1/tests/test_videoframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.051927 pyav-12.1.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-09 08:53:06.051927 pyav-12.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:05.991926 pyav-12.1.0rc2/av/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/_core.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/about.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:05.995926 pyav-12.1.0rc2/av/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/codeccontext.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/codeccontext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/codeccontext.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/fifo.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/fifo.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/format.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/format.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/frame.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/frame.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/layout.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/layout.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/layout.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/plane.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/plane.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/plane.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/resampler.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/resampler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/resampler.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/audio/stream.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/bitstream.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/bitstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/bitstream.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/buffer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/buffer.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/bytesource.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/bytesource.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:05.995926 pyav-12.1.0rc2/av/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/codec/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/codec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/codec/codec.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/codec/codec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/codec/codec.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/codec/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/codec/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22428 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/codec/context.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:05.999926 pyav-12.1.0rc2/av/container/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/core.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/core.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15242 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/input.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/input.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/input.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/output.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/output.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/output.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/pyio.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/pyio.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/streams.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/streams.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/container/streams.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:05.999926 pyav-12.1.0rc2/av/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/data/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/data/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/data/stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/data/stream.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/descriptor.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/descriptor.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/dictionary.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/dictionary.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/dictionary.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/enum.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10479 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/enum.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/error.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/error.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.003926 pyav-12.1.0rc2/av/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/context.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/filter.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/filter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/filter.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/graph.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/graph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/graph.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/link.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/link.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/link.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/pad.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/pad.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/filter/pad.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/format.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/format.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/frame.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/frame.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/logging.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/logging.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/logging.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/option.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/option.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/option.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/packet.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/packet.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/packet.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/plane.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/plane.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/plane.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.003926 pyav-12.1.0rc2/av/sidedata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/sidedata/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/sidedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/sidedata/motionvectors.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/sidedata/motionvectors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/sidedata/motionvectors.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/sidedata/sidedata.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/sidedata/sidedata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/sidedata/sidedata.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/stream.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.003926 pyav-12.1.0rc2/av/subtitles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/codeccontext.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/codeccontext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/codeccontext.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/stream.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/subtitle.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/subtitle.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/subtitles/subtitle.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.007926 pyav-12.1.0rc2/av/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/codeccontext.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/codeccontext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/codeccontext.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/format.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/format.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/frame.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22927 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/frame.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/plane.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/plane.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/plane.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/reformatter.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/reformatter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/reformatter.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/av/video/stream.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.007926 pyav-12.1.0rc2/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libav.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.007926 pyav-12.1.0rc2/include/libavcodec/
+-rw-r--r--   0 runner    (1001) docker     (127)    13444 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavcodec/avcodec.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavcodec/bsf.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.007926 pyav-12.1.0rc2/include/libavdevice/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavdevice/avdevice.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.007926 pyav-12.1.0rc2/include/libavfilter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavfilter/avfilter.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavfilter/avfiltergraph.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavfilter/buffersink.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavfilter/buffersrc.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.007926 pyav-12.1.0rc2/include/libavformat/
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavformat/avformat.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.011927 pyav-12.1.0rc2/include/libavutil/
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavutil/avutil.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavutil/channel_layout.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavutil/dict.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavutil/error.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavutil/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavutil/motion_vector.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libavutil/samplefmt.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.011927 pyav-12.1.0rc2/include/libswresample/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libswresample/swresample.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.011927 pyav-12.1.0rc2/include/libswscale/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/include/libswscale/swscale.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.011927 pyav-12.1.0rc2/pyav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-09 08:53:05.000000 pyav-12.1.0rc2/pyav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-05-09 08:53:05.000000 pyav-12.1.0rc2/pyav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:53:05.000000 pyav-12.1.0rc2/pyav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 08:53:05.000000 pyav-12.1.0rc2/pyav.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:53:05.000000 pyav-12.1.0rc2/pyav.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-09 08:53:05.000000 pyav-12.1.0rc2/pyav.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:53:06.051927 pyav-12.1.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:05.983926 pyav-12.1.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.019926 pyav-12.1.0rc2/src/av/
+-rw-r--r--   0 runner    (1001) docker     (127)   228698 2024-05-09 08:52:56.000000 pyav-12.1.0rc2/src/av/_core.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.027927 pyav-12.1.0rc2/src/av/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)   429089 2024-05-09 08:53:02.000000 pyav-12.1.0rc2/src/av/audio/codeccontext.c
+-rw-r--r--   0 runner    (1001) docker     (127)   490647 2024-05-09 08:53:02.000000 pyav-12.1.0rc2/src/av/audio/fifo.c
+-rw-r--r--   0 runner    (1001) docker     (127)   387525 2024-05-09 08:53:02.000000 pyav-12.1.0rc2/src/av/audio/format.c
+-rw-r--r--   0 runner    (1001) docker     (127)   572417 2024-05-09 08:53:01.000000 pyav-12.1.0rc2/src/av/audio/frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)   569637 2024-05-09 08:53:02.000000 pyav-12.1.0rc2/src/av/audio/layout.c
+-rw-r--r--   0 runner    (1001) docker     (127)   357622 2024-05-09 08:53:01.000000 pyav-12.1.0rc2/src/av/audio/plane.c
+-rw-r--r--   0 runner    (1001) docker     (127)   505097 2024-05-09 08:53:03.000000 pyav-12.1.0rc2/src/av/audio/resampler.c
+-rw-r--r--   0 runner    (1001) docker     (127)   406373 2024-05-09 08:53:02.000000 pyav-12.1.0rc2/src/av/audio/stream.c
+-rw-r--r--   0 runner    (1001) docker     (127)   398227 2024-05-09 08:52:55.000000 pyav-12.1.0rc2/src/av/bitstream.c
+-rw-r--r--   0 runner    (1001) docker     (127)   411731 2024-05-09 08:52:54.000000 pyav-12.1.0rc2/src/av/buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)   315061 2024-05-09 08:52:55.000000 pyav-12.1.0rc2/src/av/bytesource.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.027927 pyav-12.1.0rc2/src/av/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)   641826 2024-05-09 08:53:00.000000 pyav-12.1.0rc2/src/av/codec/codec.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1057195 2024-05-09 08:53:01.000000 pyav-12.1.0rc2/src/av/codec/context.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.031927 pyav-12.1.0rc2/src/av/container/
+-rw-r--r--   0 runner    (1001) docker     (127)   786872 2024-05-09 08:52:58.000000 pyav-12.1.0rc2/src/av/container/core.c
+-rw-r--r--   0 runner    (1001) docker     (127)   636779 2024-05-09 08:52:57.000000 pyav-12.1.0rc2/src/av/container/input.c
+-rw-r--r--   0 runner    (1001) docker     (127)   570542 2024-05-09 08:52:58.000000 pyav-12.1.0rc2/src/av/container/output.c
+-rw-r--r--   0 runner    (1001) docker     (127)   428774 2024-05-09 08:52:57.000000 pyav-12.1.0rc2/src/av/container/pyio.c
+-rw-r--r--   0 runner    (1001) docker     (127)   506624 2024-05-09 08:52:57.000000 pyav-12.1.0rc2/src/av/container/streams.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.035927 pyav-12.1.0rc2/src/av/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   357940 2024-05-09 08:53:03.000000 pyav-12.1.0rc2/src/av/data/stream.c
+-rw-r--r--   0 runner    (1001) docker     (127)   353528 2024-05-09 08:52:54.000000 pyav-12.1.0rc2/src/av/descriptor.c
+-rw-r--r--   0 runner    (1001) docker     (127)   444866 2024-05-09 08:52:56.000000 pyav-12.1.0rc2/src/av/dictionary.c
+-rw-r--r--   0 runner    (1001) docker     (127)   867500 2024-05-09 08:52:54.000000 pyav-12.1.0rc2/src/av/enum.c
+-rw-r--r--   0 runner    (1001) docker     (127)   686509 2024-05-09 08:52:54.000000 pyav-12.1.0rc2/src/av/error.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.039927 pyav-12.1.0rc2/src/av/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)   523994 2024-05-09 08:53:03.000000 pyav-12.1.0rc2/src/av/filter/context.c
+-rw-r--r--   0 runner    (1001) docker     (127)   611535 2024-05-09 08:53:04.000000 pyav-12.1.0rc2/src/av/filter/filter.c
+-rw-r--r--   0 runner    (1001) docker     (127)   614694 2024-05-09 08:53:04.000000 pyav-12.1.0rc2/src/av/filter/graph.c
+-rw-r--r--   0 runner    (1001) docker     (127)   379619 2024-05-09 08:53:04.000000 pyav-12.1.0rc2/src/av/filter/link.c
+-rw-r--r--   0 runner    (1001) docker     (127)   414805 2024-05-09 08:53:04.000000 pyav-12.1.0rc2/src/av/filter/pad.c
+-rw-r--r--   0 runner    (1001) docker     (127)   479599 2024-05-09 08:52:56.000000 pyav-12.1.0rc2/src/av/format.c
+-rw-r--r--   0 runner    (1001) docker     (127)   435749 2024-05-09 08:52:56.000000 pyav-12.1.0rc2/src/av/frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)   563016 2024-05-09 08:52:55.000000 pyav-12.1.0rc2/src/av/logging.c
+-rw-r--r--   0 runner    (1001) docker     (127)   504998 2024-05-09 08:52:55.000000 pyav-12.1.0rc2/src/av/option.c
+-rw-r--r--   0 runner    (1001) docker     (127)   492390 2024-05-09 08:52:55.000000 pyav-12.1.0rc2/src/av/packet.c
+-rw-r--r--   0 runner    (1001) docker     (127)   362713 2024-05-09 08:52:55.000000 pyav-12.1.0rc2/src/av/plane.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.039927 pyav-12.1.0rc2/src/av/sidedata/
+-rw-r--r--   0 runner    (1001) docker     (127)   540636 2024-05-09 08:52:57.000000 pyav-12.1.0rc2/src/av/sidedata/motionvectors.c
+-rw-r--r--   0 runner    (1001) docker     (127)   556413 2024-05-09 08:52:57.000000 pyav-12.1.0rc2/src/av/sidedata/sidedata.c
+-rw-r--r--   0 runner    (1001) docker     (127)   494980 2024-05-09 08:52:56.000000 pyav-12.1.0rc2/src/av/stream.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.039927 pyav-12.1.0rc2/src/av/subtitles/
+-rw-r--r--   0 runner    (1001) docker     (127)   356177 2024-05-09 08:53:05.000000 pyav-12.1.0rc2/src/av/subtitles/codeccontext.c
+-rw-r--r--   0 runner    (1001) docker     (127)   341775 2024-05-09 08:53:05.000000 pyav-12.1.0rc2/src/av/subtitles/stream.c
+-rw-r--r--   0 runner    (1001) docker     (127)   822696 2024-05-09 08:53:05.000000 pyav-12.1.0rc2/src/av/subtitles/subtitle.c
+-rw-r--r--   0 runner    (1001) docker     (127)   265628 2024-05-09 08:52:56.000000 pyav-12.1.0rc2/src/av/utils.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.047927 pyav-12.1.0rc2/src/av/video/
+-rw-r--r--   0 runner    (1001) docker     (127)   595328 2024-05-09 08:53:00.000000 pyav-12.1.0rc2/src/av/video/codeccontext.c
+-rw-r--r--   0 runner    (1001) docker     (127)   613578 2024-05-09 08:52:59.000000 pyav-12.1.0rc2/src/av/video/format.c
+-rw-r--r--   0 runner    (1001) docker     (127)  1757212 2024-05-09 08:52:59.000000 pyav-12.1.0rc2/src/av/video/frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)   430748 2024-05-09 08:52:58.000000 pyav-12.1.0rc2/src/av/video/plane.c
+-rw-r--r--   0 runner    (1001) docker     (127)   480479 2024-05-09 08:53:00.000000 pyav-12.1.0rc2/src/av/video/reformatter.c
+-rw-r--r--   0 runner    (1001) docker     (127)   424135 2024-05-09 08:53:00.000000 pyav-12.1.0rc2/src/av/video/stream.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:06.051927 pyav-12.1.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_audiofifo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_audioformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8335 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_audioframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_audiolayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_audioresampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_bitstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17838 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_codec_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_containerformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_file_probing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_python_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_seek.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_videoformat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28349 2024-05-09 08:52:46.000000 pyav-12.1.0rc2/tests/test_videoframe.py
```

### Comparing `pyav-12.1.0rc1/LICENSE.txt` & `pyav-12.1.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/PKG-INFO` & `pyav-12.1.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyav
-Version: 12.1.0rc1
+Version: 12.1.0rc2
 Summary: Pythonic bindings for FFmpeg's libraries.
 Home-page: https://github.com/WyattBlue/pyav
 Author: WyattBlue
 Author-email: wyattblue@auto-editor.com
 License: BSD
 Project-URL: Bug Reports, https://github.com/WyattBlue/pyav/issues
 Project-URL: Documentation, https://pyav.basswood-io.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyav Version: 12.1.0rc1 Summary: Pythonic bindings
+Metadata-Version: 2.1 Name: pyav Version: 12.1.0rc2 Summary: Pythonic bindings
 for FFmpeg's libraries. Home-page: https://github.com/WyattBlue/pyav Author:
 WyattBlue Author-email: wyattblue@auto-editor.com License: BSD Project-URL: Bug
 Reports, https://github.com/WyattBlue/pyav/issues Project-URL: Documentation,
 https://pyav.basswood-io.com Project-URL: Download, https://pypi.org/project/
 pyav Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
 Multimedia :: Sound/Audio :: Conversion Classifier: Topic :: Multimedia ::
 Video Classifier: Topic :: Multimedia :: Video :: Conversion Classifier: Topic
```

### Comparing `pyav-12.1.0rc1/README.md` & `pyav-12.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/__init__.py` & `pyav-12.1.0rc2/av/__init__.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/__main__.py` & `pyav-12.1.0rc2/av/__main__.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/_core.pyx` & `pyav-12.1.0rc2/av/_core.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/codeccontext.pyx` & `pyav-12.1.0rc2/av/audio/codeccontext.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/fifo.pyx` & `pyav-12.1.0rc2/av/audio/fifo.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/format.pyx` & `pyav-12.1.0rc2/av/audio/format.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/frame.pxd` & `pyav-12.1.0rc2/av/audio/frame.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/frame.pyi` & `pyav-12.1.0rc2/av/audio/frame.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/frame.pyx` & `pyav-12.1.0rc2/av/audio/frame.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/layout.pyx` & `pyav-12.1.0rc2/av/audio/layout.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/resampler.pyi` & `pyav-12.1.0rc2/av/audio/resampler.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/resampler.pyx` & `pyav-12.1.0rc2/av/audio/resampler.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/stream.pyi` & `pyav-12.1.0rc2/av/audio/stream.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/audio/stream.pyx` & `pyav-12.1.0rc2/av/audio/stream.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/bitstream.pyx` & `pyav-12.1.0rc2/av/bitstream.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/buffer.pyx` & `pyav-12.1.0rc2/av/buffer.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/bytesource.pyx` & `pyav-12.1.0rc2/av/bytesource.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/codec/codec.pyi` & `pyav-12.1.0rc2/av/codec/codec.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/codec/codec.pyx` & `pyav-12.1.0rc2/av/codec/codec.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/codec/context.pxd` & `pyav-12.1.0rc2/av/codec/context.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/codec/context.pyi` & `pyav-12.1.0rc2/av/codec/context.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/codec/context.pyx` & `pyav-12.1.0rc2/av/codec/context.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/core.pxd` & `pyav-12.1.0rc2/av/container/core.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/core.pyi` & `pyav-12.1.0rc2/av/container/core.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/core.pyx` & `pyav-12.1.0rc2/av/container/core.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/input.pyi` & `pyav-12.1.0rc2/av/container/input.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/input.pyx` & `pyav-12.1.0rc2/av/container/input.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/output.pyi` & `pyav-12.1.0rc2/av/container/output.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/output.pyx` & `pyav-12.1.0rc2/av/container/output.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/pyio.pxd` & `pyav-12.1.0rc2/av/container/pyio.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/pyio.pyx` & `pyav-12.1.0rc2/av/container/pyio.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/streams.pyi` & `pyav-12.1.0rc2/av/container/streams.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/container/streams.pyx` & `pyav-12.1.0rc2/av/container/streams.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/datasets.py` & `pyav-12.1.0rc2/av/datasets.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/deprecation.py` & `pyav-12.1.0rc2/av/deprecation.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/descriptor.pxd` & `pyav-12.1.0rc2/av/descriptor.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/descriptor.pyx` & `pyav-12.1.0rc2/av/descriptor.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/dictionary.pyx` & `pyav-12.1.0rc2/av/dictionary.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/enum.pyi` & `pyav-12.1.0rc2/av/enum.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/enum.pyx` & `pyav-12.1.0rc2/av/enum.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/error.pyi` & `pyav-12.1.0rc2/av/error.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/error.pyx` & `pyav-12.1.0rc2/av/error.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/filter/context.pyx` & `pyav-12.1.0rc2/av/filter/context.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/filter/filter.pyx` & `pyav-12.1.0rc2/av/filter/filter.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/filter/graph.pyi` & `pyav-12.1.0rc2/av/filter/graph.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/filter/graph.pyx` & `pyav-12.1.0rc2/av/filter/graph.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/filter/link.pyx` & `pyav-12.1.0rc2/av/filter/link.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/filter/pad.pxd` & `pyav-12.1.0rc2/av/filter/pad.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/filter/pad.pyx` & `pyav-12.1.0rc2/av/filter/pad.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/format.pyi` & `pyav-12.1.0rc2/av/format.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/format.pyx` & `pyav-12.1.0rc2/av/format.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/frame.pyx` & `pyav-12.1.0rc2/av/frame.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/logging.pyi` & `pyav-12.1.0rc2/av/logging.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/logging.pyx` & `pyav-12.1.0rc2/av/logging.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/option.pyi` & `pyav-12.1.0rc2/av/option.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/option.pyx` & `pyav-12.1.0rc2/av/option.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/packet.pyi` & `pyav-12.1.0rc2/av/packet.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from collections.abc import Buffer
 from fractions import Fraction
-from typing import Iterator
 
 from av.subtitles.subtitle import SubtitleSet
 
 from .stream import Stream
 
 class Packet(Buffer):
     stream: Stream
@@ -18,9 +17,9 @@
     is_keyframe: bool
     is_corrupt: bool
     is_discard: bool
     is_trusted: bool
     is_disposable: bool
 
     def __init__(self, input: int | bytes | None = None) -> None: ...
-    def decode(self) -> Iterator[SubtitleSet]: ...
+    def decode(self) -> list[SubtitleSet]: ...
     def __buffer__(self, arg1) -> memoryview: ...
```

### Comparing `pyav-12.1.0rc1/av/packet.pyx` & `pyav-12.1.0rc2/av/packet.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,21 @@
         Returns `None` if it is not known.
 
         :type: int
         """
         if self.ptr.duration != lib.AV_NOPTS_VALUE:
             return self.ptr.duration
 
+    @duration.setter
+    def duration(self, v):
+        if v is None:
+            self.ptr.duration = lib.AV_NOPTS_VALUE
+        else:
+            self.ptr.duration = v
+
     @property
     def is_keyframe(self):
         return bool(self.ptr.flags & lib.AV_PKT_FLAG_KEY)
 
     @is_keyframe.setter
     def is_keyframe(self, v):
         if v:
```

### Comparing `pyav-12.1.0rc1/av/plane.pyx` & `pyav-12.1.0rc2/av/plane.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/sidedata/motionvectors.pyi` & `pyav-12.1.0rc2/av/sidedata/motionvectors.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/sidedata/motionvectors.pyx` & `pyav-12.1.0rc2/av/sidedata/motionvectors.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/sidedata/sidedata.pyi` & `pyav-12.1.0rc2/av/sidedata/sidedata.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/sidedata/sidedata.pyx` & `pyav-12.1.0rc2/av/sidedata/sidedata.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/stream.pxd` & `pyav-12.1.0rc2/av/stream.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/stream.pyi` & `pyav-12.1.0rc2/av/stream.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/stream.pyx` & `pyav-12.1.0rc2/av/stream.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/subtitles/codeccontext.pyx` & `pyav-12.1.0rc2/av/subtitles/codeccontext.pyx`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from av.packet cimport Packet
 from av.subtitles.subtitle cimport SubtitleProxy, SubtitleSet
 
 
 cdef class SubtitleCodecContext(CodecContext):
     cdef _send_packet_and_recv(self, Packet packet):
         cdef SubtitleProxy proxy = SubtitleProxy()
-
         cdef int got_frame = 0
-        err_check(lib.avcodec_decode_subtitle2(
-            self.ptr,
-            &proxy.struct,
-            &got_frame,
-            packet.ptr if packet else NULL))
+
+        err_check(
+            lib.avcodec_decode_subtitle2(
+                self.ptr, &proxy.struct, &got_frame, packet.ptr if packet else NULL
+            )
+        )
+
         if got_frame:
             return [SubtitleSet(proxy)]
         else:
             return []
```

### Comparing `pyav-12.1.0rc1/av/subtitles/subtitle.pxd` & `pyav-12.1.0rc2/av/subtitles/subtitle.pxd`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 cimport libav as lib
 
 from av.packet cimport Packet
 
 
 cdef class SubtitleProxy:
-
     cdef lib.AVSubtitle struct
 
 
 cdef class SubtitleSet:
-
     cdef readonly Packet packet
     cdef SubtitleProxy proxy
     cdef readonly tuple rects
 
 
 cdef class Subtitle:
-
     cdef SubtitleProxy proxy
     cdef lib.AVSubtitleRect *ptr
     cdef readonly bytes type
 
 cdef class TextSubtitle(Subtitle):
     pass
 
 cdef class ASSSubtitle(Subtitle):
     pass
 
 cdef class BitmapSubtitle(Subtitle):
-
     cdef readonly planes
 
 cdef class BitmapSubtitlePlane:
-
     cdef readonly BitmapSubtitle subtitle
     cdef readonly int index
     cdef readonly long buffer_size
     cdef void *_buffer
```

### Comparing `pyav-12.1.0rc1/av/subtitles/subtitle.pyi` & `pyav-12.1.0rc2/av/subtitles/subtitle.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Iterator, Literal
 
 class SubtitleSet:
     format: int
     start_display_time: int
     end_display_time: int
     pts: int
+    rects: tuple[Subtitle]
 
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[Subtitle]: ...
     def __getitem__(self, i: int) -> Subtitle: ...
 
 class Subtitle:
     type: Literal[b"none", b"bitmap", b"text", b"ass"]
@@ -25,12 +26,12 @@
 class BitmapSubtitlePlane:
     subtitle: BitmapSubtitle
     index: int
     buffer_size: int
 
 class TextSubtitle(Subtitle):
     type: Literal[b"text"]
-    text: str
+    text: bytes
 
 class AssSubtitle(Subtitle):
     type: Literal[b"ass"]
     ass: bytes
```

### Comparing `pyav-12.1.0rc1/av/subtitles/subtitle.pyx` & `pyav-12.1.0rc2/av/subtitles/subtitle.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -141,15 +141,17 @@
         return (
             f"<{self.__class__.__module__}.{self.__class__.__name__} "
             f"{self.text!r} at 0x{id(self):x}>"
         )
 
     @property
     def text(self):
-        return self.ptr.text
+        if self.ptr.text is not NULL:
+            return PyBytes_FromString(self.ptr.text)
+        return b""
 
 
 cdef class AssSubtitle(Subtitle):
     def __repr__(self):
         return (
             f"<{self.__class__.__module__}.{self.__class__.__name__} "
             f"{self.ass!r} at 0x{id(self):x}>"
```

### Comparing `pyav-12.1.0rc1/av/utils.pyx` & `pyav-12.1.0rc2/av/utils.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/codeccontext.pyi` & `pyav-12.1.0rc2/av/video/codeccontext.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/codeccontext.pyx` & `pyav-12.1.0rc2/av/video/codeccontext.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/format.pxd` & `pyav-12.1.0rc2/av/video/format.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/format.pyi` & `pyav-12.1.0rc2/av/video/format.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/format.pyx` & `pyav-12.1.0rc2/av/video/format.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/frame.pxd` & `pyav-12.1.0rc2/av/video/frame.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/frame.pyi` & `pyav-12.1.0rc2/av/video/frame.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/frame.pyx` & `pyav-12.1.0rc2/av/video/frame.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/plane.pyx` & `pyav-12.1.0rc2/av/video/plane.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/reformatter.pyi` & `pyav-12.1.0rc2/av/video/reformatter.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/reformatter.pyx` & `pyav-12.1.0rc2/av/video/reformatter.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/stream.pyi` & `pyav-12.1.0rc2/av/video/stream.pyi`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/av/video/stream.pyx` & `pyav-12.1.0rc2/av/video/stream.pyx`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libav.pxd` & `pyav-12.1.0rc2/include/libav.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavcodec/avcodec.pxd` & `pyav-12.1.0rc2/include/libavcodec/avcodec.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavcodec/bsf.pxd` & `pyav-12.1.0rc2/include/libavcodec/bsf.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavfilter/avfilter.pxd` & `pyav-12.1.0rc2/include/libavfilter/avfilter.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavfilter/avfiltergraph.pxd` & `pyav-12.1.0rc2/include/libavfilter/avfiltergraph.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavformat/avformat.pxd` & `pyav-12.1.0rc2/include/libavformat/avformat.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavutil/avutil.pxd` & `pyav-12.1.0rc2/include/libavutil/avutil.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavutil/dict.pxd` & `pyav-12.1.0rc2/include/libavutil/dict.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavutil/error.pxd` & `pyav-12.1.0rc2/include/libavutil/error.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavutil/frame.pxd` & `pyav-12.1.0rc2/include/libavutil/frame.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libavutil/samplefmt.pxd` & `pyav-12.1.0rc2/include/libavutil/samplefmt.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libswresample/swresample.pxd` & `pyav-12.1.0rc2/include/libswresample/swresample.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/include/libswscale/swscale.pxd` & `pyav-12.1.0rc2/include/libswscale/swscale.pxd`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/pyav.egg-info/PKG-INFO` & `pyav-12.1.0rc2/pyav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyav
-Version: 12.1.0rc1
+Version: 12.1.0rc2
 Summary: Pythonic bindings for FFmpeg's libraries.
 Home-page: https://github.com/WyattBlue/pyav
 Author: WyattBlue
 Author-email: wyattblue@auto-editor.com
 License: BSD
 Project-URL: Bug Reports, https://github.com/WyattBlue/pyav/issues
 Project-URL: Documentation, https://pyav.basswood-io.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyav Version: 12.1.0rc1 Summary: Pythonic bindings
+Metadata-Version: 2.1 Name: pyav Version: 12.1.0rc2 Summary: Pythonic bindings
 for FFmpeg's libraries. Home-page: https://github.com/WyattBlue/pyav Author:
 WyattBlue Author-email: wyattblue@auto-editor.com License: BSD Project-URL: Bug
 Reports, https://github.com/WyattBlue/pyav/issues Project-URL: Documentation,
 https://pyav.basswood-io.com Project-URL: Download, https://pypi.org/project/
 pyav Classifier: Topic :: Multimedia :: Sound/Audio Classifier: Topic ::
 Multimedia :: Sound/Audio :: Conversion Classifier: Topic :: Multimedia ::
 Video Classifier: Topic :: Multimedia :: Video :: Conversion Classifier: Topic
```

### Comparing `pyav-12.1.0rc1/pyav.egg-info/SOURCES.txt` & `pyav-12.1.0rc2/pyav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/setup.py` & `pyav-12.1.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/_core.c` & `pyav-12.1.0rc2/src/av/_core.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/audio/codeccontext.c` & `pyav-12.1.0rc2/src/av/audio/codeccontext.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/audio/fifo.c` & `pyav-12.1.0rc2/src/av/audio/fifo.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/audio/format.c` & `pyav-12.1.0rc2/src/av/audio/format.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/audio/frame.c` & `pyav-12.1.0rc2/src/av/audio/frame.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/audio/layout.c` & `pyav-12.1.0rc2/src/av/audio/layout.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/audio/plane.c` & `pyav-12.1.0rc2/src/av/audio/plane.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/audio/resampler.c` & `pyav-12.1.0rc2/src/av/audio/resampler.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/audio/stream.c` & `pyav-12.1.0rc2/src/av/audio/stream.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/bitstream.c` & `pyav-12.1.0rc2/src/av/bitstream.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/buffer.c` & `pyav-12.1.0rc2/src/av/buffer.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/bytesource.c` & `pyav-12.1.0rc2/src/av/bytesource.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/codec/codec.c` & `pyav-12.1.0rc2/src/av/codec/codec.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/codec/context.c` & `pyav-12.1.0rc2/src/av/codec/context.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/container/core.c` & `pyav-12.1.0rc2/src/av/container/core.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/container/input.c` & `pyav-12.1.0rc2/src/av/container/input.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/container/output.c` & `pyav-12.1.0rc2/src/av/container/output.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/container/pyio.c` & `pyav-12.1.0rc2/src/av/container/pyio.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/container/streams.c` & `pyav-12.1.0rc2/src/av/container/streams.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/data/stream.c` & `pyav-12.1.0rc2/src/av/data/stream.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/descriptor.c` & `pyav-12.1.0rc2/src/av/descriptor.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/dictionary.c` & `pyav-12.1.0rc2/src/av/dictionary.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/enum.c` & `pyav-12.1.0rc2/src/av/enum.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/error.c` & `pyav-12.1.0rc2/src/av/error.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/filter/context.c` & `pyav-12.1.0rc2/src/av/filter/context.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/filter/filter.c` & `pyav-12.1.0rc2/src/av/filter/filter.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/filter/graph.c` & `pyav-12.1.0rc2/src/av/filter/graph.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/filter/link.c` & `pyav-12.1.0rc2/src/av/filter/link.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/filter/pad.c` & `pyav-12.1.0rc2/src/av/filter/pad.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/format.c` & `pyav-12.1.0rc2/src/av/format.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/frame.c` & `pyav-12.1.0rc2/src/av/frame.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/logging.c` & `pyav-12.1.0rc2/src/av/logging.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/option.c` & `pyav-12.1.0rc2/src/av/option.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/packet.c` & `pyav-12.1.0rc2/src/av/packet.c`

 * *Files 1% similar despite different names*

```diff
@@ -2782,14 +2782,17 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *);
 
+/* CIntFromPy.proto */
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
+
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
 #define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
 #else
@@ -2801,17 +2804,14 @@
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
-
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 #define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
@@ -2953,14 +2953,15 @@
 static PyObject *__pyx_pf_2av_6packet_6Packet_3pts___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
 static int __pyx_pf_2av_6packet_6Packet_3pts_2__set__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self, PyObject *__pyx_v_v); /* proto */
 static PyObject *__pyx_pf_2av_6packet_6Packet_3dts___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
 static int __pyx_pf_2av_6packet_6Packet_3dts_2__set__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self, PyObject *__pyx_v_v); /* proto */
 static PyObject *__pyx_pf_2av_6packet_6Packet_3pos___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_6packet_6Packet_4size___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_6packet_6Packet_8duration___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
+static int __pyx_pf_2av_6packet_6Packet_8duration_2__set__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self, PyObject *__pyx_v_v); /* proto */
 static PyObject *__pyx_pf_2av_6packet_6Packet_11is_keyframe___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
 static int __pyx_pf_2av_6packet_6Packet_11is_keyframe_2__set__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self, PyObject *__pyx_v_v); /* proto */
 static PyObject *__pyx_pf_2av_6packet_6Packet_10is_corrupt___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
 static int __pyx_pf_2av_6packet_6Packet_10is_corrupt_2__set__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self, PyObject *__pyx_v_v); /* proto */
 static PyObject *__pyx_pf_2av_6packet_6Packet_10is_discard___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_6packet_6Packet_10is_trusted___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_6packet_6Packet_13is_disposable___get__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self); /* proto */
@@ -5420,15 +5421,15 @@
   if (__pyx_t_1) {
 
     /* "av/packet.pyx":178
  *         """
  *         if self.ptr.duration != lib.AV_NOPTS_VALUE:
  *             return self.ptr.duration             # <<<<<<<<<<<<<<
  * 
- *     @property
+ *     @duration.setter
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->duration); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
@@ -5462,14 +5463,105 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "av/packet.pyx":180
  *             return self.ptr.duration
  * 
+ *     @duration.setter             # <<<<<<<<<<<<<<
+ *     def duration(self, v):
+ *         if v is None:
+ */
+
+/* Python wrapper */
+static int __pyx_pw_2av_6packet_6Packet_8duration_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_v); /*proto*/
+static int __pyx_pw_2av_6packet_6Packet_8duration_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_v) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  __pyx_r = __pyx_pf_2av_6packet_6Packet_8duration_2__set__(((struct __pyx_obj_2av_6packet_Packet *)__pyx_v_self), ((PyObject *)__pyx_v_v));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_2av_6packet_6Packet_8duration_2__set__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self, PyObject *__pyx_v_v) {
+  int __pyx_r;
+  int __pyx_t_1;
+  int __pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+
+  /* "av/packet.pyx":182
+ *     @duration.setter
+ *     def duration(self, v):
+ *         if v is None:             # <<<<<<<<<<<<<<
+ *             self.ptr.duration = lib.AV_NOPTS_VALUE
+ *         else:
+ */
+  __pyx_t_1 = (__pyx_v_v == Py_None);
+  if (__pyx_t_1) {
+
+    /* "av/packet.pyx":183
+ *     def duration(self, v):
+ *         if v is None:
+ *             self.ptr.duration = lib.AV_NOPTS_VALUE             # <<<<<<<<<<<<<<
+ *         else:
+ *             self.ptr.duration = v
+ */
+    __pyx_v_self->ptr->duration = AV_NOPTS_VALUE;
+
+    /* "av/packet.pyx":182
+ *     @duration.setter
+ *     def duration(self, v):
+ *         if v is None:             # <<<<<<<<<<<<<<
+ *             self.ptr.duration = lib.AV_NOPTS_VALUE
+ *         else:
+ */
+    goto __pyx_L3;
+  }
+
+  /* "av/packet.pyx":185
+ *             self.ptr.duration = lib.AV_NOPTS_VALUE
+ *         else:
+ *             self.ptr.duration = v             # <<<<<<<<<<<<<<
+ * 
+ *     @property
+ */
+  /*else*/ {
+    __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_v_v); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_v_self->ptr->duration = __pyx_t_2;
+  }
+  __pyx_L3:;
+
+  /* "av/packet.pyx":180
+ *             return self.ptr.duration
+ * 
+ *     @duration.setter             # <<<<<<<<<<<<<<
+ *     def duration(self, v):
+ *         if v is None:
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("av.packet.Packet.duration.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "av/packet.pyx":187
+ *             self.ptr.duration = v
+ * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_keyframe(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_KEY)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_6packet_6Packet_11is_keyframe_1__get__(PyObject *__pyx_v_self); /*proto*/
@@ -5492,34 +5584,34 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "av/packet.pyx":182
+  /* "av/packet.pyx":189
  *     @property
  *     def is_keyframe(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_KEY)             # <<<<<<<<<<<<<<
  * 
  *     @is_keyframe.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_KEY)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_KEY)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/packet.pyx":180
- *             return self.ptr.duration
+  /* "av/packet.pyx":187
+ *             self.ptr.duration = v
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_keyframe(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_KEY)
  */
 
   /* function exit code */
@@ -5529,15 +5621,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/packet.pyx":184
+/* "av/packet.pyx":191
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_KEY)
  * 
  *     @is_keyframe.setter             # <<<<<<<<<<<<<<
  *     def is_keyframe(self, v):
  *         if v:
  */
 
@@ -5559,56 +5651,56 @@
 static int __pyx_pf_2av_6packet_6Packet_11is_keyframe_2__set__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self, PyObject *__pyx_v_v) {
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "av/packet.pyx":186
+  /* "av/packet.pyx":193
  *     @is_keyframe.setter
  *     def is_keyframe(self, v):
  *         if v:             # <<<<<<<<<<<<<<
  *             self.ptr.flags |= lib.AV_PKT_FLAG_KEY
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_v); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 186, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_v); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 193, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "av/packet.pyx":187
+    /* "av/packet.pyx":194
  *     def is_keyframe(self, v):
  *         if v:
  *             self.ptr.flags |= lib.AV_PKT_FLAG_KEY             # <<<<<<<<<<<<<<
  *         else:
  *             self.ptr.flags &= ~(lib.AV_PKT_FLAG_KEY)
  */
     __pyx_v_self->ptr->flags = (__pyx_v_self->ptr->flags | AV_PKT_FLAG_KEY);
 
-    /* "av/packet.pyx":186
+    /* "av/packet.pyx":193
  *     @is_keyframe.setter
  *     def is_keyframe(self, v):
  *         if v:             # <<<<<<<<<<<<<<
  *             self.ptr.flags |= lib.AV_PKT_FLAG_KEY
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "av/packet.pyx":189
+  /* "av/packet.pyx":196
  *             self.ptr.flags |= lib.AV_PKT_FLAG_KEY
  *         else:
  *             self.ptr.flags &= ~(lib.AV_PKT_FLAG_KEY)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
     __pyx_v_self->ptr->flags = (__pyx_v_self->ptr->flags & (~AV_PKT_FLAG_KEY));
   }
   __pyx_L3:;
 
-  /* "av/packet.pyx":184
+  /* "av/packet.pyx":191
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_KEY)
  * 
  *     @is_keyframe.setter             # <<<<<<<<<<<<<<
  *     def is_keyframe(self, v):
  *         if v:
  */
 
@@ -5618,15 +5710,15 @@
   __pyx_L1_error:;
   __Pyx_AddTraceback("av.packet.Packet.is_keyframe.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "av/packet.pyx":191
+/* "av/packet.pyx":198
  *             self.ptr.flags &= ~(lib.AV_PKT_FLAG_KEY)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_corrupt(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_CORRUPT)
  */
 
@@ -5651,33 +5743,33 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "av/packet.pyx":193
+  /* "av/packet.pyx":200
  *     @property
  *     def is_corrupt(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_CORRUPT)             # <<<<<<<<<<<<<<
  * 
  *     @is_corrupt.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_CORRUPT)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_CORRUPT)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/packet.pyx":191
+  /* "av/packet.pyx":198
  *             self.ptr.flags &= ~(lib.AV_PKT_FLAG_KEY)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_corrupt(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_CORRUPT)
  */
 
@@ -5688,15 +5780,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/packet.pyx":195
+/* "av/packet.pyx":202
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_CORRUPT)
  * 
  *     @is_corrupt.setter             # <<<<<<<<<<<<<<
  *     def is_corrupt(self, v):
  *         if v:
  */
 
@@ -5718,56 +5810,56 @@
 static int __pyx_pf_2av_6packet_6Packet_10is_corrupt_2__set__(struct __pyx_obj_2av_6packet_Packet *__pyx_v_self, PyObject *__pyx_v_v) {
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "av/packet.pyx":197
+  /* "av/packet.pyx":204
  *     @is_corrupt.setter
  *     def is_corrupt(self, v):
  *         if v:             # <<<<<<<<<<<<<<
  *             self.ptr.flags |= lib.AV_PKT_FLAG_CORRUPT
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_v); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_v); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 204, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "av/packet.pyx":198
+    /* "av/packet.pyx":205
  *     def is_corrupt(self, v):
  *         if v:
  *             self.ptr.flags |= lib.AV_PKT_FLAG_CORRUPT             # <<<<<<<<<<<<<<
  *         else:
  *             self.ptr.flags &= ~(lib.AV_PKT_FLAG_CORRUPT)
  */
     __pyx_v_self->ptr->flags = (__pyx_v_self->ptr->flags | AV_PKT_FLAG_CORRUPT);
 
-    /* "av/packet.pyx":197
+    /* "av/packet.pyx":204
  *     @is_corrupt.setter
  *     def is_corrupt(self, v):
  *         if v:             # <<<<<<<<<<<<<<
  *             self.ptr.flags |= lib.AV_PKT_FLAG_CORRUPT
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "av/packet.pyx":200
+  /* "av/packet.pyx":207
  *             self.ptr.flags |= lib.AV_PKT_FLAG_CORRUPT
  *         else:
  *             self.ptr.flags &= ~(lib.AV_PKT_FLAG_CORRUPT)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
     __pyx_v_self->ptr->flags = (__pyx_v_self->ptr->flags & (~AV_PKT_FLAG_CORRUPT));
   }
   __pyx_L3:;
 
-  /* "av/packet.pyx":195
+  /* "av/packet.pyx":202
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_CORRUPT)
  * 
  *     @is_corrupt.setter             # <<<<<<<<<<<<<<
  *     def is_corrupt(self, v):
  *         if v:
  */
 
@@ -5777,15 +5869,15 @@
   __pyx_L1_error:;
   __Pyx_AddTraceback("av.packet.Packet.is_corrupt.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "av/packet.pyx":202
+/* "av/packet.pyx":209
  *             self.ptr.flags &= ~(lib.AV_PKT_FLAG_CORRUPT)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_discard(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_DISCARD)
  */
 
@@ -5810,33 +5902,33 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "av/packet.pyx":204
+  /* "av/packet.pyx":211
  *     @property
  *     def is_discard(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_DISCARD)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_DISCARD)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_DISCARD)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/packet.pyx":202
+  /* "av/packet.pyx":209
  *             self.ptr.flags &= ~(lib.AV_PKT_FLAG_CORRUPT)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_discard(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_DISCARD)
  */
 
@@ -5847,15 +5939,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/packet.pyx":206
+/* "av/packet.pyx":213
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_DISCARD)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_trusted(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_TRUSTED)
  */
 
@@ -5880,33 +5972,33 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "av/packet.pyx":208
+  /* "av/packet.pyx":215
  *     @property
  *     def is_trusted(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_TRUSTED)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_TRUSTED)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_TRUSTED)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 208, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/packet.pyx":206
+  /* "av/packet.pyx":213
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_DISCARD)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_trusted(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_TRUSTED)
  */
 
@@ -5917,15 +6009,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/packet.pyx":210
+/* "av/packet.pyx":217
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_TRUSTED)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_disposable(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_DISPOSABLE)
  */
 
@@ -5950,32 +6042,32 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "av/packet.pyx":212
+  /* "av/packet.pyx":219
  *     @property
  *     def is_disposable(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_DISPOSABLE)             # <<<<<<<<<<<<<<
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_DISPOSABLE)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int((__pyx_v_self->ptr->flags & AV_PKT_FLAG_DISPOSABLE)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(!__pyx_t_2))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/packet.pyx":210
+  /* "av/packet.pyx":217
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_TRUSTED)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def is_disposable(self):
  *         return bool(self.ptr.flags & lib.AV_PKT_FLAG_DISPOSABLE)
  */
 
@@ -6344,14 +6436,24 @@
   return __pyx_pw_2av_6packet_6Packet_4size_1__get__(o);
 }
 
 static PyObject *__pyx_getprop_2av_6packet_6Packet_duration(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_2av_6packet_6Packet_8duration_1__get__(o);
 }
 
+static int __pyx_setprop_2av_6packet_6Packet_duration(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+  if (v) {
+    return __pyx_pw_2av_6packet_6Packet_8duration_3__set__(o, v);
+  }
+  else {
+    PyErr_SetString(PyExc_NotImplementedError, "__del__");
+    return -1;
+  }
+}
+
 static PyObject *__pyx_getprop_2av_6packet_6Packet_is_keyframe(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_2av_6packet_6Packet_11is_keyframe_1__get__(o);
 }
 
 static int __pyx_setprop_2av_6packet_6Packet_is_keyframe(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
   if (v) {
     return __pyx_pw_2av_6packet_6Packet_11is_keyframe_3__set__(o, v);
@@ -6404,15 +6506,15 @@
   {(char *)"stream_index", __pyx_getprop_2av_6packet_6Packet_stream_index, 0, (char *)0, 0},
   {(char *)"stream", __pyx_getprop_2av_6packet_6Packet_stream, __pyx_setprop_2av_6packet_6Packet_stream, (char *)PyDoc_STR("\n        The :class:`Stream` this packet was demuxed from.\n        "), 0},
   {(char *)"time_base", __pyx_getprop_2av_6packet_6Packet_time_base, __pyx_setprop_2av_6packet_6Packet_time_base, (char *)PyDoc_STR("\n        The unit of time (in fractional seconds) in which timestamps are expressed.\n\n        :type: fractions.Fraction\n        "), 0},
   {(char *)"pts", __pyx_getprop_2av_6packet_6Packet_pts, __pyx_setprop_2av_6packet_6Packet_pts, (char *)PyDoc_STR("\n        The presentation timestamp in :attr:`time_base` units for this packet.\n\n        This is the time at which the packet should be shown to the user.\n\n        :type: int\n        "), 0},
   {(char *)"dts", __pyx_getprop_2av_6packet_6Packet_dts, __pyx_setprop_2av_6packet_6Packet_dts, (char *)PyDoc_STR("\n        The decoding timestamp in :attr:`time_base` units for this packet.\n\n        :type: int\n        "), 0},
   {(char *)"pos", __pyx_getprop_2av_6packet_6Packet_pos, 0, (char *)PyDoc_STR("\n        The byte position of this packet within the :class:`.Stream`.\n\n        Returns `None` if it is not known.\n\n        :type: int\n        "), 0},
   {(char *)"size", __pyx_getprop_2av_6packet_6Packet_size, 0, (char *)PyDoc_STR("\n        The size in bytes of this packet's data.\n\n        :type: int\n        "), 0},
-  {(char *)"duration", __pyx_getprop_2av_6packet_6Packet_duration, 0, (char *)PyDoc_STR("\n        The duration in :attr:`time_base` units for this packet.\n\n        Returns `None` if it is not known.\n\n        :type: int\n        "), 0},
+  {(char *)"duration", __pyx_getprop_2av_6packet_6Packet_duration, __pyx_setprop_2av_6packet_6Packet_duration, (char *)PyDoc_STR("\n        The duration in :attr:`time_base` units for this packet.\n\n        Returns `None` if it is not known.\n\n        :type: int\n        "), 0},
   {(char *)"is_keyframe", __pyx_getprop_2av_6packet_6Packet_is_keyframe, __pyx_setprop_2av_6packet_6Packet_is_keyframe, (char *)0, 0},
   {(char *)"is_corrupt", __pyx_getprop_2av_6packet_6Packet_is_corrupt, __pyx_setprop_2av_6packet_6Packet_is_corrupt, (char *)0, 0},
   {(char *)"is_discard", __pyx_getprop_2av_6packet_6Packet_is_discard, 0, (char *)0, 0},
   {(char *)"is_trusted", __pyx_getprop_2av_6packet_6Packet_is_trusted, 0, (char *)0, 0},
   {(char *)"is_disposable", __pyx_getprop_2av_6packet_6Packet_is_disposable, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
@@ -11581,254 +11683,174 @@
     return (int64_t) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int64_t");
     return (int64_t) -1;
 }
 
-/* FormatTypeName */
-#if CYTHON_COMPILING_IN_LIMITED_API
-static __Pyx_TypeName
-__Pyx_PyType_GetName(PyTypeObject* tp)
-{
-    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
-                                               __pyx_n_s_name);
-    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
-        PyErr_Clear();
-        Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__9);
-    }
-    return name;
-}
-#endif
-
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-#else
-        PyObject *from_bytes, *result = NULL;
-        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
-        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
-        if (!from_bytes) return NULL;
-        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
-        if (!py_bytes) goto limited_bad;
-        order_str = PyUnicode_FromString(little ? "little" : "big");
-        if (!order_str) goto limited_bad;
-        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
-        if (!arg_tuple) goto limited_bad;
-        if (!is_unsigned) {
-            kwds = PyDict_New();
-            if (!kwds) goto limited_bad;
-            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
-        }
-        result = PyObject_Call(from_bytes, arg_tuple, kwds);
-        limited_bad:
-        Py_XDECREF(kwds);
-        Py_XDECREF(arg_tuple);
-        Py_XDECREF(order_str);
-        Py_XDECREF(py_bytes);
-        Py_XDECREF(from_bytes);
-        return result;
-#endif
-    }
-}
-
 /* CIntFromPy */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
+    const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(long) < sizeof(long))) {
-            __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
+        if ((sizeof(int) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (long) val;
+            return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (unlikely(__Pyx_PyLong_IsNeg(x))) {
                 goto raise_neg_overflow;
             } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_DigitCount(x)) {
                     case 2:
-                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
-                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
-                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
-                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                             }
                         }
                         break;
                 }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (long) -1;
+                    return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(long) <= sizeof(unsigned long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
+            if ((sizeof(int) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_SignedDigitCount(x)) {
                     case -2:
-                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case 2:
-                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case -3:
-                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case -4:
-                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                             }
                         }
                         break;
                 }
             }
 #endif
-            if ((sizeof(long) <= sizeof(long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
+            if ((sizeof(int) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-            long val;
+            int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
 #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -11847,261 +11869,341 @@
                 long idigit;
                 int chunk_size = (sizeof(long) < 8) ? 30 : 62;
                 if (unlikely(!PyLong_CheckExact(v))) {
                     PyObject *tmp = v;
                     v = PyNumber_Long(v);
                     assert(PyLong_CheckExact(v));
                     Py_DECREF(tmp);
-                    if (unlikely(!v)) return (long) -1;
+                    if (unlikely(!v)) return (int) -1;
                 }
 #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                 if (Py_SIZE(x) == 0)
-                    return (long) 0;
+                    return (int) 0;
                 is_negative = Py_SIZE(x) < 0;
 #else
                 {
                     int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                     if (unlikely(result < 0))
-                        return (long) -1;
+                        return (int) -1;
                     is_negative = result == 1;
                 }
 #endif
                 if (is_unsigned && unlikely(is_negative)) {
                     goto raise_neg_overflow;
                 } else if (is_negative) {
                     stepval = PyNumber_Invert(v);
                     if (unlikely(!stepval))
-                        return (long) -1;
+                        return (int) -1;
                 } else {
                     stepval = __Pyx_NewRef(v);
                 }
-                val = (long) 0;
+                val = (int) 0;
                 mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
                 shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
                     PyObject *tmp, *digit;
                     digit = PyNumber_And(stepval, mask);
                     if (unlikely(!digit)) goto done;
                     idigit = PyLong_AsLong(digit);
                     Py_DECREF(digit);
                     if (unlikely(idigit < 0)) goto done;
                     tmp = PyNumber_Rshift(stepval, shift);
                     if (unlikely(!tmp)) goto done;
                     Py_DECREF(stepval); stepval = tmp;
-                    val |= ((long) idigit) << bits;
+                    val |= ((int) idigit) << bits;
                     #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                     if (Py_SIZE(stepval) == 0)
                         goto unpacking_done;
                     #endif
                 }
                 idigit = PyLong_AsLong(stepval);
                 if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
                 if (unlikely(idigit >= (1L << remaining_bits)))
                     goto raise_overflow;
-                val |= ((long) idigit) << bits;
+                val |= ((int) idigit) << bits;
             #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
             unpacking_done:
             #endif
                 if (!is_unsigned) {
-                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
                         goto raise_overflow;
                     if (is_negative)
                         val = ~val;
                 }
                 ret = 0;
             done:
                 Py_XDECREF(shift);
                 Py_XDECREF(mask);
                 Py_XDECREF(stepval);
 #endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-            return (long) -1;
+            return (int) -1;
         }
     } else {
-        long val;
+        int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (long) -1;
-        val = __Pyx_PyInt_As_long(tmp);
+        if (!tmp) return (int) -1;
+        val = __Pyx_PyInt_As_int(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to long");
-    return (long) -1;
+        "value too large to convert to int");
+    return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to long");
-    return (long) -1;
+        "can't convert negative value to int");
+    return (int) -1;
+}
+
+/* FormatTypeName */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XDECREF(name);
+        name = __Pyx_NewRef(__pyx_n_s__9);
+    }
+    return name;
+}
+#endif
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030d0000
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyLong_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        if (!is_unsigned) {
+            kwds = PyDict_New();
+            if (!kwds) goto limited_bad;
+            if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(Py_True))) goto limited_bad;
+        }
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(kwds);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(order_str);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(from_bytes);
+        return result;
+#endif
+    }
 }
 
 /* CIntFromPy */
-static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
+    const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(int) < sizeof(long))) {
-            __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
+        if ((sizeof(long) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
-            return (int) val;
+            return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (unlikely(__Pyx_PyLong_IsNeg(x))) {
                 goto raise_neg_overflow;
             } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_DigitCount(x)) {
                     case 2:
-                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
-                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
-                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
-                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                             }
                         }
                         break;
                 }
             }
 #endif
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
-                    return (int) -1;
+                    return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(int) <= sizeof(unsigned long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
+            if ((sizeof(long) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
             if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
             } else {
                 const digit* digits = __Pyx_PyLong_Digits(x);
                 assert(__Pyx_PyLong_DigitCount(x) > 1);
                 switch (__Pyx_PyLong_SignedDigitCount(x)) {
                     case -2:
-                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case 2:
-                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case -3:
-                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case 3:
-                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case -4:
-                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                     case 4:
-                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
                             if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                             }
                         }
                         break;
                 }
             }
 #endif
-            if ((sizeof(int) <= sizeof(long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
+            if ((sizeof(long) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-            int val;
+            long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
 #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
@@ -12120,99 +12222,99 @@
                 long idigit;
                 int chunk_size = (sizeof(long) < 8) ? 30 : 62;
                 if (unlikely(!PyLong_CheckExact(v))) {
                     PyObject *tmp = v;
                     v = PyNumber_Long(v);
                     assert(PyLong_CheckExact(v));
                     Py_DECREF(tmp);
-                    if (unlikely(!v)) return (int) -1;
+                    if (unlikely(!v)) return (long) -1;
                 }
 #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                 if (Py_SIZE(x) == 0)
-                    return (int) 0;
+                    return (long) 0;
                 is_negative = Py_SIZE(x) < 0;
 #else
                 {
                     int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                     if (unlikely(result < 0))
-                        return (int) -1;
+                        return (long) -1;
                     is_negative = result == 1;
                 }
 #endif
                 if (is_unsigned && unlikely(is_negative)) {
                     goto raise_neg_overflow;
                 } else if (is_negative) {
                     stepval = PyNumber_Invert(v);
                     if (unlikely(!stepval))
-                        return (int) -1;
+                        return (long) -1;
                 } else {
                     stepval = __Pyx_NewRef(v);
                 }
-                val = (int) 0;
+                val = (long) 0;
                 mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
                 shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
                     PyObject *tmp, *digit;
                     digit = PyNumber_And(stepval, mask);
                     if (unlikely(!digit)) goto done;
                     idigit = PyLong_AsLong(digit);
                     Py_DECREF(digit);
                     if (unlikely(idigit < 0)) goto done;
                     tmp = PyNumber_Rshift(stepval, shift);
                     if (unlikely(!tmp)) goto done;
                     Py_DECREF(stepval); stepval = tmp;
-                    val |= ((int) idigit) << bits;
+                    val |= ((long) idigit) << bits;
                     #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
                     if (Py_SIZE(stepval) == 0)
                         goto unpacking_done;
                     #endif
                 }
                 idigit = PyLong_AsLong(stepval);
                 if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
                 if (unlikely(idigit >= (1L << remaining_bits)))
                     goto raise_overflow;
-                val |= ((int) idigit) << bits;
+                val |= ((long) idigit) << bits;
             #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
             unpacking_done:
             #endif
                 if (!is_unsigned) {
-                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
                         goto raise_overflow;
                     if (is_negative)
                         val = ~val;
                 }
                 ret = 0;
             done:
                 Py_XDECREF(shift);
                 Py_XDECREF(mask);
                 Py_XDECREF(stepval);
 #endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-            return (int) -1;
+            return (long) -1;
         }
     } else {
-        int val;
+        long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (int) -1;
-        val = __Pyx_PyInt_As_int(tmp);
+        if (!tmp) return (long) -1;
+        val = __Pyx_PyInt_As_long(tmp);
         Py_DECREF(tmp);
         return val;
     }
 raise_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to int");
-    return (int) -1;
+        "value too large to convert to long");
+    return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to int");
-    return (int) -1;
+        "can't convert negative value to long");
+    return (long) -1;
 }
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
```

### Comparing `pyav-12.1.0rc1/src/av/plane.c` & `pyav-12.1.0rc2/src/av/plane.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/sidedata/motionvectors.c` & `pyav-12.1.0rc2/src/av/sidedata/motionvectors.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/sidedata/sidedata.c` & `pyav-12.1.0rc2/src/av/sidedata/sidedata.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/stream.c` & `pyav-12.1.0rc2/src/av/stream.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/subtitles/codeccontext.c` & `pyav-12.1.0rc2/src/av/subtitles/codeccontext.c`

 * *Files 0% similar despite different names*

```diff
@@ -2002,96 +2002,96 @@
 };
 
 
 /* "av/subtitles/subtitle.pxd":6
  * 
  * 
  * cdef class SubtitleProxy:             # <<<<<<<<<<<<<<
- * 
  *     cdef lib.AVSubtitle struct
+ * 
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy {
   PyObject_HEAD
   struct AVSubtitle __pyx_struct;
 };
 
 
-/* "av/subtitles/subtitle.pxd":11
+/* "av/subtitles/subtitle.pxd":10
  * 
  * 
  * cdef class SubtitleSet:             # <<<<<<<<<<<<<<
- * 
  *     cdef readonly Packet packet
+ *     cdef SubtitleProxy proxy
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleSet {
   PyObject_HEAD
   struct __pyx_obj_2av_6packet_Packet *packet;
   struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy *proxy;
   PyObject *rects;
 };
 
 
-/* "av/subtitles/subtitle.pxd":18
+/* "av/subtitles/subtitle.pxd":16
  * 
  * 
  * cdef class Subtitle:             # <<<<<<<<<<<<<<
- * 
  *     cdef SubtitleProxy proxy
+ *     cdef lib.AVSubtitleRect *ptr
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle {
   PyObject_HEAD
   struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy *proxy;
   struct AVSubtitleRect *ptr;
   PyObject *type;
 };
 
 
-/* "av/subtitles/subtitle.pxd":24
+/* "av/subtitles/subtitle.pxd":21
  *     cdef readonly bytes type
  * 
  * cdef class TextSubtitle(Subtitle):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_TextSubtitle {
   struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle __pyx_base;
 };
 
 
-/* "av/subtitles/subtitle.pxd":27
+/* "av/subtitles/subtitle.pxd":24
  *     pass
  * 
  * cdef class ASSSubtitle(Subtitle):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_ASSSubtitle {
   struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle __pyx_base;
 };
 
 
-/* "av/subtitles/subtitle.pxd":30
+/* "av/subtitles/subtitle.pxd":27
  *     pass
  * 
  * cdef class BitmapSubtitle(Subtitle):             # <<<<<<<<<<<<<<
- * 
  *     cdef readonly planes
+ * 
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitle {
   struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle __pyx_base;
   PyObject *planes;
 };
 
 
-/* "av/subtitles/subtitle.pxd":34
+/* "av/subtitles/subtitle.pxd":30
  *     cdef readonly planes
  * 
  * cdef class BitmapSubtitlePlane:             # <<<<<<<<<<<<<<
- * 
  *     cdef readonly BitmapSubtitle subtitle
+ *     cdef readonly int index
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitlePlane {
   PyObject_HEAD
   struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitle *subtitle;
   int index;
   long buffer_size;
   void *_buffer;
@@ -3393,15 +3393,15 @@
 /* #### Code section: module_code ### */
 
 /* "av/subtitles/codeccontext.pyx":9
  * 
  * cdef class SubtitleCodecContext(CodecContext):
  *     cdef _send_packet_and_recv(self, Packet packet):             # <<<<<<<<<<<<<<
  *         cdef SubtitleProxy proxy = SubtitleProxy()
- * 
+ *         cdef int got_frame = 0
  */
 
 static PyObject *__pyx_f_2av_9subtitles_12codeccontext_20SubtitleCodecContext__send_packet_and_recv(struct __pyx_obj_2av_9subtitles_12codeccontext_SubtitleCodecContext *__pyx_v_self, struct __pyx_obj_2av_6packet_Packet *__pyx_v_packet) {
   struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy *__pyx_v_proxy = 0;
   int __pyx_v_got_frame;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -3415,112 +3415,112 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_send_packet_and_recv", 1);
 
   /* "av/subtitles/codeccontext.pyx":10
  * cdef class SubtitleCodecContext(CodecContext):
  *     cdef _send_packet_and_recv(self, Packet packet):
  *         cdef SubtitleProxy proxy = SubtitleProxy()             # <<<<<<<<<<<<<<
- * 
  *         cdef int got_frame = 0
+ * 
  */
   __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2av_9subtitles_8subtitle_SubtitleProxy)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_proxy = ((struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/subtitles/codeccontext.pyx":12
+  /* "av/subtitles/codeccontext.pyx":11
+ *     cdef _send_packet_and_recv(self, Packet packet):
  *         cdef SubtitleProxy proxy = SubtitleProxy()
- * 
  *         cdef int got_frame = 0             # <<<<<<<<<<<<<<
- *         err_check(lib.avcodec_decode_subtitle2(
- *             self.ptr,
+ * 
+ *         err_check(
  */
   __pyx_v_got_frame = 0;
 
-  /* "av/subtitles/codeccontext.pyx":17
- *             &proxy.struct,
- *             &got_frame,
- *             packet.ptr if packet else NULL))             # <<<<<<<<<<<<<<
- *         if got_frame:
- *             return [SubtitleSet(proxy)]
+  /* "av/subtitles/codeccontext.pyx":15
+ *         err_check(
+ *             lib.avcodec_decode_subtitle2(
+ *                 self.ptr, &proxy.struct, &got_frame, packet.ptr if packet else NULL             # <<<<<<<<<<<<<<
+ *             )
+ *         )
  */
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_packet)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_packet)); if (unlikely((__pyx_t_3 < 0))) __PYX_ERR(1, 15, __pyx_L1_error)
   if (__pyx_t_3) {
     __pyx_t_2 = __pyx_v_packet->ptr;
   } else {
     __pyx_t_2 = NULL;
   }
 
   /* "av/subtitles/codeccontext.pyx":13
- * 
  *         cdef int got_frame = 0
- *         err_check(lib.avcodec_decode_subtitle2(             # <<<<<<<<<<<<<<
- *             self.ptr,
- *             &proxy.struct,
+ * 
+ *         err_check(             # <<<<<<<<<<<<<<
+ *             lib.avcodec_decode_subtitle2(
+ *                 self.ptr, &proxy.struct, &got_frame, packet.ptr if packet else NULL
  */
   __pyx_t_4 = __pyx_f_2av_5error_err_check(avcodec_decode_subtitle2(__pyx_v_self->__pyx_base.ptr, (&__pyx_v_proxy->__pyx_struct), (&__pyx_v_got_frame), __pyx_t_2), 0, NULL); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
 
-  /* "av/subtitles/codeccontext.pyx":18
- *             &got_frame,
- *             packet.ptr if packet else NULL))
+  /* "av/subtitles/codeccontext.pyx":19
+ *         )
+ * 
  *         if got_frame:             # <<<<<<<<<<<<<<
  *             return [SubtitleSet(proxy)]
  *         else:
  */
   __pyx_t_3 = (__pyx_v_got_frame != 0);
   if (__pyx_t_3) {
 
-    /* "av/subtitles/codeccontext.pyx":19
- *             packet.ptr if packet else NULL))
+    /* "av/subtitles/codeccontext.pyx":20
+ * 
  *         if got_frame:
  *             return [SubtitleSet(proxy)]             # <<<<<<<<<<<<<<
  *         else:
  *             return []
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2av_9subtitles_8subtitle_SubtitleSet), ((PyObject *)__pyx_v_proxy)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 19, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2av_9subtitles_8subtitle_SubtitleSet), ((PyObject *)__pyx_v_proxy)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 20, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 19, __pyx_L1_error)
+    __pyx_t_5 = PyList_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 20, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(1, 19, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(1, 20, __pyx_L1_error);
     __pyx_t_1 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "av/subtitles/codeccontext.pyx":18
- *             &got_frame,
- *             packet.ptr if packet else NULL))
+    /* "av/subtitles/codeccontext.pyx":19
+ *         )
+ * 
  *         if got_frame:             # <<<<<<<<<<<<<<
  *             return [SubtitleSet(proxy)]
  *         else:
  */
   }
 
-  /* "av/subtitles/codeccontext.pyx":21
+  /* "av/subtitles/codeccontext.pyx":22
  *             return [SubtitleSet(proxy)]
  *         else:
  *             return []             # <<<<<<<<<<<<<<
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 21, __pyx_L1_error)
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 22, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
   }
 
   /* "av/subtitles/codeccontext.pyx":9
  * 
  * cdef class SubtitleCodecContext(CodecContext):
  *     cdef _send_packet_and_recv(self, Packet packet):             # <<<<<<<<<<<<<<
  *         cdef SubtitleProxy proxy = SubtitleProxy()
- * 
+ *         cdef int got_frame = 0
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("av.subtitles.codeccontext.SubtitleCodecContext._send_packet_and_recv", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -4130,20 +4130,20 @@
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5frame_Frame = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.frame", "Frame", sizeof(struct __pyx_obj_2av_5frame_Frame), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_5frame_Frame),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_5frame_Frame) __PYX_ERR(13, 7, __pyx_L1_error)
   __pyx_vtabptr_2av_5frame_Frame = (struct __pyx_vtabstruct_2av_5frame_Frame*)__Pyx_GetVtable(__pyx_ptype_2av_5frame_Frame); if (unlikely(!__pyx_vtabptr_2av_5frame_Frame)) __PYX_ERR(13, 7, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.subtitles.subtitle"); if (unlikely(!__pyx_t_1)) __PYX_ERR(14, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9subtitles_8subtitle_SubtitleProxy = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "SubtitleProxy", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_SubtitleProxy) __PYX_ERR(14, 6, __pyx_L1_error)
-  __pyx_ptype_2av_9subtitles_8subtitle_SubtitleSet = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "SubtitleSet", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleSet), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleSet),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_SubtitleSet) __PYX_ERR(14, 11, __pyx_L1_error)
-  __pyx_ptype_2av_9subtitles_8subtitle_Subtitle = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "Subtitle", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_Subtitle) __PYX_ERR(14, 18, __pyx_L1_error)
-  __pyx_ptype_2av_9subtitles_8subtitle_TextSubtitle = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "TextSubtitle", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_TextSubtitle), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_TextSubtitle),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_TextSubtitle) __PYX_ERR(14, 24, __pyx_L1_error)
-  __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "ASSSubtitle", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_ASSSubtitle), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_ASSSubtitle),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle) __PYX_ERR(14, 27, __pyx_L1_error)
-  __pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitle = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "BitmapSubtitle", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitle), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitle),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitle) __PYX_ERR(14, 30, __pyx_L1_error)
-  __pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitlePlane = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "BitmapSubtitlePlane", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitlePlane), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitlePlane),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitlePlane) __PYX_ERR(14, 34, __pyx_L1_error)
+  __pyx_ptype_2av_9subtitles_8subtitle_SubtitleSet = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "SubtitleSet", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleSet), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleSet),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_SubtitleSet) __PYX_ERR(14, 10, __pyx_L1_error)
+  __pyx_ptype_2av_9subtitles_8subtitle_Subtitle = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "Subtitle", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_Subtitle) __PYX_ERR(14, 16, __pyx_L1_error)
+  __pyx_ptype_2av_9subtitles_8subtitle_TextSubtitle = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "TextSubtitle", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_TextSubtitle), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_TextSubtitle),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_TextSubtitle) __PYX_ERR(14, 21, __pyx_L1_error)
+  __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "ASSSubtitle", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_ASSSubtitle), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_ASSSubtitle),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle) __PYX_ERR(14, 24, __pyx_L1_error)
+  __pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitle = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "BitmapSubtitle", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitle), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitle),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitle) __PYX_ERR(14, 27, __pyx_L1_error)
+  __pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitlePlane = __Pyx_ImportType_3_0_10(__pyx_t_1, "av.subtitles.subtitle", "BitmapSubtitlePlane", sizeof(struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitlePlane), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitlePlane),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitlePlane) __PYX_ERR(14, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `pyav-12.1.0rc1/src/av/subtitles/stream.c` & `pyav-12.1.0rc2/src/av/subtitles/stream.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/subtitles/subtitle.c` & `pyav-12.1.0rc2/src/av/subtitles/subtitle.c`

 * *Files 0% similar despite different names*

```diff
@@ -2022,107 +2022,107 @@
 };
 
 
 /* "av/subtitles/subtitle.pxd":6
  * 
  * 
  * cdef class SubtitleProxy:             # <<<<<<<<<<<<<<
- * 
  *     cdef lib.AVSubtitle struct
+ * 
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy {
   PyObject_HEAD
   struct AVSubtitle __pyx_struct;
 };
 
 
-/* "av/subtitles/subtitle.pxd":11
+/* "av/subtitles/subtitle.pxd":10
  * 
  * 
  * cdef class SubtitleSet:             # <<<<<<<<<<<<<<
- * 
  *     cdef readonly Packet packet
+ *     cdef SubtitleProxy proxy
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleSet {
   PyObject_HEAD
   struct __pyx_obj_2av_6packet_Packet *packet;
   struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy *proxy;
   PyObject *rects;
 };
 
 
-/* "av/subtitles/subtitle.pxd":18
+/* "av/subtitles/subtitle.pxd":16
  * 
  * 
  * cdef class Subtitle:             # <<<<<<<<<<<<<<
- * 
  *     cdef SubtitleProxy proxy
+ *     cdef lib.AVSubtitleRect *ptr
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle {
   PyObject_HEAD
   struct __pyx_obj_2av_9subtitles_8subtitle_SubtitleProxy *proxy;
   struct AVSubtitleRect *ptr;
   PyObject *type;
 };
 
 
-/* "av/subtitles/subtitle.pxd":24
+/* "av/subtitles/subtitle.pxd":21
  *     cdef readonly bytes type
  * 
  * cdef class TextSubtitle(Subtitle):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_TextSubtitle {
   struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle __pyx_base;
 };
 
 
-/* "av/subtitles/subtitle.pxd":27
+/* "av/subtitles/subtitle.pxd":24
  *     pass
  * 
  * cdef class ASSSubtitle(Subtitle):             # <<<<<<<<<<<<<<
  *     pass
  * 
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_ASSSubtitle {
   struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle __pyx_base;
 };
 
 
-/* "av/subtitles/subtitle.pxd":30
+/* "av/subtitles/subtitle.pxd":27
  *     pass
  * 
  * cdef class BitmapSubtitle(Subtitle):             # <<<<<<<<<<<<<<
- * 
  *     cdef readonly planes
+ * 
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitle {
   struct __pyx_obj_2av_9subtitles_8subtitle_Subtitle __pyx_base;
   PyObject *planes;
 };
 
 
-/* "av/subtitles/subtitle.pxd":34
+/* "av/subtitles/subtitle.pxd":30
  *     cdef readonly planes
  * 
  * cdef class BitmapSubtitlePlane:             # <<<<<<<<<<<<<<
- * 
  *     cdef readonly BitmapSubtitle subtitle
+ *     cdef readonly int index
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitlePlane {
   PyObject_HEAD
   struct __pyx_obj_2av_9subtitles_8subtitle_BitmapSubtitle *subtitle;
   int index;
   long buffer_size;
   void *_buffer;
 };
 
 
-/* "av/subtitles/subtitle.pyx":151
+/* "av/subtitles/subtitle.pyx":153
  * 
  * 
  * cdef class AssSubtitle(Subtitle):             # <<<<<<<<<<<<<<
  *     def __repr__(self):
  *         return (
  */
 struct __pyx_obj_2av_9subtitles_8subtitle_AssSubtitle {
@@ -5820,17 +5820,17 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/subtitles/subtitle.pxd":13
- * cdef class SubtitleSet:
+/* "av/subtitles/subtitle.pxd":11
  * 
+ * cdef class SubtitleSet:
  *     cdef readonly Packet packet             # <<<<<<<<<<<<<<
  *     cdef SubtitleProxy proxy
  *     cdef readonly tuple rects
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_9subtitles_8subtitle_11SubtitleSet_6packet_1__get__(PyObject *__pyx_v_self); /*proto*/
@@ -5859,15 +5859,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/subtitles/subtitle.pxd":15
+/* "av/subtitles/subtitle.pxd":13
  *     cdef readonly Packet packet
  *     cdef SubtitleProxy proxy
  *     cdef readonly tuple rects             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
@@ -6830,15 +6830,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/subtitles/subtitle.pxd":22
+/* "av/subtitles/subtitle.pxd":19
  *     cdef SubtitleProxy proxy
  *     cdef lib.AVSubtitleRect *ptr
  *     cdef readonly bytes type             # <<<<<<<<<<<<<<
  * 
  * cdef class TextSubtitle(Subtitle):
  */
 
@@ -8165,17 +8165,17 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/subtitles/subtitle.pxd":32
- * cdef class BitmapSubtitle(Subtitle):
+/* "av/subtitles/subtitle.pxd":28
  * 
+ * cdef class BitmapSubtitle(Subtitle):
  *     cdef readonly planes             # <<<<<<<<<<<<<<
  * 
  * cdef class BitmapSubtitlePlane:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_9subtitles_8subtitle_14BitmapSubtitle_6planes_1__get__(PyObject *__pyx_v_self); /*proto*/
@@ -8737,17 +8737,17 @@
     __Pyx_DECREF(__pyx_v_view->obj); __pyx_v_view->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/subtitles/subtitle.pxd":36
- * cdef class BitmapSubtitlePlane:
+/* "av/subtitles/subtitle.pxd":31
  * 
+ * cdef class BitmapSubtitlePlane:
  *     cdef readonly BitmapSubtitle subtitle             # <<<<<<<<<<<<<<
  *     cdef readonly int index
  *     cdef readonly long buffer_size
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_9subtitles_8subtitle_19BitmapSubtitlePlane_8subtitle_1__get__(PyObject *__pyx_v_self); /*proto*/
@@ -8776,16 +8776,16 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/subtitles/subtitle.pxd":37
- * 
+/* "av/subtitles/subtitle.pxd":32
+ * cdef class BitmapSubtitlePlane:
  *     cdef readonly BitmapSubtitle subtitle
  *     cdef readonly int index             # <<<<<<<<<<<<<<
  *     cdef readonly long buffer_size
  *     cdef void *_buffer
  */
 
 /* Python wrapper */
@@ -8808,15 +8808,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->index); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 37, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->index); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 32, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8825,15 +8825,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/subtitles/subtitle.pxd":38
+/* "av/subtitles/subtitle.pxd":33
  *     cdef readonly BitmapSubtitle subtitle
  *     cdef readonly int index
  *     cdef readonly long buffer_size             # <<<<<<<<<<<<<<
  *     cdef void *_buffer
  */
 
 /* Python wrapper */
@@ -8856,15 +8856,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 38, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_self->buffer_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9260,15 +9260,15 @@
 }
 
 /* "av/subtitles/subtitle.pyx":146
  *         )
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def text(self):
- *         return self.ptr.text
+ *         if self.ptr.text is not NULL:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_9subtitles_8subtitle_12TextSubtitle_4text_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_2av_9subtitles_8subtitle_12TextSubtitle_4text_1__get__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
@@ -9281,45 +9281,77 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_2av_9subtitles_8subtitle_12TextSubtitle_4text___get__(struct __pyx_obj_2av_9subtitles_8subtitle_TextSubtitle *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "av/subtitles/subtitle.pyx":148
  *     @property
  *     def text(self):
- *         return self.ptr.text             # <<<<<<<<<<<<<<
+ *         if self.ptr.text is not NULL:             # <<<<<<<<<<<<<<
+ *             return PyBytes_FromString(self.ptr.text)
+ *         return b""
+ */
+  __pyx_t_1 = (__pyx_v_self->__pyx_base.ptr->text != NULL);
+  if (__pyx_t_1) {
+
+    /* "av/subtitles/subtitle.pyx":149
+ *     def text(self):
+ *         if self.ptr.text is not NULL:
+ *             return PyBytes_FromString(self.ptr.text)             # <<<<<<<<<<<<<<
+ *         return b""
+ * 
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_2 = PyBytes_FromString(__pyx_v_self->__pyx_base.ptr->text); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 149, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_r = __pyx_t_2;
+    __pyx_t_2 = 0;
+    goto __pyx_L0;
+
+    /* "av/subtitles/subtitle.pyx":148
+ *     @property
+ *     def text(self):
+ *         if self.ptr.text is not NULL:             # <<<<<<<<<<<<<<
+ *             return PyBytes_FromString(self.ptr.text)
+ *         return b""
+ */
+  }
+
+  /* "av/subtitles/subtitle.pyx":150
+ *         if self.ptr.text is not NULL:
+ *             return PyBytes_FromString(self.ptr.text)
+ *         return b""             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyStr_FromString(__pyx_v_self->__pyx_base.ptr->text); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 148, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __Pyx_INCREF(__pyx_kp_b__9);
+  __pyx_r = __pyx_kp_b__9;
   goto __pyx_L0;
 
   /* "av/subtitles/subtitle.pyx":146
  *         )
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def text(self):
- *         return self.ptr.text
+ *         if self.ptr.text is not NULL:
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("av.subtitles.subtitle.TextSubtitle.text.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9536,15 +9568,15 @@
   __Pyx_AddTraceback("av.subtitles.subtitle.TextSubtitle.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/subtitles/subtitle.pyx":152
+/* "av/subtitles/subtitle.pyx":154
  * 
  * cdef class AssSubtitle(Subtitle):
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return (
  *             f"<{self.__class__.__module__}.{self.__class__.__name__} "
  */
 
@@ -9572,124 +9604,124 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 1);
 
-  /* "av/subtitles/subtitle.pyx":153
+  /* "av/subtitles/subtitle.pyx":155
  * cdef class AssSubtitle(Subtitle):
  *     def __repr__(self):
  *         return (             # <<<<<<<<<<<<<<
  *             f"<{self.__class__.__module__}.{self.__class__.__name__} "
  *             f"{self.ass!r} at 0x{id(self):x}>"
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "av/subtitles/subtitle.pyx":154
+  /* "av/subtitles/subtitle.pyx":156
  *     def __repr__(self):
  *         return (
  *             f"<{self.__class__.__module__}.{self.__class__.__name__} "             # <<<<<<<<<<<<<<
  *             f"{self.ass!r} at 0x{id(self):x}>"
  *         )
  */
-  __pyx_t_1 = PyTuple_New(9); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(9); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
   __Pyx_INCREF(__pyx_kp_u_);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u_);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_module); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_module); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__2);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__2);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__2);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__5);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__5);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__5);
 
-  /* "av/subtitles/subtitle.pyx":155
+  /* "av/subtitles/subtitle.pyx":157
  *         return (
  *             f"<{self.__class__.__module__}.{self.__class__.__name__} "
  *             f"{self.ass!r} at 0x{id(self):x}>"             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_ass); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 155, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_ass); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 157, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(__pyx_t_4), __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 155, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(__pyx_t_4), __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 157, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_INCREF(__pyx_kp_u_at_0x);
   __pyx_t_2 += 6;
   __Pyx_GIVEREF(__pyx_kp_u_at_0x);
   PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_kp_u_at_0x);
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 155, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 157, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_Format(__pyx_t_5, __pyx_n_u_x); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 155, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Format(__pyx_t_5, __pyx_n_u_x); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 157, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 7, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__3);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__3);
   PyTuple_SET_ITEM(__pyx_t_1, 8, __pyx_kp_u__3);
 
-  /* "av/subtitles/subtitle.pyx":154
+  /* "av/subtitles/subtitle.pyx":156
  *     def __repr__(self):
  *         return (
  *             f"<{self.__class__.__module__}.{self.__class__.__name__} "             # <<<<<<<<<<<<<<
  *             f"{self.ass!r} at 0x{id(self):x}>"
  *         )
  */
-  __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 9, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 154, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 9, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 156, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "av/subtitles/subtitle.pyx":152
+  /* "av/subtitles/subtitle.pyx":154
  * 
  * cdef class AssSubtitle(Subtitle):
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return (
  *             f"<{self.__class__.__module__}.{self.__class__.__name__} "
  */
 
@@ -9702,15 +9734,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/subtitles/subtitle.pyx":158
+/* "av/subtitles/subtitle.pyx":160
  *         )
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def ass(self):
  *         if self.ptr.ass is not NULL:
  */
 
@@ -9735,57 +9767,57 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
 
-  /* "av/subtitles/subtitle.pyx":160
+  /* "av/subtitles/subtitle.pyx":162
  *     @property
  *     def ass(self):
  *         if self.ptr.ass is not NULL:             # <<<<<<<<<<<<<<
  *             return PyBytes_FromString(self.ptr.ass)
  *         return b""
  */
   __pyx_t_1 = (__pyx_v_self->__pyx_base.ptr->ass != NULL);
   if (__pyx_t_1) {
 
-    /* "av/subtitles/subtitle.pyx":161
+    /* "av/subtitles/subtitle.pyx":163
  *     def ass(self):
  *         if self.ptr.ass is not NULL:
  *             return PyBytes_FromString(self.ptr.ass)             # <<<<<<<<<<<<<<
  *         return b""
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = PyBytes_FromString(__pyx_v_self->__pyx_base.ptr->ass); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 161, __pyx_L1_error)
+    __pyx_t_2 = PyBytes_FromString(__pyx_v_self->__pyx_base.ptr->ass); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 163, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "av/subtitles/subtitle.pyx":160
+    /* "av/subtitles/subtitle.pyx":162
  *     @property
  *     def ass(self):
  *         if self.ptr.ass is not NULL:             # <<<<<<<<<<<<<<
  *             return PyBytes_FromString(self.ptr.ass)
  *         return b""
  */
   }
 
-  /* "av/subtitles/subtitle.pyx":162
+  /* "av/subtitles/subtitle.pyx":164
  *         if self.ptr.ass is not NULL:
  *             return PyBytes_FromString(self.ptr.ass)
  *         return b""             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_kp_b__9);
   __pyx_r = __pyx_kp_b__9;
   goto __pyx_L0;
 
-  /* "av/subtitles/subtitle.pyx":158
+  /* "av/subtitles/subtitle.pyx":160
  *         )
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def ass(self):
  *         if self.ptr.ass is not NULL:
  */
 
@@ -12478,38 +12510,38 @@
   }
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_TextSubtitle, (PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_TextSubtitle) < 0) __PYX_ERR(1, 139, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_TextSubtitle) < 0) __PYX_ERR(1, 139, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2av_9subtitles_8subtitle_Subtitle); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 27, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2av_9subtitles_8subtitle_Subtitle); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2av_9subtitles_8subtitle_ASSSubtitle_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle)) __PYX_ERR(3, 27, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2av_9subtitles_8subtitle_ASSSubtitle_spec, __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle) < 0) __PYX_ERR(3, 27, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle)) __PYX_ERR(3, 24, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2av_9subtitles_8subtitle_ASSSubtitle_spec, __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle) < 0) __PYX_ERR(3, 24, __pyx_L1_error)
   #else
   __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle = &__pyx_type_2av_9subtitles_8subtitle_ASSSubtitle;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle->tp_base = __pyx_ptype_2av_9subtitles_8subtitle_Subtitle;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle) < 0) __PYX_ERR(3, 27, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle) < 0) __PYX_ERR(3, 24, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle->tp_dictoffset && __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ASSSubtitle, (PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle) < 0) __PYX_ERR(3, 27, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_ASSSubtitle, (PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_ASSSubtitle) < 0) __PYX_ERR(3, 24, __pyx_L1_error)
   #if CYTHON_USE_TYPE_SPECS
   __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2av_9subtitles_8subtitle_Subtitle); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 87, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitle = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2av_9subtitles_8subtitle_BitmapSubtitle_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(!__pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitle)) __PYX_ERR(1, 87, __pyx_L1_error)
   if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2av_9subtitles_8subtitle_BitmapSubtitle_spec, __pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitle) < 0) __PYX_ERR(1, 87, __pyx_L1_error)
@@ -12566,40 +12598,40 @@
   }
   #endif
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BitmapSubtitlePlane, (PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitlePlane) < 0) __PYX_ERR(1, 122, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_BitmapSubtitlePlane) < 0) __PYX_ERR(1, 122, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2av_9subtitles_8subtitle_Subtitle); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 151, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2av_9subtitles_8subtitle_Subtitle); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2av_9subtitles_8subtitle_AssSubtitle_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle)) __PYX_ERR(1, 151, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2av_9subtitles_8subtitle_AssSubtitle_spec, __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle)) __PYX_ERR(1, 153, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2av_9subtitles_8subtitle_AssSubtitle_spec, __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle) < 0) __PYX_ERR(1, 153, __pyx_L1_error)
   #else
   __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle = &__pyx_type_2av_9subtitles_8subtitle_AssSubtitle;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle->tp_base = __pyx_ptype_2av_9subtitles_8subtitle_Subtitle;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle) < 0) __PYX_ERR(1, 153, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle->tp_dictoffset && __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AssSubtitle, (PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_AssSubtitle, (PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle) < 0) __PYX_ERR(1, 153, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle) < 0) __PYX_ERR(1, 151, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2av_9subtitles_8subtitle_AssSubtitle) < 0) __PYX_ERR(1, 153, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
   __pyx_ptype_2av_9subtitles_8subtitle___pyx_scope_struct____cinit__ = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2av_9subtitles_8subtitle___pyx_scope_struct____cinit___spec, NULL); if (unlikely(!__pyx_ptype_2av_9subtitles_8subtitle___pyx_scope_struct____cinit__)) __PYX_ERR(1, 14, __pyx_L1_error)
   if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2av_9subtitles_8subtitle___pyx_scope_struct____cinit___spec, __pyx_ptype_2av_9subtitles_8subtitle___pyx_scope_struct____cinit__) < 0) __PYX_ERR(1, 14, __pyx_L1_error)
   #else
   __pyx_ptype_2av_9subtitles_8subtitle___pyx_scope_struct____cinit__ = &__pyx_type_2av_9subtitles_8subtitle___pyx_scope_struct____cinit__;
   #endif
```

### Comparing `pyav-12.1.0rc1/src/av/utils.c` & `pyav-12.1.0rc2/src/av/utils.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/video/codeccontext.c` & `pyav-12.1.0rc2/src/av/video/codeccontext.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/video/format.c` & `pyav-12.1.0rc2/src/av/video/format.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/video/frame.c` & `pyav-12.1.0rc2/src/av/video/frame.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/video/plane.c` & `pyav-12.1.0rc2/src/av/video/plane.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/video/reformatter.c` & `pyav-12.1.0rc2/src/av/video/reformatter.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/src/av/video/stream.c` & `pyav-12.1.0rc2/src/av/video/stream.c`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/common.py` & `pyav-12.1.0rc2/tests/common.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_audiofifo.py` & `pyav-12.1.0rc2/tests/test_audiofifo.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_audioformat.py` & `pyav-12.1.0rc2/tests/test_audioformat.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_audioframe.py` & `pyav-12.1.0rc2/tests/test_audioframe.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_audiolayout.py` & `pyav-12.1.0rc2/tests/test_audiolayout.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_audioresampler.py` & `pyav-12.1.0rc2/tests/test_audioresampler.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_bitstream.py` & `pyav-12.1.0rc2/tests/test_bitstream.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_codec.py` & `pyav-12.1.0rc2/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_codec_context.py` & `pyav-12.1.0rc2/tests/test_codec_context.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_colorspace.py` & `pyav-12.1.0rc2/tests/test_colorspace.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_containerformat.py` & `pyav-12.1.0rc2/tests/test_containerformat.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_decode.py` & `pyav-12.1.0rc2/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_deprecation.py` & `pyav-12.1.0rc2/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_doctests.py` & `pyav-12.1.0rc2/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_encode.py` & `pyav-12.1.0rc2/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_enums.py` & `pyav-12.1.0rc2/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_errors.py` & `pyav-12.1.0rc2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_file_probing.py` & `pyav-12.1.0rc2/tests/test_file_probing.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_filters.py` & `pyav-12.1.0rc2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_logging.py` & `pyav-12.1.0rc2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_open.py` & `pyav-12.1.0rc2/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_options.py` & `pyav-12.1.0rc2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_packet.py` & `pyav-12.1.0rc2/tests/test_packet.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,7 +35,15 @@
         with av.open(fate_suite("hap/HAPQA_NoSnappy_127x1.mov")) as container:
             stream = container.streams.video[0]
             for i, packet in enumerate(container.demux(stream)):
                 if i == 0:
                     self.assertTrue(packet.is_disposable)
                 else:
                     self.assertFalse(packet.is_disposable)
+
+    def test_set_duration(self):
+        with av.open(fate_suite("h264/interlaced_crop.mp4")) as container:
+            for packet in container.demux():
+                old_duration = packet.duration
+                packet.duration += 10
+
+                self.assertEqual(packet.duration, old_duration + 10)
```

### Comparing `pyav-12.1.0rc1/tests/test_python_io.py` & `pyav-12.1.0rc2/tests/test_python_io.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_seek.py` & `pyav-12.1.0rc2/tests/test_seek.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_streams.py` & `pyav-12.1.0rc2/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_subtitles.py` & `pyav-12.1.0rc2/tests/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_timeout.py` & `pyav-12.1.0rc2/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_videoformat.py` & `pyav-12.1.0rc2/tests/test_videoformat.py`

 * *Files identical despite different names*

### Comparing `pyav-12.1.0rc1/tests/test_videoframe.py` & `pyav-12.1.0rc2/tests/test_videoframe.py`

 * *Files identical despite different names*


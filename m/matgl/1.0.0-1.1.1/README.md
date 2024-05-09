# Comparing `tmp/matgl-1.0.0.tar.gz` & `tmp/matgl-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-1.0.0.tar", last modified: Wed Feb 14 15:57:21 2024, max compression
+gzip compressed data, was "matgl-1.1.1.tar", last modified: Thu May  9 14:23:26 2024, max compression
```

## Comparing `matgl-1.0.0.tar` & `matgl-1.1.1.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.742328 matgl-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-14 15:55:10.000000 matgl-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-02-14 15:57:21.742328 matgl-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13849 2024-02-14 15:55:10.000000 matgl-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-02-14 15:55:11.000000 matgl-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 15:57:21.742328 matgl-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.730328 matgl-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.734328 matgl-1.0.0/src/matgl/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.734328 matgl-1.0.0/src/matgl/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/apps/pes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.734328 matgl-1.0.0/src/matgl/data/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/data/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.734328 matgl-1.0.0/src/matgl/ext/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20644 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/ext/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/ext/pymatgen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.738328 matgl-1.0.0/src/matgl/graph/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/graph/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/graph/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/graph/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.738328 matgl-1.0.0/src/matgl/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_atom_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_bond.py
--rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15438 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    22732 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_graph_convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_readout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_so3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_three_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/layers/_zbl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.738328 matgl-1.0.0/src/matgl/models/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14593 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/models/_m3gnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/models/_megnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/models/_so3net.py
--rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/models/_tensornet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/models/_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.742328 matgl-1.0.0/src/matgl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/utils/cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/utils/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)   131200 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/utils/sb_roots.npy
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/utils/so3.py
--rw-r--r--   0 runner    (1001) docker     (127)    16730 2024-02-14 15:55:11.000000 matgl-1.0.0/src/matgl/utils/training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.742328 matgl-1.0.0/src/matgl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-02-14 15:57:21.000000 matgl-1.0.0/src/matgl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-14 15:57:21.000000 matgl-1.0.0/src/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 15:57:21.000000 matgl-1.0.0/src/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-14 15:57:21.000000 matgl-1.0.0/src/matgl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-14 15:57:21.000000 matgl-1.0.0/src/matgl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-14 15:57:21.000000 matgl-1.0.0/src/matgl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:57:21.742328 matgl-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-14 15:55:11.000000 matgl-1.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-14 15:55:11.000000 matgl-1.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-14 15:55:11.000000 matgl-1.0.0/tests/test_default_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-14 15:55:11.000000 matgl-1.0.0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.417724 matgl-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-09 14:18:54.000000 matgl-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-05-09 14:23:26.417724 matgl-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-05-09 14:18:54.000000 matgl-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-09 14:18:55.000000 matgl-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:23:26.417724 matgl-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.405723 matgl-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.405723 matgl-1.1.1/src/matgl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.409724 matgl-1.1.1/src/matgl/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5689 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/apps/pes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.409724 matgl-1.1.1/src/matgl/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/data/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.409724 matgl-1.1.1/src/matgl/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22078 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/ext/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/ext/pymatgen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.409724 matgl-1.1.1/src/matgl/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14738 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/graph/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/graph/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/graph/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.413724 matgl-1.1.1/src/matgl/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_atom_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_bond.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16964 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15438 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48909 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_readout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_so3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_three_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/layers/_zbl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.413724 matgl-1.1.1/src/matgl/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19150 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/models/_chgnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/models/_m3gnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/models/_megnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15517 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/models/_so3net.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11669 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/models/_tensornet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/models/_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.417724 matgl-1.1.1/src/matgl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/utils/cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/utils/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131200 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/utils/sb_roots.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/utils/so3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-05-09 14:18:55.000000 matgl-1.1.1/src/matgl/utils/training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.417724 matgl-1.1.1/src/matgl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-05-09 14:23:26.000000 matgl-1.1.1/src/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-09 14:23:26.000000 matgl-1.1.1/src/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:23:26.000000 matgl-1.1.1/src/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 14:23:26.000000 matgl-1.1.1/src/matgl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 14:23:26.000000 matgl-1.1.1/src/matgl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 14:23:26.000000 matgl-1.1.1/src/matgl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:23:26.417724 matgl-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-09 14:18:55.000000 matgl-1.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-09 14:18:55.000000 matgl-1.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-09 14:18:55.000000 matgl-1.1.1/tests/test_default_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-09 14:18:55.000000 matgl-1.1.1/tests/test_integration.py
```

### Comparing `matgl-1.0.0/LICENSE` & `matgl-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/PKG-INFO` & `matgl-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 1.0.0
+Version: 1.1.1
 Summary: MatGL is a framework for graph deep learning for materials science.
-Author-email: Tsz Wai Ko <t1ko@ucsd.edu>, Marcel Nassar <marcel.nassar@intel.com>, Ji Qi <j1qi@ucsd.edu>, Santiago Miret <santiago.miret@intel.com>, Eliott Liu <elliottliu17@gmail.com>, Shyue Ping Ong <ongsp@ucsd.edu>
+Author-email: Tsz Wai Ko <t1ko@ucsd.edu>, Marcel Nassar <marcel.nassar@intel.com>, Ji Qi <j1qi@ucsd.edu>, Santiago Miret <santiago.miret@intel.com>, Eliott Liu <elliottliu17@gmail.com>, Bowen Deng <bowendeng@berkeley.edu>, Luis Barroso-Luque <lbluque@berkeley.edu>, Shyue Ping Ong <ongsp@ucsd.edu>
 License: BSD-3-Clause
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
@@ -17,18 +17,19 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ase
-Requires-Dist: dgl
+Requires-Dist: dgl>=2.0.0
 Requires-Dist: pymatgen
 Requires-Dist: pytorch_lightning
-Requires-Dist: torch
+Requires-Dist: torch<=2.2.1
+Requires-Dist: pydantic
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml/badge.svg)](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml)
 [![Downloads](https://static.pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 [![codecov](https://codecov.io/gh/materialsvirtuallab/matgl/branch/main/graph/badge.svg?token=3V3O79GODQ)](https://codecov.io/gh/materialsvirtuallab/matgl)
 [![PyPI](https://img.shields.io/pypi/v/matgl?logo=pypi&logoColor=white)](https://pypi.org/project/matgl?logo=pypi&logoColor=white)
@@ -43,28 +44,24 @@
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms. Graph deep learning models have been shown to consistently deliver
 exceptional performance as surrogate models for the prediction of materials properties.
 
 MatGL is built on the [Deep Graph Library (DGL)][dgl] and PyTorch, with suitable adaptations for materials-specific
 applications. The goal is for MatGL to serve as an extensible platform to develop and share materials graph deep
-learning models. For the initial release, we have re-implemented the [MatErials 3-body Graph Network (M3GNet)]
-[m3gnet] and its predecessor, [MEGNet][megnet], which were originally implemented in Tensorflow, to improve the
-usability, extensibility and scalability of these models. Here are some key improvements over the TF implementations:
-
-- A more intuitive API and class structure based on DGL.
-- Multi-GPU support via PyTorch Lightning.
+learning models, including the [MatErials 3-body Graph Network (M3GNet)][m3gnet] and its predecessor, [MEGNet].
 
 This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
 Nassar, Carmelo Gonzales).
 
 ## Status
 
 Major milestones are summarized below. Please refer to the [changelog] for details.
 
+- v1.0.0 (Feb 14 2024): Implementation of [TensorNet] and [SO3Net].
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
@@ -75,22 +72,14 @@
 in future.
 
 <div style="float: left; padding: 10px; width: 300px">
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic">
 <p>Figure: Schematic of M3GNet/MEGNet</p>
 </div>
 
-### MEGNet
-
-[MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
-machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
-array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
-[multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
-network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an output graph.
-
 ### M3GNet
 
 [Materials 3-body Graph Network (M3GNet)][m3gnet] is a new materials graph neural network architecture that
 incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
 stresses via auto-differentiation. As a framework, M3GNet has diverse applications, including:
 
@@ -101,14 +90,37 @@
   performed in the [Materials Project][mp].
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
+MatGL reimplemennts M3GNet using DGL and Pytorch. Compared to the original Tensorflow implementation, some key
+improvements over the TF implementations are:
+
+- A more intuitive API and class structure based on DGL.
+- Multi-GPU support via PyTorch Lightning.
+
+### MEGNet
+
+[MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
+machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
+array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
+[multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
+network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an
+output graph.
+
+### Other models
+
+We have implemented other models in matgl as well. A non-exhaustive list is given below.
+
+- [TensorNet], an O(3)-equivariant message-passing neural network architecture that
+  leverages Cartesian tensor representations.
+- [SO3Net],  a minimalist SO(3)-equivariant neural network.
+
 ## Installation
 
 Matgl can be installed via pip for the latest stable version:
 
 ```bash
 pip install matgl
 ```
@@ -298,7 +310,9 @@
 [apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
 [doc]: https://matgl.ai "MatGL Documentation"
 [google colab]: https://colab.research.google.com/ "Google Colab"
 [jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
 [ongemail]: mailto:ongsp@ucsd.edu "Email"
 [mqm]: https://materialsqm.com "MaterialsQM"
 [tutorials]: https://matgl.ai/tutorials "Tutorials"
+[tensornet]: https://arxiv.org/abs/2306.06482 "TensorNet"
+[so3net]: https://pubs.aip.org/aip/jcp/article-abstract/158/14/144801/2877924/SchNetPack-2-0-A-neural-network-toolbox-for "SO3Net"
```

### Comparing `matgl-1.0.0/README.md` & `matgl-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,24 @@
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms. Graph deep learning models have been shown to consistently deliver
 exceptional performance as surrogate models for the prediction of materials properties.
 
 MatGL is built on the [Deep Graph Library (DGL)][dgl] and PyTorch, with suitable adaptations for materials-specific
 applications. The goal is for MatGL to serve as an extensible platform to develop and share materials graph deep
-learning models. For the initial release, we have re-implemented the [MatErials 3-body Graph Network (M3GNet)]
-[m3gnet] and its predecessor, [MEGNet][megnet], which were originally implemented in Tensorflow, to improve the
-usability, extensibility and scalability of these models. Here are some key improvements over the TF implementations:
-
-- A more intuitive API and class structure based on DGL.
-- Multi-GPU support via PyTorch Lightning.
+learning models, including the [MatErials 3-body Graph Network (M3GNet)][m3gnet] and its predecessor, [MEGNet].
 
 This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
 Nassar, Carmelo Gonzales).
 
 ## Status
 
 Major milestones are summarized below. Please refer to the [changelog] for details.
 
+- v1.0.0 (Feb 14 2024): Implementation of [TensorNet] and [SO3Net].
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
@@ -47,22 +43,14 @@
 in future.
 
 <div style="float: left; padding: 10px; width: 300px">
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic">
 <p>Figure: Schematic of M3GNet/MEGNet</p>
 </div>
 
-### MEGNet
-
-[MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
-machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
-array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
-[multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
-network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an output graph.
-
 ### M3GNet
 
 [Materials 3-body Graph Network (M3GNet)][m3gnet] is a new materials graph neural network architecture that
 incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
 stresses via auto-differentiation. As a framework, M3GNet has diverse applications, including:
 
@@ -73,14 +61,37 @@
   performed in the [Materials Project][mp].
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
+MatGL reimplemennts M3GNet using DGL and Pytorch. Compared to the original Tensorflow implementation, some key
+improvements over the TF implementations are:
+
+- A more intuitive API and class structure based on DGL.
+- Multi-GPU support via PyTorch Lightning.
+
+### MEGNet
+
+[MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
+machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
+array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
+[multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
+network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an
+output graph.
+
+### Other models
+
+We have implemented other models in matgl as well. A non-exhaustive list is given below.
+
+- [TensorNet], an O(3)-equivariant message-passing neural network architecture that
+  leverages Cartesian tensor representations.
+- [SO3Net],  a minimalist SO(3)-equivariant neural network.
+
 ## Installation
 
 Matgl can be installed via pip for the latest stable version:
 
 ```bash
 pip install matgl
 ```
@@ -270,7 +281,9 @@
 [apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
 [doc]: https://matgl.ai "MatGL Documentation"
 [google colab]: https://colab.research.google.com/ "Google Colab"
 [jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
 [ongemail]: mailto:ongsp@ucsd.edu "Email"
 [mqm]: https://materialsqm.com "MaterialsQM"
 [tutorials]: https://matgl.ai/tutorials "Tutorials"
+[tensornet]: https://arxiv.org/abs/2306.06482 "TensorNet"
+[so3net]: https://pubs.aip.org/aip/jcp/article-abstract/158/14/144801/2877924/SchNetPack-2-0-A-neural-network-toolbox-for "SO3Net"
```

### Comparing `matgl-1.0.0/pyproject.toml` & `matgl-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 name = "matgl"
 authors = [
     { name = "Tsz Wai Ko", email = "t1ko@ucsd.edu" },
     { name = "Marcel Nassar", email = "marcel.nassar@intel.com" },
     { name = "Ji Qi", email = "j1qi@ucsd.edu" },
     { name = "Santiago Miret", email = "santiago.miret@intel.com" },
     { name = "Eliott Liu", email = "elliottliu17@gmail.com" },
+    { name = "Bowen Deng", email = "bowendeng@berkeley.edu" },
+    { name = "Luis Barroso-Luque", email = "lbluque@berkeley.edu" },
     { name = "Shyue Ping Ong", email = "ongsp@ucsd.edu" },
 ]
 description = "MatGL is a framework for graph deep learning for materials science."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
     "materials",
@@ -44,20 +46,21 @@
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "ase",
-    "dgl",
+    "dgl>=2.0.0",
     "pymatgen",
     "pytorch_lightning",
-    "torch",
+    "torch<=2.2.1",
+    "pydantic"
 ]
-version = "1.0.0"
+version = "1.1.1"
 
 [project.scripts]
 mgl = "matgl.cli:main"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `matgl-1.0.0/src/matgl/__init__.py` & `matgl-1.1.1/src/matgl/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/apps/pes.py` & `matgl-1.1.1/src/matgl/apps/pes.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,52 +16,52 @@
     import dgl
     import numpy as np
 
 
 class Potential(nn.Module, IOMixIn):
     """A class representing an interatomic potential."""
 
-    __version__ = 2
+    __version__ = 3
 
     def __init__(
         self,
         model: nn.Module,
         data_mean: torch.Tensor | float = 0.0,
         data_std: torch.Tensor | float = 1.0,
         element_refs: np.ndarray | None = None,
         calc_forces: bool = True,
         calc_stresses: bool = True,
         calc_hessian: bool = False,
-        calc_site_wise: bool = False,
+        calc_magmom: bool = False,
         calc_repuls: bool = False,
         zbl_trainable: bool = False,
         debug_mode: bool = False,
     ):
         """Initialize Potential from a model and elemental references.
 
         Args:
             model: Model for predicting energies.
             data_mean: Mean of target.
             data_std: Std dev of target.
             element_refs: Element reference values for each element.
             calc_forces: Enable force calculations.
             calc_stresses: Enable stress calculations.
             calc_hessian: Enable hessian calculations.
-            calc_site_wise: Enable site-wise property calculation.
+            calc_magmom: Enable site-wise property calculation.
             calc_repuls: Whether the ZBL repulsion is included
             zbl_trainable: Whether zbl repulsion is trainable
             debug_mode: Return gradient of total energy with respect to atomic positions and lattices for checking
         """
         super().__init__()
         self.save_args(locals())
         self.model = model
         self.calc_forces = calc_forces
         self.calc_stresses = calc_stresses
         self.calc_hessian = calc_hessian
-        self.calc_site_wise = calc_site_wise
+        self.calc_magmom = calc_magmom
         self.element_refs: AtomRef | None
         self.debug_mode = debug_mode
         self.calc_repuls = calc_repuls
 
         if calc_repuls:
             self.repuls = NuclearRepulsion(self.model.cutoff, trainable=zbl_trainable)
 
@@ -91,29 +91,24 @@
         Returns:
             (energies, forces, stresses, hessian) or (energies, forces, stresses, hessian, site-wise properties)
         """
         # st (strain) for stress calculations
         st = lat.new_zeros([g.batch_size, 3, 3])
         if self.calc_stresses:
             st.requires_grad_(True)
-        lattice = lat @ (torch.eye(3).to(st.device) + st)
+        lattice = lat @ (torch.eye(3, device=lat.device) + st)
         g.edata["lattice"] = torch.repeat_interleave(lattice, g.batch_num_edges(), dim=0)
         g.edata["pbc_offshift"] = (g.edata["pbc_offset"].unsqueeze(dim=-1) * g.edata["lattice"]).sum(dim=1)
         g.ndata["pos"] = (
             g.ndata["frac_coords"].unsqueeze(dim=-1) * torch.repeat_interleave(lattice, g.batch_num_nodes(), dim=0)
         ).sum(dim=1)
         if self.calc_forces:
             g.ndata["pos"].requires_grad_(True)
 
-        predictions = self.model(g=g, state_attr=state_attr, l_g=l_g)
-        if isinstance(predictions, tuple) and len(predictions) > 1:
-            total_energies, site_wise = predictions
-        else:
-            total_energies = predictions
-            site_wise = None
+        total_energies = self.model(g=g, state_attr=state_attr, l_g=l_g)
 
         total_energies = self.data_std * total_energies + self.data_mean
 
         if self.calc_repuls:
             total_energies += self.repuls(self.model.element_types, g)
 
         if self.element_refs is not None:
@@ -155,11 +150,11 @@
             scale = 1.0 / volume * -160.21766208
             sts = [i * j for i, j in zip(sts, scale)] if sts.dim() == 3 else [sts * scale]
             stresses = torch.cat(sts)
 
         if self.debug_mode:
             return total_energies, grads[0], grads[1]
 
-        if self.calc_site_wise:
-            return total_energies, forces, stresses, hessian, site_wise
+        if self.calc_magmom:
+            return total_energies, forces, stresses, hessian, g.ndata["magmom"]
 
         return total_energies, forces, stresses, hessian
```

### Comparing `matgl-1.0.0/src/matgl/cli.py` & `matgl-1.1.1/src/matgl/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             old_lattice = structure.lattice
             new_lattice = final_structure.lattice
             for param in ("a", "b", "c", "alpha", "beta", "gamma"):
                 print(f"{param}: {getattr(old_lattice, param):.3f} -> {getattr(new_lattice, param):.3f}")
             print("Sites (Fractional coordinates)")
 
             def fmt_fcoords(fc):
-                return np.array2string(fc, formatter={"float_kind": lambda x: "%.5f" % x})
+                return np.array2string(fc, formatter={"float_kind": lambda x: f"{x:.5f}"})
 
             for old_site, new_site in zip(structure, final_structure):
                 print(f"{old_site.species}: {fmt_fcoords(old_site.frac_coords)} -> {fmt_fcoords(new_site.frac_coords)}")
 
     return 0
```

### Comparing `matgl-1.0.0/src/matgl/config.py` & `matgl-1.1.1/src/matgl/config.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/data/transformer.py` & `matgl-1.1.1/src/matgl/data/transformer.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/ext/ase.py` & `matgl-1.1.1/src/matgl/ext/ase.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
         return g, lat, state_attr
 
 
 class PESCalculator(Calculator):
     """Potential calculator for ASE."""
 
-    implemented_properties = ("energy", "free_energy", "forces", "stress", "hessian")
+    implemented_properties = ("energy", "free_energy", "forces", "stress", "hessian", "magmoms")
 
     def __init__(
         self,
         potential: Potential,
         state_attr: torch.Tensor | None = None,
         stress_weight: float = 1.0,
         **kwargs,
@@ -141,14 +141,15 @@
             stress_weight (float): conversion factor from GPa to eV/A^3, if it is set to 1.0, the unit is in GPa
             **kwargs: Kwargs pass through to super().__init__().
         """
         super().__init__(**kwargs)
         self.potential = potential
         self.compute_stress = potential.calc_stresses
         self.compute_hessian = potential.calc_hessian
+        self.compute_magmom = potential.calc_magmom
         self.stress_weight = stress_weight
         self.state_attr = state_attr
         self.element_types = potential.model.element_types  # type: ignore
         self.cutoff = potential.model.cutoff
 
     def calculate(
         self,
@@ -168,26 +169,28 @@
         """
         properties = properties or ["energy"]
         system_changes = system_changes or all_changes
         super().calculate(atoms=atoms, properties=properties, system_changes=system_changes)
         graph, lattice, state_attr_default = Atoms2Graph(self.element_types, self.cutoff).get_graph(atoms)
         # type: ignore
         if self.state_attr is not None:
-            energies, forces, stresses, hessians = self.potential(graph, lattice, self.state_attr)
+            calc_result = self.potential(graph, lattice, self.state_attr)
         else:
-            energies, forces, stresses, hessians = self.potential(graph, lattice, state_attr_default)
+            calc_result = self.potential(graph, lattice, state_attr_default)
         self.results.update(
-            energy=energies.detach().cpu().numpy().item(),
-            free_energy=energies.detach().cpu().numpy().item(),
-            forces=forces.detach().cpu().numpy(),
+            energy=calc_result[0].detach().cpu().numpy().item(),
+            free_energy=calc_result[0].detach().cpu().numpy(),
+            forces=calc_result[1].detach().cpu().numpy(),
         )
         if self.compute_stress:
-            self.results.update(stress=stresses.detach().cpu().numpy() * self.stress_weight)
+            self.results.update(stress=calc_result[2].detach().cpu().numpy() * self.stress_weight)
         if self.compute_hessian:
-            self.results.update(hessian=hessians.detach().cpu().numpy())
+            self.results.update(hessian=calc_result[3].detach().cpu().numpy())
+        if self.compute_magmom:
+            self.results.update(magmoms=calc_result[4].detach().cpu().numpy())
 
 
 # for backward compatibility
 class M3GNetCalculator(PESCalculator):
     """M3GNet potential Calculator for ASE."""
 
     def __init__(
@@ -411,15 +414,17 @@
             append_trajectory (bool): Whether to append to prev trajectory.
             mask (np.array): either a tuple of 3 numbers (0 or 1) or a symmetric 3x3 array indicating,
                 which strain values may change for NPT simulations.
         """
         if isinstance(atoms, (Structure, Molecule)):
             atoms = AseAtomsAdaptor().get_atoms(atoms)
         self.atoms = atoms
-        self.atoms.set_calculator(PESCalculator(potential=potential, state_attr=state_attr))
+        self.atoms.set_calculator(
+            PESCalculator(potential=potential, state_attr=state_attr, stress_weight=stress_weight)
+        )
 
         if taut is None:
             taut = 100 * timestep * units.fs
         if taup is None:
             taup = 1000 * timestep * units.fs
         if mask is None:
             mask = np.array([(1, 0, 0), (0, 1, 0), (0, 0, 1)])
@@ -505,14 +510,15 @@
                 trajectory=trajectory,
                 logfile=logfile,
                 loginterval=loginterval,
                 append_trajectory=append_trajectory,
             )
 
         elif ensemble.lower() == "npt_nose_hoover":
+            self.upper_triangular_cell()
             self.dyn = NPT(
                 self.atoms,
                 timestep * units.fs,
                 temperature_K=temperature,
                 externalstress=external_stress,
                 ttime=ttime * units.fs,
                 pfactor=pfactor * units.fs,
@@ -547,7 +553,35 @@
         """
         if isinstance(atoms, (Structure, Molecule)):
             atoms = AseAtomsAdaptor().get_atoms(atoms)
         calculator = self.atoms.calc
         self.atoms = atoms
         self.dyn.atoms = atoms
         self.dyn.atoms.set_calculator(calculator)
+
+    def upper_triangular_cell(self, verbose: bool | None = False) -> None:
+        """Transform to upper-triangular cell.
+        ASE Nose-Hoover implementation only supports upper-triangular cell
+        while ASE's canonical description is lower-triangular cell.
+
+        Args:
+            verbose (bool): Whether to notify user about upper-triangular cell
+                transformation. Default = False
+        """
+        if not NPT._isuppertriangular(self.atoms.get_cell()):
+            a, b, c, alpha, beta, gamma = self.atoms.cell.cellpar()
+            angles = np.radians((alpha, beta, gamma))
+            sin_a, sin_b, _sin_g = np.sin(angles)
+            cos_a, cos_b, cos_g = np.cos(angles)
+            cos_p = (cos_g - cos_a * cos_b) / (sin_a * sin_b)
+            cos_p = np.clip(cos_p, -1, 1)
+            sin_p = (1 - cos_p**2) ** 0.5
+
+            new_basis = [
+                (a * sin_b * sin_p, a * sin_b * cos_p, a * cos_b),
+                (0, b * sin_a, b * cos_a),
+                (0, 0, c),
+            ]
+
+            self.atoms.set_cell(new_basis, scale_atoms=True)
+            if verbose:
+                print("Transformed to upper triangular unit cell.", flush=True)
```

### Comparing `matgl-1.0.0/src/matgl/ext/pymatgen.py` & `matgl-1.1.1/src/matgl/ext/pymatgen.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/graph/compute.py` & `matgl-1.1.1/src/matgl/graph/compute.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,16 @@
 def create_line_graph(g: dgl.DGLGraph, threebody_cutoff: float, directed: bool = False) -> dgl.DGLGraph:
     """
     Calculate the three body indices from pair atom indices.
 
     Args:
         g: DGL graph
         threebody_cutoff (float): cutoff for three-body interactions
-        directed (bool): Whether to create a directed line graph, or an m3gnet 3body line graph (default: False, m3gnet)
+        directed (bool): Whether to create a directed line graph, or an M3gnet 3body line graph
+            Default = False (M3Gnet)
 
     Returns:
         l_g: DGL graph containing three body information from graph
     """
     graph_with_three_body = prune_edges_by_features(g, feat_name="bond_dist", condition=lambda x: x > threebody_cutoff)
     if directed:
         lg = _create_directed_line_graph(graph_with_three_body, threebody_cutoff)
@@ -222,18 +223,18 @@
     """Creates a line graph from a graph, considers periodic boundary conditions.
 
     Args:
         graph: DGL graph representing atom graph
         threebody_cutoff: cutoff for three-body interactions
 
     Returns:
-        line_graph: DGL graph line graph of pruned graph to three body cutoff
+        line_graph: DGL line graph of pruned graph to three body cutoff
     """
     with torch.no_grad():
-        pg = prune_edges_by_features(graph, feat_name="bond_dist", condition=lambda x: x > threebody_cutoff)
+        pg = prune_edges_by_features(graph, feat_name="bond_dist", condition=lambda x: torch.gt(x, threebody_cutoff))
         src_indices, dst_indices = pg.edges()
         images = pg.edata["pbc_offset"]
         all_indices = torch.arange(pg.number_of_nodes(), device=graph.device).unsqueeze(dim=0)
         num_bonds_per_atom = torch.count_nonzero(src_indices.unsqueeze(dim=1) == all_indices, dim=0)
         num_edges_per_bond = (num_bonds_per_atom - 1).repeat_interleave(num_bonds_per_atom)
         lg_src = torch.empty(num_edges_per_bond.sum(), dtype=matgl.int_th, device=graph.device)
         lg_dst = torch.empty(num_edges_per_bond.sum(), dtype=matgl.int_th, device=graph.device)
```

### Comparing `matgl-1.0.0/src/matgl/graph/converters.py` & `matgl-1.1.1/src/matgl/graph/converters.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/graph/data.py` & `matgl-1.1.1/src/matgl/graph/data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tools to construct a dataset of DGL graphs."""
 
 from __future__ import annotations
 
 import json
 import os
+from functools import partial
 from typing import TYPE_CHECKING, Callable
 
 import dgl
 import numpy as np
 import torch
 from dgl.data import DGLDataset
 from dgl.data.utils import load_graphs, save_graphs
@@ -17,15 +18,15 @@
 import matgl
 from matgl.graph.compute import compute_pair_vector_and_distance, create_line_graph
 
 if TYPE_CHECKING:
     from matgl.graph.converters import GraphConverter
 
 
-def collate_fn(batch, include_line_graph: bool = False, multiple_values_per_target: bool = False):
+def collate_fn_graph(batch, include_line_graph: bool = False, multiple_values_per_target: bool = False):
     """Merge a list of dgl graphs to form a batch."""
     line_graphs = None
     if include_line_graph:
         graphs, lattices, line_graphs, state_attr, labels = map(list, zip(*batch))
     else:
         graphs, lattices, state_attr, labels = map(list, zip(*batch))
     g = dgl.batch(graphs)
@@ -38,15 +39,15 @@
     lat = lattices[0] if g.batch_size == 1 else torch.squeeze(torch.stack(lattices))
     if include_line_graph:
         l_g = dgl.batch(line_graphs)
         return g, lat, l_g, state_attr, labels
     return g, lat, state_attr, labels
 
 
-def collate_fn_efs(batch, include_stress: bool = True, include_line_graph: bool = False):
+def collate_fn_pes(batch, include_stress: bool = True, include_line_graph: bool = False, include_magmom: bool = False):
     """Merge a list of dgl graphs to form a batch."""
     l_g = None
     if include_line_graph:
         graphs, lattices, line_graphs, state_attr, labels = map(list, zip(*batch))
         l_g = dgl.batch(line_graphs)
     else:
         graphs, lattices, state_attr, labels = map(list, zip(*batch))
@@ -54,25 +55,32 @@
     e = torch.tensor([d["energies"] for d in labels])  # type: ignore
     f = torch.vstack([d["forces"] for d in labels])  # type: ignore
     s = (
         torch.vstack([d["stresses"] for d in labels])  # type: ignore
         if include_stress is True
         else torch.tensor(np.zeros(e.size(dim=0)), dtype=matgl.float_th)
     )
+    m = (
+        torch.vstack([d["magmoms"] for d in labels])
+        if include_magmom is True
+        else torch.tensor(np.zeros(e.size(dim=0)), dtype=matgl.float_th)
+    )
     state_attr = torch.stack(state_attr)
     lat = torch.stack(lattices)
     if include_line_graph:
+        if include_magmom:
+            return g, torch.squeeze(lat), l_g, state_attr, e, f, s, m
         return g, torch.squeeze(lat), l_g, state_attr, e, f, s
     return g, torch.squeeze(lat), state_attr, e, f, s
 
 
 def MGLDataLoader(
     train_data: dgl.data.utils.Subset,
     val_data: dgl.data.utils.Subset,
-    collate_fn: Callable,
+    collate_fn: Callable | None = None,
     test_data: dgl.data.utils.Subset = None,
     **kwargs,
 ) -> tuple[GraphDataLoader, ...]:
     """Dataloader for MatGL training.
 
     Args:
         train_data (dgl.data.utils.Subset): Training dataset.
@@ -82,16 +90,27 @@
         **kwargs: Pass-through kwargs to dgl.dataloading.GraphDataLoader. Common ones you may want to set are
             batch_size, num_workers, use_ddp, pin_memory and generator.
 
     Returns:
         tuple[GraphDataLoader, ...]: Train, validation and test data loaders. Test data
             loader is None if test_data is None.
     """
-    train_loader = GraphDataLoader(train_data, shuffle=True, collate_fn=collate_fn, **kwargs)
+    if collate_fn is None:
+        if "forces" not in train_data.dataset.labels:
+            collate_fn = collate_fn_graph
+        else:
+            if "stresses" not in train_data.dataset.labels:
+                collate_fn = partial(collate_fn_pes, include_stress=False)
+            else:
+                if "magmoms" not in train_data.dataset.labels:
+                    collate_fn = collate_fn_pes
+                else:
+                    collate_fn = partial(collate_fn_pes, include_stress=True, include_magmom=True)
 
+    train_loader = GraphDataLoader(train_data, shuffle=True, collate_fn=collate_fn, **kwargs)
     val_loader = GraphDataLoader(val_data, shuffle=False, collate_fn=collate_fn, **kwargs)
     if test_data is not None:
         test_loader = GraphDataLoader(test_data, shuffle=False, collate_fn=collate_fn, **kwargs)
         return train_loader, val_loader, test_loader
     return train_loader, val_loader
 
 
@@ -104,127 +123,146 @@
         filename_lattice: str = "lattice.pt",
         filename_line_graph: str = "dgl_line_graph.bin",
         filename_state_attr: str = "state_attr.pt",
         filename_labels: str = "labels.json",
         include_line_graph: bool = False,
         converter: GraphConverter | None = None,
         threebody_cutoff: float | None = None,
+        directed_line_graph: bool = False,
         structures: list | None = None,
         labels: dict[str, list] | None = None,
         name: str = "MGLDataset",
         graph_labels: list[int | float] | None = None,
         clear_processed: bool = False,
+        save_cache: bool = True,
+        raw_dir: str | None = None,
+        save_dir: str | None = None,
     ):
         """
         Args:
             filename: file name for storing dgl graphs.
             filename_lattice: file name for storing lattice matrixs.
             filename_line_graph: file name for storing dgl line graphs.
             filename_state_attr: file name for storing state attributes.
             filename_labels: file name for storing labels.
             include_line_graph: whether to include line graphs.
             converter: dgl graph converter.
             threebody_cutoff: cutoff for three body.
+            directed_line_graph (bool): Whether to create a directed line graph (CHGNet), or an
+                undirected 3body line graph (M3GNet)
+                Default: False (for M3GNet)
             structures: Pymatgen structure.
             labels: targets, as a dict of {name: list of values}.
             name: name of dataset.
             graph_labels: state attributes.
             clear_processed: Whether to clear the stored structures after processing into graphs. Structures
                 are not really needed after the conversion to DGL graphs and can take a significant amount of memory.
                 Setting this to True will delete the structures from memory.
+            save_cache: whether to save the processed dataset. The dataset can be reloaded from save_dir
+                Default: True
+            raw_dir : str specifying the directory that will store the downloaded data or the directory that already
+                stores the input data.
+                Default: ~/.dgl/
+            save_dir : directory to save the processed dataset. Default: same as raw_dir.
         """
         self.filename = filename
         self.filename_lattice = filename_lattice
         self.filename_line_graph = filename_line_graph
         self.filename_state_attr = filename_state_attr
         self.filename_labels = filename_labels
         self.include_line_graph = include_line_graph
         self.converter = converter
         self.structures = structures or []
         self.labels = labels or {}
         for k, v in self.labels.items():
             self.labels[k] = v.tolist() if isinstance(v, np.ndarray) else v
         self.threebody_cutoff = threebody_cutoff
+        self.directed_line_graph = directed_line_graph
         self.graph_labels = graph_labels
         self.clear_processed = clear_processed
-        super().__init__(name=name)
+        self.save_cache = save_cache
+        super().__init__(name=name, raw_dir=raw_dir, save_dir=save_dir)
 
     def has_cache(self) -> bool:
         """Check if the dgl_graph.bin exists or not."""
         files_to_check = [
             self.filename,
             self.filename_lattice,
             self.filename_state_attr,
             self.filename_labels,
         ]
         if self.include_line_graph:
             files_to_check.append(self.filename_line_graph)
-        return all(os.path.exists(f) for f in files_to_check)
+        return all(os.path.exists(os.path.join(self.save_path, f)) for f in files_to_check)
 
     def process(self):
         """Convert Pymatgen structure into dgl graphs."""
         num_graphs = len(self.structures)  # type: ignore
-        graphs = []
-        lattices = []
-        line_graphs = []
-        state_attrs = []
+        graphs, lattices, line_graphs, state_attrs = [], [], [], []
+
         for idx in trange(num_graphs):
             structure = self.structures[idx]  # type: ignore
             graph, lattice, state_attr = self.converter.get_graph(structure)  # type: ignore
             graphs.append(graph)
             lattices.append(lattice)
             state_attrs.append(state_attr)
             graph.ndata["pos"] = torch.tensor(structure.cart_coords)
             graph.edata["pbc_offshift"] = torch.matmul(graph.edata["pbc_offset"], lattice[0])
             bond_vec, bond_dist = compute_pair_vector_and_distance(graph)
             graph.edata["bond_vec"] = bond_vec
             graph.edata["bond_dist"] = bond_dist
             if self.include_line_graph:
-                line_graph = create_line_graph(graph, self.threebody_cutoff)  # type: ignore
+                line_graph = create_line_graph(graph, self.threebody_cutoff, directed=self.directed_line_graph)  # type: ignore
                 for name in ["bond_vec", "bond_dist", "pbc_offset"]:
                     line_graph.ndata.pop(name)
                 line_graphs.append(line_graph)
             graph.ndata.pop("pos")
             graph.edata.pop("pbc_offshift")
         if self.graph_labels is not None:
             state_attrs = torch.tensor(self.graph_labels).long()
         else:
-            state_attrs = torch.tensor(np.array(state_attrs))
+            state_attrs = torch.tensor(np.array(state_attrs), dtype=matgl.float_th)
 
         if self.clear_processed:
             del self.structures
             self.structures = []
 
         self.graphs = graphs
         self.lattices = lattices
         self.state_attr = state_attrs
         if self.include_line_graph:
             self.line_graphs = line_graphs
             return self.graphs, self.lattices, self.line_graphs, self.state_attr
         return self.graphs, self.lattices, self.state_attr
 
     def save(self):
-        """Save dgl graphs."""
+        """Save dgl graphs and labels to self.save_path."""
+        if self.save_cache is False:
+            return
+
+        if not os.path.exists(self.save_path):
+            os.makedirs(self.save_path)
+
         if self.labels:
-            with open(self.filename_labels, "w") as f:
-                json.dump(self.labels, f)
-        save_graphs(self.filename, self.graphs)
-        torch.save(self.lattices, self.filename_lattice)
-        torch.save(self.state_attr, self.filename_state_attr)
+            with open(os.path.join(self.save_path, self.filename_labels), "w") as file:
+                json.dump(self.labels, file)
+        save_graphs(os.path.join(self.save_path, self.filename), self.graphs)
+        torch.save(self.lattices, os.path.join(self.save_path, self.filename_lattice))
+        torch.save(self.state_attr, os.path.join(self.save_path, self.filename_state_attr))
         if self.include_line_graph:
-            save_graphs(self.filename_line_graph, self.line_graphs)
+            save_graphs(os.path.join(self.save_path, self.filename_line_graph), self.line_graphs)
 
     def load(self):
         """Load dgl graphs from files."""
-        self.graphs, _ = load_graphs(self.filename)
-        self.lattices = torch.load(self.filename_lattice)
+        self.graphs, _ = load_graphs(os.path.join(self.save_path, self.filename))
+        self.lattices = torch.load(os.path.join(self.save_path, self.filename_lattice))
         if self.include_line_graph:
-            self.line_graphs, _ = load_graphs(self.filename_line_graph)
-        self.state_attr = torch.load(self.filename_state_attr)
-        with open(self.filename_labels) as f:
+            self.line_graphs, _ = load_graphs(os.path.join(self.save_path, self.filename_line_graph))
+        self.state_attr = torch.load(os.path.join(self.save_path, self.filename_state_attr))
+        with open(os.path.join(self.save_path, self.filename_labels)) as f:
             self.labels = json.load(f)
 
     def __getitem__(self, idx: int):
         """Get graph and label with idx."""
         items = [
             self.graphs[idx],
             self.lattices[idx],
```

### Comparing `matgl-1.0.0/src/matgl/layers/__init__.py` & `matgl-1.1.1/src/matgl/layers/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,36 @@
 
 from __future__ import annotations
 
 from matgl.layers._activations import ActivationFunction
 from matgl.layers._atom_ref import AtomRef
 from matgl.layers._basis import FourierExpansion, RadialBesselFunction, SphericalBesselWithHarmonics
 from matgl.layers._bond import BondExpansion
-from matgl.layers._core import MLP, EdgeSet2Set, GatedEquivariantBlock, GatedMLP, build_gated_equivariant_mlp
+from matgl.layers._core import (
+    MLP,
+    EdgeSet2Set,
+    GatedEquivariantBlock,
+    GatedMLP,
+    GatedMLP_norm,
+    MLP_norm,
+    build_gated_equivariant_mlp,
+)
 from matgl.layers._embedding import EmbeddingBlock, NeighborEmbedding, TensorEmbedding
 from matgl.layers._graph_convolution import (
+    CHGNetAtomGraphBlock,
+    CHGNetBondGraphBlock,
+    CHGNetGraphConv,
+    CHGNetLineGraphConv,
     M3GNetBlock,
     M3GNetGraphConv,
     MEGNetBlock,
     MEGNetGraphConv,
     TensorNetInteraction,
 )
+from matgl.layers._norm import GraphNorm
 from matgl.layers._readout import (
     AttentiveFPReadout,
     GlobalPool,
     ReduceReadOut,
     Set2SetReadOut,
     WeightedAtomReadOut,
     WeightedReadOut,
```

### Comparing `matgl-1.0.0/src/matgl/layers/_activations.py` & `matgl-1.1.1/src/matgl/layers/_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/layers/_atom_ref.py` & `matgl-1.1.1/src/matgl/layers/_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/layers/_basis.py` & `matgl-1.1.1/src/matgl/layers/_basis.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/layers/_bond.py` & `matgl-1.1.1/src/matgl/layers/_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/layers/_core.py` & `matgl-1.1.1/src/matgl/layers/_core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Implementations of multi-layer perceptron (MLP) and other helper classes."""
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable
+from typing import TYPE_CHECKING, Any, Callable, Literal
 
+import dgl
 import torch
 from dgl import DGLGraph, broadcast_edges, softmax_edges, sum_edges
 from torch import Tensor, nn
 from torch.nn import LSTM, Linear, Module, ModuleList
 
+from matgl.layers._norm import GraphNorm, LayerNorm
+
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
 
 class MLP(nn.Module):
     """An implementation of a multi-layer perceptron."""
 
@@ -90,14 +93,88 @@
         x = inputs
         for layer in self.layers:
             x = layer(x)
 
         return x
 
 
+class MLP_norm(nn.Module):
+    """Multi-layer perceptron with normalization layer."""
+
+    def __init__(
+        self,
+        dims: list[int],
+        activation: nn.Module | None = None,
+        activate_last: bool = False,
+        use_bias: bool = True,
+        bias_last: bool = True,
+        normalization: Literal["graph", "layer"] | None = None,
+        normalize_hidden: bool = False,
+        norm_kwargs: dict[str, Any] | None = None,
+    ) -> None:
+        """
+        Args:
+            dims: Dimensions of each layer of MLP.
+            activation: activation: Activation function.
+            activate_last: Whether to apply activation to last layer.
+            use_bias: Whether to use bias.
+            bias_last: Whether to apply bias to last layer.
+            normalization: normalization name. "graph" or "layer"
+            normalize_hidden: Whether to normalize output of hidden layers.
+            norm_kwargs: Keyword arguments for normalization layer.
+        """
+        super().__init__()
+        self._depth = len(dims) - 1
+        self.layers = nn.ModuleList()
+        self.norm_layers = nn.ModuleList() if normalization in ("graph", "layer") else None
+        self.activation = activation if activation is not None else nn.Identity()
+        self.activate_last = activate_last
+        self.normalize_hidden = normalize_hidden
+        norm_kwargs = norm_kwargs or {}
+
+        for i, (in_dim, out_dim) in enumerate(zip(dims[:-1], dims[1:])):
+            if i < self._depth - 1:
+                self.layers.append(Linear(in_dim, out_dim, bias=use_bias))
+                if normalize_hidden:
+                    if normalization == "graph":
+                        self.norm_layers.append(GraphNorm(out_dim, **norm_kwargs))
+                    elif normalization == "layer":
+                        self.norm_layers.append(LayerNorm(out_dim, **norm_kwargs))
+            else:
+                self.layers.append(Linear(in_dim, out_dim, bias=use_bias and bias_last))
+                if normalization == "graph":
+                    self.norm_layers.append(GraphNorm(out_dim, **norm_kwargs))
+                elif normalization == "layer":
+                    self.norm_layers.append(LayerNorm(out_dim, **norm_kwargs))
+
+    def forward(self, inputs: torch.Tensor, g: dgl.Graph | None = None) -> torch.Tensor:
+        """Applies all layers in turn.
+
+        Args:
+            inputs: input feature tensor.
+            g: graph of model, needed for graph normalization
+
+        Returns:
+            output feature tensor.
+        """
+        x = inputs
+        for i in range(self._depth - 1):
+            x = self.layers[i](x)
+            if self.norm_layers is not None and self.normalize_hidden:
+                x = self.norm_layers[i](x, g)
+            x = self.activation(x)
+
+        x = self.layers[-1](x)
+        if self.norm_layers is not None:
+            x = self.norm_layers[-1](x, g)
+        if self.activate_last:
+            x = self.activation(x)
+        return x
+
+
 class GatedMLP(nn.Module):
     """An implementation of a Gated multi-layer perceptron."""
 
     def __init__(self, in_feats: int, dims: Sequence[int], activate_last: bool = True, use_bias: bool = True):
         """:param in_feats: Dimension of input features.
         :param dims: Architecture of neural networks.
         :param activate_last: Whether applying activation to last layer or not.
@@ -124,14 +201,73 @@
                 self.gates.append(nn.Linear(in_dim, out_dim, bias=use_bias))
                 self.gates.append(nn.Sigmoid())
 
     def forward(self, inputs: Tensor):
         return self.layers(inputs) * self.gates(inputs)
 
 
+class GatedMLP_norm(nn.Module):
+    """An implementation of a Gated multi-layer perceptron constructed with MLP."""
+
+    def __init__(
+        self,
+        in_feats: int,
+        dims: Sequence[int],
+        activation: nn.Module | None = None,
+        activate_last: bool = True,
+        use_bias: bool = True,
+        bias_last: bool = True,
+        normalization: Literal["graph", "layer"] | None = None,
+        normalize_hidden: bool = False,
+        norm_kwargs: dict[str, Any] | None = None,
+    ):
+        """:param in_feats: Dimension of input features.
+        :param dims: Architecture of neural networks.
+        :param activation: non-linear activation module.
+        :param activate_last: Whether applying activation to last layer or not.
+        :param use_bias: Whether to use a bias in linear layers.
+        :param bias_last: Whether applying bias to last layer or not.
+        :param normalization: normalization name.
+        :param normalize_hidden: Whether to normalize output of hidden layers.
+        :param norm_kwargs: Keyword arguments for normalization layer.
+        """
+        super().__init__()
+        self.in_feats = in_feats
+        self.dims = [in_feats, *dims]
+        self._depth = len(dims)
+        self.use_bias = use_bias
+        self.activate_last = activate_last
+
+        activation = activation if activation is not None else nn.SiLU()
+        self.layers = MLP_norm(
+            self.dims,
+            activation=activation,
+            activate_last=True,
+            use_bias=use_bias,
+            bias_last=bias_last,
+            normalization=normalization,
+            normalize_hidden=normalize_hidden,
+            norm_kwargs=norm_kwargs,
+        )
+        self.gates = MLP_norm(
+            self.dims,
+            activation,
+            activate_last=False,
+            use_bias=use_bias,
+            bias_last=bias_last,
+            normalization=normalization,
+            normalize_hidden=normalize_hidden,
+            norm_kwargs=norm_kwargs,
+        )
+        self.sigmoid = nn.Sigmoid()
+
+    def forward(self, inputs: torch.Tensor, graph: dgl.Graph | None = None) -> torch.Tensor:
+        return self.layers(inputs, graph) * self.sigmoid(self.gates(inputs, graph))
+
+
 class EdgeSet2Set(Module):
     """Implementation of Set2Set."""
 
     def __init__(self, input_dim: int, n_iters: int, n_layers: int) -> None:
         """:param input_dim: The size of each input sample.
         :param n_iters: The number of iterations.
         :param n_layers: The number of recurrent layers.
@@ -144,15 +280,15 @@
         self.lstm = LSTM(self.output_dim, self.input_dim, n_layers)
         self.reset_parameters()
 
     def reset_parameters(self):
         """Reinitialize learnable parameters."""
         self.lstm.reset_parameters()
 
-    def forward(self, g: DGLGraph, feat: Tensor):
+    def forward(self, g: DGLGraph, feat: torch.Tensor):
         """Defines the computation performed at every call.
 
         :param g: Input graph
         :param feat: Input features.
         :return: One hot vector
         """
         with g.local_scope():
```

### Comparing `matgl-1.0.0/src/matgl/layers/_embedding.py` & `matgl-1.1.1/src/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/layers/_readout.py` & `matgl-1.1.1/src/matgl/layers/_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/layers/_so3.py` & `matgl-1.1.1/src/matgl/layers/_so3.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,16 @@
         self.register_buffer("zpow", zpow.to(dtype=dtype), False)
         self.register_buffer("cAm", cAm.to(dtype=dtype), False)
         self.register_buffer("cBm", cBm.to(dtype=dtype), False)
         self.register_buffer("cPi", cPi.to(dtype=dtype), False)
 
         ls = torch.arange(0, lmax + 1)
         nls = 2 * ls + 1
-        self.lidx = torch.repeat_interleave(ls, nls).cpu()
-        self.midx = torch.cat([torch.arange(-l_id, l_id + 1) for l_id in ls]).cpu()
+        self.lidx = torch.repeat_interleave(ls, nls)
+        self.midx = torch.cat([torch.arange(-l_id, l_id + 1) for l_id in ls])
 
         self.register_buffer("flidx", self.lidx.to(dtype=dtype), False)
 
     def _generate_Ylm_coefficients(self, lmax: int):
         """
 
         Args:
@@ -352,15 +352,14 @@
             lmax: maximum angular momentum.
         """
         super().__init__()
         self.lmax = lmax
         self.n_in = n_in
         self.lidx, _ = sh_indices(lmax)
         self.scaling = nn.Linear(n_in, n_in * (lmax + 1))
-        self.lidx = self.lidx.cpu()  # added by kenko
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         s0 = x[:, 0, :]
         h = self.scaling(s0).reshape(-1, self.lmax + 1, self.n_in)
         h = h[:, self.lidx]
         y = x * torch.sigmoid(h)
         return y
```

### Comparing `matgl-1.0.0/src/matgl/layers/_three_body.py` & `matgl-1.1.1/src/matgl/layers/_three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/layers/_zbl.py` & `matgl-1.1.1/src/matgl/layers/_zbl.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/models/_m3gnet.py` & `matgl-1.1.1/src/matgl/models/_m3gnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
         self.max_n = max_n
         self.max_l = max_l
         self.n_blocks = nblocks
         self.units = units
         self.cutoff = cutoff
         self.threebody_cutoff = threebody_cutoff
-        self.include_states = include_state
+        self.include_state = include_state
         self.task_type = task_type
         self.is_intensive = is_intensive
 
     def forward(
         self,
         g: dgl.DGLGraph,
         state_attr: torch.Tensor | None = None,
@@ -276,15 +276,15 @@
                 "edge_feat": edge_feat,
                 "state_feat": state_feat,
             }
         g.ndata["node_feat"] = node_feat
         g.edata["edge_feat"] = edge_feat
         if self.is_intensive:
             field_vec = self.readout(g)
-            readout_vec = torch.hstack([field_vec, state_feat]) if self.include_states else field_vec  # type: ignore
+            readout_vec = torch.hstack([field_vec, state_feat]) if self.include_state else field_vec  # type: ignore
             fea_dict["readout"] = readout_vec
             output = self.final_layer(readout_vec)
             if self.task_type == "classification":
                 output = self.sigmoid(output)
         else:
             g.ndata["atomic_properties"] = self.final_layer(g)
             fea_dict["readout"] = g.ndata["atomic_properties"]
```

### Comparing `matgl-1.0.0/src/matgl/models/_megnet.py` & `matgl-1.1.1/src/matgl/models/_megnet.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/models/_so3net.py` & `matgl-1.1.1/src/matgl/models/_so3net.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """DGL implementation of SO3Net.
 
-A simple spherical harmonic based equivariant GNNs. For more details on TensorNet,
+A simple spherical harmonic based equivariant GNNs. For more details on SO3Net,
 please refer to::
 
     K.T. Schütt, S.S.P. Hessmann, N.W.A. Gebauer, J. Lederer, M. Gastegger. _SchNetPack 2.0: A neural network toolbox
     for atomistic machine learning. _J. Chem. Phys. 2023, 158 (14): 144801. 10.1063/5.0138367.
 """
 
 from __future__ import annotations
```

### Comparing `matgl-1.0.0/src/matgl/models/_tensornet.py` & `matgl-1.1.1/src/matgl/models/_tensornet.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,18 @@
         units: int = 64,
         ntypes_state: int | None = None,
         dim_state_embedding: int = 0,
         dim_state_feats: int | None = None,
         include_state: bool = False,
         nblocks: int = 2,
         num_rbf: int = 32,
+        max_n: int = 3,
+        max_l: int = 3,
         rbf_type: Literal["Gaussian", "SphericalBessel"] = "Gaussian",
+        use_smooth: bool = False,
         activation_type: Literal["swish", "tanh", "sigmoid", "softplus2", "softexp"] = "swish",
         cutoff: float = 5.0,
         equivariance_invariance_group: str = "O(3)",
         dtype: torch.dtype = matgl.float_th,
         width: float = 0.5,
         readout_type: Literal["set2set", "weighted_atom", "reduce_atom"] = "weighted_atom",
         task_type: Literal["classification", "regression"] = "regression",
@@ -73,24 +76,28 @@
         **kwargs,
     ):
         r"""
 
         Args:
             element_types (tuple): List of elements appearing in the dataset. Default to DEFAULT_ELEMENTS.
             units (int, optional): Hidden embedding size.
-                (default: :obj:`128`)
+                (default: :obj:`64`)
             ntypes_state (int): Number of state labels
             dim_state_embedding (int): Number of hidden neurons in state embedding
             dim_state_feats (int): Number of state features after linear layer
             include_state (bool): Whether to include states features
             nblocks (int, optional): The number of interaction layers.
                 (default: :obj:`2`)
-            num_rbf (int, optional): The number of radial basis functions :math:`\mu`.
+            num_rbf (int, optional): The number of radial basis Gaussian functions :math:`\mu`.
                 (default: :obj:`32`)
+            max_n (int): maximum of n in spherical Bessel functions
+            max_l (int): maximum of l in spherical Bessel functions
             rbf_type (str): Radial basis function. choose from 'Gaussian' or 'SphericalBessel'
+            use_smooth (bool): Whether to use the smooth version of SphericalBessel functions.
+                This is particularly important for the smoothness of PES.
             activation_type (str): Activation type. choose from 'swish', 'tanh', 'sigmoid', 'softplus2', 'softexp'
             cutoff (float): cutoff distance for interatomic interactions.
             equivariance_invariance_group (string, optional): Group under whose action on input
                 positions internal tensor features will be equivariant and scalar predictions
                 will be invariant. O(3) or SO(3).
                (default :obj:`"O(3)"`)
             dtype (torch.dtype): data type for all variables
@@ -118,15 +125,22 @@
 
         if element_types is None:
             self.element_types = DEFAULT_ELEMENTS
         else:
             self.element_types = element_types  # type: ignore
 
         self.bond_expansion = BondExpansion(
-            cutoff=cutoff, rbf_type=rbf_type, final=cutoff + 1.0, num_centers=num_rbf, width=width
+            cutoff=cutoff,
+            rbf_type=rbf_type,
+            final=cutoff + 1.0,
+            num_centers=num_rbf,
+            width=width,
+            smooth=use_smooth,
+            max_n=max_n,
+            max_l=max_l,
         )
 
         assert equivariance_invariance_group in ["O(3)", "SO(3)"], "Unknown group representation. Choose O(3) or SO(3)."
 
         self.units = units
         self.equivariance_invariance_group = equivariance_invariance_group
         self.num_layers = nblocks
@@ -136,14 +150,18 @@
         self.cutoff = cutoff
         self.dim_state_embedding = dim_state_embedding
         self.dim_state_feats = dim_state_feats
         self.include_state = include_state
         self.ntypes_state = ntypes_state
         self.task_type = task_type
 
+        # make sure the number of radial basis functions correct for tensor embedding
+        if rbf_type == "SphericalBessel":
+            num_rbf = max_n
+
         self.tensor_embedding = TensorEmbedding(
             units=units,
             degree_rbf=num_rbf,
             dim_state_embedding=dim_state_embedding,
             dim_state_feats=dim_state_feats,
             ntypes_state=ntypes_state,
             include_state=include_state,
@@ -158,16 +176,17 @@
                 TensorNetInteraction(num_rbf, units, activation, cutoff, equivariance_invariance_group, dtype)
                 for _ in range(nblocks)
                 if nblocks != 0
             }
         )
 
         self.out_norm = nn.LayerNorm(3 * units, dtype=dtype)
+        self.linear = nn.Linear(3 * units, units, dtype=dtype)
         if is_intensive:
-            input_feats = 3 * units if field == "node_feat" else units
+            input_feats = units
             if readout_type == "set2set":
                 self.readout = Set2SetReadOut(
                     in_feats=input_feats, n_iters=niters_set2set, n_layers=nlayers_set2set, field=field
                 )
                 readout_feats = 2 * input_feats  # type: ignore
             elif readout_type == "weighted_atom":
                 self.readout = WeightedAtomReadOut(in_feats=input_feats, dims=[units, units], activation=activation)
@@ -181,15 +200,15 @@
             if task_type == "classification":
                 self.sigmoid = nn.Sigmoid()
 
         else:
             if task_type == "classification":
                 raise ValueError("Classification task cannot be extensive.")
             self.final_layer = WeightedReadOut(
-                in_feats=3 * units,
+                in_feats=units,
                 dims=[units, units],
                 num_targets=ntargets,  # type: ignore
             )
 
         self.is_intensive = is_intensive
         self.reset_parameters()
 
@@ -225,14 +244,15 @@
         # Interaction layers
         for layer in self.layers:
             X = layer(g, X)
         scalars, skew_metrices, traceless_tensors = decompose_tensor(X)
 
         x = torch.cat((tensor_norm(scalars), tensor_norm(skew_metrices), tensor_norm(traceless_tensors)), dim=-1)
         x = self.out_norm(x)
+        x = self.linear(x)
 
         g.ndata["node_feat"] = x
         if self.is_intensive:
             node_vec = self.readout(g)
             vec = node_vec  # type: ignore
             output = self.final_layer(vec)
             if self.task_type == "classification":
```

### Comparing `matgl-1.0.0/src/matgl/models/_wrappers.py` & `matgl-1.1.1/src/matgl/models/_wrappers.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/utils/cutoff.py` & `matgl-1.1.1/src/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/utils/io.py` & `matgl-1.1.1/src/matgl/utils/io.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/utils/maths.py` & `matgl-1.1.1/src/matgl/utils/maths.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/utils/sb_roots.npy` & `matgl-1.1.1/src/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/src/matgl/utils/so3.py` & `matgl-1.1.1/src/matgl/utils/so3.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     Generate standard Clebsch-Gordan coefficients for complex spherical harmonics.
 
     Args:
         lmax: maximum angular momentum.
     """
     lidx, midx = sh_indices(lmax)
     cg = torch.zeros((lidx.shape[0], lidx.shape[0], lidx.shape[0]))
-    lidx = lidx.cpu().numpy()
-    midx = midx.cpu().numpy()
+    lidx = lidx.numpy()
+    midx = midx.numpy()
     for c1, (l1, m1) in enumerate(zip(lidx, midx)):
         for c2, (l2, m2) in enumerate(zip(lidx, midx)):
             for c3, (l3, m3) in enumerate(zip(lidx, midx)):
                 if abs(l1 - l2) <= l3 <= min(l1 + l2, lmax) and m3 in {
                     m1 + m2,
                     m1 - m2,
                     m2 - m1,
```

### Comparing `matgl-1.0.0/src/matgl/utils/training.py` & `matgl-1.1.1/src/matgl/utils/training.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utils for training MatGL models."""
 
 from __future__ import annotations
 
 import math
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING, Any, Literal
 
 import pytorch_lightning as pl
 import torch
 import torch.nn.functional as F
 import torchmetrics
 from torch import nn
 
@@ -115,15 +115,14 @@
         Executed on model testing.
 
         Args:
             *args: Pass-through
             **kwargs: Pass-through.
         """
         super().on_test_model_eval(*args, **kwargs)
-        torch.set_grad_enabled(True)
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
         """
         Prediction step.
 
         Args:
             batch: Data batch.
@@ -261,86 +260,107 @@
         self,
         model,
         element_refs: np.ndarray | None = None,
         include_line_graph: bool = False,
         energy_weight: float = 1.0,
         force_weight: float = 1.0,
         stress_weight: float = 0.0,
-        site_wise_weight: float = 0.0,
+        magmom_weight: float = 0.0,
         data_mean: float = 0.0,
         data_std: float = 1.0,
         loss: str = "mse_loss",
+        loss_params: dict | None = None,
         optimizer: Optimizer | None = None,
         scheduler=None,
         lr: float = 0.001,
         decay_steps: int = 1000,
         decay_alpha: float = 0.01,
         sync_dist: bool = False,
+        allow_missing_labels: bool = False,
+        magmom_target: Literal["absolute", "symbreak"] | None = "absolute",
         **kwargs,
     ):
         """
         Init PotentialLightningModule with key parameters.
 
         Args:
             model: Which type of the model for training
             element_refs: element offset for PES
             include_line_graph: whether to include line graphs
             energy_weight: relative importance of energy
             force_weight: relative importance of force
             stress_weight: relative importance of stress
-            site_wise_weight: relative importance of additional site-wise predictions.
+            magmom_weight: relative importance of additional magmom predictions.
             data_mean: average of training data
             data_std: standard deviation of training data
             loss: loss function used for training
+            loss_params: parameters for loss function
             optimizer: optimizer for training
             scheduler: scheduler for training
             lr: learning rate for training
             decay_steps: number of steps for decaying learning rate
             decay_alpha: parameter determines the minimum learning rate.
             sync_dist: whether sync logging across all GPU workers or not
+            allow_missing_labels: Whether to allow missing labels or not.
+                These should be present in the dataset as torch.nans and will be skipped in computing the loss.
+            magmom_target: Whether to predict the absolute site-wise value of magmoms or adapt the loss function
+                to predict the signed value breaking symmetry. If None given the loss function will be adapted.
             **kwargs: Passthrough to parent init.
         """
         assert energy_weight >= 0, f"energy_weight has to be >=0. Got {energy_weight}!"
         assert force_weight >= 0, f"force_weight has to be >=0. Got {force_weight}!"
         assert stress_weight >= 0, f"stress_weight has to be >=0. Got {stress_weight}!"
-        assert site_wise_weight >= 0, f"site_wise_weight has to be >=0. Got {site_wise_weight}!"
+        assert magmom_weight >= 0, f"magmom_weight has to be >=0. Got {magmom_weight}!"
 
         super().__init__(**kwargs)
 
         self.mae = torchmetrics.MeanAbsoluteError()
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
         self.register_buffer("data_mean", torch.tensor(data_mean))
         self.register_buffer("data_std", torch.tensor(data_std))
 
         self.energy_weight = energy_weight
         self.force_weight = force_weight
         self.stress_weight = stress_weight
-        self.site_wise_weight = site_wise_weight
+        self.magmom_weight = magmom_weight
         self.lr = lr
         self.decay_steps = decay_steps
         self.decay_alpha = decay_alpha
         self.include_line_graph = include_line_graph
 
         self.model = Potential(
             model=model,
             element_refs=element_refs,
             calc_stresses=stress_weight != 0,
-            calc_site_wise=site_wise_weight != 0,
+            calc_magmom=magmom_weight != 0,
             data_std=self.data_std,
             data_mean=self.data_mean,
         )
         if loss == "mse_loss":
             self.loss = F.mse_loss
+        elif loss == "huber_loss":
+            self.loss = F.huber_loss
         else:
             self.loss = F.l1_loss
+        self.loss_params = loss_params if loss_params is not None else {}
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.sync_dist = sync_dist
+        self.allow_missing_labels = allow_missing_labels
+        self.magmom_target = magmom_target
         self.save_hyperparameters(ignore=["model"])
 
+    def on_load_checkpoint(self, checkpoint: dict[str, Any]):
+        """# noqa: D200
+        hacky hacky hack to add missing keys to the state dict when changes are made.
+        """
+        for key in self.state_dict():
+            if key not in checkpoint["state_dict"]:
+                checkpoint["state_dict"][key] = self.state_dict()[key]
+
     def forward(
         self,
         g: dgl.DGLGraph,
         lat: torch.Tensor,
         l_g: dgl.DGLGraph | None = None,
         state_attr: torch.Tensor | None = None,
     ):
@@ -350,39 +370,40 @@
             l_g: Line graph
             state_attr: State attr.
 
         Returns:
             energy, force, stress, hessian and optional site_wise
         """
         if self.include_line_graph:
-            if self.model.calc_site_wise:
+            if self.model.calc_magmom:
                 e, f, s, h, m = self.model(g=g, lat=lat, l_g=l_g, state_attr=state_attr)
                 return e, f, s, h, m
             e, f, s, h = self.model(g=g, lat=lat, l_g=l_g, state_attr=state_attr)
             return e, f, s, h
-        e, f, s, h = self.model(g=g, lat=lat, state_attr=state_attr)
-        return e, f, s, h
+        else:  # noqa: RET505
+            e, f, s, h = self.model(g=g, lat=lat, state_attr=state_attr)
+            return e, f, s, h
 
     def step(self, batch: tuple):
         """Args:
             batch: Batch of training data.
 
         Returns:
             results, batch_size
         """
         preds: tuple
         labels: tuple
 
         torch.set_grad_enabled(True)
         if self.include_line_graph:
-            if self.model.calc_site_wise:
-                g, lat, l_g, state_attr, energies, forces, stresses, site_wise = batch
+            if self.model.calc_magmom:
+                g, lat, l_g, state_attr, energies, forces, stresses, magmoms = batch
                 e, f, s, _, m = self(g=g, lat=lat, state_attr=state_attr, l_g=l_g)
                 preds = (e, f, s, m)
-                labels = (energies, forces, stresses, site_wise)
+                labels = (energies, forces, stresses, magmoms)
             else:
                 g, lat, l_g, state_attr, energies, forces, stresses = batch
                 e, f, s, _ = self(g=g, lat=lat, state_attr=state_attr, l_g=l_g)
                 preds = (e, f, s)
                 labels = (energies, forces, stresses)
         else:
             g, lat, state_attr, energies, forces, stresses = batch
@@ -419,23 +440,25 @@
         Returns::
 
             {
                 "Total_Loss": total_loss,
                 "Energy_MAE": e_mae,
                 "Force_MAE": f_mae,
                 "Stress_MAE": s_mae,
+                "Magmom_MAE": m_mae,
                 "Energy_RMSE": e_rmse,
                 "Force_RMSE": f_rmse,
                 "Stress_RMSE": s_rmse,
+                "Magmom_RMSE": m_rmse
             }
 
         """
         # labels and preds are (energy, force, stress, (optional) site_wise)
-        e_loss = self.loss(labels[0] / num_atoms, preds[0] / num_atoms)
-        f_loss = self.loss(labels[1], preds[1])
+        e_loss = self.loss(labels[0] / num_atoms, preds[0] / num_atoms, **self.loss_params)
+        f_loss = self.loss(labels[1], preds[1], **self.loss_params)
 
         e_mae = self.mae(labels[0] / num_atoms, preds[0] / num_atoms)
         f_mae = self.mae(labels[1], preds[1])
 
         e_rmse = self.rmse(labels[0] / num_atoms, preds[0] / num_atoms)
         f_rmse = self.rmse(labels[1], preds[1])
 
@@ -444,35 +467,58 @@
 
         m_mae = torch.zeros(1)
         m_rmse = torch.zeros(1)
 
         total_loss = self.energy_weight * e_loss + self.force_weight * f_loss
 
         if self.model.calc_stresses:
-            s_loss = loss(labels[2], preds[2])
+            s_loss = loss(labels[2], preds[2], **self.loss_params)
             s_mae = self.mae(labels[2], preds[2])
             s_rmse = self.rmse(labels[2], preds[2])
             total_loss = total_loss + self.stress_weight * s_loss
 
-        if self.model.calc_site_wise:
-            m_loss = loss(labels[3], preds[3])
-            m_mae = self.mae(labels[3], preds[3])
-            m_rmse = self.rmse(labels[3], preds[3])
-            total_loss = total_loss + self.site_wise_weight * m_loss
+        if self.model.calc_magmom:
+            if self.allow_missing_labels:
+                valid_values = ~torch.isnan(labels[3])
+                labels_3 = labels[3][valid_values]
+                preds_3 = preds[3][valid_values]
+            else:
+                labels_3 = labels[3]
+                preds_3 = preds[3]
+
+            if len(labels_3) > 0:
+                if self.magmom_target == "symbreak":
+                    m_loss = torch.min(
+                        loss(labels_3, preds_3, **self.loss_params), loss(labels_3, -preds_3, **self.loss_params)
+                    )
+                    m_mae = torch.min(self.mae(labels_3, preds_3), self.mae(labels_3, -preds_3))
+                    m_rmse = torch.min(self.rmse(labels_3, preds_3), self.rmse(labels_3, -preds_3))
+                else:
+                    if self.magmom_target == "absolute":
+                        labels_3 = torch.abs(labels_3)
+
+                    m_loss = loss(labels_3, preds_3, **self.loss_params)
+                    m_mae = self.mae(labels_3, preds_3)
+                    m_rmse = self.rmse(labels_3, preds_3)
+
+                total_loss = total_loss + self.magmom_weight * m_loss
+            else:
+                m_mae = torch.zeros(1)
+                m_rmse = torch.zeros(1)
 
         return {
             "Total_Loss": total_loss,
             "Energy_MAE": e_mae,
             "Force_MAE": f_mae,
             "Stress_MAE": s_mae,
-            "Site_Wise_MAE": m_mae,
+            "Magmom_MAE": m_mae,
             "Energy_RMSE": e_rmse,
             "Force_RMSE": f_rmse,
             "Stress_RMSE": s_rmse,
-            "Site_Wise_RMSE": m_rmse,
+            "Magmom_RMSE": m_rmse,
         }
 
 
 def xavier_init(model: nn.Module, gain: float = 1.0, distribution: Literal["uniform", "normal"] = "uniform") -> None:
     """Xavier initialization scheme for the model.
 
     Args:
```

### Comparing `matgl-1.0.0/src/matgl.egg-info/PKG-INFO` & `matgl-1.1.1/src/matgl.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 1.0.0
+Version: 1.1.1
 Summary: MatGL is a framework for graph deep learning for materials science.
-Author-email: Tsz Wai Ko <t1ko@ucsd.edu>, Marcel Nassar <marcel.nassar@intel.com>, Ji Qi <j1qi@ucsd.edu>, Santiago Miret <santiago.miret@intel.com>, Eliott Liu <elliottliu17@gmail.com>, Shyue Ping Ong <ongsp@ucsd.edu>
+Author-email: Tsz Wai Ko <t1ko@ucsd.edu>, Marcel Nassar <marcel.nassar@intel.com>, Ji Qi <j1qi@ucsd.edu>, Santiago Miret <santiago.miret@intel.com>, Eliott Liu <elliottliu17@gmail.com>, Bowen Deng <bowendeng@berkeley.edu>, Luis Barroso-Luque <lbluque@berkeley.edu>, Shyue Ping Ong <ongsp@ucsd.edu>
 License: BSD-3-Clause
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
@@ -17,18 +17,19 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ase
-Requires-Dist: dgl
+Requires-Dist: dgl>=2.0.0
 Requires-Dist: pymatgen
 Requires-Dist: pytorch_lightning
-Requires-Dist: torch
+Requires-Dist: torch<=2.2.1
+Requires-Dist: pydantic
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml/badge.svg)](https://github.com/materialsvirtuallab/matgl/actions/workflows/testing.yml)
 [![Downloads](https://static.pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 [![codecov](https://codecov.io/gh/materialsvirtuallab/matgl/branch/main/graph/badge.svg?token=3V3O79GODQ)](https://codecov.io/gh/materialsvirtuallab/matgl)
 [![PyPI](https://img.shields.io/pypi/v/matgl?logo=pypi&logoColor=white)](https://pypi.org/project/matgl?logo=pypi&logoColor=white)
@@ -43,28 +44,24 @@
 
 MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
 natural representation for a collection of atoms. Graph deep learning models have been shown to consistently deliver
 exceptional performance as surrogate models for the prediction of materials properties.
 
 MatGL is built on the [Deep Graph Library (DGL)][dgl] and PyTorch, with suitable adaptations for materials-specific
 applications. The goal is for MatGL to serve as an extensible platform to develop and share materials graph deep
-learning models. For the initial release, we have re-implemented the [MatErials 3-body Graph Network (M3GNet)]
-[m3gnet] and its predecessor, [MEGNet][megnet], which were originally implemented in Tensorflow, to improve the
-usability, extensibility and scalability of these models. Here are some key improvements over the TF implementations:
-
-- A more intuitive API and class structure based on DGL.
-- Multi-GPU support via PyTorch Lightning.
+learning models, including the [MatErials 3-body Graph Network (M3GNet)][m3gnet] and its predecessor, [MEGNet].
 
 This effort is a collaboration between the [Materials Virtual Lab][mavrl] and Intel Labs (Santiago Miret, Marcel
 Nassar, Carmelo Gonzales).
 
 ## Status
 
 Major milestones are summarized below. Please refer to the [changelog] for details.
 
+- v1.0.0 (Feb 14 2024): Implementation of [TensorNet] and [SO3Net].
 - v0.5.1 (Jun 9 2023): Model versioning implemented.
 - v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
 - v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
 - v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
   bugs!
 
@@ -75,22 +72,14 @@
 in future.
 
 <div style="float: left; padding: 10px; width: 300px">
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic">
 <p>Figure: Schematic of M3GNet/MEGNet</p>
 </div>
 
-### MEGNet
-
-[MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
-machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
-array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
-[multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
-network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an output graph.
-
 ### M3GNet
 
 [Materials 3-body Graph Network (M3GNet)][m3gnet] is a new materials graph neural network architecture that
 incorporates 3-body interactions in MEGNet. An additional difference is the addition of the coordinates for atoms and
 the 3×3 lattice matrix in crystals, which are necessary for obtaining tensorial quantities such as forces and
 stresses via auto-differentiation. As a framework, M3GNet has diverse applications, including:
 
@@ -101,14 +90,37 @@
   performed in the [Materials Project][mp].
 - **Surrogate models for property predictions.** Like the previous MEGNet architecture, M3GNet can be used to develop
   surrogate models for property predictions, achieving in many cases accuracies that are better or similar to other
   state-of-the-art ML models.
 
 For detailed performance benchmarks, please refer to the publications in the [References](#references) section.
 
+MatGL reimplemennts M3GNet using DGL and Pytorch. Compared to the original Tensorflow implementation, some key
+improvements over the TF implementations are:
+
+- A more intuitive API and class structure based on DGL.
+- Multi-GPU support via PyTorch Lightning.
+
+### MEGNet
+
+[MatErials Graph Network (MEGNet)][megnet] is an implementation of DeepMind's [graph networks][graphnetwork] for
+machine learning in materials science. We have demonstrated its success in achieving low prediction errors in a broad
+array of properties in both [molecules and crystals][megnet]. New releases have included our recent work on
+[multi-fidelity materials property modeling][mfimegnet]. Figure 1 shows the sequential update steps of the graph
+network, whereby bonds, atoms, and global state attributes are updated using information from each other, generating an
+output graph.
+
+### Other models
+
+We have implemented other models in matgl as well. A non-exhaustive list is given below.
+
+- [TensorNet], an O(3)-equivariant message-passing neural network architecture that
+  leverages Cartesian tensor representations.
+- [SO3Net],  a minimalist SO(3)-equivariant neural network.
+
 ## Installation
 
 Matgl can be installed via pip for the latest stable version:
 
 ```bash
 pip install matgl
 ```
@@ -298,7 +310,9 @@
 [apidocs]: https://matgl.ai/matgl.html "MatGL API docs"
 [doc]: https://matgl.ai "MatGL Documentation"
 [google colab]: https://colab.research.google.com/ "Google Colab"
 [jupyternb]: https://github.com/materialsvirtuallab/matgl/tree/main/examples
 [ongemail]: mailto:ongsp@ucsd.edu "Email"
 [mqm]: https://materialsqm.com "MaterialsQM"
 [tutorials]: https://matgl.ai/tutorials "Tutorials"
+[tensornet]: https://arxiv.org/abs/2306.06482 "TensorNet"
+[so3net]: https://pubs.aip.org/aip/jcp/article-abstract/158/14/144801/2877924/SchNetPack-2-0-A-neural-network-toolbox-for "SO3Net"
```

### Comparing `matgl-1.0.0/src/matgl.egg-info/SOURCES.txt` & `matgl-1.1.1/src/matgl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,21 @@
 src/matgl/layers/_activations.py
 src/matgl/layers/_atom_ref.py
 src/matgl/layers/_basis.py
 src/matgl/layers/_bond.py
 src/matgl/layers/_core.py
 src/matgl/layers/_embedding.py
 src/matgl/layers/_graph_convolution.py
+src/matgl/layers/_norm.py
 src/matgl/layers/_readout.py
 src/matgl/layers/_so3.py
 src/matgl/layers/_three_body.py
 src/matgl/layers/_zbl.py
 src/matgl/models/__init__.py
+src/matgl/models/_chgnet.py
 src/matgl/models/_m3gnet.py
 src/matgl/models/_megnet.py
 src/matgl/models/_so3net.py
 src/matgl/models/_tensornet.py
 src/matgl/models/_wrappers.py
 src/matgl/utils/__init__.py
 src/matgl/utils/cutoff.py
```

### Comparing `matgl-1.0.0/tests/test_cli.py` & `matgl-1.1.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/tests/test_default_dtype.py` & `matgl-1.1.1/tests/test_default_dtype.py`

 * *Files identical despite different names*

### Comparing `matgl-1.0.0/tests/test_integration.py` & `matgl-1.1.1/tests/test_integration.py`

 * *Files identical despite different names*


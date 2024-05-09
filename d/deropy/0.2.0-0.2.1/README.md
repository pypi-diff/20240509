# Comparing `tmp/deropy-0.2.0.tar.gz` & `tmp/deropy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deropy-0.2.0.tar", last modified: Wed May  8 16:20:59 2024, max compression
+gzip compressed data, was "deropy-0.2.1.tar", last modified: Thu May  9 08:53:30 2024, max compression
```

## Comparing `deropy-0.2.0.tar` & `deropy-0.2.1.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.619024 deropy-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-08 16:20:54.000000 deropy-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-08 16:20:59.615024 deropy-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-08 16:20:54.000000 deropy-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.603024 deropy-0.2.0/deropy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.603024 deropy-0.2.0/deropy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/commands/transpile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.603024 deropy-0.2.0/deropy/dvm/
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/Smartcontract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/Wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.607024 deropy-0.2.0/deropy/dvm/dast/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/assignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/binaryOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/dast_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/declaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/functionCall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/functionDef.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/goto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/ifTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/variableDeclarationAdnAssignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/dast/whileLoop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.611024 deropy-0.2.0/deropy/dvm/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/AddressRaw.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/AddressString.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/AssetValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Atoi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Blid.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/BlockHeight.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/BlockTimestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Dero.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/DeroValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Function.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/HexDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/IsAddressValid.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Itoa.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/MapDelete.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/MapExists.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/MapGet.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/MapStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Panic.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Random.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Scid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/SendAssetToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/SendDeroToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Sha3256.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Signer.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Store.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Strlen.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Substr.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/Txid.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/UpdateScCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.615024 deropy-0.2.0/deropy/dvm/iast/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/IastNode.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/assignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/binaryOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/functionCall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/functionDef.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/iast_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/ifTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/variableDeclarationAdnAssignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/iast/whileLoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/dvm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.615024 deropy-0.2.0/deropy/python_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/Nameservice.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/lottery.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/minimum_sc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/python_templates/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-08 16:20:54.000000 deropy-0.2.0/deropy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.615024 deropy-0.2.0/deropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 16:20:59.000000 deropy-0.2.0/deropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:20:59.619024 deropy-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 16:20:54.000000 deropy-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:20:59.615024 deropy-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-08 16:20:54.000000 deropy-0.2.0/tests/test_compute_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-08 16:20:54.000000 deropy-0.2.0/tests/test_map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-08 16:20:54.000000 deropy-0.2.0/tests/test_storage_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-09 08:53:26.000000 deropy-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-09 08:53:30.553107 deropy-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-09 08:53:26.000000 deropy-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.537107 deropy-0.2.1/deropy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.537107 deropy-0.2.1/deropy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/commands/transpile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.537107 deropy-0.2.1/deropy/dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/Smartcontract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/Wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.541107 deropy-0.2.1/deropy/dvm/dast/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/assignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/binaryOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/dast_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/declaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/functionCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/functionDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/goto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/ifTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/variableDeclarationAdnAssignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/dast/whileLoop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.549107 deropy-0.2.1/deropy/dvm/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/AddressRaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/AddressString.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/AssetValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Atoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Blid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/BlockHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/BlockTimestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Dero.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/DeroValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/HexDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/IsAddressValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Itoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/MapDelete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/MapExists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/MapGet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/MapStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Panic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Scid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/SendAssetToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/SendDeroToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Sha3256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Strlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Substr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/Txid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/UpdateScCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/deropy/dvm/iast/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/IastNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/assignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/binaryOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/functionCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/functionDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/iast_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/ifTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/variableDeclarationAdnAssignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/iast/whileLoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/dvm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/deropy/python_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/Nameservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/lottery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/minimum_sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/python_templates/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 08:53:26.000000 deropy-0.2.1/deropy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/deropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 08:53:30.000000 deropy-0.2.1/deropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:53:30.553107 deropy-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 08:53:26.000000 deropy-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:53:30.553107 deropy-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-09 08:53:26.000000 deropy-0.2.1/tests/test_compute_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-09 08:53:26.000000 deropy-0.2.1/tests/test_map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-09 08:53:26.000000 deropy-0.2.1/tests/test_storage_functions.py
```

### Comparing `deropy-0.2.0/LICENSE` & `deropy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/PKG-INFO` & `deropy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.2.0/README.md` & `deropy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/commands/configure.py` & `deropy-0.2.1/deropy/commands/configure.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/commands/deploy.py` & `deropy-0.2.1/deropy/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/commands/generate.py` & `deropy-0.2.1/deropy/commands/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,20 +221,17 @@
     payload += [
         '                    ]',
         '                }',
         '            }',
     ]
     lines.extend(payload)
     lines += [
-        '        import pprint',
-        '        pprint.pprint(payload)',
         '        url = self.url if host is None else host',
-        '        print(f"using url {url}")',
-        '        response = requests.post(url, data=json.dumps(payload), headers=self.headers)',
-        '        pprint.pprint(response.json())']
+        '        response = requests.post(url, data=json.dumps(payload), headers=self.headers)'
+    ]
     return lines
 
 
 def _generate_method_transfer2(f_name, p):
     # create the method definition
     method_parameters = ''
     for k, v in p.items():
@@ -278,15 +275,14 @@
     payload += [
         '                    ]',
         '                }',
         '            }',
     ]
     lines.extend(payload)
     lines += ['        response = requests.post(self.url, data=json.dumps(payload), headers=self.headers)']
-    lines += ['        print(response.json())']
     return lines
 
 
 def _SC_type_to_python_type(t: str):
     if t == 'String':
         return 'str'
```

### Comparing `deropy-0.2.0/deropy/commands/simulate.py` & `deropy-0.2.1/deropy/commands/simulate.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,26 +43,17 @@
 def _simulate(simulator, sc_file, tests_file):
     if not check(simulator, sc_file, tests_file):
         return
 
     smart_contract_name = os.path.basename(sc_file).split('.')[0].lower()
     transpile_path = os.path.join(get_working_directory(), f'{smart_contract_name}.bas')
     api_path = os.path.join(get_working_directory(), f'{smart_contract_name}_api.py')
-
-    # Execute the DEROHE Simualtor
-    # We do it into a thread because we don't want to block the main thread
-    # We need to read the output from the simulator to know when it is ready to receive requests
-    # Read the output from the simulator until the Listening for requests message is displayed
-    print('Executing the DEROHE simulator')
-    p = subprocess.Popen([simulator], stdout=subprocess.PIPE, bufsize=1, close_fds=ON_POSIX)
     q = Queue()
-    t = threading.Thread(target=enqueue_output, args=(p.stdout, q))
-    t.daemon = True
-    t.start()
-    read_until(q, 'Listening for requests')
+
+    start_derohe_simulator(simulator, q)
 
     # Transpile the python smart-contract into a DEROHE smart-contract
     print('Transpiling the smart contract')
     _transpile(sc_file, transpile_path)
 
     # Deploy the smart-contract to the simulator
     print('Deploying the smart contract')
@@ -70,35 +61,46 @@
     read_until(q, "interpreting line [RETURN 0]   err:'<nil>'", 20)
 
     # Generate the API
     print('Generating the API')
     _generate(transpile_path, txid, 'simulator', api_path)
 
     # Execute the tests in the simulator
-    t = threading.Thread(target=stream_output, args=(q,))
-    t.daemon = True
-    t.start()
     print('Executing the tests')
     os.environ['API_PATH'] = f"{api_path}"
     pytest.main([tests_file, '-vxs'])
 
     # Finish reading the output from the simulator
     read_until_empty(q)
 
-    # Close the simulator
-    p.terminate()
-    p.wait()
+
+def start_derohe_simulator(simulator, q):
+    # We do it into a thread because we don't want to block the main thread
+    # We need to read the output from the simulator to know when it is ready to receive requests
+    # Read the output from the simulator until the Listening for requests message is displayed
+    print('Executing the DEROHE simulator')
+    p = subprocess.Popen([simulator], stdout=subprocess.PIPE, bufsize=1, close_fds=ON_POSIX)
+    t = threading.Thread(target=enqueue_output, args=(p.stdout, q))
+    t.daemon = True
+    t.start()
+    read_until(q, 'Listening for requests')
 
 
 def enqueue_output(out, queue):
     for line in iter(out.readline, b''):
         queue.put(line)
     out.close()
 
 
+def start_output_stream(q):
+    t = threading.Thread(target=stream_output, args=(q,))
+    t.daemon = True
+    t.start()
+
+
 def stream_output(queue):
     while True:
         try:
             line = queue.get_nowait()
         except Empty:
             time.sleep(0.1)
             continue
```

### Comparing `deropy-0.2.0/deropy/dvm/Smartcontract.py` & `deropy-0.2.1/deropy/dvm/Smartcontract.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/Wallet.py` & `deropy-0.2.1/deropy/dvm/Wallet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import hashlib
 import requests
 import time
+import logging
+
+
+from deropy.utils import active_waiting
 from deropy.dvm.Smartcontract import SmartContract
 
 
 class Wallet:
     def __init__(self, name, id, simulator: bool = False):
-        print(f'Creating wallet "{name}" (simulator: {simulator})')
+        self.logger = logging.getLogger('deropy')
+        self.logger.info(f'Creating wallet "{name}" (simulator: {simulator})')
         self.name = name
         self.id = id
         self.simulator = simulator
         wallet_port = 30000 + self.id
         self.rpc_host = f'http://127.0.0.1:{wallet_port}/json_rpc'
 
         if not simulator:
@@ -23,15 +28,15 @@
         self.raw_address = self.string_address[:33]
         self.balance = {}
 
     def _simulator_init(self):
         self.string_address = self._get_string_address()
         self.raw_address = self._get_raw_address()
 
-        print(f'Wallet "{self.name}" created: {self.string_address} - {self.raw_address} - "{self.name}')
+        self.logger.info(f'Wallet "{self.name}" created: {self.string_address} - {self.raw_address} - "{self.name}')
         self.balance = {}
 
     def _get_string_address(self):
         payload = {
             "jsonrpc": "2.0",
             "id": "1",
             "method": "GetAddress"
@@ -59,15 +64,15 @@
                             "datatype": "S",
                             "value": self.name
                         }
                     ]
                 }
             }
             response = requests.post(self.rpc_host, json=payload).json()
-            
+
             if "error" in response:
                 waiting_time = 5
                 active_waiting(f'Wallet not yet registered, trying again in {waiting_time}', waiting_time)
                 return register(self, timeout + waiting_time)
             return response
 
         def get_raw_address(self):
@@ -93,29 +98,29 @@
     def from_public_key(cls, public_key):
         wallet = cls(public_key, 1000)
         wallet.string_address = public_key
         wallet.raw_address = public_key[:33]
         return wallet
 
     def invoke_sc_function(self, func, func_args: tuple = None, dero_deposit: int = None, asset_deposit: tuple = None):
-        print(f'Invoking function "{func.__name__}({func_args})" in wallet "{self.name}" using {dero_deposit} DERO and {asset_deposit} assets')
+        self.logger.info(f'Invoking function "{func.__name__}({func_args})" in wallet "{self.name}" using {dero_deposit} DERO and {asset_deposit} assets')
         WalletSimulator.active_wallet = self.name
 
         if dero_deposit is not None:
             SmartContract.send_dero_with_tx(dero_deposit)
         if asset_deposit is not None:
             SmartContract.send_asset_with_tx(asset_deposit[0], asset_deposit[1])
 
         # Prepare the SC function parameters (can change if running in simulator)
         args = [] if func_args is None else (func_args, ) if isinstance(func_args, (int, str)) else func_args
         kwargs = {'dero_deposit': dero_deposit, 'asset_deposit': asset_deposit, 'host': self.rpc_host}
 
         if self.simulator:
             result = func(*args, **kwargs)
-            print('in simulator, waiting 2 seconds to simulate transaction')
+            self.logger.debug('in simulator, waiting 2 seconds to simulate transaction')
             time.sleep(2)
             return result
 
         return func(*args)
 
     def get_balance(self, token):
         return self.balance.get(token, 0)
@@ -129,15 +134,15 @@
     wallets = {}
     wallet_count = 0
 
     @staticmethod
     def create_wallet(name, simulator: bool = False):
         if WalletSimulator.wallet_count >= 20:
             raise Exception("Maximum number of wallets reached")
-        
+
         WalletSimulator.wallets[name] = Wallet(name, WalletSimulator.wallet_count, simulator)
         WalletSimulator.wallet_count += 1
         return WalletSimulator.wallets[name]
 
     @staticmethod
     def create_wallet_from_public_key(name, public_key):
         WalletSimulator.wallets[name] = Wallet.from_public_key(public_key)
@@ -151,20 +156,20 @@
 
     @staticmethod
     def find_wallet_id_from_raw(raw_address):
         for id, wallet in WalletSimulator.wallets.items():
             if wallet.raw_address == raw_address:
                 return id
         raise Exception("Wallet not found")
-    
+
     @staticmethod
     def get_wallet_from_raw(raw_address):
         id = WalletSimulator.find_wallet_id_from_raw(raw_address)
         return WalletSimulator.get_wallet_from_id(id)
-    
+
     @staticmethod
     def get_wallet_from_id(id):
         return WalletSimulator.wallets[id]
 
     @staticmethod
     def get_raw_address():
         return WalletSimulator.wallets[WalletSimulator.active_wallet].raw_address
@@ -179,17 +184,7 @@
 
     def get_string_address_from_id(id):
         return WalletSimulator.wallets[id].string_address
 
     @staticmethod
     def is_initialized():
         return WalletSimulator.active_wallet is not None
-    
-
-def active_waiting(msg: str, timeout: int):
-    start = time.time()
-
-    while time.time() - start < timeout:
-        for char in ['|', '/', '-', '\\']:
-            print(f'{msg} {char}', end='\r')
-            time.sleep(0.1)
-    print('')
```

### Comparing `deropy-0.2.0/deropy/dvm/dast/__init__.py` & `deropy-0.2.1/deropy/dvm/dast/__init__.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/argument.py` & `deropy-0.2.1/deropy/dvm/dast/argument.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/assignement.py` & `deropy-0.2.1/deropy/dvm/dast/assignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/binaryOperator.py` & `deropy-0.2.1/deropy/dvm/dast/binaryOperator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/compare.py` & `deropy-0.2.1/deropy/dvm/dast/compare.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/dast_converter.py` & `deropy-0.2.1/deropy/dvm/dast/dast_converter.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/declaration.py` & `deropy-0.2.1/deropy/dvm/dast/declaration.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/functionCall.py` & `deropy-0.2.1/deropy/dvm/dast/functionCall.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/functionDef.py` & `deropy-0.2.1/deropy/dvm/dast/functionDef.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/ifTest.py` & `deropy-0.2.1/deropy/dvm/dast/ifTest.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/operator.py` & `deropy-0.2.1/deropy/dvm/dast/operator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/returns.py` & `deropy-0.2.1/deropy/dvm/dast/returns.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/variableDeclarationAdnAssignement.py` & `deropy-0.2.1/deropy/dvm/dast/variableDeclarationAdnAssignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/dast/whileLoop.py` & `deropy-0.2.1/deropy/dvm/dast/whileLoop.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/AddressRaw.py` & `deropy-0.2.1/deropy/dvm/functions/AddressRaw.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/AddressString.py` & `deropy-0.2.1/deropy/dvm/functions/AddressString.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/AssetValue.py` & `deropy-0.2.1/deropy/dvm/functions/AssetValue.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class AssetValue(Function):
     def __init__(self):
         func_parameters = {
             "asset": {"type": "str", "value": None},
         }
-        super().__init__("asset_value", 10_000, 0, func_parameters)
+        super().__init__("assetvalue", 10_000, 0, func_parameters)
 
     def _exec(self, *args, **kwargs):
         asset_id = kwargs["asset"]
 
         if SmartContract.asset_value is None:
             return 0
         if asset_id not in SmartContract.asset_value:
@@ -20,9 +20,9 @@
         self.parameters["asset"]["value"] = asset_id
         return SmartContract.asset_value[asset_id]
 
     def _computeGasStorageCost(self):
         return 0
 
 
-def asset_value(asset: str):
+def assetvalue(asset: str):
     return AssetValue()(asset=asset)
```

### Comparing `deropy-0.2.0/deropy/dvm/functions/Atoi.py` & `deropy-0.2.1/deropy/dvm/functions/Atoi.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/BlockHeight.py` & `deropy-0.2.1/deropy/dvm/functions/BlockHeight.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Dero.py` & `deropy-0.2.1/deropy/dvm/functions/Dero.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/DeroValue.py` & `deropy-0.2.1/deropy/dvm/functions/DeroValue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from deropy.dvm.functions.Function import Function
 from deropy.dvm.Smartcontract import SmartContract
 
 
 class DeroValue(Function):
     def __init__(self):
         func_parameters = {}
-        super().__init__("dero_value", 10_000, 0, func_parameters)
+        super().__init__("derovalue", 10_000, 0, func_parameters)
 
     def _exec(self, *args, **kwargs):
         if SmartContract.dero_value is None:
             return 0
         if SmartContract.dero_value < 0:
             return 0
         return SmartContract.dero_value
 
     def _computeGasStorageCost(self):
         return 0
 
 
-def dero_value():
+def derovalue():
     return DeroValue()()
```

### Comparing `deropy-0.2.0/deropy/dvm/functions/Exists.py` & `deropy-0.2.1/deropy/dvm/functions/Exists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Function.py` & `deropy-0.2.1/deropy/dvm/functions/Function.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/IsAddressValid.py` & `deropy-0.2.1/deropy/dvm/functions/IsAddressValid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Itoa.py` & `deropy-0.2.1/deropy/dvm/functions/Itoa.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Keccak256.py` & `deropy-0.2.1/deropy/dvm/functions/Keccak256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Load.py` & `deropy-0.2.1/deropy/dvm/functions/Load.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/MapExists.py` & `deropy-0.2.1/deropy/dvm/functions/MapExists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/MapStore.py` & `deropy-0.2.1/deropy/dvm/functions/MapStore.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Random.py` & `deropy-0.2.1/deropy/dvm/functions/Random.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Scid.py` & `deropy-0.2.1/deropy/dvm/functions/Scid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/SendAssetToAddress.py` & `deropy-0.2.1/deropy/dvm/functions/SendAssetToAddress.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/SendDeroToAddress.py` & `deropy-0.2.1/deropy/dvm/functions/SendDeroToAddress.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Sha256.py` & `deropy-0.2.1/deropy/dvm/functions/Sha256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Sha3256.py` & `deropy-0.2.1/deropy/dvm/functions/Sha3256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Signer.py` & `deropy-0.2.1/deropy/dvm/functions/Signer.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Store.py` & `deropy-0.2.1/deropy/dvm/functions/Store.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/Substr.py` & `deropy-0.2.1/deropy/dvm/functions/Substr.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/UpdateScCode.py` & `deropy-0.2.1/deropy/dvm/functions/UpdateScCode.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/functions/__init__.py` & `deropy-0.2.1/deropy/dvm/functions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from .BlockTimestamp import block_timestamp
 from .UpdateScCode import update_sc_code
 from .IsAddressValid import is_address_valid
 from .AddressRaw import address_raw
 from .AddressString import address_string
 from .SendDeroToAddress import send_dero_to_address
 from .SendAssetToAddress import send_asset_to_address
-from .DeroValue import dero_value
-from .AssetValue import asset_value
+from .DeroValue import derovalue
+from .AssetValue import assetvalue
 from .Atoi import atoi
 from .Itoa import itoa
 from .Sha256 import sha256
 from .Sha3256 import sha3256
 from .Keccak256 import keccak256
 from .Hex import _hex
 from .HexDecode import hex_decode
@@ -52,16 +52,16 @@
     block_timestamp,
     update_sc_code,
     is_address_valid,
     address_raw,
     address_string,
     send_dero_to_address,
     send_asset_to_address,
-    dero_value,
-    asset_value,
+    derovalue,
+    assetvalue,
     atoi,
     itoa,
     sha256,
     sha3256,
     keccak256,
     _hex,
     hex_decode,
```

### Comparing `deropy-0.2.0/deropy/dvm/iast/argument.py` & `deropy-0.2.1/deropy/dvm/iast/argument.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/assignement.py` & `deropy-0.2.1/deropy/dvm/iast/assignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/binaryOperator.py` & `deropy-0.2.1/deropy/dvm/iast/binaryOperator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/compare.py` & `deropy-0.2.1/deropy/dvm/iast/compare.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/functionCall.py` & `deropy-0.2.1/deropy/dvm/iast/functionCall.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/functionDef.py` & `deropy-0.2.1/deropy/dvm/iast/functionDef.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/iast_converter.py` & `deropy-0.2.1/deropy/dvm/iast/iast_converter.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/ifTest.py` & `deropy-0.2.1/deropy/dvm/iast/ifTest.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/operator.py` & `deropy-0.2.1/deropy/dvm/iast/operator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/returns.py` & `deropy-0.2.1/deropy/dvm/iast/returns.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/variableDeclarationAdnAssignement.py` & `deropy-0.2.1/deropy/dvm/iast/variableDeclarationAdnAssignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/iast/whileLoop.py` & `deropy-0.2.1/deropy/dvm/iast/whileLoop.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/parser.py` & `deropy-0.2.1/deropy/dvm/parser.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/tester.py` & `deropy-0.2.1/deropy/dvm/tester.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/dvm/utils.py` & `deropy-0.2.1/deropy/dvm/utils.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/python_templates/Nameservice.py` & `deropy-0.2.1/deropy/python_templates/Nameservice.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/python_templates/lottery.py` & `deropy-0.2.1/deropy/python_templates/lottery.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from deropy.dvm.functions import exists, store, load, signer, random, send_dero_to_address, address_raw, update_sc_code
+from deropy.dvm.functions import exists, store, derovalue, load, signer, random, send_dero_to_address, address_raw, update_sc_code
 from deropy.dvm.Smartcontract import SmartContract, logger, sc_logger
 
 
 @sc_logger(logger)
 class Lottery(SmartContract):
     def Initialize(self) -> int:
         if exists('owner') == 0:
@@ -14,14 +14,18 @@
             return 0
         return 1
 
     def Lottery(self, val: int) -> int:
         deposit_count: int = load("deposit_count") + 1
         if val == 0:
             return 0
+
+        if val > derovalue():
+            return 1
+
         store('depositor_address' + str(deposit_count), signer())
         store('deposit_total', load('deposit_total') + val)
         store('deposit_count', deposit_count)
 
         if load('lotteryeveryXdeposit') >= deposit_count:
             return 0
```

### Comparing `deropy-0.2.0/deropy/python_templates/minimum_sc.py` & `deropy-0.2.1/deropy/python_templates/minimum_sc.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/deropy/python_templates/token.py` & `deropy-0.2.1/deropy/python_templates/token.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from deropy.dvm.functions import exists, store, load, dero_value, asset_value, signer, address_raw, send_dero_to_address
+from deropy.dvm.functions import exists, store, load, derovalue, assetvalue, signer, address_raw, send_dero_to_address
 from deropy.dvm.functions import send_asset_to_address, scid
 from deropy.dvm.Smartcontract import SmartContract, logger, sc_logger
 
 
 @sc_logger(logger)
 class Token(SmartContract):
     def InitializePrivate(self) -> int:
@@ -10,19 +10,19 @@
             store("owner", signer())
             send_asset_to_address(signer(), 1000, scid())
             return 0
         else:
             return 1
 
     def IssueTokenX(self) -> int:
-        send_asset_to_address(signer(), dero_value(), scid())
+        send_asset_to_address(signer(), derovalue(), scid())
         return 0
 
     def ConvertTokenX(self) -> int:
-        send_dero_to_address(signer(), asset_value(scid()))
+        send_dero_to_address(signer(), assetvalue(scid()))
         return 0
 
     def TransferOwnership(self, new_owner: str) -> int:
         if load('owner') != signer():
             return 1
 
         store('tmpowner', address_raw(new_owner))
@@ -30,8 +30,7 @@
 
     def ClaimOwnership(self) -> int:
         if load('tmpowner') != signer():
             return 1
 
         store('owner', signer())
         return 0
-
```

### Comparing `deropy-0.2.0/deropy.egg-info/PKG-INFO` & `deropy-0.2.1/deropy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.2.0
+Version: 0.2.1
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.2.0/deropy.egg-info/SOURCES.txt` & `deropy-0.2.1/deropy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 deropy/__init__.py
+deropy/logger.py
 deropy/main.py
 deropy/utils.py
 deropy.egg-info/PKG-INFO
 deropy.egg-info/SOURCES.txt
 deropy.egg-info/dependency_links.txt
 deropy.egg-info/entry_points.txt
 deropy.egg-info/requires.txt
```

### Comparing `deropy-0.2.0/setup.py` & `deropy-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='deropy',
-    version=os.getenv('DEROPY_VERSION') or '0.2.0',
+    version=os.getenv('DEROPY_VERSION') or '0.2.1',
     url='https://github.com/dero-hyperbolic/deropy.git',
     author_email='leocances@gmail.com',
     description='A set of tool to help of DERO smart contract development',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `deropy-0.2.0/tests/test_compute_storage.py` & `deropy-0.2.1/tests/test_compute_storage.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/tests/test_map_functions.py` & `deropy-0.2.1/tests/test_map_functions.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.0/tests/test_storage_functions.py` & `deropy-0.2.1/tests/test_storage_functions.py`

 * *Files identical despite different names*


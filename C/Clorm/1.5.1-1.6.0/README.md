# Comparing `tmp/Clorm-1.5.1.tar.gz` & `tmp/clorm-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Clorm-1.5.1.tar", last modified: Mon Mar  4 01:08:36 2024, max compression
+gzip compressed data, was "clorm-1.6.0.tar", last modified: Thu May  9 10:56:53 2024, max compression
```

## Comparing `Clorm-1.5.1.tar` & `clorm-1.6.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 01:08:36.331249 Clorm-1.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 01:08:36.331249 Clorm-1.5.1/Clorm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-03-04 01:08:36.000000 Clorm-1.5.1/Clorm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-04 01:08:36.000000 Clorm-1.5.1/Clorm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 01:08:36.000000 Clorm-1.5.1/Clorm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 01:08:36.000000 Clorm-1.5.1/Clorm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-04 01:08:36.000000 Clorm-1.5.1/Clorm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-04 01:08:36.000000 Clorm-1.5.1/Clorm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-04 01:08:29.000000 Clorm-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-04 01:08:29.000000 Clorm-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-03-04 01:08:36.331249 Clorm-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15056 2024-03-04 01:08:29.000000 Clorm-1.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 01:08:36.323249 Clorm-1.5.1/clorm/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21431 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/_clingo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/clingo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 01:08:36.327249 Clorm-1.5.1/clorm/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/lib/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/lib/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/lib/timeslot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/monkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 01:08:36.327249 Clorm-1.5.1/clorm/orm/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48716 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/_queryimpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21862 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/atsyntax.py
--rw-r--r--   0 runner    (1001) docker     (127)   129229 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    38152 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/factbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    15379 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/factcontainers.py
--rw-r--r--   0 runner    (1001) docker     (127)   117414 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/lark_fact_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    17708 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/noclingo.py
--rw-r--r--   0 runner    (1001) docker     (127)   161207 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    25194 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/symbols_facts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/orm/types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 01:08:36.327249 Clorm-1.5.1/clorm/util/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/util/oset.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/util/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-03-04 01:08:29.000000 Clorm-1.5.1/clorm/util/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-04 01:08:29.000000 Clorm-1.5.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1624 2024-03-04 01:08:29.000000 Clorm-1.5.1/runtests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 01:08:36.331249 Clorm-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-04 01:08:36.000000 Clorm-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 01:08:36.331249 Clorm-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    44195 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_clingo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_forward_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_libboolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_libdate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_libtimeslot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_monkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_mypy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_mypy_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    19488 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_orm_atsyntax.py
--rw-r--r--   0 runner    (1001) docker     (127)   116353 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_orm_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    72515 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_orm_factbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    16217 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_orm_factcontainers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18148 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_orm_noclingo.py
--rw-r--r--   0 runner    (1001) docker     (127)   135479 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_orm_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    31608 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_orm_symbols_facts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_util_oset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_util_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-03-04 01:08:29.000000 Clorm-1.5.1/tests/test_util_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:56:53.829062 clorm-1.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:56:53.829062 clorm-1.6.0/Clorm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-05-09 10:56:53.000000 clorm-1.6.0/Clorm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-09 10:56:53.000000 clorm-1.6.0/Clorm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:56:53.000000 clorm-1.6.0/Clorm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:56:53.000000 clorm-1.6.0/Clorm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 10:56:53.000000 clorm-1.6.0/Clorm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 10:56:53.000000 clorm-1.6.0/Clorm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 10:56:46.000000 clorm-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 10:56:46.000000 clorm-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-05-09 10:56:53.829062 clorm-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15056 2024-05-09 10:56:46.000000 clorm-1.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:56:53.821062 clorm-1.6.0/clorm/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21431 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/_clingo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/clingo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:56:53.821062 clorm-1.6.0/clorm/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/lib/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/lib/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/lib/timeslot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/monkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:56:53.825062 clorm-1.6.0/clorm/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48716 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/_queryimpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21862 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/atsyntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131122 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38152 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/factbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15379 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/factcontainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117414 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/lark_fact_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17709 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/noclingo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   162213 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25194 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/symbols_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/orm/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:56:53.825062 clorm-1.6.0/clorm/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/util/oset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/util/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-09 10:56:46.000000 clorm-1.6.0/clorm/util/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-09 10:56:46.000000 clorm-1.6.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1624 2024-05-09 10:56:46.000000 clorm-1.6.0/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:56:53.829062 clorm-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 10:56:53.000000 clorm-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:56:53.829062 clorm-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    44195 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_clingo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_libboolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_libdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_libtimeslot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_monkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_mypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_mypy_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19489 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_orm_atsyntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119630 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_orm_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77252 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_orm_factbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16217 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_orm_factcontainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18148 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_orm_noclingo.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135531 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_orm_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31609 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_orm_symbols_facts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16181 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_util_oset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_util_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15738 2024-05-09 10:56:46.000000 clorm-1.6.0/tests/test_util_wrapper.py
```

### Comparing `Clorm-1.5.1/Clorm.egg-info/PKG-INFO` & `clorm-1.6.0/Clorm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Clorm
-Version: 1.5.1
+Version: 1.6.0
 Summary: Clingo ORM (CLORM) provides a ORM interface for interacting with the Clingo Answer Set Programming (ASP) solver
 Home-page: https://github.com/potassco/clorm
 Author: David Rajaratnam
 Author-email: daver@gemarex.com.au
 License: MIT
 License-File: LICENSE
 Requires-Dist: clingo
@@ -27,20 +27,20 @@
 the domain as a statically written ASP program, but then to generate problem
 instances and process the results dynamically. Clorm makes this integration
 cleaner, both in terms of code readability but also by providing a framework
 that makes it easier to refactor the python code as the ASP program evolves.
 
 The documentation is available online `here <https://clorm.readthedocs.io/>`_.
 
-Note: Clorm works with Python 3.7+ and Clingo 5.5+
+Note: Clorm works with Python 3.8+ and Clingo 5.6+
 
 Installation
 ------------
 
-Clorm requires Python 3.7+ and Clingo 5.5+. It can be installed using either the
+Clorm requires Python 3.8+ and Clingo 5.6+. It can be installed using either the
 `pip` or `conda` package managers.
 
 `pip` packages can be downloaded from PyPI:
 
 .. code-block:: bash
 
     $ pip install clorm
```

### Comparing `Clorm-1.5.1/Clorm.egg-info/SOURCES.txt` & `clorm-1.6.0/Clorm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/LICENSE` & `clorm-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/PKG-INFO` & `clorm-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Clorm
-Version: 1.5.1
+Version: 1.6.0
 Summary: Clingo ORM (CLORM) provides a ORM interface for interacting with the Clingo Answer Set Programming (ASP) solver
 Home-page: https://github.com/potassco/clorm
 Author: David Rajaratnam
 Author-email: daver@gemarex.com.au
 License: MIT
 License-File: LICENSE
 Requires-Dist: clingo
@@ -27,20 +27,20 @@
 the domain as a statically written ASP program, but then to generate problem
 instances and process the results dynamically. Clorm makes this integration
 cleaner, both in terms of code readability but also by providing a framework
 that makes it easier to refactor the python code as the ASP program evolves.
 
 The documentation is available online `here <https://clorm.readthedocs.io/>`_.
 
-Note: Clorm works with Python 3.7+ and Clingo 5.5+
+Note: Clorm works with Python 3.8+ and Clingo 5.6+
 
 Installation
 ------------
 
-Clorm requires Python 3.7+ and Clingo 5.5+. It can be installed using either the
+Clorm requires Python 3.8+ and Clingo 5.6+. It can be installed using either the
 `pip` or `conda` package managers.
 
 `pip` packages can be downloaded from PyPI:
 
 .. code-block:: bash
 
     $ pip install clorm
```

### Comparing `Clorm-1.5.1/README.rst` & `clorm-1.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 the domain as a statically written ASP program, but then to generate problem
 instances and process the results dynamically. Clorm makes this integration
 cleaner, both in terms of code readability but also by providing a framework
 that makes it easier to refactor the python code as the ASP program evolves.
 
 The documentation is available online `here <https://clorm.readthedocs.io/>`_.
 
-Note: Clorm works with Python 3.7+ and Clingo 5.5+
+Note: Clorm works with Python 3.8+ and Clingo 5.6+
 
 Installation
 ------------
 
-Clorm requires Python 3.7+ and Clingo 5.5+. It can be installed using either the
+Clorm requires Python 3.8+ and Clingo 5.6+. It can be installed using either the
 `pip` or `conda` package managers.
 
 `pip` packages can be downloaded from PyPI:
 
 .. code-block:: bash
 
     $ pip install clorm
```

### Comparing `Clorm-1.5.1/clorm/_clingo.py` & `clorm-1.6.0/clorm/_clingo.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
         )
 
 
 # ------------------------------------------------------------------------------
 # Wrap clingo.Model and override some functions
 # ------------------------------------------------------------------------------
 
+
 # class Model(OModel, metaclass=WrapperMetaClass):
 class ModelOverride(object):
     """Provides access to a model during a solve call.
 
     Objects mustn't be created manually. Instead they are returned by
     ``clorm.clingo.Control.solve`` callbacks.
 
@@ -232,14 +233,15 @@
     ClormSolveHandle = make_class_wrapper(OSolveHandle, SolveHandleOverride)
 
 
 # ------------------------------------------------------------------------------
 # Wrap clingo.Control and override some functions
 # ------------------------------------------------------------------------------
 
+
 # ------------------------------------------------------------------------------
 # Helper functions to expand the assumptions list as part of a solve() call. The
 # assumptions list is a list of argument-boolean pairs where the argument can be
 # be a clingo symbol, or clorm predicate instance, or a collection of clingo
 # symbols or clorm predicates. This needs to be expanded into a list of
 # symbol-bool pairs.
 # ------------------------------------------------------------------------------
@@ -251,15 +253,15 @@
     clingo_assump = []
 
     def _add_fact(fact: Union[Predicate, Symbol], bval: bool) -> None:
         raw = fact.raw if isinstance(fact, Predicate) else fact
         clingo_assump.append((raw, bool(bval)))
 
     try:
-        for (arg, bval) in assumptions:
+        for arg, bval in assumptions:
             if isinstance(arg, Predicate):
                 _add_fact(arg, bval)
             elif isinstance(arg, Iterable):
                 for f in arg:
                     _add_fact(cast(Union[Predicate, Symbol], f), bval)
             else:
                 _add_fact(arg, bval)
```

### Comparing `Clorm-1.5.1/clorm/clingo.py` & `clorm-1.6.0/clorm/clingo.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/json.py` & `clorm-1.6.0/clorm/json.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/lib/boolean.py` & `clorm-1.6.0/clorm/lib/boolean.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/lib/date.py` & `clorm-1.6.0/clorm/lib/date.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/lib/timeslot.py` & `clorm-1.6.0/clorm/lib/timeslot.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/monkey.py` & `clorm-1.6.0/clorm/monkey.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/orm/__init__.py` & `clorm-1.6.0/clorm/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/orm/_queryimpl.py` & `clorm-1.6.0/clorm/orm/_queryimpl.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/orm/_typing.py` & `clorm-1.6.0/clorm/orm/_typing.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/orm/atsyntax.py` & `clorm-1.6.0/clorm/orm/atsyntax.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/orm/core.py` & `clorm-1.6.0/clorm/orm/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,25 @@
-# -----------------------------------------------------------------------------
-# Implementation of the core part of the Clorm ORM. In particular this provides
-# the base classes and metaclasses for the definition of fields, predicates,
-# predicate paths, and the specification of query conditions. Note: query
-# condition specification is provided here because the predicate path comparison
-# operators are overloads to return these objects. However, the rest of the
-# query API is specified with the FactBase and select querying mechanisms
-# (see factbase.py).
-# ------------------------------------------------------------------------------
+# -------------------------------------------------------------------------------------------
+# Implementation of the core part of the Clorm ORM. In particular this provides the base
+# classes and metaclasses for the definition of fields, predicates, predicate paths, and the
+# specification of query conditions. Note: query condition specification is provided here
+# because the predicate path comparison operators are overloads to return these
+# objects. However, the rest of the query API is specified with the FactBase and select
+# querying mechanisms (see factbase.py).
+# -------------------------------------------------------------------------------------------
+
+# -------------------------------------------------------------------------------------------
+# NOTE: 20242028 the semantics for the comparison operators has changed.  Instead of using the
+# python field representation we use the underlying clingo symbol object. The symbol object is
+# well defined for any comparison between symbols, whereas tuples are only well defined if the
+# types of the individual parameters are compatible. So this change leads to more natural
+# behaviour for the queries. Note: users should avoid defining unintuitive fields (for example
+# a swap field that changes the sign of an int) to avoid unintuitive Python behaviour.
+# -------------------------------------------------------------------------------------------
+
 
 from __future__ import annotations
 
 import abc
 import collections
 import collections.abc as cabc
 import datetime
@@ -280,14 +289,15 @@
 # clause. A QCondition is either a boolean condition or a comparison condition
 # depending on the operator. A comparison condition involves comparing a
 # component of a fact (specified with a PredicatePath) against some criteria. A
 # boolean condition specifies complex boolean relations consisting of comparion
 # conditions and other boolean conditions.
 # ------------------------------------------------------------------------------
 
+
 # comparator functions that always return true (or false). This is useful for
 # the cross product join operator that always returns true
 def trueall(x, y):
     return True
 
 
 def falseall(x, y):
@@ -717,14 +727,22 @@
         # Is this a leaf path
         # --------------------------------------------------------------------------
         @property
         def is_leaf(self):
             return not hasattr(self, "_predicate_class")
 
         # --------------------------------------------------------------------------
+        # If the leaf of the path is a Predicate class then return it else None
+        # --------------------------------------------------------------------------
+        @property
+        def complex(self):
+            fld = self._parent._get_field()
+            return None if fld is None else fld.complex
+
+        # --------------------------------------------------------------------------
         # attrgetter
         # --------------------------------------------------------------------------
         @property
         def attrgetter(self):
             return self._parent._attrgetter
 
         # --------------------------------------------------------------------------
@@ -1184,14 +1202,15 @@
 
 
 # ------------------------------------------------------------------------------
 # BaseField class captures the definition of a logical term ("which we will call
 # a field") between python and clingo.
 # ------------------------------------------------------------------------------
 
+
 # Create the pytocl and cltopy class member functions. If their inherit directly
 # from BaseField then just return the result of the function. If they inherit
 # from a sub-class of BaseField then call the parents conversion function first.
 def _make_pytocl(parent, fn):
     if parent == BaseField:
         return fn
     pfn = parent.pytocl
@@ -1269,14 +1288,15 @@
 
 
 # ------------------------------------------------------------------------------
 # Field definitions. All fields have the functions: pytocl, cltopy,
 # and unifies, and the properties: default and has_default
 # ------------------------------------------------------------------------------
 
+
 # Mixin class to be able to use both MetaClasses
 class _AbstractBaseFieldMeta(abc.ABCMeta, _BaseFieldMeta):
     pass
 
 
 class BaseField(object, metaclass=_AbstractBaseFieldMeta):
     """Define a mapping from ASP logical terms to Python objects.
@@ -1328,58 +1348,86 @@
        Here the ``DateField.cltopy`` is called at the end of the chain of
        translations, so it expects a Python string object as input and outputs a
        date object. ``DateField.pytocl`` does the opposite and inputs a date
        object and is expected to output a Python string object.
 
     Args:
 
-      default: A default value (or function) to be used when instantiating a
-       ``Predicate`` object. If a Python ``callable`` object is
-       specified (i.e., a function or functor) then it will be called (with no
-       arguments) when the predicate/complex-term object is instantiated.
+      default: A default value to be used when instantiating a ``Predicate`` object and no
+        value has been specified.
+
+      default_factory: A unary function (ie. a function with no arguments) for generating a
+        value when none has been specified.
 
       index (bool): Determine if this field should be indexed by default in a
-        ``FactBase```. Defaults to ``False``.
+        ``FactBase```. Defaults to ``False``. WARNING: this parameter will be deprecated in
+        a future version of Clorm. Indexing should be explicitly set in the FactBase object.
 
     """
 
-    def __init__(self, default: Any = MISSING, index: Any = MISSING) -> None:
+    def __init__(
+        self,
+        *,
+        default: Any = MISSING,
+        default_factory: Callable[[], Any] = MISSING,
+        index: Any = MISSING,
+    ) -> None:
+        """Initialize a field instance.
+
+        Args:
+
+          default: A default value to be used when instantiating a ``Predicate`` object and no
+            value has been specified.
+
+          default_factory: A unary function (ie. a function with no arguments) for generating a
+            value when none has been specified.
+
+          index (bool): Determine if this field should be indexed by default in a
+            ``FactBase```. Defaults to ``False``. WARNING: this parameter will be deprecated in
+            a future version of Clorm. Indexing should be explicitly set in the FactBase object.
+
+        """
         self._index = index if index is not MISSING else False
+        if default is not MISSING and default_factory is not MISSING:
+            raise ValueError("can not specify both default and default_factory")
 
-        if default is MISSING:
-            self._default = (False, None)
+        self._default = MISSING
+        self._default_factory = MISSING
+        if default is MISSING and default_factory is MISSING:
             return
 
-        self._default = (True, default)
         cmplx = self.complex
 
-        # Check and convert the default to a valid value. Note: if the default
-        # is a callable then we can't do this check because it could break a
-        # counter type procedure.
-        if callable(default) or (cmplx and isinstance(default, cmplx)):
-            return
+        def _process_basic_value(v):
+            return v
 
-        try:
-            if cmplx:
+        def _process_cmplx_value(v):
+            if isinstance(v, cmplx):
+                return v
+            if isinstance(v, tuple) or (isinstance(v, Predicate) and v.meta.is_tuple):
+                return cmplx(*v)
+            raise TypeError(f"Value {v} ({type(v)}) cannot be converted to type {cmplx}")
 
-                def _instance_from_tuple(v):
-                    if isinstance(v, tuple) or (isinstance(v, Predicate) and v.meta.is_tuple):
-                        return cmplx(*v)
-                    raise TypeError(f"Value {v} ({type(v)}) is not a tuple")
-
-                if cmplx.meta.is_tuple:
-                    self._default = (True, _instance_from_tuple(default))
-                else:
-                    raise ValueError("Bad default")
-            else:
-                self.pytocl(default)
-        except (TypeError, ValueError):
-            raise TypeError(
-                'Invalid default value "{}" for {}'.format(default, type(self).__name__)
-            )
+        _process_value = _process_basic_value if cmplx is None else _process_cmplx_value
+
+        # If we're using a default value then set the value (after some preprocessing).
+        if default is not MISSING:
+            try:
+                self._default = _process_value(default)
+                self.pytocl(self._default)
+            except (TypeError, ValueError):
+                raise TypeError(
+                    'Invalid default value "{}" for {}'.format(default, type(self).__name__)
+                )
+        else:
+
+            def _process_default_factory():
+                return _process_value(default_factory())
+
+            self._default_factory = _process_default_factory
 
     @staticmethod
     @abc.abstractmethod
     def cltopy(v):
         """Called when translating data from Clingo to Python"""
         raise NotImplementedError("BaseField.cltopy() must be overriden")
 
@@ -1393,38 +1441,43 @@
     @_classproperty
     @classmethod
     def complex(cls) -> Optional["Predicate"]:
         return None
 
     @property
     def has_default(self):
-        """Returns whether a default value has been set"""
-        return self._default[0]
+        """Returns whether there is a default value or default factory."""
+        return self._default is not MISSING or self._default_factory is not MISSING
 
     @property
     def has_default_factory(self):
-        """Returns whether a default value has been set"""
-        return self._default[0] and callable(self._default[1])
+        """Returns whether there is a default factory"""
+        return self._default_factory is not MISSING
+
+    @property
+    def default_factory(self):
+        """Return the default factory function."""
+        return self._default_factory
 
     @property
     def default(self):
         """Returns the default value for the field (or ``None`` if no default was set).
 
         Note: 1) if a function was specified as the default then testing
         ``default`` will call this function and return the value, 2) if your
         BaseField sub-class allows a default value of ``None`` then you need to
         check the ``has_default`` property to distinguish between no default
         value and a ``None`` default value.
 
         """
-        if not self._default[0]:
-            return None
-        if callable(self._default[1]):
-            return self._default[1]()
-        return self._default[1]
+        if self._default is not MISSING:
+            return self._default
+        if self._default_factory is not MISSING:
+            return self._default_factory()
+        return None
 
     @property
     def index(self):
         """Returns whether this field should be indexed by default in a `FactBase`"""
         return self._index
 
     def __str__(self):
@@ -1484,34 +1537,38 @@
         raise ValueError("can not specify both default and default_factory")
     if isinstance(basefield, tuple):
         try:
             module = sys._getframe(1).f_globals.get("__name__", "__main__")
         except (AttributeError, ValueError):
             module = None
         if default is not MISSING:
-            return _create_complex_term(basefield, default, module)
-        elif default_factory is not MISSING:
-            return _create_complex_term(basefield, default_factory, module)
+            return _create_complex_term(basefield, default=default, module=module)
+        if default_factory is not MISSING:
+            return _create_complex_term(basefield, default_factory=default_factory, module=module)
         return basefield
 
     if issubclass(basefield, BaseField):
         if default is not MISSING:
-            return basefield(default)
-        elif default_factory is not MISSING:
-            return basefield(default_factory)
-        return basefield
+            return basefield(default=default)
+        if default_factory is not MISSING:
+            return basefield(default_factory=default_factory)
+        complex = basefield.complex
+        if complex is not None:
+            fields = (dn.defn for dn in complex.meta)
+            default, default_factory = _make_implicit_defaults_for_complex_field(fields)
+        return basefield(default=default, default_factory=default_factory)
 
-    raise TypeError(f"{basefield} can just be of Type '{BaseField}' or '{Sequence}'")
+    raise TypeError(f"{basefield} can only be of type '{BaseField}' or '{Sequence}'")
 
 
-# ------------------------------------------------------------------------------
-# RawField is a sub-class of BaseField for storing Symbol or NoSymbol
-# objects. The behaviour of Raw with respect to using clingo.Symbol or
-# noclingo.NoSymbol is modified by the symbol mode (get_symbol_mode())
-# ------------------------------------------------------------------------------
+# ------------------------------------------------------------------------------------------
+# RawField is a sub-class of BaseField for storing Symbol objects. The behaviour of Raw with
+# respect to using clingo.Symbol or noclingo.Symbol is modified by the symbol mode
+# (get_symbol_mode())
+# ------------------------------------------------------------------------------------------
 
 
 class Raw(object):
     """A wrapper around a raw ``Symbol`` object.
 
     The ``Raw`` object is for use with a ``RawField`` field definition. It
     provides a thin wrapper around a ``clingo.Symbol`` (or ``noclingo.Symbol``)
@@ -1793,14 +1850,15 @@
 # explicit set of values.
 # ------------------------------------------------------------------------------
 # ------------------------------------------------------------------------------
 # Helper function to define a sub-class of a BaseField (or sub-class) that
 # restricts the allowable values.
 # ------------------------------------------------------------------------------
 
+
 # Support for refine_field
 def _refine_field_functor(subclass_name, field_class, valfunc):
     def _test_value(v):
         if not valfunc(v):
             raise TypeError(
                 ('Invalid value "{}" for {} (restriction of ' "{})").format(
                     v, subclass_name, field_class.__name__
@@ -2436,39 +2494,58 @@
     # Expecting a tuple and treat it as a recursive definition
     if not isinstance(defn, tuple):
         raise TypeError(errmsg.format(defn))
 
     return _create_complex_term(defn, module=module)
 
 
-def _create_complex_term(defn: Any, default_value: Any = MISSING, module: str = "") -> BaseField:
-    # NOTE: I was using a dict rather than OrderedDict which just happened to
-    # work. Apparently, in Python 3.6 this was an implmentation detail and
-    # Python 3.7 it is a language specification (see:
-    # https://stackoverflow.com/questions/1867861/how-to-keep-keys-values-in-same-order-as-declared/39537308#39537308).
-    # However, since Clorm is meant to be Python 3.5 compatible change this to
-    # use an OrderedDict.
-    # proto = { "arg{}".format(i+1) : get_field_definition(d) for i,d in enumerate(defn) }
-    proto: Dict[str, Any] = collections.OrderedDict(
-        [(f"arg{i+1}", get_field_definition(d, module)) for i, d in enumerate(defn)]
-    )
+def _make_implicit_defaults_for_complex_field(
+    fields: Tuple[BaseField],
+) -> Tuple[Any, Union[Callable[[], Any], None]]:
+    """Tries to create a default value or a default_factory.
+
+    Returns a pair (default, default_factory). If both values are MISSING then there is no way to
+    generate a default.
+
+    """
+
+    def _default_factory():
+        return tuple([field.default for field in fields])
+
+    make_default_factory = False
+    for field in fields:
+        if not field.has_default and not field.has_default_factory:
+            return (MISSING, MISSING)
+        if field.has_default_factory:
+            make_default_factory = True
+    if make_default_factory:
+        return (MISSING, _default_factory)
+    return (_default_factory(), MISSING)
+
+
+def _create_complex_term(
+    defn: Any,
+    *,
+    default: Any = MISSING,
+    default_factory: Callable[[], Any] = MISSING,
+    module: str = "",
+) -> BaseField:
+    # NOTE: relies on a dict preserving insertion order - this is true from Python 3.7+. Python
+    # 3.7 is already end-of-life so there is no longer a reason to use OrderedDict.
+    proto = {f"arg{idx+1}": get_field_definition(dn) for idx, dn in enumerate(defn)}
     class_name = (
         f'ClormAnonTuple({",".join(f"{arg[0]}={repr(arg[1])}" for arg in proto.items())})'
     )
 
-    if default_value is not MISSING:
-        default = default_value
-        set_default = True
-    else:
-        default = tuple([field.default for field in proto.values() if field.has_default])
-        set_default = len(default) == len(
-            proto
-        )  # calling type modifies proto so compare it beforehand
-        if not set_default and default:
-            raise ValueError((f"Default {default_value} must have the same length as {defn}"))
+    # if no default or default_factory is specified then see if we try to construct one from
+    # the sub-fields.
+    if default is MISSING and default_factory is MISSING:
+        default, default_factory = _make_implicit_defaults_for_complex_field(
+            tuple(proto.values())
+        )
     proto["Meta"] = type("Meta", (object,), {"is_tuple": True, "_anon": True})
 
     # For pickling to work, the __module__ variable needs to be set to the frame
     # where the named tuple is created.
     if module is not None:
         proto["__module__"] = module
     ct: Type[Predicate] = type(class_name, (Predicate,), proto)
@@ -2484,15 +2561,15 @@
                         ct = f_globals[class_name]
                     else:
                         f_globals[class_name] = ct
                     break
                 depth += 1
         except ValueError:
             pass
-    return ct.Field(default) if set_default else ct.Field()
+    return ct.Field(default=default, default_factory=default_factory)
 
 
 # ------------------------------------------------------------------------------
 # Return the list of field_paths associated with a predicate (ignoring the base
 # predicate path itself).
 # ------------------------------------------------------------------------------
 def _get_paths(predicate: Type["Predicate"]) -> List[PredicatePath]:
@@ -2546,19 +2623,19 @@
 # query between a predicate and itself. Eg. something like F.a == F.alias().a So
 # we need a way to distinguish between paths that point to the same underlying
 # predicate but use a different identifier.
 # -----------------------------------------------------------------------------
 
 PathIdentity = collections.namedtuple("PathIdentity", "predicate name")
 
+
 # --------------------------------------------------------------------------
 # One PredicateDefn object for each Predicate sub-class
 # --------------------------------------------------------------------------
 class PredicateDefn(object):
-
     """Encapsulates some meta-data for a Predicate definition.
 
     Each Predicate class will have a corresponding PredicateDefn object that specifies some
     introspective properties of the predicate.
 
     """
 
@@ -2701,21 +2778,24 @@
 
 
 def _generate_dynamic_predicate_functions(class_name: str, namespace: Dict) -> None:
     pdefn = namespace["_meta"]
 
     gdict = {
         "Predicate": Predicate,
+        "Symbol": Symbol,
         "Function": Function,
         "MISSING": MISSING,
         "AnySymbol": AnySymbol,
         "Type": Type,
+        "Any": Any,
         "Optional": Optional,
         "Sequence": Sequence,
         "_P": _P,
+        "PREDICATE_IS_TUPLE": pdefn.is_tuple,
     }
 
     for f in pdefn:
         gdict[f"{f.name}_field"] = f.defn
         gdict[f"{f.name}_pytocl"] = f.defn.pytocl
         gdict[f"{f.name}_cltopy"] = f.defn.cltopy
 
@@ -2782,35 +2862,41 @@
         "args_raw": args_raw,
         "sign_check_unify": sign_check_unify,
         "args_cltopy": args_cltopy,
     }
 
     template = PREDICATE_TEMPLATE.format(pdefn=pdefn)
     predicate_functions = expand_template(template, **expansions)
-    # print(f"INIT:\n\n{predicate_functions}\n\n")
+    #    print(f"INIT {class_name}:\n\n{predicate_functions}\n\n")
 
     ldict: Dict[str, Any] = {}
     exec(predicate_functions, gdict, ldict)
 
-    init_doc_args = f"{args_signature}*, sign=True, raw=None"
-    predicate_init = ldict["__init__"]
-    predicate_init.__name__ = "__init__"
-    predicate_init.__doc__ = f"{class_name}({init_doc_args})"
-    predicate_unify = ldict["_unify"]
-    predicate_unify.__name__ = "_unify"
-    predicate_unify.__doc__ = PREDICATE_UNIFY_DOCSTRING
-
-    namespace["__init__"] = predicate_init
-    namespace["_unify"] = predicate_unify
+    def _set_fn(fname: str, docstring: str):
+        tmp = ldict[fname]
+        tmp.__name__ = fname
+        tmp.__doc = docstring
+        namespace[fname] = tmp
+
+    # Assign the __init__, _unify, __hash__, and appropriate comparison functions
+    _set_fn("__init__", f"{class_name}({args_signature}*, sign=True, raw=None)")
+    _set_fn("_unify", PREDICATE_UNIFY_DOCSTRING)
+    _set_fn("__hash__", "Hash operator")
+    _set_fn("__eq__", "Equality operator")
+    _set_fn("__lt__", "Less than operator")
+    _set_fn("__le__", "Less than or equal operator")
+    _set_fn("__gt__", "Greater than operator")
+    _set_fn("__ge__", "Greater than operator")
 
 
 # ------------------------------------------------------------------------------
 # Metaclass constructor support functions to create the fields
 # ------------------------------------------------------------------------------
 
+
 # Generate a default predicate name from the Predicate class name.
 def _predicatedefn_default_predicate_name(class_name):
 
     # If first letter is lower-case then do nothing
     if class_name[0].islower():
         return class_name
 
@@ -3009,17 +3095,16 @@
         if is_tuple and not sign:
             raise ValueError(
                 ("Tuples cannot be negated so specifying " "'sign' is None or False is invalid")
             )
 
     reserved = set(["meta", "raw", "clone", "sign", "Field"])
 
-    # Generate the fields - NOTE: this relies on dct being an OrderedDict()
-    # which is true from Python 3.5+ (see PEP520
-    # https://www.python.org/dev/peps/pep-0520/)
+    # Generate the fields - NOTE: this relies on dict being an ordered which is true from
+    # Python 3.5+ (see PEP520 https://www.python.org/dev/peps/pep-0520/)
 
     # Predicates (or complexterms) that are defined within the current Predicate context may be
     # necessary to help resolve the postponed annotations.
     inner_predicates: Dict[str, Type[Predicate]] = {}
 
     fields_from_dct = {}
     for fname, fdefn in namespace.items():
@@ -3156,14 +3241,16 @@
     )
     return field
 
 
 # ------------------------------------------------------------------------------
 # A Metaclass for the Predicate base class
 # ------------------------------------------------------------------------------
+
+
 @__dataclass_transform__(field_descriptors=(field,))
 class _PredicateMeta(type):
     if TYPE_CHECKING:
         meta: PredicateDefn
 
     # --------------------------------------------------------------------------
     # Allocate the new metaclass
@@ -3320,15 +3407,15 @@
     # --------------------------------------------------------------------------
 
     # Get the Symbol object using the default symbol system
     @property
     def symbol(self):
         """Returns the Symbol object corresponding to the fact.
 
-        The type of the object maybe either a ``clingo.Symbol`` or ``noclingo.NoSymbol``.
+        The type of the object maybe either a ``clingo.Symbol`` or ``noclingo.Symbol``.
         """
         return self._raw
 
     # Get the underlying clingo.Symbol object
     @property
     def raw(self) -> Symbol:
         """Returns the underlying ``clingo.Symbol`` object"""
@@ -3411,80 +3498,35 @@
         return self.clone(sign=not self.sign)
 
     # --------------------------------------------------------------------------
     # Overloaded operators
     # --------------------------------------------------------------------------
     def __eq__(self, other):
         """Overloaded boolean operator."""
-        if isinstance(other, self.__class__):
-            return self._field_values == other._field_values and self._sign == other._sign
-        if self.meta.is_tuple:
-            return self._field_values == other
-        elif isinstance(other, Predicate):
-            return False
-        return NotImplemented
+        raise NotImplementedError("Predicate.__eq__() must be overriden")
 
     def __lt__(self, other):
         """Overloaded boolean operator."""
+        raise NotImplementedError("Predicate.__lt__() must be overriden")
 
-        # If it is the same predicate class then compare the sign and fields
-        if isinstance(other, self.__class__):
-
-            # Negative literals are less than positive literals
-            if self.sign != other.sign:
-                return self.sign < other.sign
-
-            return self._field_values < other._field_values
-
-        # If different predicates then compare the raw value
-        elif isinstance(other, Predicate):
-            return self.raw < other.raw
-
-        # Else an error
-        return NotImplemented
+    def __le__(self, other):
+        """Overloaded boolean operator."""
+        raise NotImplementedError("Predicate.__le__() must be overriden")
 
     def __ge__(self, other):
         """Overloaded boolean operator."""
-        result = self.__lt__(other)
-        if result is NotImplemented:
-            return NotImplemented
-        return not result
+        raise NotImplementedError("Predicate.__ge__() must be overriden")
 
     def __gt__(self, other):
         """Overloaded boolean operator."""
-
-        # If it is the same predicate class then compare the sign and fields
-        if isinstance(other, self.__class__):
-            # Positive literals are greater than negative literals
-            if self.sign != other.sign:
-                return self.sign > other.sign
-
-            return self._field_values > other._field_values
-
-        # If different predicates then compare the raw value
-        if not isinstance(other, Predicate):
-            return self.raw > other.raw
-
-        # Else an error
-        return NotImplemented
-
-    def __le__(self, other):
-        """Overloaded boolean operator."""
-        result = self.__gt__(other)
-        if result is NotImplemented:
-            return NotImplemented
-        return not result
+        raise NotImplementedError("Predicate.__gt__() must be overriden")
 
     def __hash__(self):
-        if self._hash is None:
-            if self.meta.is_tuple:
-                self._hash = hash(self._field_values)
-            else:
-                self._hash = hash((self.meta.name, self._field_values))
-        return self._hash
+        """Overload the hash function."""
+        raise NotImplementedError("Predicate.__hash__() must be overriden")
 
     def __str__(self):
         """Returns the Predicate as the string representation of an ASP fact."""
         return str(self.raw)
 
     def __repr__(self):
         return self.__str__()
@@ -3543,29 +3585,28 @@
     Optional keyword-only arguments:
 
        name: name for new class (default: anonymously generated).
 
     """
     subclass_name = name if name else "AnonSimplePredicate"
 
-    # Use an OrderedDict to ensure the correct order of the field arguments
-    proto: Dict[str, Any] = collections.OrderedDict(
-        [("arg{}".format(i + 1), RawField()) for i in range(0, arity)]
-    )
+    # Note: dict is preserves the ordering
+    proto: Dict[str, Any] = {f"arg{i+1}": RawField() for i in range(0, arity)}
     proto["Meta"] = type(
         "Meta", (object,), {"name": predicate_name, "is_tuple": False, "_anon": True}
     )
     newclass = type(subclass_name, (Predicate,), proto)
     return newclass
 
 
 # ------------------------------------------------------------------------------
 # Internal supporting functions
 # ------------------------------------------------------------------------------
 
+
 # ------------------------------------------------------------------------------
 # Helper function to check if all the paths in a collection are root paths and
 # return path objects.
 # ------------------------------------------------------------------------------
 def validate_root_paths(paths):
     def checkroot(p):
         p = path(p)
```

### Comparing `Clorm-1.5.1/clorm/orm/factbase.py` & `clorm-1.6.0/clorm/orm/factbase.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/orm/factcontainers.py` & `clorm-1.6.0/clorm/orm/factcontainers.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/orm/lark_fact_parser.py` & `clorm-1.6.0/clorm/orm/lark_fact_parser.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/orm/noclingo.py` & `clorm-1.6.0/clorm/orm/noclingo.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 function `set_symbol_mode()` and `get_symbol_mode()`. If the CLORM_NOCLINGO
 environment variable is not set, or is set to one of "0", "False", "No",
 "Disable" (case-insensitive), then the NOCLINGO mechanism is disabled and it is
 not possible to switch between modes. In this case calling `set_symbol_mode()`
 will raise an exception.
 
 """
+
 # --------------------------------------------------------------------------------
 # --------------------------------------------------------------------------------
 
 from __future__ import annotations
 
 import enum
 import os
```

### Comparing `Clorm-1.5.1/clorm/orm/query.py` & `clorm-1.6.0/clorm/orm/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,20 +53,20 @@
 # ------------------------------------------------------------------------------
 
 
 # ------------------------------------------------------------------------------
 # Defining and manipulating conditional elements
 # ------------------------------------------------------------------------------
 
+
 # ------------------------------------------------------------------------------
 # Placeholder allows for variable substituion of a query. Placeholder is
 # an abstract class that exposes no API other than its existence.
 # ------------------------------------------------------------------------------
 class Placeholder(abc.ABC):
-
     r"""An abstract class for defining parameterised queries.
 
     Currently, Clorm supports 4 placeholders: ph1\_, ph2\_, ph3\_, ph4\_. These
     correspond to the positional arguments of the query execute function call.
 
     """
 
@@ -511,14 +511,37 @@
 # comparator only takes into account predicate paths. The main thing is that
 # equality works properly. While this is a bit of a hack I think it is ok
 # provided StandardComparator is used only in this specific way within clorm and
 # is not exposed outside clorm.
 # ------------------------------------------------------------------------------
 
 
+# Helper function to try to convert Python tuples into a matching clorm anon tuple.  With this
+# we can pass a Python tuple to a query and not have to overload the Predicate comparison
+# operator and hash function to match the tuple.
+def _try_to_convert_tuple_argument_to_clorm_tuple(op, args):
+    def _try_to_convert(tup, possiblepath):
+        if not isinstance(possiblepath, PredicatePath):
+            return tup
+        complex = possiblepath.meta.complex
+        if complex is None or not complex.meta.is_tuple:
+            return tup
+        return complex(*tup)
+
+    if op not in {operator.eq, operator.ne, operator.lt, operator.le, operator.gt, operator.ge}:
+        return args
+    if len(args) != 2:
+        return args
+    if isinstance(args[0], tuple):
+        return (_try_to_convert(args[0], args[1]), args[1])
+    if isinstance(args[1], tuple):
+        return (args[0], _try_to_convert(args[1], args[0]))
+    return args
+
+
 class StandardComparator(Comparator):
     class Preference(enum.IntEnum):
         LOW = 0
         MEDIUM = 1
         HIGH = 2
 
     OpSpec = collections.namedtuple("OpSpec", "pref join where negop swapop keyable form")
@@ -621,15 +644,15 @@
             raise TypeError(
                 (
                     "Internal bug: cannot create StandardComparator() with "
                     "non-comparison operator '{}' "
                 ).format(operator)
             )
         self._operator = operator
-        self._args = tuple(args)
+        self._args = tuple(_try_to_convert_tuple_argument_to_clorm_tuple(operator, args))
         self._hashableargs = tuple(
             [hashable_path(a) if isinstance(a, PredicatePath) else a for a in self._args]
         )
         self._paths = tuple(filter(lambda x: isinstance(x, PredicatePath), self._args))
 
         tmppaths = set([])
         tmproots = set([])
@@ -785,15 +808,15 @@
         spec = StandardComparator.operators[self._operator]
         if not spec.swapop:
             raise ValueError(
                 ("Internal bug: comparator '{}' doesn't support " "the swap operation").format(
                     self._operator
                 )
             )
-        return StandardComparator(spec.swapop, reversed(self._args))
+        return StandardComparator(spec.swapop, tuple(reversed(self._args)))
 
     def keyable(self, indexes):
         spec = StandardComparator.operators[self._operator]
         return spec.keyable(self, indexes)
 
     @property
     def paths(self):
@@ -2207,14 +2230,15 @@
 
 
 # ------------------------------------------------------------------------------
 # JoinQueryPlan support functions. The JQP is a part of the query plan that
 # describes the plan to execute a single link in a join.
 # ------------------------------------------------------------------------------
 
+
 # Check that the formula only refers to paths with the allowable roots
 def _check_roots(allowable_roots, formula):
     if not formula:
         return True
     allowable_hroots = set([hashable_path(rp) for rp in allowable_roots])
     hroots = set([hashable_path(rp) for rp in formula.roots])
     return hroots.issubset(allowable_hroots)
@@ -3041,14 +3065,15 @@
 
 
 # ------------------------------------------------------------------------------
 # Implementing Queries - taking a QuerySpec, QueryPlan, and a FactMap and
 # generating an actual query.
 # ------------------------------------------------------------------------------
 
+
 # ------------------------------------------------------------------------------
 # Creates a mechanism for sorting using the order_by statements within queries.
 #
 # Works by creating a list of pairs consisting of a keyfunction and reverse
 # flag, corresponding to the orderbyblocks in reverse order. A list can then by
 # sorted by successively applying each sort function. Stable sort guarantees
 # that the the result is a multi-criteria sort.
```

### Comparing `Clorm-1.5.1/clorm/orm/symbols_facts.py` & `clorm-1.6.0/clorm/orm/symbols_facts.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/orm/types.py` & `clorm-1.6.0/clorm/orm/types.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/util/oset.py` & `clorm-1.6.0/clorm/util/oset.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/util/tools.py` & `clorm-1.6.0/clorm/util/tools.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/clorm/util/wrapper.py` & `clorm-1.6.0/clorm/util/wrapper.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/runtests.py` & `clorm-1.6.0/runtests.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/setup.py` & `clorm-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     if version_match:
         return version_match.group(1)
     raise RuntimeError("Unable to find version string.")
 
 
 setup(
     name="Clorm",
-    version = '1.5.1',
+    version = '1.6.0',
     author="David Rajaratnam",
     author_email="daver@gemarex.com.au",
     description="Clingo ORM (CLORM) provides a ORM interface for interacting with the Clingo Answer Set Programming (ASP) solver",
     license="MIT",
     url="https://github.com/potassco/clorm",
     packages=["clorm", "clorm.orm", "clorm.util", "clorm.lib"],
     package_data={"clorm": ["py.typed"]},
```

### Comparing `Clorm-1.5.1/tests/test_clingo.py` & `clorm-1.6.0/tests/test_clingo.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_forward_ref.py` & `clorm-1.6.0/tests/test_forward_ref.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_json.py` & `clorm-1.6.0/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_libboolean.py` & `clorm-1.6.0/tests/test_libboolean.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_libdate.py` & `clorm-1.6.0/tests/test_libdate.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_libtimeslot.py` & `clorm-1.6.0/tests/test_libtimeslot.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_monkey.py` & `clorm-1.6.0/tests/test_monkey.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_mypy.py` & `clorm-1.6.0/tests/test_mypy.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_mypy_query.py` & `clorm-1.6.0/tests/test_mypy_query.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_orm_atsyntax.py` & `clorm-1.6.0/tests/test_orm_atsyntax.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,14 +422,15 @@
         pass
 
     def test_register(self):
 
         SF = StringField
         IF = IntegerField
         CF = ConstantField
+
         # Functions to add to the context
         def add(a: IF, b: IF) -> IF:
             return a + b
 
         def mirror(val: CF) -> CF:
             return val
```

### Comparing `Clorm-1.5.1/tests/test_orm_core.py` & `clorm-1.6.0/tests/test_orm_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 #
 # Note: I'm trying to clearly separate tests of the official Clorm API from
 # tests of the internal implementation. Tests for the API have names
 # "test_api_XXX" while non-API tests are named "test_nonapi_XXX". This is still
 # to be completed.
 # ------------------------------------------------------------------------------
 
+# -------------------------------------------------------------------------------------------
+# NOTE: 20242028 See orm/core.py for changes to the semantics of comparison operators for
+# Predicate objects.
+# -------------------------------------------------------------------------------------------
+
+
 import collections.abc as cabc
 import datetime
 import enum
 import inspect
 import operator
 import pickle
 import sys
@@ -67,15 +73,15 @@
     dealiased_path,
     field,
     get_field_definition,
     notcontains,
     trueall,
 )
 
-from .support import check_errmsg, check_errmsg_contains
+from .support import check_errmsg, check_errmsg_contains, to_tuple
 
 # Error messages for CPython and PyPy vary
 PYPY = sys.implementation.name == "pypy"
 
 
 # ------------------------------------------------------------------------------
 # ------------------------------------------------------------------------------
@@ -265,29 +271,31 @@
 
     # --------------------------------------------------------------------------
     # Test that the field function works as expected
     # --------------------------------------------------------------------------
     def test_api_field_function(self):
         with self.subTest("with single BaseField"):
             f = field(IntegerField)
-            self.assertEqual(f, IntegerField)
+            self.assertTrue(isinstance(f, IntegerField))
 
             f = field(IntegerField, default=4)
             self.assertEqual(type(f), IntegerField)
             self.assertEqual(f.default, 4)
 
         with self.subTest("with tuple"):
             t = field((StringField, IntegerField))
             self.assertEqual(t, (StringField, IntegerField))
 
             t = field((StringField, IntegerField), default=("3", 4))
+
             self.assertIsInstance(t, BaseField)
             self.assertIsInstance(t.complex[0].meta.field, StringField)
             self.assertIsInstance(t.complex[1].meta.field, IntegerField)
-            self.assertEqual(t.default, ("3", 4))
+            self.assertEqual(t.default, t.complex("3", 4))
+            self.assertEqual(to_tuple(t.default), ("3", 4))
 
         with self.subTest("with custom field"):
             INLField = define_flat_list_field(IntegerField, name="INLField")
             t = field(INLField, default=[3, 4, 5])
             self.assertTrue(isinstance(t, INLField))
             self.assertEqual(t.default, [3, 4, 5])
 
@@ -298,26 +306,26 @@
 
             def factory():
                 nonlocal x
                 x += 1
                 return ("3", x)
 
             t = field((StringField, IntegerField), default_factory=factory)
-            self.assertEqual(t.default, ("3", 1))
-            self.assertEqual(t.default, ("3", 2))
+            self.assertEqual(to_tuple(t.default), ("3", 1))
+            self.assertEqual(to_tuple(t.default), ("3", 2))
 
         with self.subTest("with nested tuple and default"):
             t = field((StringField, (StringField, IntegerField)))
             self.assertEqual(t, (StringField, (StringField, IntegerField)))
 
             t = field((StringField, (StringField, IntegerField)), default=("3", ("1", 4)))
             self.assertIsInstance(t, BaseField)
             self.assertIsInstance(t.complex[0].meta.field, StringField)
             self.assertIsInstance(t.complex[1].meta.field, BaseField)
-            self.assertEqual(t.default, ("3", ("1", 4)))
+            self.assertEqual(to_tuple(t.default), ("3", ("1", 4)))
 
     def test_api_field_function_illegal_arguments(self):
         with self.subTest("illegal basefield type"):
             with self.assertRaises(TypeError):
                 _ = field(int)
 
         with self.subTest("unequal len basefield and default"):
@@ -457,30 +465,25 @@
         #        self.assertEqual(fld.default, None)
         #        self.assertTrue(fld.has_default)
 
         fld = IntegerField(default=5)
         self.assertEqual(fld.default, 5)
         self.assertTrue(fld.has_default)
 
-        fld = IntegerField(default=inc)
-        self.assertTrue(fld.has_default)
+        fld = IntegerField(default_factory=inc)
+        self.assertTrue(fld.has_default_factory)
         self.assertEqual(fld.default, 1)
         self.assertEqual(fld.default, 2)
 
         # Added test for bug fix to distinguish a value that evaluates to False
         # from a None value
         fld = IntegerField(default=0)
         self.assertEqual(fld.default, 0)
         self.assertTrue(fld.has_default)
 
-        # A default can also be specified as a position argument
-        fld = IntegerField(0)
-        self.assertEqual(fld.default, 0)
-        self.assertTrue(fld.has_default)
-
     # --------------------------------------------------------------------------
     # Test catching invalid instantiation of a field (such as giving a bad
     # default values for a field).
     # --------------------------------------------------------------------------
     def test_api_catch_bad_field_instantiation(self):
         with self.assertRaises(TypeError) as ctx:
             fld = IntegerField(default="bad")
@@ -513,18 +516,14 @@
         self.assertFalse(fint1.index)
         self.assertFalse(fstr1.index)
         self.assertFalse(fconst1.index)
         self.assertTrue(fint2.index)
         self.assertTrue(fstr2.index)
         self.assertTrue(fconst2.index)
 
-        # Specify with positional arguments
-        f = IntegerField(1, True)
-        self.assertTrue(f.index)
-
     # --------------------------------------------------------------------------
     # Test the SimpleField class that handles all primitive types
     # (Integer, String, Constant).
     # --------------------------------------------------------------------------
     def test_api_simplefield(self):
         symint = Number(10)
         symstr = String("A string")
@@ -779,15 +778,15 @@
         symvalue2 = Function("", [Number(2), Function("", [Function("b", []), String("B")])])
         symnlist = Function("", [symvalue1, Function("", [symvalue2, Function("", [])])])
 
         value1 = (1, ("a", "A"))
         value2 = (2, ("b", "B"))
         nlist = (value1, value2)
 
-        self.assertEqual(XField.cltopy(symnlist), nlist)
+        self.assertEqual(to_tuple(XField.cltopy(symnlist)), nlist)
         self.assertEqual(XField.pytocl(nlist), symnlist)
 
     # --------------------------------------------------------------------------
     # Test defining a field that handles python lists/sequences as a tuple of
     # arbitrary length.
     # --------------------------------------------------------------------------
     def test_api_flat_list_field(self):
@@ -831,15 +830,15 @@
         symvalue2 = Function("", [Number(2), Function("", [Function("b", []), String("B")])])
         symnlist = Function("", [symvalue1, symvalue2])
 
         value1 = (1, ("a", "A"))
         value2 = (2, ("b", "B"))
         nlist = (value1, value2)
 
-        self.assertEqual(XField.cltopy(symnlist), nlist)
+        self.assertEqual(to_tuple(XField.cltopy(symnlist)), nlist)
         self.assertEqual(XField.pytocl(nlist), symnlist)
 
     # --------------------------------------------------------------------------
     # Test the different variants for defining a nested list encoding of the
     # Python sequence (1,2,3)
     # --------------------------------------------------------------------------
     def test_api_nested_list_field_alt(self):
@@ -1011,14 +1010,31 @@
         self.assertEqual(pyresult[1], "blah")
         self.assertEqual(pyresult.arg2, "blah")
 
         clresult = td.pytocl((1, "blah"))
         self.assertEqual(clresult, clob)
 
     # --------------------------------------------------------------------------
+    # Test that we define the new comparison operators in the template
+    # --------------------------------------------------------------------------
+    def test_predicate_comparison_operator_creation(self):
+        class P(Predicate, name="p"):
+            a = IntegerField
+            b = ConstantField
+
+        p1 = P(a=1, b="x")
+        p2 = P(a=1, b="x")
+        p3 = P(a=2, b="x")
+
+        tmp = {}
+        tmp[p1] = "P"
+        self.assertEqual(p1, p2)
+        self.assertNotEqual(p1, p3)
+
+    # --------------------------------------------------------------------------
     # Test that we can define predicates using the class syntax and test that
     # the getters and setters are connected properly to the predicate classes.
     # --------------------------------------------------------------------------
     def test_simple_predicate_defn(self):
 
         # A simple nullary predicate definition
         class P(Predicate):
@@ -1128,15 +1144,15 @@
 
     # --------------------------------------------------------------------------
     # Test default value for anonymous tuple
     # --------------------------------------------------------------------------
     def test_predicate_anonymous_field_with_default(self):
         class P(Predicate):
             first = IntegerField
-            tuple_ = (IntegerField(2), StringField("42"))
+            tuple_ = (IntegerField(default=2), StringField(default="42"))
 
         p = P(first=15, tuple_=(1, "2"))
         raw_p = Function("p", [Number(15), Function("", [Number(1), String("2")])])
         self.assertEqual(p.raw, raw_p)
 
         p = P(first=15)
         raw_p = Function("p", [Number(15), Function("", [Number(2), String("42")])])
@@ -1173,29 +1189,58 @@
         r2 = R(tuple_=("b", 2))
         s2 = S(tuple_=(2, "b", 2))
         t1 = T(tuple_=(1, "a"))
         t2 = T(tuple_=(2, "b"))
         tuple1 = tuple([1, "a"])
         tuple2 = tuple([2, "b"])
 
-        # Equality works even when the types are different
+        # Equality works even when the predicate types are different
         self.assertTrue(p1.tuple_ == p1_alt.tuple_)
         self.assertTrue(p1.tuple_ == q1.tuple_)
         self.assertTrue(p1.tuple_ == t1.tuple_)
-        self.assertTrue(p1.tuple_ == tuple1)
+
+        # New behaviour. Doesn't compare directly to tuple
+        self.assertFalse(p1.tuple_ == tuple1)
+        self.assertTrue(tuple(p1.tuple_) == tuple1)
 
         self.assertNotEqual(type(p1.tuple_), type(t1.tuple_))
-        #        self.assertNotEqual(type(p1.tuple_), type(t1))
 
         self.assertTrue(p1.tuple_ != p2.tuple_)
         self.assertTrue(p1.tuple_ != q2.tuple_)
         self.assertTrue(p1.tuple_ != r2.tuple_)
         self.assertTrue(p1.tuple_ != s2.tuple_)
         self.assertTrue(p1.tuple_ != t2.tuple_)
-        self.assertTrue(p1.tuple_ != tuple2)
+
+        self.assertTrue(p1.tuple_ != tuple1)
+        self.assertFalse(tuple(p1.tuple_) != tuple1)
+
+    # --------------------------------------------------------------------------
+    # Testing comparison between tuple fields where the corresponding python tuples
+    # can contain incomparible objects.
+    # --------------------------------------------------------------------------
+    def test_predicate_with_incomparable_python_tuples(self):
+        class P(Predicate):
+            tuple_ = field((SimpleField, SimpleField))
+
+        class Q(Predicate):
+            tuple_ = field((IntegerField, IntegerField))
+
+        ptuple = P.tuple_.meta.complex
+        qtuple = Q.tuple_.meta.complex
+
+        self.assertTrue(ptuple(1, 2) == qtuple(1, 2))
+        self.assertTrue(ptuple("a", "b") != qtuple(1, 2))
+
+        # NOTE: the following throws a TypeError when comparing two Python tuples but works
+        # with clorm tuples.
+        # error: self.assertTrue(("a", "b") > (1,2))
+        self.assertTrue(ptuple("a", "b") > qtuple(1, 2))
+        self.assertTrue(ptuple("a", "b") >= qtuple(1, 2))
+        self.assertFalse(ptuple("a", "b") < qtuple(1, 2))
+        self.assertFalse(ptuple("a", "b") <= qtuple(1, 2))
 
     # --------------------------------------------------------------------------
     # Test predicates with default fields
     # --------------------------------------------------------------------------
     def test_predicate_with_multi_field(self):
 
         # Test declaration of predicates with Simple and String terms
@@ -2109,69 +2154,97 @@
     # --------------------------------------------------------------------------
     # Test predicate equality
     # --------------------------------------------------------------------------
     def test_predicate_comparison_operator_overload_signed(self):
         class P(Predicate):
             a = IntegerField
 
-        class Q(Predicate):
-            a = IntegerField
-
         p1 = P(1)
         neg_p1 = P(1, sign=False)
         p2 = P(2)
         neg_p2 = P(2, sign=False)
-        q1 = Q(1)
-
-        self.assertTrue(neg_p1 < neg_p2)
-        self.assertTrue(neg_p1 < p1)
-        self.assertTrue(neg_p1 < p2)
-        self.assertTrue(neg_p2 < p1)
-        self.assertTrue(neg_p2 < p2)
-        self.assertTrue(p1 < p2)
-
-        self.assertTrue(p2 > p1)
-        self.assertTrue(p2 > neg_p2)
-        self.assertTrue(p2 > neg_p1)
-        self.assertTrue(p1 > neg_p2)
-        self.assertTrue(p1 > neg_p1)
-        self.assertTrue(neg_p2 > neg_p1)
-
-        # Different predicate sub-classes are incomparable
 
-    #        with self.assertRaises(TypeError) as ctx:
-    #            self.assertTrue(p1 < q1)
+        # NOTE: 20240428 see note at top about change of semantics
+        self.assertTrue((neg_p1.raw < p1.raw) == (neg_p1 < p1))
+        self.assertTrue((neg_p1.raw < p2.raw) == (neg_p1 < p2))
+        self.assertTrue((neg_p2.raw < p1.raw) == (neg_p2 < p1))
+        self.assertTrue((neg_p2.raw < p2.raw) == (neg_p2 < p2))
+        self.assertTrue((p1.raw < p2.raw) == (p1 < p2))
 
     # --------------------------------------------------------------------------
     # Test a simple predicate with a field that has a function default
     # --------------------------------------------------------------------------
-    def test_predicate_with_function_default(self):
+    def test_predicate_with_default_factory(self):
         val = 0
 
         def inc():
             nonlocal val
             val += 1
             return val
 
         class Fact(Predicate):
-            anum = IntegerField(default=inc)
+            anum = IntegerField(default_factory=inc)
             astr = StringField()
 
         func = Function("fact", [Number(1), String("test")])
         f1 = Fact(1, "test")
         f2 = Fact(astr="test")  # uses the default
         f3 = Fact(astr="test")  # second use of the default
         f4 = Fact(astr="test")  # third use of the default
 
         self.assertEqual(f2.anum, 1)
         self.assertEqual(f3.anum, 2)
         self.assertEqual(f4.anum, 3)
         self.assertEqual(f1, f2)
         self.assertEqual(f1.raw, func)
 
+    # ---------------------------------------------------------------------------------------
+    # Test a predicate a complex field that has an implicit default based on its subfields
+    # ---------------------------------------------------------------------------------------
+    def test_predicate_with_anon_tuple_field_with_implicit_default_factory(self):
+        val = 0
+
+        def inc():
+            nonlocal val
+            val += 1
+            return val
+
+        class Outer(Predicate):
+            x = (IntegerField(default_factory=inc), StringField(default="blah"))
+
+        x1 = Function("", [Number(1), String("blah")])
+        x2 = Function("", [Number(2), String("blah")])
+
+        self.assertEqual(Outer().x, x1)
+        self.assertEqual(Outer().x, x2)
+
+    # ---------------------------------------------------------------------------------------
+    # Test a predicate a complex field that has an implicit default based on its subfields
+    # ---------------------------------------------------------------------------------------
+    def test_predicate_with_complex_field_with_implicit_default_factory(self):
+        val = 0
+
+        def inc():
+            nonlocal val
+            val += 1
+            return val
+
+        class X(Predicate):
+            a: int = field(IntegerField, default_factory=inc)
+            b: str = field(StringField, default="blah")
+
+        class Outer(Predicate):
+            x = field(X.Field)
+
+        x1 = Function("x", [Number(1), String("blah")])
+        x2 = Function("x", [Number(2), String("blah")])
+
+        self.assertEqual(Outer().x, x1)
+        self.assertEqual(Outer().x, x2)
+
     # --------------------------------------------------------------------------
     # Test that we can initialise using positional arguments
     # --------------------------------------------------------------------------
     def test_predicate_init_positional(self):
         class Fact(Predicate):
             anum = IntegerField(default=1)
             astr = StringField()
@@ -2316,17 +2389,17 @@
         self.assertEqual(f2, af2.raw)
         self.assertEqual(af2.atup.aint, 4)
 
         # Define a predicate with a bad default value
         with self.assertRaises(TypeError) as ctx:
 
             class Fact2(Predicate):
-                afun = Fun.Field(default=(1, "str"))
+                afun = Fun.Field(default=6)
 
-        check_errmsg("""Invalid default value "(1, 'str')" for FunField""", ctx)
+        check_errmsg("""Invalid default value "6" for FunField""", ctx)
 
     # --------------------------------------------------------------------------
     # Test the simple_predicate function as a mechanism for defining
     # predicates
     # --------------------------------------------------------------------------
     def test_simple_predicate_function(self):
         class Pred2(Predicate):
@@ -2419,14 +2492,15 @@
     #        with self.assertRaises(IndexError) as ctx: f[3] = 4
     #        with self.assertRaises(TypeError) as ctx: f['bob'] = 4
 
     # --------------------------------------------------------------------------
     # Test predicate equality
     # --------------------------------------------------------------------------
     def test_predicate_comparison_operator_overloads(self):
+        # NOTE: 20240428 see note at top about change of semantics
 
         f1 = Function("fact", [Number(1)])
         f2 = Function("fact", [Number(2)])
 
         class Fact(Predicate):
             anum = IntegerField()
 
@@ -2448,17 +2522,17 @@
                 name = "fact"
 
         ag1 = Fact2(anum=1)
 
         self.assertEqual(f1, af1.raw)
         self.assertEqual(af1.raw, f1)
         self.assertEqual(af1.raw, ag1.raw)
-        self.assertNotEqual(af1, ag1)
-        self.assertNotEqual(af1, f1)
-        self.assertNotEqual(f1, af1)
+        self.assertEqual(af1, ag1)
+        self.assertEqual(af1, f1)
+        self.assertEqual(f1, af1)
 
         self.assertTrue(af1 < af2)
         self.assertTrue(af1 <= af2)
         self.assertTrue(af2 > af1)
         self.assertTrue(af2 >= af1)
 
         # clingo.Symbol currently does not implement NotImplemented for
@@ -2474,14 +2548,16 @@
             self.assertTrue(af1 <= f2)
             self.assertTrue(f2 >= af1)
 
     # --------------------------------------------------------------------------
     # Test predicate equality
     # --------------------------------------------------------------------------
     def test_comparison_operator_overloads_complex(self):
+        # NOTE: 20240428 see note at top about change of semantics
+
         class SwapField(IntegerField):
             pytocl = lambda x: 100 - x
             cltopy = lambda x: 100 - x
 
         class AComplex(ComplexTerm):
             swap = SwapField()
             norm = IntegerField()
@@ -2493,23 +2569,20 @@
 
         rf1 = f1.raw
         rf2 = f2.raw
         rf3 = f3.raw
         for rf in [rf1, rf2, rf3]:
             self.assertEqual(rf.arguments[0], rf.arguments[1])
 
-        # Test the the comparison operator for the complex term is using the
-        # swapped values so that the comparison is opposite to what the raw
-        # field says.
         self.assertTrue(rf1 < rf2)
         self.assertTrue(rf2 < rf3)
-        self.assertTrue(f1 > f2)
-        self.assertTrue(f2 > f3)
-        self.assertTrue(f2 < f1)
-        self.assertTrue(f3 < f2)
+        self.assertTrue(f1 < f2)
+        self.assertTrue(f2 < f3)
+        self.assertTrue(f2 > f1)
+        self.assertTrue(f3 > f2)
         self.assertEqual(f3, f4)
 
     # --------------------------------------------------------------------------
     # Test unifying a symbol with a predicate
     # --------------------------------------------------------------------------
     def test_unifying_symbol_and_predicate(self):
         class Fact(Predicate):
```

### Comparing `Clorm-1.5.1/tests/test_orm_factbase.py` & `clorm-1.6.0/tests/test_orm_factbase.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,23 @@
 # Official Clorm API imports for the core complements
 from clorm.orm import (
     ComplexTerm,
     ConstantField,
     FactBase,
     IntegerField,
     Predicate,
+    SimpleField,
     StringField,
     alias,
     asc,
     desc,
     func,
     hashable_path,
     in_,
+    notin_,
     path,
     ph1_,
     ph2_,
     ph_,
 )
 from clorm.orm.core import field
 from clorm.orm.query import fixed_join_order
@@ -43,14 +45,15 @@
 # ------------------------------------------------------------------------------
 # ------------------------------------------------------------------------------
 
 __all__ = [
     "FactBaseTestCase",
     "QueryAPI1TestCase",
     "QueryAPI2TestCase",
+    "QueryWithTupleTestCase",
     "SelectJoinTestCase",
     "MembershipQueriesTestCase",
     "FactBasePicklingTestCase",
 ]
 
 # ------------------------------------------------------------------------------
 #
@@ -706,14 +709,28 @@
             "%     a(a,(a_,b_))\n"
             "% --------------------\n"
         )
         result = fb.asp_str(commented=True)
         self.assertIn(expected_sig_predC, result)
         self.assertIn(expected_sig_predA, result)
 
+    # --------------------------------------------------------------------------
+    # Test the asp output string with sorting and incomparable terms
+    # --------------------------------------------------------------------------
+    def test_factbase_aspstr_sorted_incomparable(self):
+        class A(Predicate):
+            x = field(SimpleField)
+
+        fb = FactBase([A(1), A(2), A("b")])
+        q = fb.query(A).ordered()
+        self.assertTrue(list(q.all()) == [A(1), A(2), A("b")])
+        tmpstr1 = ".\n".join(f"{x}" for x in q.all()) + ".\n"
+        tmpstr2 = fb.asp_str(sorted=True)
+        self.assertTrue(tmpstr1 == tmpstr2)
+
 
 # ------------------------------------------------------------------------------
 # Test QueryAPI version 1 (called via FactBase.select() and FactBase.delete())
 # ------------------------------------------------------------------------------
 
 
 class QueryAPI1TestCase(unittest.TestCase):
@@ -1114,14 +1131,17 @@
         q = fb.select(Afact).order_by(desc(Afact.str1), Afact.num1)
         self.assertEqual([f3, f2, f4, f1, f5], list(q.get()))
 
     # --------------------------------------------------------------------------
     #   Test that select works with order_by for complex term
     # --------------------------------------------------------------------------
     def test_api_factbase_select_order_by_complex_term(self):
+        # NOTE: behavior change 20240428 - ordering is based on the underlying clingo.Symbol
+        # object and not the python translation. So using SwapField won't change the ordering
+        # for AComplex objects.
         class SwapField(IntegerField):
             pytocl = lambda x: 100 - x
             cltopy = lambda x: 100 - x
 
         class AComplex(ComplexTerm):
             swap = SwapField(index=True)
             norm = IntegerField(index=True)
@@ -1141,18 +1161,21 @@
 
         fb = FactBase(facts=[f1, f2, f3, f4], indexes=[AFact.astr, AFact.cmplx])
 
         q = fb.select(AFact).order_by(AFact.astr)
         self.assertEqual([f1, f2, f3, f4], list(q.get()))
 
         q = fb.select(AFact).order_by(AFact.cmplx, AFact.astr)
-        self.assertEqual([f3, f4, f2, f1], list(q.get()))
+        self.assertEqual([f1, f2, f3, f4], list(q.get()))
 
         q = fb.select(AFact).where(AFact.cmplx <= ph1_).order_by(AFact.cmplx, AFact.astr)
-        self.assertEqual([f3, f4, f2], list(q.get(cmplx2)))
+        self.assertEqual([f1, f2], list(q.get(cmplx2)))
+
+        q = fb.select(AFact).where(AFact.cmplx >= ph1_).order_by(AFact.cmplx, AFact.astr)
+        self.assertEqual([f2, f3, f4], list(q.get(cmplx2)))
 
     # --------------------------------------------------------------------------
     #   Test that select works with order_by for complex term
     # --------------------------------------------------------------------------
     def test_api_factbase_select_complex_term_placeholders(self):
         class AFact(Predicate):
             astr = StringField()
@@ -1274,16 +1297,15 @@
         s2 = fb.select(Fact).where(Fact.ct1 == ph1_)
         s3 = fb.select(Fact).where(Fact.ct2 == ph1_)
         s4 = fb.select(Fact).where(Fact.ct3 == ph1_)
 
         self.assertEqual(list(s1.get(20)), [f2, f1])
         self.assertEqual(list(s2.get(CT(20, "b"))), [f2])
 
-        # NOTE: Important test as it requires tuple complex terms to have the
-        # same hash as the corresponding python tuple.
+        # NOTE: This requires Python tuple to be converted to a clorm tuple.
         self.assertEqual(list(s3.get((1, 2))), [f2])
         self.assertEqual(list(s4.get((2, 1))), [f2])
 
         # One query doesn't use the index
         s4 = fb.select(Fact).where(Fact.ct1.str1 == ph1_)
         self.assertEqual(list(s4.get("c")), [f3])
 
@@ -1687,14 +1709,110 @@
 
         # Select everything with an equality join
         with self.assertRaises(ValueError) as ctx:
             tmp = list(fb.query(F, G).all())
         check_errmsg("A query over multiple predicates is incomplete", ctx)
 
 
+# ------------------------------------------------------------------------------------------
+# Test some special cases involving passing a Python tuple instead of using the clorm tuple.
+# ------------------------------------------------------------------------------------------
+
+
+class QueryWithTupleTestCase(unittest.TestCase):
+    def setUp(self):
+        class F(Predicate):
+            atuple = field((IntegerField, StringField))
+            other = StringField
+
+        class G(Predicate):
+            atuple = field((SimpleField, StringField))
+            other = StringField
+
+        self.F = F
+        self.G = G
+
+        self.factbase = FactBase(
+            [
+                F((1, "a"), "i"),
+                F((2, "b"), "j"),
+                F((3, "a"), "k"),
+                G(("a", "a"), "x"),
+                G((2, "b"), "y"),
+                G(("e", "e"), "z"),
+            ]
+        )
+
+    # --------------------------------------------------------------------------
+    #   Some tuple predicate instance comparisons
+    # --------------------------------------------------------------------------
+    def test_basic_clorm_tuple_in_comparison(self):
+        G = self.G
+        fb = self.factbase
+        cltuple = G.atuple.meta.complex
+        expected = [
+            G((2, "b"), "y"),
+            G(("a", "a"), "x"),
+        ]
+
+        # NOTE: the version with python tuples fails to find the matching tuples because we can
+        # no longer directly compare python tuples with clorm tuples.
+
+        pytuples = {("a", "a"), (2, "b")}
+        q1 = fb.query(G).where(in_(G.atuple, pytuples)).ordered()
+        self.assertEqual(list(q1.all()), [])
+        # this fails: self.assertEqual(list(q1.all()), expected)
+
+        cltuples = {cltuple("a", "a"), cltuple(2, "b")}
+        q2 = fb.query(G).where(in_(G.atuple, cltuples)).ordered()
+        self.assertEqual(list(q2.all()), expected)
+
+    # --------------------------------------------------------------------------
+    #   Complex query where the join is on a tuple object
+    # --------------------------------------------------------------------------
+    def test_api_join_on_clorm_tuple(self):
+        F = self.F
+        G = self.G
+        fb = self.factbase
+
+        # Select everything with an equality join
+        q = fb.query(G, F).join(F.atuple == G.atuple).where(F.other == "j")
+        expected = [(G((2, "b"), "y"), F((2, "b"), "j"))]
+        self.assertEqual(list(q.all()), expected)
+
+    # --------------------------------------------------------------------------
+    #   Complex query with a where containing a tuple
+    # --------------------------------------------------------------------------
+    def test_api_where_with_python_tuple(self):
+        F = self.F
+        fb = self.factbase
+
+        # The Python tuple passed in the where clause
+        q = fb.query(F).where(F.atuple == (2, "b"))
+        expected = [F((2, "b"), "j")]
+        self.assertEqual(list(q.all()), expected)
+
+        # The Python tuple passed in the bind
+        q = fb.query(F).where(F.atuple == ph1_).bind((2, "b"))
+        expected = [F((2, "b"), "j")]
+        self.assertEqual(list(q.all()), expected)
+
+    # --------------------------------------------------------------------------
+    #   Complex query sorting on Clorm tuple where the corresponding Python tuple
+    #   is incomparable.
+    #   --------------------------------------------------------------------------
+    def test_api_sorting_with_incomparable_elements(self):
+        G = self.G
+        fb = self.factbase
+
+        q = fb.query(G).order_by(G.atuple)
+        expected = [G((2, "b"), "y"), G(("a", "a"), "x"), G(("e", "e"), "z")]
+        self.assertEqual(list(q.all()), expected)
+
+
 # ------------------------------------------------------------------------------
 # Tests for additional V2 select join  statements
 # ------------------------------------------------------------------------------
 
 
 class SelectJoinTestCase(unittest.TestCase):
     def setUp(self):
```

### Comparing `Clorm-1.5.1/tests/test_orm_factcontainers.py` & `clorm-1.6.0/tests/test_orm_factcontainers.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_orm_noclingo.py` & `clorm-1.6.0/tests/test_orm_noclingo.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_orm_query.py` & `clorm-1.6.0/tests/test_orm_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     validate_join_expression,
     validate_orderby_expression,
     validate_where_expression,
     where_expression_to_cnf,
     where_expression_to_nnf,
 )
 
-from .support import check_errmsg, check_errmsg_contains
+from .support import check_errmsg, check_errmsg_contains, to_tuple
 
 ###### NOTE: The QueryOutput tests need to be turned into QueryExecutor
 ###### tests. We can then delete QueryOutput which is not being used for
 ###### anything.
 
 
 # ------------------------------------------------------------------------------
@@ -428,15 +428,15 @@
         f1 = F(1, (1, 2))
         f2 = F(2, (3, 4))
 
         # FIXUP
         getter = make_input_alignment_functor([F], [F.acomplex])
         result = getter((f1,))
         tmp = ((1, 2),)
-        self.assertEqual(result, tmp)
+        self.assertEqual(to_tuple(result), tmp)
 
     # ------------------------------------------------------------------------------
     # ------------------------------------------------------------------------------
     def test_nonapi_StandardComparator(self):
         F = self.F
         G = self.G
         X = alias(F)
@@ -541,17 +541,17 @@
             acomplex = (IntegerField, IntegerField)
 
         f1 = F(1, (1, 2))
         f2 = F(1, (1, 3))
 
         getter = make_input_alignment_functor([F], [F.acomplex])
         result = getter((f1,))
-        self.assertEqual(result, ((1, 2),))
+        self.assertEqual(to_tuple(result), ((1, 2),))
 
-        sc = SC(operator.eq, [F.acomplex, (1, 2)])
+        sc = SC(operator.eq, [F.acomplex, F.meta[1].defn.complex(1, 2)])
         cmp = sc.make_callable([F])
         self.assertTrue(cmp((f1,)))
         self.assertFalse(cmp((f2,)))
 
     # ------------------------------------------------------------------------------
     # Test the standard comparator keyable function
     # ------------------------------------------------------------------------------
```

### Comparing `Clorm-1.5.1/tests/test_orm_symbols_facts.py` & `clorm-1.6.0/tests/test_orm_symbols_facts.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 
         class Afact3(Predicate):
             class Fun(ComplexTerm):
                 fnum = IntegerField()
 
             anum = IntegerField()
             afun = Fun.Field()
+
             #            afun=ComplexField(Fun)
             class Meta:
                 name = "afact"
 
         class Bfact(Predicate):
             anum = IntegerField()
             astr = StringField()
```

### Comparing `Clorm-1.5.1/tests/test_util_oset.py` & `clorm-1.6.0/tests/test_util_oset.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_util_tools.py` & `clorm-1.6.0/tests/test_util_tools.py`

 * *Files identical despite different names*

### Comparing `Clorm-1.5.1/tests/test_util_wrapper.py` & `clorm-1.6.0/tests/test_util_wrapper.py`

 * *Files identical despite different names*


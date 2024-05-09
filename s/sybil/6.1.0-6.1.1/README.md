# Comparing `tmp/sybil-6.1.0.tar.gz` & `tmp/sybil-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-6.1.0.tar", last modified: Mon Apr 22 18:14:13 2024, max compression
+gzip compressed data, was "sybil-6.1.1.tar", last modified: Thu May  9 05:45:47 2024, max compression
```

## Comparing `sybil-6.1.0.tar` & `sybil-6.1.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.639285 sybil-6.1.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2024-04-22 18:13:57.000000 sybil-6.1.0/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1618 2024-04-22 18:14:13.639285 sybil-6.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2024-04-22 18:13:57.000000 sybil-6.1.0/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2024-04-22 18:14:13.639285 sybil-6.1.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2024-04-22 18:13:57.000000 sybil-6.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.627285 sybil-6.1.0/sybil/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      207 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9908 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/document.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.631285 sybil-6.1.0/sybil/evaluators/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/evaluators/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/evaluators/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2352 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/evaluators/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1019 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/evaluators/python.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3210 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/evaluators/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2904 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/example.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.631285 sybil-6.1.0/sybil/integration/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/integration/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5244 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/integration/pytest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1801 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/integration/unittest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.631285 sybil-6.1.0/sybil/parsers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.631285 sybil-6.1.0/sybil/parsers/abstract/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/abstract/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      710 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/abstract/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3066 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/abstract/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2201 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/abstract/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3442 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/abstract/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/abstract/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/doctest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.631285 sybil-6.1.0/sybil/parsers/markdown/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/markdown/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/markdown/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1786 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/markdown/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6260 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/markdown/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      349 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/markdown/skip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.635285 sybil-6.1.0/sybil/parsers/myst/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      318 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/myst/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      538 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/myst/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2148 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/myst/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      993 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/myst/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3887 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/myst/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/myst/skip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.635285 sybil-6.1.0/sybil/parsers/rest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/rest/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3038 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/rest/capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/rest/clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1516 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/rest/codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/rest/doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3500 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/rest/lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      299 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/rest/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/parsers/skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1204 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/python.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3683 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/region.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6879 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/sybil.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/text.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2024-04-22 18:13:57.000000 sybil-6.1.0/sybil/typing.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.639285 sybil-6.1.0/sybil.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1618 2024-04-22 18:14:13.000000 sybil-6.1.0/sybil.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1913 2024-04-22 18:14:13.000000 sybil-6.1.0/sybil.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-22 18:14:13.000000 sybil-6.1.0/sybil.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2024-04-22 18:14:13.000000 sybil-6.1.0/sybil.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-22 18:14:13.000000 sybil-6.1.0/sybil.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-22 18:14:13.639285 sybil-6.1.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_capture.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5649 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_compatibility.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1980 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_docs_examples.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6625 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5872 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20042 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_functional.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1449 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2466 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_lexing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      765 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_markdown_lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      345 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_myst_clear.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4910 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_myst_codeblock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2796 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_myst_doctest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16683 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_myst_lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      305 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_myst_skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13265 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_rest_lexers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3286 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_skip.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12607 2024-04-22 18:13:57.000000 sybil-6.1.0/tests/test_sybil.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.170792 sybil-6.1.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1104 2024-05-09 05:45:35.000000 sybil-6.1.1/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1618 2024-05-09 05:45:47.170792 sybil-6.1.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      645 2024-05-09 05:45:35.000000 sybil-6.1.1/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      334 2024-05-09 05:45:47.170792 sybil-6.1.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2024-05-09 05:45:35.000000 sybil-6.1.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.162792 sybil-6.1.1/sybil/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      207 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9908 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/document.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.162792 sybil-6.1.1/sybil/evaluators/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/evaluators/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      143 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/evaluators/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2352 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/evaluators/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1019 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/evaluators/python.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3210 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/evaluators/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2904 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/example.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.162792 sybil-6.1.1/sybil/integration/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/integration/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5244 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/integration/pytest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1801 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/integration/unittest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.162792 sybil-6.1.1/sybil/parsers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.162792 sybil-6.1.1/sybil/parsers/abstract/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/abstract/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      710 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/abstract/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3066 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/abstract/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2201 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/abstract/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3537 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/abstract/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/abstract/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      385 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/doctest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.166792 sybil-6.1.1/sybil/parsers/markdown/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/markdown/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/markdown/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1786 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/markdown/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6147 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/markdown/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      349 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/markdown/skip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.166792 sybil-6.1.1/sybil/parsers/myst/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      318 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/myst/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      538 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/myst/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2148 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/myst/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      993 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/myst/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3887 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/myst/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/myst/skip.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.166792 sybil-6.1.1/sybil/parsers/rest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/rest/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3038 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/rest/capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/rest/clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1516 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/rest/codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/rest/doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3500 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/rest/lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      299 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/rest/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/parsers/skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1204 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/python.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3683 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/region.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6879 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/sybil.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/text.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      824 2024-05-09 05:45:35.000000 sybil-6.1.1/sybil/typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.170792 sybil-6.1.1/sybil.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1618 2024-05-09 05:45:47.000000 sybil-6.1.1/sybil.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1913 2024-05-09 05:45:47.000000 sybil-6.1.1/sybil.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-09 05:45:47.000000 sybil-6.1.1/sybil.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2024-05-09 05:45:47.000000 sybil-6.1.1/sybil.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-09 05:45:47.000000 sybil-6.1.1/sybil.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-09 05:45:47.170792 sybil-6.1.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_capture.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5649 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_compatibility.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1980 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_docs_examples.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6625 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5872 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20042 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_functional.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1449 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3116 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_lexing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      765 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_markdown_lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      345 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_myst_clear.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6249 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_myst_codeblock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2796 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_myst_doctest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16685 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_myst_lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      305 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_myst_skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13328 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_rest_lexers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3286 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_skip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12607 2024-05-09 05:45:35.000000 sybil-6.1.1/tests/test_sybil.py
```

### Comparing `sybil-6.1.0/LICENSE.txt` & `sybil-6.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/PKG-INFO` & `sybil-6.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil
-Version: 6.1.0
+Version: 6.1.1
 Summary: Automated testing for the examples in your code and documentation.
 Home-page: https://github.com/simplistix/sybil
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sybil-6.1.0/README.rst` & `sybil-6.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/setup.py` & `sybil-6.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup, find_packages
 
 base_dir = os.path.dirname(__file__)
 
 setup(
     name='sybil',
-    version='6.1.0',
+    version='6.1.1',
     author='Chris Withers',
     author_email='chris@withers.org',
     license='MIT',
     description="Automated testing for the examples in your code and documentation.",
     long_description=open('README.rst').read(),
     url='https://github.com/simplistix/sybil',
     classifiers=[
```

### Comparing `sybil-6.1.0/sybil/document.py` & `sybil-6.1.1/sybil/document.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/evaluators/doctest.py` & `sybil-6.1.1/sybil/evaluators/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/evaluators/python.py` & `sybil-6.1.1/sybil/evaluators/python.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/evaluators/skip.py` & `sybil-6.1.1/sybil/evaluators/skip.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/example.py` & `sybil-6.1.1/sybil/example.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/integration/pytest.py` & `sybil-6.1.1/sybil/integration/pytest.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/integration/unittest.py` & `sybil-6.1.1/sybil/integration/unittest.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/abstract/clear.py` & `sybil-6.1.1/sybil/parsers/abstract/clear.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/abstract/codeblock.py` & `sybil-6.1.1/sybil/parsers/abstract/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/abstract/doctest.py` & `sybil-6.1.1/sybil/parsers/abstract/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/abstract/lexers.py` & `sybil-6.1.1/sybil/parsers/abstract/lexers.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,17 +64,21 @@
             if end_match is None:
                 raise LexingException(
                     f'Could not match {end_pattern.pattern!r} in {document.path}:\n'
                     f'{document.text[source_start:]!r}'
                 )
             source_end = end_match.start()
             source = document.text[source_start:source_end]
-            lines = source.splitlines(keepends=True)
-            stripped = ''.join(line[len(prefix):] for line in lines)
             lexemes['source'] = Lexeme(
-                textwrap.dedent(stripped),
+                strip_prefix(source, prefix),
                 offset=source_start-start_match.start(),
                 line_offset=start_match.group(0).count('\n')-1
             )
             if self.mapping:
                 lexemes = {dest: lexemes[source] for source, dest in self.mapping.items()}
             yield Region(start_match.start(), source_end, lexemes=lexemes)
+
+
+def strip_prefix(text: str, prefix: str) -> str:
+    lines = text.splitlines(keepends=True)
+    prefix_length = len(prefix)
+    return textwrap.dedent(''.join(line[prefix_length:] or line[-1] for line in lines))
```

### Comparing `sybil-6.1.0/sybil/parsers/abstract/skip.py` & `sybil-6.1.1/sybil/parsers/abstract/skip.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/markdown/codeblock.py` & `sybil-6.1.1/sybil/parsers/markdown/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/markdown/lexers.py` & `sybil-6.1.1/sybil/parsers/markdown/lexers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
-import textwrap
 from typing import Optional, Dict, Pattern, Iterable, Match, List
 
 from sybil import Document, Region, Lexeme
-from sybil.parsers.abstract.lexers import BlockLexer
+from sybil.parsers.abstract.lexers import BlockLexer, strip_prefix
 
 FENCE = re.compile(r"^(?P<prefix>[ \t]*)(?P<fence>`{3,}|~{3,})", re.MULTILINE)
 
 
 class RawFencedCodeBlockLexer:
     """
     A :class:`~sybil.typing.Lexer` for Markdown fenced code blocks allowing flexible lexing
@@ -55,18 +54,16 @@
             content_end = closing.start()
             region_end = closing.end()
         content = document.text[opening.end(): content_end]
         info = self.info_pattern.match(content)
         if info is None:
             return None
         lexemes = info.groupdict()
-        lines = content[info.end():].splitlines(keepends=True)
-        stripped = ''.join(line[len(opening.group('prefix')):] for line in lines)
         lexemes['source'] = Lexeme(
-            textwrap.dedent(stripped),
+            strip_prefix(content[info.end():], opening.group('prefix')),
             offset=len(opening.group(0))+info.end(),
             line_offset=0,
         )
         if self.mapping:
             lexemes = {dest: lexemes[source] for source, dest in self.mapping.items()}
         return Region(opening.start(), region_end, lexemes=lexemes)
```

### Comparing `sybil-6.1.0/sybil/parsers/myst/clear.py` & `sybil-6.1.1/sybil/parsers/myst/clear.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/myst/codeblock.py` & `sybil-6.1.1/sybil/parsers/myst/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/myst/doctest.py` & `sybil-6.1.1/sybil/parsers/myst/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/myst/lexers.py` & `sybil-6.1.1/sybil/parsers/myst/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/rest/capture.py` & `sybil-6.1.1/sybil/parsers/rest/capture.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/rest/codeblock.py` & `sybil-6.1.1/sybil/parsers/rest/codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/rest/doctest.py` & `sybil-6.1.1/sybil/parsers/rest/doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/parsers/rest/lexers.py` & `sybil-6.1.1/sybil/parsers/rest/lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/python.py` & `sybil-6.1.1/sybil/python.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/region.py` & `sybil-6.1.1/sybil/region.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/sybil.py` & `sybil-6.1.1/sybil/sybil.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil/typing.py` & `sybil-6.1.1/sybil/typing.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/sybil.egg-info/PKG-INFO` & `sybil-6.1.1/sybil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil
-Version: 6.1.0
+Version: 6.1.1
 Summary: Automated testing for the examples in your code and documentation.
 Home-page: https://github.com/simplistix/sybil
 Author: Chris Withers
 Author-email: chris@withers.org
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sybil-6.1.0/sybil.egg-info/SOURCES.txt` & `sybil-6.1.1/sybil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_capture.py` & `sybil-6.1.1/tests/test_capture.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_codeblock.py` & `sybil-6.1.1/tests/test_codeblock.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_compatibility.py` & `sybil-6.1.1/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_docs_examples.py` & `sybil-6.1.1/tests/test_docs_examples.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_doctest.py` & `sybil-6.1.1/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_document.py` & `sybil-6.1.1/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_functional.py` & `sybil-6.1.1/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_helpers.py` & `sybil-6.1.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_lexing.py` & `sybil-6.1.1/tests/test_lexing.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,40 @@
 def test_examples_from_parsing_tests():
     lexer = BlockLexer(start_pattern=re.compile('START'), end_pattern_template='END')
     path = sample_path('lexing-fail.txt')
     with ShouldRaise(LexingException(f"Could not match 'END' in {path}:\n'\\nEDN\\n'")):
         lex('lexing-fail.txt', lexer)
 
 
+def test_indented_block():
+    lexer = BlockLexer(
+        start_pattern=re.compile('(?P<prefix> *)START\n'),
+        end_pattern_template=' {{{len_prefix}}}END'
+    )
+    region, = lex('lexing-indented-block.txt', lexer)
+    compare(
+        region.lexemes,
+        expected={
+            'source': Lexeme(
+                "".join(
+                    (
+                        "\n",
+                        "line 1\n",
+                        "\n",
+                        "  line 2\n",
+                        "\n",
+                    )
+                ),
+                offset=0,
+                line_offset=0,
+            ),
+        }
+    )
+
+
 class TestLexemeStripping:
 
     @staticmethod
     def compare_lexeme(expected: Lexeme, actual: Lexeme):
 
         def _compare(x, y, context):
             if str(x) != str(y):
```

### Comparing `sybil-6.1.0/tests/test_markdown_lexers.py` & `sybil-6.1.1/tests/test_markdown_lexers.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_myst_codeblock.py` & `sybil-6.1.1/tests/test_myst_codeblock.py`

 * *Files 18% similar despite different names*

```diff
@@ -145,7 +145,58 @@
     future_import_checks('barry_as_FLUFL', 'print_function')
 
 
 def test_functional_future_imports():
     foo = future_import_checks('annotations')
     # This will keep working but not be an effective test once PEP 563 finally lands:
     assert foo.__code__.co_flags & __future__.annotations.compiler_flag
+
+
+def test_blank_lines():
+    examples, namespace = parse(
+        'myst-codeblock-blank-lines.md', PythonCodeBlockParser(), expected=1
+    )
+    example, = examples
+    compare(example.parsed, expected=''.join((
+        '\n',
+        'y = 0\n',
+        '# now a blank line:\n',
+        '\n',
+        'y += 1\n',
+        '# two blank lines:\n',
+        '\n',
+        '\n',
+        "assert not y, 'Boom!'\n",
+    )))
+    with pytest.raises(AssertionError) as excinfo:
+        example.evaluate()
+
+    # check the line number in the exception:
+    check_excinfo(example, excinfo, 'Boom!', lineno=12)
+
+
+def test_blank_lines_indented():
+    examples, namespace = parse(
+        "myst-codeblock-blank-lines-indented.md", PythonCodeBlockParser(), expected=1
+    )
+    (example,) = examples
+    compare(
+        example.parsed,
+        expected="".join(
+            (
+                "\n",
+                "y = 0\n",
+                "# now a blank line:\n",
+                "\n",
+                "y += 1\n",
+                "# two blank lines:\n",
+                "\n",
+                "\n",
+                "assert not y, 'Boom!'\n",
+            )
+        ),
+    )
+    with pytest.raises(AssertionError) as excinfo:
+        example.evaluate()
+
+    # check the line number in the exception:
+    check_excinfo(example, excinfo, "Boom!", lineno=12)
```

### Comparing `sybil-6.1.0/tests/test_myst_doctest.py` & `sybil-6.1.1/tests/test_myst_doctest.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_myst_lexers.py` & `sybil-6.1.1/tests/test_myst_lexers.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             'options': {},
             'source': "raise Exception('boom!')\n",
         }),
         Region(701, 753, lexemes={
             'directive': 'code-block',
             'arguments': 'python',
             'options': {},
-            'source': 'define_this = 1\n',
+            'source': 'define_this = 1\n\n',
         }),
     ])
 
 
 def test_myst_directives_with_mapping():
     lexer = DirectiveLexer(directive='directivename', arguments='.*', mapping={'arguments': 'foo'})
     compare(lex('myst-lexers.md', lexer), expected=[
```

### Comparing `sybil-6.1.0/tests/test_rest_lexers.py` & `sybil-6.1.1/tests/test_rest_lexers.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,18 @@
             'arguments': 'picture.png',
             'options': {
                 'scale': '50 %',
                 'alt': 'map to buried treasure'
             },
             'source': (
                 'This is the caption of the figure (a simple paragraph).\n'
+                '\n'
+                '\n'
                 ' .. topic:: Topic Title\n'
+                '\n'
                 '     Subsequent indented lines comprise\n'
                 '     the body of the topic, and are\n'
                 '     interpreted as body elements.'
             ),
         }),
         Region(620, 783, lexemes={
             'directive': 'topic',
```

### Comparing `sybil-6.1.0/tests/test_skip.py` & `sybil-6.1.1/tests/test_skip.py`

 * *Files identical despite different names*

### Comparing `sybil-6.1.0/tests/test_sybil.py` & `sybil-6.1.1/tests/test_sybil.py`

 * *Files identical despite different names*


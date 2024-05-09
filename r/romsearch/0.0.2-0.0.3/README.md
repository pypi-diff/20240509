# Comparing `tmp/romsearch-0.0.2.tar.gz` & `tmp/romsearch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romsearch-0.0.2.tar", last modified: Tue May  7 15:35:35 2024, max compression
+gzip compressed data, was "romsearch-0.0.3.tar", last modified: Wed May  8 11:56:07 2024, max compression
```

## Comparing `romsearch-0.0.2.tar` & `romsearch-0.0.3.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.695399 romsearch-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.679399 romsearch-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.683399 romsearch-0.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/ISSUE_TEMPLATE/console_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/ISSUE_TEMPLATE/feature_request.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.683399 romsearch-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/workflows/build_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 15:35:31.000000 romsearch-0.0.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-07 15:35:31.000000 romsearch-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 15:35:31.000000 romsearch-0.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-07 15:35:31.000000 romsearch-0.0.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 15:35:31.000000 romsearch-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 15:35:31.000000 romsearch-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43659 2024-05-07 15:35:35.695399 romsearch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-07 15:35:31.000000 romsearch-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.687399 romsearch-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/1g1r.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.687399 romsearch-0.0.2/docs/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/clonelists.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/dats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/defaults.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/platforms.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs/regex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/known_issues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.687399 romsearch-0.0.2/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/datparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/dupeparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/gamefinder.rst
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/romchooser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/romdownloader.rst
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/rommover.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/romparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules/romsearch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/reference_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-07 15:35:31.000000 romsearch-0.0.2/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-07 15:35:31.000000 romsearch-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.687399 romsearch-0.0.2/romsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/configs/clonelists/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/clonelists/retool.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/configs/dats/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/dats/no-intro.yml
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/dats/redump.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/configs/platforms/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Nintendo - GameCube.yml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Sony - PlayStation 2.yml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/platforms/Sony - PlayStation.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/regex.yml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/configs/sample_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.691399 romsearch-0.0.2/romsearch/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/dev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/dev/parsing_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.695399 romsearch-0.0.2/romsearch/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/datparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/dupeparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/gamefinder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/romchooser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/romdownloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/rommover.py
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/romparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/modules/romsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.695399 romsearch-0.0.2/romsearch/util/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/discord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/general.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-07 15:35:31.000000 romsearch-0.0.2/romsearch/util/regex_matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:35:35.695399 romsearch-0.0.2/romsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43659 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 15:35:35.000000 romsearch-0.0.2/romsearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:35:35.695399 romsearch-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.896916 romsearch-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.880916 romsearch-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.884916 romsearch-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/ISSUE_TEMPLATE/console_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/ISSUE_TEMPLATE/feature_request.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.884916 romsearch-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/workflows/build_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-08 11:56:03.000000 romsearch-0.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-08 11:56:03.000000 romsearch-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-08 11:56:03.000000 romsearch-0.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-08 11:56:03.000000 romsearch-0.0.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 11:56:03.000000 romsearch-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 11:56:03.000000 romsearch-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43725 2024-05-08 11:56:07.896916 romsearch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-08 11:56:03.000000 romsearch-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.888916 romsearch-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/1g1r.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.888916 romsearch-0.0.3/docs/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/clonelists.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/dats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/defaults.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs/regex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/known_issues.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.888916 romsearch-0.0.3/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/datparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/dupeparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/gamefinder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/romchooser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/romdownloader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/rommover.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/romparser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules/romsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/reference_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-08 11:56:03.000000 romsearch-0.0.3/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-08 11:56:03.000000 romsearch-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.888916 romsearch-0.0.3/romsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/configs/clonelists/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/clonelists/retool.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/configs/dats/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/dats/no-intro.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/dats/redump.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/configs/platforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Nintendo - GameCube.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Nintendo - Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Nintendo - Super Nintendo Entertainment System.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Sony - PlayStation 2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/platforms/Sony - PlayStation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/regex.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/configs/sample_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.892916 romsearch-0.0.3/romsearch/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/dev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/dev/parsing_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.896916 romsearch-0.0.3/romsearch/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/datparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9905 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/dupeparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/gamefinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15816 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/romchooser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/romdownloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/rommover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/romparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/modules/romsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.896916 romsearch-0.0.3/romsearch/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/discord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-08 11:56:03.000000 romsearch-0.0.3/romsearch/util/regex_matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:56:07.896916 romsearch-0.0.3/romsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43725 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 11:56:07.000000 romsearch-0.0.3/romsearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:56:07.896916 romsearch-0.0.3/setup.cfg
```

### Comparing `romsearch-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml` & `romsearch-0.0.3/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/.github/ISSUE_TEMPLATE/feature_request.yml` & `romsearch-0.0.3/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/.github/workflows/build_test.yaml` & `romsearch-0.0.3/.github/workflows/build_test.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/.github/workflows/publish.yaml` & `romsearch-0.0.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/.gitignore` & `romsearch-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/.readthedocs.yaml` & `romsearch-0.0.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/CHANGES.rst` & `romsearch-0.0.3/CHANGES.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+0.0.3 (2024-05-08)
+==================
+
+Features
+--------
+
+- Added Sony - PlayStation 2
+
+Fixes
+-----
+
+Configs
+~~~~~~~
+
+- Included dash between disc and number/letter for disc matching
+- Added specific regex options for PS2
+
 0.0.2 (2024-05-07)
 ==================
 
 Features
 --------
 
 - Added Nintendo - Nintendo Entertainment System
```

### Comparing `romsearch-0.0.2/LICENSE` & `romsearch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/PKG-INFO` & `romsearch-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.2
+Version: 0.0.3
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -726,12 +726,14 @@
 
 To get started, see the [documentation](https://romsearch.readthedocs.io/en/latest/).
 
 Currently, ROMSearch is in early development, and so many features may be added over time. At the moment, ROMSearch
 works for the following consoles:
 
 * Nintendo - GameCube
+* Nintendo - Nintendo Entertainment System
 * Nintendo - Super Nintendo Entertainment System
 * Sony - PlayStation
+* Sony - PlayStation 2
 
 but be aware there may be quirks that will only become apparent over time. We encourage users to open
 [issues](https://github.com/bbtufty/romsearch/issues) as and where they find them.
```

### Comparing `romsearch-0.0.2/README.md` & `romsearch-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,12 +20,14 @@
 
 To get started, see the [documentation](https://romsearch.readthedocs.io/en/latest/).
 
 Currently, ROMSearch is in early development, and so many features may be added over time. At the moment, ROMSearch
 works for the following consoles:
 
 * Nintendo - GameCube
+* Nintendo - Nintendo Entertainment System
 * Nintendo - Super Nintendo Entertainment System
 * Sony - PlayStation
+* Sony - PlayStation 2
 
 but be aware there may be quirks that will only become apparent over time. We encourage users to open
 [issues](https://github.com/bbtufty/romsearch/issues) as and where they find them.
```

### Comparing `romsearch-0.0.2/docs/1g1r.rst` & `romsearch-0.0.3/docs/1g1r.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/Makefile` & `romsearch-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/conf.py` & `romsearch-0.0.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'romsearch'
 copyright = '2024, bbtufty'
 author = 'bbtufty'
-release = '0.0.2'
+release = '0.0.3'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc',
               'sphinx.ext.coverage',
               'sphinx.ext.napoleon',
```

### Comparing `romsearch-0.0.2/docs/configs/config.rst` & `romsearch-0.0.3/docs/configs/config.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/configs/dats.rst` & `romsearch-0.0.3/docs/configs/dats.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/configs/platforms.rst` & `romsearch-0.0.3/docs/configs/platforms.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/configs/regex.rst` & `romsearch-0.0.3/docs/configs/regex.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/configuration.rst` & `romsearch-0.0.3/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/index.rst` & `romsearch-0.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/intro.rst` & `romsearch-0.0.3/docs/intro.rst`

 * *Files 7% similar despite different names*

```diff
@@ -27,16 +27,18 @@
 To get started, see the :doc:`installation <installation>` and :doc:`configuration <configuration>` pages. For the
 philosophy behind how ROMSearch chooses a ROM, see :doc:`1G1R <1g1r>`.
 
 Currently, ROMSearch is in early development, and so many features may be added over time. At the moment, ROMSearch
 has the capability for:
 
 * Nintendo - GameCube
+* Nintendo - Nintendo Entertainment System
 * Nintendo - Super Nintendo Entertainment System
 * Sony - PlayStation
+* Sony - PlayStation 2
 
 but be aware there may be quirks that will only become apparent over time. We encourage users to open
 `issues <https://github.com/bbtufty/romsearch/issues>`_ as and where they find them. Known issues can be found at
 :doc:`known issues <known_issues>`.
 
 ROMSearch is also built in such a way that other platforms/filters can be added in a simple way using config files
 rather than manually adding to the base code. For more details of how these work, see the various
```

### Comparing `romsearch-0.0.2/docs/make.bat` & `romsearch-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/modules/datparser.rst` & `romsearch-0.0.3/docs/modules/datparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/modules/dupeparser.rst` & `romsearch-0.0.3/docs/modules/dupeparser.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/docs/modules/romdownloader.rst` & `romsearch-0.0.3/docs/modules/romdownloader.rst`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/pyproject.toml` & `romsearch-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "romsearch"
-version = "0.0.2"
+version = "0.0.3"
 description = "One Stop ROM Shop"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 
 authors = [
     {name = "bbtufty"},
```

### Comparing `romsearch-0.0.2/romsearch/__init__.py` & `romsearch-0.0.3/romsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/configs/defaults.yml` & `romsearch-0.0.3/romsearch/configs/defaults.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/configs/regex.yml` & `romsearch-0.0.3/romsearch/configs/regex.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 languages:
   pattern: "\\((([languages])(,\\s?)?)*\\)"
   type: "list"
   flags: "NOFLAG"
 
 multi_disc:
-  pattern: "\\((Dis[ck]|Seite) [0-9A-Z]\\)"
+  pattern: "\\((Dis[ck]|Seite)[-\\s][0-9A-Z]\\)"
 
 date:
   pattern: "\\s?\\((?:\\d{8}|\\d{4}-\\d{2}-\\d{2}|\\d{2}-\\d{2}-\\d{4}|\\d{2}-\\d{2}-\\d{2}|\\d{4}-\\d{2}-\\d{2}T\\d{6}|~?\\d{4}-(?:\\d{2}|xx)-xx|(?:January|February|March|April|May|June|July|August|September|October|November|December),\\s?\\d{4})\\)"
   type: "str"
 
 alt:
   pattern: "\\(Alt.*?\\)"
@@ -191,14 +191,18 @@
   pattern: "\\((?:(?!\\(|Gentei.*?)[\\s\\S])*Gentei.*?\\)"
   group: "improved_version"
 
 ideatek:
   pattern: "\\(Idea-Tek\\)"
   group: "improved_version"
 
+infinity_plus:
+  pattern: "\\(Infinity Plus\\)"
+  group: "improved_version"
+
 later:
   pattern: "\\(Later\\)"
   group: "improved_version"
 
 mega_soft:
   pattern: "\\(Mega Soft\\)"
   group: "improved_version"
@@ -211,14 +215,18 @@
   pattern: "\\(NINA-06\\)"
   group: "improved_version"
 
 np:
   pattern: "\\(NP\\)"
   group: "improved_version"
 
+premium_pack:
+  pattern: "\\(Premium Pack\\)"
+  group: "improved_version"
+
 psone_books:
   pattern: "\\(PSone Books\\)"
   group: "improved_version"
 
 renkaban:
   pattern: "\\(Renkaban\\)"
   group: "improved_version"
@@ -231,28 +239,48 @@
   pattern: "\\(Subor Keyboard\\)"
   group: "improved_version"
 
 super_mega:
   pattern: "\\(Super Mega\\)"
   group: "improved_version"
 
+super_value_set:
+  pattern: "\\(Super Value Set\\)"
+  group: "improved_version"
+
+tatacon_doukon_set:
+  pattern: "\\(Tatacon Doukon Set\\)"
+  group: "improved_version"
+
+tokubetsu:
+  pattern: "\\((?:(?!\\(|Tokubetsu-ban.*?)[\\s\\S])*Tokubetsu-ban.*?\\)"
+  group: "improved_version"
+
 txc:
   pattern: "\\(TXC\\)"
   group: "improved_version"
 
+usb_mic_doukonban:
+  pattern: "\\(USB Mic Doukonban\\)"
+  group: "improved_version"
+
 # BUDGET EDITIONS
 
 artdink:
   pattern: "\\(Artdink Best Choice\\)"
   group: "budget_edition"
 
 best_of_the_best:
   pattern: "\\(Best of the Best\\)"
   group: "budget_edition"
 
+best_hit_selection:
+  pattern: "\\(Best Hit Selection\\)"
+  group: "budget_edition"
+
 best_wing:
   pattern: "\\(Best Wing 2800\\)"
   group: "budget_edition"
 
 bps_the_choice:
   pattern: "\\(BPS the Choice\\)"
   group: "budget_edition"
@@ -269,38 +297,69 @@
   pattern: "\\(Fukyuuban\\)"
   group: "budget_edition"
 
 fukyuuban_1500:
   pattern: "\\(Fukyuuban 1500\\)"
   group: "budget_edition"
 
+greatest_hits:
+  pattern: "\\(Greatest Hits\\)"
+  group: "budget_edition"
+
+gust_best_price:
+  pattern: "\\(Gust Best Price\\)"
+  group: "budget_edition"
+
 honkakuha:
   pattern: "\\(Honkakuha de 1300\\)"
   group: "budget_edition"
 
 koei_the_best:
   pattern: "\\(Koei the Best\\)"
   group: "budget_edition"
 
 major_wave:
   pattern: "\\(Major Wave\\)"
   group: "budget_edition"
 
+mega_hits:
+  pattern: "\\(Mega Hits!\\)"
+
 playstation_the_best:
   pattern: "\\(PlayStation the Best\\)"
   group: "budget_edition"
 
 playstation_the_best_for_family:
   pattern: "\\(PlayStation the Best for Family\\)"
   group: "budget_edition"
 
+playstation_2_the_best:
+  pattern: "\\(PlayStation 2 the Best\\)"
+  group: "budget_edition"
+
+rockstar_classics:
+  pattern: "\\(Rockstar Classics\\)"
+  group: "budget_edition"
+
 spike_library:
   pattern: "\\(Spike Library\\)"
   group: "budget_edition"
 
+spike_the_best:
+  pattern: "\\(Spike the Best\\)"
+  group: "budget_edition"
+
+super_value_2800:
+  pattern: "\\(Super Value 2800\\)"
+  group: "budget_edition"
+
+ultimate_hits:
+  pattern: "\\(Ultimate Hits\\)"
+  group: "budget_edition"
+
 value_1500:
   pattern: "\\(Value 1500\\)"
   group: "budget_edition"
 
 # MODERN VERSIONS
 
 3ds_virtual_console:
@@ -551,14 +610,17 @@
 
 72_pin_cart:
   pattern: "\\(72 pin cart\\)"
 
 strictly_limited:
   pattern: "\\(Strictly Limited Games\\)"
 
+multi_tap_doukoban:
+  pattern: "\\(Multi Tap.*?Doukonban\\)"
+
 ntdec:
   pattern: "\\(NTDEC\\)"
 
 ntsc:
   pattern: "([?:-][\\s])?[(]?NTSC\\)?"
   flags: "NOFLAG"
```

### Comparing `romsearch-0.0.2/romsearch/configs/sample_config.yml` & `romsearch-0.0.3/romsearch/configs/sample_config.yml`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/dev/parsing_tools.py` & `romsearch-0.0.3/romsearch/dev/parsing_tools.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/modules/datparser.py` & `romsearch-0.0.3/romsearch/modules/datparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/modules/dupeparser.py` & `romsearch-0.0.3/romsearch/modules/dupeparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/modules/gamefinder.py` & `romsearch-0.0.3/romsearch/modules/gamefinder.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/modules/romchooser.py` & `romsearch-0.0.3/romsearch/modules/romchooser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/modules/romdownloader.py` & `romsearch-0.0.3/romsearch/modules/romdownloader.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/modules/rommover.py` & `romsearch-0.0.3/romsearch/modules/rommover.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/modules/romparser.py` & `romsearch-0.0.3/romsearch/modules/romparser.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/modules/romsearch.py` & `romsearch-0.0.3/romsearch/modules/romsearch.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/util/__init__.py` & `romsearch-0.0.3/romsearch/util/__init__.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/util/general.py` & `romsearch-0.0.3/romsearch/util/general.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/util/io.py` & `romsearch-0.0.3/romsearch/util/io.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/util/logger.py` & `romsearch-0.0.3/romsearch/util/logger.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch/util/regex_matching.py` & `romsearch-0.0.3/romsearch/util/regex_matching.py`

 * *Files identical despite different names*

### Comparing `romsearch-0.0.2/romsearch.egg-info/PKG-INFO` & `romsearch-0.0.3/romsearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romsearch
-Version: 0.0.2
+Version: 0.0.3
 Summary: One Stop ROM Shop
 Author: bbtufty
 Maintainer: bbtufty
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -726,12 +726,14 @@
 
 To get started, see the [documentation](https://romsearch.readthedocs.io/en/latest/).
 
 Currently, ROMSearch is in early development, and so many features may be added over time. At the moment, ROMSearch
 works for the following consoles:
 
 * Nintendo - GameCube
+* Nintendo - Nintendo Entertainment System
 * Nintendo - Super Nintendo Entertainment System
 * Sony - PlayStation
+* Sony - PlayStation 2
 
 but be aware there may be quirks that will only become apparent over time. We encourage users to open
 [issues](https://github.com/bbtufty/romsearch/issues) as and where they find them.
```

### Comparing `romsearch-0.0.2/romsearch.egg-info/SOURCES.txt` & `romsearch-0.0.3/romsearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/rsstt-2.6.0.tar.gz` & `tmp/rsstt-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsstt-2.6.0.tar", last modified: Fri Mar 29 15:06:42 2024, max compression
+gzip compressed data, was "rsstt-2.7.0.tar", last modified: Thu May  9 17:11:02 2024, max compression
```

## Comparing `rsstt-2.6.0.tar` & `rsstt-2.7.0.tar`

### file list

```diff
@@ -1,108 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.732900 rsstt-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-29 15:06:39.000000 rsstt-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-03-29 15:06:42.732900 rsstt-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-03-29 15:06:39.000000 rsstt-2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-29 15:06:39.000000 rsstt-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-29 15:06:39.000000 rsstt-2.6.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.732900 rsstt-2.6.0/rsstt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-03-29 15:06:42.000000 rsstt-2.6.0/rsstt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-03-29 15:06:42.000000 rsstt-2.6.0/rsstt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:06:42.000000 rsstt-2.6.0/rsstt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:06:42.000000 rsstt-2.6.0/rsstt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-03-29 15:06:42.000000 rsstt-2.6.0/rsstt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-29 15:06:42.000000 rsstt-2.6.0/rsstt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-29 15:06:42.732900 rsstt-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-29 15:06:39.000000 rsstt-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.716900 rsstt-2.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/aio_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.720900 rsstt-2.6.0/src/command/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/administration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/customization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.720900 rsstt-2.6.0/src/command/inner/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/inner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19259 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/inner/customization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/inner/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/inner/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13815 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/opml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)    36740 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/command/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.720900 rsstt-2.6.0/src/db/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/effective_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.720900 rsstt-2.6.0/src/db/migrations_pgsql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_pgsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.724900 rsstt-2.6.0/src/db/migrations_pgsql/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_pgsql/models/0_20211117110249_init.sql
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_pgsql/models/1_20211130051128_update.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_pgsql/models/2_20220306045951_update.sql
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_pgsql/models/3_20220415030554_update.sql
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_pgsql/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.724900 rsstt-2.6.0/src/db/migrations_sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_sqlite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.724900 rsstt-2.6.0/src/db/migrations_sqlite/models/
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_sqlite/models/0_20211117110249_init.sql
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_sqlite/models/1_20211130051128_update.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_sqlite/models/2_20220306045951_update.sql
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_sqlite/models/3_20220415025716_update.sql
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/migrations_sqlite/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/db/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/errors_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.728900 rsstt-2.6.0/src/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/ar.json
--rw-r--r--   0 runner    (1001) docker     (127)    17459 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/ca.json
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/cs.json
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/de.json
--rw-r--r--   0 runner    (1001) docker     (127)    25208 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/el.json
--rw-r--r--   0 runner    (1001) docker     (127)    16033 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/en.json
--rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/es.json
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/eu.json
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/fa.json
--rw-r--r--   0 runner    (1001) docker     (127)    17902 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/he.json
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/id.json
--rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/it.json
--rw-r--r--   0 runner    (1001) docker     (127)    19374 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/ja.json
--rw-r--r--   0 runner    (1001) docker     (127)    14734 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/ko.json
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/pl.json
--rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/pt.json
--rw-r--r--   0 runner    (1001) docker     (127)    23490 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/si.json
--rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/tr.json
--rw-r--r--   0 runner    (1001) docker     (127)    23044 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/uk.json
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/uz.json
--rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/yue.json
--rw-r--r--   0 runner    (1001) docker     (127)    15032 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/zh-Hans.json
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/i18n/zh-Hant.json
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/opml_template.opml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.732900 rsstt-2.6.0/src/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/emojify.json
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/html_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    14017 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/html_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    42482 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/medium.py
--rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9212 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    26755 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/post_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/table_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/tgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    11609 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/parsing/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/redirect_server.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:06:42.732900 rsstt-2.6.0/src/web/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/web/feed.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/web/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/web/req.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-03-29 15:06:39.000000 rsstt-2.6.0/src/web/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.785357 rsstt-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-09 17:10:59.000000 rsstt-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-09 17:11:02.785357 rsstt-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-05-09 17:10:59.000000 rsstt-2.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 17:10:59.000000 rsstt-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-09 17:10:59.000000 rsstt-2.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.781357 rsstt-2.7.0/rsstt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-09 17:11:02.000000 rsstt-2.7.0/rsstt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-09 17:11:02.000000 rsstt-2.7.0/rsstt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:11:02.000000 rsstt-2.7.0/rsstt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:11:02.000000 rsstt-2.7.0/rsstt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-09 17:11:02.000000 rsstt-2.7.0/rsstt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 17:11:02.000000 rsstt-2.7.0/rsstt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-09 17:11:02.785357 rsstt-2.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      853 2024-05-09 17:10:59.000000 rsstt-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.769357 rsstt-2.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    18025 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/aio_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.769357 rsstt-2.7.0/src/command/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/administration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21102 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/customization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.769357 rsstt-2.7.0/src/command/inner/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/inner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20071 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/inner/customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14619 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/inner/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14718 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/inner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17956 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/opml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36740 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/command/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.773357 rsstt-2.7.0/src/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/effective_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.765357 rsstt-2.7.0/src/db/migrations_pgsql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.773357 rsstt-2.7.0/src/db/migrations_pgsql/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_pgsql/models/0_20211117110249_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_pgsql/models/1_20211130051128_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_pgsql/models/2_20220306045951_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_pgsql/models/3_20220415030554_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_pgsql/models/4_20240425020849_display_entry_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.765357 rsstt-2.7.0/src/db/migrations_sqlite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.773357 rsstt-2.7.0/src/db/migrations_sqlite/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_sqlite/models/0_20211117110249_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_sqlite/models/1_20211130051128_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_sqlite/models/2_20220306045951_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_sqlite/models/3_20220415025716_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/migrations_sqlite/models/4_20240425020849_display_entry_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13888 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/errors_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.781357 rsstt-2.7.0/src/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/ar.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17459 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/ca.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/cs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25208 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/el.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/eu.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23314 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/fa.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17902 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/he.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17645 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/it.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19374 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/ja.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14734 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/ko.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/pl.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17189 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/pt.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23490 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/si.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17371 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/tr.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23044 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/uk.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/uz.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15172 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/yue.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/zh-Hans.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15215 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/i18n/zh-Hant.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/opml_template.opml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.781357 rsstt-2.7.0/src/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/emojify.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/html_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14017 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/html_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42586 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/medium.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9694 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27452 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/post_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/table_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15359 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/tgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/parsing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/redirect_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:11:02.781357 rsstt-2.7.0/src/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/web/feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/web/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10275 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/web/req.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-09 17:10:59.000000 rsstt-2.7.0/src/web/utils.py
```

### Comparing `rsstt-2.6.0/LICENSE` & `rsstt-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/PKG-INFO` & `rsstt-2.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7273 7374  : 2.1.Name: rsst
-00000020: 740a 5665 7273 696f 6e3a 2032 2e36 2e30  t.Version: 2.6.0
+00000020: 740a 5665 7273 696f 6e3a 2032 2e37 2e30  t.Version: 2.7.0
 00000030: 0a53 756d 6d61 7279 3a20 4120 5465 6c65  .Summary: A Tele
 00000040: 6772 616d 2052 5353 2062 6f74 2074 6861  gram RSS bot tha
 00000050: 7420 6361 7265 7320 6162 6f75 7420 796f  t cares about yo
 00000060: 7572 2072 6561 6469 6e67 2065 7870 6572  ur reading exper
 00000070: 6965 6e63 650a 486f 6d65 2d70 6167 653a  ience.Home-page:
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 526f 6e67 726f 6e67 6767 392f  com/Rongronggg9/
@@ -79,578 +79,610 @@
 000004e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
 000004f0: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
 00000500: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 00000510: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
 00000520: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
 00000530: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
 00000540: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000550: 3a3a 2049 6d70 6c65 6d65 6e74 6174 696f  :: Implementatio
-00000560: 6e20 3a3a 2043 5079 7468 6f6e 0a43 6c61  n :: CPython.Cla
-00000570: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000580: 3a20 436f 6d6d 756e 6963 6174 696f 6e73  : Communications
-00000590: 203a 3a20 4368 6174 0a43 6c61 7373 6966   :: Chat.Classif
-000005a0: 6965 723a 2054 6f70 6963 203a 3a20 496e  ier: Topic :: In
-000005b0: 7465 726e 6574 0a43 6c61 7373 6966 6965  ternet.Classifie
-000005c0: 723a 2054 6f70 6963 203a 3a20 4d75 6c74  r: Topic :: Mult
-000005d0: 696d 6564 6961 0a52 6571 7569 7265 732d  imedia.Requires-
-000005e0: 5079 7468 6f6e 3a20 3e3d 332e 390a 4465  Python: >=3.9.De
-000005f0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000600: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000610: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
-00000620: 6c65 3a20 4c49 4345 4e53 450a 5265 7175  le: LICENSE.Requ
-00000630: 6972 6573 2d44 6973 743a 2063 7279 7074  ires-Dist: crypt
-00000640: 673d 3d30 2e34 2e30 0a52 6571 7569 7265  g==0.4.0.Require
-00000650: 732d 4469 7374 3a20 7465 6c65 7468 6f6e  s-Dist: telethon
-00000660: 3d3d 312e 3334 2e30 0a52 6571 7569 7265  ==1.34.0.Require
-00000670: 732d 4469 7374 3a20 6169 6f67 7261 7068  s-Dist: aiograph
-00000680: 6669 783d 3d30 2e32 2e32 0a52 6571 7569  fix==0.2.2.Requi
-00000690: 7265 732d 4469 7374 3a20 6665 6564 7061  res-Dist: feedpa
-000006a0: 7273 6572 3d3d 362e 302e 3131 0a52 6571  rser==6.0.11.Req
-000006b0: 7569 7265 732d 4469 7374 3a20 6c69 7374  uires-Dist: list
-000006c0: 7061 7273 6572 5b6c 786d 6c5d 3d3d 302e  parser[lxml]==0.
-000006d0: 3139 0a52 6571 7569 7265 732d 4469 7374  19.Requires-Dist
-000006e0: 3a20 7069 6c6c 6f77 3d3d 3130 2e32 2e30  : pillow==10.2.0
-000006f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000700: 6265 6175 7469 6675 6c73 6f75 7034 3d3d  beautifulsoup4==
-00000710: 342e 3132 2e33 0a52 6571 7569 7265 732d  4.12.3.Requires-
-00000720: 4469 7374 3a20 6c78 6d6c 3d3d 342e 392e  Dist: lxml==4.9.
-00000730: 330a 5265 7175 6972 6573 2d44 6973 743a  3.Requires-Dist:
-00000740: 2072 6170 6964 6675 7a7a 3d3d 332e 372e   rapidfuzz==3.7.
-00000750: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-00000760: 2065 6d6f 6a69 3d3d 322e 3131 2e30 0a52   emoji==2.11.0.R
-00000770: 6571 7569 7265 732d 4469 7374 3a20 6d69  equires-Dist: mi
-00000780: 6e69 6679 2d68 746d 6c3d 3d30 2e31 352e  nify-html==0.15.
-00000790: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-000007a0: 206d 696e 6966 792d 6874 6d6c 2d6f 6e65   minify-html-one
-000007b0: 7061 7373 3d3d 302e 3135 2e30 0a52 6571  pass==0.15.0.Req
-000007c0: 7569 7265 732d 4469 7374 3a20 6d61 7470  uires-Dist: matp
-000007d0: 6c6f 746c 6962 3d3d 332e 382e 330a 5265  lotlib==3.8.3.Re
-000007e0: 7175 6972 6573 2d44 6973 743a 2061 7379  quires-Dist: asy
-000007f0: 6e63 7067 3d3d 302e 3239 2e30 0a52 6571  ncpg==0.29.0.Req
-00000800: 7569 7265 732d 4469 7374 3a20 746f 7274  uires-Dist: tort
-00000810: 6f69 7365 2d6f 726d 5b61 6363 656c 5d3d  oise-orm[accel]=
-00000820: 3d30 2e32 302e 300a 5265 7175 6972 6573  =0.20.0.Requires
-00000830: 2d44 6973 743a 2061 6572 6963 683d 3d30  -Dist: aerich==0
-00000840: 2e36 2e33 0a52 6571 7569 7265 732d 4469  .6.3.Requires-Di
-00000850: 7374 3a20 6169 6f68 7474 705b 7370 6565  st: aiohttp[spee
-00000860: 6475 7073 5d3d 3d33 2e39 2e33 0a52 6571  dups]==3.9.3.Req
-00000870: 7569 7265 732d 4469 7374 3a20 6169 6f68  uires-Dist: aioh
-00000880: 7474 702d 736f 636b 733d 3d30 2e38 2e34  ttp-socks==0.8.4
-00000890: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000008a0: 6169 6f68 7474 702d 7265 7472 793d 3d32  aiohttp-retry==2
-000008b0: 2e38 2e33 0a52 6571 7569 7265 732d 4469  .8.3.Requires-Di
-000008c0: 7374 3a20 7079 7468 6f6e 2d73 6f63 6b73  st: python-socks
-000008d0: 5b61 7379 6e63 696f 5d3d 3d32 2e34 2e34  [asyncio]==2.4.4
-000008e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000008f0: 646e 7370 7974 686f 6e5b 6964 6e61 5d3d  dnspython[idna]=
-00000900: 3d32 2e36 2e31 0a52 6571 7569 7265 732d  =2.6.1.Requires-
-00000910: 4469 7374 3a20 636f 6c6f 726c 6f67 3d3d  Dist: colorlog==
-00000920: 362e 382e 320a 5265 7175 6972 6573 2d44  6.8.2.Requires-D
-00000930: 6973 743a 2041 5053 6368 6564 756c 6572  ist: APScheduler
-00000940: 3d3d 332e 3130 2e34 0a52 6571 7569 7265  ==3.10.4.Require
-00000950: 732d 4469 7374 3a20 7079 7468 6f6e 2d64  s-Dist: python-d
-00000960: 6f74 656e 763d 3d31 2e30 2e31 0a52 6571  otenv==1.0.1.Req
-00000970: 7569 7265 732d 4469 7374 3a20 6d75 6c74  uires-Dist: mult
-00000980: 6964 6963 743d 3d36 2e30 2e35 0a52 6571  idict==6.0.5.Req
-00000990: 7569 7265 732d 4469 7374 3a20 6173 796e  uires-Dist: asyn
-000009a0: 6373 7464 6c69 623d 3d33 2e31 322e 320a  cstdlib==3.12.2.
-000009b0: 5265 7175 6972 6573 2d44 6973 743a 2063  Requires-Dist: c
-000009c0: 6163 6865 746f 6f6c 733d 3d35 2e33 2e33  achetools==5.3.3
-000009d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000009e0: 434a 4b77 7261 703d 3d32 2e32 0a52 6571  CJKwrap==2.2.Req
-000009f0: 7569 7265 732d 4469 7374 3a20 7479 7069  uires-Dist: typi
-00000a00: 6e67 2d65 7874 656e 7369 6f6e 733d 3d34  ng-extensions==4
-00000a10: 2e31 302e 300a 5265 7175 6972 6573 2d44  .10.0.Requires-D
-00000a20: 6973 743a 2075 766c 6f6f 703d 3d30 2e31  ist: uvloop==0.1
-00000a30: 392e 303b 2073 7973 5f70 6c61 7466 6f72  9.0; sys_platfor
-00000a40: 6d20 213d 2022 7769 6e33 3222 2061 6e64  m != "win32" and
-00000a50: 2073 7973 5f70 6c61 7466 6f72 6d20 213d   sys_platform !=
-00000a60: 2022 6379 6777 696e 2220 616e 6420 7379   "cygwin" and sy
-00000a70: 735f 706c 6174 666f 726d 2021 3d20 2263  s_platform != "c
-00000a80: 6c69 220a 5265 7175 6972 6573 2d44 6973  li".Requires-Dis
-00000a90: 743a 2069 7361 6c3d 3d31 2e36 2e31 3b20  t: isal==1.6.1; 
-00000aa0: 706c 6174 666f 726d 5f6d 6163 6869 6e65  platform_machine
-00000ab0: 203d 3d20 2278 3836 5f36 3422 206f 7220   == "x86_64" or 
-00000ac0: 706c 6174 666f 726d 5f6d 6163 6869 6e65  platform_machine
-00000ad0: 203d 3d20 2241 4d44 3634 2220 6f72 2070   == "AMD64" or p
-00000ae0: 6c61 7466 6f72 6d5f 6d61 6368 696e 6520  latform_machine 
-00000af0: 3d3d 2022 6161 7263 6836 3422 0a0a 3c61  == "aarch64"..<a
-00000b00: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
-00000b10: 2e6d 652f 5253 5374 545f 426f 7422 3e3c  .me/RSStT_Bot"><
-00000b20: 696d 6720 7769 6474 683d 2231 3530 2220  img width="150" 
-00000b30: 6865 6967 6874 3d22 3135 3022 2061 6c69  height="150" ali
-00000b40: 676e 3d22 6c65 6674 2220 7374 796c 653d  gn="left" style=
-00000b50: 2266 6c6f 6174 3a20 6c65 6674 3b20 6d61  "float: left; ma
-00000b60: 7267 696e 3a20 3020 3130 7078 2030 2030  rgin: 0 10px 0 0
-00000b70: 3b22 2061 6c74 3d22 5253 5374 5420 6963  ;" alt="RSStT ic
-00000b80: 6f6e 2220 7372 633d 2264 6f63 732f 7265  on" src="docs/re
-00000b90: 736f 7572 6365 732f 5253 5374 545f 6963  sources/RSStT_ic
-00000ba0: 6f6e 2e73 7667 222f 3e3c 612f 3e0a 0a23  on.svg"/><a/>..#
-00000bb0: 205b 5253 5320 746f 2054 656c 6567 7261   [RSS to Telegra
-00000bc0: 6d20 426f 745d 2868 7474 7073 3a2f 2f74  m Bot](https://t
-00000bd0: 2e6d 652f 5253 5374 545f 426f 7429 0a0a  .me/RSStT_Bot)..
-00000be0: 2a2a 4120 5465 6c65 6772 616d 2052 5353  **A Telegram RSS
-00000bf0: 2062 6f74 2074 6861 7420 6361 7265 7320   bot that cares 
-00000c00: 6162 6f75 7420 796f 7572 2072 6561 6469  about your readi
-00000c10: 6e67 2065 7870 6572 6965 6e63 652a 2a0a  ng experience**.
-00000c20: 0a5b e7ae 80e4 bd93 e4b8 ade6 9687 2052  .[............ R
-00000c30: 4541 444d 455d 2852 4541 444d 452e 7a68  EADME](README.zh
-00000c40: 2e6d 6429 0a0a 5b21 5b47 6974 4875 6220  .md)..[![GitHub 
-00000c50: 636f 6d6d 6974 2061 6374 6976 6974 795d  commit activity]
-00000c60: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000c70: 656c 6473 2e69 6f2f 6769 7468 7562 2f63  elds.io/github/c
-00000c80: 6f6d 6d69 742d 6163 7469 7669 7479 2f6d  ommit-activity/m
-00000c90: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
-00000ca0: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
-00000cb0: 3f6c 6f67 6f3d 6769 7426 6c61 6265 6c3d  ?logo=git&label=
-00000cc0: 636f 6d6d 6974 295d 2868 7474 7073 3a2f  commit)](https:/
-00000cd0: 2f67 6974 6875 622e 636f 6d2f 526f 6e67  /github.com/Rong
-00000ce0: 726f 6e67 6767 392f 5253 532d 746f 2d54  ronggg9/RSS-to-T
-00000cf0: 656c 6567 7261 6d2d 426f 742f 636f 6d6d  elegram-Bot/comm
-00000d00: 6974 7329 0a5b 215b 5472 616e 736c 6174  its).[![Translat
-00000d10: 696e 6720 7374 6174 7573 5d28 6874 7470  ing status](http
-00000d20: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000d30: 696f 2f77 6562 6c61 7465 2f70 726f 6772  io/weblate/progr
-00000d40: 6573 732f 7273 732d 746f 2d74 656c 6567  ess/rss-to-teleg
-00000d50: 7261 6d2d 626f 743f 6c6f 676f 3d77 6562  ram-bot?logo=web
-00000d60: 6c61 7465 2663 6f6c 6f72 3d69 6e66 6f72  late&color=infor
-00000d70: 6d61 7469 6f6e 616c 295d 2868 7474 7073  mational)](https
-00000d80: 3a2f 2f68 6f73 7465 642e 7765 626c 6174  ://hosted.weblat
-00000d90: 652e 6f72 672f 656e 6761 6765 2f72 7373  e.org/engage/rss
-00000da0: 2d74 6f2d 7465 6c65 6772 616d 2d62 6f74  -to-telegram-bot
-00000db0: 2f29 0a5b 215b 436f 6465 2071 7561 6c69  /).[![Code quali
-00000dc0: 7479 5d28 6874 7470 733a 2f2f 696d 672e  ty](https://img.
-00000dd0: 7368 6965 6c64 732e 696f 2f63 6f64 6566  shields.io/codef
-00000de0: 6163 746f 722f 6772 6164 652f 6769 7468  actor/grade/gith
-00000df0: 7562 2f52 6f6e 6772 6f6e 6767 6739 2f52  ub/Rongronggg9/R
-00000e00: 5353 2d74 6f2d 5465 6c65 6772 616d 2d42  SS-to-Telegram-B
-00000e10: 6f74 3f6c 6f67 6f3d 636f 6465 6661 6374  ot?logo=codefact
-00000e20: 6f72 295d 2868 7474 7073 3a2f 2f77 7777  or)](https://www
-00000e30: 2e63 6f64 6566 6163 746f 722e 696f 2f72  .codefactor.io/r
-00000e40: 6570 6f73 6974 6f72 792f 6769 7468 7562  epository/github
-00000e50: 2f72 6f6e 6772 6f6e 6767 6739 2f72 7373  /rongronggg9/rss
-00000e60: 2d74 6f2d 7465 6c65 6772 616d 2d62 6f74  -to-telegram-bot
-00000e70: 290a 5b21 5b47 6974 4875 6220 7374 6172  ).[![GitHub star
-00000e80: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
-00000e90: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000ea0: 2f73 7461 7273 2f52 6f6e 6772 6f6e 6767  /stars/Rongrongg
-00000eb0: 6739 2f52 7373 2d74 6f2d 5465 6c65 6772  g9/Rss-to-Telegr
-00000ec0: 616d 2d42 6f74 3f73 7479 6c65 3d73 6f63  am-Bot?style=soc
-00000ed0: 6961 6c29 5d28 6874 7470 733a 2f2f 6769  ial)](https://gi
-00000ee0: 7468 7562 2e63 6f6d 2f52 6f6e 6772 6f6e  thub.com/Rongron
-00000ef0: 6767 6739 2f52 5353 2d74 6f2d 5465 6c65  ggg9/RSS-to-Tele
-00000f00: 6772 616d 2d42 6f74 2f73 7461 7267 617a  gram-Bot/stargaz
-00000f10: 6572 7329 0a5b 215b 4769 7448 7562 2066  ers).[![GitHub f
-00000f20: 6f72 6b73 5d28 6874 7470 733a 2f2f 696d  orks](https://im
-00000f30: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00000f40: 6875 622f 666f 726b 732f 526f 6e67 726f  hub/forks/Rongro
-00000f50: 6e67 6767 392f 5253 532d 746f 2d54 656c  nggg9/RSS-to-Tel
-00000f60: 6567 7261 6d2d 426f 743f 7374 796c 653d  egram-Bot?style=
-00000f70: 736f 6369 616c 295d 2868 7474 7073 3a2f  social)](https:/
-00000f80: 2f67 6974 6875 622e 636f 6d2f 526f 6e67  /github.com/Rong
-00000f90: 726f 6e67 6767 392f 5253 532d 746f 2d54  ronggg9/RSS-to-T
-00000fa0: 656c 6567 7261 6d2d 426f 742f 666f 726b  elegram-Bot/fork
-00000fb0: 290a 0a5b 215b 5465 6c65 6772 616d 2062  )..[![Telegram b
-00000fc0: 6f74 5d28 6874 7470 733a 2f2f 696d 672e  ot](https://img.
-00000fd0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000fe0: 2f62 6f74 2d25 3430 5253 5374 545f 5f42  /bot-%40RSStT__B
-00000ff0: 6f74 2d32 3239 6564 393f 6c6f 676f 3d74  ot-229ed9?logo=t
-00001000: 656c 6567 7261 6d26 7374 796c 653d 666f  elegram&style=fo
-00001010: 722d 7468 652d 6261 6467 6529 5d28 6874  r-the-badge)](ht
-00001020: 7470 733a 2f2f 742e 6d65 2f52 5353 7454  tps://t.me/RSStT
-00001030: 5f42 6f74 290a 5b21 5b54 656c 6567 7261  _Bot).[![Telegra
-00001040: 6d20 6772 6f75 705d 2868 7474 7073 3a2f  m group](https:/
-00001050: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001060: 6261 6467 652f 6368 6174 2d25 3430 5253  badge/chat-%40RS
-00001070: 5374 545f 5f47 726f 7570 2d32 3239 6564  StT__Group-229ed
-00001080: 393f 6c6f 676f 3d74 656c 6567 7261 6d26  9?logo=telegram&
-00001090: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-000010a0: 6467 6529 5d28 6874 7470 733a 2f2f 742e  dge)](https://t.
-000010b0: 6d65 2f52 5353 7454 5f47 726f 7570 290a  me/RSStT_Group).
-000010c0: 5b21 5b54 656c 6567 7261 6d20 6368 616e  [![Telegram chan
-000010d0: 6e65 6c5d 2868 7474 7073 3a2f 2f69 6d67  nel](https://img
-000010e0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000010f0: 652f 6368 616e 6e65 6c2d 2534 3052 5353  e/channel-%40RSS
-00001100: 7454 5f5f 4368 616e 6e65 6c2d 3232 3965  tT__Channel-229e
-00001110: 6439 3f6c 6f67 6f3d 7465 6c65 6772 616d  d9?logo=telegram
-00001120: 2673 7479 6c65 3d66 6f72 2d74 6865 2d62  &style=for-the-b
-00001130: 6164 6765 295d 2868 7474 7073 3a2f 2f74  adge)](https://t
-00001140: 2e6d 652f 5253 5374 545f 4368 616e 6e65  .me/RSStT_Channe
-00001150: 6c29 0a0a 7c20 5b43 4841 4e47 454c 4f47  l)..| [CHANGELOG
-00001160: 5d20 7c20 5b46 4151 5d20 7c20 5b44 6f63  ] | [FAQ] | [Doc
-00001170: 756d 656e 7461 7469 6f6e 5d20 7c20 5b43  umentation] | [C
-00001180: 6861 6e6e 656c 7320 5573 696e 6720 5253  hannels Using RS
-00001190: 5374 545d 207c 0a7c 3a2d 2d2d 2d2d 2d2d  StT] |.|:-------
-000011a0: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 3a7c 2d2d  ----:|:-----:|--
-000011b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-000011c0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-000011d0: 2d2d 2d2d 2d2d 2d3a 7c0a 0a5b 4348 414e  -------:|..[CHAN
-000011e0: 4745 4c4f 475d 3a20 646f 6373 2f43 4841  GELOG]: docs/CHA
-000011f0: 4e47 454c 4f47 2e6d 640a 0a5b 4641 515d  NGELOG.md..[FAQ]
-00001200: 3a20 646f 6373 2f46 4151 2e6d 640a 0a5b  : docs/FAQ.md..[
-00001210: 446f 6375 6d65 6e74 6174 696f 6e5d 3a20  Documentation]: 
-00001220: 646f 6373 0a0a 5b43 6861 6e6e 656c 7320  docs..[Channels 
-00001230: 5573 696e 6720 5253 5374 545d 3a20 646f  Using RSStT]: do
-00001240: 6373 2f63 6861 6e6e 656c 732d 7573 696e  cs/channels-usin
-00001250: 672d 7273 7374 742e 6d64 0a0a 0a2a 2a49  g-rsstt.md...**I
-00001260: 6d70 6f72 7461 6e74 2a2a 3a20 4966 2079  mportant**: If y
-00001270: 6f75 2068 6176 6520 796f 7572 206f 776e  ou have your own
-00001280: 2052 5353 7454 2062 6f74 2028 7631 292c   RSStT bot (v1),
-00001290: 2070 6c65 6173 6520 7265 6164 2074 6865   please read the
-000012a0: 205b 6d69 6772 6174 696f 6e20 6775 6964   [migration guid
-000012b0: 655d 2864 6f63 732f 6d69 6772 6174 696f  e](docs/migratio
-000012c0: 6e2d 6775 6964 652d 7632 2e6d 6429 2074  n-guide-v2.md) t
-000012d0: 6f20 6c65 6172 6e20 686f 7720 746f 206d  o learn how to m
-000012e0: 6967 7261 7465 2074 6f20 7632 2e0a 0a23  igrate to v2...#
-000012f0: 2320 4869 6768 6c69 6768 7473 0a0a 2d20  # Highlights..- 
-00001300: 4d75 6c74 692d 7573 6572 0a2d 2049 3138  Multi-user.- I18
-00001310: 6e0a 2020 2020 2d20 456e 676c 6973 682c  n.    - English,
-00001320: 2043 6869 6e65 7365 2c20 4361 6e74 6f6e   Chinese, Canton
-00001330: 6573 652c 2049 7461 6c69 616e 2c20 616e  ese, Italian, an
-00001340: 6420 5b6d 6f72 655d 2864 6f63 732f 7472  d [more](docs/tr
-00001350: 616e 736c 6174 696f 6e2d 6775 6964 652e  anslation-guide.
-00001360: 6d64 2921 0a2d 2054 6865 2063 6f6e 7465  md)!.- The conte
-00001370: 6e74 206f 6620 7468 6520 706f 7374 7320  nt of the posts 
-00001380: 6f66 2061 6e20 5253 5320 6665 6564 2077  of an RSS feed w
-00001390: 696c 6c20 6265 2073 656e 7420 746f 2054  ill be sent to T
-000013a0: 656c 6567 7261 6d0a 2020 2020 2d20 4b65  elegram.    - Ke
-000013b0: 6570 2072 6963 682d 7465 7874 2066 6f72  ep rich-text for
-000013c0: 6d61 740a 2020 2020 2d20 4b65 6570 206d  mat.    - Keep m
-000013d0: 6564 6961 2028 6375 7374 6f6d 697a 6162  edia (customizab
-000013e0: 6c65 290a 2020 2020 2020 2020 2d20 496d  le).        - Im
-000013f0: 6167 6573 2c20 5669 6465 6f73 2c20 616e  ages, Videos, an
-00001400: 6420 4175 6469 6f20 626f 7468 2069 6e20  d Audio both in 
-00001410: 7468 6520 706f 7374 2063 6f6e 7465 6e74  the post content
-00001420: 2061 6e64 2065 6e63 6c6f 7375 7265 3b20   and enclosure; 
-00001430: 446f 6375 6d65 6e74 7320 696e 2074 6865  Documents in the
-00001440: 2070 6f73 7420 656e 636c 6f73 7572 650a   post enclosure.
-00001450: 2020 2020 2020 2020 2d20 4c6f 6e67 2069          - Long i
-00001460: 6d61 6765 7320 7769 6c6c 2062 6520 7365  mages will be se
-00001470: 6e74 2061 7320 6669 6c65 7320 746f 2070  nt as files to p
-00001480: 7265 7665 6e74 2054 656c 6567 7261 6d20  revent Telegram 
-00001490: 6672 6f6d 2063 6f6d 7072 6573 7369 6e67  from compressing
-000014a0: 2074 6865 2069 6d61 6765 2061 6e64 206d   the image and m
-000014b0: 616b 696e 6720 6974 2075 6e72 6561 6461  aking it unreada
-000014c0: 626c 650a 2020 2020 2020 2020 2d20 4472  ble.        - Dr
-000014d0: 6f70 2061 6e6e 6f79 696e 6720 6963 6f6e  op annoying icon
-000014e0: 732c 2074 6865 7920 6272 6561 6b20 7468  s, they break th
-000014f0: 6520 7265 6164 696e 6720 6578 7065 7269  e reading experi
-00001500: 656e 6365 0a20 2020 202d 2041 7574 6f6d  ence.    - Autom
-00001510: 6174 6963 616c 6c79 2072 6570 6c61 6365  atically replace
-00001520: 2065 6d6f 6a69 2073 686f 7274 636f 6465   emoji shortcode
-00001530: 7320 7769 7468 2065 6d6f 6a69 0a20 2020  s with emoji.   
-00001540: 202d 2041 7574 6f6d 6174 6963 616c 6c79   - Automatically
-00001550: 2072 6570 6c61 6365 2065 6d6f 6a69 2069   replace emoji i
-00001560: 6d61 6765 7320 7769 7468 2065 6d6f 6a69  mages with emoji
-00001570: 206f 7220 6974 7320 6465 7363 7269 7074   or its descript
-00001580: 696f 6e20 7465 7874 0a20 2020 202d 2041  ion text.    - A
-00001590: 7574 6f6d 6174 6963 616c 6c79 2064 6574  utomatically det
-000015a0: 6572 6d69 6e65 2077 6865 7468 6572 2074  ermine whether t
-000015b0: 6865 2074 6974 6c65 206f 6620 7468 6520  he title of the 
-000015c0: 5253 5320 6665 6564 2069 7320 6175 746f  RSS feed is auto
-000015d0: 2d66 696c 6c65 642c 2069 6620 736f 2c20  -filled, if so, 
-000015e0: 6f6d 6974 2074 6865 2074 6974 6c65 2028  omit the title (
-000015f0: 6375 7374 6f6d 697a 6162 6c65 290a 2020  customizable).  
-00001600: 2020 2d20 4175 746f 6d61 7469 6361 6c6c    - Automaticall
-00001610: 7920 7368 6f77 2074 6865 2061 7574 686f  y show the autho
-00001620: 722d 6e61 6d65 2028 6375 7374 6f6d 697a  r-name (customiz
-00001630: 6162 6c65 290a 2020 2020 2d20 4175 746f  able).    - Auto
-00001640: 6d61 7469 6361 6c6c 7920 7370 6c69 7420  matically split 
-00001650: 746f 6f2d 6c6f 6e67 206d 6573 7361 6765  too-long message
-00001660: 730a 2020 2020 2020 2020 2d20 4966 2063  s.        - If c
-00001670: 6f6e 6669 6775 7265 6420 5465 6c65 6772  onfigured Telegr
-00001680: 6170 682c 2074 6865 206d 6573 7361 6765  aph, the message
-00001690: 2077 696c 6c20 6265 2073 656e 7420 7669   will be sent vi
-000016a0: 6120 5465 6c65 6772 6170 6820 2863 7573  a Telegraph (cus
-000016b0: 746f 6d69 7a61 626c 6529 0a2d 205b 5661  tomizable).- [Va
-000016c0: 7269 6f75 7320 6375 7374 6f6d 697a 6162  rious customizab
-000016d0: 6c65 2066 6f72 6d61 7474 696e 6720 7365  le formatting se
-000016e0: 7474 696e 6773 5d28 646f 6373 2f66 6f72  ttings](docs/for
-000016f0: 6d61 7474 696e 672d 7365 7474 696e 6773  matting-settings
-00001700: 2e6d 6429 0a20 2020 202d 2048 6173 6874  .md).    - Hasht
-00001710: 6167 732c 2063 7573 746f 6d20 7469 746c  ags, custom titl
-00001720: 652c 2065 7463 2e0a 2d20 496e 6469 7669  e, etc..- Indivi
-00001730: 6475 616c 2070 726f 7879 2073 6574 7469  dual proxy setti
-00001740: 6e67 7320 666f 7220 5465 6c65 6772 616d  ngs for Telegram
-00001750: 2061 6e64 2052 5353 2066 6565 6473 0a2d   and RSS feeds.-
-00001760: 204f 504d 4c20 696d 706f 7274 696e 6720   OPML importing 
-00001770: 616e 6420 6578 706f 7274 696e 6720 286b  and exporting (k
-00001780: 6565 7020 6375 7374 6f6d 2074 6974 6c65  eep custom title
-00001790: 290a 2d20 4f70 7469 6d69 7a65 6420 7065  ).- Optimized pe
-000017a0: 7266 6f72 6d61 6e63 6520 2873 6565 2061  rformance (see a
-000017b0: 6c73 6f20 7468 6520 5b46 4151 5d28 646f  lso the [FAQ](do
-000017c0: 6373 2f46 4151 2e6d 6423 712d 686f 772d  cs/FAQ.md#q-how-
-000017d0: 6973 2d74 6865 2d70 6572 666f 726d 616e  is-the-performan
-000017e0: 6365 2d6f 662d 7468 652d 626f 7429 290a  ce-of-the-bot)).
-000017f0: 2d20 5573 6572 2d66 7269 656e 646c 790a  - User-friendly.
-00001800: 2d20 4854 5450 2043 6163 6869 6e67 0a0a  - HTTP Caching..
-00001810: 3c69 6d67 2073 7263 3d22 646f 6373 2f72  <img src="docs/r
-00001820: 6573 6f75 7263 6573 2f65 7861 6d70 6c65  esources/example
-00001830: 312e 706e 6722 2077 6964 7468 203d 2022  1.png" width = "
-00001840: 3330 3022 2061 6c74 3d22 222f 3e3c 696d  300" alt=""/><im
-00001850: 6720 7372 633d 2264 6f63 732f 7265 736f  g src="docs/reso
-00001860: 7572 6365 732f 6578 616d 706c 6533 2e70  urces/example3.p
-00001870: 6e67 2220 7769 6474 6820 3d20 2233 3030  ng" width = "300
-00001880: 2220 616c 743d 2222 2f3e 3c69 6d67 2073  " alt=""/><img s
-00001890: 7263 3d22 646f 6373 2f72 6573 6f75 7263  rc="docs/resourc
-000018a0: 6573 2f65 7861 6d70 6c65 342e 706e 6722  es/example4.png"
-000018b0: 2077 6964 7468 203d 2022 3330 3022 2061   width = "300" a
-000018c0: 6c74 3d22 222f 3e0a 0a23 2320 4465 706c  lt=""/>..## Depl
-000018d0: 6f79 6d65 6e74 0a0a 5b21 5b50 7950 495d  oyment..[![PyPI]
-000018e0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000018f0: 656c 6473 2e69 6f2f 7079 7069 2f76 2f72  elds.io/pypi/v/r
-00001900: 7373 7474 3f6c 6f67 6f3d 7079 7069 266c  sstt?logo=pypi&l
-00001910: 6f67 6f43 6f6c 6f72 3d77 6869 7465 295d  ogoColor=white)]
-00001920: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00001930: 672f 7072 6f6a 6563 742f 7273 7374 742f  g/project/rsstt/
-00001940: 290a 5b21 5b50 7950 4920 7075 626c 6973  ).[![PyPI publis
-00001950: 6820 7374 6174 7573 5d28 6874 7470 733a  h status](https:
-00001960: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00001970: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
-00001980: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
-00001990: 526f 6e67 726f 6e67 6767 392f 5253 532d  Rongronggg9/RSS-
-000019a0: 746f 2d54 656c 6567 7261 6d2d 426f 742f  to-Telegram-Bot/
-000019b0: 7075 626c 6973 682d 746f 2d70 7970 692e  publish-to-pypi.
-000019c0: 796d 6c3f 6c61 6265 6c3d 7075 626c 6973  yml?label=publis
-000019d0: 6826 6c6f 676f 3d70 7970 6926 6c6f 676f  h&logo=pypi&logo
-000019e0: 436f 6c6f 723d 7768 6974 6529 5d28 6874  Color=white)](ht
-000019f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001a00: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
-00001a10: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
-00001a20: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00001a30: 7773 2f70 7562 6c69 7368 2d74 6f2d 7079  ws/publish-to-py
-00001a40: 7069 2e79 6d6c 290a 5b21 5b54 6573 7450  pi.yml).[![TestP
-00001a50: 7950 4920 7075 626c 6973 6820 7374 6174  yPI publish stat
-00001a60: 7573 5d28 6874 7470 733a 2f2f 696d 672e  us](https://img.
-00001a70: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00001a80: 622f 6163 7469 6f6e 732f 776f 726b 666c  b/actions/workfl
-00001a90: 6f77 2f73 7461 7475 732f 526f 6e67 726f  ow/status/Rongro
-00001aa0: 6e67 6767 392f 5253 532d 746f 2d54 656c  nggg9/RSS-to-Tel
-00001ab0: 6567 7261 6d2d 426f 742f 7075 626c 6973  egram-Bot/publis
-00001ac0: 682d 746f 2d74 6573 742d 7079 7069 2e79  h-to-test-pypi.y
-00001ad0: 6d6c 3f6c 6162 656c 3d70 7562 6c69 7368  ml?label=publish
-00001ae0: 2532 3028 5465 7374 5079 5049 2926 6c6f  %20(TestPyPI)&lo
-00001af0: 676f 3d70 7970 6926 6c6f 676f 436f 6c6f  go=pypi&logoColo
-00001b00: 723d 7768 6974 6529 5d28 6874 7470 733a  r=white)](https:
-00001b10: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6f6e  //github.com/Ron
-00001b20: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
-00001b30: 5465 6c65 6772 616d 2d42 6f74 2f61 6374  Telegram-Bot/act
-00001b40: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00001b50: 7562 6c69 7368 2d74 6f2d 7079 7069 2e79  ublish-to-pypi.y
-00001b60: 6d6c 290a 5b21 5b50 7950 4920 2d20 446f  ml).[![PyPI - Do
-00001b70: 776e 6c6f 6164 735d 2868 7474 7073 3a2f  wnloads](https:/
-00001b80: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001b90: 7079 7069 2f64 6d2f 7273 7374 743f 6c6f  pypi/dm/rsstt?lo
-00001ba0: 676f 3d70 7970 6926 6c6f 676f 436f 6c6f  go=pypi&logoColo
-00001bb0: 723d 7768 6974 6529 5d28 6874 7470 733a  r=white)](https:
-00001bc0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00001bd0: 6374 2f72 7373 7474 2f29 0a5b 215b 5079  ct/rsstt/).[![Py
-00001be0: 5049 202d 2050 7974 686f 6e20 5665 7273  PI - Python Vers
-00001bf0: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-00001c00: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00001c10: 2f70 7976 6572 7369 6f6e 732f 7273 7374  /pyversions/rsst
-00001c20: 743f 6c6f 676f 3d70 7974 686f 6e26 6c61  t?logo=python&la
-00001c30: 6265 6c3d 266c 6162 656c 436f 6c6f 723d  bel=&labelColor=
-00001c40: 7768 6974 6529 5d28 6874 7470 733a 2f2f  white)](https://
-00001c50: 7777 772e 7079 7468 6f6e 2e6f 7267 290a  www.python.org).
-00001c60: 0a5b 215b 446f 636b 6572 2049 6d61 6765  .[![Docker Image
-00001c70: 2053 697a 6520 2874 6167 295d 2868 7474   Size (tag)](htt
-00001c80: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00001c90: 2e69 6f2f 646f 636b 6572 2f69 6d61 6765  .io/docker/image
-00001ca0: 2d73 697a 652f 726f 6e67 726f 6e67 6767  -size/rongronggg
-00001cb0: 392f 7273 732d 746f 2d74 656c 6567 7261  9/rss-to-telegra
-00001cc0: 6d2f 6c61 7465 7374 3f6c 6f67 6f3d 646f  m/latest?logo=do
-00001cd0: 636b 6572 295d 2868 7474 7073 3a2f 2f68  cker)](https://h
-00001ce0: 7562 2e64 6f63 6b65 722e 636f 6d2f 722f  ub.docker.com/r/
-00001cf0: 726f 6e67 726f 6e67 6767 392f 7273 732d  rongronggg9/rss-
-00001d00: 746f 2d74 656c 6567 7261 6d29 0a5b 215b  to-telegram).[![
-00001d10: 4275 696c 6420 7374 6174 7573 2028 6d61  Build status (ma
-00001d20: 7374 6572 295d 2868 7474 7073 3a2f 2f69  ster)](https://i
-00001d30: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00001d40: 7468 7562 2f61 6374 696f 6e73 2f77 6f72  thub/actions/wor
-00001d50: 6b66 6c6f 772f 7374 6174 7573 2f52 6f6e  kflow/status/Ron
-00001d60: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
-00001d70: 5465 6c65 6772 616d 2d42 6f74 2f70 7562  Telegram-Bot/pub
-00001d80: 6c69 7368 2d64 6f63 6b65 722d 696d 6167  lish-docker-imag
-00001d90: 652e 796d 6c3f 6272 616e 6368 3d6d 6173  e.yml?branch=mas
-00001da0: 7465 7226 6c61 6265 6c3d 6275 696c 6426  ter&label=build&
-00001db0: 6c6f 676f 3d64 6f63 6b65 7229 5d28 6874  logo=docker)](ht
-00001dc0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001dd0: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
-00001de0: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
-00001df0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00001e00: 7773 2f70 7562 6c69 7368 2d64 6f63 6b65  ws/publish-docke
-00001e10: 722d 696d 6167 652e 796d 6c3f 7175 6572  r-image.yml?quer
-00001e20: 793d 6272 616e 6368 2533 416d 6173 7465  y=branch%3Amaste
-00001e30: 7229 0a5b 215b 4275 696c 6420 7374 6174  r).[![Build stat
-00001e40: 7573 2028 6465 7629 5d28 6874 7470 733a  us (dev)](https:
-00001e50: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00001e60: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
-00001e70: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
-00001e80: 526f 6e67 726f 6e67 6767 392f 5253 532d  Rongronggg9/RSS-
-00001e90: 746f 2d54 656c 6567 7261 6d2d 426f 742f  to-Telegram-Bot/
-00001ea0: 7075 626c 6973 682d 646f 636b 6572 2d69  publish-docker-i
-00001eb0: 6d61 6765 2e79 6d6c 3f62 7261 6e63 683d  mage.yml?branch=
-00001ec0: 6465 7626 6c61 6265 6c3d 6275 696c 6425  dev&label=build%
-00001ed0: 3230 2532 3864 6576 2532 3926 6c6f 676f  20%28dev%29&logo
-00001ee0: 3d64 6f63 6b65 7229 5d28 6874 7470 733a  =docker)](https:
-00001ef0: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6f6e  //github.com/Ron
-00001f00: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
-00001f10: 5465 6c65 6772 616d 2d42 6f74 2f61 6374  Telegram-Bot/act
-00001f20: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00001f30: 7562 6c69 7368 2d64 6f63 6b65 722d 696d  ublish-docker-im
-00001f40: 6167 652e 796d 6c3f 7175 6572 793d 6272  age.yml?query=br
-00001f50: 616e 6368 2533 4164 6576 290a 5b21 5b44  anch%3Adev).[![D
-00001f60: 6f63 6b65 7220 7075 6c6c 735d 2868 7474  ocker pulls](htt
-00001f70: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00001f80: 2e69 6f2f 646f 636b 6572 2f70 756c 6c73  .io/docker/pulls
-00001f90: 2f72 6f6e 6772 6f6e 6767 6739 2f72 7373  /rongronggg9/rss
-00001fa0: 2d74 6f2d 7465 6c65 6772 616d 3f6c 6162  -to-telegram?lab
-00001fb0: 656c 3d70 756c 6c73 266c 6f67 6f3d 646f  el=pulls&logo=do
-00001fc0: 636b 6572 2663 6f6c 6f72 3d69 6e66 6f72  cker&color=infor
-00001fd0: 6d61 7469 6f6e 616c 295d 2868 7474 7073  mational)](https
-00001fe0: 3a2f 2f68 7562 2e64 6f63 6b65 722e 636f  ://hub.docker.co
-00001ff0: 6d2f 722f 726f 6e67 726f 6e67 6767 392f  m/r/rongronggg9/
-00002000: 7273 732d 746f 2d74 656c 6567 7261 6d29  rss-to-telegram)
-00002010: 0a0a 4974 2069 7320 7175 6974 6520 6561  ..It is quite ea
-00002020: 7379 2074 6f20 6465 706c 6f79 2079 6f75  sy to deploy you
-00002030: 7220 5253 5374 5420 696e 7374 616e 6365  r RSStT instance
-00002040: 2e20 5468 6520 6d6f 7374 2072 6563 6f6d  . The most recom
-00002050: 6d65 6e64 6564 2077 6179 2074 6f20 6465  mended way to de
-00002060: 706c 6f79 2052 5353 7454 2069 7320 446f  ploy RSStT is Do
-00002070: 636b 6572 2043 6f6d 706f 7365 3a20 6974  cker Compose: it
-00002080: 2069 7320 7375 6974 6162 6c65 2066 6f72   is suitable for
-00002090: 2076 6972 7475 616c 6c79 2061 6c6c 2056   virtually all V
-000020a0: 5053 2e20 5b52 6169 6c77 6179 2e61 7070  PS. [Railway.app
-000020b0: 5d28 6874 7470 733a 2f2f 7261 696c 7761  ](https://railwa
-000020c0: 792e 6170 7029 2028 6120 5061 6153 2070  y.app) (a PaaS p
-000020d0: 6c61 7466 6f72 6d29 2069 7320 616c 736f  latform) is also
-000020e0: 206f 6666 6963 6961 6c6c 7920 7375 7070   officially supp
-000020f0: 6f72 7465 642e 2059 6f75 206d 6179 2061  orted. You may a
-00002100: 6c73 6f20 696e 7374 616c 6c20 5253 5374  lso install RSSt
-00002110: 5420 6672 6f6d 2050 7950 4920 2874 7261  T from PyPI (tra
-00002120: 636b 696e 6720 606d 6173 7465 7260 2062  cking `master` b
-00002130: 7261 6e63 6829 206f 7220 5465 7374 5079  ranch) or TestPy
-00002140: 5049 2028 7472 6163 6b69 6e67 2060 6465  PI (tracking `de
-00002150: 7660 2062 7261 6e63 682c 2077 6869 6368  v` branch, which
-00002160: 2069 7320 6c61 7465 7374 2920 7573 696e   is latest) usin
-00002170: 6720 7069 702e 2046 6f72 2064 6576 656c  g pip. For devel
-00002180: 6f70 6572 7320 6f72 2065 7870 6572 6965  opers or experie
-00002190: 6e63 6564 2075 7365 7273 2c20 6469 7274  nced users, dirt
-000021a0: 7920 7275 6e20 6672 6f6d 2073 6f75 7263  y run from sourc
-000021b0: 6520 6973 2061 6c73 6f20 616e 206f 7074  e is also an opt
-000021c0: 696f 6e2e 0a0a 3c61 2068 7265 663d 2264  ion...<a href="d
-000021d0: 6f63 732f 6465 706c 6f79 6d65 6e74 2d67  ocs/deployment-g
-000021e0: 7569 6465 2e6d 6423 6f70 7469 6f6e 2d32  uide.md#option-2
-000021f0: 2d72 6169 6c77 6179 6170 7022 3e3c 696d  -railwayapp"><im
-00002200: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00002210: 6169 6c77 6179 2e61 7070 2f62 7574 746f  ailway.app/butto
-00002220: 6e2e 7376 6722 2068 6569 6768 743d 2233  n.svg" height="3
-00002230: 3022 2061 6c74 3d22 4465 706c 6f79 206f  0" alt="Deploy o
-00002240: 6e20 5261 696c 7761 7922 3e3c 2f61 3e0a  n Railway"></a>.
-00002250: 0a46 6f72 206d 6f72 6520 6465 7461 696c  .For more detail
-00002260: 732c 2072 6566 6572 2074 6f20 7468 6520  s, refer to the 
-00002270: 5b64 6570 6c6f 796d 656e 7420 6775 6964  [deployment guid
-00002280: 655d 2864 6f63 732f 6465 706c 6f79 6d65  e](docs/deployme
-00002290: 6e74 2d67 7569 6465 2e6d 6429 2e0a 0a23  nt-guide.md)...#
-000022a0: 2320 5472 616e 736c 6174 696f 6e0a 0a52  # Translation..R
-000022b0: 6561 6420 7468 6520 7472 616e 736c 6174  ead the translat
-000022c0: 696f 6e20 6775 6964 6520 5b68 6572 655d  ion guide [here]
-000022d0: 2864 6f63 732f 7472 616e 736c 6174 696f  (docs/translatio
-000022e0: 6e2d 6775 6964 652e 6d64 292e 0a0a 596f  n-guide.md)...Yo
-000022f0: 7520 6361 6e20 6865 6c70 2074 6f20 7472  u can help to tr
-00002300: 616e 736c 6174 6520 7468 6520 626f 7420  anslate the bot 
-00002310: 7573 696e 6720 5b48 6f73 7465 6420 5765  using [Hosted We
-00002320: 626c 6174 655d 2868 7474 7073 3a2f 2f68  blate](https://h
-00002330: 6f73 7465 642e 7765 626c 6174 652e 6f72  osted.weblate.or
-00002340: 672f 7072 6f6a 6563 7473 2f72 7373 2d74  g/projects/rss-t
-00002350: 6f2d 7465 6c65 6772 616d 2d62 6f74 2f29  o-telegram-bot/)
-00002360: 2e20 5370 6563 6961 6c20 7468 616e 6b73  . Special thanks
-00002370: 2074 6f20 7468 6569 7220 6672 6565 2068   to their free h
-00002380: 6f73 7469 6e67 2073 6572 7669 6365 2066  osting service f
-00002390: 6f72 206c 6962 7265 2070 726f 6a65 6374  or libre project
-000023a0: 7321 0a0a 3c61 2068 7265 663d 2268 7474  s!..<a href="htt
-000023b0: 7073 3a2f 2f68 6f73 7465 642e 7765 626c  ps://hosted.webl
-000023c0: 6174 652e 6f72 672f 656e 6761 6765 2f72  ate.org/engage/r
-000023d0: 7373 2d74 6f2d 7465 6c65 6772 616d 2d62  ss-to-telegram-b
-000023e0: 6f74 2f22 3e3c 696d 6720 7372 633d 2268  ot/"><img src="h
-000023f0: 7474 7073 3a2f 2f68 6f73 7465 642e 7765  ttps://hosted.we
-00002400: 626c 6174 652e 6f72 672f 7769 6467 6574  blate.org/widget
-00002410: 732f 7273 732d 746f 2d74 656c 6567 7261  s/rss-to-telegra
-00002420: 6d2d 626f 742f 2d2f 676c 6f73 7361 7279  m-bot/-/glossary
-00002430: 2f6d 756c 7469 2d61 7574 6f2e 7376 6722  /multi-auto.svg"
-00002440: 2077 6964 7468 203d 2022 3530 3022 2061   width = "500" a
-00002450: 6c74 3d22 2220 2f3e 3c2f 613e 0a0a 2323  lt="" /></a>..##
-00002460: 2055 7369 6e67 2074 6865 2070 7562 6c69   Using the publi
-00002470: 6320 626f 740a 0a54 6865 205b 7075 626c  c bot..The [publ
-00002480: 6963 2062 6f74 5d28 6874 7470 733a 2f2f  ic bot](https://
-00002490: 742e 6d65 2f52 5353 7454 5f42 6f74 2920  t.me/RSStT_Bot) 
-000024a0: 636f 6d65 7320 7769 7468 2061 6273 6f6c  comes with absol
-000024b0: 7574 656c 7920 6e6f 2077 6172 7261 6e74  utely no warrant
-000024c0: 792e 2049 2077 696c 6c20 7472 7920 6d79  y. I will try my
-000024d0: 2062 6573 7420 746f 206d 6169 6e74 6169   best to maintai
-000024e0: 6e20 6974 2c20 6275 7420 4920 6361 6e6e  n it, but I cann
-000024f0: 6f74 2067 7561 7261 6e74 6565 2074 6861  ot guarantee tha
-00002500: 7420 6974 2077 696c 6c20 616c 7761 7973  t it will always
-00002510: 2077 6f72 6b20 7065 7266 6563 746c 792e   work perfectly.
-00002520: 204d 6561 6e77 6869 6c65 2c20 796f 7520   Meanwhile, you 
-00002530: 7368 6f75 6c64 2022 6661 6972 2075 7365  should "fair use
-00002540: 2220 7468 6520 626f 742c 2061 766f 6964  " the bot, avoid
-00002550: 2073 7562 7363 7269 6269 6e67 2074 6f20   subscribing to 
-00002560: 746f 6f20 6d61 6e79 2052 5353 2066 6565  too many RSS fee
-00002570: 6473 2e20 200a 4966 2079 6f75 2075 7365  ds.  .If you use
-00002580: 2074 6865 205b 7075 626c 6963 2062 6f74   the [public bot
-00002590: 5d28 6874 7470 733a 2f2f 742e 6d65 2f52  ](https://t.me/R
-000025a0: 5353 7454 5f42 6f74 2920 696e 2079 6f75  SStT_Bot) in you
-000025b0: 7220 4368 616e 6e65 6c2c 2063 6f6e 7369  r Channel, consi
-000025c0: 6465 7220 6d65 6e74 696f 6e69 6e67 2074  der mentioning t
-000025d0: 6865 2062 6f74 2028 6f72 2074 6869 7320  he bot (or this 
-000025e0: 7072 6f6a 6563 7429 2069 6e20 796f 7572  project) in your
-000025f0: 2063 6861 6e6e 656c 2064 6573 6372 6970   channel descrip
-00002600: 7469 6f6e 2028 6f72 2070 696e 6e65 6420  tion (or pinned 
-00002610: 6d65 7373 6167 6529 2074 6f20 6c65 7420  message) to let 
-00002620: 6d6f 7265 2070 656f 706c 6520 6b6e 6f77  more people know
-00002630: 2061 626f 7574 2069 742e 2054 6861 7427   about it. That'
-00002640: 7320 6e6f 7420 6120 636f 6d70 756c 7369  s not a compulsi
-00002650: 6f6e 2e0a 0a23 2320 4b6e 6f77 6e20 6368  on...## Known ch
-00002660: 616e 6e65 6c73 2075 7369 6e67 2052 5353  annels using RSS
-00002670: 7454 0a0a 5761 6e74 2074 6f20 7072 6576  tT..Want to prev
-00002680: 6965 7720 7768 6174 2074 6865 206d 6573  iew what the mes
-00002690: 7361 6765 7320 7365 6e74 2062 7920 5253  sages sent by RS
-000026a0: 5374 5420 6c6f 6f6b 206c 696b 653f 2048  StT look like? H
-000026b0: 6572 6520 6973 2061 205b 6c69 7374 206f  ere is a [list o
-000026c0: 6620 6368 616e 6e65 6c73 2075 7369 6e67  f channels using
-000026d0: 2052 5353 7454 5d28 646f 6373 2f63 6861   RSStT](docs/cha
-000026e0: 6e6e 656c 732d 7573 696e 672d 7273 7374  nnels-using-rsst
-000026f0: 742e 6d64 292e 0a0a 2323 204c 6963 656e  t.md)...## Licen
-00002700: 7365 0a0a 5468 6973 2070 726f 6a65 6374  se..This project
-00002710: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00002720: 6572 205b 4147 504c 7633 5d28 4c49 4345  er [AGPLv3](LICE
-00002730: 4e53 4529 2e20 436c 6f73 6564 2d73 6f75  NSE). Closed-sou
-00002740: 7263 6520 6469 7374 7269 6275 7469 6f6e  rce distribution
-00002750: 206f 7220 626f 742d 686f 7374 696e 6720   or bot-hosting 
-00002760: 6172 6520 7374 7269 6374 6c79 2070 726f  are strictly pro
-00002770: 6869 6269 7465 642e 2049 6620 796f 7520  hibited. If you 
-00002780: 6d6f 6469 6679 2074 6865 2063 6f64 6520  modify the code 
-00002790: 616e 6420 6469 7374 7269 6275 7465 206f  and distribute o
-000027a0: 7220 686f 7374 2069 742c 206d 616b 6520  r host it, make 
-000027b0: 7375 7265 2061 6e79 2075 7365 7273 2077  sure any users w
-000027c0: 686f 2063 616e 2075 7365 2079 6f75 7220  ho can use your 
-000027d0: 626f 7420 6361 6e20 6765 7420 7468 6520  bot can get the 
-000027e0: 736f 7572 6365 2063 6f64 6520 2862 7920  source code (by 
-000027f0: 6564 6974 696e 6720 7468 6520 7265 706f  editing the repo
-00002800: 2055 524c 2069 6e20 5b60 7372 632f 6931   URL in [`src/i1
-00002810: 386e 2f5f 5f69 6e69 745f 5f2e 7079 605d  8n/__init__.py`]
-00002820: 2873 7263 2f69 3138 6e2f 5f5f 696e 6974  (src/i18n/__init
-00002830: 5f5f 2e70 7929 292e 0a0a 5468 6520 7265  __.py))...The re
-00002840: 706f 7369 746f 7279 2077 6173 2066 6f72  pository was for
-00002850: 6d65 726c 7920 6120 666f 726b 206f 6620  merly a fork of 
-00002860: 5b42 6f4b 4b65 522f 5253 532d 746f 2d54  [BoKKeR/RSS-to-T
-00002870: 656c 6567 7261 6d2d 426f 745d 2868 7474  elegram-Bot](htt
-00002880: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002890: 426f 4b4b 6552 2f52 5353 2d74 6f2d 5465  BoKKeR/RSS-to-Te
-000028a0: 6c65 6772 616d 2d42 6f74 292e 2054 6865  legram-Bot). The
-000028b0: 7920 6861 7665 2062 6565 6e20 656e 7469  y have been enti
-000028c0: 7265 6c79 2064 6966 6665 7265 6e74 2070  rely different p
-000028d0: 726f 6a65 6374 7320 7369 6e63 6520 7468  rojects since th
-000028e0: 6520 6561 726c 7920 6461 7973 206f 6620  e early days of 
-000028f0: 7468 6973 2070 726f 6a65 6374 2e0a       this project..
+00000550: 3a3a 2033 2e31 320a 436c 6173 7369 6669  :: 3.12.Classifi
+00000560: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000570: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000580: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
+00000590: 7469 6f6e 203a 3a20 4350 7974 686f 6e0a  tion :: CPython.
+000005a0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000005b0: 6320 3a3a 2043 6f6d 6d75 6e69 6361 7469  c :: Communicati
+000005c0: 6f6e 7320 3a3a 2043 6861 740a 436c 6173  ons :: Chat.Clas
+000005d0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+000005e0: 2049 6e74 6572 6e65 740a 436c 6173 7369   Internet.Classi
+000005f0: 6669 6572 3a20 546f 7069 6320 3a3a 204d  fier: Topic :: M
+00000600: 756c 7469 6d65 6469 610a 5265 7175 6972  ultimedia.Requir
+00000610: 6573 2d50 7974 686f 6e3a 203e 3d33 2e39  es-Python: >=3.9
+00000620: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000630: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+00000640: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
+00000650: 2d46 696c 653a 204c 4943 454e 5345 0a52  -File: LICENSE.R
+00000660: 6571 7569 7265 732d 4469 7374 3a20 6372  equires-Dist: cr
+00000670: 7970 7467 3d3d 302e 342e 300a 5265 7175  yptg==0.4.0.Requ
+00000680: 6972 6573 2d44 6973 743a 2074 656c 6574  ires-Dist: telet
+00000690: 686f 6e3d 3d31 2e33 352e 300a 5265 7175  hon==1.35.0.Requ
+000006a0: 6972 6573 2d44 6973 743a 2061 696f 6772  ires-Dist: aiogr
+000006b0: 6170 6866 6978 3d3d 302e 322e 320a 5265  aphfix==0.2.2.Re
+000006c0: 7175 6972 6573 2d44 6973 743a 2066 6565  quires-Dist: fee
+000006d0: 6470 6172 7365 723d 3d36 2e30 2e31 310a  dparser==6.0.11.
+000006e0: 5265 7175 6972 6573 2d44 6973 743a 206c  Requires-Dist: l
+000006f0: 6973 7470 6172 7365 725b 6c78 6d6c 5d3d  istparser[lxml]=
+00000700: 3d30 2e32 300a 5265 7175 6972 6573 2d44  =0.20.Requires-D
+00000710: 6973 743a 2070 696c 6c6f 773d 3d31 302e  ist: pillow==10.
+00000720: 332e 300a 5265 7175 6972 6573 2d44 6973  3.0.Requires-Dis
+00000730: 743a 2062 6561 7574 6966 756c 736f 7570  t: beautifulsoup
+00000740: 343d 3d34 2e31 322e 330a 5265 7175 6972  4==4.12.3.Requir
+00000750: 6573 2d44 6973 743a 206c 786d 6c3d 3d35  es-Dist: lxml==5
+00000760: 2e32 2e31 0a52 6571 7569 7265 732d 4469  .2.1.Requires-Di
+00000770: 7374 3a20 7261 7069 6466 757a 7a3d 3d33  st: rapidfuzz==3
+00000780: 2e39 2e30 0a52 6571 7569 7265 732d 4469  .9.0.Requires-Di
+00000790: 7374 3a20 656d 6f6a 693d 3d32 2e31 312e  st: emoji==2.11.
+000007a0: 310a 5265 7175 6972 6573 2d44 6973 743a  1.Requires-Dist:
+000007b0: 206d 696e 6966 792d 6874 6d6c 3d3d 302e   minify-html==0.
+000007c0: 3135 2e30 0a52 6571 7569 7265 732d 4469  15.0.Requires-Di
+000007d0: 7374 3a20 6d69 6e69 6679 2d68 746d 6c2d  st: minify-html-
+000007e0: 6f6e 6570 6173 733d 3d30 2e31 352e 300a  onepass==0.15.0.
+000007f0: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
+00000800: 6174 706c 6f74 6c69 623d 3d33 2e38 2e34  atplotlib==3.8.4
+00000810: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000820: 6173 796e 6370 673d 3d30 2e32 392e 300a  asyncpg==0.29.0.
+00000830: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000840: 6f72 746f 6973 652d 6f72 6d5b 6163 6365  ortoise-orm[acce
+00000850: 6c5d 3d3d 302e 3230 2e31 0a52 6571 7569  l]==0.20.1.Requi
+00000860: 7265 732d 4469 7374 3a20 6165 7269 6368  res-Dist: aerich
+00000870: 3d3d 302e 372e 320a 5265 7175 6972 6573  ==0.7.2.Requires
+00000880: 2d44 6973 743a 2061 696f 6874 7470 5b73  -Dist: aiohttp[s
+00000890: 7065 6564 7570 735d 3d3d 332e 392e 350a  peedups]==3.9.5.
+000008a0: 5265 7175 6972 6573 2d44 6973 743a 2061  Requires-Dist: a
+000008b0: 696f 6874 7470 2d73 6f63 6b73 3d3d 302e  iohttp-socks==0.
+000008c0: 382e 340a 5265 7175 6972 6573 2d44 6973  8.4.Requires-Dis
+000008d0: 743a 2061 696f 6874 7470 2d72 6574 7279  t: aiohttp-retry
+000008e0: 3d3d 322e 382e 330a 5265 7175 6972 6573  ==2.8.3.Requires
+000008f0: 2d44 6973 743a 2070 7974 686f 6e2d 736f  -Dist: python-so
+00000900: 636b 735b 6173 796e 6369 6f5d 3d3d 322e  cks[asyncio]==2.
+00000910: 342e 340a 5265 7175 6972 6573 2d44 6973  4.4.Requires-Dis
+00000920: 743a 2064 6e73 7079 7468 6f6e 5b69 646e  t: dnspython[idn
+00000930: 615d 3d3d 322e 362e 310a 5265 7175 6972  a]==2.6.1.Requir
+00000940: 6573 2d44 6973 743a 2063 6f6c 6f72 6c6f  es-Dist: colorlo
+00000950: 673d 3d36 2e38 2e32 0a52 6571 7569 7265  g==6.8.2.Require
+00000960: 732d 4469 7374 3a20 4150 5363 6865 6475  s-Dist: APSchedu
+00000970: 6c65 723d 3d33 2e31 302e 340a 5265 7175  ler==3.10.4.Requ
+00000980: 6972 6573 2d44 6973 743a 2070 7974 686f  ires-Dist: pytho
+00000990: 6e2d 646f 7465 6e76 3d3d 312e 302e 310a  n-dotenv==1.0.1.
+000009a0: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
+000009b0: 756c 7469 6469 6374 3d3d 362e 302e 350a  ultidict==6.0.5.
+000009c0: 5265 7175 6972 6573 2d44 6973 743a 2061  Requires-Dist: a
+000009d0: 7379 6e63 7374 646c 6962 3d3d 332e 3132  syncstdlib==3.12
+000009e0: 2e33 0a52 6571 7569 7265 732d 4469 7374  .3.Requires-Dist
+000009f0: 3a20 6361 6368 6574 6f6f 6c73 3d3d 352e  : cachetools==5.
+00000a00: 332e 330a 5265 7175 6972 6573 2d44 6973  3.3.Requires-Dis
+00000a10: 743a 2043 4a4b 7772 6170 3d3d 322e 320a  t: CJKwrap==2.2.
+00000a20: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000a30: 7970 696e 672d 6578 7465 6e73 696f 6e73  yping-extensions
+00000a40: 3d3d 342e 3131 2e30 0a52 6571 7569 7265  ==4.11.0.Require
+00000a50: 732d 4469 7374 3a20 7576 6c6f 6f70 3d3d  s-Dist: uvloop==
+00000a60: 302e 3139 2e30 3b20 7379 735f 706c 6174  0.19.0; sys_plat
+00000a70: 666f 726d 2021 3d20 2277 696e 3332 2220  form != "win32" 
+00000a80: 616e 6420 7379 735f 706c 6174 666f 726d  and sys_platform
+00000a90: 2021 3d20 2263 7967 7769 6e22 2061 6e64   != "cygwin" and
+00000aa0: 2073 7973 5f70 6c61 7466 6f72 6d20 213d   sys_platform !=
+00000ab0: 2022 636c 6922 0a52 6571 7569 7265 732d   "cli".Requires-
+00000ac0: 4469 7374 3a20 6973 616c 3d3d 312e 362e  Dist: isal==1.6.
+00000ad0: 313b 2070 6c61 7466 6f72 6d5f 6d61 6368  1; platform_mach
+00000ae0: 696e 6520 3d3d 2022 7838 365f 3634 2220  ine == "x86_64" 
+00000af0: 6f72 2070 6c61 7466 6f72 6d5f 6d61 6368  or platform_mach
+00000b00: 696e 6520 3d3d 2022 414d 4436 3422 206f  ine == "AMD64" o
+00000b10: 7220 706c 6174 666f 726d 5f6d 6163 6869  r platform_machi
+00000b20: 6e65 203d 3d20 2261 6172 6368 3634 220a  ne == "aarch64".
+00000b30: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000b40: 7222 3e0a 3c69 6d67 2073 7263 3d22 646f  r">.<img src="do
+00000b50: 6373 2f72 6573 6f75 7263 6573 2f52 5353  cs/resources/RSS
+00000b60: 7454 5f69 636f 6e2e 7376 6722 2061 6c74  tT_icon.svg" alt
+00000b70: 3d22 5253 5320 746f 2054 656c 6567 7261  ="RSS to Telegra
+00000b80: 6d20 426f 7422 2077 6964 7468 3d22 3130  m Bot" width="10
+00000b90: 3022 3e0a 3c2f 703e 0a3c 6831 2061 6c69  0">.</p>.<h1 ali
+00000ba0: 676e 3d22 6365 6e74 6572 223e 5253 5320  gn="center">RSS 
+00000bb0: 746f 2054 656c 6567 7261 6d20 426f 743c  to Telegram Bot<
+00000bc0: 2f68 313e 0a0a 3c70 2061 6c69 676e 3d22  /h1>..<p align="
+00000bd0: 6365 6e74 6572 223e 3c62 3e41 2054 656c  center"><b>A Tel
+00000be0: 6567 7261 6d20 5253 5320 626f 7420 7468  egram RSS bot th
+00000bf0: 6174 2063 6172 6573 2061 626f 7574 2079  at cares about y
+00000c00: 6f75 7220 7265 6164 696e 6720 6578 7065  our reading expe
+00000c10: 7269 656e 6365 3c2f 623e 3c2f 703e 0a0a  rience</b></p>..
+00000c20: 5b21 5b47 6974 4875 6220 636f 6d6d 6974  [![GitHub commit
+00000c30: 2061 6374 6976 6974 795d 2868 7474 7073   activity](https
+00000c40: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000c50: 6f2f 6769 7468 7562 2f63 6f6d 6d69 742d  o/github/commit-
+00000c60: 6163 7469 7669 7479 2f6d 2f52 6f6e 6772  activity/m/Rongr
+00000c70: 6f6e 6767 6739 2f52 5353 2d74 6f2d 5465  onggg9/RSS-to-Te
+00000c80: 6c65 6772 616d 2d42 6f74 3f6c 6f67 6f3d  legram-Bot?logo=
+00000c90: 6769 7426 6c61 6265 6c3d 636f 6d6d 6974  git&label=commit
+00000ca0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000cb0: 622e 636f 6d2f 526f 6e67 726f 6e67 6767  b.com/Rongronggg
+00000cc0: 392f 5253 532d 746f 2d54 656c 6567 7261  9/RSS-to-Telegra
+00000cd0: 6d2d 426f 742f 636f 6d6d 6974 7329 0a5b  m-Bot/commits).[
+00000ce0: 215b 5472 616e 736c 6174 696e 6720 7374  ![Translating st
+00000cf0: 6174 7573 5d28 6874 7470 733a 2f2f 696d  atus](https://im
+00000d00: 672e 7368 6965 6c64 732e 696f 2f77 6562  g.shields.io/web
+00000d10: 6c61 7465 2f70 726f 6772 6573 732f 7273  late/progress/rs
+00000d20: 732d 746f 2d74 656c 6567 7261 6d2d 626f  s-to-telegram-bo
+00000d30: 743f 6c6f 676f 3d77 6562 6c61 7465 2663  t?logo=weblate&c
+00000d40: 6f6c 6f72 3d69 6e66 6f72 6d61 7469 6f6e  olor=information
+00000d50: 616c 295d 2868 7474 7073 3a2f 2f68 6f73  al)](https://hos
+00000d60: 7465 642e 7765 626c 6174 652e 6f72 672f  ted.weblate.org/
+00000d70: 656e 6761 6765 2f72 7373 2d74 6f2d 7465  engage/rss-to-te
+00000d80: 6c65 6772 616d 2d62 6f74 2f29 0a5b 215b  legram-bot/).[![
+00000d90: 436f 6465 2071 7561 6c69 7479 5d28 6874  Code quality](ht
+00000da0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000db0: 732e 696f 2f63 6f64 6566 6163 746f 722f  s.io/codefactor/
+00000dc0: 6772 6164 652f 6769 7468 7562 2f52 6f6e  grade/github/Ron
+00000dd0: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
+00000de0: 5465 6c65 6772 616d 2d42 6f74 3f6c 6f67  Telegram-Bot?log
+00000df0: 6f3d 636f 6465 6661 6374 6f72 295d 2868  o=codefactor)](h
+00000e00: 7474 7073 3a2f 2f77 7777 2e63 6f64 6566  ttps://www.codef
+00000e10: 6163 746f 722e 696f 2f72 6570 6f73 6974  actor.io/reposit
+00000e20: 6f72 792f 6769 7468 7562 2f72 6f6e 6772  ory/github/rongr
+00000e30: 6f6e 6767 6739 2f72 7373 2d74 6f2d 7465  onggg9/rss-to-te
+00000e40: 6c65 6772 616d 2d62 6f74 290a 5b21 5b47  legram-bot).[![G
+00000e50: 6974 4875 6220 7374 6172 735d 2868 7474  itHub stars](htt
+00000e60: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000e70: 2e69 6f2f 6769 7468 7562 2f73 7461 7273  .io/github/stars
+00000e80: 2f52 6f6e 6772 6f6e 6767 6739 2f52 7373  /Rongronggg9/Rss
+00000e90: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
+00000ea0: 3f73 7479 6c65 3d73 6f63 6961 6c29 5d28  ?style=social)](
+00000eb0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000ec0: 6f6d 2f52 6f6e 6772 6f6e 6767 6739 2f52  om/Rongronggg9/R
+00000ed0: 5353 2d74 6f2d 5465 6c65 6772 616d 2d42  SS-to-Telegram-B
+00000ee0: 6f74 2f73 7461 7267 617a 6572 7329 0a5b  ot/stargazers).[
+00000ef0: 215b 4769 7448 7562 2066 6f72 6b73 5d28  ![GitHub forks](
+00000f00: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000f10: 6c64 732e 696f 2f67 6974 6875 622f 666f  lds.io/github/fo
+00000f20: 726b 732f 526f 6e67 726f 6e67 6767 392f  rks/Rongronggg9/
+00000f30: 5253 532d 746f 2d54 656c 6567 7261 6d2d  RSS-to-Telegram-
+00000f40: 426f 743f 7374 796c 653d 736f 6369 616c  Bot?style=social
+00000f50: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000f60: 622e 636f 6d2f 526f 6e67 726f 6e67 6767  b.com/Rongronggg
+00000f70: 392f 5253 532d 746f 2d54 656c 6567 7261  9/RSS-to-Telegra
+00000f80: 6d2d 426f 742f 666f 726b 290a 0a5b 215b  m-Bot/fork)..[![
+00000f90: 5465 6c65 6772 616d 2062 6f74 5d28 6874  Telegram bot](ht
+00000fa0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000fb0: 732e 696f 2f62 6164 6765 2f54 656c 6567  s.io/badge/Teleg
+00000fc0: 7261 6d25 3230 426f 742d 2534 3052 5353  ram%20Bot-%40RSS
+00000fd0: 7454 5f5f 426f 742d 3232 3965 6439 3f6c  tT__Bot-229ed9?l
+00000fe0: 6f67 6f3d 7465 6c65 6772 616d 2673 7479  ogo=telegram&sty
+00000ff0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00001000: 295d 2868 7474 7073 3a2f 2f74 2e6d 652f  )](https://t.me/
+00001010: 5253 5374 545f 426f 7429 0a5b 215b 5465  RSStT_Bot).[![Te
+00001020: 6c65 6772 616d 2067 726f 7570 5d28 6874  legram group](ht
+00001030: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00001040: 732e 696f 2f62 6164 6765 2f64 796e 616d  s.io/badge/dynam
+00001050: 6963 2f6a 736f 6e3f 7572 6c3d 6874 7470  ic/json?url=http
+00001060: 7325 3341 2532 4625 3246 6170 692e 7377  s%3A%2F%2Fapi.sw
+00001070: 6f2e 6d6f 6525 3246 7374 6174 7325 3246  o.moe%2Fstats%2F
+00001080: 7465 6c65 6772 616d 2532 4652 5353 7454  telegram%2FRSStT
+00001090: 5f47 726f 7570 2671 7565 7279 3d63 6f75  _Group&query=cou
+000010a0: 6e74 2663 6f6c 6f72 3d32 4341 3545 3026  nt&color=2CA5E0&
+000010b0: 6c61 6265 6c3d 5465 6c65 6772 616d 2532  label=Telegram%2
+000010c0: 3047 726f 7570 266c 6f67 6f3d 7465 6c65  0Group&logo=tele
+000010d0: 6772 616d 2663 6163 6865 5365 636f 6e64  gram&cacheSecond
+000010e0: 733d 3336 3030 2673 7479 6c65 3d66 6f72  s=3600&style=for
+000010f0: 2d74 6865 2d62 6164 6765 295d 2868 7474  -the-badge)](htt
+00001100: 7073 3a2f 2f74 2e6d 652f 5253 5374 545f  ps://t.me/RSStT_
+00001110: 4772 6f75 7029 0a5b 215b 5465 6c65 6772  Group).[![Telegr
+00001120: 616d 2063 6861 6e6e 656c 5d28 6874 7470  am channel](http
+00001130: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00001140: 696f 2f62 6164 6765 2f64 796e 616d 6963  io/badge/dynamic
+00001150: 2f6a 736f 6e3f 7572 6c3d 6874 7470 7325  /json?url=https%
+00001160: 3341 2532 4625 3246 6170 692e 7377 6f2e  3A%2F%2Fapi.swo.
+00001170: 6d6f 6525 3246 7374 6174 7325 3246 7465  moe%2Fstats%2Fte
+00001180: 6c65 6772 616d 2532 4652 5353 7454 5f43  legram%2FRSStT_C
+00001190: 6861 6e6e 656c 2671 7565 7279 3d63 6f75  hannel&query=cou
+000011a0: 6e74 2663 6f6c 6f72 3d32 4341 3545 3026  nt&color=2CA5E0&
+000011b0: 6c61 6265 6c3d 5465 6c65 6772 616d 2532  label=Telegram%2
+000011c0: 3043 6861 6e6e 656c 266c 6f67 6f3d 7465  0Channel&logo=te
+000011d0: 6c65 6772 616d 2663 6163 6865 5365 636f  legram&cacheSeco
+000011e0: 6e64 733d 3336 3030 2673 7479 6c65 3d66  nds=3600&style=f
+000011f0: 6f72 2d74 6865 2d62 6164 6765 295d 2868  or-the-badge)](h
+00001200: 7474 7073 3a2f 2f74 2e6d 652f 5253 5374  ttps://t.me/RSSt
+00001210: 545f 4368 616e 6e65 6c29 0a0a 7c20 5be7  T_Channel)..| [.
+00001220: ae80 e4bd 93e4 b8ad e696 8720 5245 4144  ........... READ
+00001230: 4d45 5d20 7c20 5b43 4841 4e47 454c 4f47  ME] | [CHANGELOG
+00001240: 5d20 7c20 5b46 4151 5d20 7c20 5b44 6f63  ] | [FAQ] | [Doc
+00001250: 756d 656e 7461 7469 6f6e 5d20 7c20 5b43  umentation] | [C
+00001260: 6861 6e6e 656c 7320 5573 696e 6720 5253  hannels Using RS
+00001270: 5374 545d 207c 0a7c 3a2d 2d2d 2d2d 2d2d  StT] |.|:-------
+00001280: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
+00001290: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 3a7c 2d2d  ----:|:-----:|--
+000012a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+000012b0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+000012c0: 2d2d 2d2d 2d2d 2d3a 7c0a 0a5b e7ae 80e4  -------:|..[....
+000012d0: bd93 e4b8 ade6 9687 2052 4541 444d 455d  ........ README]
+000012e0: 3a20 5245 4144 4d45 2e7a 682e 6d64 0a0a  : README.zh.md..
+000012f0: 5b43 4841 4e47 454c 4f47 5d3a 2064 6f63  [CHANGELOG]: doc
+00001300: 732f 4348 414e 4745 4c4f 472e 6d64 0a0a  s/CHANGELOG.md..
+00001310: 5b46 4151 5d3a 2064 6f63 732f 4641 512e  [FAQ]: docs/FAQ.
+00001320: 6d64 0a0a 5b44 6f63 756d 656e 7461 7469  md..[Documentati
+00001330: 6f6e 5d3a 2064 6f63 730a 0a5b 4368 616e  on]: docs..[Chan
+00001340: 6e65 6c73 2055 7369 6e67 2052 5353 7454  nels Using RSStT
+00001350: 5d3a 2064 6f63 732f 6368 616e 6e65 6c73  ]: docs/channels
+00001360: 2d75 7369 6e67 2d72 7373 7474 2e6d 640a  -using-rsstt.md.
+00001370: 0a3c 7461 626c 653e 0a20 2020 203c 7472  .<table>.    <tr
+00001380: 3e0a 2020 2020 2020 2020 3c74 643e 3c69  >.        <td><i
+00001390: 6d67 2073 7263 3d22 646f 6373 2f72 6573  mg src="docs/res
+000013a0: 6f75 7263 6573 2f65 7861 6d70 6c65 352e  ources/example5.
+000013b0: 706e 6722 2061 6c74 3d22 5363 7265 656e  png" alt="Screen
+000013c0: 7368 6f74 223e 3c2f 7464 3e0a 2020 2020  shot"></td>.    
+000013d0: 2020 2020 3c74 6420 726f 7773 7061 6e3d      <td rowspan=
+000013e0: 2232 223e 3c69 6d67 2073 7263 3d22 646f  "2"><img src="do
+000013f0: 6373 2f72 6573 6f75 7263 6573 2f65 7861  cs/resources/exa
+00001400: 6d70 6c65 372e 706e 6722 2061 6c74 3d22  mple7.png" alt="
+00001410: 5363 7265 656e 7368 6f74 223e 3c2f 7464  Screenshot"></td
+00001420: 3e0a 2020 2020 2020 2020 3c74 6420 726f  >.        <td ro
+00001430: 7773 7061 6e3d 2232 223e 3c69 6d67 2073  wspan="2"><img s
+00001440: 7263 3d22 646f 6373 2f72 6573 6f75 7263  rc="docs/resourc
+00001450: 6573 2f65 7861 6d70 6c65 382e 706e 6722  es/example8.png"
+00001460: 2061 6c74 3d22 5363 7265 656e 7368 6f74   alt="Screenshot
+00001470: 223e 3c2f 7464 3e0a 2020 2020 3c2f 7472  "></td>.    </tr
+00001480: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00001490: 2020 203c 7464 3e3c 696d 6720 7372 633d     <td><img src=
+000014a0: 2264 6f63 732f 7265 736f 7572 6365 732f  "docs/resources/
+000014b0: 6578 616d 706c 6536 2e70 6e67 2220 616c  example6.png" al
+000014c0: 743d 2253 6372 6565 6e73 686f 7422 3e3c  t="Screenshot"><
+000014d0: 2f74 643e 0a20 2020 203c 2f74 723e 0a3c  /td>.    </tr>.<
+000014e0: 2f74 6162 6c65 3e0a 0a23 2320 4869 6768  /table>..## High
+000014f0: 6c69 6768 7473 0a0a 2d20 4d75 6c74 692d  lights..- Multi-
+00001500: 7573 6572 0a2d 2049 3138 6e0a 2020 2020  user.- I18n.    
+00001510: 2d20 456e 676c 6973 682c 2043 6869 6e65  - English, Chine
+00001520: 7365 2c20 4361 6e74 6f6e 6573 652c 2049  se, Cantonese, I
+00001530: 7461 6c69 616e 2c20 616e 6420 5b6d 6f72  talian, and [mor
+00001540: 655d 2864 6f63 732f 7472 616e 736c 6174  e](docs/translat
+00001550: 696f 6e2d 6775 6964 652e 6d64 2921 0a2d  ion-guide.md)!.-
+00001560: 2054 6865 2063 6f6e 7465 6e74 206f 6620   The content of 
+00001570: 7468 6520 706f 7374 7320 6f66 2061 6e20  the posts of an 
+00001580: 5253 5320 6665 6564 2077 696c 6c20 6265  RSS feed will be
+00001590: 2073 656e 7420 746f 2054 656c 6567 7261   sent to Telegra
+000015a0: 6d0a 2020 2020 2d20 4b65 6570 2072 6963  m.    - Keep ric
+000015b0: 682d 7465 7874 2066 6f72 6d61 740a 2020  h-text format.  
+000015c0: 2020 2d20 4b65 6570 206d 6564 6961 2028    - Keep media (
+000015d0: 6375 7374 6f6d 697a 6162 6c65 290a 2020  customizable).  
+000015e0: 2020 2020 2020 2d20 496d 6167 6573 2c20        - Images, 
+000015f0: 5669 6465 6f73 2c20 616e 6420 4175 6469  Videos, and Audi
+00001600: 6f20 626f 7468 2069 6e20 7468 6520 706f  o both in the po
+00001610: 7374 2063 6f6e 7465 6e74 2061 6e64 2065  st content and e
+00001620: 6e63 6c6f 7375 7265 3b20 446f 6375 6d65  nclosure; Docume
+00001630: 6e74 7320 696e 2074 6865 2070 6f73 7420  nts in the post 
+00001640: 656e 636c 6f73 7572 650a 2020 2020 2020  enclosure.      
+00001650: 2020 2d20 4c6f 6e67 2069 6d61 6765 7320    - Long images 
+00001660: 7769 6c6c 2062 6520 7365 6e74 2061 7320  will be sent as 
+00001670: 6669 6c65 7320 746f 2070 7265 7665 6e74  files to prevent
+00001680: 2054 656c 6567 7261 6d20 6672 6f6d 2063   Telegram from c
+00001690: 6f6d 7072 6573 7369 6e67 2074 6865 2069  ompressing the i
+000016a0: 6d61 6765 2061 6e64 206d 616b 696e 6720  mage and making 
+000016b0: 6974 2075 6e72 6561 6461 626c 650a 2020  it unreadable.  
+000016c0: 2020 2020 2020 2d20 4472 6f70 2061 6e6e        - Drop ann
+000016d0: 6f79 696e 6720 6963 6f6e 732c 2074 6865  oying icons, the
+000016e0: 7920 6272 6561 6b20 7468 6520 7265 6164  y break the read
+000016f0: 696e 6720 6578 7065 7269 656e 6365 0a20  ing experience. 
+00001700: 2020 202d 2041 7574 6f6d 6174 6963 616c     - Automatical
+00001710: 6c79 2072 6570 6c61 6365 2065 6d6f 6a69  ly replace emoji
+00001720: 2073 686f 7274 636f 6465 7320 7769 7468   shortcodes with
+00001730: 2065 6d6f 6a69 0a20 2020 202d 2041 7574   emoji.    - Aut
+00001740: 6f6d 6174 6963 616c 6c79 2072 6570 6c61  omatically repla
+00001750: 6365 2065 6d6f 6a69 2069 6d61 6765 7320  ce emoji images 
+00001760: 7769 7468 2065 6d6f 6a69 206f 7220 6974  with emoji or it
+00001770: 7320 6465 7363 7269 7074 696f 6e20 7465  s description te
+00001780: 7874 0a20 2020 202d 2041 7574 6f6d 6174  xt.    - Automat
+00001790: 6963 616c 6c79 2064 6574 6572 6d69 6e65  ically determine
+000017a0: 2077 6865 7468 6572 2074 6865 2074 6974   whether the tit
+000017b0: 6c65 206f 6620 7468 6520 5253 5320 6665  le of the RSS fe
+000017c0: 6564 2069 7320 6175 746f 2d66 696c 6c65  ed is auto-fille
+000017d0: 642c 2069 6620 736f 2c20 6f6d 6974 2074  d, if so, omit t
+000017e0: 6865 2074 6974 6c65 2028 6375 7374 6f6d  he title (custom
+000017f0: 697a 6162 6c65 290a 2020 2020 2d20 4175  izable).    - Au
+00001800: 746f 6d61 7469 6361 6c6c 7920 7368 6f77  tomatically show
+00001810: 2074 6865 2061 7574 686f 722d 6e61 6d65   the author-name
+00001820: 2028 6375 7374 6f6d 697a 6162 6c65 290a   (customizable).
+00001830: 2020 2020 2d20 4175 746f 6d61 7469 6361      - Automatica
+00001840: 6c6c 7920 7370 6c69 7420 746f 6f2d 6c6f  lly split too-lo
+00001850: 6e67 206d 6573 7361 6765 730a 2020 2020  ng messages.    
+00001860: 2d20 4d65 7373 6167 6573 2063 616e 2062  - Messages can b
+00001870: 6520 7365 6e74 2061 7320 5465 6c65 6772  e sent as Telegr
+00001880: 6170 6820 706f 7374 7320 2863 7573 746f  aph posts (custo
+00001890: 6d69 7a61 626c 6529 0a20 2020 2020 202d  mizable).      -
+000018a0: 204d 6f73 7420 696d 6167 6573 2061 6e64   Most images and
+000018b0: 2076 6964 656f 7320 7769 6c6c 2062 6520   videos will be 
+000018c0: 7570 6c6f 6164 6564 2074 6f20 5465 6c65  uploaded to Tele
+000018d0: 6772 6170 682c 2073 6f20 7468 6174 2049  graph, so that I
+000018e0: 6e73 7461 6e74 2056 6965 7720 7769 6c6c  nstant View will
+000018f0: 206c 6f61 6420 7261 7069 646c 790a 2d20   load rapidly.- 
+00001900: 5b56 6172 696f 7573 2063 7573 746f 6d69  [Various customi
+00001910: 7a61 626c 6520 666f 726d 6174 7469 6e67  zable formatting
+00001920: 2073 6574 7469 6e67 735d 2864 6f63 732f   settings](docs/
+00001930: 666f 726d 6174 7469 6e67 2d73 6574 7469  formatting-setti
+00001940: 6e67 732e 6d64 290a 2020 2020 2d20 4861  ngs.md).    - Ha
+00001950: 7368 7461 6773 2c20 6375 7374 6f6d 2074  shtags, custom t
+00001960: 6974 6c65 2c20 6574 632e 0a2d 2049 6e64  itle, etc..- Ind
+00001970: 6976 6964 7561 6c20 7072 6f78 7920 7365  ividual proxy se
+00001980: 7474 696e 6773 2066 6f72 2054 656c 6567  ttings for Teleg
+00001990: 7261 6d20 616e 6420 5253 5320 6665 6564  ram and RSS feed
+000019a0: 730a 2d20 4f50 4d4c 2069 6d70 6f72 7469  s.- OPML importi
+000019b0: 6e67 2061 6e64 2065 7870 6f72 7469 6e67  ng and exporting
+000019c0: 2028 6b65 6570 2063 7573 746f 6d20 7469   (keep custom ti
+000019d0: 746c 6529 0a2d 204f 7074 696d 697a 6564  tle).- Optimized
+000019e0: 2070 6572 666f 726d 616e 6365 2028 7365   performance (se
+000019f0: 6520 616c 736f 2074 6865 205b 4641 515d  e also the [FAQ]
+00001a00: 2864 6f63 732f 4641 512e 6d64 2371 2d68  (docs/FAQ.md#q-h
+00001a10: 6f77 2d69 732d 7468 652d 7065 7266 6f72  ow-is-the-perfor
+00001a20: 6d61 6e63 652d 6f66 2d74 6865 2d62 6f74  mance-of-the-bot
+00001a30: 2929 0a2d 2055 7365 722d 6672 6965 6e64  )).- User-friend
+00001a40: 6c79 0a2d 2048 5454 5020 4361 6368 696e  ly.- HTTP Cachin
+00001a50: 670a 0a23 2320 4465 706c 6f79 6d65 6e74  g..## Deployment
+00001a60: 0a0a 5b21 5b64 6f63 6b65 7269 2e63 6f5d  ..[![dockeri.co]
+00001a70: 2868 7474 7073 3a2f 2f64 6f63 6b65 7269  (https://dockeri
+00001a80: 636f 2e62 6c61 6e6b 656e 7368 6970 2e69  co.blankenship.i
+00001a90: 6f2f 696d 6167 652f 726f 6e67 726f 6e67  o/image/rongrong
+00001aa0: 6767 392f 7273 732d 746f 2d74 656c 6567  gg9/rss-to-teleg
+00001ab0: 7261 6d29 5d28 6874 7470 733a 2f2f 6875  ram)](https://hu
+00001ac0: 622e 646f 636b 6572 2e63 6f6d 2f72 2f72  b.docker.com/r/r
+00001ad0: 6f6e 6772 6f6e 6767 6739 2f72 7373 2d74  ongronggg9/rss-t
+00001ae0: 6f2d 7465 6c65 6772 616d 295c 0a5b 215b  o-telegram)\.[![
+00001af0: 4275 696c 6420 7374 6174 7573 2028 6d61  Build status (ma
+00001b00: 7374 6572 295d 2868 7474 7073 3a2f 2f69  ster)](https://i
+00001b10: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00001b20: 7468 7562 2f61 6374 696f 6e73 2f77 6f72  thub/actions/wor
+00001b30: 6b66 6c6f 772f 7374 6174 7573 2f52 6f6e  kflow/status/Ron
+00001b40: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
+00001b50: 5465 6c65 6772 616d 2d42 6f74 2f70 7562  Telegram-Bot/pub
+00001b60: 6c69 7368 2d64 6f63 6b65 722d 696d 6167  lish-docker-imag
+00001b70: 652e 796d 6c3f 6272 616e 6368 3d6d 6173  e.yml?branch=mas
+00001b80: 7465 7226 6c61 6265 6c3d 6275 696c 6426  ter&label=build&
+00001b90: 6c6f 676f 3d64 6f63 6b65 7229 5d28 6874  logo=docker)](ht
+00001ba0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001bb0: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
+00001bc0: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
+00001bd0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00001be0: 7773 2f70 7562 6c69 7368 2d64 6f63 6b65  ws/publish-docke
+00001bf0: 722d 696d 6167 652e 796d 6c3f 7175 6572  r-image.yml?quer
+00001c00: 793d 6272 616e 6368 2533 416d 6173 7465  y=branch%3Amaste
+00001c10: 7229 0a5b 215b 4275 696c 6420 7374 6174  r).[![Build stat
+00001c20: 7573 2028 6465 7629 5d28 6874 7470 733a  us (dev)](https:
+00001c30: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001c40: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
+00001c50: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
+00001c60: 526f 6e67 726f 6e67 6767 392f 5253 532d  Rongronggg9/RSS-
+00001c70: 746f 2d54 656c 6567 7261 6d2d 426f 742f  to-Telegram-Bot/
+00001c80: 7075 626c 6973 682d 646f 636b 6572 2d69  publish-docker-i
+00001c90: 6d61 6765 2e79 6d6c 3f62 7261 6e63 683d  mage.yml?branch=
+00001ca0: 6465 7626 6c61 6265 6c3d 6275 696c 6425  dev&label=build%
+00001cb0: 3230 2532 3864 6576 2532 3926 6c6f 676f  20%28dev%29&logo
+00001cc0: 3d64 6f63 6b65 7229 5d28 6874 7470 733a  =docker)](https:
+00001cd0: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6f6e  //github.com/Ron
+00001ce0: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
+00001cf0: 5465 6c65 6772 616d 2d42 6f74 2f61 6374  Telegram-Bot/act
+00001d00: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
+00001d10: 7562 6c69 7368 2d64 6f63 6b65 722d 696d  ublish-docker-im
+00001d20: 6167 652e 796d 6c3f 7175 6572 793d 6272  age.yml?query=br
+00001d30: 616e 6368 2533 4164 6576 290a 0a5b 215b  anch%3Adev)..[![
+00001d40: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
+00001d50: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00001d60: 692f 762f 7273 7374 743f 6c6f 676f 3d70  i/v/rsstt?logo=p
+00001d70: 7970 6926 6c6f 676f 436f 6c6f 723d 7768  ypi&logoColor=wh
+00001d80: 6974 6526 6c61 6265 6c3d 5079 5049 295d  ite&label=PyPI)]
+00001d90: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00001da0: 672f 7072 6f6a 6563 742f 7273 7374 742f  g/project/rsstt/
+00001db0: 290a 5b21 5b54 6573 7450 7950 495d 2868  ).[![TestPyPI](h
+00001dc0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00001dd0: 6473 2e69 6f2f 6261 6467 652f 6479 6e61  ds.io/badge/dyna
+00001de0: 6d69 632f 6a73 6f6e 3f75 726c 3d68 7474  mic/json?url=htt
+00001df0: 7073 2533 4125 3246 2532 4674 6573 742e  ps%3A%2F%2Ftest.
+00001e00: 7079 7069 2e6f 7267 2532 4670 7970 6925  pypi.org%2Fpypi%
+00001e10: 3246 7273 7374 7425 3246 6a73 6f6e 2671  2Frsstt%2Fjson&q
+00001e20: 7565 7279 3d25 3234 2e69 6e66 6f2e 7665  uery=%24.info.ve
+00001e30: 7273 696f 6e26 7072 6566 6978 3d76 266c  rsion&prefix=v&l
+00001e40: 6f67 6f3d 7079 7069 266c 6f67 6f43 6f6c  ogo=pypi&logoCol
+00001e50: 6f72 3d77 6869 7465 266c 6162 656c 3d54  or=white&label=T
+00001e60: 6573 7450 7950 4929 5d28 6874 7470 733a  estPyPI)](https:
+00001e70: 2f2f 7465 7374 2e70 7970 692e 6f72 672f  //test.pypi.org/
+00001e80: 7072 6f6a 6563 742f 7273 7374 742f 290a  project/rsstt/).
+00001e90: 5b21 5b50 7950 4920 2d20 5079 7468 6f6e  [![PyPI - Python
+00001ea0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+00001eb0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001ec0: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+00001ed0: 2f72 7373 7474 3f6c 6f67 6f3d 7079 7468  /rsstt?logo=pyth
+00001ee0: 6f6e 266c 6162 656c 3d26 6c61 6265 6c43  on&label=&labelC
+00001ef0: 6f6c 6f72 3d77 6869 7465 295d 2868 7474  olor=white)](htt
+00001f00: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+00001f10: 6f72 6729 5c0a 5b21 5b50 7950 4920 7075  org)\.[![PyPI pu
+00001f20: 626c 6973 6820 7374 6174 7573 5d28 6874  blish status](ht
+00001f30: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00001f40: 732e 696f 2f67 6974 6875 622f 6163 7469  s.io/github/acti
+00001f50: 6f6e 732f 776f 726b 666c 6f77 2f73 7461  ons/workflow/sta
+00001f60: 7475 732f 526f 6e67 726f 6e67 6767 392f  tus/Rongronggg9/
+00001f70: 5253 532d 746f 2d54 656c 6567 7261 6d2d  RSS-to-Telegram-
+00001f80: 426f 742f 7075 626c 6973 682d 746f 2d70  Bot/publish-to-p
+00001f90: 7970 692e 796d 6c3f 6c61 6265 6c3d 7075  ypi.yml?label=pu
+00001fa0: 626c 6973 6826 6c6f 676f 3d70 7970 6926  blish&logo=pypi&
+00001fb0: 6c6f 676f 436f 6c6f 723d 7768 6974 6529  logoColor=white)
+00001fc0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001fd0: 2e63 6f6d 2f52 6f6e 6772 6f6e 6767 6739  .com/Rongronggg9
+00001fe0: 2f52 5353 2d74 6f2d 5465 6c65 6772 616d  /RSS-to-Telegram
+00001ff0: 2d42 6f74 2f61 6374 696f 6e73 2f77 6f72  -Bot/actions/wor
+00002000: 6b66 6c6f 7773 2f70 7562 6c69 7368 2d74  kflows/publish-t
+00002010: 6f2d 7079 7069 2e79 6d6c 290a 5b21 5b54  o-pypi.yml).[![T
+00002020: 6573 7450 7950 4920 7075 626c 6973 6820  estPyPI publish 
+00002030: 7374 6174 7573 5d28 6874 7470 733a 2f2f  status](https://
+00002040: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00002050: 6974 6875 622f 6163 7469 6f6e 732f 776f  ithub/actions/wo
+00002060: 726b 666c 6f77 2f73 7461 7475 732f 526f  rkflow/status/Ro
+00002070: 6e67 726f 6e67 6767 392f 5253 532d 746f  ngronggg9/RSS-to
+00002080: 2d54 656c 6567 7261 6d2d 426f 742f 7075  -Telegram-Bot/pu
+00002090: 626c 6973 682d 746f 2d74 6573 742d 7079  blish-to-test-py
+000020a0: 7069 2e79 6d6c 3f6c 6162 656c 3d70 7562  pi.yml?label=pub
+000020b0: 6c69 7368 2532 3028 5465 7374 5079 5049  lish%20(TestPyPI
+000020c0: 2926 6c6f 676f 3d70 7970 6926 6c6f 676f  )&logo=pypi&logo
+000020d0: 436f 6c6f 723d 7768 6974 6529 5d28 6874  Color=white)](ht
+000020e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000020f0: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
+00002100: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
+00002110: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00002120: 7773 2f70 7562 6c69 7368 2d74 6f2d 7465  ws/publish-to-te
+00002130: 7374 2d70 7970 692e 796d 6c29 0a5b 215b  st-pypi.yml).[![
+00002140: 5079 5049 202d 2044 6f77 6e6c 6f61 6473  PyPI - Downloads
+00002150: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00002160: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
+00002170: 2f72 7373 7474 3f6c 6f67 6f3d 7079 7069  /rsstt?logo=pypi
+00002180: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
+00002190: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+000021a0: 6f72 672f 7072 6f6a 6563 742f 7273 7374  org/project/rsst
+000021b0: 742f 290a 0a49 7420 6973 2071 7569 7465  t/)..It is quite
+000021c0: 2065 6173 7920 746f 2064 6570 6c6f 7920   easy to deploy 
+000021d0: 796f 7572 2052 5353 7454 2069 6e73 7461  your RSStT insta
+000021e0: 6e63 652e 2054 6865 206d 6f73 7420 7265  nce. The most re
+000021f0: 636f 6d6d 656e 6465 6420 7761 7920 746f  commended way to
+00002200: 2064 6570 6c6f 7920 5253 5374 5420 6973   deploy RSStT is
+00002210: 2044 6f63 6b65 7220 436f 6d70 6f73 653a   Docker Compose:
+00002220: 2069 7420 6973 2073 7569 7461 626c 6520   it is suitable 
+00002230: 666f 7220 7669 7274 7561 6c6c 7920 616c  for virtually al
+00002240: 6c20 5650 532e 205b 5261 696c 7761 792e  l VPS. [Railway.
+00002250: 6170 705d 2868 7474 7073 3a2f 2f72 6169  app](https://rai
+00002260: 6c77 6179 2e61 7070 2920 2861 2050 6161  lway.app) (a Paa
+00002270: 5320 706c 6174 666f 726d 2920 6973 2061  S platform) is a
+00002280: 6c73 6f20 6f66 6669 6369 616c 6c79 2073  lso officially s
+00002290: 7570 706f 7274 6564 2e20 596f 7520 6d61  upported. You ma
+000022a0: 7920 616c 736f 2069 6e73 7461 6c6c 2052  y also install R
+000022b0: 5353 7454 2066 726f 6d20 5b50 7950 495d  SStT from [PyPI]
+000022c0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000022d0: 672f 7072 6f6a 6563 742f 7273 7374 742f  g/project/rsstt/
+000022e0: 2920 2874 7261 636b 696e 6720 606d 6173  ) (tracking `mas
+000022f0: 7465 7260 2062 7261 6e63 6829 206f 7220  ter` branch) or 
+00002300: 5b54 6573 7450 7950 495d 2868 7474 7073  [TestPyPI](https
+00002310: 3a2f 2f74 6573 742e 7079 7069 2e6f 7267  ://test.pypi.org
+00002320: 2f70 726f 6a65 6374 2f72 7373 7474 2f29  /project/rsstt/)
+00002330: 2028 7472 6163 6b69 6e67 2060 6465 7660   (tracking `dev`
+00002340: 2062 7261 6e63 682c 2077 6869 6368 2069   branch, which i
+00002350: 7320 616c 7761 7973 2075 702d 746f 2d64  s always up-to-d
+00002360: 6174 6529 2075 7369 6e67 2070 6970 2e20  ate) using pip. 
+00002370: 466f 7220 6465 7665 6c6f 7065 7273 206f  For developers o
+00002380: 7220 6578 7065 7269 656e 6365 6420 7573  r experienced us
+00002390: 6572 732c 2064 6972 7479 2072 756e 2066  ers, dirty run f
+000023a0: 726f 6d20 736f 7572 6365 2069 7320 616c  rom source is al
+000023b0: 736f 2061 6e20 6f70 7469 6f6e 2e0a 0a3c  so an option...<
+000023c0: 6120 6872 6566 3d22 646f 6373 2f64 6570  a href="docs/dep
+000023d0: 6c6f 796d 656e 742d 6775 6964 652e 6d64  loyment-guide.md
+000023e0: 236f 7074 696f 6e2d 322d 7261 696c 7761  #option-2-railwa
+000023f0: 7961 7070 223e 3c69 6d67 2073 7263 3d22  yapp"><img src="
+00002400: 6874 7470 733a 2f2f 7261 696c 7761 792e  https://railway.
+00002410: 6170 702f 6275 7474 6f6e 2e73 7667 2220  app/button.svg" 
+00002420: 6865 6967 6874 3d22 3330 2220 616c 743d  height="30" alt=
+00002430: 2244 6570 6c6f 7920 6f6e 2052 6169 6c77  "Deploy on Railw
+00002440: 6179 223e 3c2f 613e 0a0a 466f 7220 6d6f  ay"></a>..For mo
+00002450: 7265 2064 6574 6169 6c73 2c20 7265 6665  re details, refe
+00002460: 7220 746f 2074 6865 205b 6465 706c 6f79  r to the [deploy
+00002470: 6d65 6e74 2067 7569 6465 5d28 646f 6373  ment guide](docs
+00002480: 2f64 6570 6c6f 796d 656e 742d 6775 6964  /deployment-guid
+00002490: 652e 6d64 292e 0a0a 2323 2054 7261 6e73  e.md)...## Trans
+000024a0: 6c61 7469 6f6e 0a0a 5265 6164 2074 6865  lation..Read the
+000024b0: 2074 7261 6e73 6c61 7469 6f6e 2067 7569   translation gui
+000024c0: 6465 205b 6865 7265 5d28 646f 6373 2f74  de [here](docs/t
+000024d0: 7261 6e73 6c61 7469 6f6e 2d67 7569 6465  ranslation-guide
+000024e0: 2e6d 6429 2e0a 0a59 6f75 2063 616e 2068  .md)...You can h
+000024f0: 656c 7020 746f 2074 7261 6e73 6c61 7465  elp to translate
+00002500: 2074 6865 2062 6f74 2075 7369 6e67 205b   the bot using [
+00002510: 486f 7374 6564 2057 6562 6c61 7465 5d28  Hosted Weblate](
+00002520: 6874 7470 733a 2f2f 686f 7374 6564 2e77  https://hosted.w
+00002530: 6562 6c61 7465 2e6f 7267 2f70 726f 6a65  eblate.org/proje
+00002540: 6374 732f 7273 732d 746f 2d74 656c 6567  cts/rss-to-teleg
+00002550: 7261 6d2d 626f 742f 292e 2053 7065 6369  ram-bot/). Speci
+00002560: 616c 2074 6861 6e6b 7320 746f 2074 6865  al thanks to the
+00002570: 6972 2066 7265 6520 686f 7374 696e 6720  ir free hosting 
+00002580: 7365 7276 6963 6520 666f 7220 6c69 6272  service for libr
+00002590: 6520 7072 6f6a 6563 7473 210a 0a3c 6120  e projects!..<a 
+000025a0: 6872 6566 3d22 6874 7470 733a 2f2f 686f  href="https://ho
+000025b0: 7374 6564 2e77 6562 6c61 7465 2e6f 7267  sted.weblate.org
+000025c0: 2f65 6e67 6167 652f 7273 732d 746f 2d74  /engage/rss-to-t
+000025d0: 656c 6567 7261 6d2d 626f 742f 223e 3c69  elegram-bot/"><i
+000025e0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000025f0: 686f 7374 6564 2e77 6562 6c61 7465 2e6f  hosted.weblate.o
+00002600: 7267 2f77 6964 6765 7473 2f72 7373 2d74  rg/widgets/rss-t
+00002610: 6f2d 7465 6c65 6772 616d 2d62 6f74 2f2d  o-telegram-bot/-
+00002620: 2f67 6c6f 7373 6172 792f 6d75 6c74 692d  /glossary/multi-
+00002630: 6175 746f 2e73 7667 2220 7769 6474 6820  auto.svg" width 
+00002640: 3d20 2235 3030 2220 616c 743d 2222 202f  = "500" alt="" /
+00002650: 3e3c 2f61 3e0a 0a23 2320 5573 696e 6720  ></a>..## Using 
+00002660: 7468 6520 7075 626c 6963 2062 6f74 0a0a  the public bot..
+00002670: 5468 6520 5b70 7562 6c69 6320 626f 745d  The [public bot]
+00002680: 2868 7474 7073 3a2f 2f74 2e6d 652f 5253  (https://t.me/RS
+00002690: 5374 545f 426f 7429 2063 6f6d 6573 2077  StT_Bot) comes w
+000026a0: 6974 6820 6162 736f 6c75 7465 6c79 206e  ith absolutely n
+000026b0: 6f20 7761 7272 616e 7479 2e20 4920 7769  o warranty. I wi
+000026c0: 6c6c 2074 7279 206d 7920 6265 7374 2074  ll try my best t
+000026d0: 6f20 6d61 696e 7461 696e 2069 742c 2062  o maintain it, b
+000026e0: 7574 2049 2063 616e 6e6f 7420 6775 6172  ut I cannot guar
+000026f0: 616e 7465 6520 7468 6174 2069 7420 7769  antee that it wi
+00002700: 6c6c 2061 6c77 6179 7320 776f 726b 2070  ll always work p
+00002710: 6572 6665 6374 6c79 2e20 4d65 616e 7768  erfectly. Meanwh
+00002720: 696c 652c 2079 6f75 2073 686f 756c 6420  ile, you should 
+00002730: 2266 6169 7220 7573 6522 2074 6865 2062  "fair use" the b
+00002740: 6f74 2c20 6176 6f69 6420 7375 6273 6372  ot, avoid subscr
+00002750: 6962 696e 6720 746f 2074 6f6f 206d 616e  ibing to too man
+00002760: 7920 5253 5320 6665 6564 732e 2020 0a49  y RSS feeds.  .I
+00002770: 6620 796f 7520 7573 6520 7468 6520 5b70  f you use the [p
+00002780: 7562 6c69 6320 626f 745d 2868 7474 7073  ublic bot](https
+00002790: 3a2f 2f74 2e6d 652f 5253 5374 545f 426f  ://t.me/RSStT_Bo
+000027a0: 7429 2069 6e20 796f 7572 2043 6861 6e6e  t) in your Chann
+000027b0: 656c 2c20 636f 6e73 6964 6572 206d 656e  el, consider men
+000027c0: 7469 6f6e 696e 6720 7468 6520 626f 7420  tioning the bot 
+000027d0: 286f 7220 7468 6973 2070 726f 6a65 6374  (or this project
+000027e0: 2920 696e 2079 6f75 7220 6368 616e 6e65  ) in your channe
+000027f0: 6c20 6465 7363 7269 7074 696f 6e20 286f  l description (o
+00002800: 7220 7069 6e6e 6564 206d 6573 7361 6765  r pinned message
+00002810: 2920 746f 206c 6574 206d 6f72 6520 7065  ) to let more pe
+00002820: 6f70 6c65 206b 6e6f 7720 6162 6f75 7420  ople know about 
+00002830: 6974 2e20 5468 6174 2773 206e 6f74 2061  it. That's not a
+00002840: 2063 6f6d 7075 6c73 696f 6e2e 0a0a 2323   compulsion...##
+00002850: 204b 6e6f 776e 2063 6861 6e6e 656c 7320   Known channels 
+00002860: 7573 696e 6720 5253 5374 540a 0a57 616e  using RSStT..Wan
+00002870: 7420 746f 2070 7265 7669 6577 2077 6861  t to preview wha
+00002880: 7420 7468 6520 6d65 7373 6167 6573 2073  t the messages s
+00002890: 656e 7420 6279 2052 5353 7454 206c 6f6f  ent by RSStT loo
+000028a0: 6b20 6c69 6b65 3f20 4865 7265 2069 7320  k like? Here is 
+000028b0: 6120 5b6c 6973 7420 6f66 2063 6861 6e6e  a [list of chann
+000028c0: 656c 7320 7573 696e 6720 5253 5374 545d  els using RSStT]
+000028d0: 2864 6f63 732f 6368 616e 6e65 6c73 2d75  (docs/channels-u
+000028e0: 7369 6e67 2d72 7373 7474 2e6d 6429 2e0a  sing-rsstt.md)..
+000028f0: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
+00002900: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
+00002910: 656e 7365 6420 756e 6465 7220 5b41 4750  ensed under [AGP
+00002920: 4c76 335d 284c 4943 454e 5345 292e 2043  Lv3](LICENSE). C
+00002930: 6c6f 7365 642d 736f 7572 6365 2064 6973  losed-source dis
+00002940: 7472 6962 7574 696f 6e20 6f72 2062 6f74  tribution or bot
+00002950: 2d68 6f73 7469 6e67 2061 7265 2073 7472  -hosting are str
+00002960: 6963 746c 7920 7072 6f68 6962 6974 6564  ictly prohibited
+00002970: 2e20 4966 2079 6f75 206d 6f64 6966 7920  . If you modify 
+00002980: 7468 6520 636f 6465 2061 6e64 2064 6973  the code and dis
+00002990: 7472 6962 7574 6520 6f72 2068 6f73 7420  tribute or host 
+000029a0: 6974 2c20 6d61 6b65 2073 7572 6520 616e  it, make sure an
+000029b0: 7920 7573 6572 7320 7768 6f20 6361 6e20  y users who can 
+000029c0: 7573 6520 796f 7572 2062 6f74 2063 616e  use your bot can
+000029d0: 2067 6574 2074 6865 2073 6f75 7263 6520   get the source 
+000029e0: 636f 6465 2028 6279 2065 6469 7469 6e67  code (by editing
+000029f0: 2074 6865 2072 6570 6f20 5552 4c20 696e   the repo URL in
+00002a00: 205b 6073 7263 2f69 3138 6e2f 5f5f 696e   [`src/i18n/__in
+00002a10: 6974 5f5f 2e70 7960 5d28 7372 632f 6931  it__.py`](src/i1
+00002a20: 386e 2f5f 5f69 6e69 745f 5f2e 7079 2929  8n/__init__.py))
+00002a30: 2e0a 0a54 6865 2072 6570 6f73 6974 6f72  ...The repositor
+00002a40: 7920 7761 7320 666f 726d 6572 6c79 2061  y was formerly a
+00002a50: 2066 6f72 6b20 6f66 205b 426f 4b4b 6552   fork of [BoKKeR
+00002a60: 2f52 5353 2d74 6f2d 5465 6c65 6772 616d  /RSS-to-Telegram
+00002a70: 2d42 6f74 5d28 6874 7470 733a 2f2f 6769  -Bot](https://gi
+00002a80: 7468 7562 2e63 6f6d 2f42 6f4b 4b65 522f  thub.com/BoKKeR/
+00002a90: 5253 532d 746f 2d54 656c 6567 7261 6d2d  RSS-to-Telegram-
+00002aa0: 426f 7429 2e20 5468 6579 2068 6176 6520  Bot). They have 
+00002ab0: 6265 656e 2065 6e74 6972 656c 7920 6469  been entirely di
+00002ac0: 6666 6572 656e 7420 7072 6f6a 6563 7473  fferent projects
+00002ad0: 2073 696e 6365 2074 6865 2065 6172 6c79   since the early
+00002ae0: 2064 6179 7320 6f66 2074 6869 7320 7072   days of this pr
+00002af0: 6f6a 6563 742e 0a                        oject..
```

### Comparing `rsstt-2.6.0/README.md` & `rsstt-2.7.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,47 @@
-<a href="https://t.me/RSStT_Bot"><img width="150" height="150" align="left" style="float: left; margin: 0 10px 0 0;" alt="RSStT icon" src="docs/resources/RSStT_icon.svg"/><a/>
+<p align="center">
+<img src="docs/resources/RSStT_icon.svg" alt="RSS to Telegram Bot" width="100">
+</p>
+<h1 align="center">RSS to Telegram Bot</h1>
 
-# [RSS to Telegram Bot](https://t.me/RSStT_Bot)
-
-**A Telegram RSS bot that cares about your reading experience**
-
-[简体中文 README](README.zh.md)
+<p align="center"><b>A Telegram RSS bot that cares about your reading experience</b></p>
 
 [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/Rongronggg9/RSS-to-Telegram-Bot?logo=git&label=commit)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/commits)
 [![Translating status](https://img.shields.io/weblate/progress/rss-to-telegram-bot?logo=weblate&color=informational)](https://hosted.weblate.org/engage/rss-to-telegram-bot/)
 [![Code quality](https://img.shields.io/codefactor/grade/github/Rongronggg9/RSS-to-Telegram-Bot?logo=codefactor)](https://www.codefactor.io/repository/github/rongronggg9/rss-to-telegram-bot)
 [![GitHub stars](https://img.shields.io/github/stars/Rongronggg9/Rss-to-Telegram-Bot?style=social)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/Rongronggg9/RSS-to-Telegram-Bot?style=social)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/fork)
 
-[![Telegram bot](https://img.shields.io/badge/bot-%40RSStT__Bot-229ed9?logo=telegram&style=for-the-badge)](https://t.me/RSStT_Bot)
-[![Telegram group](https://img.shields.io/badge/chat-%40RSStT__Group-229ed9?logo=telegram&style=for-the-badge)](https://t.me/RSStT_Group)
-[![Telegram channel](https://img.shields.io/badge/channel-%40RSStT__Channel-229ed9?logo=telegram&style=for-the-badge)](https://t.me/RSStT_Channel)
+[![Telegram bot](https://img.shields.io/badge/Telegram%20Bot-%40RSStT__Bot-229ed9?logo=telegram&style=for-the-badge)](https://t.me/RSStT_Bot)
+[![Telegram group](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.swo.moe%2Fstats%2Ftelegram%2FRSStT_Group&query=count&color=2CA5E0&label=Telegram%20Group&logo=telegram&cacheSeconds=3600&style=for-the-badge)](https://t.me/RSStT_Group)
+[![Telegram channel](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.swo.moe%2Fstats%2Ftelegram%2FRSStT_Channel&query=count&color=2CA5E0&label=Telegram%20Channel&logo=telegram&cacheSeconds=3600&style=for-the-badge)](https://t.me/RSStT_Channel)
+
+| [简体中文 README] | [CHANGELOG] | [FAQ] | [Documentation] | [Channels Using RSStT] |
+|:-------------:|:-----------:|:-----:|-----------------|:----------------------:|
 
-| [CHANGELOG] | [FAQ] | [Documentation] | [Channels Using RSStT] |
-|:-----------:|:-----:|-----------------|:----------------------:|
+[简体中文 README]: README.zh.md
 
 [CHANGELOG]: docs/CHANGELOG.md
 
 [FAQ]: docs/FAQ.md
 
 [Documentation]: docs
 
 [Channels Using RSStT]: docs/channels-using-rsstt.md
 
-
-**Important**: If you have your own RSStT bot (v1), please read the [migration guide](docs/migration-guide-v2.md) to learn how to migrate to v2.
+<table>
+    <tr>
+        <td><img src="docs/resources/example5.png" alt="Screenshot"></td>
+        <td rowspan="2"><img src="docs/resources/example7.png" alt="Screenshot"></td>
+        <td rowspan="2"><img src="docs/resources/example8.png" alt="Screenshot"></td>
+    </tr>
+    <tr>
+        <td><img src="docs/resources/example6.png" alt="Screenshot"></td>
+    </tr>
+</table>
 
 ## Highlights
 
 - Multi-user
 - I18n
     - English, Chinese, Cantonese, Italian, and [more](docs/translation-guide.md)!
 - The content of the posts of an RSS feed will be sent to Telegram
@@ -42,39 +51,38 @@
         - Long images will be sent as files to prevent Telegram from compressing the image and making it unreadable
         - Drop annoying icons, they break the reading experience
     - Automatically replace emoji shortcodes with emoji
     - Automatically replace emoji images with emoji or its description text
     - Automatically determine whether the title of the RSS feed is auto-filled, if so, omit the title (customizable)
     - Automatically show the author-name (customizable)
     - Automatically split too-long messages
-        - If configured Telegraph, the message will be sent via Telegraph (customizable)
+    - Messages can be sent as Telegraph posts (customizable)
+      - Most images and videos will be uploaded to Telegraph, so that Instant View will load rapidly
 - [Various customizable formatting settings](docs/formatting-settings.md)
     - Hashtags, custom title, etc.
 - Individual proxy settings for Telegram and RSS feeds
 - OPML importing and exporting (keep custom title)
 - Optimized performance (see also the [FAQ](docs/FAQ.md#q-how-is-the-performance-of-the-bot))
 - User-friendly
 - HTTP Caching
 
-<img src="docs/resources/example1.png" width = "300" alt=""/><img src="docs/resources/example3.png" width = "300" alt=""/><img src="docs/resources/example4.png" width = "300" alt=""/>
-
 ## Deployment
 
-[![PyPI](https://img.shields.io/pypi/v/rsstt?logo=pypi&logoColor=white)](https://pypi.org/project/rsstt/)
-[![PyPI publish status](https://img.shields.io/github/actions/workflow/status/Rongronggg9/RSS-to-Telegram-Bot/publish-to-pypi.yml?label=publish&logo=pypi&logoColor=white)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-to-pypi.yml)
-[![TestPyPI publish status](https://img.shields.io/github/actions/workflow/status/Rongronggg9/RSS-to-Telegram-Bot/publish-to-test-pypi.yml?label=publish%20(TestPyPI)&logo=pypi&logoColor=white)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-to-pypi.yml)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/rsstt?logo=pypi&logoColor=white)](https://pypi.org/project/rsstt/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rsstt?logo=python&label=&labelColor=white)](https://www.python.org)
-
-[![Docker Image Size (tag)](https://img.shields.io/docker/image-size/rongronggg9/rss-to-telegram/latest?logo=docker)](https://hub.docker.com/r/rongronggg9/rss-to-telegram)
+[![dockeri.co](https://dockerico.blankenship.io/image/rongronggg9/rss-to-telegram)](https://hub.docker.com/r/rongronggg9/rss-to-telegram)\
 [![Build status (master)](https://img.shields.io/github/actions/workflow/status/Rongronggg9/RSS-to-Telegram-Bot/publish-docker-image.yml?branch=master&label=build&logo=docker)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-docker-image.yml?query=branch%3Amaster)
 [![Build status (dev)](https://img.shields.io/github/actions/workflow/status/Rongronggg9/RSS-to-Telegram-Bot/publish-docker-image.yml?branch=dev&label=build%20%28dev%29&logo=docker)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-docker-image.yml?query=branch%3Adev)
-[![Docker pulls](https://img.shields.io/docker/pulls/rongronggg9/rss-to-telegram?label=pulls&logo=docker&color=informational)](https://hub.docker.com/r/rongronggg9/rss-to-telegram)
 
-It is quite easy to deploy your RSStT instance. The most recommended way to deploy RSStT is Docker Compose: it is suitable for virtually all VPS. [Railway.app](https://railway.app) (a PaaS platform) is also officially supported. You may also install RSStT from PyPI (tracking `master` branch) or TestPyPI (tracking `dev` branch, which is latest) using pip. For developers or experienced users, dirty run from source is also an option.
+[![PyPI](https://img.shields.io/pypi/v/rsstt?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/rsstt/)
+[![TestPyPI](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Ftest.pypi.org%2Fpypi%2Frsstt%2Fjson&query=%24.info.version&prefix=v&logo=pypi&logoColor=white&label=TestPyPI)](https://test.pypi.org/project/rsstt/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rsstt?logo=python&label=&labelColor=white)](https://www.python.org)\
+[![PyPI publish status](https://img.shields.io/github/actions/workflow/status/Rongronggg9/RSS-to-Telegram-Bot/publish-to-pypi.yml?label=publish&logo=pypi&logoColor=white)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-to-pypi.yml)
+[![TestPyPI publish status](https://img.shields.io/github/actions/workflow/status/Rongronggg9/RSS-to-Telegram-Bot/publish-to-test-pypi.yml?label=publish%20(TestPyPI)&logo=pypi&logoColor=white)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-to-test-pypi.yml)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/rsstt?logo=pypi&logoColor=white)](https://pypi.org/project/rsstt/)
+
+It is quite easy to deploy your RSStT instance. The most recommended way to deploy RSStT is Docker Compose: it is suitable for virtually all VPS. [Railway.app](https://railway.app) (a PaaS platform) is also officially supported. You may also install RSStT from [PyPI](https://pypi.org/project/rsstt/) (tracking `master` branch) or [TestPyPI](https://test.pypi.org/project/rsstt/) (tracking `dev` branch, which is always up-to-date) using pip. For developers or experienced users, dirty run from source is also an option.
 
 <a href="docs/deployment-guide.md#option-2-railwayapp"><img src="https://railway.app/button.svg" height="30" alt="Deploy on Railway"></a>
 
 For more details, refer to the [deployment guide](docs/deployment-guide.md).
 
 ## Translation
```

#### html2text {}

```diff
@@ -1,94 +1,99 @@
-_[_R_S_S_t_T_ _i_c_o_n_]
-_#_ _[_R_S_S_ _t_o_ _T_e_l_e_g_r_a_m_ _B_o_t_]_(_h_t_t_p_s_:_/_/_t_._m_e_/_R_S_S_t_T___B_o_t_)_ _*_*_A_ _T_e_l_e_g_r_a_m_ _R_S_S_ _b_o_t_ _t_h_a_t_ _c_a_r_e_s
-_a_b_o_u_t_ _y_o_u_r_ _r_e_a_d_i_n_g_ _e_x_p_e_r_i_e_n_c_e_*_*_ _[_ç_®__ä_½__ä_¸_­_æ___ _R_E_A_D_M_E_]_(_R_E_A_D_M_E_._z_h_._m_d_)_ _[_!_[_G_i_t_H_u_b
-_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_m_m_i_t_-_a_c_t_i_v_i_t_y_/_m_/_R_o_n_g_r_o_n_g_g_g_9_/
-_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_?_l_o_g_o_=_g_i_t_&_l_a_b_e_l_=_c_o_m_m_i_t_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-
-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_c_o_m_m_i_t_s_)_ _[_!_[_T_r_a_n_s_l_a_t_i_n_g_ _s_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_w_e_b_l_a_t_e_/
-_p_r_o_g_r_e_s_s_/_r_s_s_-_t_o_-_t_e_l_e_g_r_a_m_-_b_o_t_?_l_o_g_o_=_w_e_b_l_a_t_e_&_c_o_l_o_r_=_i_n_f_o_r_m_a_t_i_o_n_a_l_)_]_(_h_t_t_p_s_:_/_/
-_h_o_s_t_e_d_._w_e_b_l_a_t_e_._o_r_g_/_e_n_g_a_g_e_/_r_s_s_-_t_o_-_t_e_l_e_g_r_a_m_-_b_o_t_/_)_ _[_!_[_C_o_d_e_ _q_u_a_l_i_t_y_]_(_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-
-_B_o_t_?_l_o_g_o_=_c_o_d_e_f_a_c_t_o_r_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._c_o_d_e_f_a_c_t_o_r_._i_o_/_r_e_p_o_s_i_t_o_r_y_/_g_i_t_h_u_b_/_r_o_n_g_r_o_n_g_g_g_9_/
-_r_s_s_-_t_o_-_t_e_l_e_g_r_a_m_-_b_o_t_)_ _[_!_[_G_i_t_H_u_b_ _s_t_a_r_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/
-_R_o_n_g_r_o_n_g_g_g_9_/_R_s_s_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_?_s_t_y_l_e_=_s_o_c_i_a_l_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_R_o_n_g_r_o_n_g_g_g_9_/
-_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_s_t_a_r_g_a_z_e_r_s_)_ _[_!_[_G_i_t_H_u_b_ _f_o_r_k_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
-_f_o_r_k_s_/_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_?_s_t_y_l_e_=_s_o_c_i_a_l_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
-_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_f_o_r_k_)_ _[_!_[_T_e_l_e_g_r_a_m_ _b_o_t_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_b_a_d_g_e_/_b_o_t_-_%_4_0_R_S_S_t_T_____B_o_t_-_2_2_9_e_d_9_?_l_o_g_o_=_t_e_l_e_g_r_a_m_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_)_]_(_h_t_t_p_s_:_/_/
-_t_._m_e_/_R_S_S_t_T___B_o_t_)_ _[_!_[_T_e_l_e_g_r_a_m_ _g_r_o_u_p_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_t_-
-_%_4_0_R_S_S_t_T_____G_r_o_u_p_-_2_2_9_e_d_9_?_l_o_g_o_=_t_e_l_e_g_r_a_m_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_)_]_(_h_t_t_p_s_:_/_/_t_._m_e_/
-_R_S_S_t_T___G_r_o_u_p_)_ _[_!_[_T_e_l_e_g_r_a_m_ _c_h_a_n_n_e_l_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_n_n_e_l_-
-_%_4_0_R_S_S_t_T_____C_h_a_n_n_e_l_-_2_2_9_e_d_9_?_l_o_g_o_=_t_e_l_e_g_r_a_m_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_)_]_(_h_t_t_p_s_:_/_/_t_._m_e_/
-_R_S_S_t_T___C_h_a_n_n_e_l_)_ _|_ _[_C_H_A_N_G_E_L_O_G_]_ _|_ _[_F_A_Q_]_ _|_ _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_ _|_ _[_C_h_a_n_n_e_l_s_ _U_s_i_n_g_ _R_S_S_t_T_]
-_|_ _|_:_-_-_-_-_-_-_-_-_-_-_-_:_|_:_-_-_-_-_-_:_|_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_|_:_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_:_|
-_[_C_H_A_N_G_E_L_O_G_]_:_ _d_o_c_s_/_C_H_A_N_G_E_L_O_G_._m_d_ _[_F_A_Q_]_:_ _d_o_c_s_/_F_A_Q_._m_d_ _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_:_ _d_o_c_s
-_[_C_h_a_n_n_e_l_s_ _U_s_i_n_g_ _R_S_S_t_T_]_:_ _d_o_c_s_/_c_h_a_n_n_e_l_s_-_u_s_i_n_g_-_r_s_s_t_t_._m_d_ _*_*_I_m_p_o_r_t_a_n_t_*_*_:_ _I_f_ _y_o_u_ _h_a_v_e
-_y_o_u_r_ _o_w_n_ _R_S_S_t_T_ _b_o_t_ _(_v_1_)_,_ _p_l_e_a_s_e_ _r_e_a_d_ _t_h_e_ _[_m_i_g_r_a_t_i_o_n_ _g_u_i_d_e_]_(_d_o_c_s_/_m_i_g_r_a_t_i_o_n_-
-_g_u_i_d_e_-_v_2_._m_d_)_ _t_o_ _l_e_a_r_n_ _h_o_w_ _t_o_ _m_i_g_r_a_t_e_ _t_o_ _v_2_._ _#_#_ _H_i_g_h_l_i_g_h_t_s_ _-_ _M_u_l_t_i_-_u_s_e_r_ _-_ _I_1_8_n_ _-
-_E_n_g_l_i_s_h_,_ _C_h_i_n_e_s_e_,_ _C_a_n_t_o_n_e_s_e_,_ _I_t_a_l_i_a_n_,_ _a_n_d_ _[_m_o_r_e_]_(_d_o_c_s_/_t_r_a_n_s_l_a_t_i_o_n_-_g_u_i_d_e_._m_d_)_!_ _-
-_T_h_e_ _c_o_n_t_e_n_t_ _o_f_ _t_h_e_ _p_o_s_t_s_ _o_f_ _a_n_ _R_S_S_ _f_e_e_d_ _w_i_l_l_ _b_e_ _s_e_n_t_ _t_o_ _T_e_l_e_g_r_a_m_ _-_ _K_e_e_p_ _r_i_c_h_-
-_t_e_x_t_ _f_o_r_m_a_t_ _-_ _K_e_e_p_ _m_e_d_i_a_ _(_c_u_s_t_o_m_i_z_a_b_l_e_)_ _-_ _I_m_a_g_e_s_,_ _V_i_d_e_o_s_,_ _a_n_d_ _A_u_d_i_o_ _b_o_t_h_ _i_n_ _t_h_e
-_p_o_s_t_ _c_o_n_t_e_n_t_ _a_n_d_ _e_n_c_l_o_s_u_r_e_;_ _D_o_c_u_m_e_n_t_s_ _i_n_ _t_h_e_ _p_o_s_t_ _e_n_c_l_o_s_u_r_e_ _-_ _L_o_n_g_ _i_m_a_g_e_s_ _w_i_l_l
-_b_e_ _s_e_n_t_ _a_s_ _f_i_l_e_s_ _t_o_ _p_r_e_v_e_n_t_ _T_e_l_e_g_r_a_m_ _f_r_o_m_ _c_o_m_p_r_e_s_s_i_n_g_ _t_h_e_ _i_m_a_g_e_ _a_n_d_ _m_a_k_i_n_g_ _i_t
-_u_n_r_e_a_d_a_b_l_e_ _-_ _D_r_o_p_ _a_n_n_o_y_i_n_g_ _i_c_o_n_s_,_ _t_h_e_y_ _b_r_e_a_k_ _t_h_e_ _r_e_a_d_i_n_g_ _e_x_p_e_r_i_e_n_c_e_ _-
-_A_u_t_o_m_a_t_i_c_a_l_l_y_ _r_e_p_l_a_c_e_ _e_m_o_j_i_ _s_h_o_r_t_c_o_d_e_s_ _w_i_t_h_ _e_m_o_j_i_ _-_ _A_u_t_o_m_a_t_i_c_a_l_l_y_ _r_e_p_l_a_c_e_ _e_m_o_j_i
-_i_m_a_g_e_s_ _w_i_t_h_ _e_m_o_j_i_ _o_r_ _i_t_s_ _d_e_s_c_r_i_p_t_i_o_n_ _t_e_x_t_ _-_ _A_u_t_o_m_a_t_i_c_a_l_l_y_ _d_e_t_e_r_m_i_n_e_ _w_h_e_t_h_e_r_ _t_h_e
-_t_i_t_l_e_ _o_f_ _t_h_e_ _R_S_S_ _f_e_e_d_ _i_s_ _a_u_t_o_-_f_i_l_l_e_d_,_ _i_f_ _s_o_,_ _o_m_i_t_ _t_h_e_ _t_i_t_l_e_ _(_c_u_s_t_o_m_i_z_a_b_l_e_)_ _-
-_A_u_t_o_m_a_t_i_c_a_l_l_y_ _s_h_o_w_ _t_h_e_ _a_u_t_h_o_r_-_n_a_m_e_ _(_c_u_s_t_o_m_i_z_a_b_l_e_)_ _-_ _A_u_t_o_m_a_t_i_c_a_l_l_y_ _s_p_l_i_t_ _t_o_o_-
-_l_o_n_g_ _m_e_s_s_a_g_e_s_ _-_ _I_f_ _c_o_n_f_i_g_u_r_e_d_ _T_e_l_e_g_r_a_p_h_,_ _t_h_e_ _m_e_s_s_a_g_e_ _w_i_l_l_ _b_e_ _s_e_n_t_ _v_i_a_ _T_e_l_e_g_r_a_p_h
-_(_c_u_s_t_o_m_i_z_a_b_l_e_)_ _-_ _[_V_a_r_i_o_u_s_ _c_u_s_t_o_m_i_z_a_b_l_e_ _f_o_r_m_a_t_t_i_n_g_ _s_e_t_t_i_n_g_s_]_(_d_o_c_s_/_f_o_r_m_a_t_t_i_n_g_-
-_s_e_t_t_i_n_g_s_._m_d_)_ _-_ _H_a_s_h_t_a_g_s_,_ _c_u_s_t_o_m_ _t_i_t_l_e_,_ _e_t_c_._ _-_ _I_n_d_i_v_i_d_u_a_l_ _p_r_o_x_y_ _s_e_t_t_i_n_g_s_ _f_o_r
-_T_e_l_e_g_r_a_m_ _a_n_d_ _R_S_S_ _f_e_e_d_s_ _-_ _O_P_M_L_ _i_m_p_o_r_t_i_n_g_ _a_n_d_ _e_x_p_o_r_t_i_n_g_ _(_k_e_e_p_ _c_u_s_t_o_m_ _t_i_t_l_e_)_ _-
-_O_p_t_i_m_i_z_e_d_ _p_e_r_f_o_r_m_a_n_c_e_ _(_s_e_e_ _a_l_s_o_ _t_h_e_ _[_F_A_Q_]_(_d_o_c_s_/_F_A_Q_._m_d_#_q_-_h_o_w_-_i_s_-_t_h_e_-_p_e_r_f_o_r_m_a_n_c_e_-
-_o_f_-_t_h_e_-_b_o_t_)_)_ _-_ _U_s_e_r_-_f_r_i_e_n_d_l_y_ _-_ _H_T_T_P_ _C_a_c_h_i_n_g_ _#_#_ _D_e_p_l_o_y_m_e_n_t_ _[_!_[_P_y_P_I_]_(_h_t_t_p_s_:_/_/
-_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_r_s_s_t_t_?_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_)_]_(_h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/
-_p_r_o_j_e_c_t_/_r_s_s_t_t_/_)_ _[_!_[_P_y_P_I_ _p_u_b_l_i_s_h_ _s_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/
-_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_p_u_b_l_i_s_h_-_t_o_-
-_p_y_p_i_._y_m_l_?_l_a_b_e_l_=_p_u_b_l_i_s_h_&_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
-_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_u_b_l_i_s_h_-_t_o_-_p_y_p_i_._y_m_l_)_ _[_!
-_[_T_e_s_t_P_y_P_I_ _p_u_b_l_i_s_h_ _s_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/
-_s_t_a_t_u_s_/_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_p_u_b_l_i_s_h_-_t_o_-_t_e_s_t_-
-_p_y_p_i_._y_m_l_?_l_a_b_e_l_=_p_u_b_l_i_s_h_%_2_0_(_T_e_s_t_P_y_P_I_)_&_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_)_]_(_h_t_t_p_s_:_/_/
-_g_i_t_h_u_b_._c_o_m_/_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_u_b_l_i_s_h_-_t_o_-
-_p_y_p_i_._y_m_l_)_ _[_!_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/
-_r_s_s_t_t_?_l_o_g_o_=_p_y_p_i_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_)_]_(_h_t_t_p_s_:_/_/_p_y_p_i_._o_r_g_/_p_r_o_j_e_c_t_/_r_s_s_t_t_/_)_ _[_!_[_P_y_P_I_ _-
-_P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/
-_r_s_s_t_t_?_l_o_g_o_=_p_y_t_h_o_n_&_l_a_b_e_l_=_&_l_a_b_e_l_C_o_l_o_r_=_w_h_i_t_e_)_]_(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_)_ _[_!_[_D_o_c_k_e_r
-_I_m_a_g_e_ _S_i_z_e_ _(_t_a_g_)_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_k_e_r_/_i_m_a_g_e_-_s_i_z_e_/_r_o_n_g_r_o_n_g_g_g_9_/_r_s_s_-_t_o_-
-_t_e_l_e_g_r_a_m_/_l_a_t_e_s_t_?_l_o_g_o_=_d_o_c_k_e_r_)_]_(_h_t_t_p_s_:_/_/_h_u_b_._d_o_c_k_e_r_._c_o_m_/_r_/_r_o_n_g_r_o_n_g_g_g_9_/_r_s_s_-_t_o_-
-_t_e_l_e_g_r_a_m_)_ _[_!_[_B_u_i_l_d_ _s_t_a_t_u_s_ _(_m_a_s_t_e_r_)_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/
-_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_p_u_b_l_i_s_h_-_d_o_c_k_e_r_-
-_i_m_a_g_e_._y_m_l_?_b_r_a_n_c_h_=_m_a_s_t_e_r_&_l_a_b_e_l_=_b_u_i_l_d_&_l_o_g_o_=_d_o_c_k_e_r_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
-_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_u_b_l_i_s_h_-_d_o_c_k_e_r_-
-_i_m_a_g_e_._y_m_l_?_q_u_e_r_y_=_b_r_a_n_c_h_%_3_A_m_a_s_t_e_r_)_ _[_!_[_B_u_i_l_d_ _s_t_a_t_u_s_ _(_d_e_v_)_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_p_u_b_l_i_s_h_-_d_o_c_k_e_r_-
-_i_m_a_g_e_._y_m_l_?_b_r_a_n_c_h_=_d_e_v_&_l_a_b_e_l_=_b_u_i_l_d_%_2_0_%_2_8_d_e_v_%_2_9_&_l_o_g_o_=_d_o_c_k_e_r_)_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/
-_R_o_n_g_r_o_n_g_g_g_9_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_p_u_b_l_i_s_h_-_d_o_c_k_e_r_-
-_i_m_a_g_e_._y_m_l_?_q_u_e_r_y_=_b_r_a_n_c_h_%_3_A_d_e_v_)_ _[_!_[_D_o_c_k_e_r_ _p_u_l_l_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_o_c_k_e_r_/
-_p_u_l_l_s_/_r_o_n_g_r_o_n_g_g_g_9_/_r_s_s_-_t_o_-_t_e_l_e_g_r_a_m_?_l_a_b_e_l_=_p_u_l_l_s_&_l_o_g_o_=_d_o_c_k_e_r_&_c_o_l_o_r_=_i_n_f_o_r_m_a_t_i_o_n_a_l_)_]
-_(_h_t_t_p_s_:_/_/_h_u_b_._d_o_c_k_e_r_._c_o_m_/_r_/_r_o_n_g_r_o_n_g_g_g_9_/_r_s_s_-_t_o_-_t_e_l_e_g_r_a_m_)_ _I_t_ _i_s_ _q_u_i_t_e_ _e_a_s_y_ _t_o
-_d_e_p_l_o_y_ _y_o_u_r_ _R_S_S_t_T_ _i_n_s_t_a_n_c_e_._ _T_h_e_ _m_o_s_t_ _r_e_c_o_m_m_e_n_d_e_d_ _w_a_y_ _t_o_ _d_e_p_l_o_y_ _R_S_S_t_T_ _i_s_ _D_o_c_k_e_r
-_C_o_m_p_o_s_e_:_ _i_t_ _i_s_ _s_u_i_t_a_b_l_e_ _f_o_r_ _v_i_r_t_u_a_l_l_y_ _a_l_l_ _V_P_S_._ _[_R_a_i_l_w_a_y_._a_p_p_]_(_h_t_t_p_s_:_/_/
-_r_a_i_l_w_a_y_._a_p_p_)_ _(_a_ _P_a_a_S_ _p_l_a_t_f_o_r_m_)_ _i_s_ _a_l_s_o_ _o_f_f_i_c_i_a_l_l_y_ _s_u_p_p_o_r_t_e_d_._ _Y_o_u_ _m_a_y_ _a_l_s_o
-_i_n_s_t_a_l_l_ _R_S_S_t_T_ _f_r_o_m_ _P_y_P_I_ _(_t_r_a_c_k_i_n_g_ _`_m_a_s_t_e_r_`_ _b_r_a_n_c_h_)_ _o_r_ _T_e_s_t_P_y_P_I_ _(_t_r_a_c_k_i_n_g_ _`_d_e_v_`
-_b_r_a_n_c_h_,_ _w_h_i_c_h_ _i_s_ _l_a_t_e_s_t_)_ _u_s_i_n_g_ _p_i_p_._ _F_o_r_ _d_e_v_e_l_o_p_e_r_s_ _o_r_ _e_x_p_e_r_i_e_n_c_e_d_ _u_s_e_r_s_,_ _d_i_r_t_y
-_r_u_n_ _f_r_o_m_ _s_o_u_r_c_e_ _i_s_ _a_l_s_o_ _a_n_ _o_p_t_i_o_n_._ _[_D_e_p_l_o_y_ _o_n_ _R_a_i_l_w_a_y_]_F_o_r_ _m_o_r_e_ _d_e_t_a_i_l_s_,_ _r_e_f_e_r
-_t_o_ _t_h_e_ _[_d_e_p_l_o_y_m_e_n_t_ _g_u_i_d_e_]_(_d_o_c_s_/_d_e_p_l_o_y_m_e_n_t_-_g_u_i_d_e_._m_d_)_._ _#_#_ _T_r_a_n_s_l_a_t_i_o_n_ _R_e_a_d_ _t_h_e
-_t_r_a_n_s_l_a_t_i_o_n_ _g_u_i_d_e_ _[_h_e_r_e_]_(_d_o_c_s_/_t_r_a_n_s_l_a_t_i_o_n_-_g_u_i_d_e_._m_d_)_._ _Y_o_u_ _c_a_n_ _h_e_l_p_ _t_o_ _t_r_a_n_s_l_a_t_e
-_t_h_e_ _b_o_t_ _u_s_i_n_g_ _[_H_o_s_t_e_d_ _W_e_b_l_a_t_e_]_(_h_t_t_p_s_:_/_/_h_o_s_t_e_d_._w_e_b_l_a_t_e_._o_r_g_/_p_r_o_j_e_c_t_s_/_r_s_s_-_t_o_-
-_t_e_l_e_g_r_a_m_-_b_o_t_/_)_._ _S_p_e_c_i_a_l_ _t_h_a_n_k_s_ _t_o_ _t_h_e_i_r_ _f_r_e_e_ _h_o_s_t_i_n_g_ _s_e_r_v_i_c_e_ _f_o_r_ _l_i_b_r_e
-_p_r_o_j_e_c_t_s_!_ _#_#_ _U_s_i_n_g_ _t_h_e_ _p_u_b_l_i_c_ _b_o_t_ _T_h_e_ _[_p_u_b_l_i_c_ _b_o_t_]_(_h_t_t_p_s_:_/_/_t_._m_e_/_R_S_S_t_T___B_o_t_)
-_c_o_m_e_s_ _w_i_t_h_ _a_b_s_o_l_u_t_e_l_y_ _n_o_ _w_a_r_r_a_n_t_y_._ _I_ _w_i_l_l_ _t_r_y_ _m_y_ _b_e_s_t_ _t_o_ _m_a_i_n_t_a_i_n_ _i_t_,_ _b_u_t_ _I
-_c_a_n_n_o_t_ _g_u_a_r_a_n_t_e_e_ _t_h_a_t_ _i_t_ _w_i_l_l_ _a_l_w_a_y_s_ _w_o_r_k_ _p_e_r_f_e_c_t_l_y_._ _M_e_a_n_w_h_i_l_e_,_ _y_o_u_ _s_h_o_u_l_d
-_"_f_a_i_r_ _u_s_e_"_ _t_h_e_ _b_o_t_,_ _a_v_o_i_d_ _s_u_b_s_c_r_i_b_i_n_g_ _t_o_ _t_o_o_ _m_a_n_y_ _R_S_S_ _f_e_e_d_s_._ _I_f_ _y_o_u_ _u_s_e_ _t_h_e
-_[_p_u_b_l_i_c_ _b_o_t_]_(_h_t_t_p_s_:_/_/_t_._m_e_/_R_S_S_t_T___B_o_t_)_ _i_n_ _y_o_u_r_ _C_h_a_n_n_e_l_,_ _c_o_n_s_i_d_e_r_ _m_e_n_t_i_o_n_i_n_g_ _t_h_e
-_b_o_t_ _(_o_r_ _t_h_i_s_ _p_r_o_j_e_c_t_)_ _i_n_ _y_o_u_r_ _c_h_a_n_n_e_l_ _d_e_s_c_r_i_p_t_i_o_n_ _(_o_r_ _p_i_n_n_e_d_ _m_e_s_s_a_g_e_)_ _t_o_ _l_e_t
-_m_o_r_e_ _p_e_o_p_l_e_ _k_n_o_w_ _a_b_o_u_t_ _i_t_._ _T_h_a_t_'_s_ _n_o_t_ _a_ _c_o_m_p_u_l_s_i_o_n_._ _#_#_ _K_n_o_w_n_ _c_h_a_n_n_e_l_s_ _u_s_i_n_g
-_R_S_S_t_T_ _W_a_n_t_ _t_o_ _p_r_e_v_i_e_w_ _w_h_a_t_ _t_h_e_ _m_e_s_s_a_g_e_s_ _s_e_n_t_ _b_y_ _R_S_S_t_T_ _l_o_o_k_ _l_i_k_e_?_ _H_e_r_e_ _i_s_ _a
-_[_l_i_s_t_ _o_f_ _c_h_a_n_n_e_l_s_ _u_s_i_n_g_ _R_S_S_t_T_]_(_d_o_c_s_/_c_h_a_n_n_e_l_s_-_u_s_i_n_g_-_r_s_s_t_t_._m_d_)_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s
-_p_r_o_j_e_c_t_ _i_s_ _l_i_c_e_n_s_e_d_ _u_n_d_e_r_ _[_A_G_P_L_v_3_]_(_L_I_C_E_N_S_E_)_._ _C_l_o_s_e_d_-_s_o_u_r_c_e_ _d_i_s_t_r_i_b_u_t_i_o_n_ _o_r_ _b_o_t_-
-_h_o_s_t_i_n_g_ _a_r_e_ _s_t_r_i_c_t_l_y_ _p_r_o_h_i_b_i_t_e_d_._ _I_f_ _y_o_u_ _m_o_d_i_f_y_ _t_h_e_ _c_o_d_e_ _a_n_d_ _d_i_s_t_r_i_b_u_t_e_ _o_r_ _h_o_s_t
-_i_t_,_ _m_a_k_e_ _s_u_r_e_ _a_n_y_ _u_s_e_r_s_ _w_h_o_ _c_a_n_ _u_s_e_ _y_o_u_r_ _b_o_t_ _c_a_n_ _g_e_t_ _t_h_e_ _s_o_u_r_c_e_ _c_o_d_e_ _(_b_y
-_e_d_i_t_i_n_g_ _t_h_e_ _r_e_p_o_ _U_R_L_ _i_n_ _[_`_s_r_c_/_i_1_8_n_/_____i_n_i_t_____._p_y_`_]_(_s_r_c_/_i_1_8_n_/_____i_n_i_t_____._p_y_)_)_._ _T_h_e
-_r_e_p_o_s_i_t_o_r_y_ _w_a_s_ _f_o_r_m_e_r_l_y_ _a_ _f_o_r_k_ _o_f_ _[_B_o_K_K_e_R_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_]_(_h_t_t_p_s_:_/_/
-_g_i_t_h_u_b_._c_o_m_/_B_o_K_K_e_R_/_R_S_S_-_t_o_-_T_e_l_e_g_r_a_m_-_B_o_t_)_._ _T_h_e_y_ _h_a_v_e_ _b_e_e_n_ _e_n_t_i_r_e_l_y_ _d_i_f_f_e_r_e_n_t
-_p_r_o_j_e_c_t_s_ _s_i_n_c_e_ _t_h_e_ _e_a_r_l_y_ _d_a_y_s_ _o_f_ _t_h_i_s_ _p_r_o_j_e_c_t_.
+                             [RSS to Telegram Bot]
+                       ************ RRSSSS ttoo TTeelleeggrraamm BBoott ************
+          AA TTeelleeggrraamm RRSSSS bboott tthhaatt ccaarreess aabboouutt yyoouurr rreeaaddiinngg eexxppeerriieennccee
+[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/
+Rongronggg9/RSS-to-Telegram-Bot?logo=git&label=commit)](https://github.com/
+Rongronggg9/RSS-to-Telegram-Bot/commits) [![Translating status](https://
+img.shields.io/weblate/progress/rss-to-telegram-
+bot?logo=weblate&color=informational)](https://hosted.weblate.org/engage/rss-
+to-telegram-bot/) [![Code quality](https://img.shields.io/codefactor/grade/
+github/Rongronggg9/RSS-to-Telegram-Bot?logo=codefactor)](https://
+www.codefactor.io/repository/github/rongronggg9/rss-to-telegram-bot) [![GitHub
+stars](https://img.shields.io/github/stars/Rongronggg9/Rss-to-Telegram-
+Bot?style=social)](https://github.com/Rongronggg9/RSS-to-Telegram-Bot/
+stargazers) [![GitHub forks](https://img.shields.io/github/forks/Rongronggg9/
+RSS-to-Telegram-Bot?style=social)](https://github.com/Rongronggg9/RSS-to-
+Telegram-Bot/fork) [![Telegram bot](https://img.shields.io/badge/
+Telegram%20Bot-%40RSStT__Bot-229ed9?logo=telegram&style=for-the-badge)](https:/
+/t.me/RSStT_Bot) [![Telegram group](https://img.shields.io/badge/dynamic/
+json?url=https%3A%2F%2Fapi.swo.moe%2Fstats%2Ftelegram%2FRSStT_Group&query=count&color=2CA5E0&label=Telegram%20Group&logo=telegram&cacheSeconds=3600&style=for-
+the-badge)](https://t.me/RSStT_Group) [![Telegram channel](https://
+img.shields.io/badge/dynamic/
+json?url=https%3A%2F%2Fapi.swo.moe%2Fstats%2Ftelegram%2FRSStT_Channel&query=count&color=2CA5E0&label=Telegram%20Channel&logo=telegram&cacheSeconds=3600&style=for-
+the-badge)](https://t.me/RSStT_Channel) | [ç®ä½ä¸­æ README] | [CHANGELOG] |
+[FAQ] | [Documentation] | [Channels Using RSStT] | |:-------------:|:----------
+-:|:-----:|-----------------|:----------------------:| [ç®ä½ä¸­æ README]:
+README.zh.md [CHANGELOG]: docs/CHANGELOG.md [FAQ]: docs/FAQ.md [Documentation]:
+docs [Channels Using RSStT]: docs/channels-using-rsstt.md
+[Screenshot] [Screenshot] [Screenshot]
+[Screenshot]
+## Highlights - Multi-user - I18n - English, Chinese, Cantonese, Italian, and
+[more](docs/translation-guide.md)! - The content of the posts of an RSS feed
+will be sent to Telegram - Keep rich-text format - Keep media (customizable) -
+Images, Videos, and Audio both in the post content and enclosure; Documents in
+the post enclosure - Long images will be sent as files to prevent Telegram from
+compressing the image and making it unreadable - Drop annoying icons, they
+break the reading experience - Automatically replace emoji shortcodes with
+emoji - Automatically replace emoji images with emoji or its description text -
+Automatically determine whether the title of the RSS feed is auto-filled, if
+so, omit the title (customizable) - Automatically show the author-name
+(customizable) - Automatically split too-long messages - Messages can be sent
+as Telegraph posts (customizable) - Most images and videos will be uploaded to
+Telegraph, so that Instant View will load rapidly - [Various customizable
+formatting settings](docs/formatting-settings.md) - Hashtags, custom title,
+etc. - Individual proxy settings for Telegram and RSS feeds - OPML importing
+and exporting (keep custom title) - Optimized performance (see also the [FAQ]
+(docs/FAQ.md#q-how-is-the-performance-of-the-bot)) - User-friendly - HTTP
+Caching ## Deployment [![dockeri.co](https://dockerico.blankenship.io/image/
+rongronggg9/rss-to-telegram)](https://hub.docker.com/r/rongronggg9/rss-to-
+telegram)\ [![Build status (master)](https://img.shields.io/github/actions/
+workflow/status/Rongronggg9/RSS-to-Telegram-Bot/publish-docker-
+image.yml?branch=master&label=build&logo=docker)](https://github.com/
+Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-docker-
+image.yml?query=branch%3Amaster) [![Build status (dev)](https://img.shields.io/
+github/actions/workflow/status/Rongronggg9/RSS-to-Telegram-Bot/publish-docker-
+image.yml?branch=dev&label=build%20%28dev%29&logo=docker)](https://github.com/
+Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-docker-
+image.yml?query=branch%3Adev) [![PyPI](https://img.shields.io/pypi/v/
+rsstt?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/rsstt/)
+[![TestPyPI](https://img.shields.io/badge/dynamic/
+json?url=https%3A%2F%2Ftest.pypi.org%2Fpypi%2Frsstt%2Fjson&query=%24.info.version&prefix=v&logo=pypi&logoColor=white&label=TestPyPI)]
+(https://test.pypi.org/project/rsstt/) [![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/rsstt?logo=python&label=&labelColor=white)]
+(https://www.python.org)\ [![PyPI publish status](https://img.shields.io/
+github/actions/workflow/status/Rongronggg9/RSS-to-Telegram-Bot/publish-to-
+pypi.yml?label=publish&logo=pypi&logoColor=white)](https://github.com/
+Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-to-pypi.yml) [!
+[TestPyPI publish status](https://img.shields.io/github/actions/workflow/
+status/Rongronggg9/RSS-to-Telegram-Bot/publish-to-test-
+pypi.yml?label=publish%20(TestPyPI)&logo=pypi&logoColor=white)](https://
+github.com/Rongronggg9/RSS-to-Telegram-Bot/actions/workflows/publish-to-test-
+pypi.yml) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
+rsstt?logo=pypi&logoColor=white)](https://pypi.org/project/rsstt/) It is quite
+easy to deploy your RSStT instance. The most recommended way to deploy RSStT is
+Docker Compose: it is suitable for virtually all VPS. [Railway.app](https://
+railway.app) (a PaaS platform) is also officially supported. You may also
+install RSStT from [PyPI](https://pypi.org/project/rsstt/) (tracking `master`
+branch) or [TestPyPI](https://test.pypi.org/project/rsstt/) (tracking `dev`
+branch, which is always up-to-date) using pip. For developers or experienced
+users, dirty run from source is also an option. _[_D_e_p_l_o_y_ _o_n_ _R_a_i_l_w_a_y_]For more
+details, refer to the [deployment guide](docs/deployment-guide.md). ##
+Translation Read the translation guide [here](docs/translation-guide.md). You
+can help to translate the bot using [Hosted Weblate](https://
+hosted.weblate.org/projects/rss-to-telegram-bot/). Special thanks to their free
+hosting service for libre projects! ## Using the public bot The [public bot]
+(https://t.me/RSStT_Bot) comes with absolutely no warranty. I will try my best
+to maintain it, but I cannot guarantee that it will always work perfectly.
+Meanwhile, you should "fair use" the bot, avoid subscribing to too many RSS
+feeds. If you use the [public bot](https://t.me/RSStT_Bot) in your Channel,
+consider mentioning the bot (or this project) in your channel description (or
+pinned message) to let more people know about it. That's not a compulsion. ##
+Known channels using RSStT Want to preview what the messages sent by RSStT look
+like? Here is a [list of channels using RSStT](docs/channels-using-rsstt.md).
+## License This project is licensed under [AGPLv3](LICENSE). Closed-source
+distribution or bot-hosting are strictly prohibited. If you modify the code and
+distribute or host it, make sure any users who can use your bot can get the
+source code (by editing the repo URL in [`src/i18n/__init__.py`](src/i18n/
+__init__.py)). The repository was formerly a fork of [BoKKeR/RSS-to-Telegram-
+Bot](https://github.com/BoKKeR/RSS-to-Telegram-Bot). They have been entirely
+different projects since the early days of this project.
```

### Comparing `rsstt-2.6.0/requirements.txt` & `rsstt-2.7.0/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # telegram and telegraph
 cryptg==0.4.0
-telethon==1.34.0
+telethon==1.35.0
 aiographfix==0.2.2
 
 # feed parsing
 feedparser==6.0.11  # feedparser@git+https://github.com/Rongronggg9/feedparser.git@develop
-listparser[lxml]==0.19
-pillow==10.2.0
+listparser[lxml]==0.20
+pillow==10.3.0
 beautifulsoup4==4.12.3
-lxml==4.9.3
-rapidfuzz==3.7.0
-emoji==2.11.0
+lxml==5.2.1
+rapidfuzz==3.9.0
+emoji==2.11.1
 minify-html==0.15.0
 minify-html-onepass==0.15.0
-matplotlib==3.8.3
+matplotlib==3.8.4
 
 # db
 asyncpg==0.29.0
-tortoise-orm[accel]==0.20.0
-aerich==0.6.3
+tortoise-orm[accel]==0.20.1
+aerich==0.7.2
 
 # network
-aiohttp[speedups]==3.9.3
+aiohttp[speedups]==3.9.5
 aiohttp-socks==0.8.4
 aiohttp-retry==2.8.3
 python-socks[asyncio]==2.4.4
 dnspython[idna]==2.6.1
 
 # utils
 colorlog==6.8.2
 APScheduler==3.10.4
 python-dotenv==1.0.1
 multidict==6.0.5
-asyncstdlib==3.12.2
+asyncstdlib==3.12.3
 cachetools==5.3.3
 CJKwrap==2.2
-typing-extensions==4.10.0
+typing-extensions==4.11.0
 uvloop==0.19.0; sys_platform!='win32' and sys_platform!='cygwin' and sys_platform!='cli'
 isal==1.6.1; platform_machine=='x86_64' or platform_machine=='AMD64' or platform_machine=='aarch64'
```

### Comparing `rsstt-2.6.0/rsstt.egg-info/PKG-INFO` & `rsstt-2.7.0/rsstt.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7273 7374  : 2.1.Name: rsst
-00000020: 740a 5665 7273 696f 6e3a 2032 2e36 2e30  t.Version: 2.6.0
+00000020: 740a 5665 7273 696f 6e3a 2032 2e37 2e30  t.Version: 2.7.0
 00000030: 0a53 756d 6d61 7279 3a20 4120 5465 6c65  .Summary: A Tele
 00000040: 6772 616d 2052 5353 2062 6f74 2074 6861  gram RSS bot tha
 00000050: 7420 6361 7265 7320 6162 6f75 7420 796f  t cares about yo
 00000060: 7572 2072 6561 6469 6e67 2065 7870 6572  ur reading exper
 00000070: 6965 6e63 650a 486f 6d65 2d70 6167 653a  ience.Home-page:
 00000080: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000090: 636f 6d2f 526f 6e67 726f 6e67 6767 392f  com/Rongronggg9/
@@ -79,578 +79,610 @@
 000004e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
 000004f0: 300a 436c 6173 7369 6669 6572 3a20 5072  0.Classifier: Pr
 00000500: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 00000510: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
 00000520: 332e 3131 0a43 6c61 7373 6966 6965 723a  3.11.Classifier:
 00000530: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
 00000540: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000550: 3a3a 2049 6d70 6c65 6d65 6e74 6174 696f  :: Implementatio
-00000560: 6e20 3a3a 2043 5079 7468 6f6e 0a43 6c61  n :: CPython.Cla
-00000570: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
-00000580: 3a20 436f 6d6d 756e 6963 6174 696f 6e73  : Communications
-00000590: 203a 3a20 4368 6174 0a43 6c61 7373 6966   :: Chat.Classif
-000005a0: 6965 723a 2054 6f70 6963 203a 3a20 496e  ier: Topic :: In
-000005b0: 7465 726e 6574 0a43 6c61 7373 6966 6965  ternet.Classifie
-000005c0: 723a 2054 6f70 6963 203a 3a20 4d75 6c74  r: Topic :: Mult
-000005d0: 696d 6564 6961 0a52 6571 7569 7265 732d  imedia.Requires-
-000005e0: 5079 7468 6f6e 3a20 3e3d 332e 390a 4465  Python: >=3.9.De
-000005f0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000600: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000610: 6b64 6f77 6e0a 4c69 6365 6e73 652d 4669  kdown.License-Fi
-00000620: 6c65 3a20 4c49 4345 4e53 450a 5265 7175  le: LICENSE.Requ
-00000630: 6972 6573 2d44 6973 743a 2063 7279 7074  ires-Dist: crypt
-00000640: 673d 3d30 2e34 2e30 0a52 6571 7569 7265  g==0.4.0.Require
-00000650: 732d 4469 7374 3a20 7465 6c65 7468 6f6e  s-Dist: telethon
-00000660: 3d3d 312e 3334 2e30 0a52 6571 7569 7265  ==1.34.0.Require
-00000670: 732d 4469 7374 3a20 6169 6f67 7261 7068  s-Dist: aiograph
-00000680: 6669 783d 3d30 2e32 2e32 0a52 6571 7569  fix==0.2.2.Requi
-00000690: 7265 732d 4469 7374 3a20 6665 6564 7061  res-Dist: feedpa
-000006a0: 7273 6572 3d3d 362e 302e 3131 0a52 6571  rser==6.0.11.Req
-000006b0: 7569 7265 732d 4469 7374 3a20 6c69 7374  uires-Dist: list
-000006c0: 7061 7273 6572 5b6c 786d 6c5d 3d3d 302e  parser[lxml]==0.
-000006d0: 3139 0a52 6571 7569 7265 732d 4469 7374  19.Requires-Dist
-000006e0: 3a20 7069 6c6c 6f77 3d3d 3130 2e32 2e30  : pillow==10.2.0
-000006f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000700: 6265 6175 7469 6675 6c73 6f75 7034 3d3d  beautifulsoup4==
-00000710: 342e 3132 2e33 0a52 6571 7569 7265 732d  4.12.3.Requires-
-00000720: 4469 7374 3a20 6c78 6d6c 3d3d 342e 392e  Dist: lxml==4.9.
-00000730: 330a 5265 7175 6972 6573 2d44 6973 743a  3.Requires-Dist:
-00000740: 2072 6170 6964 6675 7a7a 3d3d 332e 372e   rapidfuzz==3.7.
-00000750: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-00000760: 2065 6d6f 6a69 3d3d 322e 3131 2e30 0a52   emoji==2.11.0.R
-00000770: 6571 7569 7265 732d 4469 7374 3a20 6d69  equires-Dist: mi
-00000780: 6e69 6679 2d68 746d 6c3d 3d30 2e31 352e  nify-html==0.15.
-00000790: 300a 5265 7175 6972 6573 2d44 6973 743a  0.Requires-Dist:
-000007a0: 206d 696e 6966 792d 6874 6d6c 2d6f 6e65   minify-html-one
-000007b0: 7061 7373 3d3d 302e 3135 2e30 0a52 6571  pass==0.15.0.Req
-000007c0: 7569 7265 732d 4469 7374 3a20 6d61 7470  uires-Dist: matp
-000007d0: 6c6f 746c 6962 3d3d 332e 382e 330a 5265  lotlib==3.8.3.Re
-000007e0: 7175 6972 6573 2d44 6973 743a 2061 7379  quires-Dist: asy
-000007f0: 6e63 7067 3d3d 302e 3239 2e30 0a52 6571  ncpg==0.29.0.Req
-00000800: 7569 7265 732d 4469 7374 3a20 746f 7274  uires-Dist: tort
-00000810: 6f69 7365 2d6f 726d 5b61 6363 656c 5d3d  oise-orm[accel]=
-00000820: 3d30 2e32 302e 300a 5265 7175 6972 6573  =0.20.0.Requires
-00000830: 2d44 6973 743a 2061 6572 6963 683d 3d30  -Dist: aerich==0
-00000840: 2e36 2e33 0a52 6571 7569 7265 732d 4469  .6.3.Requires-Di
-00000850: 7374 3a20 6169 6f68 7474 705b 7370 6565  st: aiohttp[spee
-00000860: 6475 7073 5d3d 3d33 2e39 2e33 0a52 6571  dups]==3.9.3.Req
-00000870: 7569 7265 732d 4469 7374 3a20 6169 6f68  uires-Dist: aioh
-00000880: 7474 702d 736f 636b 733d 3d30 2e38 2e34  ttp-socks==0.8.4
-00000890: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000008a0: 6169 6f68 7474 702d 7265 7472 793d 3d32  aiohttp-retry==2
-000008b0: 2e38 2e33 0a52 6571 7569 7265 732d 4469  .8.3.Requires-Di
-000008c0: 7374 3a20 7079 7468 6f6e 2d73 6f63 6b73  st: python-socks
-000008d0: 5b61 7379 6e63 696f 5d3d 3d32 2e34 2e34  [asyncio]==2.4.4
-000008e0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000008f0: 646e 7370 7974 686f 6e5b 6964 6e61 5d3d  dnspython[idna]=
-00000900: 3d32 2e36 2e31 0a52 6571 7569 7265 732d  =2.6.1.Requires-
-00000910: 4469 7374 3a20 636f 6c6f 726c 6f67 3d3d  Dist: colorlog==
-00000920: 362e 382e 320a 5265 7175 6972 6573 2d44  6.8.2.Requires-D
-00000930: 6973 743a 2041 5053 6368 6564 756c 6572  ist: APScheduler
-00000940: 3d3d 332e 3130 2e34 0a52 6571 7569 7265  ==3.10.4.Require
-00000950: 732d 4469 7374 3a20 7079 7468 6f6e 2d64  s-Dist: python-d
-00000960: 6f74 656e 763d 3d31 2e30 2e31 0a52 6571  otenv==1.0.1.Req
-00000970: 7569 7265 732d 4469 7374 3a20 6d75 6c74  uires-Dist: mult
-00000980: 6964 6963 743d 3d36 2e30 2e35 0a52 6571  idict==6.0.5.Req
-00000990: 7569 7265 732d 4469 7374 3a20 6173 796e  uires-Dist: asyn
-000009a0: 6373 7464 6c69 623d 3d33 2e31 322e 320a  cstdlib==3.12.2.
-000009b0: 5265 7175 6972 6573 2d44 6973 743a 2063  Requires-Dist: c
-000009c0: 6163 6865 746f 6f6c 733d 3d35 2e33 2e33  achetools==5.3.3
-000009d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000009e0: 434a 4b77 7261 703d 3d32 2e32 0a52 6571  CJKwrap==2.2.Req
-000009f0: 7569 7265 732d 4469 7374 3a20 7479 7069  uires-Dist: typi
-00000a00: 6e67 2d65 7874 656e 7369 6f6e 733d 3d34  ng-extensions==4
-00000a10: 2e31 302e 300a 5265 7175 6972 6573 2d44  .10.0.Requires-D
-00000a20: 6973 743a 2075 766c 6f6f 703d 3d30 2e31  ist: uvloop==0.1
-00000a30: 392e 303b 2073 7973 5f70 6c61 7466 6f72  9.0; sys_platfor
-00000a40: 6d20 213d 2022 7769 6e33 3222 2061 6e64  m != "win32" and
-00000a50: 2073 7973 5f70 6c61 7466 6f72 6d20 213d   sys_platform !=
-00000a60: 2022 6379 6777 696e 2220 616e 6420 7379   "cygwin" and sy
-00000a70: 735f 706c 6174 666f 726d 2021 3d20 2263  s_platform != "c
-00000a80: 6c69 220a 5265 7175 6972 6573 2d44 6973  li".Requires-Dis
-00000a90: 743a 2069 7361 6c3d 3d31 2e36 2e31 3b20  t: isal==1.6.1; 
-00000aa0: 706c 6174 666f 726d 5f6d 6163 6869 6e65  platform_machine
-00000ab0: 203d 3d20 2278 3836 5f36 3422 206f 7220   == "x86_64" or 
-00000ac0: 706c 6174 666f 726d 5f6d 6163 6869 6e65  platform_machine
-00000ad0: 203d 3d20 2241 4d44 3634 2220 6f72 2070   == "AMD64" or p
-00000ae0: 6c61 7466 6f72 6d5f 6d61 6368 696e 6520  latform_machine 
-00000af0: 3d3d 2022 6161 7263 6836 3422 0a0a 3c61  == "aarch64"..<a
-00000b00: 2068 7265 663d 2268 7474 7073 3a2f 2f74   href="https://t
-00000b10: 2e6d 652f 5253 5374 545f 426f 7422 3e3c  .me/RSStT_Bot"><
-00000b20: 696d 6720 7769 6474 683d 2231 3530 2220  img width="150" 
-00000b30: 6865 6967 6874 3d22 3135 3022 2061 6c69  height="150" ali
-00000b40: 676e 3d22 6c65 6674 2220 7374 796c 653d  gn="left" style=
-00000b50: 2266 6c6f 6174 3a20 6c65 6674 3b20 6d61  "float: left; ma
-00000b60: 7267 696e 3a20 3020 3130 7078 2030 2030  rgin: 0 10px 0 0
-00000b70: 3b22 2061 6c74 3d22 5253 5374 5420 6963  ;" alt="RSStT ic
-00000b80: 6f6e 2220 7372 633d 2264 6f63 732f 7265  on" src="docs/re
-00000b90: 736f 7572 6365 732f 5253 5374 545f 6963  sources/RSStT_ic
-00000ba0: 6f6e 2e73 7667 222f 3e3c 612f 3e0a 0a23  on.svg"/><a/>..#
-00000bb0: 205b 5253 5320 746f 2054 656c 6567 7261   [RSS to Telegra
-00000bc0: 6d20 426f 745d 2868 7474 7073 3a2f 2f74  m Bot](https://t
-00000bd0: 2e6d 652f 5253 5374 545f 426f 7429 0a0a  .me/RSStT_Bot)..
-00000be0: 2a2a 4120 5465 6c65 6772 616d 2052 5353  **A Telegram RSS
-00000bf0: 2062 6f74 2074 6861 7420 6361 7265 7320   bot that cares 
-00000c00: 6162 6f75 7420 796f 7572 2072 6561 6469  about your readi
-00000c10: 6e67 2065 7870 6572 6965 6e63 652a 2a0a  ng experience**.
-00000c20: 0a5b e7ae 80e4 bd93 e4b8 ade6 9687 2052  .[............ R
-00000c30: 4541 444d 455d 2852 4541 444d 452e 7a68  EADME](README.zh
-00000c40: 2e6d 6429 0a0a 5b21 5b47 6974 4875 6220  .md)..[![GitHub 
-00000c50: 636f 6d6d 6974 2061 6374 6976 6974 795d  commit activity]
-00000c60: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000c70: 656c 6473 2e69 6f2f 6769 7468 7562 2f63  elds.io/github/c
-00000c80: 6f6d 6d69 742d 6163 7469 7669 7479 2f6d  ommit-activity/m
-00000c90: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
-00000ca0: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
-00000cb0: 3f6c 6f67 6f3d 6769 7426 6c61 6265 6c3d  ?logo=git&label=
-00000cc0: 636f 6d6d 6974 295d 2868 7474 7073 3a2f  commit)](https:/
-00000cd0: 2f67 6974 6875 622e 636f 6d2f 526f 6e67  /github.com/Rong
-00000ce0: 726f 6e67 6767 392f 5253 532d 746f 2d54  ronggg9/RSS-to-T
-00000cf0: 656c 6567 7261 6d2d 426f 742f 636f 6d6d  elegram-Bot/comm
-00000d00: 6974 7329 0a5b 215b 5472 616e 736c 6174  its).[![Translat
-00000d10: 696e 6720 7374 6174 7573 5d28 6874 7470  ing status](http
-00000d20: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000d30: 696f 2f77 6562 6c61 7465 2f70 726f 6772  io/weblate/progr
-00000d40: 6573 732f 7273 732d 746f 2d74 656c 6567  ess/rss-to-teleg
-00000d50: 7261 6d2d 626f 743f 6c6f 676f 3d77 6562  ram-bot?logo=web
-00000d60: 6c61 7465 2663 6f6c 6f72 3d69 6e66 6f72  late&color=infor
-00000d70: 6d61 7469 6f6e 616c 295d 2868 7474 7073  mational)](https
-00000d80: 3a2f 2f68 6f73 7465 642e 7765 626c 6174  ://hosted.weblat
-00000d90: 652e 6f72 672f 656e 6761 6765 2f72 7373  e.org/engage/rss
-00000da0: 2d74 6f2d 7465 6c65 6772 616d 2d62 6f74  -to-telegram-bot
-00000db0: 2f29 0a5b 215b 436f 6465 2071 7561 6c69  /).[![Code quali
-00000dc0: 7479 5d28 6874 7470 733a 2f2f 696d 672e  ty](https://img.
-00000dd0: 7368 6965 6c64 732e 696f 2f63 6f64 6566  shields.io/codef
-00000de0: 6163 746f 722f 6772 6164 652f 6769 7468  actor/grade/gith
-00000df0: 7562 2f52 6f6e 6772 6f6e 6767 6739 2f52  ub/Rongronggg9/R
-00000e00: 5353 2d74 6f2d 5465 6c65 6772 616d 2d42  SS-to-Telegram-B
-00000e10: 6f74 3f6c 6f67 6f3d 636f 6465 6661 6374  ot?logo=codefact
-00000e20: 6f72 295d 2868 7474 7073 3a2f 2f77 7777  or)](https://www
-00000e30: 2e63 6f64 6566 6163 746f 722e 696f 2f72  .codefactor.io/r
-00000e40: 6570 6f73 6974 6f72 792f 6769 7468 7562  epository/github
-00000e50: 2f72 6f6e 6772 6f6e 6767 6739 2f72 7373  /rongronggg9/rss
-00000e60: 2d74 6f2d 7465 6c65 6772 616d 2d62 6f74  -to-telegram-bot
-00000e70: 290a 5b21 5b47 6974 4875 6220 7374 6172  ).[![GitHub star
-00000e80: 735d 2868 7474 7073 3a2f 2f69 6d67 2e73  s](https://img.s
-00000e90: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
-00000ea0: 2f73 7461 7273 2f52 6f6e 6772 6f6e 6767  /stars/Rongrongg
-00000eb0: 6739 2f52 7373 2d74 6f2d 5465 6c65 6772  g9/Rss-to-Telegr
-00000ec0: 616d 2d42 6f74 3f73 7479 6c65 3d73 6f63  am-Bot?style=soc
-00000ed0: 6961 6c29 5d28 6874 7470 733a 2f2f 6769  ial)](https://gi
-00000ee0: 7468 7562 2e63 6f6d 2f52 6f6e 6772 6f6e  thub.com/Rongron
-00000ef0: 6767 6739 2f52 5353 2d74 6f2d 5465 6c65  ggg9/RSS-to-Tele
-00000f00: 6772 616d 2d42 6f74 2f73 7461 7267 617a  gram-Bot/stargaz
-00000f10: 6572 7329 0a5b 215b 4769 7448 7562 2066  ers).[![GitHub f
-00000f20: 6f72 6b73 5d28 6874 7470 733a 2f2f 696d  orks](https://im
-00000f30: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
-00000f40: 6875 622f 666f 726b 732f 526f 6e67 726f  hub/forks/Rongro
-00000f50: 6e67 6767 392f 5253 532d 746f 2d54 656c  nggg9/RSS-to-Tel
-00000f60: 6567 7261 6d2d 426f 743f 7374 796c 653d  egram-Bot?style=
-00000f70: 736f 6369 616c 295d 2868 7474 7073 3a2f  social)](https:/
-00000f80: 2f67 6974 6875 622e 636f 6d2f 526f 6e67  /github.com/Rong
-00000f90: 726f 6e67 6767 392f 5253 532d 746f 2d54  ronggg9/RSS-to-T
-00000fa0: 656c 6567 7261 6d2d 426f 742f 666f 726b  elegram-Bot/fork
-00000fb0: 290a 0a5b 215b 5465 6c65 6772 616d 2062  )..[![Telegram b
-00000fc0: 6f74 5d28 6874 7470 733a 2f2f 696d 672e  ot](https://img.
-00000fd0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000fe0: 2f62 6f74 2d25 3430 5253 5374 545f 5f42  /bot-%40RSStT__B
-00000ff0: 6f74 2d32 3239 6564 393f 6c6f 676f 3d74  ot-229ed9?logo=t
-00001000: 656c 6567 7261 6d26 7374 796c 653d 666f  elegram&style=fo
-00001010: 722d 7468 652d 6261 6467 6529 5d28 6874  r-the-badge)](ht
-00001020: 7470 733a 2f2f 742e 6d65 2f52 5353 7454  tps://t.me/RSStT
-00001030: 5f42 6f74 290a 5b21 5b54 656c 6567 7261  _Bot).[![Telegra
-00001040: 6d20 6772 6f75 705d 2868 7474 7073 3a2f  m group](https:/
-00001050: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001060: 6261 6467 652f 6368 6174 2d25 3430 5253  badge/chat-%40RS
-00001070: 5374 545f 5f47 726f 7570 2d32 3239 6564  StT__Group-229ed
-00001080: 393f 6c6f 676f 3d74 656c 6567 7261 6d26  9?logo=telegram&
-00001090: 7374 796c 653d 666f 722d 7468 652d 6261  style=for-the-ba
-000010a0: 6467 6529 5d28 6874 7470 733a 2f2f 742e  dge)](https://t.
-000010b0: 6d65 2f52 5353 7454 5f47 726f 7570 290a  me/RSStT_Group).
-000010c0: 5b21 5b54 656c 6567 7261 6d20 6368 616e  [![Telegram chan
-000010d0: 6e65 6c5d 2868 7474 7073 3a2f 2f69 6d67  nel](https://img
-000010e0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000010f0: 652f 6368 616e 6e65 6c2d 2534 3052 5353  e/channel-%40RSS
-00001100: 7454 5f5f 4368 616e 6e65 6c2d 3232 3965  tT__Channel-229e
-00001110: 6439 3f6c 6f67 6f3d 7465 6c65 6772 616d  d9?logo=telegram
-00001120: 2673 7479 6c65 3d66 6f72 2d74 6865 2d62  &style=for-the-b
-00001130: 6164 6765 295d 2868 7474 7073 3a2f 2f74  adge)](https://t
-00001140: 2e6d 652f 5253 5374 545f 4368 616e 6e65  .me/RSStT_Channe
-00001150: 6c29 0a0a 7c20 5b43 4841 4e47 454c 4f47  l)..| [CHANGELOG
-00001160: 5d20 7c20 5b46 4151 5d20 7c20 5b44 6f63  ] | [FAQ] | [Doc
-00001170: 756d 656e 7461 7469 6f6e 5d20 7c20 5b43  umentation] | [C
-00001180: 6861 6e6e 656c 7320 5573 696e 6720 5253  hannels Using RS
-00001190: 5374 545d 207c 0a7c 3a2d 2d2d 2d2d 2d2d  StT] |.|:-------
-000011a0: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 3a7c 2d2d  ----:|:-----:|--
-000011b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
-000011c0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
-000011d0: 2d2d 2d2d 2d2d 2d3a 7c0a 0a5b 4348 414e  -------:|..[CHAN
-000011e0: 4745 4c4f 475d 3a20 646f 6373 2f43 4841  GELOG]: docs/CHA
-000011f0: 4e47 454c 4f47 2e6d 640a 0a5b 4641 515d  NGELOG.md..[FAQ]
-00001200: 3a20 646f 6373 2f46 4151 2e6d 640a 0a5b  : docs/FAQ.md..[
-00001210: 446f 6375 6d65 6e74 6174 696f 6e5d 3a20  Documentation]: 
-00001220: 646f 6373 0a0a 5b43 6861 6e6e 656c 7320  docs..[Channels 
-00001230: 5573 696e 6720 5253 5374 545d 3a20 646f  Using RSStT]: do
-00001240: 6373 2f63 6861 6e6e 656c 732d 7573 696e  cs/channels-usin
-00001250: 672d 7273 7374 742e 6d64 0a0a 0a2a 2a49  g-rsstt.md...**I
-00001260: 6d70 6f72 7461 6e74 2a2a 3a20 4966 2079  mportant**: If y
-00001270: 6f75 2068 6176 6520 796f 7572 206f 776e  ou have your own
-00001280: 2052 5353 7454 2062 6f74 2028 7631 292c   RSStT bot (v1),
-00001290: 2070 6c65 6173 6520 7265 6164 2074 6865   please read the
-000012a0: 205b 6d69 6772 6174 696f 6e20 6775 6964   [migration guid
-000012b0: 655d 2864 6f63 732f 6d69 6772 6174 696f  e](docs/migratio
-000012c0: 6e2d 6775 6964 652d 7632 2e6d 6429 2074  n-guide-v2.md) t
-000012d0: 6f20 6c65 6172 6e20 686f 7720 746f 206d  o learn how to m
-000012e0: 6967 7261 7465 2074 6f20 7632 2e0a 0a23  igrate to v2...#
-000012f0: 2320 4869 6768 6c69 6768 7473 0a0a 2d20  # Highlights..- 
-00001300: 4d75 6c74 692d 7573 6572 0a2d 2049 3138  Multi-user.- I18
-00001310: 6e0a 2020 2020 2d20 456e 676c 6973 682c  n.    - English,
-00001320: 2043 6869 6e65 7365 2c20 4361 6e74 6f6e   Chinese, Canton
-00001330: 6573 652c 2049 7461 6c69 616e 2c20 616e  ese, Italian, an
-00001340: 6420 5b6d 6f72 655d 2864 6f63 732f 7472  d [more](docs/tr
-00001350: 616e 736c 6174 696f 6e2d 6775 6964 652e  anslation-guide.
-00001360: 6d64 2921 0a2d 2054 6865 2063 6f6e 7465  md)!.- The conte
-00001370: 6e74 206f 6620 7468 6520 706f 7374 7320  nt of the posts 
-00001380: 6f66 2061 6e20 5253 5320 6665 6564 2077  of an RSS feed w
-00001390: 696c 6c20 6265 2073 656e 7420 746f 2054  ill be sent to T
-000013a0: 656c 6567 7261 6d0a 2020 2020 2d20 4b65  elegram.    - Ke
-000013b0: 6570 2072 6963 682d 7465 7874 2066 6f72  ep rich-text for
-000013c0: 6d61 740a 2020 2020 2d20 4b65 6570 206d  mat.    - Keep m
-000013d0: 6564 6961 2028 6375 7374 6f6d 697a 6162  edia (customizab
-000013e0: 6c65 290a 2020 2020 2020 2020 2d20 496d  le).        - Im
-000013f0: 6167 6573 2c20 5669 6465 6f73 2c20 616e  ages, Videos, an
-00001400: 6420 4175 6469 6f20 626f 7468 2069 6e20  d Audio both in 
-00001410: 7468 6520 706f 7374 2063 6f6e 7465 6e74  the post content
-00001420: 2061 6e64 2065 6e63 6c6f 7375 7265 3b20   and enclosure; 
-00001430: 446f 6375 6d65 6e74 7320 696e 2074 6865  Documents in the
-00001440: 2070 6f73 7420 656e 636c 6f73 7572 650a   post enclosure.
-00001450: 2020 2020 2020 2020 2d20 4c6f 6e67 2069          - Long i
-00001460: 6d61 6765 7320 7769 6c6c 2062 6520 7365  mages will be se
-00001470: 6e74 2061 7320 6669 6c65 7320 746f 2070  nt as files to p
-00001480: 7265 7665 6e74 2054 656c 6567 7261 6d20  revent Telegram 
-00001490: 6672 6f6d 2063 6f6d 7072 6573 7369 6e67  from compressing
-000014a0: 2074 6865 2069 6d61 6765 2061 6e64 206d   the image and m
-000014b0: 616b 696e 6720 6974 2075 6e72 6561 6461  aking it unreada
-000014c0: 626c 650a 2020 2020 2020 2020 2d20 4472  ble.        - Dr
-000014d0: 6f70 2061 6e6e 6f79 696e 6720 6963 6f6e  op annoying icon
-000014e0: 732c 2074 6865 7920 6272 6561 6b20 7468  s, they break th
-000014f0: 6520 7265 6164 696e 6720 6578 7065 7269  e reading experi
-00001500: 656e 6365 0a20 2020 202d 2041 7574 6f6d  ence.    - Autom
-00001510: 6174 6963 616c 6c79 2072 6570 6c61 6365  atically replace
-00001520: 2065 6d6f 6a69 2073 686f 7274 636f 6465   emoji shortcode
-00001530: 7320 7769 7468 2065 6d6f 6a69 0a20 2020  s with emoji.   
-00001540: 202d 2041 7574 6f6d 6174 6963 616c 6c79   - Automatically
-00001550: 2072 6570 6c61 6365 2065 6d6f 6a69 2069   replace emoji i
-00001560: 6d61 6765 7320 7769 7468 2065 6d6f 6a69  mages with emoji
-00001570: 206f 7220 6974 7320 6465 7363 7269 7074   or its descript
-00001580: 696f 6e20 7465 7874 0a20 2020 202d 2041  ion text.    - A
-00001590: 7574 6f6d 6174 6963 616c 6c79 2064 6574  utomatically det
-000015a0: 6572 6d69 6e65 2077 6865 7468 6572 2074  ermine whether t
-000015b0: 6865 2074 6974 6c65 206f 6620 7468 6520  he title of the 
-000015c0: 5253 5320 6665 6564 2069 7320 6175 746f  RSS feed is auto
-000015d0: 2d66 696c 6c65 642c 2069 6620 736f 2c20  -filled, if so, 
-000015e0: 6f6d 6974 2074 6865 2074 6974 6c65 2028  omit the title (
-000015f0: 6375 7374 6f6d 697a 6162 6c65 290a 2020  customizable).  
-00001600: 2020 2d20 4175 746f 6d61 7469 6361 6c6c    - Automaticall
-00001610: 7920 7368 6f77 2074 6865 2061 7574 686f  y show the autho
-00001620: 722d 6e61 6d65 2028 6375 7374 6f6d 697a  r-name (customiz
-00001630: 6162 6c65 290a 2020 2020 2d20 4175 746f  able).    - Auto
-00001640: 6d61 7469 6361 6c6c 7920 7370 6c69 7420  matically split 
-00001650: 746f 6f2d 6c6f 6e67 206d 6573 7361 6765  too-long message
-00001660: 730a 2020 2020 2020 2020 2d20 4966 2063  s.        - If c
-00001670: 6f6e 6669 6775 7265 6420 5465 6c65 6772  onfigured Telegr
-00001680: 6170 682c 2074 6865 206d 6573 7361 6765  aph, the message
-00001690: 2077 696c 6c20 6265 2073 656e 7420 7669   will be sent vi
-000016a0: 6120 5465 6c65 6772 6170 6820 2863 7573  a Telegraph (cus
-000016b0: 746f 6d69 7a61 626c 6529 0a2d 205b 5661  tomizable).- [Va
-000016c0: 7269 6f75 7320 6375 7374 6f6d 697a 6162  rious customizab
-000016d0: 6c65 2066 6f72 6d61 7474 696e 6720 7365  le formatting se
-000016e0: 7474 696e 6773 5d28 646f 6373 2f66 6f72  ttings](docs/for
-000016f0: 6d61 7474 696e 672d 7365 7474 696e 6773  matting-settings
-00001700: 2e6d 6429 0a20 2020 202d 2048 6173 6874  .md).    - Hasht
-00001710: 6167 732c 2063 7573 746f 6d20 7469 746c  ags, custom titl
-00001720: 652c 2065 7463 2e0a 2d20 496e 6469 7669  e, etc..- Indivi
-00001730: 6475 616c 2070 726f 7879 2073 6574 7469  dual proxy setti
-00001740: 6e67 7320 666f 7220 5465 6c65 6772 616d  ngs for Telegram
-00001750: 2061 6e64 2052 5353 2066 6565 6473 0a2d   and RSS feeds.-
-00001760: 204f 504d 4c20 696d 706f 7274 696e 6720   OPML importing 
-00001770: 616e 6420 6578 706f 7274 696e 6720 286b  and exporting (k
-00001780: 6565 7020 6375 7374 6f6d 2074 6974 6c65  eep custom title
-00001790: 290a 2d20 4f70 7469 6d69 7a65 6420 7065  ).- Optimized pe
-000017a0: 7266 6f72 6d61 6e63 6520 2873 6565 2061  rformance (see a
-000017b0: 6c73 6f20 7468 6520 5b46 4151 5d28 646f  lso the [FAQ](do
-000017c0: 6373 2f46 4151 2e6d 6423 712d 686f 772d  cs/FAQ.md#q-how-
-000017d0: 6973 2d74 6865 2d70 6572 666f 726d 616e  is-the-performan
-000017e0: 6365 2d6f 662d 7468 652d 626f 7429 290a  ce-of-the-bot)).
-000017f0: 2d20 5573 6572 2d66 7269 656e 646c 790a  - User-friendly.
-00001800: 2d20 4854 5450 2043 6163 6869 6e67 0a0a  - HTTP Caching..
-00001810: 3c69 6d67 2073 7263 3d22 646f 6373 2f72  <img src="docs/r
-00001820: 6573 6f75 7263 6573 2f65 7861 6d70 6c65  esources/example
-00001830: 312e 706e 6722 2077 6964 7468 203d 2022  1.png" width = "
-00001840: 3330 3022 2061 6c74 3d22 222f 3e3c 696d  300" alt=""/><im
-00001850: 6720 7372 633d 2264 6f63 732f 7265 736f  g src="docs/reso
-00001860: 7572 6365 732f 6578 616d 706c 6533 2e70  urces/example3.p
-00001870: 6e67 2220 7769 6474 6820 3d20 2233 3030  ng" width = "300
-00001880: 2220 616c 743d 2222 2f3e 3c69 6d67 2073  " alt=""/><img s
-00001890: 7263 3d22 646f 6373 2f72 6573 6f75 7263  rc="docs/resourc
-000018a0: 6573 2f65 7861 6d70 6c65 342e 706e 6722  es/example4.png"
-000018b0: 2077 6964 7468 203d 2022 3330 3022 2061   width = "300" a
-000018c0: 6c74 3d22 222f 3e0a 0a23 2320 4465 706c  lt=""/>..## Depl
-000018d0: 6f79 6d65 6e74 0a0a 5b21 5b50 7950 495d  oyment..[![PyPI]
-000018e0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000018f0: 656c 6473 2e69 6f2f 7079 7069 2f76 2f72  elds.io/pypi/v/r
-00001900: 7373 7474 3f6c 6f67 6f3d 7079 7069 266c  sstt?logo=pypi&l
-00001910: 6f67 6f43 6f6c 6f72 3d77 6869 7465 295d  ogoColor=white)]
-00001920: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
-00001930: 672f 7072 6f6a 6563 742f 7273 7374 742f  g/project/rsstt/
-00001940: 290a 5b21 5b50 7950 4920 7075 626c 6973  ).[![PyPI publis
-00001950: 6820 7374 6174 7573 5d28 6874 7470 733a  h status](https:
-00001960: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00001970: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
-00001980: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
-00001990: 526f 6e67 726f 6e67 6767 392f 5253 532d  Rongronggg9/RSS-
-000019a0: 746f 2d54 656c 6567 7261 6d2d 426f 742f  to-Telegram-Bot/
-000019b0: 7075 626c 6973 682d 746f 2d70 7970 692e  publish-to-pypi.
-000019c0: 796d 6c3f 6c61 6265 6c3d 7075 626c 6973  yml?label=publis
-000019d0: 6826 6c6f 676f 3d70 7970 6926 6c6f 676f  h&logo=pypi&logo
-000019e0: 436f 6c6f 723d 7768 6974 6529 5d28 6874  Color=white)](ht
-000019f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001a00: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
-00001a10: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
-00001a20: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00001a30: 7773 2f70 7562 6c69 7368 2d74 6f2d 7079  ws/publish-to-py
-00001a40: 7069 2e79 6d6c 290a 5b21 5b54 6573 7450  pi.yml).[![TestP
-00001a50: 7950 4920 7075 626c 6973 6820 7374 6174  yPI publish stat
-00001a60: 7573 5d28 6874 7470 733a 2f2f 696d 672e  us](https://img.
-00001a70: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00001a80: 622f 6163 7469 6f6e 732f 776f 726b 666c  b/actions/workfl
-00001a90: 6f77 2f73 7461 7475 732f 526f 6e67 726f  ow/status/Rongro
-00001aa0: 6e67 6767 392f 5253 532d 746f 2d54 656c  nggg9/RSS-to-Tel
-00001ab0: 6567 7261 6d2d 426f 742f 7075 626c 6973  egram-Bot/publis
-00001ac0: 682d 746f 2d74 6573 742d 7079 7069 2e79  h-to-test-pypi.y
-00001ad0: 6d6c 3f6c 6162 656c 3d70 7562 6c69 7368  ml?label=publish
-00001ae0: 2532 3028 5465 7374 5079 5049 2926 6c6f  %20(TestPyPI)&lo
-00001af0: 676f 3d70 7970 6926 6c6f 676f 436f 6c6f  go=pypi&logoColo
-00001b00: 723d 7768 6974 6529 5d28 6874 7470 733a  r=white)](https:
-00001b10: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6f6e  //github.com/Ron
-00001b20: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
-00001b30: 5465 6c65 6772 616d 2d42 6f74 2f61 6374  Telegram-Bot/act
-00001b40: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00001b50: 7562 6c69 7368 2d74 6f2d 7079 7069 2e79  ublish-to-pypi.y
-00001b60: 6d6c 290a 5b21 5b50 7950 4920 2d20 446f  ml).[![PyPI - Do
-00001b70: 776e 6c6f 6164 735d 2868 7474 7073 3a2f  wnloads](https:/
-00001b80: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00001b90: 7079 7069 2f64 6d2f 7273 7374 743f 6c6f  pypi/dm/rsstt?lo
-00001ba0: 676f 3d70 7970 6926 6c6f 676f 436f 6c6f  go=pypi&logoColo
-00001bb0: 723d 7768 6974 6529 5d28 6874 7470 733a  r=white)](https:
-00001bc0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-00001bd0: 6374 2f72 7373 7474 2f29 0a5b 215b 5079  ct/rsstt/).[![Py
-00001be0: 5049 202d 2050 7974 686f 6e20 5665 7273  PI - Python Vers
-00001bf0: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-00001c00: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-00001c10: 2f70 7976 6572 7369 6f6e 732f 7273 7374  /pyversions/rsst
-00001c20: 743f 6c6f 676f 3d70 7974 686f 6e26 6c61  t?logo=python&la
-00001c30: 6265 6c3d 266c 6162 656c 436f 6c6f 723d  bel=&labelColor=
-00001c40: 7768 6974 6529 5d28 6874 7470 733a 2f2f  white)](https://
-00001c50: 7777 772e 7079 7468 6f6e 2e6f 7267 290a  www.python.org).
-00001c60: 0a5b 215b 446f 636b 6572 2049 6d61 6765  .[![Docker Image
-00001c70: 2053 697a 6520 2874 6167 295d 2868 7474   Size (tag)](htt
-00001c80: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00001c90: 2e69 6f2f 646f 636b 6572 2f69 6d61 6765  .io/docker/image
-00001ca0: 2d73 697a 652f 726f 6e67 726f 6e67 6767  -size/rongronggg
-00001cb0: 392f 7273 732d 746f 2d74 656c 6567 7261  9/rss-to-telegra
-00001cc0: 6d2f 6c61 7465 7374 3f6c 6f67 6f3d 646f  m/latest?logo=do
-00001cd0: 636b 6572 295d 2868 7474 7073 3a2f 2f68  cker)](https://h
-00001ce0: 7562 2e64 6f63 6b65 722e 636f 6d2f 722f  ub.docker.com/r/
-00001cf0: 726f 6e67 726f 6e67 6767 392f 7273 732d  rongronggg9/rss-
-00001d00: 746f 2d74 656c 6567 7261 6d29 0a5b 215b  to-telegram).[![
-00001d10: 4275 696c 6420 7374 6174 7573 2028 6d61  Build status (ma
-00001d20: 7374 6572 295d 2868 7474 7073 3a2f 2f69  ster)](https://i
-00001d30: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
-00001d40: 7468 7562 2f61 6374 696f 6e73 2f77 6f72  thub/actions/wor
-00001d50: 6b66 6c6f 772f 7374 6174 7573 2f52 6f6e  kflow/status/Ron
-00001d60: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
-00001d70: 5465 6c65 6772 616d 2d42 6f74 2f70 7562  Telegram-Bot/pub
-00001d80: 6c69 7368 2d64 6f63 6b65 722d 696d 6167  lish-docker-imag
-00001d90: 652e 796d 6c3f 6272 616e 6368 3d6d 6173  e.yml?branch=mas
-00001da0: 7465 7226 6c61 6265 6c3d 6275 696c 6426  ter&label=build&
-00001db0: 6c6f 676f 3d64 6f63 6b65 7229 5d28 6874  logo=docker)](ht
-00001dc0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001dd0: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
-00001de0: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
-00001df0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
-00001e00: 7773 2f70 7562 6c69 7368 2d64 6f63 6b65  ws/publish-docke
-00001e10: 722d 696d 6167 652e 796d 6c3f 7175 6572  r-image.yml?quer
-00001e20: 793d 6272 616e 6368 2533 416d 6173 7465  y=branch%3Amaste
-00001e30: 7229 0a5b 215b 4275 696c 6420 7374 6174  r).[![Build stat
-00001e40: 7573 2028 6465 7629 5d28 6874 7470 733a  us (dev)](https:
-00001e50: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00001e60: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
-00001e70: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
-00001e80: 526f 6e67 726f 6e67 6767 392f 5253 532d  Rongronggg9/RSS-
-00001e90: 746f 2d54 656c 6567 7261 6d2d 426f 742f  to-Telegram-Bot/
-00001ea0: 7075 626c 6973 682d 646f 636b 6572 2d69  publish-docker-i
-00001eb0: 6d61 6765 2e79 6d6c 3f62 7261 6e63 683d  mage.yml?branch=
-00001ec0: 6465 7626 6c61 6265 6c3d 6275 696c 6425  dev&label=build%
-00001ed0: 3230 2532 3864 6576 2532 3926 6c6f 676f  20%28dev%29&logo
-00001ee0: 3d64 6f63 6b65 7229 5d28 6874 7470 733a  =docker)](https:
-00001ef0: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6f6e  //github.com/Ron
-00001f00: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
-00001f10: 5465 6c65 6772 616d 2d42 6f74 2f61 6374  Telegram-Bot/act
-00001f20: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
-00001f30: 7562 6c69 7368 2d64 6f63 6b65 722d 696d  ublish-docker-im
-00001f40: 6167 652e 796d 6c3f 7175 6572 793d 6272  age.yml?query=br
-00001f50: 616e 6368 2533 4164 6576 290a 5b21 5b44  anch%3Adev).[![D
-00001f60: 6f63 6b65 7220 7075 6c6c 735d 2868 7474  ocker pulls](htt
-00001f70: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00001f80: 2e69 6f2f 646f 636b 6572 2f70 756c 6c73  .io/docker/pulls
-00001f90: 2f72 6f6e 6772 6f6e 6767 6739 2f72 7373  /rongronggg9/rss
-00001fa0: 2d74 6f2d 7465 6c65 6772 616d 3f6c 6162  -to-telegram?lab
-00001fb0: 656c 3d70 756c 6c73 266c 6f67 6f3d 646f  el=pulls&logo=do
-00001fc0: 636b 6572 2663 6f6c 6f72 3d69 6e66 6f72  cker&color=infor
-00001fd0: 6d61 7469 6f6e 616c 295d 2868 7474 7073  mational)](https
-00001fe0: 3a2f 2f68 7562 2e64 6f63 6b65 722e 636f  ://hub.docker.co
-00001ff0: 6d2f 722f 726f 6e67 726f 6e67 6767 392f  m/r/rongronggg9/
-00002000: 7273 732d 746f 2d74 656c 6567 7261 6d29  rss-to-telegram)
-00002010: 0a0a 4974 2069 7320 7175 6974 6520 6561  ..It is quite ea
-00002020: 7379 2074 6f20 6465 706c 6f79 2079 6f75  sy to deploy you
-00002030: 7220 5253 5374 5420 696e 7374 616e 6365  r RSStT instance
-00002040: 2e20 5468 6520 6d6f 7374 2072 6563 6f6d  . The most recom
-00002050: 6d65 6e64 6564 2077 6179 2074 6f20 6465  mended way to de
-00002060: 706c 6f79 2052 5353 7454 2069 7320 446f  ploy RSStT is Do
-00002070: 636b 6572 2043 6f6d 706f 7365 3a20 6974  cker Compose: it
-00002080: 2069 7320 7375 6974 6162 6c65 2066 6f72   is suitable for
-00002090: 2076 6972 7475 616c 6c79 2061 6c6c 2056   virtually all V
-000020a0: 5053 2e20 5b52 6169 6c77 6179 2e61 7070  PS. [Railway.app
-000020b0: 5d28 6874 7470 733a 2f2f 7261 696c 7761  ](https://railwa
-000020c0: 792e 6170 7029 2028 6120 5061 6153 2070  y.app) (a PaaS p
-000020d0: 6c61 7466 6f72 6d29 2069 7320 616c 736f  latform) is also
-000020e0: 206f 6666 6963 6961 6c6c 7920 7375 7070   officially supp
-000020f0: 6f72 7465 642e 2059 6f75 206d 6179 2061  orted. You may a
-00002100: 6c73 6f20 696e 7374 616c 6c20 5253 5374  lso install RSSt
-00002110: 5420 6672 6f6d 2050 7950 4920 2874 7261  T from PyPI (tra
-00002120: 636b 696e 6720 606d 6173 7465 7260 2062  cking `master` b
-00002130: 7261 6e63 6829 206f 7220 5465 7374 5079  ranch) or TestPy
-00002140: 5049 2028 7472 6163 6b69 6e67 2060 6465  PI (tracking `de
-00002150: 7660 2062 7261 6e63 682c 2077 6869 6368  v` branch, which
-00002160: 2069 7320 6c61 7465 7374 2920 7573 696e   is latest) usin
-00002170: 6720 7069 702e 2046 6f72 2064 6576 656c  g pip. For devel
-00002180: 6f70 6572 7320 6f72 2065 7870 6572 6965  opers or experie
-00002190: 6e63 6564 2075 7365 7273 2c20 6469 7274  nced users, dirt
-000021a0: 7920 7275 6e20 6672 6f6d 2073 6f75 7263  y run from sourc
-000021b0: 6520 6973 2061 6c73 6f20 616e 206f 7074  e is also an opt
-000021c0: 696f 6e2e 0a0a 3c61 2068 7265 663d 2264  ion...<a href="d
-000021d0: 6f63 732f 6465 706c 6f79 6d65 6e74 2d67  ocs/deployment-g
-000021e0: 7569 6465 2e6d 6423 6f70 7469 6f6e 2d32  uide.md#option-2
-000021f0: 2d72 6169 6c77 6179 6170 7022 3e3c 696d  -railwayapp"><im
-00002200: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
-00002210: 6169 6c77 6179 2e61 7070 2f62 7574 746f  ailway.app/butto
-00002220: 6e2e 7376 6722 2068 6569 6768 743d 2233  n.svg" height="3
-00002230: 3022 2061 6c74 3d22 4465 706c 6f79 206f  0" alt="Deploy o
-00002240: 6e20 5261 696c 7761 7922 3e3c 2f61 3e0a  n Railway"></a>.
-00002250: 0a46 6f72 206d 6f72 6520 6465 7461 696c  .For more detail
-00002260: 732c 2072 6566 6572 2074 6f20 7468 6520  s, refer to the 
-00002270: 5b64 6570 6c6f 796d 656e 7420 6775 6964  [deployment guid
-00002280: 655d 2864 6f63 732f 6465 706c 6f79 6d65  e](docs/deployme
-00002290: 6e74 2d67 7569 6465 2e6d 6429 2e0a 0a23  nt-guide.md)...#
-000022a0: 2320 5472 616e 736c 6174 696f 6e0a 0a52  # Translation..R
-000022b0: 6561 6420 7468 6520 7472 616e 736c 6174  ead the translat
-000022c0: 696f 6e20 6775 6964 6520 5b68 6572 655d  ion guide [here]
-000022d0: 2864 6f63 732f 7472 616e 736c 6174 696f  (docs/translatio
-000022e0: 6e2d 6775 6964 652e 6d64 292e 0a0a 596f  n-guide.md)...Yo
-000022f0: 7520 6361 6e20 6865 6c70 2074 6f20 7472  u can help to tr
-00002300: 616e 736c 6174 6520 7468 6520 626f 7420  anslate the bot 
-00002310: 7573 696e 6720 5b48 6f73 7465 6420 5765  using [Hosted We
-00002320: 626c 6174 655d 2868 7474 7073 3a2f 2f68  blate](https://h
-00002330: 6f73 7465 642e 7765 626c 6174 652e 6f72  osted.weblate.or
-00002340: 672f 7072 6f6a 6563 7473 2f72 7373 2d74  g/projects/rss-t
-00002350: 6f2d 7465 6c65 6772 616d 2d62 6f74 2f29  o-telegram-bot/)
-00002360: 2e20 5370 6563 6961 6c20 7468 616e 6b73  . Special thanks
-00002370: 2074 6f20 7468 6569 7220 6672 6565 2068   to their free h
-00002380: 6f73 7469 6e67 2073 6572 7669 6365 2066  osting service f
-00002390: 6f72 206c 6962 7265 2070 726f 6a65 6374  or libre project
-000023a0: 7321 0a0a 3c61 2068 7265 663d 2268 7474  s!..<a href="htt
-000023b0: 7073 3a2f 2f68 6f73 7465 642e 7765 626c  ps://hosted.webl
-000023c0: 6174 652e 6f72 672f 656e 6761 6765 2f72  ate.org/engage/r
-000023d0: 7373 2d74 6f2d 7465 6c65 6772 616d 2d62  ss-to-telegram-b
-000023e0: 6f74 2f22 3e3c 696d 6720 7372 633d 2268  ot/"><img src="h
-000023f0: 7474 7073 3a2f 2f68 6f73 7465 642e 7765  ttps://hosted.we
-00002400: 626c 6174 652e 6f72 672f 7769 6467 6574  blate.org/widget
-00002410: 732f 7273 732d 746f 2d74 656c 6567 7261  s/rss-to-telegra
-00002420: 6d2d 626f 742f 2d2f 676c 6f73 7361 7279  m-bot/-/glossary
-00002430: 2f6d 756c 7469 2d61 7574 6f2e 7376 6722  /multi-auto.svg"
-00002440: 2077 6964 7468 203d 2022 3530 3022 2061   width = "500" a
-00002450: 6c74 3d22 2220 2f3e 3c2f 613e 0a0a 2323  lt="" /></a>..##
-00002460: 2055 7369 6e67 2074 6865 2070 7562 6c69   Using the publi
-00002470: 6320 626f 740a 0a54 6865 205b 7075 626c  c bot..The [publ
-00002480: 6963 2062 6f74 5d28 6874 7470 733a 2f2f  ic bot](https://
-00002490: 742e 6d65 2f52 5353 7454 5f42 6f74 2920  t.me/RSStT_Bot) 
-000024a0: 636f 6d65 7320 7769 7468 2061 6273 6f6c  comes with absol
-000024b0: 7574 656c 7920 6e6f 2077 6172 7261 6e74  utely no warrant
-000024c0: 792e 2049 2077 696c 6c20 7472 7920 6d79  y. I will try my
-000024d0: 2062 6573 7420 746f 206d 6169 6e74 6169   best to maintai
-000024e0: 6e20 6974 2c20 6275 7420 4920 6361 6e6e  n it, but I cann
-000024f0: 6f74 2067 7561 7261 6e74 6565 2074 6861  ot guarantee tha
-00002500: 7420 6974 2077 696c 6c20 616c 7761 7973  t it will always
-00002510: 2077 6f72 6b20 7065 7266 6563 746c 792e   work perfectly.
-00002520: 204d 6561 6e77 6869 6c65 2c20 796f 7520   Meanwhile, you 
-00002530: 7368 6f75 6c64 2022 6661 6972 2075 7365  should "fair use
-00002540: 2220 7468 6520 626f 742c 2061 766f 6964  " the bot, avoid
-00002550: 2073 7562 7363 7269 6269 6e67 2074 6f20   subscribing to 
-00002560: 746f 6f20 6d61 6e79 2052 5353 2066 6565  too many RSS fee
-00002570: 6473 2e20 200a 4966 2079 6f75 2075 7365  ds.  .If you use
-00002580: 2074 6865 205b 7075 626c 6963 2062 6f74   the [public bot
-00002590: 5d28 6874 7470 733a 2f2f 742e 6d65 2f52  ](https://t.me/R
-000025a0: 5353 7454 5f42 6f74 2920 696e 2079 6f75  SStT_Bot) in you
-000025b0: 7220 4368 616e 6e65 6c2c 2063 6f6e 7369  r Channel, consi
-000025c0: 6465 7220 6d65 6e74 696f 6e69 6e67 2074  der mentioning t
-000025d0: 6865 2062 6f74 2028 6f72 2074 6869 7320  he bot (or this 
-000025e0: 7072 6f6a 6563 7429 2069 6e20 796f 7572  project) in your
-000025f0: 2063 6861 6e6e 656c 2064 6573 6372 6970   channel descrip
-00002600: 7469 6f6e 2028 6f72 2070 696e 6e65 6420  tion (or pinned 
-00002610: 6d65 7373 6167 6529 2074 6f20 6c65 7420  message) to let 
-00002620: 6d6f 7265 2070 656f 706c 6520 6b6e 6f77  more people know
-00002630: 2061 626f 7574 2069 742e 2054 6861 7427   about it. That'
-00002640: 7320 6e6f 7420 6120 636f 6d70 756c 7369  s not a compulsi
-00002650: 6f6e 2e0a 0a23 2320 4b6e 6f77 6e20 6368  on...## Known ch
-00002660: 616e 6e65 6c73 2075 7369 6e67 2052 5353  annels using RSS
-00002670: 7454 0a0a 5761 6e74 2074 6f20 7072 6576  tT..Want to prev
-00002680: 6965 7720 7768 6174 2074 6865 206d 6573  iew what the mes
-00002690: 7361 6765 7320 7365 6e74 2062 7920 5253  sages sent by RS
-000026a0: 5374 5420 6c6f 6f6b 206c 696b 653f 2048  StT look like? H
-000026b0: 6572 6520 6973 2061 205b 6c69 7374 206f  ere is a [list o
-000026c0: 6620 6368 616e 6e65 6c73 2075 7369 6e67  f channels using
-000026d0: 2052 5353 7454 5d28 646f 6373 2f63 6861   RSStT](docs/cha
-000026e0: 6e6e 656c 732d 7573 696e 672d 7273 7374  nnels-using-rsst
-000026f0: 742e 6d64 292e 0a0a 2323 204c 6963 656e  t.md)...## Licen
-00002700: 7365 0a0a 5468 6973 2070 726f 6a65 6374  se..This project
-00002710: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00002720: 6572 205b 4147 504c 7633 5d28 4c49 4345  er [AGPLv3](LICE
-00002730: 4e53 4529 2e20 436c 6f73 6564 2d73 6f75  NSE). Closed-sou
-00002740: 7263 6520 6469 7374 7269 6275 7469 6f6e  rce distribution
-00002750: 206f 7220 626f 742d 686f 7374 696e 6720   or bot-hosting 
-00002760: 6172 6520 7374 7269 6374 6c79 2070 726f  are strictly pro
-00002770: 6869 6269 7465 642e 2049 6620 796f 7520  hibited. If you 
-00002780: 6d6f 6469 6679 2074 6865 2063 6f64 6520  modify the code 
-00002790: 616e 6420 6469 7374 7269 6275 7465 206f  and distribute o
-000027a0: 7220 686f 7374 2069 742c 206d 616b 6520  r host it, make 
-000027b0: 7375 7265 2061 6e79 2075 7365 7273 2077  sure any users w
-000027c0: 686f 2063 616e 2075 7365 2079 6f75 7220  ho can use your 
-000027d0: 626f 7420 6361 6e20 6765 7420 7468 6520  bot can get the 
-000027e0: 736f 7572 6365 2063 6f64 6520 2862 7920  source code (by 
-000027f0: 6564 6974 696e 6720 7468 6520 7265 706f  editing the repo
-00002800: 2055 524c 2069 6e20 5b60 7372 632f 6931   URL in [`src/i1
-00002810: 386e 2f5f 5f69 6e69 745f 5f2e 7079 605d  8n/__init__.py`]
-00002820: 2873 7263 2f69 3138 6e2f 5f5f 696e 6974  (src/i18n/__init
-00002830: 5f5f 2e70 7929 292e 0a0a 5468 6520 7265  __.py))...The re
-00002840: 706f 7369 746f 7279 2077 6173 2066 6f72  pository was for
-00002850: 6d65 726c 7920 6120 666f 726b 206f 6620  merly a fork of 
-00002860: 5b42 6f4b 4b65 522f 5253 532d 746f 2d54  [BoKKeR/RSS-to-T
-00002870: 656c 6567 7261 6d2d 426f 745d 2868 7474  elegram-Bot](htt
-00002880: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002890: 426f 4b4b 6552 2f52 5353 2d74 6f2d 5465  BoKKeR/RSS-to-Te
-000028a0: 6c65 6772 616d 2d42 6f74 292e 2054 6865  legram-Bot). The
-000028b0: 7920 6861 7665 2062 6565 6e20 656e 7469  y have been enti
-000028c0: 7265 6c79 2064 6966 6665 7265 6e74 2070  rely different p
-000028d0: 726f 6a65 6374 7320 7369 6e63 6520 7468  rojects since th
-000028e0: 6520 6561 726c 7920 6461 7973 206f 6620  e early days of 
-000028f0: 7468 6973 2070 726f 6a65 6374 2e0a       this project..
+00000550: 3a3a 2033 2e31 320a 436c 6173 7369 6669  :: 3.12.Classifi
+00000560: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000570: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000580: 6f6e 203a 3a20 496d 706c 656d 656e 7461  on :: Implementa
+00000590: 7469 6f6e 203a 3a20 4350 7974 686f 6e0a  tion :: CPython.
+000005a0: 436c 6173 7369 6669 6572 3a20 546f 7069  Classifier: Topi
+000005b0: 6320 3a3a 2043 6f6d 6d75 6e69 6361 7469  c :: Communicati
+000005c0: 6f6e 7320 3a3a 2043 6861 740a 436c 6173  ons :: Chat.Clas
+000005d0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+000005e0: 2049 6e74 6572 6e65 740a 436c 6173 7369   Internet.Classi
+000005f0: 6669 6572 3a20 546f 7069 6320 3a3a 204d  fier: Topic :: M
+00000600: 756c 7469 6d65 6469 610a 5265 7175 6972  ultimedia.Requir
+00000610: 6573 2d50 7974 686f 6e3a 203e 3d33 2e39  es-Python: >=3.9
+00000620: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
+00000630: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
+00000640: 6d61 726b 646f 776e 0a4c 6963 656e 7365  markdown.License
+00000650: 2d46 696c 653a 204c 4943 454e 5345 0a52  -File: LICENSE.R
+00000660: 6571 7569 7265 732d 4469 7374 3a20 6372  equires-Dist: cr
+00000670: 7970 7467 3d3d 302e 342e 300a 5265 7175  yptg==0.4.0.Requ
+00000680: 6972 6573 2d44 6973 743a 2074 656c 6574  ires-Dist: telet
+00000690: 686f 6e3d 3d31 2e33 352e 300a 5265 7175  hon==1.35.0.Requ
+000006a0: 6972 6573 2d44 6973 743a 2061 696f 6772  ires-Dist: aiogr
+000006b0: 6170 6866 6978 3d3d 302e 322e 320a 5265  aphfix==0.2.2.Re
+000006c0: 7175 6972 6573 2d44 6973 743a 2066 6565  quires-Dist: fee
+000006d0: 6470 6172 7365 723d 3d36 2e30 2e31 310a  dparser==6.0.11.
+000006e0: 5265 7175 6972 6573 2d44 6973 743a 206c  Requires-Dist: l
+000006f0: 6973 7470 6172 7365 725b 6c78 6d6c 5d3d  istparser[lxml]=
+00000700: 3d30 2e32 300a 5265 7175 6972 6573 2d44  =0.20.Requires-D
+00000710: 6973 743a 2070 696c 6c6f 773d 3d31 302e  ist: pillow==10.
+00000720: 332e 300a 5265 7175 6972 6573 2d44 6973  3.0.Requires-Dis
+00000730: 743a 2062 6561 7574 6966 756c 736f 7570  t: beautifulsoup
+00000740: 343d 3d34 2e31 322e 330a 5265 7175 6972  4==4.12.3.Requir
+00000750: 6573 2d44 6973 743a 206c 786d 6c3d 3d35  es-Dist: lxml==5
+00000760: 2e32 2e31 0a52 6571 7569 7265 732d 4469  .2.1.Requires-Di
+00000770: 7374 3a20 7261 7069 6466 757a 7a3d 3d33  st: rapidfuzz==3
+00000780: 2e39 2e30 0a52 6571 7569 7265 732d 4469  .9.0.Requires-Di
+00000790: 7374 3a20 656d 6f6a 693d 3d32 2e31 312e  st: emoji==2.11.
+000007a0: 310a 5265 7175 6972 6573 2d44 6973 743a  1.Requires-Dist:
+000007b0: 206d 696e 6966 792d 6874 6d6c 3d3d 302e   minify-html==0.
+000007c0: 3135 2e30 0a52 6571 7569 7265 732d 4469  15.0.Requires-Di
+000007d0: 7374 3a20 6d69 6e69 6679 2d68 746d 6c2d  st: minify-html-
+000007e0: 6f6e 6570 6173 733d 3d30 2e31 352e 300a  onepass==0.15.0.
+000007f0: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
+00000800: 6174 706c 6f74 6c69 623d 3d33 2e38 2e34  atplotlib==3.8.4
+00000810: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000820: 6173 796e 6370 673d 3d30 2e32 392e 300a  asyncpg==0.29.0.
+00000830: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000840: 6f72 746f 6973 652d 6f72 6d5b 6163 6365  ortoise-orm[acce
+00000850: 6c5d 3d3d 302e 3230 2e31 0a52 6571 7569  l]==0.20.1.Requi
+00000860: 7265 732d 4469 7374 3a20 6165 7269 6368  res-Dist: aerich
+00000870: 3d3d 302e 372e 320a 5265 7175 6972 6573  ==0.7.2.Requires
+00000880: 2d44 6973 743a 2061 696f 6874 7470 5b73  -Dist: aiohttp[s
+00000890: 7065 6564 7570 735d 3d3d 332e 392e 350a  peedups]==3.9.5.
+000008a0: 5265 7175 6972 6573 2d44 6973 743a 2061  Requires-Dist: a
+000008b0: 696f 6874 7470 2d73 6f63 6b73 3d3d 302e  iohttp-socks==0.
+000008c0: 382e 340a 5265 7175 6972 6573 2d44 6973  8.4.Requires-Dis
+000008d0: 743a 2061 696f 6874 7470 2d72 6574 7279  t: aiohttp-retry
+000008e0: 3d3d 322e 382e 330a 5265 7175 6972 6573  ==2.8.3.Requires
+000008f0: 2d44 6973 743a 2070 7974 686f 6e2d 736f  -Dist: python-so
+00000900: 636b 735b 6173 796e 6369 6f5d 3d3d 322e  cks[asyncio]==2.
+00000910: 342e 340a 5265 7175 6972 6573 2d44 6973  4.4.Requires-Dis
+00000920: 743a 2064 6e73 7079 7468 6f6e 5b69 646e  t: dnspython[idn
+00000930: 615d 3d3d 322e 362e 310a 5265 7175 6972  a]==2.6.1.Requir
+00000940: 6573 2d44 6973 743a 2063 6f6c 6f72 6c6f  es-Dist: colorlo
+00000950: 673d 3d36 2e38 2e32 0a52 6571 7569 7265  g==6.8.2.Require
+00000960: 732d 4469 7374 3a20 4150 5363 6865 6475  s-Dist: APSchedu
+00000970: 6c65 723d 3d33 2e31 302e 340a 5265 7175  ler==3.10.4.Requ
+00000980: 6972 6573 2d44 6973 743a 2070 7974 686f  ires-Dist: pytho
+00000990: 6e2d 646f 7465 6e76 3d3d 312e 302e 310a  n-dotenv==1.0.1.
+000009a0: 5265 7175 6972 6573 2d44 6973 743a 206d  Requires-Dist: m
+000009b0: 756c 7469 6469 6374 3d3d 362e 302e 350a  ultidict==6.0.5.
+000009c0: 5265 7175 6972 6573 2d44 6973 743a 2061  Requires-Dist: a
+000009d0: 7379 6e63 7374 646c 6962 3d3d 332e 3132  syncstdlib==3.12
+000009e0: 2e33 0a52 6571 7569 7265 732d 4469 7374  .3.Requires-Dist
+000009f0: 3a20 6361 6368 6574 6f6f 6c73 3d3d 352e  : cachetools==5.
+00000a00: 332e 330a 5265 7175 6972 6573 2d44 6973  3.3.Requires-Dis
+00000a10: 743a 2043 4a4b 7772 6170 3d3d 322e 320a  t: CJKwrap==2.2.
+00000a20: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000a30: 7970 696e 672d 6578 7465 6e73 696f 6e73  yping-extensions
+00000a40: 3d3d 342e 3131 2e30 0a52 6571 7569 7265  ==4.11.0.Require
+00000a50: 732d 4469 7374 3a20 7576 6c6f 6f70 3d3d  s-Dist: uvloop==
+00000a60: 302e 3139 2e30 3b20 7379 735f 706c 6174  0.19.0; sys_plat
+00000a70: 666f 726d 2021 3d20 2277 696e 3332 2220  form != "win32" 
+00000a80: 616e 6420 7379 735f 706c 6174 666f 726d  and sys_platform
+00000a90: 2021 3d20 2263 7967 7769 6e22 2061 6e64   != "cygwin" and
+00000aa0: 2073 7973 5f70 6c61 7466 6f72 6d20 213d   sys_platform !=
+00000ab0: 2022 636c 6922 0a52 6571 7569 7265 732d   "cli".Requires-
+00000ac0: 4469 7374 3a20 6973 616c 3d3d 312e 362e  Dist: isal==1.6.
+00000ad0: 313b 2070 6c61 7466 6f72 6d5f 6d61 6368  1; platform_mach
+00000ae0: 696e 6520 3d3d 2022 7838 365f 3634 2220  ine == "x86_64" 
+00000af0: 6f72 2070 6c61 7466 6f72 6d5f 6d61 6368  or platform_mach
+00000b00: 696e 6520 3d3d 2022 414d 4436 3422 206f  ine == "AMD64" o
+00000b10: 7220 706c 6174 666f 726d 5f6d 6163 6869  r platform_machi
+00000b20: 6e65 203d 3d20 2261 6172 6368 3634 220a  ne == "aarch64".
+00000b30: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00000b40: 7222 3e0a 3c69 6d67 2073 7263 3d22 646f  r">.<img src="do
+00000b50: 6373 2f72 6573 6f75 7263 6573 2f52 5353  cs/resources/RSS
+00000b60: 7454 5f69 636f 6e2e 7376 6722 2061 6c74  tT_icon.svg" alt
+00000b70: 3d22 5253 5320 746f 2054 656c 6567 7261  ="RSS to Telegra
+00000b80: 6d20 426f 7422 2077 6964 7468 3d22 3130  m Bot" width="10
+00000b90: 3022 3e0a 3c2f 703e 0a3c 6831 2061 6c69  0">.</p>.<h1 ali
+00000ba0: 676e 3d22 6365 6e74 6572 223e 5253 5320  gn="center">RSS 
+00000bb0: 746f 2054 656c 6567 7261 6d20 426f 743c  to Telegram Bot<
+00000bc0: 2f68 313e 0a0a 3c70 2061 6c69 676e 3d22  /h1>..<p align="
+00000bd0: 6365 6e74 6572 223e 3c62 3e41 2054 656c  center"><b>A Tel
+00000be0: 6567 7261 6d20 5253 5320 626f 7420 7468  egram RSS bot th
+00000bf0: 6174 2063 6172 6573 2061 626f 7574 2079  at cares about y
+00000c00: 6f75 7220 7265 6164 696e 6720 6578 7065  our reading expe
+00000c10: 7269 656e 6365 3c2f 623e 3c2f 703e 0a0a  rience</b></p>..
+00000c20: 5b21 5b47 6974 4875 6220 636f 6d6d 6974  [![GitHub commit
+00000c30: 2061 6374 6976 6974 795d 2868 7474 7073   activity](https
+00000c40: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000c50: 6f2f 6769 7468 7562 2f63 6f6d 6d69 742d  o/github/commit-
+00000c60: 6163 7469 7669 7479 2f6d 2f52 6f6e 6772  activity/m/Rongr
+00000c70: 6f6e 6767 6739 2f52 5353 2d74 6f2d 5465  onggg9/RSS-to-Te
+00000c80: 6c65 6772 616d 2d42 6f74 3f6c 6f67 6f3d  legram-Bot?logo=
+00000c90: 6769 7426 6c61 6265 6c3d 636f 6d6d 6974  git&label=commit
+00000ca0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000cb0: 622e 636f 6d2f 526f 6e67 726f 6e67 6767  b.com/Rongronggg
+00000cc0: 392f 5253 532d 746f 2d54 656c 6567 7261  9/RSS-to-Telegra
+00000cd0: 6d2d 426f 742f 636f 6d6d 6974 7329 0a5b  m-Bot/commits).[
+00000ce0: 215b 5472 616e 736c 6174 696e 6720 7374  ![Translating st
+00000cf0: 6174 7573 5d28 6874 7470 733a 2f2f 696d  atus](https://im
+00000d00: 672e 7368 6965 6c64 732e 696f 2f77 6562  g.shields.io/web
+00000d10: 6c61 7465 2f70 726f 6772 6573 732f 7273  late/progress/rs
+00000d20: 732d 746f 2d74 656c 6567 7261 6d2d 626f  s-to-telegram-bo
+00000d30: 743f 6c6f 676f 3d77 6562 6c61 7465 2663  t?logo=weblate&c
+00000d40: 6f6c 6f72 3d69 6e66 6f72 6d61 7469 6f6e  olor=information
+00000d50: 616c 295d 2868 7474 7073 3a2f 2f68 6f73  al)](https://hos
+00000d60: 7465 642e 7765 626c 6174 652e 6f72 672f  ted.weblate.org/
+00000d70: 656e 6761 6765 2f72 7373 2d74 6f2d 7465  engage/rss-to-te
+00000d80: 6c65 6772 616d 2d62 6f74 2f29 0a5b 215b  legram-bot/).[![
+00000d90: 436f 6465 2071 7561 6c69 7479 5d28 6874  Code quality](ht
+00000da0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000db0: 732e 696f 2f63 6f64 6566 6163 746f 722f  s.io/codefactor/
+00000dc0: 6772 6164 652f 6769 7468 7562 2f52 6f6e  grade/github/Ron
+00000dd0: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
+00000de0: 5465 6c65 6772 616d 2d42 6f74 3f6c 6f67  Telegram-Bot?log
+00000df0: 6f3d 636f 6465 6661 6374 6f72 295d 2868  o=codefactor)](h
+00000e00: 7474 7073 3a2f 2f77 7777 2e63 6f64 6566  ttps://www.codef
+00000e10: 6163 746f 722e 696f 2f72 6570 6f73 6974  actor.io/reposit
+00000e20: 6f72 792f 6769 7468 7562 2f72 6f6e 6772  ory/github/rongr
+00000e30: 6f6e 6767 6739 2f72 7373 2d74 6f2d 7465  onggg9/rss-to-te
+00000e40: 6c65 6772 616d 2d62 6f74 290a 5b21 5b47  legram-bot).[![G
+00000e50: 6974 4875 6220 7374 6172 735d 2868 7474  itHub stars](htt
+00000e60: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000e70: 2e69 6f2f 6769 7468 7562 2f73 7461 7273  .io/github/stars
+00000e80: 2f52 6f6e 6772 6f6e 6767 6739 2f52 7373  /Rongronggg9/Rss
+00000e90: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
+00000ea0: 3f73 7479 6c65 3d73 6f63 6961 6c29 5d28  ?style=social)](
+00000eb0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000ec0: 6f6d 2f52 6f6e 6772 6f6e 6767 6739 2f52  om/Rongronggg9/R
+00000ed0: 5353 2d74 6f2d 5465 6c65 6772 616d 2d42  SS-to-Telegram-B
+00000ee0: 6f74 2f73 7461 7267 617a 6572 7329 0a5b  ot/stargazers).[
+00000ef0: 215b 4769 7448 7562 2066 6f72 6b73 5d28  ![GitHub forks](
+00000f00: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000f10: 6c64 732e 696f 2f67 6974 6875 622f 666f  lds.io/github/fo
+00000f20: 726b 732f 526f 6e67 726f 6e67 6767 392f  rks/Rongronggg9/
+00000f30: 5253 532d 746f 2d54 656c 6567 7261 6d2d  RSS-to-Telegram-
+00000f40: 426f 743f 7374 796c 653d 736f 6369 616c  Bot?style=social
+00000f50: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+00000f60: 622e 636f 6d2f 526f 6e67 726f 6e67 6767  b.com/Rongronggg
+00000f70: 392f 5253 532d 746f 2d54 656c 6567 7261  9/RSS-to-Telegra
+00000f80: 6d2d 426f 742f 666f 726b 290a 0a5b 215b  m-Bot/fork)..[![
+00000f90: 5465 6c65 6772 616d 2062 6f74 5d28 6874  Telegram bot](ht
+00000fa0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000fb0: 732e 696f 2f62 6164 6765 2f54 656c 6567  s.io/badge/Teleg
+00000fc0: 7261 6d25 3230 426f 742d 2534 3052 5353  ram%20Bot-%40RSS
+00000fd0: 7454 5f5f 426f 742d 3232 3965 6439 3f6c  tT__Bot-229ed9?l
+00000fe0: 6f67 6f3d 7465 6c65 6772 616d 2673 7479  ogo=telegram&sty
+00000ff0: 6c65 3d66 6f72 2d74 6865 2d62 6164 6765  le=for-the-badge
+00001000: 295d 2868 7474 7073 3a2f 2f74 2e6d 652f  )](https://t.me/
+00001010: 5253 5374 545f 426f 7429 0a5b 215b 5465  RSStT_Bot).[![Te
+00001020: 6c65 6772 616d 2067 726f 7570 5d28 6874  legram group](ht
+00001030: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00001040: 732e 696f 2f62 6164 6765 2f64 796e 616d  s.io/badge/dynam
+00001050: 6963 2f6a 736f 6e3f 7572 6c3d 6874 7470  ic/json?url=http
+00001060: 7325 3341 2532 4625 3246 6170 692e 7377  s%3A%2F%2Fapi.sw
+00001070: 6f2e 6d6f 6525 3246 7374 6174 7325 3246  o.moe%2Fstats%2F
+00001080: 7465 6c65 6772 616d 2532 4652 5353 7454  telegram%2FRSStT
+00001090: 5f47 726f 7570 2671 7565 7279 3d63 6f75  _Group&query=cou
+000010a0: 6e74 2663 6f6c 6f72 3d32 4341 3545 3026  nt&color=2CA5E0&
+000010b0: 6c61 6265 6c3d 5465 6c65 6772 616d 2532  label=Telegram%2
+000010c0: 3047 726f 7570 266c 6f67 6f3d 7465 6c65  0Group&logo=tele
+000010d0: 6772 616d 2663 6163 6865 5365 636f 6e64  gram&cacheSecond
+000010e0: 733d 3336 3030 2673 7479 6c65 3d66 6f72  s=3600&style=for
+000010f0: 2d74 6865 2d62 6164 6765 295d 2868 7474  -the-badge)](htt
+00001100: 7073 3a2f 2f74 2e6d 652f 5253 5374 545f  ps://t.me/RSStT_
+00001110: 4772 6f75 7029 0a5b 215b 5465 6c65 6772  Group).[![Telegr
+00001120: 616d 2063 6861 6e6e 656c 5d28 6874 7470  am channel](http
+00001130: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00001140: 696f 2f62 6164 6765 2f64 796e 616d 6963  io/badge/dynamic
+00001150: 2f6a 736f 6e3f 7572 6c3d 6874 7470 7325  /json?url=https%
+00001160: 3341 2532 4625 3246 6170 692e 7377 6f2e  3A%2F%2Fapi.swo.
+00001170: 6d6f 6525 3246 7374 6174 7325 3246 7465  moe%2Fstats%2Fte
+00001180: 6c65 6772 616d 2532 4652 5353 7454 5f43  legram%2FRSStT_C
+00001190: 6861 6e6e 656c 2671 7565 7279 3d63 6f75  hannel&query=cou
+000011a0: 6e74 2663 6f6c 6f72 3d32 4341 3545 3026  nt&color=2CA5E0&
+000011b0: 6c61 6265 6c3d 5465 6c65 6772 616d 2532  label=Telegram%2
+000011c0: 3043 6861 6e6e 656c 266c 6f67 6f3d 7465  0Channel&logo=te
+000011d0: 6c65 6772 616d 2663 6163 6865 5365 636f  legram&cacheSeco
+000011e0: 6e64 733d 3336 3030 2673 7479 6c65 3d66  nds=3600&style=f
+000011f0: 6f72 2d74 6865 2d62 6164 6765 295d 2868  or-the-badge)](h
+00001200: 7474 7073 3a2f 2f74 2e6d 652f 5253 5374  ttps://t.me/RSSt
+00001210: 545f 4368 616e 6e65 6c29 0a0a 7c20 5be7  T_Channel)..| [.
+00001220: ae80 e4bd 93e4 b8ad e696 8720 5245 4144  ........... READ
+00001230: 4d45 5d20 7c20 5b43 4841 4e47 454c 4f47  ME] | [CHANGELOG
+00001240: 5d20 7c20 5b46 4151 5d20 7c20 5b44 6f63  ] | [FAQ] | [Doc
+00001250: 756d 656e 7461 7469 6f6e 5d20 7c20 5b43  umentation] | [C
+00001260: 6861 6e6e 656c 7320 5573 696e 6720 5253  hannels Using RS
+00001270: 5374 545d 207c 0a7c 3a2d 2d2d 2d2d 2d2d  StT] |.|:-------
+00001280: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
+00001290: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 3a7c 2d2d  ----:|:-----:|--
+000012a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+000012b0: 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :---------------
+000012c0: 2d2d 2d2d 2d2d 2d3a 7c0a 0a5b e7ae 80e4  -------:|..[....
+000012d0: bd93 e4b8 ade6 9687 2052 4541 444d 455d  ........ README]
+000012e0: 3a20 5245 4144 4d45 2e7a 682e 6d64 0a0a  : README.zh.md..
+000012f0: 5b43 4841 4e47 454c 4f47 5d3a 2064 6f63  [CHANGELOG]: doc
+00001300: 732f 4348 414e 4745 4c4f 472e 6d64 0a0a  s/CHANGELOG.md..
+00001310: 5b46 4151 5d3a 2064 6f63 732f 4641 512e  [FAQ]: docs/FAQ.
+00001320: 6d64 0a0a 5b44 6f63 756d 656e 7461 7469  md..[Documentati
+00001330: 6f6e 5d3a 2064 6f63 730a 0a5b 4368 616e  on]: docs..[Chan
+00001340: 6e65 6c73 2055 7369 6e67 2052 5353 7454  nels Using RSStT
+00001350: 5d3a 2064 6f63 732f 6368 616e 6e65 6c73  ]: docs/channels
+00001360: 2d75 7369 6e67 2d72 7373 7474 2e6d 640a  -using-rsstt.md.
+00001370: 0a3c 7461 626c 653e 0a20 2020 203c 7472  .<table>.    <tr
+00001380: 3e0a 2020 2020 2020 2020 3c74 643e 3c69  >.        <td><i
+00001390: 6d67 2073 7263 3d22 646f 6373 2f72 6573  mg src="docs/res
+000013a0: 6f75 7263 6573 2f65 7861 6d70 6c65 352e  ources/example5.
+000013b0: 706e 6722 2061 6c74 3d22 5363 7265 656e  png" alt="Screen
+000013c0: 7368 6f74 223e 3c2f 7464 3e0a 2020 2020  shot"></td>.    
+000013d0: 2020 2020 3c74 6420 726f 7773 7061 6e3d      <td rowspan=
+000013e0: 2232 223e 3c69 6d67 2073 7263 3d22 646f  "2"><img src="do
+000013f0: 6373 2f72 6573 6f75 7263 6573 2f65 7861  cs/resources/exa
+00001400: 6d70 6c65 372e 706e 6722 2061 6c74 3d22  mple7.png" alt="
+00001410: 5363 7265 656e 7368 6f74 223e 3c2f 7464  Screenshot"></td
+00001420: 3e0a 2020 2020 2020 2020 3c74 6420 726f  >.        <td ro
+00001430: 7773 7061 6e3d 2232 223e 3c69 6d67 2073  wspan="2"><img s
+00001440: 7263 3d22 646f 6373 2f72 6573 6f75 7263  rc="docs/resourc
+00001450: 6573 2f65 7861 6d70 6c65 382e 706e 6722  es/example8.png"
+00001460: 2061 6c74 3d22 5363 7265 656e 7368 6f74   alt="Screenshot
+00001470: 223e 3c2f 7464 3e0a 2020 2020 3c2f 7472  "></td>.    </tr
+00001480: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00001490: 2020 203c 7464 3e3c 696d 6720 7372 633d     <td><img src=
+000014a0: 2264 6f63 732f 7265 736f 7572 6365 732f  "docs/resources/
+000014b0: 6578 616d 706c 6536 2e70 6e67 2220 616c  example6.png" al
+000014c0: 743d 2253 6372 6565 6e73 686f 7422 3e3c  t="Screenshot"><
+000014d0: 2f74 643e 0a20 2020 203c 2f74 723e 0a3c  /td>.    </tr>.<
+000014e0: 2f74 6162 6c65 3e0a 0a23 2320 4869 6768  /table>..## High
+000014f0: 6c69 6768 7473 0a0a 2d20 4d75 6c74 692d  lights..- Multi-
+00001500: 7573 6572 0a2d 2049 3138 6e0a 2020 2020  user.- I18n.    
+00001510: 2d20 456e 676c 6973 682c 2043 6869 6e65  - English, Chine
+00001520: 7365 2c20 4361 6e74 6f6e 6573 652c 2049  se, Cantonese, I
+00001530: 7461 6c69 616e 2c20 616e 6420 5b6d 6f72  talian, and [mor
+00001540: 655d 2864 6f63 732f 7472 616e 736c 6174  e](docs/translat
+00001550: 696f 6e2d 6775 6964 652e 6d64 2921 0a2d  ion-guide.md)!.-
+00001560: 2054 6865 2063 6f6e 7465 6e74 206f 6620   The content of 
+00001570: 7468 6520 706f 7374 7320 6f66 2061 6e20  the posts of an 
+00001580: 5253 5320 6665 6564 2077 696c 6c20 6265  RSS feed will be
+00001590: 2073 656e 7420 746f 2054 656c 6567 7261   sent to Telegra
+000015a0: 6d0a 2020 2020 2d20 4b65 6570 2072 6963  m.    - Keep ric
+000015b0: 682d 7465 7874 2066 6f72 6d61 740a 2020  h-text format.  
+000015c0: 2020 2d20 4b65 6570 206d 6564 6961 2028    - Keep media (
+000015d0: 6375 7374 6f6d 697a 6162 6c65 290a 2020  customizable).  
+000015e0: 2020 2020 2020 2d20 496d 6167 6573 2c20        - Images, 
+000015f0: 5669 6465 6f73 2c20 616e 6420 4175 6469  Videos, and Audi
+00001600: 6f20 626f 7468 2069 6e20 7468 6520 706f  o both in the po
+00001610: 7374 2063 6f6e 7465 6e74 2061 6e64 2065  st content and e
+00001620: 6e63 6c6f 7375 7265 3b20 446f 6375 6d65  nclosure; Docume
+00001630: 6e74 7320 696e 2074 6865 2070 6f73 7420  nts in the post 
+00001640: 656e 636c 6f73 7572 650a 2020 2020 2020  enclosure.      
+00001650: 2020 2d20 4c6f 6e67 2069 6d61 6765 7320    - Long images 
+00001660: 7769 6c6c 2062 6520 7365 6e74 2061 7320  will be sent as 
+00001670: 6669 6c65 7320 746f 2070 7265 7665 6e74  files to prevent
+00001680: 2054 656c 6567 7261 6d20 6672 6f6d 2063   Telegram from c
+00001690: 6f6d 7072 6573 7369 6e67 2074 6865 2069  ompressing the i
+000016a0: 6d61 6765 2061 6e64 206d 616b 696e 6720  mage and making 
+000016b0: 6974 2075 6e72 6561 6461 626c 650a 2020  it unreadable.  
+000016c0: 2020 2020 2020 2d20 4472 6f70 2061 6e6e        - Drop ann
+000016d0: 6f79 696e 6720 6963 6f6e 732c 2074 6865  oying icons, the
+000016e0: 7920 6272 6561 6b20 7468 6520 7265 6164  y break the read
+000016f0: 696e 6720 6578 7065 7269 656e 6365 0a20  ing experience. 
+00001700: 2020 202d 2041 7574 6f6d 6174 6963 616c     - Automatical
+00001710: 6c79 2072 6570 6c61 6365 2065 6d6f 6a69  ly replace emoji
+00001720: 2073 686f 7274 636f 6465 7320 7769 7468   shortcodes with
+00001730: 2065 6d6f 6a69 0a20 2020 202d 2041 7574   emoji.    - Aut
+00001740: 6f6d 6174 6963 616c 6c79 2072 6570 6c61  omatically repla
+00001750: 6365 2065 6d6f 6a69 2069 6d61 6765 7320  ce emoji images 
+00001760: 7769 7468 2065 6d6f 6a69 206f 7220 6974  with emoji or it
+00001770: 7320 6465 7363 7269 7074 696f 6e20 7465  s description te
+00001780: 7874 0a20 2020 202d 2041 7574 6f6d 6174  xt.    - Automat
+00001790: 6963 616c 6c79 2064 6574 6572 6d69 6e65  ically determine
+000017a0: 2077 6865 7468 6572 2074 6865 2074 6974   whether the tit
+000017b0: 6c65 206f 6620 7468 6520 5253 5320 6665  le of the RSS fe
+000017c0: 6564 2069 7320 6175 746f 2d66 696c 6c65  ed is auto-fille
+000017d0: 642c 2069 6620 736f 2c20 6f6d 6974 2074  d, if so, omit t
+000017e0: 6865 2074 6974 6c65 2028 6375 7374 6f6d  he title (custom
+000017f0: 697a 6162 6c65 290a 2020 2020 2d20 4175  izable).    - Au
+00001800: 746f 6d61 7469 6361 6c6c 7920 7368 6f77  tomatically show
+00001810: 2074 6865 2061 7574 686f 722d 6e61 6d65   the author-name
+00001820: 2028 6375 7374 6f6d 697a 6162 6c65 290a   (customizable).
+00001830: 2020 2020 2d20 4175 746f 6d61 7469 6361      - Automatica
+00001840: 6c6c 7920 7370 6c69 7420 746f 6f2d 6c6f  lly split too-lo
+00001850: 6e67 206d 6573 7361 6765 730a 2020 2020  ng messages.    
+00001860: 2d20 4d65 7373 6167 6573 2063 616e 2062  - Messages can b
+00001870: 6520 7365 6e74 2061 7320 5465 6c65 6772  e sent as Telegr
+00001880: 6170 6820 706f 7374 7320 2863 7573 746f  aph posts (custo
+00001890: 6d69 7a61 626c 6529 0a20 2020 2020 202d  mizable).      -
+000018a0: 204d 6f73 7420 696d 6167 6573 2061 6e64   Most images and
+000018b0: 2076 6964 656f 7320 7769 6c6c 2062 6520   videos will be 
+000018c0: 7570 6c6f 6164 6564 2074 6f20 5465 6c65  uploaded to Tele
+000018d0: 6772 6170 682c 2073 6f20 7468 6174 2049  graph, so that I
+000018e0: 6e73 7461 6e74 2056 6965 7720 7769 6c6c  nstant View will
+000018f0: 206c 6f61 6420 7261 7069 646c 790a 2d20   load rapidly.- 
+00001900: 5b56 6172 696f 7573 2063 7573 746f 6d69  [Various customi
+00001910: 7a61 626c 6520 666f 726d 6174 7469 6e67  zable formatting
+00001920: 2073 6574 7469 6e67 735d 2864 6f63 732f   settings](docs/
+00001930: 666f 726d 6174 7469 6e67 2d73 6574 7469  formatting-setti
+00001940: 6e67 732e 6d64 290a 2020 2020 2d20 4861  ngs.md).    - Ha
+00001950: 7368 7461 6773 2c20 6375 7374 6f6d 2074  shtags, custom t
+00001960: 6974 6c65 2c20 6574 632e 0a2d 2049 6e64  itle, etc..- Ind
+00001970: 6976 6964 7561 6c20 7072 6f78 7920 7365  ividual proxy se
+00001980: 7474 696e 6773 2066 6f72 2054 656c 6567  ttings for Teleg
+00001990: 7261 6d20 616e 6420 5253 5320 6665 6564  ram and RSS feed
+000019a0: 730a 2d20 4f50 4d4c 2069 6d70 6f72 7469  s.- OPML importi
+000019b0: 6e67 2061 6e64 2065 7870 6f72 7469 6e67  ng and exporting
+000019c0: 2028 6b65 6570 2063 7573 746f 6d20 7469   (keep custom ti
+000019d0: 746c 6529 0a2d 204f 7074 696d 697a 6564  tle).- Optimized
+000019e0: 2070 6572 666f 726d 616e 6365 2028 7365   performance (se
+000019f0: 6520 616c 736f 2074 6865 205b 4641 515d  e also the [FAQ]
+00001a00: 2864 6f63 732f 4641 512e 6d64 2371 2d68  (docs/FAQ.md#q-h
+00001a10: 6f77 2d69 732d 7468 652d 7065 7266 6f72  ow-is-the-perfor
+00001a20: 6d61 6e63 652d 6f66 2d74 6865 2d62 6f74  mance-of-the-bot
+00001a30: 2929 0a2d 2055 7365 722d 6672 6965 6e64  )).- User-friend
+00001a40: 6c79 0a2d 2048 5454 5020 4361 6368 696e  ly.- HTTP Cachin
+00001a50: 670a 0a23 2320 4465 706c 6f79 6d65 6e74  g..## Deployment
+00001a60: 0a0a 5b21 5b64 6f63 6b65 7269 2e63 6f5d  ..[![dockeri.co]
+00001a70: 2868 7474 7073 3a2f 2f64 6f63 6b65 7269  (https://dockeri
+00001a80: 636f 2e62 6c61 6e6b 656e 7368 6970 2e69  co.blankenship.i
+00001a90: 6f2f 696d 6167 652f 726f 6e67 726f 6e67  o/image/rongrong
+00001aa0: 6767 392f 7273 732d 746f 2d74 656c 6567  gg9/rss-to-teleg
+00001ab0: 7261 6d29 5d28 6874 7470 733a 2f2f 6875  ram)](https://hu
+00001ac0: 622e 646f 636b 6572 2e63 6f6d 2f72 2f72  b.docker.com/r/r
+00001ad0: 6f6e 6772 6f6e 6767 6739 2f72 7373 2d74  ongronggg9/rss-t
+00001ae0: 6f2d 7465 6c65 6772 616d 295c 0a5b 215b  o-telegram)\.[![
+00001af0: 4275 696c 6420 7374 6174 7573 2028 6d61  Build status (ma
+00001b00: 7374 6572 295d 2868 7474 7073 3a2f 2f69  ster)](https://i
+00001b10: 6d67 2e73 6869 656c 6473 2e69 6f2f 6769  mg.shields.io/gi
+00001b20: 7468 7562 2f61 6374 696f 6e73 2f77 6f72  thub/actions/wor
+00001b30: 6b66 6c6f 772f 7374 6174 7573 2f52 6f6e  kflow/status/Ron
+00001b40: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
+00001b50: 5465 6c65 6772 616d 2d42 6f74 2f70 7562  Telegram-Bot/pub
+00001b60: 6c69 7368 2d64 6f63 6b65 722d 696d 6167  lish-docker-imag
+00001b70: 652e 796d 6c3f 6272 616e 6368 3d6d 6173  e.yml?branch=mas
+00001b80: 7465 7226 6c61 6265 6c3d 6275 696c 6426  ter&label=build&
+00001b90: 6c6f 676f 3d64 6f63 6b65 7229 5d28 6874  logo=docker)](ht
+00001ba0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001bb0: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
+00001bc0: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
+00001bd0: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00001be0: 7773 2f70 7562 6c69 7368 2d64 6f63 6b65  ws/publish-docke
+00001bf0: 722d 696d 6167 652e 796d 6c3f 7175 6572  r-image.yml?quer
+00001c00: 793d 6272 616e 6368 2533 416d 6173 7465  y=branch%3Amaste
+00001c10: 7229 0a5b 215b 4275 696c 6420 7374 6174  r).[![Build stat
+00001c20: 7573 2028 6465 7629 5d28 6874 7470 733a  us (dev)](https:
+00001c30: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001c40: 2f67 6974 6875 622f 6163 7469 6f6e 732f  /github/actions/
+00001c50: 776f 726b 666c 6f77 2f73 7461 7475 732f  workflow/status/
+00001c60: 526f 6e67 726f 6e67 6767 392f 5253 532d  Rongronggg9/RSS-
+00001c70: 746f 2d54 656c 6567 7261 6d2d 426f 742f  to-Telegram-Bot/
+00001c80: 7075 626c 6973 682d 646f 636b 6572 2d69  publish-docker-i
+00001c90: 6d61 6765 2e79 6d6c 3f62 7261 6e63 683d  mage.yml?branch=
+00001ca0: 6465 7626 6c61 6265 6c3d 6275 696c 6425  dev&label=build%
+00001cb0: 3230 2532 3864 6576 2532 3926 6c6f 676f  20%28dev%29&logo
+00001cc0: 3d64 6f63 6b65 7229 5d28 6874 7470 733a  =docker)](https:
+00001cd0: 2f2f 6769 7468 7562 2e63 6f6d 2f52 6f6e  //github.com/Ron
+00001ce0: 6772 6f6e 6767 6739 2f52 5353 2d74 6f2d  gronggg9/RSS-to-
+00001cf0: 5465 6c65 6772 616d 2d42 6f74 2f61 6374  Telegram-Bot/act
+00001d00: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f70  ions/workflows/p
+00001d10: 7562 6c69 7368 2d64 6f63 6b65 722d 696d  ublish-docker-im
+00001d20: 6167 652e 796d 6c3f 7175 6572 793d 6272  age.yml?query=br
+00001d30: 616e 6368 2533 4164 6576 290a 0a5b 215b  anch%3Adev)..[![
+00001d40: 5079 5049 5d28 6874 7470 733a 2f2f 696d  PyPI](https://im
+00001d50: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00001d60: 692f 762f 7273 7374 743f 6c6f 676f 3d70  i/v/rsstt?logo=p
+00001d70: 7970 6926 6c6f 676f 436f 6c6f 723d 7768  ypi&logoColor=wh
+00001d80: 6974 6526 6c61 6265 6c3d 5079 5049 295d  ite&label=PyPI)]
+00001d90: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00001da0: 672f 7072 6f6a 6563 742f 7273 7374 742f  g/project/rsstt/
+00001db0: 290a 5b21 5b54 6573 7450 7950 495d 2868  ).[![TestPyPI](h
+00001dc0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00001dd0: 6473 2e69 6f2f 6261 6467 652f 6479 6e61  ds.io/badge/dyna
+00001de0: 6d69 632f 6a73 6f6e 3f75 726c 3d68 7474  mic/json?url=htt
+00001df0: 7073 2533 4125 3246 2532 4674 6573 742e  ps%3A%2F%2Ftest.
+00001e00: 7079 7069 2e6f 7267 2532 4670 7970 6925  pypi.org%2Fpypi%
+00001e10: 3246 7273 7374 7425 3246 6a73 6f6e 2671  2Frsstt%2Fjson&q
+00001e20: 7565 7279 3d25 3234 2e69 6e66 6f2e 7665  uery=%24.info.ve
+00001e30: 7273 696f 6e26 7072 6566 6978 3d76 266c  rsion&prefix=v&l
+00001e40: 6f67 6f3d 7079 7069 266c 6f67 6f43 6f6c  ogo=pypi&logoCol
+00001e50: 6f72 3d77 6869 7465 266c 6162 656c 3d54  or=white&label=T
+00001e60: 6573 7450 7950 4929 5d28 6874 7470 733a  estPyPI)](https:
+00001e70: 2f2f 7465 7374 2e70 7970 692e 6f72 672f  //test.pypi.org/
+00001e80: 7072 6f6a 6563 742f 7273 7374 742f 290a  project/rsstt/).
+00001e90: 5b21 5b50 7950 4920 2d20 5079 7468 6f6e  [![PyPI - Python
+00001ea0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+00001eb0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001ec0: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+00001ed0: 2f72 7373 7474 3f6c 6f67 6f3d 7079 7468  /rsstt?logo=pyth
+00001ee0: 6f6e 266c 6162 656c 3d26 6c61 6265 6c43  on&label=&labelC
+00001ef0: 6f6c 6f72 3d77 6869 7465 295d 2868 7474  olor=white)](htt
+00001f00: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+00001f10: 6f72 6729 5c0a 5b21 5b50 7950 4920 7075  org)\.[![PyPI pu
+00001f20: 626c 6973 6820 7374 6174 7573 5d28 6874  blish status](ht
+00001f30: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00001f40: 732e 696f 2f67 6974 6875 622f 6163 7469  s.io/github/acti
+00001f50: 6f6e 732f 776f 726b 666c 6f77 2f73 7461  ons/workflow/sta
+00001f60: 7475 732f 526f 6e67 726f 6e67 6767 392f  tus/Rongronggg9/
+00001f70: 5253 532d 746f 2d54 656c 6567 7261 6d2d  RSS-to-Telegram-
+00001f80: 426f 742f 7075 626c 6973 682d 746f 2d70  Bot/publish-to-p
+00001f90: 7970 692e 796d 6c3f 6c61 6265 6c3d 7075  ypi.yml?label=pu
+00001fa0: 626c 6973 6826 6c6f 676f 3d70 7970 6926  blish&logo=pypi&
+00001fb0: 6c6f 676f 436f 6c6f 723d 7768 6974 6529  logoColor=white)
+00001fc0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001fd0: 2e63 6f6d 2f52 6f6e 6772 6f6e 6767 6739  .com/Rongronggg9
+00001fe0: 2f52 5353 2d74 6f2d 5465 6c65 6772 616d  /RSS-to-Telegram
+00001ff0: 2d42 6f74 2f61 6374 696f 6e73 2f77 6f72  -Bot/actions/wor
+00002000: 6b66 6c6f 7773 2f70 7562 6c69 7368 2d74  kflows/publish-t
+00002010: 6f2d 7079 7069 2e79 6d6c 290a 5b21 5b54  o-pypi.yml).[![T
+00002020: 6573 7450 7950 4920 7075 626c 6973 6820  estPyPI publish 
+00002030: 7374 6174 7573 5d28 6874 7470 733a 2f2f  status](https://
+00002040: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
+00002050: 6974 6875 622f 6163 7469 6f6e 732f 776f  ithub/actions/wo
+00002060: 726b 666c 6f77 2f73 7461 7475 732f 526f  rkflow/status/Ro
+00002070: 6e67 726f 6e67 6767 392f 5253 532d 746f  ngronggg9/RSS-to
+00002080: 2d54 656c 6567 7261 6d2d 426f 742f 7075  -Telegram-Bot/pu
+00002090: 626c 6973 682d 746f 2d74 6573 742d 7079  blish-to-test-py
+000020a0: 7069 2e79 6d6c 3f6c 6162 656c 3d70 7562  pi.yml?label=pub
+000020b0: 6c69 7368 2532 3028 5465 7374 5079 5049  lish%20(TestPyPI
+000020c0: 2926 6c6f 676f 3d70 7970 6926 6c6f 676f  )&logo=pypi&logo
+000020d0: 436f 6c6f 723d 7768 6974 6529 5d28 6874  Color=white)](ht
+000020e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000020f0: 2f52 6f6e 6772 6f6e 6767 6739 2f52 5353  /Rongronggg9/RSS
+00002100: 2d74 6f2d 5465 6c65 6772 616d 2d42 6f74  -to-Telegram-Bot
+00002110: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00002120: 7773 2f70 7562 6c69 7368 2d74 6f2d 7465  ws/publish-to-te
+00002130: 7374 2d70 7970 692e 796d 6c29 0a5b 215b  st-pypi.yml).[![
+00002140: 5079 5049 202d 2044 6f77 6e6c 6f61 6473  PyPI - Downloads
+00002150: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00002160: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
+00002170: 2f72 7373 7474 3f6c 6f67 6f3d 7079 7069  /rsstt?logo=pypi
+00002180: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
+00002190: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+000021a0: 6f72 672f 7072 6f6a 6563 742f 7273 7374  org/project/rsst
+000021b0: 742f 290a 0a49 7420 6973 2071 7569 7465  t/)..It is quite
+000021c0: 2065 6173 7920 746f 2064 6570 6c6f 7920   easy to deploy 
+000021d0: 796f 7572 2052 5353 7454 2069 6e73 7461  your RSStT insta
+000021e0: 6e63 652e 2054 6865 206d 6f73 7420 7265  nce. The most re
+000021f0: 636f 6d6d 656e 6465 6420 7761 7920 746f  commended way to
+00002200: 2064 6570 6c6f 7920 5253 5374 5420 6973   deploy RSStT is
+00002210: 2044 6f63 6b65 7220 436f 6d70 6f73 653a   Docker Compose:
+00002220: 2069 7420 6973 2073 7569 7461 626c 6520   it is suitable 
+00002230: 666f 7220 7669 7274 7561 6c6c 7920 616c  for virtually al
+00002240: 6c20 5650 532e 205b 5261 696c 7761 792e  l VPS. [Railway.
+00002250: 6170 705d 2868 7474 7073 3a2f 2f72 6169  app](https://rai
+00002260: 6c77 6179 2e61 7070 2920 2861 2050 6161  lway.app) (a Paa
+00002270: 5320 706c 6174 666f 726d 2920 6973 2061  S platform) is a
+00002280: 6c73 6f20 6f66 6669 6369 616c 6c79 2073  lso officially s
+00002290: 7570 706f 7274 6564 2e20 596f 7520 6d61  upported. You ma
+000022a0: 7920 616c 736f 2069 6e73 7461 6c6c 2052  y also install R
+000022b0: 5353 7454 2066 726f 6d20 5b50 7950 495d  SStT from [PyPI]
+000022c0: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+000022d0: 672f 7072 6f6a 6563 742f 7273 7374 742f  g/project/rsstt/
+000022e0: 2920 2874 7261 636b 696e 6720 606d 6173  ) (tracking `mas
+000022f0: 7465 7260 2062 7261 6e63 6829 206f 7220  ter` branch) or 
+00002300: 5b54 6573 7450 7950 495d 2868 7474 7073  [TestPyPI](https
+00002310: 3a2f 2f74 6573 742e 7079 7069 2e6f 7267  ://test.pypi.org
+00002320: 2f70 726f 6a65 6374 2f72 7373 7474 2f29  /project/rsstt/)
+00002330: 2028 7472 6163 6b69 6e67 2060 6465 7660   (tracking `dev`
+00002340: 2062 7261 6e63 682c 2077 6869 6368 2069   branch, which i
+00002350: 7320 616c 7761 7973 2075 702d 746f 2d64  s always up-to-d
+00002360: 6174 6529 2075 7369 6e67 2070 6970 2e20  ate) using pip. 
+00002370: 466f 7220 6465 7665 6c6f 7065 7273 206f  For developers o
+00002380: 7220 6578 7065 7269 656e 6365 6420 7573  r experienced us
+00002390: 6572 732c 2064 6972 7479 2072 756e 2066  ers, dirty run f
+000023a0: 726f 6d20 736f 7572 6365 2069 7320 616c  rom source is al
+000023b0: 736f 2061 6e20 6f70 7469 6f6e 2e0a 0a3c  so an option...<
+000023c0: 6120 6872 6566 3d22 646f 6373 2f64 6570  a href="docs/dep
+000023d0: 6c6f 796d 656e 742d 6775 6964 652e 6d64  loyment-guide.md
+000023e0: 236f 7074 696f 6e2d 322d 7261 696c 7761  #option-2-railwa
+000023f0: 7961 7070 223e 3c69 6d67 2073 7263 3d22  yapp"><img src="
+00002400: 6874 7470 733a 2f2f 7261 696c 7761 792e  https://railway.
+00002410: 6170 702f 6275 7474 6f6e 2e73 7667 2220  app/button.svg" 
+00002420: 6865 6967 6874 3d22 3330 2220 616c 743d  height="30" alt=
+00002430: 2244 6570 6c6f 7920 6f6e 2052 6169 6c77  "Deploy on Railw
+00002440: 6179 223e 3c2f 613e 0a0a 466f 7220 6d6f  ay"></a>..For mo
+00002450: 7265 2064 6574 6169 6c73 2c20 7265 6665  re details, refe
+00002460: 7220 746f 2074 6865 205b 6465 706c 6f79  r to the [deploy
+00002470: 6d65 6e74 2067 7569 6465 5d28 646f 6373  ment guide](docs
+00002480: 2f64 6570 6c6f 796d 656e 742d 6775 6964  /deployment-guid
+00002490: 652e 6d64 292e 0a0a 2323 2054 7261 6e73  e.md)...## Trans
+000024a0: 6c61 7469 6f6e 0a0a 5265 6164 2074 6865  lation..Read the
+000024b0: 2074 7261 6e73 6c61 7469 6f6e 2067 7569   translation gui
+000024c0: 6465 205b 6865 7265 5d28 646f 6373 2f74  de [here](docs/t
+000024d0: 7261 6e73 6c61 7469 6f6e 2d67 7569 6465  ranslation-guide
+000024e0: 2e6d 6429 2e0a 0a59 6f75 2063 616e 2068  .md)...You can h
+000024f0: 656c 7020 746f 2074 7261 6e73 6c61 7465  elp to translate
+00002500: 2074 6865 2062 6f74 2075 7369 6e67 205b   the bot using [
+00002510: 486f 7374 6564 2057 6562 6c61 7465 5d28  Hosted Weblate](
+00002520: 6874 7470 733a 2f2f 686f 7374 6564 2e77  https://hosted.w
+00002530: 6562 6c61 7465 2e6f 7267 2f70 726f 6a65  eblate.org/proje
+00002540: 6374 732f 7273 732d 746f 2d74 656c 6567  cts/rss-to-teleg
+00002550: 7261 6d2d 626f 742f 292e 2053 7065 6369  ram-bot/). Speci
+00002560: 616c 2074 6861 6e6b 7320 746f 2074 6865  al thanks to the
+00002570: 6972 2066 7265 6520 686f 7374 696e 6720  ir free hosting 
+00002580: 7365 7276 6963 6520 666f 7220 6c69 6272  service for libr
+00002590: 6520 7072 6f6a 6563 7473 210a 0a3c 6120  e projects!..<a 
+000025a0: 6872 6566 3d22 6874 7470 733a 2f2f 686f  href="https://ho
+000025b0: 7374 6564 2e77 6562 6c61 7465 2e6f 7267  sted.weblate.org
+000025c0: 2f65 6e67 6167 652f 7273 732d 746f 2d74  /engage/rss-to-t
+000025d0: 656c 6567 7261 6d2d 626f 742f 223e 3c69  elegram-bot/"><i
+000025e0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000025f0: 686f 7374 6564 2e77 6562 6c61 7465 2e6f  hosted.weblate.o
+00002600: 7267 2f77 6964 6765 7473 2f72 7373 2d74  rg/widgets/rss-t
+00002610: 6f2d 7465 6c65 6772 616d 2d62 6f74 2f2d  o-telegram-bot/-
+00002620: 2f67 6c6f 7373 6172 792f 6d75 6c74 692d  /glossary/multi-
+00002630: 6175 746f 2e73 7667 2220 7769 6474 6820  auto.svg" width 
+00002640: 3d20 2235 3030 2220 616c 743d 2222 202f  = "500" alt="" /
+00002650: 3e3c 2f61 3e0a 0a23 2320 5573 696e 6720  ></a>..## Using 
+00002660: 7468 6520 7075 626c 6963 2062 6f74 0a0a  the public bot..
+00002670: 5468 6520 5b70 7562 6c69 6320 626f 745d  The [public bot]
+00002680: 2868 7474 7073 3a2f 2f74 2e6d 652f 5253  (https://t.me/RS
+00002690: 5374 545f 426f 7429 2063 6f6d 6573 2077  StT_Bot) comes w
+000026a0: 6974 6820 6162 736f 6c75 7465 6c79 206e  ith absolutely n
+000026b0: 6f20 7761 7272 616e 7479 2e20 4920 7769  o warranty. I wi
+000026c0: 6c6c 2074 7279 206d 7920 6265 7374 2074  ll try my best t
+000026d0: 6f20 6d61 696e 7461 696e 2069 742c 2062  o maintain it, b
+000026e0: 7574 2049 2063 616e 6e6f 7420 6775 6172  ut I cannot guar
+000026f0: 616e 7465 6520 7468 6174 2069 7420 7769  antee that it wi
+00002700: 6c6c 2061 6c77 6179 7320 776f 726b 2070  ll always work p
+00002710: 6572 6665 6374 6c79 2e20 4d65 616e 7768  erfectly. Meanwh
+00002720: 696c 652c 2079 6f75 2073 686f 756c 6420  ile, you should 
+00002730: 2266 6169 7220 7573 6522 2074 6865 2062  "fair use" the b
+00002740: 6f74 2c20 6176 6f69 6420 7375 6273 6372  ot, avoid subscr
+00002750: 6962 696e 6720 746f 2074 6f6f 206d 616e  ibing to too man
+00002760: 7920 5253 5320 6665 6564 732e 2020 0a49  y RSS feeds.  .I
+00002770: 6620 796f 7520 7573 6520 7468 6520 5b70  f you use the [p
+00002780: 7562 6c69 6320 626f 745d 2868 7474 7073  ublic bot](https
+00002790: 3a2f 2f74 2e6d 652f 5253 5374 545f 426f  ://t.me/RSStT_Bo
+000027a0: 7429 2069 6e20 796f 7572 2043 6861 6e6e  t) in your Chann
+000027b0: 656c 2c20 636f 6e73 6964 6572 206d 656e  el, consider men
+000027c0: 7469 6f6e 696e 6720 7468 6520 626f 7420  tioning the bot 
+000027d0: 286f 7220 7468 6973 2070 726f 6a65 6374  (or this project
+000027e0: 2920 696e 2079 6f75 7220 6368 616e 6e65  ) in your channe
+000027f0: 6c20 6465 7363 7269 7074 696f 6e20 286f  l description (o
+00002800: 7220 7069 6e6e 6564 206d 6573 7361 6765  r pinned message
+00002810: 2920 746f 206c 6574 206d 6f72 6520 7065  ) to let more pe
+00002820: 6f70 6c65 206b 6e6f 7720 6162 6f75 7420  ople know about 
+00002830: 6974 2e20 5468 6174 2773 206e 6f74 2061  it. That's not a
+00002840: 2063 6f6d 7075 6c73 696f 6e2e 0a0a 2323   compulsion...##
+00002850: 204b 6e6f 776e 2063 6861 6e6e 656c 7320   Known channels 
+00002860: 7573 696e 6720 5253 5374 540a 0a57 616e  using RSStT..Wan
+00002870: 7420 746f 2070 7265 7669 6577 2077 6861  t to preview wha
+00002880: 7420 7468 6520 6d65 7373 6167 6573 2073  t the messages s
+00002890: 656e 7420 6279 2052 5353 7454 206c 6f6f  ent by RSStT loo
+000028a0: 6b20 6c69 6b65 3f20 4865 7265 2069 7320  k like? Here is 
+000028b0: 6120 5b6c 6973 7420 6f66 2063 6861 6e6e  a [list of chann
+000028c0: 656c 7320 7573 696e 6720 5253 5374 545d  els using RSStT]
+000028d0: 2864 6f63 732f 6368 616e 6e65 6c73 2d75  (docs/channels-u
+000028e0: 7369 6e67 2d72 7373 7474 2e6d 6429 2e0a  sing-rsstt.md)..
+000028f0: 0a23 2320 4c69 6365 6e73 650a 0a54 6869  .## License..Thi
+00002900: 7320 7072 6f6a 6563 7420 6973 206c 6963  s project is lic
+00002910: 656e 7365 6420 756e 6465 7220 5b41 4750  ensed under [AGP
+00002920: 4c76 335d 284c 4943 454e 5345 292e 2043  Lv3](LICENSE). C
+00002930: 6c6f 7365 642d 736f 7572 6365 2064 6973  losed-source dis
+00002940: 7472 6962 7574 696f 6e20 6f72 2062 6f74  tribution or bot
+00002950: 2d68 6f73 7469 6e67 2061 7265 2073 7472  -hosting are str
+00002960: 6963 746c 7920 7072 6f68 6962 6974 6564  ictly prohibited
+00002970: 2e20 4966 2079 6f75 206d 6f64 6966 7920  . If you modify 
+00002980: 7468 6520 636f 6465 2061 6e64 2064 6973  the code and dis
+00002990: 7472 6962 7574 6520 6f72 2068 6f73 7420  tribute or host 
+000029a0: 6974 2c20 6d61 6b65 2073 7572 6520 616e  it, make sure an
+000029b0: 7920 7573 6572 7320 7768 6f20 6361 6e20  y users who can 
+000029c0: 7573 6520 796f 7572 2062 6f74 2063 616e  use your bot can
+000029d0: 2067 6574 2074 6865 2073 6f75 7263 6520   get the source 
+000029e0: 636f 6465 2028 6279 2065 6469 7469 6e67  code (by editing
+000029f0: 2074 6865 2072 6570 6f20 5552 4c20 696e   the repo URL in
+00002a00: 205b 6073 7263 2f69 3138 6e2f 5f5f 696e   [`src/i18n/__in
+00002a10: 6974 5f5f 2e70 7960 5d28 7372 632f 6931  it__.py`](src/i1
+00002a20: 386e 2f5f 5f69 6e69 745f 5f2e 7079 2929  8n/__init__.py))
+00002a30: 2e0a 0a54 6865 2072 6570 6f73 6974 6f72  ...The repositor
+00002a40: 7920 7761 7320 666f 726d 6572 6c79 2061  y was formerly a
+00002a50: 2066 6f72 6b20 6f66 205b 426f 4b4b 6552   fork of [BoKKeR
+00002a60: 2f52 5353 2d74 6f2d 5465 6c65 6772 616d  /RSS-to-Telegram
+00002a70: 2d42 6f74 5d28 6874 7470 733a 2f2f 6769  -Bot](https://gi
+00002a80: 7468 7562 2e63 6f6d 2f42 6f4b 4b65 522f  thub.com/BoKKeR/
+00002a90: 5253 532d 746f 2d54 656c 6567 7261 6d2d  RSS-to-Telegram-
+00002aa0: 426f 7429 2e20 5468 6579 2068 6176 6520  Bot). They have 
+00002ab0: 6265 656e 2065 6e74 6972 656c 7920 6469  been entirely di
+00002ac0: 6666 6572 656e 7420 7072 6f6a 6563 7473  fferent projects
+00002ad0: 2073 696e 6365 2074 6865 2065 6172 6c79   since the early
+00002ae0: 2064 6179 7320 6f66 2074 6869 7320 7072   days of this pr
+00002af0: 6f6a 6563 742e 0a                        oject..
```

### Comparing `rsstt-2.6.0/rsstt.egg-info/SOURCES.txt` & `rsstt-2.7.0/rsstt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,26 +33,24 @@
 src/command/inner/customization.py
 src/command/inner/sub.py
 src/command/inner/utils.py
 src/db/__init__.py
 src/db/config.py
 src/db/effective_utils.py
 src/db/models.py
-src/db/migrations_pgsql/__init__.py
-src/db/migrations_pgsql/models/0_20211117110249_init.sql
-src/db/migrations_pgsql/models/1_20211130051128_update.sql
-src/db/migrations_pgsql/models/2_20220306045951_update.sql
-src/db/migrations_pgsql/models/3_20220415030554_update.sql
-src/db/migrations_pgsql/models/__init__.py
-src/db/migrations_sqlite/__init__.py
-src/db/migrations_sqlite/models/0_20211117110249_init.sql
-src/db/migrations_sqlite/models/1_20211130051128_update.sql
-src/db/migrations_sqlite/models/2_20220306045951_update.sql
-src/db/migrations_sqlite/models/3_20220415025716_update.sql
-src/db/migrations_sqlite/models/__init__.py
+src/db/migrations_pgsql/models/0_20211117110249_init.py
+src/db/migrations_pgsql/models/1_20211130051128_update.py
+src/db/migrations_pgsql/models/2_20220306045951_update.py
+src/db/migrations_pgsql/models/3_20220415030554_update.py
+src/db/migrations_pgsql/models/4_20240425020849_display_entry_tags.py
+src/db/migrations_sqlite/models/0_20211117110249_init.py
+src/db/migrations_sqlite/models/1_20211130051128_update.py
+src/db/migrations_sqlite/models/2_20220306045951_update.py
+src/db/migrations_sqlite/models/3_20220415025716_update.py
+src/db/migrations_sqlite/models/4_20240425020849_display_entry_tags.py
 src/i18n/__init__.py
 src/i18n/ar.json
 src/i18n/ca.json
 src/i18n/cs.json
 src/i18n/de.json
 src/i18n/el.json
 src/i18n/en.json
```

### Comparing `rsstt-2.6.0/rsstt.egg-info/requires.txt` & `rsstt-2.7.0/rsstt.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 cryptg==0.4.0
-telethon==1.34.0
+telethon==1.35.0
 aiographfix==0.2.2
 feedparser==6.0.11
-listparser[lxml]==0.19
-pillow==10.2.0
+listparser[lxml]==0.20
+pillow==10.3.0
 beautifulsoup4==4.12.3
-lxml==4.9.3
-rapidfuzz==3.7.0
-emoji==2.11.0
+lxml==5.2.1
+rapidfuzz==3.9.0
+emoji==2.11.1
 minify-html==0.15.0
 minify-html-onepass==0.15.0
-matplotlib==3.8.3
+matplotlib==3.8.4
 asyncpg==0.29.0
-tortoise-orm[accel]==0.20.0
-aerich==0.6.3
-aiohttp[speedups]==3.9.3
+tortoise-orm[accel]==0.20.1
+aerich==0.7.2
+aiohttp[speedups]==3.9.5
 aiohttp-socks==0.8.4
 aiohttp-retry==2.8.3
 python-socks[asyncio]==2.4.4
 dnspython[idna]==2.6.1
 colorlog==6.8.2
 APScheduler==3.10.4
 python-dotenv==1.0.1
 multidict==6.0.5
-asyncstdlib==3.12.2
+asyncstdlib==3.12.3
 cachetools==5.3.3
 CJKwrap==2.2
-typing-extensions==4.10.0
+typing-extensions==4.11.0
 
 [:platform_machine == "x86_64" or platform_machine == "AMD64" or platform_machine == "aarch64"]
 isal==1.6.1
 
 [:sys_platform != "win32" and sys_platform != "cygwin" and sys_platform != "cli"]
 uvloop==0.19.0
```

### Comparing `rsstt-2.6.0/setup.cfg` & `rsstt-2.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 	Operating System :: POSIX :: Linux
 	Operating System :: Microsoft :: Windows
 	Operating System :: MacOS
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Communications :: Chat
 	Topic :: Internet
 	Topic :: Multimedia
 
 [requirements-files]
 install_requires = requirements.txt
```

### Comparing `rsstt-2.6.0/setup.py` & `rsstt-2.7.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,21 @@
 
 PROJ_ROOT = Path(__file__).parent
 
 version = re.search(r"""__version__ *= *['"]([^'"]+)['"]""", (PROJ_ROOT / "src/version.py").read_text())[1]
 
 replacePackagePath = partial(re.compile(r'^src').sub, 'rsstt')
 
-source_packages = find_packages(include=['src', 'src.*'])
-proj_packages = [replacePackagePath(name) for name in source_packages]
+# DB migrations are not Python packages, but they should also be included in the package
+source_packages = find_packages(PROJ_ROOT, include=['src', 'src.*'])
+db_migrations_dirs = [
+    str(path.relative_to(PROJ_ROOT)).replace('/', '.')
+    for path in (PROJ_ROOT / 'src' / 'db').glob('migrations_*/**')
+    if path.is_dir()
+]
+proj_packages = [replacePackagePath(name) for name in source_packages + db_migrations_dirs]
 
 setup(
     version=version,
     packages=proj_packages,
     package_dir={'rsstt': 'src'},
 )
```

### Comparing `rsstt-2.6.0/src/__init__.py` & `rsstt-2.7.0/src/__init__.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/aio_helper.py` & `rsstt-2.7.0/src/aio_helper.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/command/administration.py` & `rsstt-2.7.0/src/command/administration.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/command/customization.py` & `rsstt-2.7.0/src/command/customization.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     send_mode: -1=force link, 0=auto, 1=force Telegraph, 2=force message
     length_limit: Telegraph length limit, valid when send_mode==0. If exceeded, send via Telegraph; If is 0,
         send via Telegraph when a post cannot be sent in a single message
     link_preview: 0=auto, 1=force enable
     display_author: -1=disable, 0=auto, 1=force display
     display_via: -2=completely disable, -1=disable but display link, 0=auto, 1=force display
     display_title: -1=disable, 0=auto, 1=force display
+    display_entry_tags: -1=disable, 1=force display
     style: 0=RSStT, 1=flowerss
     """
     chat_id = chat_id or event.chat_id
     callback_tail = get_callback_tail(event, chat_id)
     sub_id, action, param, page = parse_customization_callback_data(event.data)
 
     if sub_id is None and not set_user_default:
@@ -158,15 +159,15 @@
         return
 
     update_interval_flag = False
     if sub.interval is not None:
         sub.interval = None
         update_interval_flag = True
     sub.length_limit = sub.notify = sub.send_mode = sub.link_preview = sub.display_author = sub.display_media = \
-        sub.display_title = sub.display_via = sub.style = -100
+        sub.display_title = sub.display_entry_tags = sub.display_via = sub.style = -100
     await sub.save()
     if update_interval_flag:
         await inner.utils.update_interval(sub)
     info = await inner.customization.get_sub_info(sub, lang, additional_guide=True)
     buttons = await inner.customization.get_customization_buttons(sub, lang=lang, page=page, tail=callback_tail)
     await event.edit(info, buttons=buttons, parse_mode='html', link_preview=False)
 
@@ -202,17 +203,17 @@
     tasks = []
     for sub in subs:
         if sub.interval is not None:
             sub.interval = None
             tasks.append(inner.utils.update_interval(sub))
         sub.interval = None
         sub.length_limit = sub.notify = sub.send_mode = sub.link_preview = sub.display_author = sub.display_media = \
-            sub.display_title = sub.display_via = sub.style = -100
+            sub.display_title = sub.display_entry_tags = sub.display_via = sub.style = -100
     await db.Sub.bulk_update(subs, ('interval', 'length_limit', 'notify', 'send_mode', 'link_preview', 'display_author',
-                                    'display_media', 'display_title', 'display_via', 'style'))
+                                    'display_media', 'display_title', 'display_entry_tags', 'display_via', 'style'))
     for task in tasks:
         env.loop.create_task(task)
     await event.edit(i18n[lang]['reset_all_successful'])
 
 
 @command_gatekeeper(only_manager=False)
 async def cmd_activate_or_deactivate_subs(event: Union[events.NewMessage.Event, Message],
@@ -395,23 +396,23 @@
     hashtags = inner.utils.parse_hashtags(hashtags) if hashtags else None
     if not sub:
         await event.respond(i18n[lang]['permission_denied_no_direct_use'] % '/set')
         return
     if not hashtags and not sub.tags:
         await event.respond(i18n[lang]['cmd_set_hashtags_usage_prompt_html'], parse_mode='html')
         return
-    hashtags_str = ' '.join(hashtags) if hashtags else None
-    if hashtags_str and len(hashtags_str) > 255:
+    try:
+        await inner.customization.set_sub_hashtags(sub, hashtags)
+    except inner.customization.TooManyHashtagsError:
         await event.respond(i18n[lang]['set_hashtags_failure_too_many'])
         return
-    await inner.customization.set_sub_hashtags(sub, hashtags_str)
     await event.respond(
         (
                 ((i18n[lang]['set_hashtags_success_html'] + '\n'
-                  + f'<b>{inner.utils.construct_hashtags(hashtags)}</b>')
-                 if hashtags
+                  + f'<b>{inner.utils.construct_hashtags(sub.tags)}</b>')
+                 if sub.tags
                  else i18n[lang]['set_hashtags_success_cleared'])
                 + '\n\n' +
                 await inner.customization.get_sub_info(sub, lang=lang)
         ),
         buttons=(Button.inline(i18n[lang]['other_settings_button'], data=f'set={sub.id}' + callback_tail),),
         parse_mode='html', link_preview=False)
```

### Comparing `rsstt-2.6.0/src/command/inner/customization.py` & `rsstt-2.7.0/src/command/inner/customization.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,35 @@
 from telethon import Button
 from telethon.tl.types import KeyboardButtonCallback
 
 from ... import db, env
 from ...i18n import i18n
 from .utils import arrange_grid, update_interval, activate_or_deactivate_sub, formatting_time, logger, \
     construct_hashtags
+from ...parsing.utils import escape_hashtags
 
 SUB_OPTIONS_EXHAUSTIVE_VALUES = {
     "notify": (1, 0),
     "send_mode": (0, 1, 2, -1),
     "link_preview": (0, 1, -1),
     "display_media": (0, 1, -1),
     "display_author": (0, 1, -1),
     "display_via": (0, 1, -3, -1, -4, -2),
     "display_title": (0, 1, -1),
+    "display_entry_tags": (1, -1),
     "style": (0, 1)
 }
 
 FALLBACK_TO_USER_DEFAULT_EMOJI = "↩️"
 
 
+class TooManyHashtagsError(ValueError):
+    pass
+
+
 async def get_sub_info(sub: db.Sub,
                        lang: Optional[str] = None,
                        additional_guide: bool = False) -> str:
     if not isinstance(sub.feed, db.Feed):
         await sub.fetch_related('feed')
     return (
             f"<b>{i18n[lang]['subscription_info']}</b>\n\n"
@@ -50,40 +56,42 @@
                                     lang: Optional[str] = None,
                                     page: Optional[int] = None,
                                     tail: str = '') -> tuple[tuple[KeyboardButtonCallback, ...], ...]:
     page = page or 1
     is_user = isinstance(sub_or_user, db.User)
     if is_user:
         interval_d = length_limit_d = notify_d = send_mode_d = link_preview_d = display_media_d = display_author_d = \
-            display_via_d = display_title_d = style_d = False
+            display_via_d = display_title_d = display_entry_tags_d = style_d = False
         all_default = None
     else:
         if not isinstance(sub_or_user.user, db.User):
             await sub_or_user.fetch_related('user')
         interval_d = sub_or_user.interval is None
         length_limit_d = sub_or_user.length_limit == -100
         notify_d = sub_or_user.notify == -100
         send_mode_d = sub_or_user.send_mode == -100
         link_preview_d = sub_or_user.link_preview == -100
         display_media_d = sub_or_user.display_media == -100
         display_author_d = sub_or_user.display_author == -100
         display_via_d = sub_or_user.display_via == -100
         display_title_d = sub_or_user.display_title == -100
+        display_entry_tags_d = sub_or_user.display_entry_tags == -100
         style_d = sub_or_user.style == -100
         all_default = all((interval_d, length_limit_d, notify_d, send_mode_d, link_preview_d, display_media_d,
-                           display_author_d, display_via_d, display_title_d, style_d))
+                           display_author_d, display_via_d, display_title_d, display_entry_tags_d, style_d))
     interval = sub_or_user.user.interval if interval_d else sub_or_user.interval
     length_limit = sub_or_user.user.length_limit if length_limit_d else sub_or_user.length_limit
     notify = sub_or_user.user.notify if notify_d else sub_or_user.notify
     send_mode = sub_or_user.user.send_mode if send_mode_d else sub_or_user.send_mode
     link_preview = sub_or_user.user.link_preview if link_preview_d else sub_or_user.link_preview
     display_media = sub_or_user.user.display_media if display_media_d else sub_or_user.display_media
     display_author = sub_or_user.user.display_author if display_author_d else sub_or_user.display_author
     display_via = sub_or_user.user.display_via if display_via_d else sub_or_user.display_via
     display_title = sub_or_user.user.display_title if display_title_d else sub_or_user.display_title
+    display_entry_tags = sub_or_user.user.display_entry_tags if display_entry_tags_d else sub_or_user.display_entry_tags
     style = sub_or_user.user.style if style_d else sub_or_user.style
     buttons = (
         (
             Button.inline(
                 FALLBACK_TO_USER_DEFAULT_EMOJI + i18n[lang]['reset_all_button'],
                 data=f'reset_all_confirm{tail}',
             )
@@ -178,14 +186,26 @@
                     if is_user
                     else f'set={sub_or_user.id},display_title|{page}{tail}'
                 ),
             ),
         ),
         (
             Button.inline(
+                f"{i18n[lang]['display_entry_tags']}: "
+                + (FALLBACK_TO_USER_DEFAULT_EMOJI if display_entry_tags_d else '')
+                + i18n[lang][f'display_entry_tags_{display_entry_tags}'],
+                data=(
+                    f'set_default=display_entry_tags{tail}'
+                    if is_user
+                    else f'set={sub_or_user.id},display_entry_tags|{page}{tail}'
+                ),
+            ),
+        ),
+        (
+            Button.inline(
                 f"{i18n[lang]['display_via']}: "
                 + (FALLBACK_TO_USER_DEFAULT_EMOJI if display_via_d else '')
                 + i18n[lang][f'display_via_{display_via}'],
                 data=(
                     f'set_default=display_via{tail}'
                     if is_user
                     else f'set={sub_or_user.id},display_via|{page}{tail}'
@@ -456,19 +476,18 @@
     for sub in subs:
         sub.title = None
     return await db.Sub.bulk_update(subs, ['title'])
 
 
 async def set_sub_hashtags(sub: db.Sub, hashtags: Union[Iterable[str], str, None]) -> db.Sub:
     if hashtags is None or isinstance(hashtags, str):
-        hashtags_str = hashtags
+        new_hashtags = hashtags
     else:
-        filtered_hashtags = []
-        for hashtag in hashtags:
-            hashtag = hashtag.strip(' \n\r\t#')
-            if hashtag:
-                filtered_hashtags.append(hashtag)
-        hashtags_str = ' '.join(filtered_hashtags) if filtered_hashtags else None
-    if sub.tags == hashtags_str:
-        return sub
-    sub.tags = hashtags_str
-    await sub.save()
+        new_hashtags = ' '.join(escape_hashtags(hashtags))
+    if new_hashtags and len(new_hashtags) > 255:
+        raise TooManyHashtagsError('Hashtags too long')
+    elif not new_hashtags:
+        new_hashtags = None
+    if sub.tags != new_hashtags:
+        sub.tags = new_hashtags
+        await sub.save()
+    return sub
```

### Comparing `rsstt-2.6.0/src/command/inner/sub.py` & `rsstt-2.7.0/src/command/inner/sub.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from urllib.parse import urljoin
 from cachetools import TTLCache
 from os import path
 
 from ... import db, web, env
 from ...aio_helper import run_async
 from ...i18n import i18n
-from .utils import update_interval, list_sub, get_http_last_modified, filter_urls, logger, escape_html, \
+from .utils import update_interval, list_sub, filter_urls, logger, escape_html, \
     check_sub_limit, calculate_update
 from ...parsing.utils import html_space_stripper
 
 FeedSnifferCache = TTLCache(maxsize=256, ttl=60 * 60 * 24)
 
 with open(path.normpath(path.join(path.dirname(__file__), '../..', 'opml_template.opml')), 'r') as __template:
     OPML_TEMPLATE = __template.read()
@@ -69,45 +69,53 @@
                 return ret
 
             if feed_url_original != feed_url:
                 logger.info(f'Sub {feed_url_original} redirected to {feed_url}')
                 if feed:
                     await migrate_to_new_url(feed, feed_url)
 
+            wr = wf.web_response
+            assert wr is not None
+
             # need to use get_or_create because we've changed feed_url to the redirected one
             title = rss_d.feed.title
             title = html_space_stripper(title) if title else ''
             feed, created_new_feed = await db.Feed.get_or_create(defaults={'title': title}, link=feed_url)
             if created_new_feed or feed.state == 0:
                 feed.state = 1
                 feed.error_count = 0
                 feed.next_check_time = None
-                etag = wf.headers and wf.headers.get('ETag')
+                etag = wr.etag
                 if etag:
                     feed.etag = etag
-                feed.last_modified = get_http_last_modified(wf.headers)
+                feed.last_modified = wr.last_modified
                 feed.entry_hashes = list(calculate_update(old_hashes=None, entries=rss_d.entries)[0])
                 await feed.save()  # now we get the id
                 db.effective_utils.EffectiveTasks.update(feed.id)
 
         sub_title = sub_title if feed.title != sub_title else None
 
         if not _sub:  # create a new sub if needed
-            _sub, created_new_sub = await db.Sub.get_or_create(user_id=user_id, feed=feed,
-                                                               defaults={'title': sub_title if sub_title else None,
-                                                                         'interval': None,
-                                                                         'notify': -100,
-                                                                         'send_mode': -100,
-                                                                         'length_limit': -100,
-                                                                         'link_preview': -100,
-                                                                         'display_author': -100,
-                                                                         'display_via': -100,
-                                                                         'display_title': -100,
-                                                                         'style': -100,
-                                                                         'display_media': -100})
+            _sub, created_new_sub = await db.Sub.get_or_create(
+                user_id=user_id, feed=feed,
+                defaults={
+                    'title': sub_title if sub_title else None,
+                    'interval': None,
+                    'notify': -100,
+                    'send_mode': -100,
+                    'length_limit': -100,
+                    'link_preview': -100,
+                    'display_author': -100,
+                    'display_via': -100,
+                    'display_title': -100,
+                    'display_entry_tags': -100,
+                    'style': -100,
+                    'display_media': -100
+                }
+            )
 
         if not created_new_sub:
             if _sub.title == sub_title and _sub.state == 1:
                 ret['sub'] = None
                 ret['msg'] = 'ERROR: ' + i18n[lang]['already_subscribed']
                 return ret
```

### Comparing `rsstt-2.6.0/src/command/inner/utils.py` & `rsstt-2.7.0/src/command/inner/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from typing import Any, Union, Optional
 from collections.abc import Iterable, Mapping, Sequence
 
 import asyncio
 import re
 from collections import defaultdict
 from itertools import chain, repeat
-from datetime import datetime
-from email.utils import parsedate_to_datetime
 from telethon import Button
 from telethon.tl.types import KeyboardButtonCallback
 
 try:
     from isal.isal_zlib import crc32
 except ImportError:
     from zlib import crc32
@@ -29,15 +27,15 @@
         return re.findall(r'(?<=#)[^\s#]+', text)
     return re.findall(r'\S+', text)
 
 
 def construct_hashtags(tags: Union[Iterable[str], str]) -> str:
     if isinstance(tags, str):
         tags = parse_hashtags(tags)
-    return ' '.join(f'#{tag}' for tag in tags)
+    return '#' + ' #'.join(tags)
 
 
 def calculate_update(old_hashes: Optional[Sequence[str]], entries: Sequence[dict]) \
         -> tuple[Iterable[str], Iterable[dict]]:
     new_hashes_d = {
         hex(crc32(guid.encode('utf-8')))[2:]: entry
         for guid, entry in (
@@ -74,29 +72,14 @@
             (f'{days}d' if days > 0 or long else '')
             + (f'{hours}h' if hours > 0 or long else '')
             + (f'{minutes}min' if minutes > 0 or long else '')
             + (f'{seconds}s' if seconds > 0 or long else '')
     )
 
 
-def get_http_last_modified(headers: Optional[Mapping]) -> datetime:
-    """
-    :param headers: dict of headers
-    :return: last modified time
-    """
-    last_modified = headers.get('Last-Modified') or headers.get('Date') if headers else None
-    try:
-        return parsedate_to_datetime(last_modified) if last_modified else datetime.utcnow()
-    except ValueError:
-        try:
-            return datetime.fromisoformat(last_modified)  # why some websites are so freaky? I can't understand
-        except ValueError:
-            return datetime.utcnow()
-
-
 def arrange_grid(to_arrange: Iterable, columns: int = 8, rows: int = 13) -> tuple[tuple[Any, ...], ...]:
     """
     :param to_arrange: `Iterable` containing objects to arrange
     :param columns: 1-based, telegram limit: 8 (row 1-12), 4 (row 13)
     :param rows: 1-based, telegram limit: 13
     :return: grid (2D tuple) with objects arranged
     """
```

### Comparing `rsstt-2.6.0/src/command/misc.py` & `rsstt-2.7.0/src/command/misc.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/command/monitor.py` & `rsstt-2.7.0/src/command/monitor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,240 +1,322 @@
 from __future__ import annotations
-from typing import Union
-from typing_extensions import Final
-from collections.abc import MutableMapping, Iterable
+from typing import Union, Final, Optional
+from collections.abc import MutableMapping, Iterable, Mapping
 
 import gc
 import asyncio
+import logging
 from datetime import datetime, timedelta, timezone
 from email.utils import format_datetime
 from collections import defaultdict, Counter
+from contextlib import AbstractContextManager
 from itertools import islice
 from traceback import format_exc
 from telethon.errors import BadRequestError
 
 from . import inner
 from .utils import escape_html, unsub_all_and_leave_chat
-from .inner.utils import update_interval, deactivate_feed, calculate_update
 from .. import log, db, env, web, locks
 from ..errors_collection import EntityNotFoundError, UserBlockedErrors
 from ..i18n import i18n
 from ..parsing.post import get_post_from_entry, Post
 from ..parsing.utils import html_space_stripper
 
 logger = log.getLogger('RSStT.monitor')
 
-NOT_UPDATED: Final = 'not_updated'
-CACHED: Final = 'cached'
-EMPTY: Final = 'empty'
-FAILED: Final = 'failed'
-UPDATED: Final = 'updated'
-SKIPPED: Final = 'skipped'
+TIMEOUT: Final[int] = 10 * 60  # 10 minutes
 
 # it may cause memory leak, but they are too small that leaking thousands of that is still not a big deal!
 __user_unsub_all_lock_bucket: dict[int, asyncio.Lock] = defaultdict(asyncio.Lock)
 __user_blocked_counter = Counter()
 
 
-class MonitoringLogs:
-    monitoring_counts = 0
-    not_updated = 0
-    cached = 0
-    empty = 0
-    failed = 0
-    updated = 0
-    skipped = 0
-    timeout = 0
+# TODO: move inside MonitoringStat once the minimum Python requirement is 3.10
+# @staticmethod
+def _gen_property(key: str):
+    def getter(self):
+        return self.counter[key]
+
+    def setter(self, value):
+        self.counter[key] = value
+
+    return property(getter, setter)
+
+
+class MonitoringStat(AbstractContextManager):
+    # TODO: make __monitor directly call this class's method to log and make statistics
+    class Meta:
+        counter: MutableMapping[str, int] = Counter()
+        last_summary_time: float = env.loop.time()
+        task_finished: set[object] = set()
+        task_in_progress: set[object] = set()
+        task_stuck: set[object] = set()
+        summary_period: float = TIMEOUT  # seconds
+
+    not_updated: int = _gen_property('not_updated')
+    cached: int = _gen_property('cached')
+    empty: int = _gen_property('empty')
+    failed: int = _gen_property('failed')
+    updated: int = _gen_property('updated')
+    skipped: int = _gen_property('skipped')
+    timeout: int = _gen_property('timeout')
+    cancelled: int = _gen_property('cancelled')
+    unknown_error: int = _gen_property('unknown_error')
+    timeout_unknown_error: int = _gen_property('timeout_unknown_error')
+
+    @staticmethod
+    def _stat(counter: Mapping) -> str:
+        return ', '.join(filter(None, (
+            f'updated({counter["updated"]})',
+            f'not updated({counter["not_updated"]}, including {counter["cached"]} cached and {counter["empty"]} empty)',
+            f'fetch failed({counter["failed"]})' if counter["failed"] else '',
+            f'skipped({counter["skipped"]})' if counter["skipped"] else '',
+            f'timeout({counter["timeout"]})' if counter["timeout"] else '',
+            f'cancelled({counter["cancelled"]})' if counter["cancelled"] else '',
+            f'unknown error({counter["unknown_error"]})' if counter["unknown_error"] else '',
+            f'timeout w/ unknown error({counter["timeout_unknown_error"]})' if counter["timeout_unknown_error"] else '',
+        )))
+
+    def __init__(self):
+        self.print_summary()
+        self.counter: MutableMapping[str, int] = Counter()
+        self._token = object()
+        self.Meta.task_in_progress.add(self._token)
 
-    @classmethod
-    def log(cls, not_updated: int, cached: int, empty: int, failed: int, updated: int, skipped: int, timeout: int):
-        cls.not_updated += not_updated
-        cls.cached += cached
-        cls.empty += empty
-        cls.failed += failed
-        cls.updated += updated
-        cls.skipped += skipped
-        cls.timeout += timeout
-        logger.debug(f'Finished feeds monitoring task: '
-                     f'updated({updated}), '
-                     f'not updated({not_updated}, including {cached} cached and {empty} empty), '
-                     f'fetch failed({failed}), '
-                     f'skipped({skipped}), '
-                     f'timeout({timeout})')
-        cls.monitoring_counts += 1
-        if cls.monitoring_counts == 10:
-            cls.print_summary()
-            gc.collect()
+    def __exit__(self, *args):
+        meta = self.Meta
+        try:
+            meta.counter += self.counter
+            level = logging.DEBUG
+            if self.timeout or self.cancelled or self.unknown_error or self.timeout_unknown_error:
+                level = logging.WARNING
+            msg = f'Finished a monitoring task: {self._stat(self.counter)}'
+            logger.log(level, msg)
+        finally:
+            meta.task_in_progress.discard(self._token)
+            meta.task_stuck.discard(self._token)
+            meta.task_finished.add(self._token)
+            self.print_summary()
 
     @classmethod
     def print_summary(cls):
+        meta = cls.Meta
+        now = env.loop.time()
+        time_diff = round(now - meta.last_summary_time)
+        if time_diff < meta.summary_period:
+            return
         logger.info(
-            f'Monitoring tasks summary in last 10 minutes: '
-            f'updated({cls.updated}), '
-            f'not updated({cls.not_updated}, including {cls.cached} cached and {cls.empty} empty), '
-            f'fetch failed({cls.failed}), '
-            f'skipped({cls.skipped}), '
-            f'timeout({cls.timeout})'
+            f'{len(meta.task_finished)} monitoring tasks finished in the past {time_diff}s'
+            + (f', while {len(meta.task_in_progress)} are still in progress' if meta.task_in_progress else '') +
+            f'. Subtask summary of finished tasks: {cls._stat(meta.counter)}'
         )
-        cls.not_updated = cls.cached = cls.empty = cls.failed = cls.updated = cls.skipped = cls.timeout = 0
-        cls.monitoring_counts = 0
+        if meta.task_stuck:
+            logger.warning(
+                f'{len(meta.task_stuck)} monitoring tasks are still in progress after >{time_diff}s, '
+                'are they stuck?'
+            )
+        meta.last_summary_time = now
+        meta.task_stuck |= meta.task_in_progress
+        meta.task_in_progress.clear()
+        meta.task_finished.clear()
+        meta.counter.clear()
+        gc.collect()
 
 
 async def run_monitor_task():
     feed_id_to_monitor = db.effective_utils.EffectiveTasks.get_tasks()
     if not feed_id_to_monitor:
         return
 
     feeds = await db.Feed.filter(id__in=feed_id_to_monitor)
 
-    logger.debug('Started feeds monitoring task.')
-    wait_for = 10 * 60
-    timeout_errors = []
-
-    result = await asyncio.gather(*(asyncio.wait_for(__monitor(feed), timeout=wait_for) for feed in feeds),
-                                  return_exceptions=True)
-
-    not_updated = 0
-    cached = 0
-    empty = 0
-    failed = 0
-    updated = 0
-    skipped = 0
-    timeout = 0
-
-    for f, r in zip(feeds, result):
-        if r is NOT_UPDATED:
-            not_updated += 1
-        elif r is CACHED:
-            not_updated += 1
-            cached += 1
-        elif r is EMPTY:
-            not_updated += 1
-            empty += 1
-        elif r is UPDATED:
-            updated += 1
-        elif r is FAILED:
-            failed += 1
-        elif r is SKIPPED:
-            skipped += 1
-        elif isinstance(r, asyncio.TimeoutError):
-            timeout += 1
-            timeout_errors.append((f, r))
-        elif isinstance(r, BaseException):
-            raise r
-        else:
-            raise TypeError(f'Unknown monitor result type: {r}')
-
-    MonitoringLogs.log(not_updated, cached, empty, failed, updated, skipped, timeout)
-    if timeout_errors:
-        logger.error(f'Timeout detected during a feeds monitoring task, '
-                     f'totally {timeout} feed(s) timed out after {wait_for}s:')
-        for feed, error in timeout_errors:
-            logger.error(f'The TimeoutError of the feed ({feed.link}) in the task:', exc_info=error)
+    logger.debug('Started a monitoring task.')
+    wait_for = TIMEOUT
+
+    with MonitoringStat() as stat:
+        task_feed_map = {
+            env.loop.create_task(__monitor(feed, stat)): feed
+            for feed in feeds
+        }
+        done, pending = await asyncio.wait(task_feed_map.keys(), timeout=wait_for)
+
+        for task in pending:
+            task.cancel()
+            try:
+                await task
+            except asyncio.CancelledError as e:
+                stat.timeout += 1
+                feed = task_feed_map[task]
+                logger.error(f'Monitoring subtask timed out after {wait_for}s: {feed.link}', exc_info=e)
+            except Exception as e:
+                stat.timeout_unknown_error += 1
+                feed = task_feed_map[task]
+                logger.error(
+                    f'Monitoring subtask timed out after {wait_for}s and caused an unknown error: {feed.link}',
+                    exc_info=e
+                )
+
+        for task in done:
+            try:
+                await task
+            except asyncio.CancelledError as e:
+                stat.cancelled += 1
+                feed = task_feed_map[task]
+                logger.error(f'Monitoring subtask failed due to CancelledError: {feed.link}', exc_info=e)
+            except Exception as e:
+                stat.unknown_error += 1
+                feed = task_feed_map[task]
+                logger.error(f'Monitoring failed due to an unknown error: {feed.link}', exc_info=e)
+
+
+def _defer_next_check_as_per_server_side_cache(wf: web.WebFeed) -> Optional[datetime]:
+    wr = wf.web_response
+    assert wr is not None
+    expires = wr.expires
+    now = wr.now
+
+    # defer next check as per Cloudflare cache
+    # https://developers.cloudflare.com/cache/concepts/cache-responses/
+    # https://developers.cloudflare.com/cache/how-to/edge-browser-cache-ttl/
+    if expires and wf.headers.get('cf-cache-status') in {'HIT', 'MISS', 'EXPIRED', 'REVALIDATED'} and expires > now:
+        return expires
+
+    # defer next check as per RSSHub TTL (or Cache-Control max-age)
+    # only apply when TTL > 5min,
+    # as it is the default value of RSSHub and disabling cache won't change it in some legacy versions
+    rss_d = wf.rss_d
+    if rss_d.feed.get('generator') == 'RSSHub' and (updated_str := rss_d.feed.get('updated')):
+        ttl_in_minute_str: str = rss_d.feed.get('ttl', '')
+        ttl_in_second = int(ttl_in_minute_str) * 60 if ttl_in_minute_str.isdecimal() else None
+        if ttl_in_second is None:
+            ttl_in_second = wr.max_age
+        if ttl_in_second and ttl_in_second > 300:
+            updated = web.utils.rfc_2822_8601_to_datetime(updated_str)
+            if updated and (next_check_time := updated + timedelta(seconds=ttl_in_second)) > now:
+                return next_check_time
+
+    return None
 
 
-async def __monitor(feed: db.Feed) -> str:
+async def __monitor(feed: db.Feed, stat: MonitoringStat) -> None:
     """
     Monitor the update of a feed.
 
-    :param feed: the feed object to be monitored
-    :return: monitoring result
+    :param feed: Feed object to be monitored
+    :return: None
     """
     now = datetime.now(timezone.utc)
     if feed.next_check_time and now < feed.next_check_time:
-        return SKIPPED  # skip this monitor task
+        stat.skipped += 1
+        return  # skip this monitor task
 
     subs = await feed.subs.filter(state=1)
     if not subs:  # nobody has subbed it
         logger.warning(f'Feed {feed.id} ({feed.link}) has no active subscribers.')
-        await update_interval(feed)
-        return SKIPPED
+        await inner.utils.update_interval(feed)
+        stat.skipped += 1
+        return
 
     if all(locks.user_flood_lock(sub.user_id).locked() for sub in subs):
-        return SKIPPED  # all subscribers are experiencing flood wait, skip this monitor task
+        stat.skipped += 1
+        return  # all subscribers are experiencing flood wait, skip this monitor task
 
     headers = {
         'If-Modified-Since': format_datetime(feed.last_modified or feed.updated_at)
     }
     if feed.etag:
         headers['If-None-Match'] = feed.etag
 
     wf = await web.feed_get(feed.link, headers=headers, verbose=False)
     rss_d = wf.rss_d
 
     no_error = True
+    new_next_check_time: Optional[datetime] = None  # clear next_check_time by default
     feed_updated_fields = set()
     try:
         if wf.status == 304:  # cached
             logger.debug(f'Fetched (not updated, cached): {feed.link}')
-            return CACHED
+            stat.not_updated += 1
+            stat.cached += 1
+            return
 
         if rss_d is None:  # error occurred
             no_error = False
             feed.error_count += 1
             feed_updated_fields.add('error_count')
             if feed.error_count % 20 == 0:  # error_count is always > 0
                 logger.warning(f'Fetch failed ({feed.error_count}th retry, {wf.error}): {feed.link}')
             if feed.error_count >= 100:
-                logger.error(f'Deactivated feed due to too many errors: {feed.link}')
+                logger.error(f'Deactivated due to too many ({feed.error_count}) errors '
+                             f'(current: {wf.error}): {feed.link}')
                 await __deactivate_feed_and_notify_all(feed, subs, reason=wf.error)
-                return FAILED
-            if feed.error_count >= 10:  # too much error, delay next check
+                stat.failed += 1
+                return
+            if feed.error_count >= 10:  # too much error, defer next check
                 interval = feed.interval or db.EffectiveOptions.default_interval
-                next_check_interval = min(interval, 15) * min(feed.error_count // 10 + 1, 5)
-                if next_check_interval > interval:
-                    feed.next_check_time = now + timedelta(minutes=next_check_interval)
-                    feed_updated_fields.add('next_check_time')
-            return FAILED
+                if (next_check_interval := min(interval, 15) * min(feed.error_count // 10 + 1, 5)) > interval:
+                    new_next_check_time = now + timedelta(minutes=next_check_interval)
+            logger.debug(f'Fetched (failed, {feed.error_count}th retry, {wf.error}): {feed.link}')
+            stat.failed += 1
+            return
+
+        wr = wf.web_response
+        assert wr is not None
+        wr.now = now
 
-        etag = wf.headers and wf.headers.get('ETag')
-        if etag:
+        if (etag := wr.etag) and etag != feed.etag:
             feed.etag = etag
             feed_updated_fields.add('etag')
 
+        new_next_check_time = _defer_next_check_as_per_server_side_cache(wf)
+
         if not rss_d.entries:  # empty
-            logger.debug(f'Fetched (empty): {feed.link}')
-            return EMPTY
+            logger.debug(f'Fetched (not updated, empty): {feed.link}')
+            stat.not_updated += 1
+            stat.empty += 1
+            return
 
         title = rss_d.feed.title
         title = html_space_stripper(title) if title else ''
         if title != feed.title:
             logger.debug(f'Feed title changed ({feed.title} -> {title}): {feed.link}')
             feed.title = title
             feed_updated_fields.add('title')
 
-        new_hashes, updated_entries = calculate_update(feed.entry_hashes, rss_d.entries)
+        new_hashes, updated_entries = inner.utils.calculate_update(feed.entry_hashes, rss_d.entries)
         updated_entries = tuple(updated_entries)
 
         if not updated_entries:  # not updated
             logger.debug(f'Fetched (not updated): {feed.link}')
-            return NOT_UPDATED
+            stat.not_updated += 1
+            return
 
         logger.debug(f'Updated: {feed.link}')
-        feed.last_modified = inner.utils.get_http_last_modified(wf.headers)
+        feed.last_modified = wr.last_modified
         feed.entry_hashes = list(islice(new_hashes, max(len(rss_d.entries) * 2, 100))) or None
         feed_updated_fields.update({'last_modified', 'entry_hashes'})
     finally:
         if no_error:
             if feed.error_count > 0:
                 feed.error_count = 0
                 feed_updated_fields.add('error_count')
-            if feed.next_check_time:
-                feed.next_check_time = None
-                feed_updated_fields.add('next_check_time')
             if wf.url != feed.link:
                 new_url_feed = await inner.sub.migrate_to_new_url(feed, wf.url)
                 feed = new_url_feed if isinstance(new_url_feed, db.Feed) else feed
 
+        if new_next_check_time != feed.next_check_time:
+            feed.next_check_time = new_next_check_time
+            feed_updated_fields.add('next_check_time')
+
         if feed_updated_fields:
             await feed.save(update_fields=feed_updated_fields)
 
     await asyncio.gather(*(__notify_all(feed, subs, entry) for entry in reversed(updated_entries)))
-
-    return UPDATED
+    stat.updated += 1
+    return
 
 
 async def __notify_all(feed: db.Feed, subs: Iterable[db.Sub], entry: MutableMapping):
     link = entry.get('link')
     try:
         post = await get_post_from_entry(entry, feed.title, feed.link)
     except Exception as e:
@@ -244,15 +326,16 @@
                                  f'(feed: {feed.link}). '
                                  f'Please check:<br><br>' +
                                  format_exc().replace('\n', '<br>'),
                                  feed_title=feed.title, link=link)
             await error_message.send_formatted_post(env.ERROR_LOGGING_CHAT, send_mode=2)
         except Exception as e:
             logger.error(f'Failed to send parsing error message for {link} (feed: {feed.link}):', exc_info=e)
-            await env.bot.send_message(env.ERROR_LOGGING_CHAT, 'A parsing error message cannot be sent, please check the logs.')
+            await env.bot.send_message(env.ERROR_LOGGING_CHAT,
+                                       'A parsing error message cannot be sent, please check the logs.')
         return
     res = await asyncio.gather(
         *(asyncio.wait_for(__send(sub, post), 8.5 * 60) for sub in subs),
         return_exceptions=True
     )
     for sub, exc in zip(subs, res):
         if not isinstance(exc, Exception):
@@ -263,15 +346,15 @@
 
 
 async def __send(sub: db.Sub, post: Union[str, Post]):
     user_id = sub.user_id
     try:
         try:
             await env.bot.get_input_entity(user_id)  # verify that the input entity can be gotten first
-        except ValueError:  # cannot get the input entity, the bot may be banned by the user
+        except ValueError:  # cannot get the input entity, the user may have banned the bot
             return await __locked_unsub_all_and_leave_chat(user_id=user_id, err_msg=type(EntityNotFoundError).__name__)
         try:
             if isinstance(post, str):
                 await env.bot.send_message(user_id, post, parse_mode='html', silent=not sub.notify)
                 return
             await post.send_formatted_post_according_to_sub(sub)
             if __user_blocked_counter[user_id]:  # reset the counter if success
@@ -291,15 +374,16 @@
                                  title=post.title, feed_title=post.feed_title, link=post.link, author=post.author,
                                  feed_link=post.feed_link)
             await error_message.send_formatted_post(env.ERROR_LOGGING_CHAT, send_mode=2)
         except Exception as e:
             logger.error(f'Failed to send sending error message for {post.link} '
                          f'(feed: {post.feed_link}, user: {sub.user_id}):',
                          exc_info=e)
-            await env.bot.send_message(env.ERROR_LOGGING_CHAT, 'An sending error message cannot be sent, please check the logs.')
+            await env.bot.send_message(env.ERROR_LOGGING_CHAT,
+                                       'An sending error message cannot be sent, please check the logs.')
 
 
 async def __locked_unsub_all_and_leave_chat(user_id: int, err_msg: str):
     user_unsub_all_lock = __user_unsub_all_lock_bucket[user_id]
     if user_unsub_all_lock.locked():
         return  # no need to unsub twice!
     async with user_unsub_all_lock:
@@ -311,15 +395,15 @@
         logger.error(f'User blocked ({err_msg}): {user_id}')
         await unsub_all_and_leave_chat(user_id)
 
 
 async def __deactivate_feed_and_notify_all(feed: db.Feed,
                                            subs: Iterable[db.Sub],
                                            reason: Union[web.WebError, str] = None):
-    await deactivate_feed(feed)
+    await inner.utils.deactivate_feed(feed)
 
     if not subs:  # nobody has subbed it or no active sub exists
         return
 
     langs: tuple[str, ...] = await asyncio.gather(
         *(sub.user.get_or_none().values_list('lang', flat=True) for sub in subs)
     )
```

### Comparing `rsstt-2.6.0/src/command/opml.py` & `rsstt-2.7.0/src/command/opml.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/command/sub.py` & `rsstt-2.7.0/src/command/sub.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/command/utils.py` & `rsstt-2.7.0/src/command/utils.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/compat.py` & `rsstt-2.7.0/src/compat.py`

 * *Files 11% similar despite different names*

```diff
@@ -159,76 +159,80 @@
     return ret
 
 
 class OpmlMixin(listparser.opml.OpmlMixin):
     """
     Monkey-patching `listparser.opml.OpmlMixin` to support `text` and `title_orig`
     https://github.com/kurtmckee/listparser/issues/71
-    Copied and modified from
-    https://github.com/kurtmckee/listparser/blob/1910c45232f679e63294c1bc1bcc1520a10b0383/src/listparser/opml.py#L20-L82
+
+    Originated from listparser v0.20 (MIT License)
+    https://github.com/kurtmckee/listparser/blob/v0.20/src/listparser/opml.py#L21-L76
+    Copyright 2009-2024 Kurt McKee <contactme@kurtmckee.org>
+    Copyright 2023-2024 RSS to Telegram Bot contributors
+    Distributed along with RSS to Telegram Bot under AGPLv3 License
     """
 
-    def start_opml_outline(self, attrs):
-        url = None
+    def start_opml_outline(self, attrs: dict[str, str]) -> None:
         # Find an appropriate title in @text or @title (else empty)
-        text = attrs.get('text', '').strip()
-        title_orig = attrs.get('title', '').strip()
+        # ================ DIFF ================
+        # if attrs.get("text", "").strip():
+        #     title = attrs["text"].strip()
+        # else:
+        #     title = attrs.get("title", "").strip()
+        text = attrs.get("text", "").strip()
+        title_orig = attrs.get("title", "").strip()
         title = text or title_orig
 
-        # Search for the URL regardless of xmlUrl's case
-        for k, v in attrs.items():
-            if k.lower() == 'xmlurl':
-                url = v.strip()
-                break
-
+        url = None
         append_to = None
 
         # Determine whether the outline is a feed or subscription list
-        if url is not None:
+        if "xmlurl" in attrs:
             # It's a feed
-            append_to = 'feeds'
-            if attrs.get('type', '').strip().lower() == 'source':
+            url = attrs.get("xmlurl", "").strip()
+            append_to = "feeds"
+            if attrs.get("type", "").strip().lower() == "source":
                 # Actually, it's a subscription list!
-                append_to = 'lists'
-        elif attrs.get('type', '').lower() in ('link', 'include'):
+                append_to = "lists"
+        elif attrs.get("type", "").lower() in ("link", "include"):
             # It's a subscription list
-            append_to = 'lists'
-            url = attrs.get('url', '').strip()
+            append_to = "lists"
+            url = attrs.get("url", "").strip()
         elif title:
             # Assume that this is a grouping node
             self.hierarchy.append(title)
             return
         # Look for an opportunity URL
-        if not url and 'htmlurl' in (k.lower() for k in attrs.keys()):
-            for k, v in attrs.items():
-                if k.lower() == 'htmlurl':
-                    url = v.strip()
-            append_to = 'opportunities'
+        if not url and "htmlurl" in attrs:
+            url = attrs["htmlurl"].strip()
+            append_to = "opportunities"
         if not url:
             # Maintain the hierarchy
-            self.hierarchy.append('')
+            self.hierarchy.append("")
             return
         if url not in self.found_urls and append_to:
-            # This is a brand new URL
-            obj = listparser.common.SuperDict({'url': url, 'title': title, 'text': text, 'title_orig': title_orig})
+            # This is a brand-new URL
+            # ================ DIFF ================
+            # obj = common.SuperDict({"url": url, "title": title})
+            obj = listparser.common.SuperDict({"url": url, "title": title, "text": text, "title_orig": title_orig})
             self.found_urls[url] = (append_to, obj)
             self.harvest[append_to].append(obj)
         else:
             obj = self.found_urls[url][1]
 
         # Handle categories and tags
-        obj.setdefault('categories', [])
-        if 'category' in attrs.keys():
-            for i in attrs['category'].split(','):
-                tmp = [j.strip() for j in i.split('/') if j.strip()]
-                if tmp and tmp not in obj['categories']:
-                    obj['categories'].append(tmp)
+        obj.setdefault("categories", [])
+        if "category" in attrs.keys():
+            for i in attrs["category"].split(","):
+                tmp = [j.strip() for j in i.split("/") if j.strip()]
+                if tmp and tmp not in obj["categories"]:
+                    obj["categories"].append(tmp)
         # Copy the current hierarchy into `categories`
-        if self.hierarchy and self.hierarchy not in obj['categories']:
-            obj['categories'].append(copy.copy(self.hierarchy))
+        if self.hierarchy and self.hierarchy not in obj["categories"]:
+            obj["categories"].append(copy.copy(self.hierarchy))
         # Copy all single-element `categories` into `tags`
-        obj['tags'] = [i[0] for i in obj['categories'] if len(i) == 1]
+        obj["tags"] = [i[0] for i in obj["categories"] if len(i) == 1]
 
-        self.hierarchy.append('')
+        self.hierarchy.append("")
 
 
 listparser.opml.OpmlMixin.start_opml_outline = OpmlMixin.start_opml_outline
```

### Comparing `rsstt-2.6.0/src/db/effective_utils.py` & `rsstt-2.7.0/src/db/effective_utils.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/db/migrations_pgsql/models/0_20211117110249_init.sql` & `rsstt-2.7.0/src/db/migrations_pgsql/models/0_20211117110249_init.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
--- upgrade --
-CREATE TABLE IF NOT EXISTS "aerich" (
+from tortoise import BaseDBAsyncClient
+
+
+async def upgrade(db: BaseDBAsyncClient) -> str:
+    return """
+        CREATE TABLE IF NOT EXISTS "aerich" (
     "id" SERIAL NOT NULL PRIMARY KEY,
     "version" VARCHAR(255) NOT NULL,
     "app" VARCHAR(20) NOT NULL,
     "content" JSONB NOT NULL
 );
 CREATE TABLE IF NOT EXISTS "feed" (
     "created_at" TIMESTAMPTZ NOT NULL  DEFAULT CURRENT_TIMESTAMP,
@@ -82,8 +86,13 @@
 COMMENT ON COLUMN "sub"."send_mode" IS 'Send mode: -1=force link, 0=auto, 1=force Telegraph, 2=force message';
 COMMENT ON COLUMN "sub"."length_limit" IS 'Telegraph length limit, valid when send_mode==0. If exceed, send via Telegraph; If is 0, send via Telegraph when a post cannot be send in a single message';
 COMMENT ON COLUMN "sub"."link_preview" IS 'Enable link preview or not? 0=auto, 1=force enable';
 COMMENT ON COLUMN "sub"."display_author" IS 'Display author or not?-1=disable, 0=auto, 1=force display';
 COMMENT ON COLUMN "sub"."display_via" IS 'Display via or not?-2=completely disable, -1=disable but display link, 0=auto, 1=force display';
 COMMENT ON COLUMN "sub"."display_title" IS 'Display title or not?-1=disable, 0=auto, 1=force display';
 COMMENT ON COLUMN "sub"."style" IS 'Style of posts: 0=RSStT, 1=flowerss';
-COMMENT ON TABLE "sub" IS 'Sub model.';
+COMMENT ON TABLE "sub" IS 'Sub model.';"""
+
+
+async def downgrade(db: BaseDBAsyncClient) -> str:
+    return """
+        """
```

### Comparing `rsstt-2.6.0/src/db/migrations_pgsql/models/2_20220306045951_update.sql` & `rsstt-2.7.0/src/db/migrations_pgsql/models/2_20220306045951_update.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,31 @@
--- upgrade --
-ALTER TABLE "sub" ADD "display_media" SMALLINT NOT NULL  DEFAULT 0;
+from tortoise import BaseDBAsyncClient
+
+
+async def upgrade(db: BaseDBAsyncClient) -> str:
+    return """
+        ALTER TABLE "sub" ADD "display_media" SMALLINT NOT NULL  DEFAULT 0;
 ALTER TABLE "user" ADD "send_mode" SMALLINT NOT NULL  DEFAULT 0;
 ALTER TABLE "user" ADD "display_author" SMALLINT NOT NULL  DEFAULT 0;
 ALTER TABLE "user" ADD "display_media" SMALLINT NOT NULL  DEFAULT 0;
 ALTER TABLE "user" ADD "display_title" SMALLINT NOT NULL  DEFAULT 0;
 ALTER TABLE "user" ADD "notify" SMALLINT NOT NULL  DEFAULT 1;
 ALTER TABLE "user" ADD "link_preview" SMALLINT NOT NULL  DEFAULT 0;
 ALTER TABLE "user" ADD "style" SMALLINT NOT NULL  DEFAULT 0;
 ALTER TABLE "user" ADD "length_limit" SMALLINT NOT NULL  DEFAULT 0;
 ALTER TABLE "user" ADD "interval" SMALLINT;
-ALTER TABLE "user" ADD "display_via" SMALLINT NOT NULL  DEFAULT 0;
--- downgrade --
-ALTER TABLE "sub" DROP COLUMN "display_media";
+ALTER TABLE "user" ADD "display_via" SMALLINT NOT NULL  DEFAULT 0;"""
+
+
+async def downgrade(db: BaseDBAsyncClient) -> str:
+    return """
+        ALTER TABLE "sub" DROP COLUMN "display_media";
 ALTER TABLE "user" DROP COLUMN "send_mode";
 ALTER TABLE "user" DROP COLUMN "display_author";
 ALTER TABLE "user" DROP COLUMN "display_media";
 ALTER TABLE "user" DROP COLUMN "display_title";
 ALTER TABLE "user" DROP COLUMN "notify";
 ALTER TABLE "user" DROP COLUMN "link_preview";
 ALTER TABLE "user" DROP COLUMN "style";
 ALTER TABLE "user" DROP COLUMN "length_limit";
 ALTER TABLE "user" DROP COLUMN "interval";
-ALTER TABLE "user" DROP COLUMN "display_via";
+ALTER TABLE "user" DROP COLUMN "display_via";"""
```

### Comparing `rsstt-2.6.0/src/db/migrations_sqlite/models/0_20211117110249_init.sql` & `rsstt-2.7.0/src/db/migrations_sqlite/models/0_20211117110249_init.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,13 @@
--- upgrade --
-CREATE TABLE IF NOT EXISTS "aerich" (
+from tortoise import BaseDBAsyncClient
+
+
+async def upgrade(db: BaseDBAsyncClient) -> str:
+    return """
+        CREATE TABLE IF NOT EXISTS "aerich" (
     "id" INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL,
     "version" VARCHAR(255) NOT NULL,
     "app" VARCHAR(20) NOT NULL,
     "content" JSON NOT NULL
 );
 CREATE TABLE IF NOT EXISTS "feed" (
     "created_at" TIMESTAMP NOT NULL  DEFAULT CURRENT_TIMESTAMP /* The time this row was created */,
@@ -47,8 +51,13 @@
     "display_author" SMALLINT NOT NULL  DEFAULT 0 /* Display author or not?-1=disable, 0=auto, 1=force display */,
     "display_via" SMALLINT NOT NULL  DEFAULT 0 /* Display via or not?-2=completely disable, -1=disable but display link, 0=auto, 1=force display */,
     "display_title" SMALLINT NOT NULL  DEFAULT 0 /* Display title or not?-1=disable, 0=auto, 1=force display */,
     "style" SMALLINT NOT NULL  DEFAULT 0 /* Style of posts: 0=RSStT, 1=flowerss */,
     "feed_id" INT NOT NULL REFERENCES "feed" ("id") ON DELETE CASCADE,
     "user_id" BIGINT NOT NULL REFERENCES "user" ("id") ON DELETE CASCADE,
     CONSTRAINT "uid_sub_user_id_029239" UNIQUE ("user_id", "feed_id")
-) /* Sub model. */;
+) /* Sub model. */;"""
+
+
+async def downgrade(db: BaseDBAsyncClient) -> str:
+    return """
+        """
```

### Comparing `rsstt-2.6.0/src/db/models.py` & `rsstt-2.7.0/src/db/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     notify = fields.SmallIntField(default=1)
     send_mode = fields.SmallIntField(default=0)
     length_limit = fields.SmallIntField(default=0)
     link_preview = fields.SmallIntField(default=0)
     display_author = fields.SmallIntField(default=0)
     display_via = fields.SmallIntField(default=0)
     display_title = fields.SmallIntField(default=0)
+    display_entry_tags = fields.SmallIntField(default=-1)
     style = fields.SmallIntField(default=0)
     display_media = fields.SmallIntField(default=0)
 
     class Meta:
         table = 'user'
 
     def __str__(self):
@@ -84,14 +85,16 @@
     class Meta:
         table = 'feed'
 
     def __str__(self):
         return self.link
 
 
+# TODO: migrate the default value of all fields after `notify` (inclusive) to -100
+# TODO: description makes a lot trouble on SQLite, remove the description of all fields after `notify` (inclusive)
 class Sub(Model, Base):
     """
     Sub model.
 
     Stores subscriptions (who subscribed which feed) and their options, many to many relation.
     """
     id = fields.IntField(pk=True)
@@ -118,14 +121,16 @@
     display_author = fields.SmallIntField(default=0, description='Display author or not?'
                                                                  '-1=disable, 0=auto, 1=force display')
     display_via = fields.SmallIntField(default=0, description='Display via or not?'
                                                               '-2=completely disable, -1=disable but display link, '
                                                               '0=auto, 1=force display')
     display_title = fields.SmallIntField(default=0, description='Display title or not?'
                                                                 '-1=disable, 0=auto, 1=force display')
+    # new field, use the de facto default value (-100) and with description unset to avoid future migration
+    display_entry_tags = fields.SmallIntField(default=-100)
     style = fields.SmallIntField(default=0, description='Style of posts: '
                                                         '0=RSStT, 1=flowerss')
     display_media = fields.SmallIntField(default=0, description='Display media or not?'
                                                                 '-1=disable, 0=enable')
 
     class Meta:
         table = 'sub'
```

### Comparing `rsstt-2.6.0/src/env.py` & `rsstt-2.7.0/src/env.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
-from typing import Optional
+from typing import Optional, Union
 from typing_extensions import Final
 
 import asyncio
 import os
 import sys
 import colorlog
 import re
 import argparse
 from telethon import TelegramClient
 from telethon.tl.types import User, InputPeerUser
 from python_socks import parse_proxy_url
 from dotenv import load_dotenv
 from pathlib import Path
-from distutils.version import StrictVersion
 from functools import partial
 
 from .version import __version__
 
 
 # ----- utils -----
 def __bool_parser(var: Optional[str], default_value: bool = False) -> bool:
@@ -35,14 +34,53 @@
     return default_value
 
 
 def __list_parser(var: Optional[str]) -> list[str]:
     return re.split(r'[\s,;，；]+', var.strip()) if var else []
 
 
+def __decompose_version(version: str) -> list[Union[int, str]]:
+    def buf_put(as_int: bool):
+        nonlocal buf
+        if not buf:
+            raise ValueError(f'Empty part in version string: {version}')
+        parts.append(int(buf) if as_int else buf)
+        buf = ''
+
+    parts = []
+    buf = ''
+    for i, char in enumerate(version):
+        if char == '.':
+            buf_put(as_int=True)
+            continue
+        if not char.isdecimal():
+            buf_put(as_int=True)
+            parts.append(version[i:])
+            break
+        buf += char
+    if buf:
+        buf_put(as_int=True)
+    return parts
+
+
+def __compare_version(version1: str, version2: str) -> tuple[int, list[Union[int, str]], list[Union[int, str]]]:
+    """loose comparison, only compare the numeric parts"""
+    parts1 = __decompose_version(version1)
+    parts2 = __decompose_version(version2)
+    marker = 0
+    for part1, part2 in zip(parts1, parts2):
+        if not (isinstance(part1, int) and isinstance(part2, int)):
+            break
+        if part1 == part2:
+            continue
+        marker = 1 if part1 > part2 else -1
+        break
+    return marker, parts1, parts2
+
+
 # ----- setup logging -----
 __configure_logging = partial(
     colorlog.basicConfig,
     format='%(log_color)s%(asctime)s:%(levelname)s:%(name)s - %(message)s',
     datefmt='%Y-%m-%d-%H:%M:%S'
 )
 __configure_logging(level=colorlog.DEBUG if __bool_parser(os.environ.get('DEBUG')) else colorlog.INFO)
@@ -77,65 +115,65 @@
 logger.info(f'Config folder: {config_folder_path}')
 
 # ----- load .env -----
 dot_env_paths = (os.path.join(config_folder_path, '.env'),
                  os.path.join(os.path.abspath('.'), '.env'))
 if is_self_run_as_a_whole_package:
     dot_env_paths = (os.path.normpath(os.path.join(self_path, '..', '.env')),) + dot_env_paths
-for dot_env_path in sorted(set(dot_env_paths), key=dot_env_paths.index):
+for dot_env_path in dict.fromkeys(dot_env_paths):  # remove duplicates while keeping the order
     if os.path.isfile(dot_env_path):
         load_dotenv(dot_env_path, override=True)
         logger.info(f'Found .env file at "{dot_env_path}", loaded')
 
+
 # ----- get version -----
-_version = 'dirty'
+def __get_version():
+    version = 'dirty'
+    if is_self_run_as_a_whole_package:
+        # noinspection PyBroadException
+        try:
+            with open(os.path.normpath(os.path.join(self_path, '..', '.version')), 'r') as v:
+                version = v.read().strip()
+        except Exception:
+            version = 'dirty'
+
+        if not version or version == '@':
+            version = 'dirty'
+
+    if version == 'dirty':
+        from subprocess import Popen, PIPE, DEVNULL
+
+        # noinspection PyBroadException
+        try:
+            with Popen(['git', 'describe', '--tags', '--dirty', '--broken', '--always'],
+                       shell=False, stdout=PIPE, stderr=DEVNULL, bufsize=-1) as git:
+                git.wait(3)
+                version = git.stdout.read().decode().strip()
+            with Popen(['git', 'branch', '--show-current'],
+                       shell=False, stdout=PIPE, stderr=DEVNULL, bufsize=-1) as git:
+                git.wait(3)
+                if branch := git.stdout.read().decode().strip():
+                    version += f'@{branch}'
+        except Exception:
+            version = 'dirty'
 
-if is_self_run_as_a_whole_package:
-    # noinspection PyBroadException
     try:
-        with open(os.path.normpath(os.path.join(self_path, '..', '.version')), 'r') as v:
-            _version = v.read().strip()
-    except Exception:
-        _version = 'dirty'
-
-    if not _version or _version == '@':
-        _version = 'dirty'
-
-if _version == 'dirty':
-    from subprocess import Popen, PIPE, DEVNULL
+        sign, version_decomposed, version_pkg_decomposed = __compare_version(version.lstrip('v'), __version__)
+        if sign <= -1:  # outdated version: older than pkg ver
+            version = __version__
+            if isinstance(version_decomposed[-1], str) and not isinstance(version_pkg_decomposed[-1], str):
+                version += re.sub(r'^-\d+(?=-)', '', version_decomposed[-1])  # trim ahead commit count
+            version = f'v{version}'
+    except ValueError:
+        version = f'v{__version__}'
 
-    # noinspection PyBroadException
-    try:
-        with Popen(['git', 'describe', '--tags', '--dirty', '--broken', '--always'],
-                   shell=False, stdout=PIPE, stderr=DEVNULL, bufsize=-1) as __git:
-            __git.wait(3)
-            _version = __git.stdout.read().decode().strip()
-        with Popen(['git', 'branch', '--show-current'],
-                   shell=False, stdout=PIPE, stderr=DEVNULL, bufsize=-1) as __git:
-            __git.wait(3)
-            __git = __git.stdout.read().decode().strip()
-            if __git:
-                _version += f'@{__git}'
-    except Exception:
-        _version = 'dirty'
+    return version
 
-_version_match = re.match(r'^v?\d+\.\d+(\.\w+(\.\w+)?)?', _version)
-if _version_match:
-    try:
-        if StrictVersion(_version_match[0].lstrip('v')) < StrictVersion(__version__):
-            _version = _version[_version_match.end():]
-            _version = re.sub(r'(?<!\d{4})-\d+-(?!\d{2})', '', _version, count=1)
-            _version = f'v{__version__}-{_version}' if _version else f'v{__version__}'
-    except ValueError:
-        _version = f'v{__version__}'
-else:
-    _version = f'v{__version__}' + (f'-{_version}' if _version and _version != 'dirty' else '')
 
-VERSION: Final = _version
-del _version, _version_match
+VERSION: Final = __get_version()
 
 # ----- basic config -----
 SAMPLE_APIS: Final = {
     # https://github.com/DrKLO/Telegram/blob/master/TMessagesProj/src/main/java/org/telegram/messenger/BuildVars.java
     4: '014b35b6184100b085b0d0572f9b5103',
     # https://github.com/TelegramMessenger/Telegram-iOS/blob/master/build-system/verify.sh
     8: '7245de8e747a0d6fbe11f7cc14fcc0bb',
```

### Comparing `rsstt-2.6.0/src/errors_collection.py` & `rsstt-2.7.0/src/errors_collection.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/__init__.py` & `rsstt-2.7.0/src/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/ar.json` & `rsstt-2.7.0/src/i18n/ar.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/ca.json` & `rsstt-2.7.0/src/i18n/ca.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/cs.json` & `rsstt-2.7.0/src/i18n/cs.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/de.json` & `rsstt-2.7.0/src/i18n/de.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/el.json` & `rsstt-2.7.0/src/i18n/el.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/en.json` & `rsstt-2.7.0/src/i18n/en.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985849056603773%*

 * *Differences: {"'l10n_cmd_set'": "{'display_entry_tags': 'Hashtags from post (feed entry)', "*

 * *                   "'display_entry_tags_-1': 'Disable', 'display_entry_tags_1': 'Enable'}"}*

```diff
@@ -68,14 +68,17 @@
         "send_opml_reply_placeholder": "The OPML file to be imported (extension name must be .opml)"
     },
     "l10n_cmd_set": {
         "display_author": "Author",
         "display_author_-1": "Disable",
         "display_author_0": "Auto",
         "display_author_1": "Enable",
+        "display_entry_tags": "Hashtags from post (feed entry)",
+        "display_entry_tags_-1": "Disable",
+        "display_entry_tags_1": "Enable",
         "display_media": "Media",
         "display_media_-1": "Disable",
         "display_media_0": "Enable",
         "display_media_1": "Only media, no content",
         "display_media_only_effective_if_send_mode_auto_and_telegram": "The current send mode will never display media in Telegram messages.",
         "display_title": "Post title",
         "display_title_-1": "Disable",
```

### Comparing `rsstt-2.6.0/src/i18n/es.json` & `rsstt-2.7.0/src/i18n/es.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/eu.json` & `rsstt-2.7.0/src/i18n/eu.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/fa.json` & `rsstt-2.7.0/src/i18n/uz.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9672985347985348%*

 * *Differences: {"'l10n_error_reasons'": "{'feed_invalid': 'RSS feed yaroqsiz', 'url_invalid': 'URL yaroqsiz', "*

 * *                         "'network_error': 'Tarmoq xatosi', 'internal_error': 'Ichki xato', "*

 * *                         "'status_code_error': 'HTTP holat kodi hatoligi', "*

 * *                         "'uncaught_internal_error': 'Tugallanmagan ichki xato', "*

 * *                         "'operation_timeout_error': 'Operatsiya vaqti tugashi', 'action_invalid': "*

 * *                         "'Amaliyot yaroqsiz', 'sub_limit_re […]*

```diff
@@ -158,47 +158,47 @@
     "l10n_cmd_unsub_all": {
         "unsub_all_cancel": "",
         "unsub_all_confirm": "",
         "unsub_all_confirm_prompt": "",
         "unsub_all_successful": ""
     },
     "l10n_error_reasons": {
-        "action_invalid": "\u0627\u0642\u062f\u0627\u0645 \u0646\u0627\u0645\u0639\u062a\u0628\u0631",
+        "action_invalid": "Amaliyot yaroqsiz",
         "callback_already_running_prompt": "",
         "edit_conflict_prompt": "",
-        "feed_invalid": "\u062e\u0648\u0631\u0627\u06a9 RSS \u0645\u0639\u062a\u0628\u0631 \u0646\u06cc\u0633\u062a",
+        "feed_invalid": "RSS feed yaroqsiz",
         "flood_wait_prompt": "",
-        "internal_error": "\u062e\u0637\u0627\u06cc \u062f\u0627\u062e\u0644\u06cc",
+        "internal_error": "Ichki xato",
         "message_too_long_prompt": "",
-        "network_error": "\u062e\u0637\u0627 \u062f\u0631 \u0634\u0628\u06a9\u0647",
-        "operation_timeout_error": "\u067e\u0627\u06cc\u0627\u0646 \u0632\u0645\u0627\u0646 \u0639\u0645\u0644\u06cc\u0627\u062a",
-        "status_code_error": "\u062e\u0637\u0627 \u062f\u0631 \u0648\u0636\u0639\u06cc\u062a HTTP",
-        "sub_limit_reached": "\u0645\u0642\u062f\u0627\u0631 \u0627\u0634\u062a\u0631\u0627\u06a9 \u062f\u0631 \u062d\u0627\u0644 \u0631\u0633\u06cc\u062f\u0646 \u0628\u0647 \u0645\u062d\u062f\u0648\u062f\u06cc\u062a\u200c\u0647\u0627 \u0627\u0633\u062a",
-        "uncaught_internal_error": "\u062e\u0637\u0627\u06cc \u06a9\u0634\u0641 \u0646\u0634\u062f\u0647",
-        "url_invalid": "URL \u0645\u0639\u062a\u0628\u0631 \u0646\u06cc\u0633\u062a"
+        "network_error": "Tarmoq xatosi",
+        "operation_timeout_error": "Operatsiya vaqti tugashi",
+        "status_code_error": "HTTP holat kodi hatoligi",
+        "sub_limit_reached": "Obuna soni chegarasiga yetdi",
+        "uncaught_internal_error": "Tugallanmagan ichki xato",
+        "url_invalid": "URL yaroqsiz"
     },
     "l10n_info": {
-        "iso_639_code": "fa",
-        "lang_code": "fa",
-        "lang_native_name": "\u0641\u0627\u0631\u0633\u06cc",
-        "language_name": "\u0641\u0627\u0631\u0633\u06cc",
+        "iso_639_code": "uz",
+        "lang_code": "uz",
+        "lang_native_name": "",
+        "language_name": "",
         "rsstt_slogan": "",
-        "select_lang_prompt": "\u0644\u0637\u0641\u0627 \u0632\u0628\u0627\u0646 \u062e\u0648\u062f \u0631\u0627 \u0627\u0646\u062a\u062e\u0627\u0628 \u06a9\u0646\u06cc\u062f.",
-        "welcome_prompt": "\u0628\u0647 \u0631\u0628\u0627\u062a RSS to Telegram \u062e\u0648\u0634 \u0622\u0645\u062f\u06cc\u062f."
+        "select_lang_prompt": "",
+        "welcome_prompt": ""
     },
     "l10n_misc": {
         "back": "",
         "cancel": "",
         "canceled_by_user": "",
         "channel": "",
         "choose_sub_prompt": "",
         "group": "",
         "n_subscriptions_in_total": "",
         "next_page": "",
-        "other_settings_button": "\u0633\u0627\u06cc\u0631 \u062a\u0646\u0638\u06cc\u0645\u0627\u062a \u2026",
+        "other_settings_button": "",
         "previous_page": "",
         "processing": "",
         "subscribe": "",
         "subscription_list": "",
         "unsubscribe": "",
         "user": ""
     },
@@ -225,12 +225,12 @@
         "feed_title": "",
         "feed_url": "",
         "hashtags": "",
         "subscription_info": "",
         "subscription_title": ""
     },
     "l10n_sub_status": {
-        "already_subscribed": "\u0627\u0634\u062a\u0631\u0627\u06a9 \u062f\u0627\u0631\u06cc\u062f",
-        "no_subscription": "\u0634\u0645\u0627 \u0647\u06cc\u0686 \u0627\u0634\u062a\u0631\u0627\u06a9\u06cc \u0646\u062f\u0627\u0631\u06cc\u062f",
-        "subscription_not_exist": "\u0627\u0634\u062a\u0631\u0627\u06a9 \u0645\u0639\u062a\u0628\u0631 \u0646\u06cc\u0633\u062a"
+        "already_subscribed": "",
+        "no_subscription": "",
+        "subscription_not_exist": ""
     }
 }
```

### Comparing `rsstt-2.6.0/src/i18n/fr.json` & `rsstt-2.7.0/src/i18n/fr.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/he.json` & `rsstt-2.7.0/src/i18n/he.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/id.json` & `rsstt-2.7.0/src/i18n/id.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/it.json` & `rsstt-2.7.0/src/i18n/it.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/ja.json` & `rsstt-2.7.0/src/i18n/ja.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/ko.json` & `rsstt-2.7.0/src/i18n/ko.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/pl.json` & `rsstt-2.7.0/src/i18n/pl.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/pt.json` & `rsstt-2.7.0/src/i18n/pt.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/ru.json` & `rsstt-2.7.0/src/i18n/ru.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/si.json` & `rsstt-2.7.0/src/i18n/si.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/tr.json` & `rsstt-2.7.0/src/i18n/tr.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/uk.json` & `rsstt-2.7.0/src/i18n/uk.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/i18n/yue.json` & `rsstt-2.7.0/src/i18n/yue.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985849056603773%*

 * *Differences: {"'l10n_cmd_set'": "{'display_entry_tags': '嚟自文章 (源條目) 嘅 hashtag', 'display_entry_tags_-1': '閂', "*

 * *                   "'display_entry_tags_1': '開'}"}*

```diff
@@ -68,14 +68,17 @@
         "send_opml_reply_placeholder": "OPML \u6a94\u6848 (\u526f\u6a94\u540d\u4e00\u5b9a\u8981\u4fc2 .opml)"
     },
     "l10n_cmd_set": {
         "display_author": "\u4f5c\u8005",
         "display_author_-1": "\u9582",
         "display_author_0": "\u81ea\u52d5",
         "display_author_1": "\u958b",
+        "display_entry_tags": "\u569f\u81ea\u6587\u7ae0 (\u6e90\u689d\u76ee) \u5605 hashtag",
+        "display_entry_tags_-1": "\u9582",
+        "display_entry_tags_1": "\u958b",
         "display_media": "\u5a92\u9ad4",
         "display_media_-1": "\u9582",
         "display_media_0": "\u958b",
         "display_media_1": "\u53ea\u6709\u5a92\u9ad4\uff0c\u5187\u5167\u5bb9",
         "display_media_only_effective_if_send_mode_auto_and_telegram": "\u800c\u5bb6\u5605\u50b3\u9001\u65b9\u5f0f\u9ede\u90fd\u5514\u6703\u55ba Telegram \u8a0a\u606f\u5ea6\u5c55\u793a\u5a92\u9ad4\u3002",
         "display_title": "\u6587\u7ae0\u6a19\u984c",
         "display_title_-1": "\u9582",
```

### Comparing `rsstt-2.6.0/src/i18n/zh-Hans.json` & `rsstt-2.7.0/src/i18n/zh-Hans.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985849056603773%*

 * *Differences: {"'l10n_cmd_set'": "{'display_entry_tags': '来自文章 (源条目) 的 hashtag', 'display_entry_tags_-1': '禁用', "*

 * *                   "'display_entry_tags_1': '启用'}"}*

```diff
@@ -68,14 +68,17 @@
         "send_opml_reply_placeholder": "OPML \u6587\u4ef6 (\u6269\u5c55\u540d\u5fc5\u987b\u4e3a .opml)"
     },
     "l10n_cmd_set": {
         "display_author": "\u4f5c\u8005",
         "display_author_-1": "\u7981\u7528",
         "display_author_0": "\u81ea\u52a8",
         "display_author_1": "\u542f\u7528",
+        "display_entry_tags": "\u6765\u81ea\u6587\u7ae0 (\u6e90\u6761\u76ee) \u7684 hashtag",
+        "display_entry_tags_-1": "\u7981\u7528",
+        "display_entry_tags_1": "\u542f\u7528",
         "display_media": "\u5a92\u4f53",
         "display_media_-1": "\u7981\u7528",
         "display_media_0": "\u542f\u7528",
         "display_media_1": "\u4ec5\u5a92\u4f53\uff0c\u65e0\u5185\u5bb9",
         "display_media_only_effective_if_send_mode_auto_and_telegram": "\u76ee\u524d\u7684\u53d1\u9001\u65b9\u5f0f\u6c38\u8fdc\u4e0d\u5728 Telegram \u6d88\u606f\u91cc\u663e\u793a\u5a92\u4f53\u3002",
         "display_title": "\u6587\u7ae0\u6807\u9898",
         "display_title_-1": "\u7981\u7528",
```

### Comparing `rsstt-2.6.0/src/i18n/zh-Hant.json` & `rsstt-2.7.0/src/i18n/zh-Hant.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985849056603773%*

 * *Differences: {"'l10n_cmd_set'": "{'display_entry_tags': '來自文章 (源條目) 的 hashtag', 'display_entry_tags_-1': '禁用', "*

 * *                   "'display_entry_tags_1': '啟用'}"}*

```diff
@@ -68,14 +68,17 @@
         "send_opml_reply_placeholder": "OPML \u6a94 (\u64f4\u5c55\u540d\u5fc5\u9808\u7232 .opml)"
     },
     "l10n_cmd_set": {
         "display_author": "\u4f5c\u8005",
         "display_author_-1": "\u7981\u7528",
         "display_author_0": "\u81ea\u52d5",
         "display_author_1": "\u555f\u7528",
+        "display_entry_tags": "\u4f86\u81ea\u6587\u7ae0 (\u6e90\u689d\u76ee) \u7684 hashtag",
+        "display_entry_tags_-1": "\u7981\u7528",
+        "display_entry_tags_1": "\u555f\u7528",
         "display_media": "\u5a92\u9ad4",
         "display_media_-1": "\u7981\u7528",
         "display_media_0": "\u555f\u7528",
         "display_media_1": "\u50c5\u5a92\u9ad4\uff0c\u7121\u5167\u5bb9",
         "display_media_only_effective_if_send_mode_auto_and_telegram": "\u73fe\u5728\u7684\u50b3\u9001\u65b9\u5f0f\u6c38\u9060\u4e0d\u6703\u5728 Telegram \u6d88\u606f\u4e2d\u986f\u793a\u5a92\u9ad4\u3002",
         "display_title": "\u6587\u7ae0\u6a19\u984c",
         "display_title_-1": "\u7981\u7528",
```

### Comparing `rsstt-2.6.0/src/locks.py` & `rsstt-2.7.0/src/locks.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/log.py` & `rsstt-2.7.0/src/log.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/parsing/emojify.json` & `rsstt-2.7.0/src/parsing/emojify.json`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/parsing/html_node.py` & `rsstt-2.7.0/src/parsing/html_node.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/parsing/html_parser.py` & `rsstt-2.7.0/src/parsing/html_parser.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/parsing/medium.py` & `rsstt-2.7.0/src/parsing/medium.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,16 +249,16 @@
     typeFallbackAllowSelfUrls: bool = False
     # noinspection PyTypeChecker
     inputMediaExternalType: Optional[Union[type[InputMediaPhotoExternal], type[InputMediaDocumentExternal]]] = None
 
     def __init__(self, urls: Union[str, list[str]], type_fallback_urls: Optional[Union[str, list[str]]] = None):
         super().__init__()
         urls = urls if isinstance(urls, list) else [urls]
-        # dedup, should not use a set because sequence is important
-        self.urls: list[str] = sorted(set(urls), key=urls.index)
+        # dedup while keeping the order
+        self.urls: list[str] = list(dict.fromkeys(urls))
         self.original_urls: tuple[str, ...] = tuple(self.urls)
         self.chosen_url: Optional[str] = self.urls[0]
         self._server_change_count: int = 0
         self.size = self.width = self.height = None
         self.max_width = self.max_height = -1  # use for long pic judgment
         self.type_fallback_urls: list[str] = type_fallback_urls if isinstance(type_fallback_urls, list) \
             else [type_fallback_urls] if type_fallback_urls and isinstance(type_fallback_urls, str) \
@@ -873,15 +873,16 @@
         videos: list[tuple[Union[MessageMediaDocument, Video], Union[VIDEO]]] = []
         gifs: list[tuple[Union[MessageMediaDocument, Animation], ANIMATION]] = []
         audios: list[tuple[Union[MessageMediaDocument, Audio], AUDIO]] = []
         files: list[tuple[Union[MessageMediaDocument, File], FILE]] = []
 
         link_nodes: list[Text] = []
         for medium, medium_and_type in zip(self._media, media_and_types):
-            if isinstance(medium_and_type, Exception):
+            # Since Python 3.8, asyncio.CancelledError has been a subclass of BaseException rather than Exception
+            if isinstance(medium_and_type, (Exception, asyncio.CancelledError)):
                 if type(medium_and_type) in UserBlockedErrors:  # user blocked, let it go
                     raise medium_and_type
                 logger.debug('Upload media failed:', exc_info=medium_and_type)
                 link_nodes.append(medium.get_link_html_node())
                 continue
             file, file_type = medium_and_type
             if file_type == IMAGE:
```

### Comparing `rsstt-2.6.0/src/parsing/message.py` & `rsstt-2.7.0/src/parsing/message.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/parsing/post.py` & `rsstt-2.7.0/src/parsing/post.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,69 @@
 from __future__ import annotations
 from typing import Optional
 
-from .. import db, env
+from .. import db
 from ..errors_collection import MediaSendFailErrors
 from .utils import parse_entry, logger, Enclosure
 from .post_formatter import PostFormatter
 from .message import MessageDispatcher
 
 
 async def get_post_from_entry(entry, feed_title: str, feed_link: str = None) -> 'Post':
     entry_parsed = await parse_entry(entry, feed_link)
-    return Post(entry_parsed.content, entry_parsed.title, feed_title, entry_parsed.link, entry_parsed.author,
-                feed_link=feed_link, enclosures=entry_parsed.enclosures)
+    return Post(
+        html=entry_parsed.content,
+        title=entry_parsed.title,
+        feed_title=feed_title,
+        link=entry_parsed.link,
+        author=entry_parsed.author,
+        tags=entry_parsed.tags,
+        feed_link=feed_link,
+        enclosures=entry_parsed.enclosures
+    )
 
 
 class Post:
     def __init__(self,
                  html: str,
                  title: Optional[str] = None,
                  feed_title: Optional[str] = None,
                  link: Optional[str] = None,
                  author: Optional[str] = None,
+                 tags: Optional[list[str]] = None,
                  feed_link: Optional[str] = None,
                  enclosures: list[Enclosure] = None):
         """
         :param html: HTML content
         :param title: post title
         :param feed_title: feed title
         :param link: post link
         :param author: post author
+        :param tags: post tags
         :param feed_link: the url of the feed where the post from
         """
         self.html = html
         self.title = title
         self.feed_title = feed_title
         self.link = link
         self.author = author
+        self.tags = tags
         self.feed_link = feed_link
         self.enclosures = enclosures
 
-        self.post_formatter = PostFormatter(html=self.html,
-                                            title=self.title,
-                                            feed_title=self.feed_title,
-                                            link=self.link,
-                                            author=self.author,
-                                            feed_link=self.feed_link,
-                                            enclosures=self.enclosures)
+        self.post_formatter = PostFormatter(
+            html=self.html,
+            title=self.title,
+            feed_title=self.feed_title,
+            link=self.link,
+            author=self.author,
+            tags=self.tags,
+            feed_link=self.feed_link,
+            enclosures=self.enclosures
+        )
 
     async def send_formatted_post_according_to_sub(self, sub: db.Sub):
         if not isinstance(sub.feed, db.User):
             await sub.fetch_related('user')
         user: db.User = sub.user
         await self.send_formatted_post(
             user_id=sub.user_id,
@@ -57,14 +71,15 @@
             tags=sub.tags.split(' ') if sub.tags else [],
             send_mode=sub.send_mode if sub.send_mode != -100 else user.send_mode,
             length_limit=sub.length_limit if sub.length_limit != -100 else user.length_limit,
             link_preview=sub.link_preview if sub.link_preview != -100 else user.link_preview,
             display_author=sub.display_author if sub.display_author != -100 else user.display_author,
             display_via=sub.display_via if sub.display_via != -100 else user.display_via,
             display_title=sub.display_title if sub.display_title != -100 else user.display_title,
+            display_entry_tags=sub.display_entry_tags if sub.display_entry_tags != -100 else user.display_entry_tags,
             style=sub.style if sub.style != -100 else user.style,
             display_media=sub.display_media if sub.display_media != -100 else user.display_media,
             silent=not (sub.notify if sub.notify != -100 else user.notify)
         )
 
     async def send_formatted_post(self,
                                   user_id: int,
@@ -72,14 +87,15 @@
                                   tags: Optional[list[str]] = None,
                                   send_mode: int = 0,
                                   length_limit: int = 0,
                                   link_preview: int = 0,
                                   display_author: int = 0,
                                   display_via: int = 0,
                                   display_title: int = 0,
+                                  display_entry_tags: int = -1,
                                   style: int = 0,
                                   display_media: int = 0,
                                   silent: bool = False):
         """
         Send formatted post.
 
         :param user_id: user id
@@ -88,14 +104,15 @@
         :param send_mode: -1=force link, 0=auto, 1=force Telegraph, 2=force message
         :param length_limit: Telegraph length limit, valid when send_mode==0. If exceeded, send via Telegraph; If is 0,
             send via Telegraph when a post cannot be sent in a single message
         :param link_preview: 0=auto, 1=force enable
         :param display_author: -1=disable, 0=auto, 1=force display
         :param display_via: -2=completely disable, -1=disable but display link, 0=auto, 1=force display
         :param display_title: -1=disable, 0=auto, 1=force display
+        :param display_entry_tags: -1=disable, 1=force display
         :param style: 0=RSStT, 1=flowerss
         :param display_media: -1=disable, 0=enable
         :param silent: whether to send with notification sound
         """
         for _ in range(3):
             try:
                 formatted_post_tuple = \
@@ -103,14 +120,15 @@
                                                                  tags=tags,
                                                                  send_mode=send_mode,
                                                                  length_limit=length_limit,
                                                                  link_preview=link_preview,
                                                                  display_author=display_author,
                                                                  display_via=display_via,
                                                                  display_title=display_title,
+                                                                 display_entry_tags=display_entry_tags,
                                                                  style=style,
                                                                  display_media=display_media)
 
                 if formatted_post_tuple is None:
                     logger.debug(f'Post {self.link} is not sent to user {user_id} due to empty content')
                     return  # skip
 
@@ -164,10 +182,11 @@
                 length_limit=user.length_limit,
                 link_preview=user.link_preview,
                 display_author=user.display_author,
                 display_via=user.display_via,
                 display_title=user.display_title,
                 style=user.style,
                 display_media=user.display_media,
-                silent=not user.notify
+                silent=not user.notify,
+                display_entry_tags=user.display_entry_tags,
             )
         return await self.send_formatted_post_according_to_sub(sub=sub)
```

### Comparing `rsstt-2.6.0/src/parsing/post_formatter.py` & `rsstt-2.7.0/src/parsing/post_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,39 +62,43 @@
 class PostFormatter:
     def __init__(self,
                  html: str,
                  title: Optional[str] = None,
                  feed_title: Optional[str] = None,
                  link: Optional[str] = None,
                  author: Optional[str] = None,
+                 tags: Optional[list[str]] = None,
                  feed_link: str = None,
                  enclosures: list[utils.Enclosure] = None):
         """
         :param html: HTML content
         :param title: post title
         :param feed_title: feed title
         :param link: post link
         :param author: post author
+        :param tags: post tags
         :param feed_link: the url of the feed where the post from
         """
         self.html = html
         self.title = title
         self.feed_title = feed_title
         self.link = link
         self.author = author
+        self.tags = tags
         self.feed_link = feed_link
         self.enclosures = enclosures
 
         self.parsed: bool = False
         self.html_tree: Optional[HtmlTree] = None
         self.media: Optional[Media] = None
         self.enclosure_medium_l: Optional[list[AbstractMedium]] = None
         self.parsed_html: Optional[str] = None
         self.plain_length: Optional[int] = None
         self.telegraph_link: Optional[Union[str, False]] = None  # if generating failed, will be False
+        self.tags_escaped: Optional[list[str]] = None
 
         self.__title_similarity: Optional[int] = None
 
         self.__lock = asyncio.Lock()
         self.__post_bucket: dict[
             str,  # option hash
             Optional[tuple[
@@ -113,14 +117,15 @@
                                  tags: Optional[list[str]] = None,
                                  send_mode: int = 0,
                                  length_limit: int = 0,
                                  link_preview: int = 0,
                                  display_author: int = 0,
                                  display_via: int = 0,
                                  display_title: int = 0,
+                                 display_entry_tags: int = -1,
                                  style: int = 0,
                                  display_media: int = 0) -> Optional[tuple[str, bool, bool]]:
         """
         Get formatted post.
 
         :param sub_title: Sub title, overriding feed title if set
         :param tags: Tags of the sub
@@ -128,33 +133,35 @@
         :param length_limit: Telegraph length limit, valid when send_mode==0. If exceeded, send via Telegraph; If is 0,
             send via Telegraph when a post cannot be sent in a single message
         :param link_preview: 0=auto, 1=force enable
         :param display_author: -1=disable, 0=auto, 1=force display
         :param display_via: -3=disable but display link as post title, -2=completely disable,
             -1=disable but display link at the end, 0=feed title and link, 1=feed title and link as post title
         :param display_title: -1=disable, 0=auto, 1=force display
+        :param display_entry_tags: -1=disable, 1=force display
         :param style: 0=RSStT, 1=flowerss
         :param display_media: -1=disable, 0=enable
         :return: (formatted post, need media, need linkpreview)
         """
         assert send_mode in {FORCE_LINK, AUTO, FORCE_TELEGRAPH, FORCE_MESSAGE}
         assert isinstance(length_limit, int) and length_limit >= 0
         assert link_preview in {DISABLE, AUTO, FORCE_ENABLE}
         assert display_author in {DISABLE, AUTO, FORCE_DISPLAY}
         assert display_via in {NO_FEED_TITLE_BUT_LINK_AS_POST_TITLE, COMPLETELY_DISABLE, NO_FEED_TITLE_BUT_TEXT_LINK,
                                NO_FEED_TITLE_BUT_BARE_LINK, FEED_TITLE_AND_LINK, FEED_TITLE_AND_LINK_AS_POST_TITLE}
         assert display_title in {DISABLE, AUTO, FORCE_DISPLAY}
+        assert display_entry_tags in {DISABLE, FORCE_DISPLAY}
         assert display_media in {DISABLE, AUTO, ONLY_MEDIA_NO_CONTENT}
         assert style in {RSSTT, FLOWERSS}
 
         sub_title = (sub_title or self.feed_title)
         tags = tags or []
 
         param_hash = f'{sub_title}|{tags}|{send_mode}|{length_limit}|{link_preview}|' \
-                     f'{display_author}|{display_via}|{display_title}|{display_media}|{style}'
+                     f'{display_author}|{display_via}|{display_title}|{display_entry_tags}|{display_media}|{style}'
 
         if param_hash in self.__param_to_option_cache:
             option_hash = self.__param_to_option_cache[param_hash]
             if option_hash in self.__post_bucket:
                 return self.__post_bucket[option_hash]
 
         # ---- generate parsed_html if needed ----
@@ -211,14 +218,21 @@
                         and (
                                 not (self.author and sub_title and self.author in sub_title)
                                 or via_type not in (FEED_TITLE_VIA_NO_LINK and FEED_TITLE_VIA_W_LINK)
                         )
                 )
         )
 
+        # ---- determine tags ----
+        if display_entry_tags == FORCE_DISPLAY:
+            if self.tags_escaped is None:
+                self.tags_escaped = list(utils.escape_hashtags(self.tags))
+            if self.tags_escaped:
+                tags = utils.merge_tags(tags, self.tags_escaped) if tags else self.tags_escaped
+
         # ---- determine message_style ----
         if style == FLOWERSS:
             message_style = FLOWERSS_STYLE
         else:  # RSSTT
             message_style = NORMAL_STYLE
 
         # ---- determine message_type ----
@@ -338,15 +352,15 @@
                                                 message_type=message_type,
                                                 message_style=message_style)
             self.__post_bucket[option_hash] = post, need_media, need_link_preview
             return post, need_media, need_link_preview
 
     def get_post_header_and_footer(self,
                                    sub_title: Optional[str],
-                                   tags: list,
+                                   tags: list[str],
                                    title_type: TypePostTitleType,
                                    via_type: TypeViaType,
                                    need_author: bool,
                                    message_type: TypeMessageType,
                                    message_style: TypeMessageStyle) -> tuple[str, str]:
         # RSStT style:
         # {title}
@@ -391,15 +405,15 @@
         #   LINK_MESSAGE || NO_VIA: (* nothing)
         #   NORMAL_MESSAGE: source (* text link)
 
         feed_title = sub_title or self.feed_title
         title = self.title or 'Untitled'
 
         # ---- hashtags ----
-        tags_html = Text(' '.join('#' + tag for tag in tags)).get_html() if tags else None
+        tags_html = Text('#' + ' #'.join(tags)).get_html() if tags else None
 
         # ---- author ----
         author_html = Text(f'(author: {self.author})').get_html() if need_author and self.author else None
 
         if message_style == NORMAL_STYLE:
             # ---- title ----
             if message_type == TELEGRAPH_MESSAGE:
@@ -482,15 +496,15 @@
             )
 
             return header, footer
         raise ValueError(f'Unknown message style: {message_style}')
 
     def generate_formatted_post(self,
                                 sub_title: Optional[str],
-                                tags: list,
+                                tags: list[str],
                                 title_type: TypePostTitleType,
                                 via_type: TypeViaType,
                                 need_author: bool,
                                 message_type: TypeMessageType,
                                 message_style: TypeMessageStyle) -> str:
         header, footer = self.get_post_header_and_footer(sub_title=sub_title,
                                                          tags=tags,
```

### Comparing `rsstt-2.6.0/src/parsing/splitter.py` & `rsstt-2.7.0/src/parsing/splitter.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/parsing/table_drawer.py` & `rsstt-2.7.0/src/parsing/table_drawer.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/parsing/tgraph.py` & `rsstt-2.7.0/src/parsing/tgraph.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/parsing/utils.py` & `rsstt-2.7.0/src/parsing/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
-from typing import Optional, Sequence, Union
+from typing import Optional, Sequence, Union, Final, Iterable
 
 import re
 import json
+import string
 from contextlib import suppress
 from bs4.element import Tag
 from html import unescape
 from emoji import emojize
 from telethon.tl.types import TypeMessageEntity
 from functools import partial
 from urllib.parse import urljoin
 from os import path
+from itertools import chain
 
 from .. import log
 from ..aio_helper import run_async
 from ..compat import parsing_utils_html_validator_minify
 
 logger = log.getLogger('RSStT.parsing')
 
 # noinspection SpellCheckingInspection
-SPACES = (
+SPACES: Final[str] = (
     # all characters here, except for \u200c, \u200d and \u2060, are converted to space on TDesktop, but Telegram
     # Android preserves all
     ' '  # '\x20', SPACE
     '\xa0'  # NO-BREAK SPACE
     '\u2002'  # EN SPACE
     '\u2003'  # EM SPACE
     '\u2004'  # THREE-PER-EM SPACE
@@ -37,15 +39,15 @@
     # '\u200c'  # ZERO WIDTH NON-JOINER, ZWNJ, important for emoji or some languages
     # '\u200d'  # ZERO WIDTH JOINER, ZWJ, important for emoji or some languages
     '\u202f'  # NARROW NO-BREAK SPACE
     '\u205f'  # MEDIUM MATHEMATICAL SPACE, MMSP
     # '\u2060'  # WORD JOINER
     '\u3000'  # IDEOGRAPHIC SPACE
 )
-INVALID_CHARACTERS = (
+INVALID_CHARACTERS: Final[str] = (
     # all characters here are converted to space server-side
     '\x00'  # NULL
     '\x01'  # START OF HEADING
     '\x02'  # START OF TEXT
     '\x03'  # END OF TEXT
     '\x04'  # END OF TRANSMISSION
     '\x05'  # ENQUIRY
@@ -72,25 +74,30 @@
     '\x1c'  # FILE SEPARATOR
     '\x1d'  # GROUP SEPARATOR
     '\x1e'  # RECORD SEPARATOR
     '\x1f'  # UNIT SEPARATOR
     '\u2028'  # LINE SEPARATOR
     '\u2029'  # PARAGRAPH SEPARATOR
 )
+CHARACTERS_TO_ESCAPE_IN_HASHTAG: Final[str] = ''.join(
+    # all characters here will be replaced with '_'
+    sorted(set(SPACES + INVALID_CHARACTERS + string.punctuation + string.whitespace))
+)
 
 # load emoji dict
 with open(path.join(path.dirname(__file__), 'emojify.json'), 'r', encoding='utf-8') as emojify_json:
     EMOJI_DICT = json.load(emojify_json)
 
 replaceInvalidCharacter = partial(re.compile(rf'[{INVALID_CHARACTERS}]').sub, ' ')  # use initially
 replaceSpecialSpace = partial(re.compile(rf'[{SPACES[1:]}]').sub, ' ')  # use carefully
 stripBr = partial(re.compile(r'\s*<br\s*/?\s*>\s*').sub, '<br>')
 stripLineEnd = partial(re.compile(rf'[{SPACES}]+\n').sub, '\n')  # use firstly
 stripNewline = partial(re.compile(r'\n{3,}').sub, '\n\n')  # use secondly
 stripAnySpace = partial(re.compile(r'\s+').sub, ' ')
+escapeHashtag = partial(re.compile(rf'[{CHARACTERS_TO_ESCAPE_IN_HASHTAG}]+').sub, '_')
 isAbsoluteHttpLink = re.compile(r'^https?://').match
 isSmallIcon = re.compile(r'(width|height): ?(([012]?\d|30)(\.\d)?px|([01](\.\d)?|2)r?em)').search
 
 
 class Enclosure:
     def __init__(self, url: str, length: Union[int, str], _type: str, duration: str = None, thumbnail: str = None):
         self.url = url
@@ -152,14 +159,15 @@
 
 
 async def parse_entry(entry, feed_link: Optional[str] = None):
     class EntryParsed:
         content: str = ''
         link: Optional[str] = None
         author: Optional[str] = None
+        tags: Optional[list[str]] = None
         title: Optional[str] = None
         enclosures: list[Enclosure] = None
 
     # entry.summary returns summary(Atom) or description(RSS)
     content = entry.get('content') or entry.get('summary', '')
 
     if isinstance(content, list):  # Atom
@@ -180,14 +188,16 @@
     author = entry['author'] if ('author' in entry and type(entry['author']) is str) else None
     author = html_space_stripper(author) if author else None
     EntryParsed.author = author or None  # reject empty string
     # hmm, some entries do have no title, should we really set up a feed hospital?
     title = entry.get('title')
     title = html_space_stripper(title, enable_emojify=True) if title else None
     EntryParsed.title = title or None  # reject empty string
+    if (tags := entry.get('tags')) and isinstance(tags, list):
+        EntryParsed.tags = list(filter(None, (tag.get('term') for tag in tags)))
 
     enclosures = []
 
     if isinstance(entry.get('links'), list):
         for link in (link for link in entry['links'] if link.get('rel') == 'enclosure' and link.get('href')):
             enclosures.append(Enclosure(url=resolve_relative_link(feed_link, link['href']),
                                         length=link.get('length'),
@@ -257,15 +267,15 @@
 
 
 def copy_entities(entities: Sequence[TypeMessageEntity]) -> list[TypeMessageEntity]:
     return [copy_entity(entity) for entity in entities]
 
 
 def compare_entity(a: TypeMessageEntity, b: TypeMessageEntity, ignore_position: bool = False) -> bool:
-    if type(a) != type(b):
+    if type(a) is type(b):
         return False
 
     a_dict = a.to_dict()
     b_dict = b.to_dict()
     if ignore_position:
         for d in (a_dict, b_dict):
             for key in ('offset', 'length'):
@@ -295,7 +305,19 @@
             new_start_pos = min(start_pos, contiguous_entity.offset)
             new_end_pos = max(end_pos, contiguous_entity.offset + contiguous_entity.length)
             entity = copy_entity(entity)
             entity.offset = new_start_pos
             entity.length = new_end_pos - new_start_pos
         merged_entities.append(entity)
     return merged_entities
+
+
+def escape_hashtag(tag: str) -> str:
+    return escapeHashtag(tag).strip('_')
+
+
+def escape_hashtags(tags: Optional[Iterable[str]]) -> Iterable[str]:
+    return filter(None, map(escape_hashtag, tags)) if tags else ()
+
+
+def merge_tags(*tag_lists: Optional[Iterable[str]]) -> list[str]:
+    return list(dict.fromkeys(chain(*tag_lists)))
```

### Comparing `rsstt-2.6.0/src/redirect_server.py` & `rsstt-2.7.0/src/redirect_server.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/web/feed.py` & `rsstt-2.7.0/src/web/feed.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from ssl import SSLError
 from functools import partial
 
 from .. import log
 from ..aio_helper import run_async
 from ..compat import bozo_exception_removal_wrapper
 from .req import get
-from .utils import WebFeed, WebError, sentinel
+from .utils import WebResponse, WebFeed, WebError, sentinel
 
 FEED_ACCEPT: Final = 'application/rss+xml, application/rdf+xml, application/atom+xml, ' \
                      'application/xml;q=0.9, text/xml;q=0.8, text/*;q=0.7, application/*;q=0.6'
 
 
 async def feed_get(url: str, timeout: Optional[float] = sentinel, web_semaphore: Union[bool, asyncio.Semaphore] = None,
                    headers: Optional[dict] = None, verbose: bool = True) -> WebFeed:
@@ -27,20 +27,21 @@
     _headers = {}
     if headers:
         _headers.update(headers)
     if 'Accept' not in _headers:
         _headers['Accept'] = FEED_ACCEPT
 
     try:
-        resp = await get(url, timeout, web_semaphore, decode=False, headers=_headers)
+        resp: WebResponse = await get(url, timeout, web_semaphore, decode=False, headers=_headers)
         rss_content = resp.content
         ret.content = rss_content
         ret.url = resp.url
         ret.headers = resp.headers
         ret.status = resp.status
+        ret.web_response = resp
 
         # some rss feed implement http caching improperly :(
         if resp.status == 200 and int(resp.headers.get('Content-Length', '1')) == 0:
             ret.status = 304
             # ret.msg = f'"Content-Length" is 0'
             return ret
```

### Comparing `rsstt-2.6.0/src/web/media.py` & `rsstt-2.7.0/src/web/media.py`

 * *Files identical despite different names*

### Comparing `rsstt-2.6.0/src/web/req.py` & `rsstt-2.7.0/src/web/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,14 @@
     _headers = HEADER_TEMPLATE.copy()
     if headers:
         _headers.update(headers)
 
     async def _fetch():
         async with aiohttp.ClientSession(
                 connector=proxy_connector,
-                timeout=aiohttp.ClientTimeout(total=timeout),
                 headers=_headers,
                 cookie_jar=YummyCookieJar()
         ) as session:
             async with session.request(
                     method,
                     url,
                     read_bufsize=read_bufsize,
@@ -200,15 +199,15 @@
             if (PROXY and proxy_filter(host, parse=False))
             else aiohttp.TCPConnector(family=socket_family, ssl=ssl_context)
         )
 
         try:
             async with semaphore_to_use:
                 async with locks.overall_web_semaphore:
-                    ret = await asyncio.wait_for(_fetch(), timeout and timeout + 0.1)
+                    ret = await asyncio.wait_for(_fetch(), timeout)
                     if socket_family == AF_INET6 and tries < max_tries \
                             and ret.status in STATUSES_SHOULD_RETRY_IN_IPV4:
                         raise RetryInIpv4(ret.status, ret.reason)
                     return ret
         except EXCEPTIONS_SHOULD_RETRY as e:
             if isinstance(e, RetryInIpv4):
                 retry_in_v4_flag = True
```


# Comparing `tmp/honcho_ai-0.0.7.tar.gz` & `tmp/honcho_ai-0.0.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "honcho_ai-0.0.7.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `honcho_ai-0.0.7.tar` & `honcho_ai-0.0.8a1.tar`

### file list

```diff
@@ -1,11 +1,85 @@
--rw-r--r--   0        0        0    34523 2024-02-29 09:17:36.878653 honcho_ai-0.0.7/LICENSE
--rw-r--r--   0        0        0     1357 2024-03-17 02:40:12.855561 honcho_ai-0.0.7/README.md
--rw-r--r--   0        0        0      549 2024-03-21 19:23:06.566512 honcho_ai-0.0.7/honcho/__init__.py
--rw-r--r--   0        0        0     1281 2024-03-21 19:23:06.566846 honcho_ai-0.0.7/honcho/cache.py
--rw-r--r--   0        0        0    50750 2024-04-01 17:58:55.192634 honcho_ai-0.0.7/honcho/client.py
--rw-r--r--   0        0        0       52 2024-03-21 19:23:06.568417 honcho_ai-0.0.7/honcho/ext/__init__.py
--rw-r--r--   0        0        0     2304 2024-04-01 17:58:55.192828 honcho_ai-0.0.7/honcho/ext/langchain.py
--rw-r--r--   0        0        0     2190 2024-04-01 05:16:27.970972 honcho_ai-0.0.7/honcho/schemas.py
--rw-r--r--   0        0        0    49718 2024-04-01 17:58:55.193225 honcho_ai-0.0.7/honcho/sync_client.py
--rw-r--r--   0        0        0      985 2024-04-01 17:58:55.194216 honcho_ai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1954 1970-01-01 00:00:00.000000 honcho_ai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/__init__.py
+-rw-r--r--   0        0        0    64415 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_base_client.py
+-rw-r--r--   0        0        0    17622 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_resource.py
+-rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_response.py
+-rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_version.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/lib/.keep
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/__init__.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/__init__.py
+-rw-r--r--   0        0        0    19418 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/apps.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/__init__.py
+-rw-r--r--   0        0        0    28295 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/users.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/collections/__init__.py
+-rw-r--r--   0        0        0    32165 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/collections/collections.py
+-rw-r--r--   0        0        0    23953 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/collections/documents.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/__init__.py
+-rw-r--r--   0        0        0    21471 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/messages.py
+-rw-r--r--   0        0        0    24422 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/metamessages.py
+-rw-r--r--   0        0        0    36225 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/resources/apps/users/sessions/sessions.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/app.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/app_create_params.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/app_update_params.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/page_user.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/user.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/user_create_params.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/user_list_params.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/user_update_params.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/agent_chat.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_create_params.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_list_params.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_query_params.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_query_response.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collection_update_params.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/page_collection.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/page_session.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_chat_params.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_create_params.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_list_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_stream_params.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/session_update_params.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/document.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/document_create_params.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/document_list_params.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/document_update_params.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/collections/page_document.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/__init__.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/message.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/message_create_params.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/message_list_params.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/message_update_params.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage_create_params.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage_get_params.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage_list_params.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/metamessage_update_params.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/page_message.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/src/honcho/types/apps/users/sessions/page_metamessage.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/LICENSE
+-rw-r--r--   0        0        0     4419 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/pyproject.toml
+-rw-r--r--   0        0        0    13524 2020-02-02 00:00:00.000000 honcho_ai-0.0.8a1/PKG-INFO
```


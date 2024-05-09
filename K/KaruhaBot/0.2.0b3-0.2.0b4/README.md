# Comparing `tmp/KaruhaBot-0.2.0b3.tar.gz` & `tmp/karuhabot-0.2.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KaruhaBot-0.2.0b3.tar", last modified: Tue Apr  2 12:10:42 2024, max compression
+gzip compressed data, was "karuhabot-0.2.0b4.tar", last modified: Thu May  9 15:31:26 2024, max compression
```

## Comparing `KaruhaBot-0.2.0b3.tar` & `karuhabot-0.2.0b4.tar`

### file list

```diff
@@ -1,70 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.962828 KaruhaBot-0.2.0b3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.958828 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 12:10:42.000000 KaruhaBot-0.2.0b3/KaruhaBot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-04-02 12:10:42.958828 KaruhaBot-0.2.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.950827 KaruhaBot-0.2.0b3/karuha/
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29966 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.950827 KaruhaBot-0.2.0b3/karuha/command/
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/decoractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12054 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/command/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.954828 KaruhaBot-0.2.0b3/karuha/data/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/data/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.954828 KaruhaBot-0.2.0b3/karuha/event/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31583 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/event/sys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/plugin_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.954828 KaruhaBot-0.2.0b3/karuha/text/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/drafty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    16074 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/text/textchain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.958828 KaruhaBot-0.2.0b3/karuha/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/event_catcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/utils/proxy_propery.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/karuha/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:10:42.962828 KaruhaBot-0.2.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:42.958828 KaruhaBot-0.2.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_command_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2024-04-02 12:10:37.000000 KaruhaBot-0.2.0b3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:26.924236 karuhabot-0.2.0b4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:26.924236 karuhabot-0.2.0b4/KaruhaBot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-09 15:31:26.000000 karuhabot-0.2.0b4/KaruhaBot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-09 15:31:26.000000 karuhabot-0.2.0b4/KaruhaBot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:31:26.000000 karuhabot-0.2.0b4/KaruhaBot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 15:31:26.000000 karuhabot-0.2.0b4/KaruhaBot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 15:31:26.000000 karuhabot-0.2.0b4/KaruhaBot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-09 15:31:26.924236 karuhabot-0.2.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:26.916236 karuhabot-0.2.0b4/karuha/
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29966 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:26.916236 karuhabot-0.2.0b4/karuha/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/command/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/command/decoractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/command/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/command/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:26.920236 karuhabot-0.2.0b4/karuha/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/data/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/data/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/data/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/data/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/data/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:26.920236 karuhabot-0.2.0b4/karuha/event/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/event/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32306 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/event/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/event/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/event/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/event/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/event/sys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/plugin_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22949 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:26.920236 karuhabot-0.2.0b4/karuha/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/text/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/text/drafty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/text/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/text/textchain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:26.920236 karuhabot-0.2.0b4/karuha/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/utils/decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/utils/event_catcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/utils/invoker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/utils/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/utils/proxy_propery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/karuha/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:31:26.924236 karuhabot-0.2.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:26.924236 karuhabot-0.2.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/test_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/test_command_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11497 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8882 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-05-09 15:31:21.000000 karuhabot-0.2.0b4/tests/utils.py
```

### Comparing `KaruhaBot-0.2.0b3/KaruhaBot.egg-info/PKG-INFO` & `karuhabot-0.2.0b4/KaruhaBot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaruhaBot
-Version: 0.2.0b3
+Version: 0.2.0b4
 Summary: A simple Tinode chatbot framework.
 Home-page: https://github.com/Visecy/Karuha
 Author: Visecy
 Author-email: Visecy@visecy.org
 Maintainer: Ovizro
 Maintainer-email: Ovizro@visecy.org
 License: Apache 2.0
@@ -178,15 +178,16 @@
 
 ## About More
 Of course, Karuha provides more APIs than just these. If you are interested in learning more, please refer to the source code of the library.
 
 ### Development Goals
 Features that may be added in the future include:
 
-- [ ] APIs related to user information getting and setting
+- [x] APIs related to user information getting and setting
+- [ ] Match rule for command
 - [ ] Automatic argument parsing in argparse format for commands
 
 ### Module Development
 Currently, Karuha's support for module development is relatively simple. There are no dedicated APIs for defining chatbot modules, but predefined commands can still be supported.
 
 The way to define commands in external modules is similar to the normal definition. But to avoid affecting the user's related command settings, we need to create a new CommandCollection. The method to establish a command collection and define commands in it is as follows:
```

### Comparing `KaruhaBot-0.2.0b3/LICENSE` & `karuhabot-0.2.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/PKG-INFO` & `karuhabot-0.2.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KaruhaBot
-Version: 0.2.0b3
+Version: 0.2.0b4
 Summary: A simple Tinode chatbot framework.
 Home-page: https://github.com/Visecy/Karuha
 Author: Visecy
 Author-email: Visecy@visecy.org
 Maintainer: Ovizro
 Maintainer-email: Ovizro@visecy.org
 License: Apache 2.0
@@ -178,15 +178,16 @@
 
 ## About More
 Of course, Karuha provides more APIs than just these. If you are interested in learning more, please refer to the source code of the library.
 
 ### Development Goals
 Features that may be added in the future include:
 
-- [ ] APIs related to user information getting and setting
+- [x] APIs related to user information getting and setting
+- [ ] Match rule for command
 - [ ] Automatic argument parsing in argparse format for commands
 
 ### Module Development
 Currently, Karuha's support for module development is relatively simple. There are no dedicated APIs for defining chatbot modules, but predefined commands can still be supported.
 
 The way to define commands in external modules is similar to the normal definition. But to avoid affecting the user's related command settings, we need to create a new CommandCollection. The method to establish a command collection and define commands in it is as follows:
```

### Comparing `KaruhaBot-0.2.0b3/README.md` & `karuhabot-0.2.0b4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,16 @@
 
 ## About More
 Of course, Karuha provides more APIs than just these. If you are interested in learning more, please refer to the source code of the library.
 
 ### Development Goals
 Features that may be added in the future include:
 
-- [ ] APIs related to user information getting and setting
+- [x] APIs related to user information getting and setting
+- [ ] Match rule for command
 - [ ] Automatic argument parsing in argparse format for commands
 
 ### Module Development
 Currently, Karuha's support for module development is relatively simple. There are no dedicated APIs for defining chatbot modules, but predefined commands can still be supported.
 
 The way to define commands in external modules is similar to the normal definition. But to avoid affecting the user's related command settings, we need to create a new CommandCollection. The method to establish a command collection and define commands in it is as follows:
```

### Comparing `KaruhaBot-0.2.0b3/karuha/__init__.py` & `karuhabot-0.2.0b4/karuha/runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,17 @@
 """
 A simple Tinode chatbot framework
 """
 
 import asyncio
-import os
-from pathlib import Path
 from typing import Dict, List
 
-
-WORKDIR = Path(os.environ.get("KARUHA_HOME", ".bot"))  # dir to storage bot data
-
-
-from .version import __version__
-from .config import get_config, load_config, init_config, save_config, Config
-from .config import Server as ServerConfig, Bot as BotConfig
+from .config import get_config
 from .bot import Bot
-from .event import on, on_event, Event
 from .event.sys import SystemStartEvent, SystemStopEvent
-from .exception import KaruhaException
-from .command import CommandCollection, AbstractCommand, AbstractCommandParser, BaseSession, MessageSession, CommandSession, get_collection, on_command
-from .text import Drafty, BaseText, PlainText, Message, TextChain
 from .logger import logger
 
 
 _bot_cache: Dict[str, Bot] = {}
 _loop = None
 
 
@@ -102,48 +90,7 @@
     try:
         asyncio.run(async_run())
     except (KeyboardInterrupt, asyncio.CancelledError):  # pragma: no cover
         pass
 
 
 from .plugin_server import init_server
-
-
-__all__ = [
-    # bot
-    "add_bot",
-    "try_add_bot",
-    "get_bot",
-    "async_run",
-    "run",
-    "Bot",
-    # config
-    "get_config",
-    "init_config",
-    "load_config",
-    "save_config",
-    "Config",
-    "BotConfig",
-    "ServerConfig",
-    # event
-    "Event",
-    # text
-    "Drafty",
-    "BaseText",
-    "PlainText",
-    "Message",
-    "TextChain",
-    # command
-    "CommandCollection",
-    "AbstractCommand",
-    "AbstractCommandParser",
-    "get_collection",
-    "BaseSession",
-    "MessageSession",
-    "CommandSession",
-    # decorator
-    "on",
-    "on_event",
-    "on_command",
-    # exception
-    "KaruhaException"
-]
```

### Comparing `KaruhaBot-0.2.0b3/karuha/__main__.py` & `karuhabot-0.2.0b4/karuha/__main__.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/bot.py` & `karuhabot-0.2.0b4/karuha/bot.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/command/__init__.py` & `karuhabot-0.2.0b4/karuha/command/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,49 @@
+from .rule import *  # noqa: F403
+from .session import BaseSession, MessageSession, CommandSession
 from .command import AbstractCommand, FunctionCommand, ParamFunctionCommand
 from .collection import (CommandCollection, add_sub_collection, get_collection,
                          new_collection, remove_sub_collection, reset_collection,
                          set_collection, set_collection_factory, set_prefix)
-from .decoractor import on_command
-from .parser import (AbstractCommandParser, ParamParser, ParamParserFlag,
-                     SimpleCommandParser)
-from .session import BaseSession, MessageSession, CommandSession
+from .decoractor import on_command, on_rule
+from .parser import AbstractCommandParser, SimpleCommandParser
 
 from ..event.command import (BaseCommandEvent, CommandCompleteEvent, CommandEvent,
                     CommandFailEvent, CommandNotFoundEvent,
                     CommandPrepareEvent)
 
 
 __all__ = [
     # command
     "AbstractCommand",
     "FunctionCommand",
     "ParamFunctionCommand",
     # parser
     "AbstractCommandParser",
     "SimpleCommandParser",
-    "ParamParser",
-    "ParamParserFlag",
     # session
     "BaseSession",
     "MessageSession",
+    "CommandSession",
+    # rule
+    "BaseRule",
+    "KeywordRule",
+    "MentionMeRule",
+    "MentionRule",
+    "NotRule",
+    "OrRule",
+    "RegexRule",
+    "SeqIDRule",
+    "TopicRule",
+    "UserIDRule",
+    "AndRule",
+    "QuoteRule",
+    "ToMeRule",
+    "NoopRule",
+    "rule",
     # collection
     "CommandCollection",
     "get_collection",
     "new_collection",
     "add_sub_collection",
     "remove_sub_collection",
     "reset_collection",
@@ -40,8 +55,9 @@
     "CommandEvent",
     "CommandFailEvent",
     "CommandNotFoundEvent",
     "CommandPrepareEvent",
     "CommandCompleteEvent",
     # decorator
     "on_command",
+    "on_rule",
 ]
```

### Comparing `KaruhaBot-0.2.0b3/karuha/command/collection.py` & `karuhabot-0.2.0b4/karuha/command/collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,103 +1,98 @@
 import asyncio
 import sys
-from typing import Any, Callable, Dict, Iterable, List, Optional, Set, TypeVar, Union, overload
+from typing import Any, Callable, Dict, Generator, Iterable, List, Optional, Set, TypeVar, Union, overload
 from typing_extensions import ParamSpec
 
-from ..utils.dispatcher import _ContextHelper
+from ..utils.context import _ContextHelper
 from ..logger import logger
 from ..text.message import Message
-from ..event.message import MessageDispatcher
 from ..exception import KaruhaCommandError, KaruhaException
-from .parser import AbstractCommandParser, ParamParserFlag, SimpleCommandParser
-from .command import AbstractCommand, ParamFunctionCommand, FunctionCommand, CommandMessage
+from .parser import AbstractCommandParser, SimpleCommandParser
+from .rule import BaseRule, MessageRuleDispatcher, NoopRule
+from .command import AbstractCommand, FunctionCommand
+from .session import CommandMessage
 
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
 class CommandCollection(_ContextHelper):
-    __slots__ = ["commands", "name_parser", "sub_collections", "_dispatcher"]
+    __slots__ = ["commands", "name_parser", "sub_collections", "_dispatcher", "rule"]
 
     commands: Dict[str, AbstractCommand]
     sub_collections: List["CommandCollection"]
 
-    def __init__(self, /, name_parser: AbstractCommandParser) -> None:
+    def __init__(self, /, name_parser: AbstractCommandParser, *, rule: Optional[BaseRule] = None) -> None:
         self.commands = {}
         self.name_parser = name_parser
         self.sub_collections = []
         self._dispatcher = None
+        self.rule = rule
     
     def add_command(self, command: AbstractCommand, /) -> None:
         self._check_name(command.__name__)
         self.commands[command.__name__] = command
         for alias in command.alias:
             self._check_name(alias)
             self.commands[alias] = command
     
     def get_command(self, name: str, default: Optional[AbstractCommand] = None, /) -> Optional[AbstractCommand]:
-        command = self.commands.get(name)
-        if command is not None:
-            return command
-        for i in self.sub_collections:
-            command = i.get_command(name)
-            if command is not None:
-                return command
+        for c in self._get_commands(name):
+            return c
         return default
         
     @overload
     def on_command(
         self,
         name: Optional[str] = ...,
         /, *,
         alias: Optional[Iterable[str]] = ...,
-        flags: ParamParserFlag = ...
+        rule: Optional[BaseRule] = ...,
     ) -> Callable[[Callable[P, R]], FunctionCommand[P, R]]: ...
 
     @overload
     def on_command(
         self,
         func: Callable[P, R],
         /, *,
         alias: Optional[Iterable[str]] = ...,
-        flags: ParamParserFlag = ...
+        rule: Optional[BaseRule] = ...,
     ) -> FunctionCommand[P, R]: ...
 
     def on_command(
             self,
             func_or_name: Union[str, Callable[P, R], None] = None,
-            /, *,
-            flags: ParamParserFlag = ParamParserFlag.FULL,
+            /,
             **kwds: Any
     ) -> Union[Callable[[Callable[P, R]], FunctionCommand[P, R]], FunctionCommand[P, R]]:
         def inner(func: Callable[P, R]) -> FunctionCommand[P, R]:
             if isinstance(func_or_name, str):
                 name = func_or_name
             else:
                 name = func.__name__
-            if flags == ParamParserFlag.NONE:
-                cmd = FunctionCommand.from_function(func, name=name, **kwds)
-            else:
-                cmd = ParamFunctionCommand.from_function(func, name=name, flags=flags, **kwds)
+            cmd = FunctionCommand.from_function(func, name=name, **kwds)
             self.add_command(cmd)
             return cmd
     
         if isinstance(func_or_name, str) or func_or_name is None:
             return inner
         return inner(func_or_name)
     
     async def run(self, message: Message) -> None:
         result = self.name_parser.parse(message)
         if result is None:
             return
         
         name, argv = result
-        command = self.get_command(name)
-        if command is None:
+        for command in self._get_commands(name):
+            if command.rule is None or command.rule.match(message):
+                break
+        else:
             CommandNotFoundEvent.new(self, name)
             logger.error(f"command {name} not found")
             return
         
         try:
             await command.call_command(CommandMessage.from_message(message, command, self, name, argv))
         except KaruhaException:
@@ -119,56 +114,61 @@
         self._dispatcher.deactivate()
         self._dispatcher = None
     
     def __getitem__(self, name: str, /) -> AbstractCommand:
         command = self.get_command(name)
         if command is not None:
             return command
-        # CommandNotFoundEvent.new(self, name)
         raise KaruhaCommandError(f"command {name} is not registered", name=name, collection=self)
     
     @property
     def activated(self) -> bool:
         return self._dispatcher is not None
     
+    def _get_commands(self, name: str, /) -> Generator[AbstractCommand, None, None]:
+        if name in self.commands:
+            yield self.commands[name]
+        for i in self.sub_collections:
+            yield from i._get_commands(name)
+    
     def _check_name(self, name: str) -> None:
         if name in self.commands:
             raise ValueError(f"command {name} is already registered")
         if not self.name_parser.check_name(name):
             raise ValueError(f"command {name} is not valid")
     
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} with {len(self.commands)} commands at 0x{id(self):016x}>"
 
 
-class CommandDispatcher(MessageDispatcher):
+class CommandDispatcher(MessageRuleDispatcher):
     __slots__ = ["collection"]
 
     def __init__(self, collection: CommandCollection, *, once: bool = False) -> None:
-        super().__init__(once=once)
+        super().__init__(collection.rule or NoopRule(), 0.8, once=once)
         self.collection = collection
     
     def match(self, message: Message, /) -> float:
         if self.collection.name_parser.precheck(message):
-            return 0.8
+            return super().match(message)
         return 0
     
     def run(self, message: Message) -> asyncio.Task:
         return asyncio.create_task(self.collection.run(message))
 
 
 _default_prefix = ('/',)
 _default_collection: Optional[CommandCollection] = None
 _sub_collections: Set[CommandCollection] = set()
 
 
-def get_collection() -> CommandCollection:
+def get_collection(*args: Any, **kwds: Any) -> CommandCollection:
     global _default_collection
     if _default_collection is None:
-        _default_collection = new_collection()
+        _default_collection = new_collection(*args, **kwds)
         _default_collection.activate()
         _default_collection.sub_collections.extend(_sub_collections)
     return _default_collection
 
 
 def set_collection(collection: CommandCollection) -> None:
     global _default_collection
@@ -190,17 +190,18 @@
     global _default_collection
     if _default_collection is None:
         return
     _default_collection.deactivate()
     _default_collection = None
 
 
-def new_collection() -> CommandCollection:
+def new_collection(*, rule: Optional[BaseRule] = None) -> CommandCollection:
     return CommandCollection(
-        SimpleCommandParser(_default_prefix)
+        SimpleCommandParser(_default_prefix),
+        rule=rule
     )
 
 
 __collection_factory_backup = new_collection
 
 
 def set_prefix(*prefix: str) -> None:
@@ -208,15 +209,15 @@
     if _default_collection is not None or new_collection is not __collection_factory_backup:
         raise RuntimeError("cannot set prefix after collection is created")
     elif not prefix:  # pragma: no cover
         raise ValueError("prefix must be at least one")
     _default_prefix = prefix
 
 
-def set_collection_factory(factory: Optional[Callable[[], CommandCollection]], reset: bool = False) -> None:
+def set_collection_factory(factory: Optional[Callable[..., CommandCollection]], reset: bool = False) -> None:
     global new_collection
     if _default_collection is not None:
         if reset:
             reset_collection()
         else:
             raise RuntimeError("cannot set default collection factory after collection is created")
     new_collection = factory or __collection_factory_backup
```

### Comparing `KaruhaBot-0.2.0b3/karuha/command/command.py` & `karuhabot-0.2.0b4/karuha/command/command.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,31 @@
 import asyncio
 import sys
 from abc import ABC, abstractmethod
 from inspect import signature
-from typing import Any, Callable, Generic, Iterable, Optional, Tuple, TypeVar, Union
+from typing import Any, Callable, Generic, Iterable, Optional, Tuple, TypeVar
 from venv import logger
 
 from typing_extensions import ParamSpec, Self
 
-from ..text.textchain import BaseText
 from ..event.message import Message
 from ..exception import KaruhaCommandCanceledError, KaruhaCommandError
+from .rule import BaseRule
 
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
-class CommandMessage(Message, frozen=True, arbitrary_types_allowed=True):
-    name: str
-    argv: Tuple[Union[str, BaseText], ...]
-    command: "AbstractCommand"
-    collection: "CommandCollection"
-
-    @classmethod
-    def from_message(
-            cls,
-            message: Message,
-            /,
-            command: "AbstractCommand",
-            collection: "CommandCollection",
-            name: str,
-            argv: Iterable[Union[str, BaseText]]
-    ) -> Self:
-        data = dict(message)
-        data["command"] = command
-        data["collection"] = collection
-        data["name"] = name
-        data["argv"] = tuple(argv)
-        return cls(**data)
-
-
-from .parser import ParamParser, ParamParserFlag
-
-
 class AbstractCommand(ABC):
-    __slots__ = ["__name__", "alias"]
+    __slots__ = ["__name__", "alias", "rule"]
 
-    def __init__(self, name: str, /, alias: Optional[Iterable[str]] = None) -> None:
+    def __init__(self, name: str, /, alias: Optional[Iterable[str]] = None, *, rule: Optional[BaseRule] = None) -> None:
         self.__name__ = name
+        self.rule = rule
         if alias is None:
             self.alias = ()
         else:
             self.alias = tuple(alias)
     
     @property
     def name(self) -> str:
@@ -59,31 +33,42 @@
     
     @abstractmethod
     async def call_command(self, message: "CommandMessage") -> Any:
         pass
 
 
 class FunctionCommand(AbstractCommand, Generic[P, R]):
-    __slots__ = ["__func__"]
+    __slots__ = ["__func__", "__signature__"]
 
-    def __init__(self, name: str, func: Callable[P, R], /, alias: Optional[Iterable[str]] = None) -> None:
-        super().__init__(name, alias)
+    def __init__(
+        self,
+        name: str,
+        func: Callable[P, R],
+        /,
+        alias: Optional[Iterable[str]] = None,
+        *,
+        rule: Optional[BaseRule] = None,
+    ) -> None:
+        super().__init__(name, alias, rule=rule)
         self.__func__ = func
-    
+        self.__signature__ = signature(func)
+
     def parse_message(self, message: Message) -> Tuple[tuple, dict]:  # pragma: no cover
-        return (self, message), {}
-    
+        args, kwargs = message.extract_handler_params(self.__signature__)
+        return tuple(args), kwargs
+
     async def call_command(self, message: "CommandMessage") -> Any:
         logger.debug(f"preparing command {self.name}")
         prepare_event = CommandPrepareEvent(message.collection, self, message)
         try:
             await prepare_event.trigger()
         except KaruhaCommandCanceledError:
-            logger.info(f"command {self.name} canceled")
+            logger.info(f"command {self.name} canceled before run")
             raise
+        
         try:
             args, kwargs = self.parse_message(message)
             result = self.__func__(*args, **kwargs)  # type: ignore
             if asyncio.iscoroutine(result):
                 result = await result
         except KaruhaCommandCanceledError:
             logger.info(f"command {self.name} canceled")
@@ -92,48 +77,32 @@
             CommandFailEvent.new(message.collection, self, sys.exc_info())  # type: ignore
             logger.error(f"run command {self.name} failed", exc_info=True)
             raise KaruhaCommandError(f"run command {self.name} failed", name=self.name, command=self) from e
         else:
             logger.info(f"command {self.name} complete")
             CommandCompleteEvent.new(message.collection, self, result)
         return result
-    
+
     def __call__(self, *args: P.args, **kwds: P.kwargs) -> R:
         return self.__func__(*args, **kwds)
-    
-    @classmethod
-    def from_function(cls, /, func: Callable, *, name: Optional[str] = None, alias: Optional[Iterable[str]] = None) -> Self:
-        if name is None:  # pragma: no cover
-            name = func.__name__
-        return cls(name, func, alias=alias)
 
-
-class ParamFunctionCommand(FunctionCommand[P, R]):
-    __slots__ = ["parser"]
-
-    def __init__(self, name: str, func: Callable[P, R], parser: ParamParser, /, alias: Optional[Iterable[str]] = None) -> None:
-        super().__init__(name, func, alias)
-        self.parser = parser
-    
-    def parse_message(self, message: "CommandMessage") -> Tuple[tuple, dict]:
-        return self.parser.parse(message)
-    
     @classmethod
     def from_function(
-            cls,
-            /,
-            func: Callable[P, R],
-            *,
-            name: Optional[str] = None,
-            alias: Optional[Iterable[str]] = None,
-            flags: ParamParserFlag = ParamParserFlag.FULL
+        cls,
+        /,
+        func: Callable,
+        *,
+        name: Optional[str] = None,
+        alias: Optional[Iterable[str]] = None,
+        rule: Optional[BaseRule] = None,
     ) -> Self:
         if name is None:  # pragma: no cover
             name = func.__name__
-        sig = signature(func)
-        parser = ParamParser.from_signature(sig, flags=flags)
-        return cls(name, func, parser, alias=alias)
+        return cls(name, func, alias=alias, rule=rule)
+
+
+ParamFunctionCommand = FunctionCommand
 
 
 from ..event.command import (CommandCompleteEvent, CommandFailEvent,
                              CommandPrepareEvent)
-from .collection import CommandCollection
+from .session import CommandMessage
```

### Comparing `KaruhaBot-0.2.0b3/karuha/command/session.py` & `karuhabot-0.2.0b4/karuha/session.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 import asyncio
 import os
 import re
-from collections import deque
-from typing import Any, Deque, Dict, NoReturn, Optional, Tuple, Union
+from typing import Any, Dict, Optional, Union
 
-from ..bot import Bot
-from ..event.message import Message, MessageDispatcher, get_message_lock
-from ..exception import KaruhaRuntimeError, KaruhaCommandCanceledError
-from ..text import BaseText, Drafty
-from ..text.textchain import (Bold, Button, File, Form, Image, NewLine, PlainText,
-                              TextChain)
-from ..utils.dispatcher import FutureDispatcher
+from .bot import Bot
 
 
 class BaseSession(object):
     __slots__ = ["bot", "topic"]
 
     def __init__(self, /, bot: Bot, topic: str) -> None:
         self.bot = bot
         self.topic = topic
     
     async def send(
             self,
-            text: Union[str, dict, Drafty, BaseText],
+            text: Union[str, dict, "Drafty", "BaseText"],
             /, *,
             head: Optional[Dict[str, Any]] = None,
             timeout: Optional[float] = None
     ) -> Optional[int]:
         if isinstance(text, str) and '\n' in text:
             text = PlainText(text)
         if isinstance(text, BaseText):
@@ -75,42 +68,43 @@
     
     async def wait_reply(
             self,
             topic: Optional[str] = None,
             user_id: Optional[str] = None,
             pattern: Optional[re.Pattern] = None,
             priority: float = 1.2
-    ) -> Message:
+    ) -> "Message":
         loop = asyncio.get_running_loop()
         dispatcher = SessionDispatcher(
             self,
             loop.create_future(),
             topic=topic,
             user_id=user_id,
             pattern=pattern,
             priority=priority
         )
         message = await dispatcher.wait()
         return message
     
-    async def send_form(self, title: Union[str, BaseText], *button: Union[str, Button], **kwds: Any) -> int:
+    async def send_form(self, title: Union[str, "BaseText"], *button: Union[str, "Button"], **kwds: Any) -> int:
         chain = TextChain(Bold(content=PlainText(title)) if isinstance(title, str) else title)
         pred_resp = []
         for i in button:
             if isinstance(i, str):
                 name = i.strip().lower()
                 i = Button(text=i, name=name)
                 pred_resp.append({name: 1})
             elif i.name is not None:
                 pred_resp.append({i.name: 1 if i.val is None else i.val})
             else:
                 pred_resp.append(None)
             chain += TextChain(NewLine, i)
 
         async with get_message_lock():
+            # Obtain the message lock to ensure that the returned message is intercepted by the dispatcher
             seq_id = await self.send(Form(content=chain), **kwds)
             if not button:
                 return 0
             elif seq_id is None:
                 raise KaruhaRuntimeError("failed to fetch message id")
             
             loop = asyncio.get_running_loop()
@@ -119,70 +113,31 @@
                 loop.create_future(),
                 seq_id=seq_id
             )
             dispatcher.activate()
         try:
             resp = await dispatcher.wait()
         except:  # noqa: E722
+            # The dispatcher will automatically deactivate after receiving a message,
+            # so you only need to actively deactivate it when an exception occurs
             dispatcher.deactivate()
             raise
         return pred_resp.index(resp)
     
-    async def confirm(self, title: Union[str, BaseText], **kwds: Any) -> bool:
+    async def confirm(self, title: Union[str, "BaseText"], **kwds: Any) -> bool:
         return not await self.send_form(title, "Yes", "No", **kwds)
 
 
-class MessageSession(BaseSession):
-    __slots__ = ["_messages"]
-
-    def __init__(self, /, bot: Bot, message: Message) -> None:
-        super().__init__(bot, message.topic)
-        self._messages = deque((message,))
-    
-    async def wait_reply(
-            self,
-            topic: Optional[str] = None,
-            user_id: Optional[str] = None,
-            pattern: Optional[re.Pattern] = None,
-            priority: float = 1.2
-    ) -> Message:
-        message = await super().wait_reply(topic, user_id, pattern, priority)
-        self._add_message(message)
-        return message
-    
-    def _add_message(self, message: Message) -> None:
-        assert message.bot is self.bot
-        if message.topic != self.topic:
-            return
-        self._messages.append(message)
-
-    @property
-    def messages(self) -> Tuple[Message, ...]:
-        return tuple(self._messages)
-    
-    @property
-    def last_message(self) -> Message:
-        return self._messages[-1]
-
-
-class CommandSession(MessageSession):
-    __slots__ = []
-
-    _messages: Deque["CommandMessage"]
-
-    def cancel(self) -> NoReturn:
-        raise KaruhaCommandCanceledError
-    
-    @property
-    def messages(self) -> Tuple["CommandMessage", ...]:
-        return tuple(self._messages)
-    
-    @property
-    def last_message(self) -> "CommandMessage":
-        return self._messages[-1]
+from .exception import KaruhaRuntimeError
+from .text.drafty import Drafty
+from .text.textchain import (BaseText, Bold, Button, File, Form, Image,
+                             NewLine, PlainText, TextChain)
+from .text.message import Message
+from .utils.dispatcher import FutureDispatcher
+from .event.message import MessageDispatcher, get_message_lock
 
 
 class SessionDispatcher(MessageDispatcher, FutureDispatcher[Message]):
     __slots__ = ["session", "priority", "topic", "user_id", "pattern"]
 
     def __init__(
             self,
@@ -247,10 +202,7 @@
                 self._cache[id(message)] = resp
                 return self.priority
         return -1
     
     def run(self, message: Message) -> None:
         resp = self._cache.get((id(message)))
         self.future.set_result(resp)
-
-
-from .command import CommandMessage
```

### Comparing `KaruhaBot-0.2.0b3/karuha/config.py` & `karuhabot-0.2.0b4/karuha/config.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/data/__init__.py` & `karuhabot-0.2.0b4/karuha/data/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-from .cache import get_user_tags, get_user_cred, clear_meta_cache
-from .user import BaseUser, User, get_user, get_user_list
+from .cache import get_user_tags, get_user_cred, clear_cache
+from .user import BaseUser, User, get_user, get_user_list, try_get_user
 from .topic import BaseTopic, Topic, TopicSub, get_topic, get_p2p_topic, get_group_topic
 from .sub import ensure_sub, has_sub
 from .data import get_data
 
 
 __all__ = [
     "BaseUser",
     "User",
     "BaseTopic",
     "Topic",
     "TopicSub",
     "get_user",
     "get_user_list",
+    "try_get_user",
     "get_topic",
     "get_p2p_topic",
     "get_group_topic",
     "ensure_sub",
     "has_sub",
     "get_user_tags",
     "get_user_cred",
     "get_data",
-    "clear_meta_cache",
+    "clear_cache",
 ]
```

### Comparing `KaruhaBot-0.2.0b3/karuha/data/cache.py` & `karuhabot-0.2.0b4/karuha/data/cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from typing import (FrozenSet, Iterable, List, Optional, Tuple, TypeVar, Union,
                     overload)
 
 from pydantic import BaseModel
 from tinode_grpc import pb
 
+from ..event.sys import SystemStartEvent
+
+from ..event.message import MessageEvent
+
 from ..bot import Bot
 from ..event import on
 from ..event.bot import MetaEvent
-from ..store import (DataModel, MemoryStore, PrimaryKey, TopicBoundDataModel,
+from ..store import (DataModel, LruStore, MemoryStore, MessageBoundDataModel, PrimaryKey, TopicBoundDataModel,
                      UserBoundDataModel)
+from ..text import Message
 from .meta import (BaseDesc, BaseSubscription, CommonDesc, Cred,
                    GroupTopicDesc, P2PTopicDesc, Subscription, TopicInfo,
                    UserCred, UserDesc, UserTags)
 from .sub import ensure_sub
 
 T = TypeVar("T", bound=BaseModel)
 
@@ -48,18 +53,23 @@
     desc: P2PTopicDesc
 
 
 class SubscriptionCache(TopicBoundDataModel, UserBoundDataModel):
     sub: BaseSubscription
 
 
+class MessageCache(MessageBoundDataModel):
+    message: Message
+
+
 user_cache = MemoryStore[UserCache]("user_meta_cache")
 group_cache = MemoryStore[GroupTopicCache]("group_meta_cache")
 p2p_cache = MemoryStore[P2PTopicCache]("p2p_meta_cache")
 subscription_cache = MemoryStore[SubscriptionCache]("sub_meta_cache")
+message_cache = LruStore[MessageCache]("message_cache")
 
 
 def update_user_cache(
     user_id: str,
     desc: Optional[BaseDesc] = None,
     tags: Optional[UserTags] = None,
     cred: Optional[UserCred] = None,
@@ -99,14 +109,30 @@
     if (topic, user_id) not in subscription_cache:
         subscription_cache.add(SubscriptionCache(topic=topic, user_id=user_id, sub=sub))
         return
     cache = subscription_cache[topic, user_id]
     cache.sub = _update_model(cache.sub, sub)
 
 
+def update_message_cache(message: Message) -> None:
+    if (message.topic, message.seq_id) not in message_cache:
+        message_cache.add(MessageCache(topic=message.topic, seq_id=message.seq_id, message=message))
+        return
+    cache = message_cache[message.topic, message.seq_id]
+    cache.message = message
+
+
+def try_get_user_desc(bot: Bot, /, user_id: str) -> Optional[BaseDesc]:
+    if user_id == "me":
+        cache = user_cache.get(bot.uid)
+    else:
+        cache = user_cache.get(user_id)
+    return cache and cache.desc
+
+
 async def get_user_desc(bot: Bot, /, user_id: str, *, ensure_meta: bool = False) -> BaseDesc:
     assert user_id.startswith("usr") or user_id == "me", "user_id must be a user"
     if user_id == "me":
         user = user_cache.get(bot.uid)
     else:
         assert not ensure_meta, "only 'me' can be used with ensure_meta=True"
         user = user_cache.get(user_id)
@@ -114,14 +140,22 @@
         return user.desc
     await ensure_sub(bot, user_id)
     _, user = await bot.get(user_id, "desc")
     assert user is not None
     return UserDesc.from_meta(user.desc)
 
 
+def try_get_group_desc(bot: Bot, /, topic_id: str) -> Optional[BaseDesc]:
+    assert topic_id.startswith("grp"), "topic_id must be a group topic"
+    topic = group_cache.get(topic_id)
+    desc = topic and topic.desc
+    assert desc is None or isinstance(desc, BaseDesc)
+    return desc
+
+
 async def get_group_desc(
     bot: Bot, /, topic_id: str, *, ensure_meta: bool = False
 ) -> BaseDesc:
     assert topic_id.startswith("grp"), "topic_id must be a group topic"
     topic = group_cache.get(topic_id)
     if (
         topic is not None
@@ -132,14 +166,26 @@
         return topic.desc
     await ensure_sub(bot, topic_id)
     _, topic = await bot.get(topic_id, "desc")
     assert topic is not None
     return GroupTopicDesc.from_meta(topic.desc)
 
 
+def try_get_p2p_desc(bot: Bot, /, topic_id: str) -> Optional[TopicInfo]:
+    if topic_id.startswith("p2p"):
+        topic = group_cache.get(topic_id)
+        desc = topic and topic.desc
+        assert isinstance(desc, TopicInfo)
+        return desc
+    assert topic_id.startswith("usr")
+    user_pair = frozenset((bot.uid, topic_id))
+    topic = p2p_cache.get(user_pair)
+    return topic and topic.desc
+
+
 async def _get_p2p_topic(bot: Bot, /, topic_id: str) -> TopicInfo:
     topic = group_cache.get(topic_id)
     if (
         topic is not None
         and topic.desc is not None
         and isinstance(topic.desc, TopicInfo)
     ):
@@ -161,14 +207,19 @@
         return topic.desc
     await ensure_sub(bot, user_id)
     _, topic = await bot.get(user_id, "desc")
     assert topic is not None
     return P2PTopicDesc.from_meta(topic.desc)
 
 
+def try_get_sub(bot: Bot, /, topic_id: str) -> Optional[BaseSubscription]:
+    sub = subscription_cache.get((topic_id, bot.uid))
+    return sub and sub.sub
+
+
 async def get_sub(bot: Bot, /, topic_id: str, *, ensure_meta: bool = False) -> BaseSubscription:
     assert topic_id != "me", "topic_id must not be 'me'"
     sub = subscription_cache.get((topic_id, bot.uid))
     if sub is not None and (not ensure_meta or isinstance(sub.sub, Subscription)):
         return sub.sub
     await ensure_sub(bot, topic_id)
     _, sub_meta = await bot.get("me", "sub")
@@ -228,21 +279,14 @@
         return cache.cred.copy()
     await ensure_sub(bot, "me")
     _, cred_meta = await bot.get("me", "cred")
     assert cred_meta is not None
     return [Cred(method=c.method, value=c.value, done=c.done) for c in cred_meta.cred]
 
 
-def clear_meta_cache() -> None:
-    user_cache.clear()
-    p2p_cache.clear()
-    group_cache.clear()
-    subscription_cache.clear()
-
-
 def cache_user(user_id: str, desc: pb.TopicDesc) -> None:
     user = UserDesc.from_meta(desc)
     update_user_cache(user_id, desc=user)
 
 
 def cache_p2p_topic(user_id: str, topic_id: str, desc: pb.TopicDesc) -> None:
     topic = P2PTopicDesc.from_meta(desc)
@@ -292,15 +336,15 @@
 
 
 @on(MetaEvent)
 def handle_meta(event: MetaEvent) -> None:
     meta = event.server_message
     user = event.bot.uid
     topic = meta.topic
-    if meta.desc:
+    if meta.HasField("desc"):
         if topic == "me":
             cache_user(user, meta.desc)
         elif topic.startswith("usr"):
             cache_p2p_topic(user, topic, meta.desc)
         else:
             cache_group_topic(user, topic, meta.desc)
     if meta.sub:
@@ -317,7 +361,21 @@
         update_user_cache(
             topic,
             cred=[
                 {"method": c.method, "value": c.value, "done": c.done}
                 for c in meta.cred
             ],  # type: ignore
         )
+
+
+@on(MessageEvent)
+def handle_message(event: MessageEvent) -> None:
+    update_message_cache(event.message)
+
+
+@on(SystemStartEvent)
+def clear_cache() -> None:
+    user_cache.clear()
+    p2p_cache.clear()
+    group_cache.clear()
+    subscription_cache.clear()
+    message_cache.clear()
```

### Comparing `KaruhaBot-0.2.0b3/karuha/data/meta.py` & `karuhabot-0.2.0b4/karuha/data/meta.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Self
 
-from pydantic import BaseModel, Json, model_validator
+from pydantic import BaseModel, Json, model_serializer, model_validator
 from tinode_grpc import pb
 
 from ..utils.decode import msg2dict
 
 
 class AccessPermission(BaseModel):
     """
@@ -66,14 +66,35 @@
                 result["delete"] = True
             elif i == "O":
                 result["owner"] = True
             else:
                 raise ValueError(f"unknown permission: {i}")
         return result
 
+    @model_serializer(mode="plain")
+    def serialize(self) -> str:
+        result = ""
+        if self.join:
+            result += "J"
+        if self.read:
+            result += "R"
+        if self.write:
+            result += "W"
+        if self.presence:
+            result += "P"
+        if self.approve:
+            result += "A"
+        if self.sharing:
+            result += "S"
+        if self.delete:
+            result += "D"
+        if self.owner:
+            result += "O"
+        return result
+
 
 class Cred(BaseModel):
     method: str
     value: str
     done: bool = False
```

### Comparing `KaruhaBot-0.2.0b3/karuha/data/sub.py` & `karuhabot-0.2.0b4/karuha/data/sub.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/data/topic.py` & `karuhabot-0.2.0b4/karuha/data/topic.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 from typing import Any, Dict, List, Literal, Optional, overload
 
 from pydantic import BaseModel
 from pydantic_core import to_json
 from tinode_grpc import pb
 
 from ..bot import Bot
-from .meta import Access, CommonDesc, DefaultAccess, GroupTopicDesc, Subscription
-from .cache import get_my_sub, p2p_cache, get_group_desc, get_p2p_desc, get_sub, get_user_desc
+from .cache import (get_group_desc, get_my_sub, get_p2p_desc, get_sub,
+                    get_user_desc, try_get_group_desc, try_get_p2p_desc, try_get_sub,
+                    try_get_user_desc)
+from .meta import (Access, CommonDesc, DefaultAccess, GroupTopicDesc,
+                   Subscription)
 
 
 class BaseInfo(BaseModel, frozen=True):
     public: Optional[Dict[str, Any]] = None
     trusted: Optional[Dict[str, Any]] = None
     private: Optional[Dict[str, Any]] = None
 
@@ -138,51 +141,107 @@
         await bot.set(topic_id, desc=set_desc)
         return
     extra = pb.ClientExtra(on_behalf_of=topic_id)
     await bot.subscribe("me", set=pb.SetQuery(desc=set_desc), extra=extra)
     await bot.leave("me", extra=extra)
 
 
+def try_get_p2p_topic(bot: Bot, /, topic_id: str) -> Optional[BaseTopic]:
+    desc = try_get_user_desc(bot, topic_id)
+    info = try_get_p2p_desc(bot, topic_id)
+    sub = try_get_sub(bot, topic_id)
+    if desc is not None:
+        if isinstance(desc, CommonDesc) and info is not None and sub is not None:
+            return Topic(
+                topic=topic_id,
+                public=desc.public,
+                trusted=desc.trusted,
+                private=sub.private,
+                created=info.created,
+                updated=info.updated,
+                touched=info.touched,
+                defacs=desc.defacs,
+                acs=sub.acs,
+                seq=info.seq,
+                read=sub.read,
+                recv=sub.recv,
+                clear=sub.clear,
+            )
+        return BaseTopic(
+            topic=topic_id,
+            public=desc.public,
+            trusted=desc.trusted,
+        )
+
+
 @overload
 async def get_p2p_topic(bot: Bot, /, topic_id: str, *, ensure_topic: Literal[True]) -> Topic: ...
 @overload
 async def get_p2p_topic(bot: Bot, /, topic_id: str, *, ensure_topic: bool = False) -> BaseTopic: ...
 
 
 async def get_p2p_topic(bot: Bot, /, topic_id: str, *, ensure_topic: bool = False) -> BaseTopic:
-    user_desc = await get_user_desc(bot, user_id=topic_id, ensure_meta=False)
+    desc = await get_user_desc(bot, user_id=topic_id, ensure_meta=False)
     sub = await get_sub(bot, topic_id=topic_id, ensure_meta=False)
-    if (
-        not isinstance(user_desc, CommonDesc)
-        or (not ensure_topic and frozenset((topic_id, bot.uid)) not in p2p_cache)
-    ):
+    info = try_get_p2p_desc(bot, topic_id)
+    if isinstance(desc, CommonDesc) and ensure_topic and info is None:
+        info = await get_p2p_desc(bot, topic_id)
+    elif not isinstance(desc, CommonDesc) or info is None:
         return BaseTopic(
             topic=topic_id,
-            public=user_desc.public,
-            trusted=user_desc.trusted,
+            public=desc.public,
+            trusted=desc.trusted,
             private=sub.private,
         )
-    p2p_desc = await get_p2p_desc(bot, user_id=topic_id)
     return Topic(
         topic=topic_id,
-        public=user_desc.public,
-        trusted=user_desc.trusted,
+        public=desc.public,
+        trusted=desc.trusted,
         private=sub.private,
-        created=p2p_desc.created,
-        updated=p2p_desc.updated,
-        touched=p2p_desc.touched,
-        seq=p2p_desc.seq,
-        defacs=user_desc.defacs,
+        created=info.created,
+        updated=info.updated,
+        touched=info.touched,
+        seq=info.seq,
+        defacs=desc.defacs,
         acs=sub.acs,
         read=sub.read,
         recv=sub.recv,
         clear=sub.clear
     )
 
 
+def try_get_group_topic(bot: Bot, /, topic_id: str) -> Optional[BaseTopic]:
+    desc = try_get_group_desc(bot, topic_id)
+    sub = try_get_sub(bot, topic_id)
+    if isinstance(desc, GroupTopicDesc) and sub is not None:
+        return Topic(
+            topic=topic_id,
+            public=desc.public,
+            trusted=desc.trusted,
+            private=sub.private,
+            is_chan=desc.is_chan,
+            defacs=desc.defacs,
+            acs=sub.acs,
+            seq=desc.seq,
+            created=desc.created,
+            updated=desc.updated,
+            touched=desc.touched,
+            read=sub.read,
+            recv=sub.recv,
+            clear=sub.clear
+        )
+    elif desc is not None:
+        return BaseTopic(
+            topic=topic_id,
+            public=desc.public,
+            trusted=desc.trusted,
+            private=sub and sub.private,
+        )
+
+
 @overload
 async def get_group_topic(bot: Bot, /, topic_id: str, *, ensure_topic: Literal[True]) -> Topic: ...
 @overload
 async def get_group_topic(bot: Bot, /, topic_id: str, *, ensure_topic: bool = False) -> BaseTopic: ...
 
 
 async def get_group_topic(bot: Bot, /, topic_id: str, *, ensure_topic: bool = False) -> BaseTopic:
```

### Comparing `KaruhaBot-0.2.0b3/karuha/data/user.py` & `karuhabot-0.2.0b4/karuha/data/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from typing import List, Literal, Optional, overload
 
 from ..bot import Bot
-from .cache import get_sub, get_topic_sub, get_user_desc
+from .cache import get_sub, get_topic_sub, get_user_desc, try_get_sub, try_get_user_desc
 from .meta import Access, DefaultAccess, Subscription, UserDesc
 from .topic import BaseInfo
 
 
 class BaseUser(BaseInfo, frozen=True):
     user_id: str
 
@@ -37,14 +37,45 @@
     touched: Optional[datetime] = None
     read: Optional[int] = None
     recv: Optional[int] = None
     clear: Optional[int] = None
     acs: Optional[Access] = None
 
 
+def try_get_user(bot: Bot, /, user_id: str = "me") -> Optional[BaseUser]:
+    if user_id == bot.uid:
+        user_id = "me"
+    desc = try_get_user_desc(bot, user_id)
+    if user_id == "me":
+        sub = None
+    else:
+        sub = try_get_sub(bot, user_id)
+    if isinstance(desc, UserDesc) and sub is not None:
+        return User(
+            user_id=bot.uid,
+            public=desc.public,
+            trusted=desc.trusted,
+            private=sub and sub.private,
+            state=desc.state,
+            state_at=desc.state_at,
+            created=desc.created,
+            updated=desc.updated,
+            touched=desc.touched,
+            defacs=desc.defacs,
+            acs=sub and sub.acs,
+        )
+    elif desc is not None:
+        return BaseUser(
+            user_id=bot.uid,
+            public=desc.public,
+            trusted=desc.trusted,
+            private=sub and sub.private
+        )
+
+
 @overload
 async def get_user(bot: Bot, /, user_id: str = "me", *, ensure_user: Literal[True]) -> User: ...
 @overload
 async def get_user(bot: Bot, /, user_id: str = "me", *, ensure_user: bool = False) -> BaseUser: ...
 
 
 async def get_user(bot: Bot, /, user_id: str = "me", *, ensure_user: bool = False) -> BaseUser:
```

### Comparing `KaruhaBot-0.2.0b3/karuha/event/bot.py` & `karuhabot-0.2.0b4/karuha/event/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import asyncio
 from functools import partial
-from typing import Any, Awaitable, Callable, Coroutine, Mapping, Optional
+from typing import Any, Awaitable, Callable, Coroutine, Mapping, Optional, TypeVar
 from typing_extensions import Self
 
 from google.protobuf.message import Message
 from tinode_grpc import pb
 
 from .. import bot
 from .base import Event, handler_runner
+from ..session import BaseSession
 from ..utils.proxy_propery import ProxyProperty
+from ..utils.invoker import Dependency, depend_property
 
 
 def ensure_text_len(text: str, length: int = 128) -> str:
     if len(text) < length:
         return text
     tail_length = length // 4
     return f"{text[:length-tail_length]} ... {text[-tail_length:]}"
 
 
 class BotEvent(Event):
     __slots__ = ["bot"]
 
+    bot: Dependency["bot.Bot"]
+
     def __init__(self, bot: "bot.Bot", /) -> None:
         self.bot = bot
 
     def call_handler(self, handler: Callable[[Self], Coroutine]) -> Awaitable:
         return self.bot._create_task(handler_runner(self, self.bot.logger, handler))
 
 
@@ -54,26 +58,33 @@
     __slots__ = []
 
 
 bot.Bot.initialize_event_callback = BotInitEvent.new
 bot.Bot.finalize_event_callback = BotFinishEvent.new_and_wait
 
 
+T = TypeVar("T")
+ProxyPropertyType = Dependency[ProxyProperty[T]]
+SessionProperty = depend_property(lambda ev: BaseSession(ev.bot, ev.topic))
+
+
 # Server Event Part
 # =========================
 
 
 ServerMessageProperty = partial(ProxyProperty, "server_message")
 
 
 class ServerEvent(BotEvent):
     """base class for all events from server"""
 
     __slots__ = ["server_message"]
 
+    server_message: Dependency[Message]
+
     def __init__(self, bot: "bot.Bot", message: Message) -> None:
         super().__init__(bot)
         self.server_message = message
 
     def __init_subclass__(cls, on_field: str, **kwds: Any) -> None:
         super().__init_subclass__(**kwds)
         bot.Bot.server_event_callbacks[on_field].append(cls.new)
@@ -111,23 +122,24 @@
     for the possible values of the `head` field.
     """
 
     __slots__ = []
 
     server_message: pb.ServerData
 
-    topic: ProxyProperty[str] = ServerMessageProperty()
-    from_user_id: ProxyProperty[str] = ServerMessageProperty()
-    timestamp: ProxyProperty[int] = ServerMessageProperty()
-    deleted_at: ProxyProperty[int] = ServerMessageProperty()
-    seq_id: ProxyProperty[int] = ServerMessageProperty()
-    head: ProxyProperty[Mapping[str, bytes]] = ServerMessageProperty()
-    content: ProxyProperty[bytes] = ServerMessageProperty()
+    topic: ProxyPropertyType[str] = ServerMessageProperty()
+    from_user_id: ProxyPropertyType[str] = ServerMessageProperty()
+    timestamp: ProxyPropertyType[int] = ServerMessageProperty()
+    deleted_at: ProxyPropertyType[int] = ServerMessageProperty()
+    seq_id: ProxyPropertyType[int] = ServerMessageProperty()
+    head: ProxyPropertyType[Mapping[str, bytes]] = ServerMessageProperty()
+    content: ProxyPropertyType[bytes] = ServerMessageProperty()
+    session = SessionProperty
 
-    @property
+    @depend_property
     def text(self) -> str:
         return self.content.decode(errors="ignore")
 
 
 class CtrlEvent(ServerEvent, on_field="ctrl"):
     """
     Generic response indicating an error or a success condition. The message is sent to the originating session.
@@ -147,19 +159,20 @@
     ```
     """
 
     __slots__ = []
 
     server_message: pb.ServerCtrl
 
-    id: ProxyProperty[str] = ServerMessageProperty()
-    topic: ProxyProperty[str] = ServerMessageProperty()
-    code: ProxyProperty[int] = ServerMessageProperty()
-    text: ProxyProperty[str] = ServerMessageProperty()
-    params: ProxyProperty[Mapping[str, bytes]] = ServerMessageProperty()
+    id: ProxyPropertyType[str] = ServerMessageProperty()
+    topic: ProxyPropertyType[str] = ServerMessageProperty()
+    code: ProxyPropertyType[int] = ServerMessageProperty()
+    text: ProxyPropertyType[str] = ServerMessageProperty()
+    params: ProxyPropertyType[Mapping[str, bytes]] = ServerMessageProperty()
+    session = SessionProperty
     
     async def __default_handler__(self) -> None:
         tid = self.server_message.id
         self.bot._set_reply_message(tid, self.server_message)
 
 
 class MetaEvent(ServerEvent, on_field="meta"):
@@ -270,16 +283,17 @@
     ```
     """
 
     __slots__ = []
 
     server_message: pb.ServerMeta
 
-    id: ProxyProperty[str] = ServerMessageProperty()
-    topic: ProxyProperty[str] = ServerMessageProperty()
+    id: ProxyPropertyType[str] = ServerMessageProperty()
+    topic: ProxyPropertyType[str] = ServerMessageProperty()
+    session = SessionProperty
     
     async def __default_handler__(self) -> None:
         tid = self.server_message.id
         self.bot._set_reply_message(tid, self.server_message)
 
 
 class PresEvent(ServerEvent, on_field="pres"):
@@ -328,22 +342,23 @@
     Timestamp is not present in `{pres}` messages.
     """  # noqa
 
     __slots__ = []
 
     server_message: pb.ServerPres
 
-    topic: ProxyProperty[str] = ServerMessageProperty()
-    src: ProxyProperty[str] = ServerMessageProperty()
-    what: ProxyProperty["pb.ServerPres.What"] = ServerMessageProperty()
-    user_agent: ProxyProperty[str] = ServerMessageProperty()
-    seq_id: ProxyProperty[int] = ServerMessageProperty()
-    del_id: ProxyProperty[int] = ServerMessageProperty()
-    target_user_id: ProxyProperty[str] = ServerMessageProperty()
-    actor_user_id: ProxyProperty[str] = ServerMessageProperty()
+    topic: ProxyPropertyType[str] = ServerMessageProperty()
+    src: ProxyPropertyType[str] = ServerMessageProperty()
+    what: ProxyPropertyType["pb.ServerPres.What"] = ServerMessageProperty()
+    user_agent: ProxyPropertyType[str] = ServerMessageProperty()
+    seq_id: ProxyPropertyType[int] = ServerMessageProperty()
+    del_id: ProxyPropertyType[int] = ServerMessageProperty()
+    target_user_id: ProxyPropertyType[str] = ServerMessageProperty()
+    actor_user_id: ProxyPropertyType[str] = ServerMessageProperty()
+    session = SessionProperty
 
     async def __default_handler__(self) -> None:
         msg = self.server_message
         if msg.topic != "me":
             return
         if msg.what == pb.ServerPres.ON:
             await self.bot.subscribe(msg.src, get="desc sub")
@@ -389,20 +404,21 @@
     ```
     """
 
     __slots__ = []
 
     server_message: pb.ServerInfo
 
-    topic: ProxyProperty[str] = ServerMessageProperty()
-    from_user_id: ProxyProperty[str] = ServerMessageProperty()
-    what: ProxyProperty["pb.InfoNote"] = ServerMessageProperty()
-    seq_id: ProxyProperty[int] = ServerMessageProperty()
-    src: ProxyProperty[str] = ServerMessageProperty()
-    payload: ProxyProperty[bytes] = ServerMessageProperty()
+    topic: ProxyPropertyType[str] = ServerMessageProperty()
+    from_user_id: ProxyPropertyType[str] = ServerMessageProperty()
+    what: ProxyPropertyType["pb.InfoNote"] = ServerMessageProperty()
+    seq_id: ProxyPropertyType[int] = ServerMessageProperty()
+    src: ProxyPropertyType[str] = ServerMessageProperty()
+    payload: ProxyPropertyType[bytes] = ServerMessageProperty()
+    session = SessionProperty
 
 
 # Client Event Part
 # =========================
 
 
 ClientMessageProperty = partial(ProxyProperty, "client_message")
@@ -459,17 +475,17 @@
     The `token` contains an encrypted string which can be used for authentication.
     Expiration time of the token is passed as `expires`.
     """
     __slots__ = []
 
     client_message: pb.ClientLogin
 
-    id: ProxyProperty[str] = ClientMessageProperty()
-    scheme: ProxyProperty[str] = ClientMessageProperty()
-    secret: ProxyProperty[bytes] = ClientMessageProperty()
+    id: ProxyPropertyType[str] = ClientMessageProperty()
+    scheme: ProxyPropertyType[str] = ClientMessageProperty()
+    secret: ProxyPropertyType[bytes] = ClientMessageProperty()
 
     async def __default_handler__(self) -> None:
         await self.bot.subscribe(
             "me",
             get="sub desc tags cred"
         )
 
@@ -535,18 +551,19 @@
     """
 
     __slots__ = []
 
     client_message: pb.ClientPub
     response_message: Optional[pb.ServerCtrl]
     
-    id: ProxyProperty[str] = ClientMessageProperty()
-    topic: ProxyProperty[str] = ClientMessageProperty()
-    head: ProxyProperty[Mapping[str, bytes]] = ClientMessageProperty()
-    content: ProxyProperty[bytes] = ClientMessageProperty()
+    id: ProxyPropertyType[str] = ClientMessageProperty()
+    topic: ProxyPropertyType[str] = ClientMessageProperty()
+    head: ProxyPropertyType[Mapping[str, bytes]] = ClientMessageProperty()
+    content: ProxyPropertyType[bytes] = ClientMessageProperty()
+    session = SessionProperty
     
     async def __default_handler__(self) -> None:
         self.bot.logger.info(f"({self.topic})<= {ensure_text_len(self.text)}")
 
     @property
     def text(self) -> str:
         return self.content.decode(errors="ignore")
@@ -671,16 +688,17 @@
     ```
     """
 
     __slots__ = []
 
     client_message: pb.ClientSub
 
-    id: ProxyProperty[str] = ClientMessageProperty()
-    topic: ProxyProperty[str] = ClientMessageProperty()
+    id: ProxyPropertyType[str] = ClientMessageProperty()
+    topic: ProxyPropertyType[str] = ClientMessageProperty()
+    session = SessionProperty
 
 
 class LeaveEvent(ClientEvent, on_field="leave"):
     """
     This is a counterpart to `{sub}` message. It also serves two functions:
     * leaving the topic without unsubscribing (`unsub=false`)
     * unsubscribing (`unsub=true`)
@@ -699,10 +717,11 @@
     ```
     """
 
     __slots__ = []
 
     client_message: pb.ClientLeave
 
-    id: ProxyProperty[str] = ClientMessageProperty()
-    topic: ProxyProperty[str] = ClientMessageProperty()
-    unsub: ProxyProperty[bool] = ClientMessageProperty()
+    id: ProxyPropertyType[str] = ClientMessageProperty()
+    topic: ProxyPropertyType[str] = ClientMessageProperty()
+    unsub: ProxyPropertyType[bool] = ClientMessageProperty()
+    session = SessionProperty
```

### Comparing `KaruhaBot-0.2.0b3/karuha/event/command.py` & `karuhabot-0.2.0b4/karuha/event/command.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/event/message.py` & `karuhabot-0.2.0b4/karuha/event/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import asyncio
 from functools import partial
 from typing import Dict, Union
 
 from typing_extensions import Self
 
 from ..bot import Bot, decode_mapping
-from ..text import BaseText, Drafty, Message
+from ..text import BaseText, Drafty
+from ..text.message import Message
 from ..utils.dispatcher import AbstractDispatcher
+from ..utils.locks import Lock
 from ..utils.proxy_propery import ProxyProperty
 from . import on
-from .bot import BotEvent, DataEvent, BotInitEvent, ensure_text_len
+from .bot import BotEvent, DataEvent, ensure_text_len
 
 
 MessageProperty = partial(ProxyProperty, "message", mutable=True)
 
 
 class MessageEvent(BotEvent):
     """a parsed DataMessage"""
@@ -60,28 +61,16 @@
 
 class MessageDispatcher(AbstractDispatcher[Message]):
     __slots__ = []
 
     dispatchers = set()
 
 
-_message_lock = None
-
-
-def get_message_lock() -> asyncio.Lock:
-    global _message_lock
-    if _message_lock is None:
-        _message_lock = asyncio.Lock()
-    return _message_lock
+def get_message_lock() -> Lock:
+    return MessageEvent.get_lock()
 
 
 def reset_message_lock() -> None:
-    global _message_lock
-    _message_lock = None
+    del MessageEvent.__event_lock__
 
 
 on_message = on(MessageEvent)
-
-
-@on(BotInitEvent)
-def _(event: BotInitEvent) -> None:
-    reset_message_lock()
```

### Comparing `KaruhaBot-0.2.0b3/karuha/event/plugin.py` & `karuhabot-0.2.0b4/karuha/event/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 from functools import partial
 from typing import Awaitable, Callable, Coroutine, Union
 
 from tinode_grpc import pb
 from typing_extensions import Self
 
 from ..command.session import BaseSession
-
-from .. import get_all_bots, _get_running_loop
 from ..bot import Bot
 from ..logger import logger
 from ..utils.proxy_propery import ProxyProperty
+from ..utils.invoker import depend_property, Dependency
+from ..runner import get_all_bots, _get_running_loop
 from . import on
 from .base import Event
-from .bot import BotEvent
+from .bot import BotEvent, ProxyPropertyType, SessionProperty
 
 
 class PluginServerEvent(Event):
     """base class for all event from plugin server"""
     __slots__ = ["raw_message"]
 
+    raw_message: Dependency[Union[pb.TopicEvent, pb.AccountEvent, pb.SubscriptionEvent, pb.MessageEvent]]
+
     def __init__(self, message: Union[pb.TopicEvent, pb.AccountEvent, pb.SubscriptionEvent, pb.MessageEvent]) -> None:
         super().__init__()
         self.raw_message = message
 
-    @property
+    @depend_property
     def action(self) -> pb.Crud:
         return self.raw_message.action
 
     def call_handler(self, handler: Callable[[Self], Coroutine]) -> Awaitable:
         loop = _get_running_loop()
         future = asyncio.run_coroutine_threadsafe(handler(self), loop)
         return asyncio.wrap_future(future, loop=loop)
@@ -38,26 +40,26 @@
 
 
 class TopicEvent(PluginServerEvent):
     __slots__ = []
 
     raw_message: pb.TopicEvent
     
-    name: ProxyProperty[str] = PluginServerProperty()
-    desc: ProxyProperty["pb.TopicDesc"] = PluginServerProperty()
+    name: ProxyPropertyType[str] = PluginServerProperty()
+    desc: ProxyPropertyType["pb.TopicDesc"] = PluginServerProperty()
 
 
 class AccountEvent(PluginServerEvent):
     __slots__ = []
 
     raw_message: pb.AccountEvent
 
-    user_id: ProxyProperty[str] = PluginServerProperty()
-    action: ProxyProperty["pb.Crud"] = PluginServerProperty()
-    public: ProxyProperty[bytes] = PluginServerProperty()
+    user_id: ProxyPropertyType[str] = PluginServerProperty()
+    action: ProxyPropertyType["pb.Crud"] = PluginServerProperty()
+    public: ProxyPropertyType[bytes] = PluginServerProperty()
 
     async def __default_handler__(self) -> None:
         action = self.action
         if action == pb.Crud.CREATE:
             for i in get_all_bots():
                 if not i.config.auto_subscribe_new_user:
                     logger.debug(f"ignore auto subscribe for {i.name}")
@@ -67,41 +69,46 @@
 
 
 class SubscriptionEvent(PluginServerEvent):
     __slots__ = []
 
     raw_message: pb.SubscriptionEvent
 
-    user_id: ProxyProperty[str] = PluginServerProperty()
-    topic: ProxyProperty[str] = PluginServerProperty()
+    user_id: ProxyPropertyType[str] = PluginServerProperty()
+    topic: ProxyPropertyType[str] = PluginServerProperty()
 
+    session = SessionProperty
 
-class MessageEvent(PluginServerEvent, property_export={"data": "msg"}):
+
+class MessageEvent(PluginServerEvent):
     __slots__ = []
 
     raw_message: pb.MessageEvent
 
-    data: ProxyProperty["pb.ServerData"] = PluginServerProperty(name="msg")
-    topic = ProxyProperty[str]("data")
-    from_user_id = ProxyProperty[str]("data")
-    user_id = ProxyProperty[str]("data", name="from_user_id")
-    content = ProxyProperty[bytes]("data")
+    data: ProxyPropertyType["pb.ServerData"] = PluginServerProperty(name="msg")
+    topic = ProxyPropertyType[str]("data")
+    from_user_id = ProxyPropertyType[str]("data")
+    user_id = ProxyPropertyType[str]("data", name="from_user_id")
+    content = ProxyPropertyType[bytes]("data")
+
+    session = SessionProperty
 
 
 class AccountCreateEvent(BotEvent):
     __slots__ = ["raw_message"]
 
     raw_message: pb.AccountEvent
 
-    user_id: ProxyProperty[str] = PluginServerProperty()
-    action: ProxyProperty["pb.Crud"] = PluginServerProperty()
-    public: ProxyProperty[bytes] = PluginServerProperty()
+    user_id: ProxyPropertyType[str] = PluginServerProperty()
+    action: ProxyPropertyType["pb.Crud"] = PluginServerProperty()
+    public: ProxyPropertyType[bytes] = PluginServerProperty()
 
     def __init__(self, bot: Bot, message: pb.AccountEvent) -> None:
         super().__init__(bot)
         self.raw_message = message
     
-    def get_session(self) -> BaseSession:
+    @depend_property
+    def session(self) -> BaseSession:
         return BaseSession(self.bot, self.user_id)
 
 
 on_new_account = on(AccountCreateEvent)
```

### Comparing `KaruhaBot-0.2.0b3/karuha/logger.py` & `karuhabot-0.2.0b4/karuha/logger.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/plugin_server.py` & `karuhabot-0.2.0b4/karuha/plugin_server.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/store.py` & `karuhabot-0.2.0b4/karuha/store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import os
 import warnings
 from abc import abstractmethod
 from collections import deque
 from inspect import isabstract
-from typing import (Any, ClassVar, Dict, Generic, Iterable, Iterator, List,
-                    Literal, Optional, Tuple, Type, TypeVar, Union, cast,
+from typing import (Any, ClassVar, Deque, Dict, Generic, Iterable, Iterator,
+                    List, Literal, Optional, Tuple, Type, TypeVar, Union, cast,
                     overload)
 from weakref import WeakKeyDictionary, WeakSet
 
 from aiofiles import open as aio_open
 from aiofiles import os as aio_os
 from aiofiles import ospath as aio_ospath
 from pydantic import (BaseModel, Field, GetCoreSchemaHandler, StrictInt,
@@ -169,22 +169,22 @@
             self.discard(i)
 
     @abstractmethod
     def get_all(self) -> Iterable[T_Data]:
         raise NotImplementedError
 
     @abstractmethod
-    def keys(self) -> Iterator[Any]:
+    def keys(self) -> Iterable[Any]:
         raise NotImplementedError
 
-    def values(self) -> Iterator[T_Data]:
+    def values(self) -> Iterable[T_Data]:
         for key in self.keys():
             yield self[key]
 
-    def items(self) -> Iterator[Tuple[Any, T_Data]]:
+    def items(self) -> Iterable[Tuple[Any, T_Data]]:
         for key in self.keys():
             yield key, self[key]
 
     @classmethod
     def get_store_class(cls, name: str, /) -> Type[Self]:
         return cls.__store_collection__.get(name, cls)
 
@@ -390,14 +390,109 @@
     def prepare_data(self) -> None:
         pass
 
     def update_data(self) -> None:
         pass
 
 
+class LruStore(AbstractDataStore[T_Data], store_type="lru"):
+    __slots__ = ["_cache", "_index"]
+
+    def __init__(
+        self, name: StrictStr, maxlen: int = 128, *, data_type: Optional[Type[T_Data]] = None
+    ) -> None:
+        super().__init__(name, data_type=data_type)
+        self._cache: Deque[T_Data] = deque(maxlen=maxlen)
+        self._index: Dict[Any, T_Data] = {}
+    
+    def get(
+        self, key: Any, /, default: Optional[T_Data] = None
+    ) -> Optional[T_Data]:
+        item = self._index.get(key, default)
+        if item is not None:
+            self.move_to_end(item)
+        return item
+
+    def add(self, data: T_Data, /, *, copy: bool = False) -> None:
+        if copy:
+            data = data.model_copy()
+        if len(self._cache) == self._cache.maxlen:
+            old = self._cache[0]
+            if old.__primary_key__ is not None:
+                del self._index[old.get_primary_key()]
+        self._cache.append(data)
+        data.set_data_store(self)
+        if data.__primary_key__ is not None:
+            self._index[data.get_primary_key()] = data
+    
+    def update(self, data: T_Data) -> None:
+        self.move_to_end(data)
+    
+    def get_all(self) -> List[T_Data]:
+        return list(self._cache)
+    
+    def discard(self, data: T_Data, /) -> bool:
+        try:
+            self._cache.remove(data)
+        except ValueError:
+            return False
+        if data.__primary_key__ is not None:
+            self._index.pop(data.get_primary_key())
+        return True
+    
+    def remove(self, data: T_Data) -> None:
+        self._cache.remove(data)
+        if data.__primary_key__ is not None:
+            del self._index[data.get_primary_key()]
+    
+    def clear(self) -> None:
+        self._cache.clear()
+        self._index.clear()
+    
+    def move_to_end(self, data: T_Data, /) -> None:
+        if data not in self._cache:
+            raise ValueError("data not in store")
+        self._cache.remove(data)
+        self._cache.append(data)
+    
+    def keys(self) -> Iterable[Any]:
+        return self._index.keys()
+    
+    def values(self) -> Iterable[T_Data]:
+        return self._index.values()
+    
+    def items(self) -> Iterable[Tuple[Any, T_Data]]:
+        return self._index.items()
+
+    @property
+    def maxlen(self) -> StrictInt:
+        maxlen = self._cache.maxlen
+        assert maxlen is not None
+        return maxlen
+    
+    def __getitem__(self, __key: Any) -> T_Data:
+        item = self._index[__key]
+        self.move_to_end(item)
+        return item
+    
+    def __contains__(self, __key: Any) -> bool:
+        if isinstance(__key, DataModel):
+            if __key.__primary_key__ is not None:
+                return __key.get_primary_key() in self._index
+            else:
+                return __key in self._cache
+        return __key in self._index
+
+    def __iter__(self) -> Iterator[T_Data]:
+        return iter(self._cache)
+    
+    def __len__(self) -> StrictInt:
+        return len(self._cache)
+
+
 class AbstractAsyncCachedStore(AbstractCachedDataStore[T_Data]):
     __slots__ = ["_load_tasks", "_save_tasks", "_wait_list", "_loaded"]
 
     enable_async_backend: ClassVar[bool] = greenback is not None
 
     def __init__(
         self, name: StrictStr, *, data_type: Optional[Type[T_Data]] = None
@@ -607,14 +702,26 @@
     data_type: Optional[Type[T_Data]] = None,
     **kwds: Any,
 ) -> JsonFileStore[T_Data]: ...
 
 
 @overload
 def get_store(
+    store_type: Literal["lru"],
+    /,
+    name: str = ...,
+    maxlen: int = ...,
+    *args: Any,
+    data_type: Optional[Type[T_Data]] = None,
+    **kwds: Any,
+) -> LruStore[T_Data]: ...
+
+
+@overload
+def get_store(
     store_type: str,
     /,
     name: str = ...,
     *args: Any,
     data_type: Optional[Type[T_Data]] = None,
     **kwds: Any,
 ) -> AbstractDataStore[T_Data]: ...
```

### Comparing `KaruhaBot-0.2.0b3/karuha/text/__init__.py` & `karuhabot-0.2.0b4/karuha/text/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Provides a text representation and a converter between the two that are easier to read and use than Drafty.
 """
 
 from .drafty import Drafty, DraftyFormat, DraftyExtend
 from .textchain import *
 from .convert import drafty2tree, tree2text, drafty2text, eval_spans, to_span_tree
-from .message import Message
+from .message import Message, MessageSession, Head
 
 
 DraftyMessage = Drafty
 
 
 __all__ = [
     # drafty
@@ -41,9 +41,11 @@
     "Audio",
     "Video",
     # converter
     "drafty2tree",
     "tree2text",
     "drafty2text",
     # message
-    "Message"
+    "Message",
+    "MessageSession",
+    "Head",
 ]
```

### Comparing `KaruhaBot-0.2.0b3/karuha/text/convert.py` & `karuhabot-0.2.0b4/karuha/text/convert.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/text/drafty.py` & `karuhabot-0.2.0b4/karuha/text/drafty.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/text/textchain.py` & `karuhabot-0.2.0b4/karuha/text/textchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 import mimetypes
 import os
 import operator as op
 from abc import abstractmethod
 from base64 import b64decode, b64encode
 from typing import (Any, ClassVar, Dict, Final, Generator, List, Literal,
-                    Mapping, MutableMapping, Optional, SupportsIndex, Type,
-                    Union)
+                    MutableMapping, Optional, Sequence, SupportsIndex, Type,
+                    Union, overload)
 
 from aiofiles import open as aio_open
 from pydantic import AnyHttpUrl, BaseModel, model_validator
 from typing_extensions import Self
 
 from .drafty import Drafty, DraftyExtend, DraftyFormat, ExtendType, InlineType
 
 
 class BaseText(BaseModel):
     __slots__ = []
 
     @abstractmethod
     def to_drafty(self) -> Drafty:
         raise NotImplementedError
-    
+
     def split(self, /, sep: Optional[str] = None, maxsplit: SupportsIndex = -1) -> List["BaseText"]:
         return [self]
-    
+
     def startswith(self, /, prefix: str) -> bool:
         return str(self).startswith(prefix)
-    
+
     def endswith(self, /, suffix: str) -> bool:
         return str(self).endswith(suffix)
-    
+
     def __len__(self) -> int:
         return len(str(self))
 
+    def __contains__(self, other: Union[str, "BaseText"]) -> bool:
+        if isinstance(other, str):
+            return other in str(self)
+        return any(
+            other in i if i is not self else other == i
+            for i in self.split()
+        )
+
     def __add__(self, other: Union[str, "BaseText"]) -> "BaseText":
         if not other:
             return self
         if isinstance(other, str):
             other = PlainText(other)
         if not self:
             return other
         if not isinstance(other, TextChain) and isinstance(other, BaseText):
             return TextChain(self, other)
         return NotImplemented
-    
+
     def __radd__(self, other: str) -> "BaseText":
         if not other:
             return self
         if isinstance(other, str):
             return TextChain(PlainText(other), self)
         return NotImplemented
-    
+
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} {str(self)!r}>"
-    
+
     @abstractmethod
     def __str__(self) -> str:
         return "unknown"
 
 
 class _Text(BaseText):
     text: str
@@ -110,49 +118,68 @@
 class InlineCode(_Text):
     def to_drafty(self) -> Drafty:
         df = super().to_drafty()
         df.fmt.append(DraftyFormat(at=0, len=len(self), tp="CO"))
         return df
 
 
-class TextChain(BaseText, Mapping):
+class TextChain(BaseText, Sequence):
     contents: List[BaseText]
 
-    def __init__(self, *args: BaseText) -> None:
-        super().__init__(contents=args)  # type: ignore
+    def __init__(self, *args: Union[BaseText, str]) -> None:
+        contents = [
+            PlainText(t) if isinstance(t, str) else t
+            for t in args if t
+        ]
+        super().__init__(contents=contents)  # type: ignore
     
     def to_drafty(self) -> Drafty:
         if not self.contents:
             return Drafty(txt=" ")
         it = iter(self.contents)
         base = next(it).to_drafty()
         for i in it:
             base += i.to_drafty()
         return base
     
     def split(self, /, sep: Optional[str] = None, maxsplit: SupportsIndex = -1) -> List[BaseText]:
+        if not self:
+            return []
         maxsplit = op.index(maxsplit)
-        if maxsplit == 0:
-            return [self]
+        remain_count = maxsplit - len(self.contents) + 1
+        if maxsplit >= 0 and remain_count < 0:
+            content = self.contents[:maxsplit]
+            content.append(self[maxsplit:])
+            return content
+    
         result = []
         for i in self.contents:
-            result.extend(i.split(sep, maxsplit))
-        if maxsplit > 0 and len(result) > maxsplit + 1:
-            remain = TextChain(*result[maxsplit + 1:])
-            result = result[:maxsplit + 1]
-            result.append(remain)
+            if maxsplit >= 0 and remain_count < 0:
+                result.append(i)
+            else:
+                sp = i.split(sep, remain_count)
+                result.extend(sp)
+                remain_count -= len(sp) - 1
         return result
     
     def take(self) -> BaseText:
         if len(self.contents) == 1:
             return self.contents[0]
         return self
     
-    def __getitem__(self, key: SupportsIndex, /) -> BaseText:
-        return self.contents[key]
+    @overload
+    def __getitem__(self, key: SupportsIndex, /) -> BaseText: ...
+    @overload
+    def __getitem__(self, key: slice, /) -> "TextChain": ...
+
+    def __getitem__(self, key: Union[SupportsIndex, slice], /) -> BaseText:
+        item = self.contents[key]
+        if isinstance(item, list):
+            return TextChain(*item)
+        return item
 
     def __iter__(self) -> Generator[BaseText, None, None]:
         yield from self.contents
     
     def __len__(self) -> int:
         return len(self.contents)
```

### Comparing `KaruhaBot-0.2.0b3/karuha/utils/argparse.py` & `karuhabot-0.2.0b4/karuha/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/utils/decode.py` & `karuhabot-0.2.0b4/karuha/utils/decode.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/utils/dispatcher.py` & `karuhabot-0.2.0b4/karuha/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/karuha/utils/event_catcher.py` & `karuhabot-0.2.0b4/karuha/utils/event_catcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import asyncio
-from types import TracebackType
-from typing import Generic, Optional, Type
-from typing_extensions import Self
+from typing import Generic, Optional, Type, TypeVar
 
-from ..event import T_Event
+from ..event import Event
+from .context import _ContextHelper
 
 
-class EventCatcher(Generic[T_Event]):
+T_Event = TypeVar("T_Event", bound=Event)
+
+
+class EventCatcher(Generic[T_Event], _ContextHelper):
     __slots__ = ["event_type", "future", "events"]
 
     def __init__(self, event_type: Type[T_Event]) -> None:
         self.event_type = event_type
         self.events = []
         self.future = None
     
     def catch_event_nowait(self) -> T_Event:
         return self.events.pop()
     
     async def catch_event(self, timeout: Optional[float] = None) -> T_Event:
         if self.events:
             return self.catch_event_nowait()
-        assert self.future is None, "catcher is already waiting"
+        assert self.future is None, "catcher is already waited"
         loop = asyncio.get_running_loop()
         self.future = loop.create_future()
         try:
             return await asyncio.wait_for(self.future, timeout)
         finally:
             self.future = None
     
     @property
     def caught(self) -> bool:
         return bool(self.events)
 
+    def activate(self) -> None:
+        self.event_type.add_handler(self)
+    
+    def deactivate(self) -> None:
+        self.event_type.remove_handler(self)
+
     async def __call__(self, event: T_Event) -> None:
         if self.future:
             self.future.set_result(event)
         else:
             self.events.append(event)
-    
-    def __enter__(self) -> Self:
-        self.event_type.add_handler(self)
-        return self
-    
-    def __exit__(self, exec_type: Type[BaseException], exec_ins: BaseException, traceback: TracebackType) -> None:
-        self.event_type.remove_handler(self)
```

### Comparing `KaruhaBot-0.2.0b3/karuha/utils/proxy_propery.py` & `karuhabot-0.2.0b4/karuha/utils/proxy_propery.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/setup.py` & `karuhabot-0.2.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/tests/test_bot.py` & `karuhabot-0.2.0b4/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/tests/test_command.py` & `karuhabot-0.2.0b4/tests/test_text.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,227 +1,235 @@
-from inspect import Parameter, signature
-from typing import List, Optional, Tuple
 from unittest import TestCase
 
-from karuha.bot import Bot
-from karuha.text import BaseText, PlainText, Drafty, Message
-from karuha.command.collection import (add_sub_collection, get_collection, new_collection, remove_sub_collection,
-                                       reset_collection, set_collection,
-                                       set_collection_factory, set_prefix)
-from karuha.command.command import CommandMessage, FunctionCommand, ParamFunctionCommand
-from karuha.command.parser import (BOT_PARAM, SESSION_PARAM,
-                                   MetaParamDispatcher, ParamDispatcher, ParamParser,
-                                   ParamParserFlag, SimpleCommandParser)
-from karuha.command.session import MessageSession
-from karuha.exception import KaruhaCommandError, KaruhaParserError
-
-from .utils import bot_mock, new_test_message, new_test_command_message
-
-
-class TestCommand(TestCase):
-    def test_name_parser(self) -> None:
-        simple_parser = SimpleCommandParser(["!"])
-        message0 = new_test_message(b"!test")
-        self.assertEqual(simple_parser.parse(message0), ("test", []))
-        message1 = new_test_message(b"\"!test\"")
-        self.assertEqual(simple_parser.parse(message1), ("test", []))
-        message2 = new_test_message(b"{\"txt\": \"test\"}")
-        self.assertIsNone(simple_parser.parse(message2))
-        message3 = new_test_message(b"\"!!test test test test\"")
-        self.assertEqual(
-            simple_parser.parse(message3),
-            ("!test", [PlainText("test"), PlainText("test"), PlainText("test")])
-        )
-        message4 = new_test_message(b"\"!\"")
-        self.assertEqual(simple_parser.parse(message4), ('', []))
-        message5 = new_test_message(b"\"\"")
-        self.assertIsNone(simple_parser.parse(message5))
-    
-    def test_meta_param_dispatcher(self) -> None:
-        with MetaParamDispatcher("test", str, lambda d, x: d.name, ParamParserFlag.MESSAGE_DATA) as d:
-            self.assertAlmostEqual(
-                d.match(Parameter("test", Parameter.POSITIONAL_ONLY, annotation=str)),
-                1.4
-            )
-            self.assertAlmostEqual(
-                d.match(Parameter("test", Parameter.KEYWORD_ONLY, annotation=str, default="test")),
-                1.6
-            )
-            self.assertAlmostEqual(
-                d.match(Parameter("test", Parameter.KEYWORD_ONLY)),
-                1.2
-            )
-            self.assertAlmostEqual(
-                d.match(Parameter("test1", Parameter.KEYWORD_ONLY, annotation=str)),
-                0.4
-            )
-        self.assertAlmostEqual(
-            BOT_PARAM.match(
-                Parameter("bot", Parameter.POSITIONAL_OR_KEYWORD, annotation=Optional[Bot])
-            ), 1.5
-        )
-        self.assertAlmostEqual(
-            SESSION_PARAM.match(
-                Parameter("sess", Parameter.POSITIONAL_OR_KEYWORD, annotation=MessageSession)
-            ), 0.8
-        )
-
-        message = new_test_command_message()
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("name", Parameter.POSITIONAL_ONLY))(message),
-            "test"
-        )
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("name", Parameter.POSITIONAL_ONLY, annotation=str))(message),
-            "test"
-        )
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("argc", Parameter.POSITIONAL_ONLY))(message),
-            0
-        )
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("argv", Parameter.POSITIONAL_ONLY))(message),
-            ()
-        )
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("argv", Parameter.POSITIONAL_ONLY, annotation=list))(message),
-            []
+from karuha.text import PlainText, Form, Drafty, drafty2tree, drafty2text
+from karuha.text.textchain import File, Mention, Quote, TextChain, Bold, Hidden
+from karuha.text.convert import eval_spans, to_span_tree
+from karuha.event.message import MessageEvent
+
+from .utils import bot_mock, new_test_message
+
+
+example1 = Drafty.model_validate_json(
+    """
+{
+   "txt":  "this is bold, code and italic, strike combined bold and italic an url: https://www.example.com/abc#fragment and another www.tinode.co this is a @mention and a #hashtag in a string second #hashtag",
+   "fmt": [
+       { "at":8, "len":4,"tp":"ST" },{ "at":14, "len":4, "tp":"CO" },{ "at":23, "len":6, "tp":"EM"},
+       { "at":31, "len":6, "tp":"DL" },{ "tp":"BR", "len":1, "at":37 },{ "at":56, "len":6, "tp":"EM" },
+       { "at":47, "len":15, "tp":"ST" },{ "tp":"BR", "len":1, "at":62 },{ "at":120, "len":13, "tp":"EM" },
+       { "at":71, "len":36, "key":0 },{ "at":120, "len":13, "key":1 },{ "tp":"BR", "len":1, "at":133 },
+       { "at":144, "len":8, "key":2 },{ "at":159, "len":8, "key":3 },{ "tp":"BR", "len":1, "at":179 },
+       { "at":187, "len":8, "key":3 },{ "tp":"BR", "len":1, "at":195 }
+   ],
+   "ent": [
+       { "tp":"LN", "data":{ "url":"https://www.example.com/abc#fragment" } },
+       { "tp":"LN", "data":{ "url":"http://www.tinode.co" } },
+       { "tp":"MN", "data":{ "val":"mention" } },
+       { "tp":"HT", "data":{ "val":"hashtag" } }
+   ]
+}
+    """.strip()  # noqa: E501
+)
+
+example2 = Drafty.model_validate_json(
+    """
+{
+    "txt": "Do you agree? Yes No",
+    "fmt": [
+        {"len": 20, "tp": "FM"},
+        {"len": 13, "tp": "ST"},
+        {"at": 13, "len": 1, "tp": "BR"},
+        {"at": 14, "len": 3},
+        {"at": 17, "len": 1, "tp": "BR"},
+        {"at": 18, "len": 2, "key": 1}
+    ],
+    "ent": [
+        {"tp": "BN", "data": {"name": "yes", "act": "pub", "val": "oh yes!"}},
+        {"tp": "BN", "data": {"name": "no", "act": "pub"}}
+    ]
+}
+    """.strip()
+)
+
+
+class TestText(TestCase):
+    def test_init(self) -> None:
+        self.assertEqual(
+            example1.txt,
+            "this is bold, code and italic, strike combined bold and italic an url: "
+            "https://www.example.com/abc#fragment and another www.tinode.co this "
+            "is a @mention and a #hashtag in a string second #hashtag"
+        )
+        t = PlainText("Hello world!\n")
+        self.assertEqual(str(t), "Hello world!\n")
+        self.assertEqual(len(t), 13)
+        self.assertEqual(str(t[0]), "H")
+        self.assertEqual(str(t[1:]), "ello world!\n")
+        empty = TextChain()
+        self.assertEqual(len(empty), 0)
+        self.assertEqual(str(empty), "")
+        self.assertEqual(empty.to_drafty(), Drafty.from_str(' '))
+
+    def test_span(self) -> None:
+        spans, attachments = eval_spans(example1)
+        self.assertFalse(attachments)
+        self.assertEqual(len(spans), len(example1.fmt))
+        spans = to_span_tree(spans)
+        self.assertEqual(len(spans), len(example1.fmt) - 2)
+
+        spans = drafty2tree(example2)
+        # print(spans)
+        self.assertEqual(len(spans), 1)
+
+    def test_convert(self) -> None:
+        txt = PlainText("Hello world!\n")
+        df = txt.to_drafty()
+
+        self.assertEqual(df.txt, "Hello world! ")
+        self.assertTrue(df.fmt)
+        self.assertFalse(df.ent)
+        rtxt = drafty2text(df)
+        self.assertEqual(txt, rtxt)
+
+        tx1 = drafty2text(example1)
+        tx2 = drafty2text(example2)
+        self.assertIsInstance(tx2, Form)
+        df1 = tx1.to_drafty()
+        df2 = tx2.to_drafty()
+        self.assertEqual(df2.txt, example2.txt)
+        self.assertListEqual(df2.ent, example2.ent)
+        self.assertListEqual(df2.fmt, example2.fmt)
+        self.assertSetEqual(set(df1.fmt), set(example1.fmt))
+
+    def test_message(self) -> None:
+        message = new_test_message(b"test")
+        self.assertEqual(message.text, "test")
+        self.assertEqual(message.raw_text, "test")
+        self.assertEqual(message.content, b"test")
+
+        message = new_test_message(b"\"test\"")
+        self.assertIsInstance(message.text, PlainText)
+        self.assertEqual(message.text, PlainText("test"))
+        self.assertEqual(message.raw_text, "test")
+
+        message = new_test_message(b"{\"txt\": \"test\"}")
+        self.assertIsInstance(message.text, PlainText)
+        self.assertEqual(message.text, PlainText("test"))
+        self.assertIsInstance(message.raw_text, Drafty)
+        self.assertEqual(message.raw_text, Drafty(txt="test"))
+
+        message = new_test_message(
+            b"{\"txt\": \"test\", \"fmt\": [{\"at\": 0, \"len\": 4, \"tp\": \"ST\"}]}"
+        )
+        assert isinstance(message.text, Bold)
+        self.assertEqual(message.text.content, PlainText("test"))
+        self.assertEqual(
+            message.raw_text,
+            Drafty(txt="test", fmt=[{"at": 0, "len": 4, "tp": "ST"}])  # type: ignore
+        )
+
+        message = new_test_message(
+            b"{\"txt\": \"test\", \"fmt\": [{\"at\": 0, \"len\": -1, \"tp\": \"ST\"}]}"
+        )
+        self.assertIsInstance(message.text, str)
+        self.assertIsInstance(message.raw_text, str)
+
+        message = new_test_message(
+            b"{\"txt\": \"hello world\", \"fmt\": [{\"at\": 6, \"len\": 15, \"tp\": \"ST\"}]}"
+        )
+        assert isinstance(message.text, TextChain)
+        world = message.text[1]
+        assert isinstance(world, Bold)
+        self.assertEqual(world.content, PlainText("world"))
+        self.assertIsInstance(message.raw_text, Drafty)
+
+        message = new_test_message(
+            b"{\"txt\": \"test\", \"fmt\": [{\"at\": 0, \"len\": 4}]}"
+        )
+        assert isinstance(message.text, Hidden)
+        self.assertEqual(message.text.content, PlainText("test"))
+        self.assertIsInstance(message.raw_text, Drafty)
+
+    def test_message_event(self) -> None:
+        ev = MessageEvent(
+            bot_mock,
+            "", "", 0, {},
+            b"\"\""
+        )
+        self.assertEqual(ev.text, "")
+        self.assertEqual(ev.raw_text, "")
+        self.assertEqual(ev.content, b"\"\"")
+
+    def test_drafty_ops(self) -> None:
+        df = Drafty.from_str("Hello")
+        df = df + " world"
+        self.assertEqual(str(df), "Hello world")
+        df1 = "Hello" + Drafty.from_str(" world")
+        self.assertEqual(df, df1)
+
+    def test_file(self) -> None:
+        f = File(
+            name="test.txt",
+            raw_val=b"test"  # type: ignore
         )
-        message = CommandMessage.from_message(
-            message,
-            FunctionCommand("test", lambda: None),
-            new_collection(),
-            "test",
-            [PlainText("test")]
-        )
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("argc", Parameter.POSITIONAL_ONLY, annotation=int))(message),
-            1
-        )
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("argv", Parameter.POSITIONAL_ONLY, annotation=List[str]))(message),
-            ["test"]
-        )
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("argv", Parameter.POSITIONAL_ONLY, annotation=List[BaseText]))(message),
-            [PlainText("test")]
-        )
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("argv", Parameter.POSITIONAL_ONLY, annotation=Tuple[str, ...]))(message),
-            ("test",)
-        )
-        self.assertEqual(
-            ParamDispatcher.dispatch(Parameter("argv", Parameter.POSITIONAL_ONLY, annotation=Tuple[BaseText, ...]))(message),
-            (PlainText("test"),)
+        self.assertEqual(f.val, "dGVzdA==")
+        self.assertEqual(f.mime, "text/plain")
+        
+        df = Drafty.model_validate(
+            {
+                "ent": [
+                    {
+                        "data": {
+                            "mime": "text/plain",
+                            "name": "test.txt",
+                            "size": 4,
+                            "val": "dGVzdA==",
+                        },
+                        "tp": "EX",
+                    }
+                ],
+                "fmt": [{"at": -1}],
+            }
         )
+        f = drafty2text(df)
+        self.assertIsInstance(f, File)
     
-    def test_param_parser(self) -> None:
-        def cmd_meta(bot: Bot, message: Message, /, user_id: Optional[str], content: bytes, argv: list) -> None:
-            pass
-
-        sig = signature(cmd_meta)
-        parser = ParamParser.from_signature(sig)
-        msg = new_test_command_message()
-        args, kwargs = parser.parse(msg)
-        self.assertEqual(args, (bot_mock, msg))
-        self.assertEqual(kwargs, {"user_id": "user", "content": b"\"test\"", "argv": []})
-
-        with self.assertRaises(KaruhaParserError):
-            ParamParser.from_signature(sig, flags=ParamParserFlag.MESSAGE_DATA)
-        with self.assertRaises(KaruhaParserError):
-            ParamParser.from_signature(signature(lambda *message: ...))
-        
-        def cmd_text(text: PlainText, raw_text: Drafty) -> None:
-            pass
-
-        sig = signature(cmd_text)
-        parser = ParamParser.from_signature(sig, flags=ParamParserFlag.MESSAGE_DATA)
-        with self.assertRaises(KaruhaParserError):
-            parser.parse(new_test_command_message())
-        args, kwargs = parser.parse(new_test_command_message(b"{\"txt\": \"test\"}"))
-        self.assertEqual(args, ())
-        self.assertEqual(kwargs, {"text": PlainText("test"), "raw_text": Drafty(txt="test")})
-
-        def cmd_plain_text(text: str, raw_text: str) -> None:
-            pass
-
-        sig = signature(cmd_plain_text)
-        parser = ParamParser.from_signature(sig, flags=ParamParserFlag.MESSAGE_DATA)
-        args, kwargs = parser.parse(new_test_command_message(b"{\"txt\": \"test\"}"))
-        self.assertEqual(args, ())
-        self.assertEqual(kwargs, {"text": "test", "raw_text": "test"})
-
-        def cmd_no_annotation(text, /, raw_text, content) -> None:
-            pass
-
-        sig = signature(cmd_no_annotation)
-        parser = ParamParser.from_signature(sig, flags=ParamParserFlag.META)
-        args, kwargs = parser.parse(new_test_command_message(b"{\"txt\": \"test\"}"))
-        self.assertEqual(args, (PlainText("test"),))
-        self.assertEqual(kwargs, {"raw_text": Drafty(txt="test"), "content": b"{\"txt\": \"test\"}"})
+    def test_quote(self) -> None:
+        df = Drafty.model_validate(
+            {
+                "txt": "user quote textuser text",
+                "fmt": [
+                    {"len": 4},
+                    {"at": 4, "len": 1, "tp": "BR"},
+                    {"len": 15, "tp": "QQ"}
+                ],
+                "ent": [
+                    {"tp": "MN", "data": {"val": "user_id"}}
+                ]
+            }
+        )
+        t = drafty2text(df)
+        assert isinstance(t, TextChain)
+        self.assertEqual(len(t), 2)
+        qq = t[0]
+        assert isinstance(qq, Quote) and isinstance(qq.content, TextChain)
+        self.assertEqual(len(qq.content), 2)
+        self.assertEqual(qq.content[0], Mention(text="user", val="user_id"))
+        self.assertEqual(qq.content[1], PlainText("\nquote text"))
+        self.assertEqual(t[1], PlainText("user text"))
     
-    def test_function_command(self) -> None:
-        with new_collection() as clt:
-            called = False
-
-            with self.assertRaises(KaruhaCommandError):
-                clt["test"]
-
-            @clt.on_command("test", flags=ParamParserFlag.NONE)
-            def test(bot: Bot, /, message: Message, *, text: PlainText) -> None:
-                nonlocal called
-                called = True
-
-            self.assertIsInstance(test, FunctionCommand)
-            self.assertIs(clt["test"], test)
-            test(bot_mock, new_test_message(), text=PlainText("test"))
-            self.assertTrue(called)
-
-            with self.assertRaises(ValueError):
-                clt.add_command(test)
-            
-    def test_collection(self) -> None:
-        reset_collection()
-        set_prefix('/', '#')
-        c = new_collection()
-        self.assertFalse(c.activated)
-        self.assertIsInstance(c.name_parser, SimpleCommandParser)
-        self.assertEqual(c.name_parser.prefixs, ('/', '#'))  # type: ignore
-        cd = get_collection()
-        self.assertTrue(cd.activated)
-        self.assertNotEqual(c, cd)
-        with self.assertRaises(RuntimeError):
-            set_prefix('!')
-        
-        reset_collection()
-        set_prefix('/')
-        set_collection_factory(lambda: c)
-
-        @self.addCleanup
-        def cleanup() -> None:
-            reset_collection()
-            set_collection_factory(None)
-
-        self.assertIs(get_collection(), c)
-        with self.assertRaises(RuntimeError):
-            set_collection_factory(lambda: c)
-        set_collection(cd)
-        self.assertIs(get_collection(), cd)
-        set_collection_factory(lambda: c, reset=True)
-        self.assertIs(get_collection(), c)
-
-    def test_sub_collection(self) -> None:
-        reset_collection()
-        c = new_collection()
-        c.add_command(ParamFunctionCommand.from_function(lambda bot: ..., name="test"))
-
-        cd = get_collection()
-        cd.sub_collections.append(c)
-        with self.assertRaises(KeyError):
-            remove_sub_collection(c)
-        self.assertIsNotNone(cd.get_command("test"))
-
-        add_sub_collection(c)
-        reset_collection()
-        cd1 = get_collection()
-        self.assertIsNot(cd, cd1)
-        self.assertEqual(cd1.sub_collections, [c])
+    def test_split(self) -> None:
+        txt = PlainText("Hello world! Hello world!")
+        self.assertEqual([str(i) for i in txt.split(maxsplit=1)], "Hello world! Hello world!".split(maxsplit=1))
+        tc = TextChain(*txt.split(maxsplit=2))
+        self.assertEqual(len(tc), 3)
+        self.assertEqual(tc[2], "Hello world!")
+        self.assertEqual(tc.split(), txt.split())
+        self.assertEqual(tc.split(maxsplit=2), txt.split(maxsplit=2))
+        sp = tc.split(maxsplit=1)
+        self.assertEqual(len(sp), 2)
+        self.assertEqual(sp[0], "Hello")
+        self.assertEqual(sp[1], TextChain("world!", "Hello world!"))
+
+        tc = TextChain("Hello world!", "Hello world!")
+        self.assertEqual(tc.split(), ["Hello", "world!", "Hello", "world!"])
+        self.assertEqual(tc.split(maxsplit=2), ["Hello", "world!", "Hello world!"])
```

### Comparing `KaruhaBot-0.2.0b3/tests/test_command_run.py` & `karuhabot-0.2.0b4/tests/test_command_run.py`

 * *Files identical despite different names*

### Comparing `KaruhaBot-0.2.0b3/tests/test_data.py` & `karuhabot-0.2.0b4/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from pydantic_core import to_json
 from tinode_grpc import pb
 
-from karuha.data.cache import UserCache, clear_meta_cache, get_user_cred, get_user_tags, update_user_cache, user_cache
+from karuha.data.cache import UserCache, clear_cache, get_user_cred, get_user_tags, update_user_cache, user_cache
 from karuha.data.meta import AccessPermission, BaseDesc, Cred, UserDesc
 from karuha.data.topic import BaseTopic, Topic, TopicSub, get_topic, get_topic_list
 from karuha.data.user import BaseUser, User, get_user
 
 from .utils import AsyncBotTestCase
 
 
@@ -103,15 +103,15 @@
         self.assertIsInstance(user, User)
         self.assertIsNone(user.fn)
         self.assertEqual(user.note, "test note")
         self.assertTrue(user.staff)
         self.assertFalse(user.verified)
 
     async def test_me_sub_meta(self) -> None:
-        clear_meta_cache()
+        clear_cache()
         task = asyncio.create_task(get_topic_list(self.bot, ensure_topic_sub=True))
         get_msg = await self.bot.consum_message()
         assert get_msg.get
         get_msg = get_msg.get
         meta = pb.ServerMeta(
             id=get_msg.id,
             topic="me",
@@ -220,15 +220,15 @@
             )]
         )
         self.bot.receive_message(pb.ServerMsg(meta=meta))
         cred = await self.wait_for(task)
         self.assertEqual(cred, [Cred(method="email", value="test@example.com")])
     
     async def test_p2p_meta(self) -> None:
-        clear_meta_cache()
+        clear_cache()
         task = asyncio.create_task(get_topic(self.bot, "usr_test_1", ensure_topic=True))
         sub_msg = await self.bot.consum_message()
         assert sub_msg.HasField("sub") and sub_msg.sub.topic == "usr_test_1"
         self.bot.confirm_message()
 
         get_msg = await self.bot.consum_message()
         assert get_msg.HasField("get")
@@ -260,15 +260,15 @@
         assert topic.acs
         self.assertEqual(
             topic.acs.want,
             AccessPermission(join=True, read=True, write=True, presence=True, approve=True)
         )
     
     async def test_topic_meta(self) -> None:
-        clear_meta_cache()
+        clear_cache()
         task = asyncio.create_task(get_topic(self.bot, "grp_test_1", ensure_topic=True))
         sub_msg = await self.bot.consum_message()
         assert sub_msg.HasField("sub") and sub_msg.sub.topic == "grp_test_1"
         self.bot.confirm_message()
 
         get_msg = await self.bot.consum_message()
         assert get_msg.HasField("get")
```

### Comparing `KaruhaBot-0.2.0b3/tests/test_session.py` & `karuhabot-0.2.0b4/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,16 @@
         pubmsg = msg.pub
         self.bot.confirm_message(pubmsg.id, seq=114)
         self.bot.receive_content(
             b'{"ent":[{"data":{"mime":"application/json","val":{"resp":{"yes":1},"seq":114}},'
             b'"tp":"EX"}],"fmt":[{"at":-1}],"txt":"Yes"}',
         )
         bid = await asyncio.wait_for(form_task, timeout=TEST_TIMEOUT)
+        async with get_message_lock():
+            pass
         self.assertEqual(bid, 0)
 
     async def test_form1(self) -> None:
         ss = MessageSession(self.bot, new_test_message())
         form_task = asyncio.create_task(
             ss.send_form(
                 "title", "Yes", Button(text="No"), Button(text="Cancel", name="cancel")
```

### Comparing `KaruhaBot-0.2.0b3/tests/test_store.py` & `karuhabot-0.2.0b4/tests/test_store.py`

 * *Files 20% similar despite different names*

```diff
@@ -97,14 +97,36 @@
         self.assertEqual(list(store.get_all()), [])
         self.assertNotIn(data1, store)
 
         self.assertFalse(store.discard(data))
         self.assertFalse(store.discard(data1))
         self.assertFalse(store)
 
+    def test_lru_store(self) -> None:
+        store = get_store("lru", maxlen=3, data_type=DataPk1)
+        store.add(DataPk1(pk1="test1", content="test1"))
+        store.add(DataPk1(pk1="test2", content="test2"))
+        store.add(DataPk1(pk1="test3", content="test3"))
+        self.assertEqual([d.content for d in store.get_all()], ["test1", "test2", "test3"])
+        store.add(DataPk1(pk1="test4", content="test4"))
+        self.assertEqual([d.content for d in store.get_all()], ["test2", "test3", "test4"])
+        t2 = store["test2"]
+        self.assertEqual([d.content for d in store.get_all()], ["test3", "test4", "test2"])
+        with self.assertRaises(KeyError):
+            store["test1"]
+        store.remove(store["test3"])
+        self.assertEqual([d.content for d in store.get_all()], ["test4", "test2"])
+        store.add(DataPk1(pk1="test5", content="test5"))
+        self.assertEqual([d.content for d in store.get_all()], ["test4", "test2", "test5"])
+        t2.content = "test2_new"
+        self.assertEqual([d.content for d in store.get_all()], ["test4", "test5", "test2_new"])
+        self.assertTrue(store.discard(t2))
+        self.assertEqual([d.content for d in store.get_all()], ["test4", "test5"])
+        self.assertFalse(store.discard(t2))
+
     async def test_json_store(self) -> None:
         await greenback.ensure_portal()
         store = get_store("json", data_type=DataPk1)
         self.assertIsInstance(store, JsonFileStore)
         self.assertIs(store, get_store("json", data_type=DataPk1))
         self.assertTrue(store.async_backend_available())
         store.clear()
```

### Comparing `KaruhaBot-0.2.0b3/tests/utils.py` & `karuhabot-0.2.0b4/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 from karuha import async_run, try_add_bot
 from karuha.bot import Bot, State
 from karuha.command.collection import new_collection
 from karuha.command.command import CommandMessage, FunctionCommand
 from karuha.config import Server as ServerConfig
 from karuha.config import init_config
-from karuha.event import T_Event
 from karuha.store import T
 from karuha.text.message import Message
+from karuha.utils.event_catcher import T_Event
 from karuha.utils.event_catcher import EventCatcher as _EventCatcher
 
 
 TEST_TIMEOUT = 3
 
 
 @coroutine
@@ -185,14 +185,15 @@
                 await run_forever()
     
     def _get_channel(self, server_config: ServerConfig) -> grpc_aio.Channel:
         return NoopChannel()
 
 
 bot_mock = BotMock("test", "basic", "123456", log_level="DEBUG")
+bot_mock.user_id = "usr"
 
 
 class EventCatcher(_EventCatcher[T_Event]):
     __slots__ = []
 
     async def catch_event(self, timeout: float = TEST_TIMEOUT) -> T_Event:
         return await super().catch_event(timeout)
```


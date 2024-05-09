# Comparing `tmp/webchecks-0.1.tar.gz` & `tmp/webchecks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webchecks-0.1.tar", last modified: Sat Apr 27 20:54:07 2024, max compression
+gzip compressed data, was "webchecks-0.1.1.tar", last modified: Thu May  9 16:36:49 2024, max compression
```

## Comparing `webchecks-0.1.tar` & `webchecks-0.1.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 online    (1001) online    (1001)        0 2024-04-27 20:54:07.320589 webchecks-0.1/
--rw-rw-r--   0 online    (1001) online    (1001)     1523 2024-03-15 13:38:15.000000 webchecks-0.1/LICENSE
--rw-rw-r--   0 online    (1001) online    (1001)       35 2024-04-27 20:27:20.000000 webchecks-0.1/MANIFEST.in
--rw-r--r--   0 online    (1001) online    (1001)     8854 2024-04-27 20:54:07.320589 webchecks-0.1/PKG-INFO
--rw-rw-r--   0 online    (1001) online    (1001)     6275 2024-04-27 20:53:35.000000 webchecks-0.1/README.md
--rw-rw-r--   0 online    (1001) online    (1001)     8172 2024-03-30 16:33:58.000000 webchecks-0.1/TUTORIAL.md
--rw-rw-r--   0 online    (1001) online    (1001)      891 2024-04-27 20:51:20.000000 webchecks-0.1/pyproject.toml
--rw-rw-r--   0 online    (1001) online    (1001)       38 2024-04-27 20:54:07.320589 webchecks-0.1/setup.cfg
--rw-rw-r--   0 online    (1001) online    (1001)      236 2024-03-15 13:30:05.000000 webchecks-0.1/setup.py
-drwxrwxr-x   0 online    (1001) online    (1001)        0 2024-04-27 20:54:07.312589 webchecks-0.1/test/
--rw-rw-r--   0 online    (1001) online    (1001)        0 2023-04-02 15:07:20.000000 webchecks-0.1/test/__init__.py
--rw-rw-r--   0 online    (1001) online    (1001)     3555 2024-03-30 16:03:06.000000 webchecks-0.1/test/test_access.py
--rw-rw-r--   0 online    (1001) online    (1001)     2209 2024-03-30 15:09:27.000000 webchecks-0.1/test/test_baseprofile.py
--rw-rw-r--   0 online    (1001) online    (1001)     4244 2024-03-30 16:02:27.000000 webchecks-0.1/test/test_dryrun_project.py
--rw-rw-r--   0 online    (1001) online    (1001)     4558 2024-03-30 12:04:21.000000 webchecks-0.1/test/test_file_ops.py
--rw-rw-r--   0 online    (1001) online    (1001)     2266 2024-03-30 16:03:46.000000 webchecks-0.1/test/test_globalcache.py
--rw-rw-r--   0 online    (1001) online    (1001)     2745 2024-03-30 07:38:22.000000 webchecks-0.1/test/test_queue.py
--rw-rw-r--   0 online    (1001) online    (1001)    12720 2024-03-30 10:41:47.000000 webchecks-0.1/test/test_security.py
--rw-rw-r--   0 online    (1001) online    (1001)      929 2024-03-30 07:16:49.000000 webchecks-0.1/test/test_singleton.py
--rw-rw-r--   0 online    (1001) online    (1001)    10296 2024-03-30 15:46:00.000000 webchecks-0.1/test/test_url.py
-drwxrwxr-x   0 online    (1001) online    (1001)        0 2024-04-27 20:54:07.312589 webchecks-0.1/webchecks/
--rw-rw-r--   0 online    (1001) online    (1001)    15056 2024-03-30 16:07:48.000000 webchecks-0.1/webchecks/Project.py
--rw-rw-r--   0 online    (1001) online    (1001)     1213 2024-03-29 19:53:52.000000 webchecks-0.1/webchecks/__init__.py
-drwxrwxr-x   0 online    (1001) online    (1001)        0 2024-04-27 20:54:07.312589 webchecks-0.1/webchecks/access/
--rw-rw-r--   0 online    (1001) online    (1001)     3194 2024-03-30 14:27:47.000000 webchecks-0.1/webchecks/access/AccessHead.py
--rw-rw-r--   0 online    (1001) online    (1001)     6601 2024-03-30 14:24:43.000000 webchecks-0.1/webchecks/access/Gateway.py
--rw-rw-r--   0 online    (1001) online    (1001)     9837 2024-03-30 14:25:11.000000 webchecks-0.1/webchecks/access/RequestJS.py
--rw-rw-r--   0 online    (1001) online    (1001)     2700 2024-03-30 14:25:25.000000 webchecks-0.1/webchecks/access/RequestNoJS.py
--rw-rw-r--   0 online    (1001) online    (1001)     6033 2024-03-30 00:44:55.000000 webchecks-0.1/webchecks/access/RobotsFile.py
--rw-rw-r--   0 online    (1001) online    (1001)        0 2023-04-29 18:11:21.000000 webchecks-0.1/webchecks/access/__init__.py
--rw-rw-r--   0 online    (1001) online    (1001)     3718 2024-03-30 10:29:20.000000 webchecks-0.1/webchecks/access/security.py
-drwxrwxr-x   0 online    (1001) online    (1001)        0 2024-04-27 20:54:07.312589 webchecks-0.1/webchecks/archive/
--rw-rw-r--   0 online    (1001) online    (1001)     1996 2024-03-30 00:30:56.000000 webchecks-0.1/webchecks/archive/AccessNode.py
--rw-rw-r--   0 online    (1001) online    (1001)     9352 2024-03-30 16:06:10.000000 webchecks-0.1/webchecks/archive/FileArchive.py
--rw-rw-r--   0 online    (1001) online    (1001)     5980 2024-03-30 15:11:40.000000 webchecks-0.1/webchecks/archive/GlobalCache.py
--rw-rw-r--   0 online    (1001) online    (1001)        0 2023-04-02 15:07:20.000000 webchecks-0.1/webchecks/archive/__init__.py
--rw-rw-r--   0 online    (1001) online    (1001)     2195 2024-03-30 00:58:27.000000 webchecks-0.1/webchecks/config.py
-drwxrwxr-x   0 online    (1001) online    (1001)        0 2024-04-27 20:54:07.316589 webchecks-0.1/webchecks/monitor/
--rw-rw-r--   0 online    (1001) online    (1001)     1241 2024-03-30 15:32:01.000000 webchecks-0.1/webchecks/monitor/KeywordFinder.py
--rw-rw-r--   0 online    (1001) online    (1001)     4133 2024-03-30 14:26:19.000000 webchecks-0.1/webchecks/monitor/Report.py
--rw-rw-r--   0 online    (1001) online    (1001)        0 2023-09-12 14:49:41.000000 webchecks-0.1/webchecks/monitor/__init__.py
-drwxrwxr-x   0 online    (1001) online    (1001)        0 2024-04-27 20:54:07.316589 webchecks-0.1/webchecks/profiles/
--rw-rw-r--   0 online    (1001) online    (1001)    11257 2024-03-30 16:01:07.000000 webchecks-0.1/webchecks/profiles/BaseProfile.py
--rw-rw-r--   0 online    (1001) online    (1001)      192 2024-03-30 00:28:22.000000 webchecks-0.1/webchecks/profiles/ProfileConstants.py
--rw-rw-r--   0 online    (1001) online    (1001)        0 2023-04-29 18:11:21.000000 webchecks-0.1/webchecks/profiles/__init__.py
--rw-rw-r--   0 online    (1001) online    (1001)      789 2024-03-30 00:28:43.000000 webchecks-0.1/webchecks/profiles/profileDB.py
-drwxrwxr-x   0 online    (1001) online    (1001)        0 2024-04-27 20:54:07.316589 webchecks-0.1/webchecks/utils/
--rw-rw-r--   0 online    (1001) online    (1001)      544 2024-03-30 14:30:00.000000 webchecks-0.1/webchecks/utils/Error.py
--rw-rw-r--   0 online    (1001) online    (1001)      318 2024-03-30 00:34:10.000000 webchecks-0.1/webchecks/utils/OptionsError.py
--rw-rw-r--   0 online    (1001) online    (1001)        0 2023-09-03 18:37:42.000000 webchecks-0.1/webchecks/utils/__init__.py
--rw-rw-r--   0 online    (1001) online    (1001)      295 2024-03-30 01:02:01.000000 webchecks-0.1/webchecks/utils/check.py
--rw-rw-r--   0 online    (1001) online    (1001)     1873 2024-03-30 00:34:21.000000 webchecks-0.1/webchecks/utils/constants.py
--rw-rw-r--   0 online    (1001) online    (1001)     4386 2024-03-30 11:53:36.000000 webchecks-0.1/webchecks/utils/file_ops.py
--rw-rw-r--   0 online    (1001) online    (1001)     2484 2024-03-30 00:47:10.000000 webchecks-0.1/webchecks/utils/messaging.py
--rw-rw-r--   0 online    (1001) online    (1001)      303 2024-03-30 00:25:36.000000 webchecks-0.1/webchecks/utils/singleton.py
--rw-rw-r--   0 online    (1001) online    (1001)     2972 2024-03-30 00:26:19.000000 webchecks-0.1/webchecks/utils/timedqueue.py
--rw-rw-r--   0 online    (1001) online    (1001)     7090 2024-03-30 10:58:12.000000 webchecks-0.1/webchecks/utils/url.py
-drwxrwxr-x   0 online    (1001) online    (1001)        0 2024-04-27 20:54:07.316589 webchecks-0.1/webchecks.egg-info/
--rw-r--r--   0 online    (1001) online    (1001)     8854 2024-04-27 20:54:07.000000 webchecks-0.1/webchecks.egg-info/PKG-INFO
--rw-rw-r--   0 online    (1001) online    (1001)     1355 2024-04-27 20:54:07.000000 webchecks-0.1/webchecks.egg-info/SOURCES.txt
--rw-rw-r--   0 online    (1001) online    (1001)        1 2024-04-27 20:54:07.000000 webchecks-0.1/webchecks.egg-info/dependency_links.txt
--rw-rw-r--   0 online    (1001) online    (1001)      175 2024-04-27 20:54:07.000000 webchecks-0.1/webchecks.egg-info/requires.txt
--rw-rw-r--   0 online    (1001) online    (1001)       15 2024-04-27 20:54:07.000000 webchecks-0.1/webchecks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-09 16:36:37.000000 webchecks-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 16:36:37.000000 webchecks-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-05-09 16:36:49.127711 webchecks-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-09 16:36:37.000000 webchecks-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-09 16:36:37.000000 webchecks-0.1.1/TUTORIAL.md
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-09 16:36:37.000000 webchecks-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:36:49.127711 webchecks-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-09 16:36:37.000000 webchecks-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.123711 webchecks-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_baseprofile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_dryrun_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_globalcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-05-09 16:36:37.000000 webchecks-0.1.1/test/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.123711 webchecks-0.1.1/webchecks/
+-rw-r--r--   0 runner    (1001) docker     (127)    15056 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/Project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.123711 webchecks-0.1.1/webchecks/access/
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/AccessHead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/Gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/RequestJS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/RequestNoJS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/RobotsFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/access/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/archive/AccessNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/archive/FileArchive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/archive/GlobalCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/monitor/KeywordFinder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/monitor/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    11257 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/profiles/BaseProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/profiles/ProfileConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/profiles/profileDB.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/Error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/OptionsError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/messaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/timedqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-05-09 16:36:37.000000 webchecks-0.1.1/webchecks/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:36:49.127711 webchecks-0.1.1/webchecks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 16:36:49.000000 webchecks-0.1.1/webchecks.egg-info/top_level.txt
```

### Comparing `webchecks-0.1/LICENSE` & `webchecks-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/PKG-INFO` & `webchecks-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webchecks
-Version: 0.1
+Version: 0.1.1
 Summary:  WebChecks is a BSD-licensed web search and research tool in Python traversing a given set of domains. 
 Author: CopperEagle
 License: Copyright (c) WebChecks developers.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -42,15 +42,15 @@
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: bs4==0.0.1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: selenium==4.12.0
 Requires-Dist: selenium-wire==5.1.0
 Requires-Dist: typing_extensions==4.7.1
-Requires-Dist: urllib3==2.0.4
+Requires-Dist: urllib3==2.0.7
 Requires-Dist: webdriver-manager==4.0.0
 
 # WebChecks
 
 [![Python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 ![Version](https://img.shields.io/badge/Webchecks_version-0.1-darkgreen)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
@@ -120,15 +120,15 @@
 ```
 
 Note: If you require Javascript then make sure you have Firefox because this is what is being used currently by this project.
 
 ## How to use it
 
 Basic use is fairly straight forward. *ALMOST ALL* calls the user performs is using the Project class.
-For more examples and how to programmatically access the results, enable compression, using profiles, etc. check out ![the tutorial](TUTORIAL.md).
+For more examples and how to programmatically access the results, enable compression, using profiles, etc. check out [the tutorial](TUTORIAL.md).
 
 ```python
 from webchecks import Project
 
 # Give name and starting address. The latter may be a list of URLs.
 proj = Project("project_name", "mywebsite.com/coolsite.html")
```

### Comparing `webchecks-0.1/README.md` & `webchecks-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 ```
 
 Note: If you require Javascript then make sure you have Firefox because this is what is being used currently by this project.
 
 ## How to use it
 
 Basic use is fairly straight forward. *ALMOST ALL* calls the user performs is using the Project class.
-For more examples and how to programmatically access the results, enable compression, using profiles, etc. check out ![the tutorial](TUTORIAL.md).
+For more examples and how to programmatically access the results, enable compression, using profiles, etc. check out [the tutorial](TUTORIAL.md).
 
 ```python
 from webchecks import Project
 
 # Give name and starting address. The latter may be a list of URLs.
 proj = Project("project_name", "mywebsite.com/coolsite.html")
```

### Comparing `webchecks-0.1/TUTORIAL.md` & `webchecks-0.1.1/TUTORIAL.md`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/pyproject.toml` & `webchecks-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webchecks"
-version = "0.1"
+version = "0.1.1"
 description = " WebChecks is a BSD-licensed web search and research tool in Python traversing a given set of domains. "
 readme = "README.md"
 authors = [{ name = "CopperEagle" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
@@ -19,15 +19,15 @@
     "beautifulsoup4==4.12.2",
 	"bs4==0.0.1",
 	"python-dotenv==1.0.0",
 	"requests==2.31.0",
 	"selenium==4.12.0",
 	"selenium-wire==5.1.0",
 	"typing_extensions==4.7.1",
-	"urllib3==2.0.4",
+	"urllib3==2.0.7",
 	"webdriver-manager==4.0.0",
 ]
 requires-python = ">=3.9"
 
 
 [project.urls]
 Homepage = "https://github.com/CopperEagle/WebChecks"
```

### Comparing `webchecks-0.1/test/test_access.py` & `webchecks-0.1.1/test/test_access.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/test/test_baseprofile.py` & `webchecks-0.1.1/test/test_baseprofile.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/test/test_dryrun_project.py` & `webchecks-0.1.1/test/test_dryrun_project.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/test/test_file_ops.py` & `webchecks-0.1.1/test/test_file_ops.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/test/test_globalcache.py` & `webchecks-0.1.1/test/test_globalcache.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/test/test_queue.py` & `webchecks-0.1.1/test/test_queue.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/test/test_security.py` & `webchecks-0.1.1/test/test_security.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/test/test_singleton.py` & `webchecks-0.1.1/test/test_singleton.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/test/test_url.py` & `webchecks-0.1.1/test/test_url.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/Project.py` & `webchecks-0.1.1/webchecks/Project.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/__init__.py` & `webchecks-0.1.1/webchecks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 """
 
 
 from .Project import Project
 from .profiles.BaseProfile import BaseProfile
 
 
-__version__ = "0.1"
+__version__ = "0.1.1"
```

### Comparing `webchecks-0.1/webchecks/access/AccessHead.py` & `webchecks-0.1.1/webchecks/access/AccessHead.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/access/Gateway.py` & `webchecks-0.1.1/webchecks/access/Gateway.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/access/RequestJS.py` & `webchecks-0.1.1/webchecks/access/RequestJS.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/access/RequestNoJS.py` & `webchecks-0.1.1/webchecks/access/RequestNoJS.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/access/RobotsFile.py` & `webchecks-0.1.1/webchecks/access/RobotsFile.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/access/security.py` & `webchecks-0.1.1/webchecks/access/security.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/archive/AccessNode.py` & `webchecks-0.1.1/webchecks/archive/AccessNode.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/archive/FileArchive.py` & `webchecks-0.1.1/webchecks/archive/FileArchive.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/archive/GlobalCache.py` & `webchecks-0.1.1/webchecks/archive/GlobalCache.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/config.py` & `webchecks-0.1.1/webchecks/config.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/monitor/KeywordFinder.py` & `webchecks-0.1.1/webchecks/monitor/KeywordFinder.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/monitor/Report.py` & `webchecks-0.1.1/webchecks/monitor/Report.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/profiles/BaseProfile.py` & `webchecks-0.1.1/webchecks/profiles/BaseProfile.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/profiles/profileDB.py` & `webchecks-0.1.1/webchecks/profiles/profileDB.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/utils/Error.py` & `webchecks-0.1.1/webchecks/utils/Error.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/utils/constants.py` & `webchecks-0.1.1/webchecks/utils/constants.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/utils/file_ops.py` & `webchecks-0.1.1/webchecks/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/utils/messaging.py` & `webchecks-0.1.1/webchecks/utils/messaging.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/utils/timedqueue.py` & `webchecks-0.1.1/webchecks/utils/timedqueue.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks/utils/url.py` & `webchecks-0.1.1/webchecks/utils/url.py`

 * *Files identical despite different names*

### Comparing `webchecks-0.1/webchecks.egg-info/PKG-INFO` & `webchecks-0.1.1/webchecks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webchecks
-Version: 0.1
+Version: 0.1.1
 Summary:  WebChecks is a BSD-licensed web search and research tool in Python traversing a given set of domains. 
 Author: CopperEagle
 License: Copyright (c) WebChecks developers.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
@@ -42,15 +42,15 @@
 Requires-Dist: beautifulsoup4==4.12.2
 Requires-Dist: bs4==0.0.1
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: requests==2.31.0
 Requires-Dist: selenium==4.12.0
 Requires-Dist: selenium-wire==5.1.0
 Requires-Dist: typing_extensions==4.7.1
-Requires-Dist: urllib3==2.0.4
+Requires-Dist: urllib3==2.0.7
 Requires-Dist: webdriver-manager==4.0.0
 
 # WebChecks
 
 [![Python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=white)](https://www.python.org)
 ![Version](https://img.shields.io/badge/Webchecks_version-0.1-darkgreen)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
@@ -120,15 +120,15 @@
 ```
 
 Note: If you require Javascript then make sure you have Firefox because this is what is being used currently by this project.
 
 ## How to use it
 
 Basic use is fairly straight forward. *ALMOST ALL* calls the user performs is using the Project class.
-For more examples and how to programmatically access the results, enable compression, using profiles, etc. check out ![the tutorial](TUTORIAL.md).
+For more examples and how to programmatically access the results, enable compression, using profiles, etc. check out [the tutorial](TUTORIAL.md).
 
 ```python
 from webchecks import Project
 
 # Give name and starting address. The latter may be a list of URLs.
 proj = Project("project_name", "mywebsite.com/coolsite.html")
```

### Comparing `webchecks-0.1/webchecks.egg-info/SOURCES.txt` & `webchecks-0.1.1/webchecks.egg-info/SOURCES.txt`

 * *Files identical despite different names*


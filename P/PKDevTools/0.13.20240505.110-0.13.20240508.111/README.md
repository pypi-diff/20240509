# Comparing `tmp/PKDevTools-0.13.20240505.110.tar.gz` & `tmp/PKDevTools-0.13.20240508.111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240505.110.tar", last modified: Sun May  5 06:13:58 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240508.111.tar", last modified: Wed May  8 23:03:16 2024, max compression
```

## Comparing `PKDevTools-0.13.20240505.110.tar` & `PKDevTools-0.13.20240508.111.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 06:13:58.337943 PKDevTools-0.13.20240505.110/
--rw-rw-rw-   0        0        0     1086 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-05 06:13:58.322325 PKDevTools-0.13.20240505.110/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:13:58.337943 PKDevTools-0.13.20240505.110/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6376 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2534 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    14378 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5081 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    10828 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-05 06:13:51.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-05-05 06:13:58.322325 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-05 06:13:49.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-05 06:13:58.000000 PKDevTools-0.13.20240505.110/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-05-05 06:13:58.337943 PKDevTools-0.13.20240505.110/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/README.md
--rw-rw-rw-   0        0        0       86 2024-05-05 06:13:58.337943 PKDevTools-0.13.20240505.110/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-05-05 06:12:52.000000 PKDevTools-0.13.20240505.110/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 23:03:16.181588 PKDevTools-0.13.20240508.111/
+-rw-rw-rw-   0        0        0     1086 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-08 23:03:16.165962 PKDevTools-0.13.20240508.111/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-08 23:03:16.181588 PKDevTools-0.13.20240508.111/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6376 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2534 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    14378 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5081 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    10868 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-08 23:03:10.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-05-08 23:03:16.181588 PKDevTools-0.13.20240508.111/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-05-08 23:03:16.000000 PKDevTools-0.13.20240508.111/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2024-05-08 23:03:16.000000 PKDevTools-0.13.20240508.111/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 23:03:16.000000 PKDevTools-0.13.20240508.111/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-05-08 23:03:16.000000 PKDevTools-0.13.20240508.111/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-08 23:03:09.000000 PKDevTools-0.13.20240508.111/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-05-08 23:03:16.000000 PKDevTools-0.13.20240508.111/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-08 23:03:16.000000 PKDevTools-0.13.20240508.111/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-05-08 23:03:16.181588 PKDevTools-0.13.20240508.111/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-08 23:03:16.197212 PKDevTools-0.13.20240508.111/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-05-08 23:02:21.000000 PKDevTools-0.13.20240508.111/setup.py
```

### Comparing `PKDevTools-0.13.20240505.110/LICENSE` & `PKDevTools-0.13.20240508.111/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/__init__.py` & `PKDevTools-0.13.20240508.111/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         self.logLevel = defaultLogger.level
 
         self.keyboardInterruptEvent = keyboardInterruptEvent
         self.stockList = stockList
         self.dataCallbackHandler = dataCallbackHandler
         self.progressCallbackHandler = progressCallbackHandler
         self.fetcher = fetcher
+        self.intradayNSEFetcher = None
         self.configManager = configManager
         self.candlePatterns = candlePatterns
         self.screener = screener
         self.refreshDatabase = True
 
     def _setupLogger(self):
         # create the logger to use.
```

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240508.111/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240508.111/PKDevTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240505.110
+Version: 0.13.20240508.111
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240505.110.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240508.111.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240505.110/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240508.111/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/PKG-INFO` & `PKDevTools-0.13.20240508.111/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240505.110
+Version: 0.13.20240508.111
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240505.110.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240508.111.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240505.110/README.md` & `PKDevTools-0.13.20240508.111/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240505.110/setup.py` & `PKDevTools-0.13.20240508.111/setup.py`

 * *Files identical despite different names*


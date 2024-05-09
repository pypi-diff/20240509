# Comparing `tmp/rcsb_utils_struct-0.46.tar.gz` & `tmp/rcsb_utils_struct-0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb_utils_struct-0.46.tar", last modified: Wed Apr 24 17:47:00 2024, max compression
+gzip compressed data, was "rcsb_utils_struct-0.47.tar", last modified: Thu May  9 12:58:08 2024, max compression
```

## Comparing `rcsb_utils_struct-0.46.tar` & `rcsb_utils_struct-0.47.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/
--rw-r--r--   0 vsts      (1001) docker     (127)     2730 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      111 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1006 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.868362 rcsb_utils_struct-0.46/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.868362 rcsb_utils_struct-0.46/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/rcsb/utils/struct/
--rw-r--r--   0 vsts      (1001) docker     (127)    13214 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/CathClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15694 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/EcodClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3191 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/EntryInfoProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21605 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/Scop2ClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16717 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/ScopClassificationProvider.py
--rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/rcsb/utils/struct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      623 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 17:45:33.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-24 17:47:00.000000 rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-24 17:47:00.872362 rcsb_utils_struct-0.46/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2325 2024-04-24 17:44:41.000000 rcsb_utils_struct-0.46/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 12:58:08.746850 rcsb_utils_struct-0.47/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2808 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    11357 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      111 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-05-09 12:58:08.746850 rcsb_utils_struct-0.47/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1006 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 12:58:08.742850 rcsb_utils_struct-0.47/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 12:58:08.742850 rcsb_utils_struct-0.47/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 12:58:08.746850 rcsb_utils_struct-0.47/rcsb/utils/struct/
+-rw-r--r--   0 vsts      (1001) docker     (127)    13214 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/rcsb/utils/struct/CathClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15694 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/rcsb/utils/struct/EcodClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3191 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/rcsb/utils/struct/EntryInfoProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22122 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/rcsb/utils/struct/Scop2ClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16717 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/rcsb/utils/struct/ScopClassificationProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/rcsb/utils/struct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 12:58:08.746850 rcsb_utils_struct-0.47/rcsb.utils.struct.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1926 2024-05-09 12:58:08.000000 rcsb_utils_struct-0.47/rcsb.utils.struct.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      623 2024-05-09 12:58:08.000000 rcsb_utils_struct-0.47/rcsb.utils.struct.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 12:58:08.000000 rcsb_utils_struct-0.47/rcsb.utils.struct.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 12:57:00.000000 rcsb_utils_struct-0.47/rcsb.utils.struct.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-05-09 12:58:08.000000 rcsb_utils_struct-0.47/rcsb.utils.struct.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-05-09 12:58:08.000000 rcsb_utils_struct-0.47/rcsb.utils.struct.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-09 12:58:08.746850 rcsb_utils_struct-0.47/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2325 2024-05-09 12:56:15.000000 rcsb_utils_struct-0.47/setup.py
```

### Comparing `rcsb_utils_struct-0.46/HISTORY.txt` & `rcsb_utils_struct-0.47/HISTORY.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,8 +32,9 @@
  23-Sep-2021    V0.39 Update SCOP version and path details
  16-Nov-2021    V0.40 Append additional ECOD annotations for given entryId and chainId instead of overwriting
  24-Feb-2022    V0.41 Resolve duplication issues with Scop2 tree node list, and fix parent ID lists for nodes with multiple parents
   9-Mar-2022    V0.42 Fix issue related to V0.41 update to Scop2 provider
   6-Jan-2023    V0.43 Configuration changes to support tox 4
  18-Apr-2023    V0.44 Fix Ecod and Scop2 provider fall-back file import
  18-Jul-2023    V0.45 Resolve duplication issues with Scop2 families and CATH residue range lists
- 24-Apr-2024    V0.46 Turn off fetching of source SCOP2/SCOP2B data following shutdown of host website; rely on latest fallback instead
+ 24-Apr-2024    V0.46 Turn off fetching of source SCOP2/SCOP2B data following shutdown of host website; rely on latest fallback instead
+  9-May-2024    V0.47 Tweak to above update (V0.46); update setuptools config
```

### Comparing `rcsb_utils_struct-0.46/LICENSE` & `rcsb_utils_struct-0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb_utils_struct-0.46/PKG-INFO` & `rcsb_utils_struct-0.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.struct
-Version: 0.46
+Version: 0.47
 Summary: RCSB Python utility classes for accessing PDB primary structure data and features associated with these data
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb_utils_struct-0.46/README.md` & `rcsb_utils_struct-0.47/README.md`

 * *Files identical despite different names*

### Comparing `rcsb_utils_struct-0.46/rcsb/utils/struct/CathClassificationProvider.py` & `rcsb_utils_struct-0.47/rcsb/utils/struct/CathClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_utils_struct-0.46/rcsb/utils/struct/EcodClassificationProvider.py` & `rcsb_utils_struct-0.47/rcsb/utils/struct/EcodClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_utils_struct-0.46/rcsb/utils/struct/EntryInfoProvider.py` & `rcsb_utils_struct-0.47/rcsb/utils/struct/EntryInfoProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_utils_struct-0.46/rcsb/utils/struct/Scop2ClassificationProvider.py` & `rcsb_utils_struct-0.47/rcsb/utils/struct/Scop2ClassificationProvider.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 #
 #  Updates:
 #   10-Sep-2021 jdw split tree with type and class roots
 #   24-Feb-2022 dwp Resolve duplication issues with Scop2 tree node list, and fix parent ID lists for nodes with multiple parents
 #   18-Apr-2023 aae Use "pickle" as default file format
 #   18-Jul-2023 dwp Resolve duplication issues with Scop2 families list
 #   23-Apr-2024 dwp SCOP2/SCOP2B website was shut down--turn off fetching of source data until/if new site is made available again
+#    9-May-2024 dwp Adjust reload process to not re-download fallback data upon every instantiation
 ##
 """
   Extract SCOP2 domain assignments, term descriptions and SCOP2 classification hierarchy
   from SCOP2 and SCOP2B flat files.
 
 """
 
 import collections
-import datetime
+# import datetime
 import logging
 import os.path
 import sys
 
 from rcsb.utils.io.FileUtil import FileUtil
 from rcsb.utils.io.MarshalUtil import MarshalUtil
 from rcsb.utils.io.StashableBase import StashableBase
@@ -42,19 +43,20 @@
         self.__useCache = useCache
         super(Scop2ClassificationProvider, self).__init__(self.__cachePath, [dirName])
         #
         self.__version = "latest"
         self.__fmt = "pickle"
         self.__mU = MarshalUtil(workPath=self.__dirPath)
         #
+        self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=self.__useCache, fmt=self.__fmt)
         # Temporarily turn off fetching of source data until new site is made available again
-        # self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=self.__useCache, fmt=self.__fmt)
         # if not useCache and not self.testCache():
-        self.__fetchFromBackup(fmt=self.__fmt)
-        self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=True, fmt=self.__fmt)
+        #     ok = self.__fetchFromBackup(fmt=self.__fmt)
+        #     if ok:
+        #         self.__nD, self.__ntD, self.__pAD, self.__pBD, self.__pBRootD, self.__fD, self.__sfD, self.__sf2bD = self.__reload(useCache=True, fmt=self.__fmt)
         if not self.testCache():
             logger.error("Failed to build SCOP2 CACHE")
 
     def testCache(self):
         logger.info(
             "SCOP2 lengths nD %d pAD %d pBD %d pBRootD %d fD %d sfD %d sf2bD %d",
             len(self.__nD), len(self.__pAD), len(self.__pBD), len(self.__pBRootD), len(self.__fD), len(self.__sfD), len(self.__sf2bD)
@@ -189,59 +191,66 @@
         nD = ntD = pAD = pBD = pBRootD = fD = sfD = sf2bD = {}
         fn = self.__getAssignmentFileName(fmt=fmt)
         assignmentPath = os.path.join(self.__dirPath, fn)
         self.__mU.mkdir(self.__dirPath)
         #
         if useCache and self.__mU.exists(assignmentPath):
             sD = self.__mU.doImport(assignmentPath, fmt=fmt)
-            logger.debug("Domain name count %d", len(sD["names"]))
-            self.__version = sD["version"]
-            nD = sD["names"]
-            ntD = sD["nametypes"]
-            pAD = sD["parentsType"]
-            pBD = sD["parentsClass"]
-            pBRootD = sD["parentsClassRoot"]
-            fD = sD["families"]
-            sfD = sD["superfamilies"]
-            sf2bD = sD["superfamilies2b"]
+        else:
+            ok = self.__fetchFromBackup(fmt=fmt)
+            sD = self.__mU.doImport(assignmentPath, fmt=fmt)
+            if not ok and sD:
+                logger.error("failed to fetch from fallback - fetch status %r len(sD) %r", ok, len(sD))
+        #
+        logger.debug("Domain name count %d", len(sD["names"]))
+        self.__version = sD["version"]
+        nD = sD["names"]
+        ntD = sD["nametypes"]
+        pAD = sD["parentsType"]
+        pBD = sD["parentsClass"]
+        pBRootD = sD["parentsClassRoot"]
+        fD = sD["families"]
+        sfD = sD["superfamilies"]
+        sf2bD = sD["superfamilies2b"]
+
+        # Temporarily turn off fetching of source data until new site is made available again
+        # elif not useCache:
+        #     nmL, dmL, scop2bL, _ = self.__fetchFromSource()
+        #     #
+        #     ok = False
+        #     nD = self.__extractNames(nmL)
+        #     logger.info("Domain name dictionary (%d)", len(nD))
+        #     pAD, pBD, pBRootD, ntD, fD, sfD, domToSfD = self.__extractDomainHierarchy(dmL)
+        #     #
+        #     logger.info("Domain node parent hierarchy (protein type) (%d)", len(pAD))
+        #     logger.info("Domain node parent hierarchy (structural class) (%d)", len(pBD))
+        #     logger.info("Domain node parent hierarchy (structural class root) (%d)", len(pBRootD))
+        #     logger.info("SCOP2 core domain assignments (family %d) (sf %d)", len(fD), len(sfD))
+        #     #
+        #     sf2bD = self.__extractScop2bSuperFamilyAssignments(scop2bL, domToSfD)
+        #     logger.info("SCOP2B SF domain assignments (%d)", len(sf2bD))
+        #     #
+        #     tS = datetime.datetime.now().isoformat()
+        #     # vS = datetime.datetime.now().strftime("%Y-%m-%d")
+        #     vS = self.__version
+        #     sD = {
+        #         "version": vS,
+        #         "created": tS,
+        #         "names": nD,
+        #         "nametypes": ntD,
+        #         "parentsType": pAD,
+        #         "parentsClass": pBD,
+        #         "parentsClassRoot": pBRootD,
+        #         "families": fD,
+        #         "superfamilies": sfD,
+        #         "superfamilies2b": sf2bD
+        #     }
+        #     ok = self.__mU.doExport(assignmentPath, sD, fmt=fmt, indent=3)
+        #     logger.info("Cache save status %r", ok)
 
-        elif not useCache:
-            nmL, dmL, scop2bL, _ = self.__fetchFromSource()
-            #
-            ok = False
-            nD = self.__extractNames(nmL)
-            logger.info("Domain name dictionary (%d)", len(nD))
-            pAD, pBD, pBRootD, ntD, fD, sfD, domToSfD = self.__extractDomainHierarchy(dmL)
-            #
-            logger.info("Domain node parent hierarchy (protein type) (%d)", len(pAD))
-            logger.info("Domain node parent hierarchy (structural class) (%d)", len(pBD))
-            logger.info("Domain node parent hierarchy (structural class root) (%d)", len(pBRootD))
-            logger.info("SCOP2 core domain assignments (family %d) (sf %d)", len(fD), len(sfD))
-            #
-            sf2bD = self.__extractScop2bSuperFamilyAssignments(scop2bL, domToSfD)
-            logger.info("SCOP2B SF domain assignments (%d)", len(sf2bD))
-            #
-            tS = datetime.datetime.now().isoformat()
-            # vS = datetime.datetime.now().strftime("%Y-%m-%d")
-            vS = self.__version
-            sD = {
-                "version": vS,
-                "created": tS,
-                "names": nD,
-                "nametypes": ntD,
-                "parentsType": pAD,
-                "parentsClass": pBD,
-                "parentsClassRoot": pBRootD,
-                "families": fD,
-                "superfamilies": sfD,
-                "superfamilies2b": sf2bD
-            }
-            ok = self.__mU.doExport(assignmentPath, sD, fmt=fmt, indent=3)
-            logger.info("Cache save status %r", ok)
-            #
         return nD, ntD, pAD, pBD, pBRootD, fD, sfD, sf2bD
 
     def __fetchFromBackup(self, fmt="pickle"):
         urlTarget = "https://raw.githubusercontent.com/rcsb/py-rcsb_exdb_assets/master/fall_back/SCOP2"
         #
         fn = self.__getAssignmentFileName(fmt=fmt)
         assignmentPath = os.path.join(self.__dirPath, fn)
```

### Comparing `rcsb_utils_struct-0.46/rcsb/utils/struct/ScopClassificationProvider.py` & `rcsb_utils_struct-0.47/rcsb/utils/struct/ScopClassificationProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/PKG-INFO` & `rcsb_utils_struct-0.47/rcsb.utils.struct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.struct
-Version: 0.46
+Version: 0.47
 Summary: RCSB Python utility classes for accessing PDB primary structure data and features associated with these data
 Home-page: https://github.com/rcsb/py-rcsb_utils_seq
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb_utils_struct-0.46/rcsb.utils.struct.egg-info/SOURCES.txt` & `rcsb_utils_struct-0.47/rcsb.utils.struct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb_utils_struct-0.46/setup.py` & `rcsb_utils_struct-0.47/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/wwpdb.utils.wf-0.35.3.tar.gz` & `tmp/wwpdb_utils_wf-0.35.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.wf-0.35.3.tar", last modified: Thu Feb  8 22:07:53 2024, max compression
+gzip compressed data, was "wwpdb_utils_wf-0.35.4.tar", last modified: Thu May  9 20:24:05 2024, max compression
```

## Comparing `wwpdb.utils.wf-0.35.3.tar` & `wwpdb_utils_wf-0.35.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 22:07:53.752896 wwpdb.utils.wf-0.35.3/
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-02-08 22:07:53.752896 wwpdb.utils.wf-0.35.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      485 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-02-08 22:07:53.752896 wwpdb.utils.wf-0.35.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2105 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 22:07:53.744896 wwpdb.utils.wf-0.35.3/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 22:07:53.748896 wwpdb.utils.wf-0.35.3/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 22:07:53.748896 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/
--rw-r--r--   0 vsts      (1001) docker     (127)     3229 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/DataSelector.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4658 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/DataValueContainer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3661 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/WfDataObject.py
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 22:07:53.748896 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/
--rw-r--r--   0 vsts      (1001) docker     (127)     6846 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/DbApiUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16002 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/DbCommand.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/DbConnection.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1946 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/LocalDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3018 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/StatusDbApi.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1281 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/WFEtime.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47456 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/WfDbApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4251 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/WfTracking.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11637 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/dbAPI.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 22:07:53.752896 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/
--rw-r--r--   0 vsts      (1001) docker     (127)    65854 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/AnnotationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11876 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/ChemCompUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/DictUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3595 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/DpUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18242 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6275 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/FileUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13301 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/FormatUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50817 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/NmrUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13901 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/PdbxUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3840 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/PrdSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3427 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/ReportUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5580 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/SFConvert.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5698 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/SeqStatsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11212 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/SeqdbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1456 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/UtilsBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27740 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/ValidationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 22:07:53.752896 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/process/
--rw-r--r--   0 vsts      (1001) docker     (127)    15843 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/process/ActionRegistry.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7456 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/process/ActionRegistryIo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11325 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/process/ProcessRunner.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/process/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 22:07:53.752896 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/schema/
--rw-r--r--   0 vsts      (1001) docker     (127)    12006 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/schema/WfSchemaMap.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/schema/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11697 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/schema/database_descriptions.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      233 2024-02-08 22:06:51.000000 wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/schema/mandatory_items.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-08 22:07:53.752896 wwpdb.utils.wf-0.35.3/wwpdb.utils.wf.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-02-08 22:07:53.000000 wwpdb.utils.wf-0.35.3/wwpdb.utils.wf.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1724 2024-02-08 22:07:53.000000 wwpdb.utils.wf-0.35.3/wwpdb.utils.wf.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-08 22:07:53.000000 wwpdb.utils.wf-0.35.3/wwpdb.utils.wf.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-08 22:07:43.000000 wwpdb.utils.wf-0.35.3/wwpdb.utils.wf.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-02-08 22:07:53.000000 wwpdb.utils.wf-0.35.3/wwpdb.utils.wf.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-02-08 22:07:53.000000 wwpdb.utils.wf-0.35.3/wwpdb.utils.wf.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      485 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2103 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.484543 wwpdb_utils_wf-0.35.4/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.488543 wwpdb_utils_wf-0.35.4/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.488543 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3229 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/DataSelector.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4658 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/DataValueContainer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3661 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/WfDataObject.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.488543 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6846 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbApiUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16002 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbCommand.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbConnection.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1946 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/LocalDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3018 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/StatusDbApi.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1281 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WFEtime.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47456 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WfDbApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4251 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WfTracking.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11637 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/dbAPI.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.492544 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/
+-rw-r--r--   0 vsts      (1001) docker     (127)    65854 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/AnnotationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11876 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ChemCompUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3611 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/DictUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4666 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/DpUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18242 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6275 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/FileUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13301 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/FormatUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50817 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/NmrUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18848 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/PdbxUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3840 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/PrdSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3427 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ReportUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5580 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SFConvert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5698 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SeqStatsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11212 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SeqdbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1456 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/UtilsBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    27740 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ValidationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15843 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ActionRegistry.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7456 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ActionRegistryIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11325 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ProcessRunner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/
+-rw-r--r--   0 vsts      (1001) docker     (127)    12006 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/WfSchemaMap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11697 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/database_descriptions.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      233 2024-05-09 20:22:43.000000 wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/mandatory_items.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-09 20:24:05.496544 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1724 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-09 20:23:48.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      132 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-09 20:24:05.000000 wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.wf-0.35.3/LICENSE` & `wwpdb_utils_wf-0.35.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/PKG-INFO` & `wwpdb_utils_wf-0.35.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.35.3
+Version: 0.35.4
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 Requires-Dist: mysqlclient
-Requires-Dist: wwpdb.utils.config>=0.22.2
+Requires-Dist: wwpdb.utils.config~=0.41
 Requires-Dist: wwpdb.io
 Requires-Dist: mmcif
-Requires-Dist: wwpdb.utils.dp~=0.47
+Requires-Dist: wwpdb.utils.dp~=0.51
 Requires-Dist: wwpdb.utils.session
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 See:  README.md
```

### Comparing `wwpdb.utils.wf-0.35.3/setup.py` & `wwpdb_utils_wf-0.35.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     #
-    install_requires=["mysqlclient", "wwpdb.utils.config >= 0.22.2", "wwpdb.io", "mmcif", "wwpdb.utils.dp ~= 0.47", "wwpdb.utils.session"],
+    install_requires=["mysqlclient", "wwpdb.utils.config ~= 0.41", "wwpdb.io", "mmcif", "wwpdb.utils.dp ~= 0.51", "wwpdb.utils.session"],
     packages=find_packages(exclude=["wwpdb.utils.tests_wf", "mock-data", "tests.*"]),
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
         "": ["*.md", "*.rst", "*.txt", "*.cfg"],
     },
     #
     # These basic tests require no database services -
```

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/DataSelector.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/DataSelector.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/DataValueContainer.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/DataValueContainer.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/WfDataObject.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/WfDataObject.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/DbApiUtil.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbApiUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/DbCommand.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbCommand.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/DbConnection.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/DbConnection.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/LocalDbApi.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/LocalDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/StatusDbApi.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/StatusDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/WFEtime.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WFEtime.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/WfDbApi.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WfDbApi.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/WfTracking.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/WfTracking.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/dbapi/dbAPI.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/dbapi/dbAPI.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/AnnotationUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/AnnotationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/ChemCompUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ChemCompUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/DictUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/DictUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/DpUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/DpUtils.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Each method in the class handles its own exceptions and returns
     True on success or False otherwise.
 
     """
 
     def __init__(self, verbose=False, log=sys.stderr):
         super(DpUtils, self).__init__(verbose, log)
-        self.__cleanUp = False
+        self.__cleanUp = True
         """Flag to remove any temporary directories created by this class.
         """
         #
 
     def polymerLinkageDistanceOp(self, **kwArgs):
         """Calculate polymer linkage distances -"""
         try:
@@ -95,7 +95,34 @@
                 dp.cleanup()
             if self._verbose:
                 self._lfh.write("+DpUtils.centreOfMassCalculation() - PDBx     file path: %s\n" % pdbxPath)
             return True
         except Exception as _e:  # noqa: F841
             traceback.print_exc(file=self._lfh)
             return False
+
+    def generateComplexityOp(self, **kwargs):
+        """Generates complexity report"""
+        try:
+            (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwargs)
+            pdbxPath = inpObjD["src"].getFilePathReference()
+            pdbxOutputPath = outObjD["dst"].getFilePathReference()
+            dirPath = outObjD["dst"].getDirPathReference()
+            logPath = os.path.join(dirPath, "generate-complexity.log")
+
+            cI = ConfigInfo()
+            siteId = cI.get("SITE_PREFIX")
+
+            dp = RcsbDpUtility(tmpPath=dirPath, siteId=siteId, verbose=self._verbose, log=self._lfh)
+            dp.imp(pdbxPath)
+            dp.op("annot-complexity")
+            dp.expLog(logPath)
+            dp.exp(pdbxOutputPath)
+
+            if self.__cleanUp:
+                dp.cleanup()
+            if self._verbose:
+                self._lfh.write("+DpUtils.generatComplexityOp() - PDBx     file path: %s\n" % pdbxPath)
+            return True
+        except Exception as _e:  # noqa: F841
+            traceback.print_exc(file=self._lfh)
+            return False
```

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/EmUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/EmUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/FileUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/FileUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/FormatUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/FormatUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/NmrUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/NmrUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/PdbxUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/PdbxUtils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ##
 # File:    PdxUtils.py
 # Date:    10-April-2010
 #
 # Updates:
 # 24-April-2010  jdw statusOp method to return a dictionary of common status items.
+#  9-May-2024    zf  add fetchAnnAutoOp
 #
 ##
 """
 Module of data access utility operations supporting the call protocol of the ProcessRunner() class.
 
 """
 __docformat__ = "restructuredtext en"
@@ -15,14 +16,15 @@
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.01"
 
 import sys
 import traceback
 
+from wwpdb.utils.config.ConfigInfo import ConfigInfo
 from wwpdb.utils.wf.plugins.UtilsBase import UtilsBase
 
 from mmcif.core.mmciflib import ParseCifSimple  # pylint: disable=no-name-in-module
 
 
 class CifFile(object):
 
@@ -74,15 +76,14 @@
         self.__block = None
         """ Target block -
         """
         self.__blockList = []
         self.__targetBlockName = None
         self.__targetBlockIndex = 0
         self.__cifFile = None
-        self.__blockList = []
         self._lfh = log
 
     def __getBlock(self, pdbxPath):
         """Open the input PDBx file and set the target data block.
 
         Returns:
 
@@ -200,14 +201,73 @@
             #
             return True
         except Exception as _e:  # noqa: F841
             if self._verbose:
                 traceback.print_exc(file=self._lfh)
             return False
 
+    def __templateFetchAnnAuto(self, kwD):
+        """Template fetch column method.
+
+        This method supports recovering the values of an attribute (or column of attributes).
+
+        Selector defines the following selector parameters:
+        - targetCategoryName  name of the target category
+        - targetAttributeName name of the target attribute
+
+        Only container types *list* and *value* are support.
+        """
+        try:
+            (inpObjD, outObjD, _uD, _pD) = self._getArgs(kwD)
+            pdbxPath = str(inpObjD["src"].getFilePathReference())
+            if not self.__getBlock(pdbxPath):
+                return False
+            #
+            targetCategory = str(inpObjD["src"].getSelectCategoryName())
+            if not self.__block.IsTablePresent(targetCategory):
+                return False
+
+            attributeList = inpObjD["src"].getSelectAttributeList()
+            targetAttribute = str(attributeList[0])
+
+            myTable = self.__block.GetTable(targetCategory)
+            cL = []
+            # colNames = list(myTable.GetColumnNames())
+            rList = list(myTable.GetColumn(cL, targetAttribute))
+
+            if outObjD["dst1"].getContainerTypeName() == "value":
+                outObjD["dst1"].setValue(rList[0])
+            elif outObjD["dst1"].getContainerTypeName() == "list":
+                outObjD["dst1"].setValue(rList)
+            else:
+                return False
+            #
+            yes_no_value = self.__getAnnModAutoCompleteFlag()
+            if outObjD["dst2"].getContainerTypeName() == "value":
+                outObjD["dst2"].setValue(yes_no_value)
+            elif outObjD["dst2"].getContainerTypeName() == "list":
+                outObjD["dst2"].setValue([ yes_no_value ])
+            else:
+                return False
+            #
+            cI = ConfigInfo()
+            siteName = cI.get("SITE_NAME")
+            if outObjD["dst3"].getContainerTypeName() == "value":
+                outObjD["dst3"].setValue(siteName)
+            elif outObjD["dst3"].getContainerTypeName() == "list":
+                outObjD["dst3"].setValue([ siteName ])
+            else:
+                return False
+            #
+            return True
+        except Exception as _e:  # noqa: F841
+            if self._verbose:
+                traceback.print_exc(file=self._lfh)
+            return False
+
     def __getCategoryRowCount(self, kwD):
         """Template method to count category size/test for existence .
 
         Input src defines pdbx file and dst will hold integer row count.
 
         User defined parameter 'category':
         - name of category to which the test is applied
@@ -247,14 +307,17 @@
 
     def selectOp(self, **kwArgs):
         return self.__templateSelection(kwArgs)
 
     def fetchOp(self, **kwArgs):
         return self.__templateFetchAttribute(kwArgs)
 
+    def fetchAnnAutoOp(self, **kwArgs):
+        return self.__templateFetchAnnAuto(kwArgs)
+
     def statusOp(self, **kwArgs):
         return self.__fetchStatusDictionary(kwArgs)
 
     def __fetchStatusDictionary(self, kwD):
         """
         depDB = {}
         Done -
@@ -380,7 +443,66 @@
 
             outObjD["dst"].setValue(d)
             return True
         except Exception as _e:  # noqa: F841
             if self._verbose:
                 traceback.print_exc(file=self._lfh)
             return False
+        #
+
+    def __getAnnModAutoCompleteFlag(self):
+        """
+        """
+        try:
+            ret = "NO"
+            if self.__block.IsTablePresent("exptl"):
+                table = self.__block.GetTable("exptl")
+                if table and (table.GetNumRows() > 0):
+                    if table.IsColumnPresent("method"):
+                        val = table(0, "method")
+                        val = val.strip().upper()
+                        if (val == "ELECTRON MICROSCOPY") or (val == "SOLID-STATE NMR") or (val == "SOLUTION NMR"):
+                            ret = "YES"
+                        #
+                    #
+                #
+            #
+            if ret == "NO":
+                return ret
+            #
+            assemblyCategories = { "pdbx_struct_assembly": [ "id", "details" ], \
+                                   "pdbx_struct_assembly_gen": [ "assembly_id", "oper_expression", "asym_id_list" ], \
+                                   "pdbx_struct_oper_list": [ "id", "matrix[1][1]", "matrix[1][2]", "matrix[1][3]", \
+                                   "vector[1]", "matrix[2][1]", "matrix[2][2]", "matrix[2][3]", "vector[2]", "matrix[3][1]", \
+                                   "matrix[3][2]", "matrix[3][3]", "vector[3]" ] }
+            #
+            for cate,items in assemblyCategories.items():
+                if self.__block.IsTablePresent(cate):
+                    table = self.__block.GetTable(cate)
+                    if table and (table.GetNumRows() > 0):
+                        valList = []
+                        for item in items:
+                            if table.IsColumnPresent(item):
+                                val = table(0, item)
+                                if val and (val != ".") and (val != "?"):
+                                    valList.append(val)
+                                #
+                            #
+                        #
+                        if len(valList) != len(items):
+                            ret = "NO"
+                        #
+                    else:
+                        ret = "NO"
+                    #
+                else:
+                    ret = "NO"
+                #
+                if ret == "NO":
+                    return ret
+                #
+            #
+            return ret
+        except Exception as _e:
+            traceback.print_exc(file=sys.stderr)
+            return "NO"
+        #
```

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/PrdSearchUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/PrdSearchUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/ReportUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ReportUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/SFConvert.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SFConvert.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/SeqStatsUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SeqStatsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/SeqdbUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/SeqdbUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/UtilsBase.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/UtilsBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/plugins/ValidationUtils.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/plugins/ValidationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/process/ActionRegistry.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ActionRegistry.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/process/ActionRegistryIo.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ActionRegistryIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/process/ProcessRunner.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/process/ProcessRunner.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/schema/WfSchemaMap.py` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/WfSchemaMap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb/utils/wf/schema/database_descriptions.txt` & `wwpdb_utils_wf-0.35.4/wwpdb/utils/wf/schema/database_descriptions.txt`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb.utils.wf.egg-info/PKG-INFO` & `wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.wf
-Version: 0.35.3
+Version: 0.35.4
 Summary: OneDep WF status DB access utilities
 Home-page: https://github.com/rcsb/py-wwpdb_utils_wf
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 Requires-Dist: mysqlclient
-Requires-Dist: wwpdb.utils.config>=0.22.2
+Requires-Dist: wwpdb.utils.config~=0.41
 Requires-Dist: wwpdb.io
 Requires-Dist: mmcif
-Requires-Dist: wwpdb.utils.dp~=0.47
+Requires-Dist: wwpdb.utils.dp~=0.51
 Requires-Dist: wwpdb.utils.session
 Provides-Extra: dev
 Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 
 See:  README.md
```

### Comparing `wwpdb.utils.wf-0.35.3/wwpdb.utils.wf.egg-info/SOURCES.txt` & `wwpdb_utils_wf-0.35.4/wwpdb.utils.wf.egg-info/SOURCES.txt`

 * *Files identical despite different names*


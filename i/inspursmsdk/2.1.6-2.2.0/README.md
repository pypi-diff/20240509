# Comparing `tmp/inspursmsdk-2.1.6.tar.gz` & `tmp/inspursmsdk-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inspursmsdk-2.1.6.tar", last modified: Thu Apr 11 02:29:18 2024, max compression
+gzip compressed data, was "dist/inspursmsdk-2.2.0.tar", last modified: Thu May  9 06:32:59 2024, max compression
```

## Comparing `inspursmsdk-2.1.6.tar` & `inspursmsdk-2.2.0.tar`

### file list

```diff
@@ -1,88 +1,84 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/
--rw-r--r--   0 root         (0) root         (0)      991 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      896 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      230 2024-04-11 02:26:45.000000 inspursmsdk-2.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-11 02:26:45.000000 inspursmsdk-2.1.6/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/
--rw-r--r--   0 root         (0) root         (0)    49818 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/IpmiFunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
--rw-r--r--   0 root         (0) root         (0)    16391 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/commonInfoStr.py
--rw-r--r--   0 root         (0) root         (0)      693 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/eventLogString.py
--rw-r--r--   0 root         (0) root         (0)     3787 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/sensorEventStr.py
--rw-r--r--   0 root         (0) root         (0)    51098 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
--rw-r--r--   0 root         (0) root         (0)     5698 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/showSensorDesc.py
--rw-r--r--   0 root         (0) root         (0)    21216 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/RedfishFunc.py
--rw-r--r--   0 root         (0) root         (0)   300270 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/RestFunc.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12152 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/backup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/
--rw-r--r--   0 root         (0) root         (0)    44672 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/A7.xml
--rw-r--r--   0 root         (0) root         (0)    18131 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M4.xml
--rw-r--r--   0 root         (0) root         (0)    54444 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M5.xml
--rw-r--r--   0 root         (0) root         (0)    84520 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6-N.xml
--rw-r--r--   0 root         (0) root         (0)    81800 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6.xml
--rw-r--r--   0 root         (0) root         (0)    46178 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M7.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF3180A6.xml
--rw-r--r--   0 root         (0) root         (0)    30946 2024-04-11 02:26:49.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF3280A6.xml
--rw-r--r--   0 root         (0) root         (0)   360127 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5180M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5280M5.xml
--rw-r--r--   0 root         (0) root         (0)    36922 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5468A5.xml
--rw-r--r--   0 root         (0) root         (0)    29961 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5488A5.xml
--rw-r--r--   0 root         (0) root         (0)   360290 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5112M5.xml
--rw-r--r--   0 root         (0) root         (0)   360210 2024-04-11 02:26:48.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5212M5.xml
--rw-r--r--   0 root         (0) root         (0)    66019 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/command/restore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/
--rw-r--r--   0 root         (0) root         (0)     1613 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/NF5180M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/NF5280M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/SA5112M5.yml
--rw-r--r--   0 root         (0) root         (0)     1959 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/SA5212M5.yml
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/conf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/
--rw-r--r--   0 root         (0) root         (0)    44318 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/Base.py
--rw-r--r--   0 root         (0) root         (0)     2590 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA5.py
--rw-r--r--   0 root         (0) root         (0)     3023 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA6.py
--rw-r--r--   0 root         (0) root         (0)     6333 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA7.py
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA7_11308.py
--rw-r--r--   0 root         (0) root         (0)   744218 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM5.py
--rw-r--r--   0 root         (0) root         (0)   604752 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6.py
--rw-r--r--   0 root         (0) root         (0)    18029 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6_41401.py
--rw-r--r--   0 root         (0) root         (0)    16476 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6_4140a.py
--rw-r--r--   0 root         (0) root         (0)   288628 2024-04-11 02:26:47.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM7.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM7_13505.py
--rw-r--r--   0 root         (0) root         (0)    45791 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/I24M6.py
--rw-r--r--   0 root         (0) root         (0)     8558 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/IBase.py
--rw-r--r--   0 root         (0) root         (0)    14826 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5180M5.py
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5180M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    15217 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5.py
--rw-r--r--   0 root         (0) root         (0)      510 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5Impl.py
--rw-r--r--   0 root         (0) root         (0)    59696 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5_435.py
--rw-r--r--   0 root         (0) root         (0)     2193 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5_436.py
--rw-r--r--   0 root         (0) root         (0)    47115 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/NS5160M6.py
--rw-r--r--   0 root         (0) root         (0)   122296 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/ResEntity.py
--rw-r--r--   0 root         (0) root         (0)      512 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/SA5212M5Impl.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/route/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/route/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5311 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/route/route.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/
--rw-r--r--   0 root         (0) root         (0)     4718 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/HostTypeJudge.py
--rw-r--r--   0 root         (0) root         (0)     4788 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/RedfishClient.py
--rw-r--r--   0 root         (0) root         (0)    10339 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/RegularCheckUtil.py
--rw-r--r--   0 root         (0) root         (0)     7686 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/RequestClient.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7550 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/configUtil.py
--rw-r--r--   0 root         (0) root         (0)     1812 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/fileUtil.py
--rw-r--r--   0 root         (0) root         (0)     7590 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/inspur_sm_sdk/util/parameterConversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      896 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2682 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-11 02:29:17.000000 inspursmsdk-2.1.6/inspursmsdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5216 2024-04-11 02:26:46.000000 inspursmsdk-2.1.6/ism.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 02:29:18.000000 inspursmsdk-2.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2024-04-11 02:26:45.000000 inspursmsdk-2.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:32:59.000000 inspursmsdk-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)      849 2024-05-09 06:29:57.000000 inspursmsdk-2.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      896 2024-05-09 06:32:59.000000 inspursmsdk-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-09 06:29:57.000000 inspursmsdk-2.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-09 06:29:42.000000 inspursmsdk-2.2.0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:32:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:32:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/
+-rw-r--r--   0 root         (0) root         (0)    49979 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/IpmiFunc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:32:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/biosPostEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    16391 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/commonInfoStr.py
+-rw-r--r--   0 root         (0) root         (0)      693 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/eventLogString.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/sensorEventStr.py
+-rw-r--r--   0 root         (0) root         (0)    51098 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py
+-rw-r--r--   0 root         (0) root         (0)     5697 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/showSensorDesc.py
+-rw-r--r--   0 root         (0) root         (0)    21216 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/RedfishFunc.py
+-rw-r--r--   0 root         (0) root         (0)   310435 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/RestFunc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12152 2024-05-09 06:30:00.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/backup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:32:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/
+-rw-r--r--   0 root         (0) root         (0)    44672 2024-05-09 06:30:00.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/A7.xml
+-rw-r--r--   0 root         (0) root         (0)    18001 2024-05-09 06:30:00.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M4.xml
+-rw-r--r--   0 root         (0) root         (0)    54050 2024-05-09 06:30:00.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M5.xml
+-rw-r--r--   0 root         (0) root         (0)    84400 2024-05-09 06:30:00.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M6-N.xml
+-rw-r--r--   0 root         (0) root         (0)    81680 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M6.xml
+-rw-r--r--   0 root         (0) root         (0)    46082 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M7.xml
+-rw-r--r--   0 root         (0) root         (0)   117980 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M7_5.10.00.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF3180A6.xml
+-rw-r--r--   0 root         (0) root         (0)    30946 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF3280A6.xml
+-rw-r--r--   0 root         (0) root         (0)   354128 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5180M5.xml
+-rw-r--r--   0 root         (0) root         (0)   354211 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5280M5.xml
+-rw-r--r--   0 root         (0) root         (0)    36922 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5468A5.xml
+-rw-r--r--   0 root         (0) root         (0)    29961 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5488A5.xml
+-rw-r--r--   0 root         (0) root         (0)   354291 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/SA5112M5.xml
+-rw-r--r--   0 root         (0) root         (0)   354213 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/SA5212M5.xml
+-rw-r--r--   0 root         (0) root         (0)    66019 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/command/restore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:32:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/
+-rw-r--r--   0 root         (0) root         (0)    44334 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/Base.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonA5.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonA6.py
+-rw-r--r--   0 root         (0) root         (0)     6333 2024-05-09 06:29:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonA7.py
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonA7_11308.py
+-rw-r--r--   0 root         (0) root         (0)   744312 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM5.py
+-rw-r--r--   0 root         (0) root         (0)   608250 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM6.py
+-rw-r--r--   0 root         (0) root         (0)    18067 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM6_41401.py
+-rw-r--r--   0 root         (0) root         (0)    16476 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM6_4140a.py
+-rw-r--r--   0 root         (0) root         (0)   272646 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM7.py
+-rw-r--r--   0 root         (0) root         (0)     3883 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM7_13505.py
+-rw-r--r--   0 root         (0) root         (0)    45791 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/I24M6.py
+-rw-r--r--   0 root         (0) root         (0)     8558 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/IBase.py
+-rw-r--r--   0 root         (0) root         (0)    14826 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5180M5.py
+-rw-r--r--   0 root         (0) root         (0)      339 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5180M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    15217 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5280M5.py
+-rw-r--r--   0 root         (0) root         (0)      510 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5280M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)    59696 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5280M5_435.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5280M5_436.py
+-rw-r--r--   0 root         (0) root         (0)    47115 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/NS5160M6.py
+-rw-r--r--   0 root         (0) root         (0)   123026 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/ResEntity.py
+-rw-r--r--   0 root         (0) root         (0)      512 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/SA5212M5Impl.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:32:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/route/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/route/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/route/interfaceRoute.yml
+-rw-r--r--   0 root         (0) root         (0)     2398 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/route/modelRoute.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:32:59.000000 inspursmsdk-2.2.0/inspur_sm_sdk/util/
+-rw-r--r--   0 root         (0) root         (0)     4720 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/util/HostTypeJudge.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/util/RedfishClient.py
+-rw-r--r--   0 root         (0) root         (0)    10339 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/util/RegularCheckUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7742 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/util/RequestClient.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8030 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/util/configUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/util/fileUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7590 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/inspur_sm_sdk/util/parameterConversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:32:59.000000 inspursmsdk-2.2.0/inspursmsdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      896 2024-05-09 06:32:58.000000 inspursmsdk-2.2.0/inspursmsdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2609 2024-05-09 06:32:58.000000 inspursmsdk-2.2.0/inspursmsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 06:32:58.000000 inspursmsdk-2.2.0/inspursmsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-09 06:32:58.000000 inspursmsdk-2.2.0/inspursmsdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-09 06:32:58.000000 inspursmsdk-2.2.0/inspursmsdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5044 2024-05-09 06:29:58.000000 inspursmsdk-2.2.0/ism.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 06:32:59.000000 inspursmsdk-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-09 06:29:57.000000 inspursmsdk-2.2.0/setup.py
```

### Comparing `inspursmsdk-2.1.6/MANIFEST.in` & `inspursmsdk-2.2.0/MANIFEST.in`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,13 @@
 include inspur_sm_sdk/command/bios/NF5468A5.xml
 include inspur_sm_sdk/command/bios/NF5488A5.xml
 include inspur_sm_sdk/command/bios/SA5112M5.xml
 include inspur_sm_sdk/command/bios/SA5212M5.xml
 include inspur_sm_sdk/command/bios/A7.xml
 include inspur_sm_sdk/command/bios/M7.xml
 include inspur_sm_sdk/command/bios/M6-N.xml
-include inspur_sm_sdk/conf/NF5180M5.yml
-include inspur_sm_sdk/conf/NF5280M5.yml
-include inspur_sm_sdk/conf/NF5468A5.yml
-include inspur_sm_sdk/conf/NF5488A5.yml
-include inspur_sm_sdk/conf/SA5112M5.yml
-include inspur_sm_sdk/conf/SA5212M5.yml
-include inspur_sm_sdk/route/route.yml
+include inspur_sm_sdk/command/bios/M7_5.10.00.xml
+include inspur_sm_sdk/route/interfaceRoute.yml
+include inspur_sm_sdk/route/modelRoute.yml
 include __init__.py
 include ism.py
 include README.md
```

### Comparing `inspursmsdk-2.1.6/PKG-INFO` & `inspursmsdk-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.1.6
+Version: 2.2.0
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/IpmiFunc.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/IpmiFunc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1164,15 +1164,15 @@
     if result['code'] != 0:
         return ''
     num_list = result['data']
     cmd_str = ' '.join(num_list).replace(' ', '').replace('\n', '')
     if len(cmd_str) < 24:
         return ''
     version = cmd_str[4:10]
-    bmcversion = str(int(version[0:2],16))+'.'+str(int(version[2:4],16))
+    bmcversion = str(int(version[0:2],16))+'.'+str(int(version[2:4],16))+'.'+str(int(version[4:6],16))
     return bmcversion
 
 
 # 获取设备信息
 def getM6DeviceNumByIpmi(client,data):
     '''
     get Device Number info
@@ -1238,16 +1238,18 @@
 
 def getFirmwareVersoinByMcinfo(client):
     result = getMcInfoByIpmi(client)
     if result['code'] != 0:
         return ''
     data = result['data']
     bmcVersion_0 = data['firmware_revision']
-    bmcVersion_1 = eval(data['aux_firmware_rev_info'].split(";")[0])
-    bmcVersion = str(bmcVersion_0) + str(int(str(bmcVersion_1), 16)).zfill(2)
+    bmcVersion_1 = data['aux_firmware_rev_info'].split(";")[0]
+    bmcVersion_00 = int(bmcVersion_0.split(".")[0], 16)
+    bmcVersion_01 = int(bmcVersion_0.split(".")[1], 16)
+    bmcVersion = str(bmcVersion_00) + "." + str(bmcVersion_01).zfill(3) + str(bmcVersion_1).zfill(3)
     return bmcVersion
 
 
 # 获取M6机型web界面的登录加密方式，01加密，00不加密
 def judge_encrypt(client):
     cmd = "raw 0x3c 0x05 0x28"
     result = getLineRawByIpmi(client, cmd)
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/biosPostEventStr.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/biosPostEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/commonInfoStr.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/commonInfoStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/eventLogString.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/eventLogString.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/sensorEventStr.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/sensorEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/sensorSpecificEventStr.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/M5Log/showSensorDesc.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/M5Log/showSensorDesc.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             if type == 0x0:
                 pass
             elif type == 0x6F:
                 offset = getbits(item.event_data1, 3, 0)
                 if m_Max_allowed_SensorSpecific_offset[item['sensor_type']] >= offset:
                     eventdesc = sensor_specific_event[item['sensor_type']][offset]
                 else:
-                    eventdesc = eventLogStrings.STR_EVENT_LOG_INVALID_OFFSET;
+                    eventdesc = eventLogStrings.STR_EVENT_LOG_INVALID_OFFSET
             elif (type >= 0x01) and (type <= 0x0C):
                 offset = getbits(item['event_data1'], 3, 0)
                 if m_Max_allowed_offset[type] >= offset:
                     eventdesc = sensorEvent_Str[type][offset]
                 else:
                     eventdesc = eventLogStrings['STR_EVENT_LOG_INVALID_OFFSET']
             else:
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/RedfishFunc.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/RedfishFunc.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/RestFunc.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/RestFunc.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     ISM_ENCODER = False
 import requests
 
 # sys.path.append("..")
 sys.path.append(os.path.dirname(sys.path[0]))
 
 retry_count = 3
+# M7 加密方式，0 不加密，1 RSA加密，2 Blowfish 加密
+# global encrypt_type_flag
+encrypt_type_flag = 0
 
 
 def formatError(url, response):
     try:
         code = str(response.status_code)
     except BaseException:
         code = "1500"
@@ -1050,18 +1053,22 @@
         JSON['data'] = result
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/media/general", response)
     return JSON
 
 
-def setMediaRedirection(client, mediaSettings):
-    # print(mediaSettings)
-    flag = IpmiFunc.judge_encrypt(client)
-    if flag == 1:
+def setMediaRedirection(client, mediaSettings, ff="M6"):
+    if ff == "H2":
+        return setMediaRedirectionH2(client, mediaSettings)
+    if encrypt_type_flag == 1:
+        mediaSettings['cd_remote_password'] = encrypt_rsa(mediaSettings['cd_remote_password'], client.type)
+        mediaSettings['hd_remote_password'] = encrypt_rsa(mediaSettings['hd_remote_password'], client.type)
+        mediaSettings['encrypt_flag'] = 1
+    elif encrypt_type_flag == 2:
         mediaSettings['cd_remote_password'] = Encrypt(mediaSettings['cd_remote_password'])
         mediaSettings['hd_remote_password'] = Encrypt(mediaSettings['hd_remote_password'])
         mediaSettings['encrypt_flag'] = 1
     response = client.request("PUT", "api/settings/media/general", client.getHearder(), data=None, json=mediaSettings)
     JSON = {}
     if response is None:
         JSON['code'] = 1
@@ -1072,14 +1079,39 @@
         JSON['data'] = result
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/media/general", response)
     return JSON
 
 
+def setMediaRedirectionH2(client, mediaSettings):
+    if encrypt_type_flag == 1:
+        mediaSettings['cd_remote_password'] = encrypt_rsa(mediaSettings['cd_remote_password'], 'H2')
+        mediaSettings['hd_remote_password'] = encrypt_rsa(mediaSettings['hd_remote_password'], 'H2')
+        mediaSettings['encrypt_flag'] = 1
+    elif encrypt_type_flag == 2:
+        mediaSettings['cd_remote_password'] = Encrypt(mediaSettings['cd_remote_password'])
+        mediaSettings['hd_remote_password'] = Encrypt(mediaSettings['hd_remote_password'])
+        mediaSettings['encrypt_flag'] = 1
+    # print(mediaSettings)
+    response = client.request("PUT", "api/settings/media/general", client.getHearder(), data=None, json=mediaSettings)
+    JSON = {}
+    if response is None:
+        JSON['code'] = 1
+        JSON['data'] = 'Failed to call BMC interface api/settings/media/general, response is none'
+    elif response.status_code in range(200, 300):
+        result = response.json()
+        JSON['code'] = 0
+        JSON['data'] = result
+    else:
+        JSON['code'] = 1
+        JSON['data'] = formatError("api/settings/media/general", response)
+    return JSON
+
+
 def getMediaInstance(client):
     response = client.request("GET", "api/settings/media/instance", client.getHearder(), data=None)
     JSON = {}
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/settings/media/instance, response is none'
     elif response.status_code == 200:
@@ -1287,25 +1319,35 @@
         JSON['data'] = result
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/users/" + str(id), response)
     return JSON
 
 
-def addUserByRestM6(client, args):
+def addUserByRestM6(client, args, ff="M6"):
     JSON = {}
     if args.uname is None or args.uname == "":
         JSON['code'] = 1
         JSON['data'] = 'uname cannot be none'
         return JSON
 
     # uname = Encrypt(args.uname, "add")
     # upass = Encrypt(args.upass, "add")
-    uname = args.uname
-    upass = args.upass
+    if encrypt_type_flag == 1:
+        uname = encrypt_rsa(args.uname, client.type)
+        upass = encrypt_rsa(args.upass, client.type)
+        session_confirm = encrypt_rsa(args.passcode, client.type)
+    elif encrypt_type_flag == 2:
+        uname = Encrypt(args.uname, "addadd")
+        upass = Encrypt(args.upass, "addadd")
+        session_confirm = ""
+    else:
+        uname = args.uname
+        upass = args.upass
+        session_confirm = ""
 
     data = {"OEMProprietary_level_Privilege": 1,
             "UserOperation": 0,
             "access": args.access,
             "channel_type": 4,
             "confirm_password": upass,
             "creation_time": 0,
@@ -1317,15 +1359,15 @@
             "kvm": args.kvm,
             "name": uname,
             "changepassword": 1,
             "password": upass,
             "password_size": "bytes_16",
             "prev_snmp": 0,
             "privilege": "",
-            "session_confirm": "",
+            "session_confirm": session_confirm,
             "snmp": 0,
             "snmp_access": 0,
             "snmp_authentication_protocol": None,
             "snmp_privacy_protocol": None,
             "sol": args.sol,
             "ssh_key": "Not Available",
             "userid": args.userid,
@@ -1369,20 +1411,30 @@
         JSON['data'] = result
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/users/" + str(args.userID), response)
     return JSON
 
 
-def setUserByRestM6(client, args):
+def setUserByRestM6(client, args, ff="M6"):
     JSON = {}
     if args.uname is None or args.uname == "":
         JSON['code'] = 1
         JSON['data'] = 'uname cannot be none'
         return JSON
+    if encrypt_type_flag == 2:
+        args.json['confirm_password'] = Encrypt(args.json['confirm_password'], "addadd")
+        args.json['password'] = Encrypt(args.json['password'], "addadd")
+        args.json['session_confirm'] = Encrypt(args.json['session_confirm'], "addadd")
+        args.json['name'] = Encrypt(args.json['name'], "addadd")
+    elif encrypt_type_flag == 1:
+        args.json['confirm_password'] = encrypt_rsa(args.json['confirm_password'], client.type)
+        args.json['password'] = encrypt_rsa(args.json['password'], client.type)
+        args.json['session_confirm'] = encrypt_rsa(args.json['session_confirm'], client.type)
+        args.json['name'] = encrypt_rsa(args.json['name'], client.type)
     response = client.request("PUT", "api/settings/users/" + str(args.userid), client.getHearder(), data=None,
                               json=args.json)
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/settings/users/, response is none'
     elif response.status_code == 200:
         JSON['code'] = 0
@@ -2751,48 +2803,104 @@
             }
     except BaseException:
         headers = {}
     return headers
 
 
 def login_M6(client):
+    global encrypt_type_flag
     try:
         headers = {}
         flag = IpmiFunc.judge_encrypt(client)
         if flag == 1:
             randomtag = client.request("GET", "api/randomtag", data=None, json=None)
             if randomtag is not None and randomtag.status_code == 200 and 'random' in randomtag.json():
                 data = {
                     "username": Encrypt(client.username),
                     "password": Encrypt(client.passcode),
                     "encrypt_flag": 1,
                     "login_tag": randomtag.json().get('random')
                 }
                 response = client.request("POST", "api/session", data=data)
-                if response is not None and response.status_code == 200:
+                if response is not None and response.status_code in range(200, 300):
+                    encrypt_type_flag = 2
                     headers = {
                         "X-CSRFToken": response.json()["CSRFToken"],
                         "Cookie": response.headers["set-cookie"]
                     }
+                else:
+                    # M6 好像也没有RSA加密方式
+                    data = {
+                        "username": encrypt_rsa(client.username, client.type),
+                        "password": encrypt_rsa(client.passcode, client.type),
+                        "encrypt_flag": 1,
+                        "login_tag": randomtag.json().get('random')
+                    }
+                    response = client.request("POST", "api/session", data=data)
+                    if response is not None and response.status_code in range(200, 300):
+                        encrypt_type_flag = 1
+                        headers = {
+                            "X-CSRFToken": response.json()["CSRFToken"],
+                            "Cookie": response.headers["set-cookie"]
+                        }
         else:
             data = {
                 "username": client.username,
                 "password": client.passcode,
             }
             response = client.request("POST", "api/session", data=data)
             if response is not None and response.status_code == 200:
+                encrypt_type_flag = 0
                 headers = {
                     "X-CSRFToken": response.json()["CSRFToken"],
                     "Cookie": response.headers["set-cookie"]
                 }
     except:
         headers = {}
     return headers
 
 
+def encrypt_rsa(sourceStr, ff="M7"):
+    try:
+        if sourceStr is None or sourceStr == "":
+            return sourceStr
+        from Crypto.Cipher import PKCS1_v1_5
+        from Crypto.PublicKey import RSA
+        if ff == "M6":
+            encrypt_key = "-----BEGIN PUBLIC KEY-----\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAv03c1doV6WQiuElhNqb\n" \
+                      "WatOf/va4K7fYjKpFjgpZ+yP0GVJEUtVDBr0Ohb9RWajX1K2OvWiwc1bWpG3Nd3vdOep8edzDp7d6Z\n" \
+                      "74Pno0JG7DwJqP9zNCwJjAiPy9Yqd+TK/++JwdTQkW2CrhIF58vFIKEfMGrSCLN108rfIvBBi3Jf/3b\n" \
+                      "FM1Y+LAd+9Zza2hIbq/yKQRpVHifoa2s64c//JvC+ZW4KzXbcWXAT73IAKyZCCEyrj7r5HSn5C1rQg2\n" \
+                      "HOWJvrew8q2d5KWN+YkvDIFLMVMyVWOAJf7h0yPo5vZeGi1vM90fngh5podmMXpSGs4Pr3c9PgyQnEk9\n" \
+                      "xJgQi3QIDAQAB==\n-----END PUBLIC KEY-----"
+        # M7 & H2
+        else:
+            encrypt_key = "-----BEGIN PUBLIC KEY-----\nMIICIjANBgkqhkiG9w0BAQEFAAOCAg8AMIICCgKCAgEAvAIoJ+F0MiuinN903RNX\n"\
+                    "z4umR3b0OackykNmXP+d5qRmxfRS6ymjGwmS1hxBVkGNAulpoeqNDQ1oeilc6IOI\n"\
+                    "6QgsRDzSas4/cXY7/ndz1TK2ocBhh9bxwHfBa0STFyK8004lQ2FKjJj9zrUMC67w\n"\
+                    "U3qvU5np2pddqaIunEEExeU88ZVsNS7jBYDlN/XDdT6sqs0qAicley9ogfeRSh95\n"\
+                    "9KxCG3QnyMSNDk+Gf8Yp4z6hfc8ON1FYsQfFh3yVScvHp0UKbuhs+Mt7TjoyALel\n"\
+                    "cGY18eFt0evYT+n7arRRvdjsDfQz8mJTXYxBy5eTgIVt7s8hufuqtnVH3chkp5o1\n"\
+                    "32LiTTutoliyLsyr+uRitnYPH97vE+edESimql1112ozzs8Axjsh4ugX8YhU2jdA\n"\
+                    "BZSNz6AqfmnALbHRaaxoWinyuKRGA1LPMFSwW3pkbJ8RFqm7PJIza/IKmarqb1S1\n"\
+                    "2d9EqyWjIKD+KAnrsSRttfhgujf5qPCye3m0XhAIDC96JkRsv3x/erD8PQp69fdP\n"\
+                    "QdzTLnHTFSpzDE8KFyj3+YL99ejzxg3TW7/JAeJRX/XXAygRf/1GGOIxv1odXfOn\n"\
+                    "HOlA5ssqfj1Ch6zxEMuf/my6bz5M309pRQheNoEHBMDJlCRQPNeLN5ILw3n9c2cT\n"\
+                    "RUUIfwZlDzalqfR8zWNh0VUCAwEAAQ==\n-----END PUBLIC KEY-----"
+        if sourceStr is None:
+            return None
+        pub_key = RSA.importKey(encrypt_key)
+        pub_cipher = PKCS1_v1_5.new(pub_key)
+        cryptedStr = base64.b64encode(pub_cipher.encrypt(sourceStr.encode()))
+        cryptedStr = str(cryptedStr, encoding='utf-8')
+        return cryptedStr
+    except Exception as e:
+        return sourceStr
+
+
 def logout(client):
     try:
         responds = client.request("DELETE", "api/session", client.getHearder())
     except BaseException:
         return
     return
 
@@ -2801,42 +2909,26 @@
     list_str = []
     for word in wordstr:
         number = ord(word)
         list_str.append(str(hex(number ^ 127)[2:]))
     return "-".join(list_str)
 
 
-def Encrypt(code):
-    l = len(code)
-    if l % 8 != 0:
-        code = code + '\0' * (8 - (l % 8))
-    code = code.encode('utf-8')
-    if sys.version_info < (3, 0):
-        cl = Blowfish.new('secret', Blowfish.MODE_ECB)
-    else:
-        cl = Blowfish.new('secret'.encode('utf-8'), Blowfish.MODE_ECB)
-    encode = cl.encrypt(code)
-    cryptedStr = base64.b64encode(encode)
-    cryptedStr = cryptedStr.decode('utf-8')
-    return cryptedStr
-
-
-def Encrypt1(key, code):
+def Encrypt(code, key="secret"):
     l = len(code)
     if l % 8 != 0:
         code = code + '\0' * (8 - (l % 8))
     code = code.encode('utf-8')
     if sys.version_info < (3, 0):
         cl = Blowfish.new(key, Blowfish.MODE_ECB)
     else:
         cl = Blowfish.new(key.encode('utf-8'), Blowfish.MODE_ECB)
     encode = cl.encrypt(code)
     cryptedStr = base64.b64encode(encode)
-    cryptedStr = cryptedStr.decode('utf-8')
-    return cryptedStr
+    return str(cryptedStr, encoding='utf-8')
 
 
 def getSnmpM5ByRest(client):
     JSON = {}
     response = client.request("GET", "api/settings/netsnmpconf", client.getHearder(), None, None, None, None)
     if response is None:
         JSON['code'] = 1
@@ -2883,15 +2975,25 @@
         JSON['data'] = result
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/snmp", response)
     return JSON
 
 
-def setTrapComByRest(client, trapinfo):
+def setTrapComByRest(client, trapinfo, ff="M6"):
+    if encrypt_type_flag == 1:
+        trapinfo['SnmpTrapCfg']['Community'] = encrypt_rsa(trapinfo['SnmpTrapCfg']['Community'], client.type)
+        trapinfo['SnmpTrapCfg']['AUTHProtocol'] = encrypt_rsa(trapinfo['SnmpTrapCfg']['AUTHProtocol'], client.type)
+        trapinfo['SnmpTrapCfg']['AUTHPwd'] = encrypt_rsa(trapinfo['SnmpTrapCfg']['AUTHPwd'], client.type)
+        trapinfo['SnmpTrapCfg']['PRIVPwd'] = encrypt_rsa(trapinfo['SnmpTrapCfg']['PRIVPwd'], client.type)
+    elif encrypt_type_flag == 2:
+        trapinfo['SnmpTrapCfg']['Community'] = Encrypt(trapinfo['SnmpTrapCfg']['Community'])
+        trapinfo['SnmpTrapCfg']['AUTHProtocol'] = Encrypt(trapinfo['SnmpTrapCfg']['AUTHProtocol'])
+        trapinfo['SnmpTrapCfg']['AUTHPwd'] = Encrypt(trapinfo['SnmpTrapCfg']['AUTHPwd'])
+        trapinfo['SnmpTrapCfg']['PRIVPwd'] = Encrypt(trapinfo['SnmpTrapCfg']['PRIVPwd'])
     JSON = {}
     response = client.request("PUT", "api/settings/snmp", client.getHearder(), json=trapinfo)
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/settings/snmp, response is none'
     elif response.status_code == 200:
         result = response.json()
@@ -3410,15 +3512,14 @@
     response = client.request("GET", "api/logs/alertLog", client.getHearder(), None, None, None, None)
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/logs/alertLog, response is none'
     elif response.status_code == 200:
         JSON['code'] = 0
         result = response.json()
-        # { "logtime": "2000-01-01T08:00:54+08:00", "timestamp": 946684854, "type": "BMC", "severity": "Warning", "status": "Assert", "errorCode": "1801A101", "desc": "Time_SYNC_Fail Transition to Non-Critical from OK sync ME failed", "adviser": "Step1:Check whether NTP server is normal.\nStep2:Please contact Inspur FAE.", "id": 3 },
         loglist = []
         for item in result:
             # txbean = EventLogTXBean()
             txlog = collections.OrderedDict()
             txlog["Id"] = item["id"]
             txlog['Severity'] = item["severity"]
             txlog["EventTimestamp"] = item["logtime"]
@@ -3777,17 +3878,41 @@
             JSON['data'] = formatError("api/diagnose/bmc-reset", response)
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/diagnose/bmc-reset", response)
     return JSON
 
 
-# 开机自检代码
+def resetBMCM7(client, type):
+    JSON = {}
+    if type.upper() != "BMC" and type.upper() != "KVM":
+        JSON['code'] = 1
+        JSON['data'] = 'reset BMC or KVM only.'
+    data = {
+        "reset": type.upper(),
+        "currentuserpassword": encrypt_rsa(client.passcode)
+    }
+    response = client.request("POST", "api/diagnose/bmc-reset", client.getHearder(), json=data)
+    if response is None:
+        JSON['code'] = 1
+        JSON['data'] = 'Failed to call BMC interface api/diagnose/bmc-reset ,response is none'
+    elif response.status_code in range(200, 300):
+        try:
+            JSON["code"] = 0
+            JSON["data"] = "reset " + type + " success"
+        except:
+            JSON['code'] = 1
+            JSON['data'] = formatError("api/diagnose/bmc-reset", response)
+    else:
+        JSON['code'] = 1
+        JSON['data'] = formatError("api/diagnose/bmc-reset", response)
+    return JSON
 
 
+# 开机自检代码
 def getBiosPostCode(client):
     JSON = {}
     response = client.request("GET", "api/diagnose/bios-post-code", client.getHearder())
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/diagnose/bios-post-code,response is none'
     elif response.status_code == 200:
@@ -3965,16 +4090,18 @@
             JSON['data'] = formatError("api/settings/ldap-settings", response)
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/ldap-settings", response)
     return JSON
 
 
-def setLDAPM6(client, ldap, data_file):
+def setLDAPM6(client, ldap, data_file, ff="M6"):
     JSON = {}
+    if encrypt_type_flag == 1:
+        ldap['password'] = encrypt_rsa(ldap['password'], client.type)
     response = client.request("PUT", "api/settings/ldap-settings", client.getHearder(), json=ldap, data=data_file)
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/settings/ldap-settings ,response is none'
     elif response.status_code == 200:
         try:
             JSON["code"] = 0
@@ -4115,16 +4242,18 @@
             JSON['data'] = formatError("api/settings/active-directory-settings", response)
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/active-directory-settings", response)
     return JSON
 
 
-def setADM6(client, ldap):
+def setADM6(client, ldap, ff="M6"):
     JSON = {}
+    if encrypt_type_flag == 1:
+        ldap["secret_password"] = encrypt_rsa(ldap["secret_password"], client.type)
     response = client.request("PUT", "api/settings/active-directory-settings", client.getHearder(), json=ldap)
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/settings/active-directory-settings ,response is none'
     elif response.status_code == 200:
         try:
             JSON["code"] = 0
@@ -4618,18 +4747,28 @@
     if sys.version_info < (3, 0):
         with open(filepath.decode("utf-8"), 'rb') as f:
             content = f.read()
             m = '------{0}{1}Content-Disposition: form-data; name="fwimage"; filename="{3}" {1}Content-Type: application/octet-stream{1}{1}{2}{1}------{0}--{1}'.format(
                 'WebKitFormBoundarykbIa9fEjntByHHtE', '\r\n', content, file_name)
             header["Content-Type"] = "multipart/form-data;boundary=----WebKitFormBoundarykbIa9fEjntByHHtE"
     else:
-        m = encoder.MultipartEncoder(
-            fields={'fwimage': (file_name, open(filepath, 'rb').read(), 'application/octet-stream')},
-            boundary='----WebKitFormBoundarykbIa9fEjntByHHtE'
-        )
+        if encrypt_type_flag == 1:
+            m = encoder.MultipartEncoder(
+                fields={
+                    'fwimage': (file_name, open(filepath, 'rb').read(), 'application/octet-stream'),
+                    'currentuserpassword': encrypt_rsa(client.passcode, platform)
+
+                },
+                boundary='----WebKitFormBoundarydTPdpAwLgxeeqJki'
+            )
+        else:
+            m = encoder.MultipartEncoder(
+                fields={'fwimage': (file_name, open(filepath, 'rb').read(), 'application/octet-stream')},
+                boundary='----WebKitFormBoundarydTPdpAwLgxeeqJki'
+            )
         header["Content-Type"] = m.content_type
 
     upload = client.request("POST", "api/maintenance/hpm/firmware", data=m, headers=header, timeout=500)
     if upload is None:
         JSON["code"] = 1
         JSON["data"] = "Failed to call BMC interface api/maintenance/hpm/firmware ,response is none."
     elif upload.status_code == 200:
@@ -5324,14 +5463,30 @@
         JSON['data'] = result
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/service-sessions/" + str(id), response)
     return JSON
 
 
+def deleteSessionBMCByRestA7(client, id, data):
+    JSON = {}
+    response = client.request("DELETE", "api/settings/service-sessions/" + str(id), client.getHearder(), json=data)
+    if response is None:
+        JSON['code'] = 1
+        JSON['data'] = 'Failed to call BMC interface api/settings/service-sessions/, response is none'
+    elif response.status_code in range(200, 300):
+        JSON['code'] = 0
+        result = response.json()
+        JSON['data'] = result
+    else:
+        JSON['code'] = 1
+        JSON['data'] = formatError("api/settings/service-sessions/" + str(id), response)
+    return JSON
+
+
 def getHddBMCByRest(client):
     JSON = {}
     header = client.getHearder()
     response = client.request("GET", "api/status/SATA_HDDinfo", header, None, None, None, timeout=500)
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/status/SATA_HDDinfo, response is none'
@@ -5455,16 +5610,21 @@
         JSON['data'] = result
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/smtpcfg", response)
     return JSON
 
 
-def setSMTPByRest(client, smtpinfo):
+def setSMTPByRest(client, smtpinfo, ff="M6"):
     JSON = {}
+    # flag = judge_encrypt(client)
+    if encrypt_type_flag == 1:
+        smtpinfo["SmtpCfg"]["PassWord"] = encrypt_rsa(smtpinfo["SmtpCfg"]["PassWord"], client.type)
+    elif encrypt_type_flag == 2:
+        smtpinfo["SmtpCfg"]["PassWord"] = Encrypt(smtpinfo["SmtpCfg"]["PassWord"], "addadd")
     response = client.request("PUT", "api/settings/smtpcfg", client.getHearder(), json=smtpinfo)
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/settings/smtpcfg, response is none'
     elif response.status_code == 200:
         result = response.json()
         JSON['code'] = 0
@@ -5487,16 +5647,24 @@
         JSON['data'] = result
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/snmpconf", response)
     return JSON
 
 
-def setSNMPByRest(client, smtpinfo):
+def setSNMPByRest(client, smtpinfo, ff="M6"):
     JSON = {}
+    if encrypt_type_flag == 1:
+        smtpinfo['SnmpCfg']['AUTHProtocol'] = encrypt_rsa(smtpinfo['SnmpCfg']['AUTHProtocol'], client.type)
+        smtpinfo['SnmpCfg']['AUTHPwd'] = encrypt_rsa(smtpinfo['SnmpCfg']['AUTHPwd'], client.type)
+        smtpinfo['SnmpCfg']['PRIVPwd'] = encrypt_rsa(smtpinfo['SnmpCfg']['PRIVPwd'], client.type)
+        smtpinfo['SnmpCfg']['ReadOnlyCommunity'] = encrypt_rsa(smtpinfo['SnmpCfg']['ReadOnlyCommunity'], client.type)
+        smtpinfo['SnmpCfg']['ReadWriteCommunity'] = encrypt_rsa(smtpinfo['SnmpCfg']['ReadWriteCommunity'], client.type)
+        smtpinfo['SnmpCfg']['ConfirmReadOnlyCommunity'] = encrypt_rsa(smtpinfo['SnmpCfg']['ConfirmReadOnlyCommunity'], client.type)
+        smtpinfo['SnmpCfg']['ConfirmReadWriteCommunity'] = encrypt_rsa(smtpinfo['SnmpCfg']['ConfirmReadWriteCommunity'], client.type)
     response = client.request("PUT", "api/settings/snmpconf", client.getHearder(), json=smtpinfo)
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/settings/snmpconf, response is none'
     elif response.status_code == 200:
         result = response.json()
         JSON['code'] = 0
@@ -7653,15 +7821,15 @@
     return JSON
 
 
 # PFR security check
 def securityCheckByRest(client):
     JSON = {}
     data = {
-        "currentuserpassword": Encrypt1(client.passcode, "addadd")
+        "currentuserpassword": Encrypt(client.passcode, "addadd")
     }
     response = client.request("PUT", "api/maintenance/hpm/security_check", client.getHearder(), json=data)
     if response is None:
         JSON['code'] = 1
         JSON['data'] = 'Failed to call BMC interface api/maintenance/hpm/security_check, response is none'
     elif response.status_code == 200:
         JSON['code'] = 0
@@ -7812,14 +7980,30 @@
             JSON['data'] = formatError("api/settings/snmp", response)
     else:
         JSON['code'] = 1
         JSON['data'] = formatError("api/settings/snmp", response)
     return JSON
 
 
+def getgpu(client):
+    JSON = {}
+    response = client.request("GET", "api/gpu/gpu_info", client.getHearder(), None, None, None, None)
+    if response is None:
+        JSON['code'] = 1
+        JSON['data'] = 'Failed to call BMC interface api/gpu/gpu_info, response is none'
+    elif response.status_code in range(200, 300):
+        result = response.json()
+        JSON['code'] = 0
+        JSON['data'] = result
+    else:
+        JSON['code'] = 1
+        JSON['data'] = formatError("api/gpu/gpu_info", response)
+    return JSON
+
+
 class NF5280M5_SensorDesc():
 
     def __init__(self):
         command_path = os.path.dirname(os.path.realpath(__file__))
         ipmi_path = os.path.join(command_path, "M5Log")
         sys.path.append(ipmi_path)
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/backup.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/backup.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/A7.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/A7.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M4.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M4.xml`

 * *Files 0% similar despite different names*

#### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M4.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M4.xml`

```diff
@@ -375,15 +375,14 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3e 0x21 0x27 0x00 0x01</getter>
       <setters>
         <setter>
           <cmd>raw 0x3e 0x20 0x27 0x00 $in</cmd>
           <value>0~24</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validatePatrolScrubInterval</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Restore AC Power Loss</description>
         <belongto>Chipset</belongto>
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M5.xml`

 * *Files 1% similar despite different names*

#### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M5.xml`

```diff
@@ -944,15 +944,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xDA</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xDA $in</cmd>
           <value>0~3</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateM5LegacyVgaSocket</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Enforce POR</description>
         <belongto>Processor</belongto>
@@ -1273,15 +1272,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF1 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>SDDC/SDDC Plus One</description>
         <belongto>Processor</belongto>
@@ -1338,15 +1336,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF7</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF7 $in</cmd>
           <value>0 ~ 24</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validatePatrolScrubInterval</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>FRB-2 Timer</description>
         <belongto>ServerMgmt</belongto>
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6-N.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M6-N.xml`

 * *Files 0% similar despite different names*

#### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6-N.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M6-N.xml`

```diff
@@ -1593,15 +1593,14 @@
         <location>Socket Configuration/Processor Configuration/Core Disable Number</location>
       </name>
       <getter>CoreEn</getter>
       <setters>
         <setter>
           <cmd>$in</cmd>
           <value>0~38</value>
-          <validation>com.inspur.ism.server.service.bios.BiosItemValueValidate.validateWaitTime</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Memory Frequency</description>
         <belongto>Processor</belongto>
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M6.xml`

 * *Files 0% similar despite different names*

#### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M6.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M6.xml`

```diff
@@ -1592,15 +1592,14 @@
         <location>Socket Configuration/Processor Configuration/Core Disable Number</location>
       </name>
       <getter>CoreEn</getter>
       <setters>
         <setter>
           <cmd>$in</cmd>
           <value>$in:0~38</value>
-          <validation>com.inspur.ism.server.service.bios.BiosItemValueValidate.validateWaitTime</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Memory Frequency</description>
         <belongto>Processor</belongto>
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M7.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M7.xml`

 * *Files 0% similar despite different names*

#### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/M7.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/M7.xml`

```diff
@@ -160,15 +160,14 @@
     </cfgItem>
     <cfgItem>
       <name>
         <description>Static Turbo Mode</description>
         <belongto>Processor</belongto>
         <location>Socket Configuration-Advanced Power Management Configuration-Hardware PM State Control</location>
       </name>
-      <parent>InspurSocketSetup</parent>
       <getter>ControlTurboPStatus</getter>
       <conditions>
         <condition>
           <key>PowerProfile</key>
           <value>CUSTOM</value>
         </condition>
       </conditions>
@@ -217,15 +216,14 @@
       <name>
         <description>Power/Performance Profile</description>
         <belongto>Processor</belongto>
         <location>Socket Configuration-Advanced Power Management Configuration-Power and Perfromance Profile
                     Configuration</location>
         <!--CustomID为快手时选项隐藏-->
       </name>
-      <parent>InspurSocketSetup</parent>
       <getter>PowerProfile</getter>
       <setters>
         <setter>
           <cmd>HIGH_PERFORMANCE_COMPUTE</cmd>
           <value>High Performance Compute</value>
         </setter>
         <setter>
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF3180A6.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF3180A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF3280A6.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF3280A6.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5180M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5280M5.xml`

 * *Files 0% similar despite different names*

#### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5180M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5280M5.xml`

```diff
@@ -567,29 +567,27 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x28</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x28 $in</cmd>
           <value>0 ~ 5</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Media detect count</description>
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x29</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x29 $in</cmd>
           <value>1 ~ 50</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CSM Support</description>
         <belongto>Advanced</belongto>
@@ -1759,16 +1757,14 @@
         </setter>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x64 0x01 0x00</cmd>
           <value>Skip</value>
         </setter>
       </setters>
     </cfgItem>
-    <!--与文档不匹配-->
-    <!--至此与文档不匹配-->
     <cfgItem>
       <name>
         <description>Restore AC Power Loss</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x65</getter>
       <setters>
@@ -1860,29 +1856,27 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x6A</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x6A $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MCTP Bus Owner</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x6B</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x6B $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>System Errors</description>
         <belongto>Chipset</belongto>
@@ -2440,15 +2434,14 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x8C</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x8C $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Spare Interrupt</description>
         <belongto>Chipset</belongto>
@@ -3065,29 +3058,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xB0</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xB0 $in</cmd>
           <value>0 ~ 0x3F</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PCIE Corrected Error Threshold</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xB1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xB1 $in</cmd>
           <value>0 ~ 0x7FFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PCIE AER Corrected Errors</description>
         <belongto>Chipset</belongto>
@@ -4130,15 +4121,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF1 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>SDDC/SDDC Plus One</description>
         <belongto>Processor</belongto>
@@ -4195,15 +4185,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF5</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF5 $in</cmd>
           <value>0~255</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateLegacyVGAStack</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Patrol Scrub</description>
         <belongto>Processor</belongto>
@@ -4226,15 +4215,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF7</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF7 $in</cmd>
           <value>0 ~ 24</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validatePatrolScrubInterval</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Patrol Scrub Address Mode</description>
         <belongto>Processor</belongto>
@@ -4524,14 +4512,18 @@
           <cmd>raw 0x3c 0x48 0x01 0x0D 0x04 0x00</cmd>
           <value>Option 4</value>
         </setter>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x0D 0x05 0x00</cmd>
           <value>Option 5</value>
         </setter>
+        <setter>
+          <cmd>raw 0x3c 0x48 0x01 0x0D 0x06 0x00</cmd>
+          <value>Auto(V)</value>
+        </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Socket0 IOU0(IIO PCIe Br1)</description>
         <belongto>Processor</belongto>
       </name>
@@ -6916,15 +6908,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x7D</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x7D $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -6943,15 +6934,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x7F</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x7F $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -6978,15 +6968,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x81</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x81 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -7119,15 +7108,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x89</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x89 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7146,15 +7134,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x8B</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x8B $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7181,15 +7168,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x8D</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x8D $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7322,15 +7308,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x95</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x95 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7349,15 +7334,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x97</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x97 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7384,15 +7368,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x99</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x99 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7525,15 +7508,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA1 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7552,15 +7534,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA3</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA3 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7587,15 +7568,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA5</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA5 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7728,15 +7708,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xAD</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xAD $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7755,15 +7734,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xAF</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xAF $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7790,15 +7768,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xB1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xB1 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7931,15 +7908,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xB9</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xB9 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -7958,15 +7934,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xBB</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xBB $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -7993,15 +7968,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xBD</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xBD $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -8915,29 +8889,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF0</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF0 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL1 Time Window</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF1 $in</cmd>
           <value>0 ~ 56</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL2 Limit</description>
         <belongto>Processor</belongto>
@@ -8960,29 +8932,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF3</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF3 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL2 Time Window</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF4</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF4 $in</cmd>
           <value>0 ~ 56</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Monitor/Mwait Support</description>
         <belongto>Processor</belongto>
@@ -9317,29 +9287,27 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x02 0x06</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x02 0x06 $in</cmd>
           <value>0~100</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Setup Prompt Timeout</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x02 0x0F</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x02 0x0F $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Bootup NumLock State</description>
         <belongto>Boot</belongto>
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5280M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5180M5.xml`

 * *Files 0% similar despite different names*

#### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5280M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5180M5.xml`

```diff
@@ -567,29 +567,27 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x28</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x28 $in</cmd>
           <value>0 ~ 5</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Media detect count</description>
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x29</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x29 $in</cmd>
           <value>1 ~ 50</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CSM Support</description>
         <belongto>Advanced</belongto>
@@ -1759,14 +1757,16 @@
         </setter>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x64 0x01 0x00</cmd>
           <value>Skip</value>
         </setter>
       </setters>
     </cfgItem>
+    <!--与文档不匹配-->
+    <!--至此与文档不匹配-->
     <cfgItem>
       <name>
         <description>Restore AC Power Loss</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x65</getter>
       <setters>
@@ -1858,29 +1858,27 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x6A</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x6A $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MCTP Bus Owner</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x6B</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x6B $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>System Errors</description>
         <belongto>Chipset</belongto>
@@ -2438,15 +2436,14 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x8C</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x8C $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Spare Interrupt</description>
         <belongto>Chipset</belongto>
@@ -3063,29 +3060,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xB0</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xB0 $in</cmd>
           <value>0 ~ 0x3F</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PCIE Corrected Error Threshold</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xB1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xB1 $in</cmd>
           <value>0 ~ 0x7FFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PCIE AER Corrected Errors</description>
         <belongto>Chipset</belongto>
@@ -4128,15 +4123,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF1 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>SDDC/SDDC Plus One</description>
         <belongto>Processor</belongto>
@@ -4193,15 +4187,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF5</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF5 $in</cmd>
           <value>0~255</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateLegacyVGAStack</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Patrol Scrub</description>
         <belongto>Processor</belongto>
@@ -4224,15 +4217,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF7</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF7 $in</cmd>
           <value>0 ~ 24</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validatePatrolScrubInterval</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Patrol Scrub Address Mode</description>
         <belongto>Processor</belongto>
@@ -4522,18 +4514,14 @@
           <cmd>raw 0x3c 0x48 0x01 0x0D 0x04 0x00</cmd>
           <value>Option 4</value>
         </setter>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x0D 0x05 0x00</cmd>
           <value>Option 5</value>
         </setter>
-        <setter>
-          <cmd>raw 0x3c 0x48 0x01 0x0D 0x06 0x00</cmd>
-          <value>Auto(V)</value>
-        </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Socket0 IOU0(IIO PCIe Br1)</description>
         <belongto>Processor</belongto>
       </name>
@@ -6918,15 +6906,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x7D</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x7D $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -6945,15 +6932,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x7F</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x7F $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -6980,15 +6966,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x81</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x81 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -7121,15 +7106,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x89</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x89 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7148,15 +7132,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x8B</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x8B $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7183,15 +7166,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x8D</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x8D $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7324,15 +7306,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x95</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x95 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7351,15 +7332,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x97</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x97 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7386,15 +7366,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x99</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x99 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7527,15 +7506,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA1 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7554,15 +7532,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA3</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA3 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7589,15 +7566,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA5</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA5 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7730,15 +7706,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xAD</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xAD $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7757,15 +7732,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xAF</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xAF $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7792,15 +7766,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xB1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xB1 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7933,15 +7906,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xB9</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xB9 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -7960,15 +7932,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xBB</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xBB $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -7995,15 +7966,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xBD</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xBD $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -8917,29 +8887,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF0</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF0 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL1 Time Window</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF1 $in</cmd>
           <value>0 ~ 56</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL2 Limit</description>
         <belongto>Processor</belongto>
@@ -8962,29 +8930,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF3</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF3 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL2 Time Window</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF4</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF4 $in</cmd>
           <value>0 ~ 56</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Monitor/Mwait Support</description>
         <belongto>Processor</belongto>
@@ -9319,29 +9285,27 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x02 0x06</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x02 0x06 $in</cmd>
           <value>0~100</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Setup Prompt Timeout</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x02 0x0F</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x02 0x0F $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Bootup NumLock State</description>
         <belongto>Boot</belongto>
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5468A5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5468A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/NF5488A5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/NF5488A5.xml`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5112M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/SA5112M5.xml`

 * *Files 0% similar despite different names*

#### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5112M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/SA5112M5.xml`

```diff
@@ -567,29 +567,27 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x28</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x28 $in</cmd>
           <value>0 ~ 5</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Media detect count</description>
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x29</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x29 $in</cmd>
           <value>1 ~ 50</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CSM Support</description>
         <belongto>Advanced</belongto>
@@ -1860,29 +1858,27 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x6A</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x6A $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MCTP Bus Owner</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x6B</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x6B $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>System Errors</description>
         <belongto>Chipset</belongto>
@@ -2440,15 +2436,14 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x8C</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x8C $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Spare Interrupt</description>
         <belongto>Chipset</belongto>
@@ -3065,29 +3060,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xB0</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xB0 $in</cmd>
           <value>0 ~ 0x3F</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PCIE Corrected Error Threshold</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xB1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xB1 $in</cmd>
           <value>0 ~ 0x7FFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PCIE AER Corrected Errors</description>
         <belongto>Chipset</belongto>
@@ -4130,15 +4123,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF1 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>SDDC/SDDC Plus One</description>
         <belongto>Processor</belongto>
@@ -4195,15 +4187,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF5</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF5 $in</cmd>
           <value>0~255</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateLegacyVGAStack</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Patrol Scrub</description>
         <belongto>Processor</belongto>
@@ -4226,15 +4217,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF7</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF7 $in</cmd>
           <value>0 ~ 24</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validatePatrolScrubInterval</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Patrol Scrub Address Mode</description>
         <belongto>Processor</belongto>
@@ -6920,15 +6910,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x7D</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x7D $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -6947,15 +6936,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x7F</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x7F $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -6982,15 +6970,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x81</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x81 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -7123,15 +7110,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x89</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x89 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7150,15 +7136,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x8B</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x8B $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7185,15 +7170,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x8D</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x8D $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7326,15 +7310,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x95</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x95 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7353,15 +7336,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x97</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x97 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7388,15 +7370,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x99</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x99 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7529,15 +7510,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA1 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7556,15 +7536,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA3</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA3 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7591,15 +7570,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA5</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA5 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7732,15 +7710,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xAD</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xAD $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7759,15 +7736,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xAF</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xAF $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7794,15 +7770,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xB1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xB1 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7935,15 +7910,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xB9</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xB9 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -7962,15 +7936,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xBB</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xBB $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -7997,15 +7970,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xBD</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xBD $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -8919,29 +8891,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF0</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF0 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL1 Time Window</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF1 $in</cmd>
           <value>0 ~ 56</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL2 Limit</description>
         <belongto>Processor</belongto>
@@ -8964,29 +8934,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF3</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF3 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL2 Time Window</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF4</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF4 $in</cmd>
           <value>0 ~ 56</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Monitor/Mwait Support</description>
         <belongto>Processor</belongto>
@@ -9321,29 +9289,27 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x02 0x06</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x02 0x06 $in</cmd>
           <value>0~100</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Setup Prompt Timeout</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x02 0x0F</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x02 0x0F $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Bootup NumLock State</description>
         <belongto>Boot</belongto>
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5212M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/SA5212M5.xml`

 * *Files 0% similar despite different names*

#### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/bios/SA5212M5.xml` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/bios/SA5212M5.xml`

```diff
@@ -567,29 +567,27 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x28</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x28 $in</cmd>
           <value>0 ~ 5</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Media detect count</description>
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x29</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x29 $in</cmd>
           <value>1 ~ 50</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CSM Support</description>
         <belongto>Advanced</belongto>
@@ -1858,29 +1856,27 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x6A</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x6A $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MCTP Bus Owner</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x6B</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x6B $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>System Errors</description>
         <belongto>Chipset</belongto>
@@ -2438,15 +2434,14 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0x8C</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0x8C $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Spare Interrupt</description>
         <belongto>Chipset</belongto>
@@ -3063,29 +3058,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xB0</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xB0 $in</cmd>
           <value>0 ~ 0x3F</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PCIE Corrected Error Threshold</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xB1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xB1 $in</cmd>
           <value>0 ~ 0x7FFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PCIE AER Corrected Errors</description>
         <belongto>Chipset</belongto>
@@ -4128,15 +4121,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF1 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>SDDC/SDDC Plus One</description>
         <belongto>Processor</belongto>
@@ -4193,15 +4185,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF5</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF5 $in</cmd>
           <value>0~255</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateLegacyVGAStack</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Patrol Scrub</description>
         <belongto>Processor</belongto>
@@ -4224,15 +4215,14 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x00 0xF7</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x00 0xF7 $in</cmd>
           <value>0 ~ 24</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validatePatrolScrubInterval</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Patrol Scrub Address Mode</description>
         <belongto>Processor</belongto>
@@ -6918,15 +6908,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x7D</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x7D $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -6945,15 +6934,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x7F</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x7F $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -6980,15 +6968,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x81</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x81 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket0-1)</description>
         <belongto>Processor</belongto>
@@ -7121,15 +7108,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x89</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x89 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7148,15 +7134,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x8B</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x8B $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7183,15 +7168,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x8D</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x8D $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket0-2)</description>
         <belongto>Processor</belongto>
@@ -7324,15 +7308,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x95</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x95 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7351,15 +7334,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x97</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x97 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7386,15 +7368,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0x99</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0x99 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 0-3)</description>
         <belongto>Processor</belongto>
@@ -7527,15 +7508,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA1 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7554,15 +7534,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA3</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA3 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7589,15 +7568,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xA5</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xA5 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-1)</description>
         <belongto>Processor</belongto>
@@ -7730,15 +7708,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xAD</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xAD $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7757,15 +7734,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xAF</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xAF $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7792,15 +7768,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xB1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xB1 $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-2)</description>
         <belongto>Processor</belongto>
@@ -7933,15 +7908,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xB9</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xB9 $in</cmd>
           <value>20 ~ 27</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>CfgBar attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -7960,15 +7934,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xBB</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xBB $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar1 attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -7995,15 +7968,14 @@
         <belongto>Advanced</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xBD</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xBD $in</cmd>
           <value>20 ~ 39</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>MemBar2 attribute(Socket 1-3)</description>
         <belongto>Processor</belongto>
@@ -8917,29 +8889,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF0</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF0 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL1 Time Window</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF1</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF1 $in</cmd>
           <value>0 ~ 56</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL2 Limit</description>
         <belongto>Processor</belongto>
@@ -8962,29 +8932,27 @@
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF3</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF3 $in</cmd>
           <value>0 ~ 32767</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>PL2 Time Window</description>
         <belongto>Processor</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x01 0xF4</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x01 0xF4 $in</cmd>
           <value>0 ~ 56</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Monitor/Mwait Support</description>
         <belongto>Processor</belongto>
@@ -9319,29 +9287,27 @@
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x02 0x06</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x02 0x06 $in</cmd>
           <value>0~100</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Setup Prompt Timeout</description>
         <belongto>Chipset</belongto>
       </name>
       <getter>raw 0x3c 0x49 0x02 0x0F</getter>
       <setters>
         <setter>
           <cmd>raw 0x3c 0x48 0x02 0x0F $in</cmd>
           <value>0~0xFFFF</value>
-          <validation>com.inspur.isa.biosconfig.service.BiosItemValueValidate.validateCorrectableErrorThreshold</validation>
         </setter>
       </setters>
     </cfgItem>
     <cfgItem>
       <name>
         <description>Bootup NumLock State</description>
         <belongto>Boot</belongto>
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/command/restore.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/command/restore.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/Base.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/Base.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,75 +66,75 @@
             product = fru
             frubean = collections.OrderedDict()
             if product.get('Product Name', None):
                 frubean["FRUName"] = product['Product Name']
             else:
                 frubean["FRUName"] = None
 
-            if product['Chassis Type']:
+            if 'Chassis Type' in product:
                 frubean["ChassisType"] = product['Chassis Type']
             else:
                 frubean["ChassisType"] = None
 
-            if product['Chassis Part Number']:
+            if 'Chassis Part Number' in product:
                 frubean["ChassisPartNumber"] = product['Chassis Part Number']
             else:
                 frubean["ChassisPartNumber"] = None
 
-            if product['Chassis Serial']:
+            if 'Chassis Serial' in product:
                 frubean["ChassisSerial"] = product['Chassis Serial']
             else:
                 frubean["ChassisSerial"] = None
 
-            if product['Board Mfg']:
+            if 'Board Mfg' in product:
                 frubean["BoardMfg"] = product['Board Mfg']
             else:
                 frubean["BoardMfg"] = None
 
-            if product['Board Product']:
+            if 'Board Product' in product:
                 frubean["BoardProduct"] = product['Board Product']
             else:
                 frubean["BoardProduct"] = None
 
-            if product['Board Serial']:
+            if 'Board Serial' in product:
                 frubean["BoardSerial"] = product['Board Serial']
             else:
                 frubean["BoardSerial"] = None
 
-            if product['Board Part Number']:
+            if 'Board Part Number' in product:
                 frubean["BoardPartNumber"] = product['Board Part Number']
             else:
                 frubean["BoardPartNumber"] = None
 
-            if product['Product Manufacturer']:
+            if 'Product Manufacturer' in product:
                 frubean["ProductManufacturer"] = product['Product Manufacturer']
             else:
                 frubean["ProductManufacturer"] = None
 
-            if product['Product Name']:
+            if 'Product Name' in product:
                 frubean["ProductName"] = product['Product Name']
             else:
                 frubean["ProductName"] = None
 
-            if product['Product Part Number']:
+            if 'Product Part Number' in product:
                 frubean["ProductPartNumber"] = product['Product Part Number']
             else:
                 frubean["ProductPartNumber"] = None
 
-            if product.get('Product Version', None):
+            if 'Product Version' in product:
                 frubean["ProductVersion"] = product['Product Version']
             else:
                 frubean["ProductVersion"] = None
 
-            if product['Product Serial']:
+            if 'Product Serial' in product:
                 frubean["ProductSerial"] = product['Product Serial']
             else:
                 frubean["ProductSerial"] = None
 
-            if product['Product Asset Tag']:
+            if 'Product Asset Tag' in product:
                 frubean["ProductAssetTag"] = product['Product Asset Tag']
             else:
                 frubean["ProductAssetTag"] = None
 
             FRUlist.append(frubean)
             FRU = [{"FRU": FRUlist}]
             res.State('Success')
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA5.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonA5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA6.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonA6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonA7.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonA7.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM5.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM5.py`

 * *Files 0% similar despite different names*

```diff
@@ -11750,15 +11750,15 @@
                 px[item['slotNum']] = item['devId']
         return pd, pv, px
     else:
         return [], {}, {}
 
 
 def createVirtualDrive(client, args):
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         result = showpdInfo(client, args)
         return result
     result = ResultBean()
     if args.ctrlId is None or args.access is None or args.cache is None or args.init is None \
             or args.rlevel is None or args.slot is None or args.size is None or args.r is None or \
             args.w is None or args.io is None or args.select is None:
         result.State('Failure')
@@ -12102,15 +12102,15 @@
         result.State('Failure')
         result.Message(
             ["Device information Not Available (Device absent or failed to get)!"])
         return result
     elif raidtype == '00' or raidtype == '02' or raidtype == '03':
         result = setLogicalDrive_LSI(args, client)
     elif raidtype == 'ff':
-        if args.Info is not None:
+        if 'Info' in args and args.Info is not None:
             raidDict = {}
             LSIresult = showLogicalInfo_LSI(client, args)
             if LSIresult.State == 'Success':
                 LSI = LSIresult.Message
                 raidDict['LSI'] = LSI
             else:
                 return LSIresult
@@ -12133,15 +12133,15 @@
                 'Failure: failed to establish connection to the host, please check the user/passcode/host/port',
                 'usage: isrest [-h] [-V] -H HOST -U USERNAME -P PASSWORD -p PORT subcommand ...'])
         return result
     return result
 
 
 def setLogicalDrive_LSI(args, client):
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         result = showLogicalInfo_LSI(client, args)
         return result
     else:
         cid, vd = getLogicalInfo_LSI(client, args)
 
     result = ResultBean()
     if args.ctrlId is None or args.ldiskId is None or args.option is None:
@@ -12397,15 +12397,15 @@
         result.State('Failure')
         result.Message(
             ["Device information Not Available (Device absent or failed to get)!"])
         return result
     elif raidtype == '00' or raidtype == '02' or raidtype == '03':
         result = setPhysicalDrive_LSI(args, client)
     elif raidtype == 'ff':
-        if args.Info is not None:
+        if 'Info' in args and args.Info is not None:
             raidDict = {}
             LSIresult = showPhysicalInfo_LSI(args, client)
             if LSIresult.State == 'Success':
                 LSI = LSIresult.Message
                 raidDict['LSI'] = LSI
             else:
                 return LSIresult
@@ -12425,15 +12425,15 @@
         result.Message(["get raid type error."])
         return result
     return result
 
 
 def setPhysicalDrive_LSI(args, client):
     result = ResultBean()
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         result = showPhysicalInfo_LSI(client, args)
         return result
     else:
         cid, pd = getPhysicalInfo_LSI(client, args)
     if args.ctrlId is None or args.deviceId is None or args.option is None:
         result.State('Failure')
         result.Message(["argument ctrl_id, device_id or option is missing"])
@@ -17402,15 +17402,15 @@
     result.State('Success')
     result.Message([gpu_info])
     return result
 
 
 def printGPUInfo(responds, args, gpuinfo):
     result = ResultBean()
-    args.hostType = args.hostPlatform
+    args.hostType = args.productName
     if responds is None:
         result.State('Failure')
         result.Message('GPU information request failed!')
         return result
     elif responds.status_code == 200:
         result = responds.json()
         dict = DICTVALUE()  # 实例化对象
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM6.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,17 @@
     NCSIBean,
     DNSBean,
     SessionBean,
     SensorBean,
     Sensor,
     FruBean,
     PowerConsumptionBean,
-    SuspendBean)
+    SuspendBean,
+    HBABean,
+    HBAPost)
 retry_count = 0
 
 
 class CommonM6(Base):
 
     def getcapabilities(self, client, args):
         res = ResultBean()
@@ -909,52 +911,68 @@
                 errorinfo = ",".join(errorlist)
                 errordict[bios_dict.get(bioskey)]=errorinfo
         if errordict == {}:
             return True, None
         else:
             return False, errordict
 
-    def setbios(self, client, args):
-        def update_infoList(infoList):
-            flag = False
-            attr_result = RedfishFunc.getBIOSAttrByRedfish(client, login_header)
-            if "code" in attr_result and attr_result.get('code') == 0 and attr_result.get('data') != "":
-                json_url = attr_result.get('data')
-                json_result = RedfishFunc.getBIOSAttrJsonByRedfish(client, login_header, json_url)
-                if "code" in json_result and json_result.get('code') == 0 and json_result.get('data') != {}:
-                    flag = True
-                    json_data = json_result.get('data')
-                    if "UefiBootOrder1" in json_data.keys():
-                        item_value = json_data.get("UefiBootOrder1")
-                        for item_1 in infoList:
-                            if item_1.get('getter') == "UefiBootOrder1" or \
-                                    item_1.get('getter') == "UefiBootOrder2" or \
-                                    item_1.get('getter') == "UefiBootOrder3" or \
-                                    item_1.get('getter') == "UefiBootOrder4":
-                                setter_list = []
-                                for item_2 in item_value:
-                                    setter_list.append(
-                                        {"cmd": item_2.get("ValueName"), "value": item_2.get("ValueName")})
-                                item_1['setter'] = setter_list
-                    elif "LegacyBootOrder1" in json_data.keys():
-                        item_value = json_data.get("LegacyBootOrder1")
-                        for item_1 in infoList:
-                            if item_1.get('getter') == "LegacyBootOrder1" or \
-                                    item_1.get('getter') == "LegacyBootOrder2" or \
-                                    item_1.get('getter') == "LegacyBootOrder3" or \
-                                    item_1.get('getter') == "LegacyBootOrder4":
-                                setter_list = []
-                                for item_2 in item_value:
-                                    setter_list.append(
-                                        {"cmd": item_2.get("ValueName"), "value": item_2.get("ValueName")})
-                                item_1['setter'] = setter_list
-            return flag, infoList
+    def getXmlFileName(self, res):
+        xml_path = os.path.join(IpmiFunc.command_path, "bios") + os.path.sep
+        if "IioVmdOnStackPch" in res.keys():
+            xmlfilepath = xml_path + "M6-N.xml"
+        else:
+            xmlfilepath = xml_path + "M6.xml"
+        return xmlfilepath
+
+    def update_xmlinfo(self, client, login_header, xmlhelp):
+        Bios_result = ResultBean()
+        attr_result = RedfishFunc.getBIOSAttrByRedfish(client, login_header)
+        if attr_result.get('code') == 0:
+            json_url = attr_result.get('data')
+            json_result = RedfishFunc.getBIOSAttrJsonByRedfish(client, login_header, json_url)
+            if json_result.get('code') == 0:
+                json_data = json_result.get('data')
+                if "UefiBootOrder1" in json_data.keys():
+                    item_value = json_data.get("UefiBootOrder1")
+                    for item_1 in xmlhelp:
+                        if item_1.get('getter') == "UefiBootOrder1" or \
+                                item_1.get('getter') == "UefiBootOrder2" or \
+                                item_1.get('getter') == "UefiBootOrder3" or \
+                                item_1.get('getter') == "UefiBootOrder4":
+                            setter_list = []
+                            for item_2 in item_value:
+                                setter_list.append(
+                                    {"cmd": item_2.get("ValueName"), "value": item_2.get("ValueName")})
+                            item_1['setter'] = setter_list
+                elif "LegacyBootOrder1" in json_data.keys():
+                    item_value = json_data.get("LegacyBootOrder1")
+                    for item_1 in xmlhelp:
+                        if item_1.get('getter') == "LegacyBootOrder1" or \
+                                item_1.get('getter') == "LegacyBootOrder2" or \
+                                item_1.get('getter') == "LegacyBootOrder3" or \
+                                item_1.get('getter') == "LegacyBootOrder4":
+                            setter_list = []
+                            for item_2 in item_value:
+                                setter_list.append(
+                                    {"cmd": item_2.get("ValueName"), "value": item_2.get("ValueName")})
+                            item_1['setter'] = setter_list
+                Bios_result.State('Success')
+                Bios_result.Message([xmlhelp])
+            else:
+                Bios_result.State('Failure')
+                Bios_result.Message([str(json_result.get('data'))])
+        else:
+            Bios_result.State('Failure')
+            Bios_result.Message([str(attr_result.get('data'))])
 
+        return Bios_result
+
+    def setbios(self, client, args):
         Bios_result = ResultBean()
-        # args.list = False
+        # 不输入-L
         if 'list' not in args or ('list' in args and args.list is False):
             if args.attribute is None and args.value is None and args.fileurl is None:
                 Bios_result.Message(['please input a command at least.'])
                 Bios_result.State('Failure')
                 return Bios_result
             elif args.attribute is None and args.value is None and args.fileurl is not None:
                 if not os.path.exists(args.fileurl) or not os.path.isfile(args.fileurl):
@@ -984,34 +1002,29 @@
             Bios_result.Message(['login session service failed, please check username/password/host/port'])
             return Bios_result
         data = {'Attributes': {}}
         result = RedfishFunc.getBiosV1ByRedfish(client, login_header)
         boot_option = ['UEFIBootOption1', 'UEFIBootOption2', 'UEFIBootOption3', 'UEFIBootOption4', 'LegacyBootOption1',
                        'LegacyBootOption2', 'LegacyBootOption3', 'LegacyBootOption4']
         if result.get('code') == 0 and result.get('data') is not None:
-            xml_path = os.path.join(IpmiFunc.command_path, "bios") + os.path.sep
-            if "IioVmdOnStackPch" in result.get('data').keys():
-                xmlfilepath = xml_path + "M6-N.xml"
-                xmlfilename = "M6-N.xml"
-            else:
-                xmlfilepath = xml_path + "M6.xml"
-                xmlfilename = "M6.xml"
+            xmlfilepath = self.getXmlFileName(result.get('data'))
             if os.path.exists(xmlfilepath) is False:
-                Bios_result.Message([str(xmlfilename) + ' file not exist.'])
+                Bios_result.Message([os.path.basename(xmlfilepath) + ' file not exist.'])
                 Bios_result.State('Failure')
                 RedfishFunc.logout(client, login_id, login_header)
                 return Bios_result
             biosconfutil = configUtil.configUtil()  # 实例化类对象
             blongtoSet, descriptionList, infoList = biosconfutil.getSetOption(xmlfilepath)  # 读取xml文件，返回信息
-            flag, infoList = update_infoList(infoList)
-            if not flag:
+            updateresult = self.update_xmlinfo(client, login_header, infoList)
+            if updateresult.State != "Success":
                 Bios_result.Message(["get BIOS attribute failed."])
                 Bios_result.State('Failure')
                 RedfishFunc.logout(client, login_id, login_header)
-                return Bios_result
+                return updateresult
+            infoList = updateresult.Message[0]
             if 'list' in args and args.list:
                 help_list = []
                 for info in infoList:
                     help_list.append('{:<35}: {}'.format(info['description'], list(item.get('value') for item in info.get('setter'))))
                 Bios_result.Message(help_list)
                 Bios_result.State('Success')
                 RedfishFunc.logout(client, login_id, login_header)
@@ -1027,77 +1040,112 @@
 
             if args.attribute is None and args.value is None and args.fileurl is not None:
                 for key, value in biosJson.items():
                     if str(value).lower() == "enable":
                         value = "Enabled"
                     if str(value).lower() == "disable":
                         value = "Disabled"
-                    if judgeAttInList(key.replace(" ", ""), descriptionList) is False:
+                    if self.judgeAttInListM5(key.replace(" ", ""), descriptionList) is False:
                         Bios_result.State('Failure')
                         Bios_result.Message(["Please check your attribute spell of '{0}' by -L parameter!".format(key)])
                         # logout
                         RedfishFunc.logout(client, login_id, login_header)
                         return Bios_result
                     # 执行单个设置 先读取文件，判断-a -v是否在列表中
-                    if judgeAttInList(des_key[key.replace(" ", "")], result.get('data').keys()) is False:
+                    if self.judgeAttInListM5(des_key[key.replace(" ", "")], result.get('data').keys()) is False:
                         Bios_result.State('Failure')
                         Bios_result.Message(["'{0}' is not in set options.".format(key)])
                         # logout
                         RedfishFunc.logout(client, login_id, login_header)
                         return Bios_result
                     if key in boot_option:
                         for item in des_value[key.replace(" ", "")]:
                             if str(item).startswith(value):
                                 value = item
                                 break
-                    if value not in des_value[key.replace(" ", "")]:
-                        Bios_result.State('Failure')
-                        Bios_result.Message(["{0} does not support setting to {1}!".format(key, value)])
-                        # logout
-                        RedfishFunc.logout(client, login_id, login_header)
-                        return Bios_result
-                    # if str(value).isdigit():
-                    #     data['Attributes'][des_key[key.replace(" ", "")]] = int(value)
-                    # else:
-                    #     data['Attributes'][des_key[key.replace(" ", "")]] = value
-                    data['Attributes'][des_key[key.replace(" ", "")]] = value
+
+                    values = des_value.get(key.replace(" ", ""), [])
+                    if len(values) == 1:
+                        valuestr = values[0]
+                        if "~" in valuestr:
+                            min = valuestr.split("~")[0]
+                            max = valuestr.split("~")[1]
+                        elif "-" in valuestr:
+                            min = valuestr.split("-")[0]
+                            max = valuestr.split("-")[1]
+                        if int(value) < int(min) or int(value) > int(max):
+                            Bios_result.State('Failure')
+                            Bios_result.Message(["The scope of {0} is {1}!".format(key, valuestr)])
+                            # logout
+                            RedfishFunc.logout(client, login_id, login_header)
+                            return Bios_result
+
+                    else:
+                        if str(value) not in des_value[key.replace(" ", "")]:
+                            Bios_result.State('Failure')
+                            Bios_result.Message(["{0} does not support setting to {1}!".format(key, value)])
+                            # logout
+                            RedfishFunc.logout(client, login_id, login_header)
+                            return Bios_result
+                        data['Attributes'][des_key[key.replace(" ", "")]] = str(value)
             elif args.attribute is not None and args.value is not None and args.fileurl is None:
                 if str(args.value).lower() == "enable":
                     args.value = "Enabled"
                 if str(args.value).lower() == "disable":
                     args.value = "Disabled"
-                if judgeAttInList(args.attribute.replace(" ", ""), descriptionList) is False:
+                if self.judgeAttInListM5(args.attribute.replace(" ", ""), descriptionList) is False:
                     Bios_result.State('Failure')
                     Bios_result.Message(
                         ["Please check your attribute spell of '{0}' by -L parameter!".format(args.attribute)])
                     # logout
                     RedfishFunc.logout(client, login_id, login_header)
                     return Bios_result
-                if judgeAttInList(des_key[args.attribute.replace(" ", "")], result.get('data').keys()) is False:
+                if self.judgeAttInListM5(des_key[args.attribute.replace(" ", "")], result.get('data').keys()) is False:
                     Bios_result.State('Failure')
                     Bios_result.Message(["'{0}' is not in set options.".format(args.attribute)])
                     # logout
                     RedfishFunc.logout(client, login_id, login_header)
                     return Bios_result
                 if args.attribute in boot_option:
                     for item in des_value[args.attribute.replace(" ", "")]:
                         if str(item).startswith(args.value):
                             args.value = item
                             break
-                if args.value not in des_value[args.attribute.replace(" ", "")]:
-                    Bios_result.State('Failure')
-                    Bios_result.Message(["{0} does not support setting to {1}!".format(args.attribute, args.value)])
-                    # logout
-                    RedfishFunc.logout(client, login_id, login_header)
-                    return Bios_result
-                data['Attributes'][des_key[args.attribute.replace(" ", "")]] = args.value
+
+                values = des_value.get(args.attribute.replace(" ", ""), [])
+                if len(values) == 1:
+                    valuestr = values[0]
+                    if "~" in valuestr:
+                        min = valuestr.split("~")[0]
+                        max = valuestr.split("~")[1]
+                    elif "-" in valuestr:
+                        min = valuestr.split("-")[0]
+                        max = valuestr.split("-")[1]
+                    if int(args.value) < int(min) or int(args.value) > int(max):
+                        Bios_result.State('Failure')
+                        Bios_result.Message(["The scope of {0} is {1}!".format(args.attribute, valuestr)])
+                        # logout
+                        RedfishFunc.logout(client, login_id, login_header)
+                        return Bios_result
+
+                    data['Attributes'][des_key[args.attribute.replace(" ", "")]] = int(args.value)
+                else:
+                    if str(args.value) not in values:
+                        Bios_result.State('Failure')
+                        Bios_result.Message(["{0} does not support setting to {1}!".format(args.attribute, args.value)])
+                        # logout
+                        RedfishFunc.logout(client, login_id, login_header)
+                        return Bios_result
+                    data['Attributes'][des_key[args.attribute.replace(" ", "")]] = str(args.value)
+
             # 获取future
             future_result = RedfishFunc.getBiosFuture(client, login_header)
             # 检查前置项
-            conditionflag, conditionmessage = self.judgeCondition(data['Attributes'], future_result.get('data'), result.get('data'), infoList)
+            conditionflag, conditionmessage = self.judgeCondition(data['Attributes'], future_result.get('data'),
+                                                                  result.get('data'), infoList)
             if not conditionflag:
                 Bios_result.State('Failure')
                 Bios_result.Message([conditionmessage])
                 # logout
                 RedfishFunc.logout(client, login_id, login_header)
                 return Bios_result
 
@@ -5925,15 +5973,15 @@
                 session_result.UserPrivilege(item.get('user_privilege', None))
                 seList.append(session_result.dict)
             result.State('Success')
             result.Message(seList)
         else:
             result.State("Failure")
             result.Message(
-                ["get power status error, error code " + str(info.get('code'))])
+                ["get sessions info error, error code " + str(info.get('code'))])
 
         RestFunc.logout(client)
         return result
 
     def delsession(self, client, args):
         result = ResultBean()
         headers = RestFunc.login_M6(client)
@@ -6064,20 +6112,26 @@
                 if cpu.get('proc_status') == 1:
                     # 在位
                     name = 'CPU' + str(cpu.get('proc_id', 0))
                     cpu_singe.CommonName(name)
                     cpu_singe.Location('mainboard')
                     if 'proc_name' in cpu:
                         cpu_singe.Model(cpu.get('proc_name'))
+                    else:
+                        cpu_singe.Model(cpu.get(None))
+                    if "Manufacturer" in cpu:
+                        cpu_singe.Manufacturer(cpu.get('Manufacturer', None))
+                    elif 'proc_name' in cpu:
                         if 'Intel' in cpu.get('proc_name'):
-                            cpu_singe.Manufacturer('Intel')
+                            cpu_singe.Manufacturer('Intel(R) Corporation')
+                        elif 'AMD' in cpu.get('proc_name'):
+                            cpu_singe.Manufacturer('AMD')
                         else:
                             cpu_singe.Manufacturer(None)
                     else:
-                        cpu_singe.Model(cpu.get(None))
                         cpu_singe.Manufacturer(None)
 
                     cpu_singe.L1CacheKiB(cpu.get('proc_l1cache_size', None))
                     cpu_singe.L2CacheKiB(cpu.get('proc_l2cache_size', None))
                     cpu_singe.L3CacheKiB(cpu.get('proc_l3cache_size', None))
                     # 通过sensor获取cpu_DTS_Temp
                     sensor = IpmiFunc.getSensorByNameByIpmi(
@@ -6221,17 +6275,15 @@
                                 'mem_mod_socket_num', 0))
                     else:
                         name = memory.get('mem_mod_slot', None)
                     memory_singe.CommonName(name)
                     memory_singe.Location('mainboard')
                     memory_singe.Manufacturer(
                         memory.get('mem_mod_vendor', None))
-                    memory_singe.CapacityMiB(
-                        memory.get('mem_mod_size') *
-                        1024 if 'mem_mod_size' in memory else None)
+                    memory_singe.CapacityGiB(memory.get('mem_mod_size') if 'mem_mod_size' in memory else None)
                     memory_singe.OperatingSpeedMhz(
                         memory.get('mem_mod_frequency', None))
                     memory_singe.CurrentSpeedMhz(memory.get('mem_mod_current_frequency', None))
                     memory_singe.AssetTag(memory.get('mem_mod_asset_tag', None))
                     memory_singe.SerialNumber(
                         memory.get('mem_mod_serial_num', None))
                     memory_singe.MemoryDeviceType(
@@ -6431,15 +6483,15 @@
         hard_info = RestFunc.getHardDiskInfoByRest(client)
         if hard_info == {}:
             result.State('Failure')
             result.Message(['get hard disk info failed'])
         elif hard_info.get('code') == 0 and hard_info.get('data') is not None:
             hard_data = hard_info.get('data')
             hard_dict = {0: 'No', 1: 'Yes'}
-            FrontRear_dict = {1: 'Front', 0: 'Rear'}
+            FrontRear_dict = {1: 'Front', 0: 'Rear', 2: 'Onboard', 3: 'Inner'}
             hardList = []
             idx = 0
             while idx < len(hard_data):
                 hard_result = HardBackBean()
                 hsrd_info = hard_data[idx]
                 hard_result.Id(hsrd_info.get('h_id', None))
                 hard_result.Present(hard_dict.get(hsrd_info.get('present', 0)))
@@ -6549,16 +6601,22 @@
                     hdd_dict['Model'] = str(item['model']).strip()
                 if "SN" in item:
                     hdd_dict['SN'] = str(item['SN']).strip()
                 if "firmware" in item:
                     hdd_dict['Firmware'] = str(item['firmware']).strip()
                 if "location" in item:
                     hdd_dict['Location'] = str(item['location']).strip()
+                    # 比M6多位置字段
+                if "locationstring" in item:
+                    hdd_dict['Location'] = str(item['locationstring']).strip()
                 if "manufacture" in item:
                     hdd_dict['Manufacture'] = str(item['manufacture']).strip()
+                if "capablespeed" in item:
+                    # 比M6多最大速率字段
+                    hdd_dict['CapableSpeed'] = str(item['capablespeed']).strip()
                 hdd_list.append(hdd_dict)
             result.State("Success")
             result.Message(hdd_list)
         else:
             result.State("Failure")
             result.Message(["get hard disk info error, error info: " + str(hdd_info.get('data'))])
         RestFunc.logout(client)
@@ -6583,15 +6641,18 @@
             back_data = back_info.get('data')
             back_dict = {0: 'No', 1: 'Yes'}
             backList = []
             idx = 0
             while idx < len(back_data):
                 back_result = BackplaneBean()
                 back_info = back_data[idx]
-                back_result.Id(back_info.get('backplane_index', None))
+                if "backplane_index" in back_info:
+                    back_result.Id(back_info.get('backplane_index', None))
+                else:
+                    back_result.Id(back_info.get('id', None))
                 back_result.Present(back_dict.get(back_info.get('present', 0)))
                 back_result.CPLDVersion(back_info.get('cpld_version', None))
                 back_result.PortCount(back_info.get('port_count', 0))
                 back_result.DriverCount(back_info.get('driver_count', 0))
                 back_result.Temperature(back_info.get('temperature', None))
                 back_result.Location(back_info.get('front', None))
                 idx += 1
@@ -6603,14 +6664,19 @@
             result.Message(
                 ["get disk back plane info error, error code " + str(back_info.get('code'))])
 
         RestFunc.logout(client)
         return result
 
     def getpcie(self, client, args):
+        def gethex(id):
+            if id:
+                return hex(id)
+            else:
+                return None
         headers = RestFunc.login_M6(client)
         if headers == {}:
             login_res = ResultBean()
             login_res.State("Failure")
             login_res.Message(
                 ["login error, please check username/password/host/port"])
             return login_res
@@ -6628,27 +6694,34 @@
             List = []
             for i in range(size):
                 if data[i] == {}:
                     continue
                 pcie = Pcie()
                 pcie.Id(data[i].get('id', i))
                 pcie.CommonName(data[i].get('DeviceLocator'))
-                pcie.Location('mainboard')
+                pcie.Location(data[i].get('DeviceLocator'))
                 if data[i].get('present', None) == 1:
                     pcie.Type(ListPCIEDevType[data[i].get('dev_type')] if data[i].get(
                         'dev_type') is not None else None)
                     pcie.SlotBus(hex(data[i].get('bus_num'))
                                  if 'bus_num' in data[i] else None)
                     pcie.SlotDevice(
                         hex(data[i].get('dev_num')) if 'dev_num' in data[i] else None)
                     pcie.SlotFunction(
                         hex(data[i].get('func_num')) if 'func_num' in data[i] else None)
                     pcie.State('Enabled')
                     pcie.DeviceID(data[i].get('device_name', None))
                     pcie.VendorID(data[i].get('vendor_name', None))
+                    pcie.State('Present')
+                    pcie.DeviceName(data[i].get('device_name', None))
+                    pcie.DeviceID(gethex(data[i].get('device_id', None)))
+                    pcie.SubDeviceID(gethex(data[i].get('sub_device_id', None)))
+                    pcie.VendorName(data[i].get('vendor_name', None))
+                    pcie.VendorID(gethex(data[i].get('vendor_id', None)))
+                    pcie.SubVendorID(gethex(data[i].get('sub_vendor_id', None)))
                     pcie.RatedLinkSpeed("GEN" +
                                         str(data[i].get('max_link_speed', 0)))
                     pcie.RatedLinkWidth("X" +
                                         str(data[i].get('max_link_width', 0)))
                     pcie.CurrentLinkSpeed(
                         "GEN" + str(data[i].get('current_link_speed', 0)))
                     pcie.CurrentLinkWidth(
@@ -6709,19 +6782,19 @@
                 "Unknown": "NA",
                 255: "NA"}
             nicRes.State("Success")
             PCIElist = []
             data = res.get('data')['sys_adapters']
             for ada in data:
                 PCIEinfo = NICBean()
-                PCIEinfo.CommonName(ada['location'])
+                PCIEinfo.CommonName(ada.get('location', 'NA'))
                 PCIEinfo.Location("mainboard")
                 adapterinfo = NICController()
                 adapterinfo.Id(ada['id'])
-                adapterinfo.Location(ada['location'])
+                adapterinfo.Location(ada.get('location', 'NA'))
                 if ada['vendor'] == "":
                     adapterinfo.Manufacturer(None)
                     PCIEinfo.Manufacturer(None)
                 else:
                     if "0x" in ada['vendor']:
                         maf = PCI_IDS_LIST.get(
                             int(ada['vendor'], 16), ada['vendor'])
@@ -9776,15 +9849,14 @@
                         return smtpinfo
                     if not RegularCheckUtil.checkSMTPPassword(PassWord):
                         smtpinfo.State("Failure")
                         smtpinfo.Message(
                             ["SMTP server password(-PW) cannot contain ' '(space)."])
                         RestFunc.logout(client)
                         return smtpinfo
-                    # PassWord = RestFunc.Encrypt1('add', PassWord)
                 else:
                     if SMTPAUTH == 1:
                         smtpinfo.State("Failure")
                         smtpinfo.Message(
                             ["SMTP server password(-PW) is needed,when serverAuthentication(-Auth) is enable."])
                         RestFunc.logout(client)
                         return smtpinfo
@@ -11403,15 +11475,15 @@
                         return res
                 set_res = IpmiFunc.setPsuConfigByIpmi(client, set_cmd)
                 if set_res.get('code') == 0:
                     res.State("Success")
                     res.Message(["set psu config success."])
                 else:
                     res.State("Failure")
-                    res.Message(["set psu config failed."])
+                    res.Message([str(set_res.get('data'))])
             else:
                 res.State("Failure")
                 res.Message(["get psu count failed."])
         except Exception as e:
             res.State("Failure")
             res.Message([str(e)])
         return res
@@ -11673,15 +11745,15 @@
 
         res = ResultBean()
         try:
             login_header, login_id = RedfishFunc.login(client)
             if login_header == {} or "login error" in login_id or login_id == '':
                 res.State("Failure")
                 res.Message(['login session service failed.'])
-                return
+                return res
 
             local_time = ftime()
             file_name_init = str(args.host) + "_bios_" + str(local_time) + ".conf"
             if args.fileurl == ".":
                 file_name = file_name_init
                 file_path = os.path.abspath(".")
             elif args.fileurl == "..":
@@ -11958,15 +12030,15 @@
             if pd['ControllerName'] not in ctrl_list_dict:
                 ctrl_list_dict[pd['ControllerName']] = []
             ctrl_list_dict[pd['ControllerName']].append(pd.get('DeviceID', pd.get('slotNum')))
     else:
         result.State("Failure")
         result.Message(['get physical disk information failed!' + res.get('data')])
         return result
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         for pd in ctrl_list_dict:
             ctrl_list_dict.get(pd).sort()
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
@@ -12334,15 +12406,15 @@
         result.State("Failure")
         result.Message([res.get('data')])
         return result
 
     for pd in ctrl_ld_list_dict:
         ctrl_ld_list_dict.get(pd).sort()
 
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             raidDict['Virtual Drive ID'] = ctrl_ld_list_dict.get(ctrl_id_name_dict.get(ctrlid))
@@ -12497,15 +12569,15 @@
     else:
         result.State("Failure")
         result.Message([res.get('data')])
 
     for pd in ctrl_list_dict:
         ctrl_list_dict.get(pd).sort()
 
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             pdiskList = []
@@ -13328,15 +13400,15 @@
                     args.access = 1
                 user_old["access"] = args.access
                 user_old["group_name"] = args.group
             user_old["UserOperation"] = 1
             user_old["changepassword"] = 0
             user_old["confirm_password"] = ""
             user_old["password"] = ""
-            user_old["session_confirm"] = ""
+            user_old["session_confirm"] = client.passcode
 
             user_old["password_size"] = "bytes_16"
             user_old["email_format"] = "ami_format"
             if args.email is not None:
                 user_old["email_id"] = args.email
             else:
                 user_old["email_id"] = ''
@@ -13632,15 +13704,15 @@
                 args.uname = user_old['name']
             else:
                 user_old['name'] = args.uname
             user_old["UserOperation"] = 1
             user_old["changepassword"] = 0
             user_old["confirm_password"] = ""
             user_old["password"] = ""
-            user_old["session_confirm"] = ""
+            user_old["session_confirm"] = client.passcode
             user_old["password_size"] = "bytes_16"
             user_old["email_format"] = "ami_format"
             if args.email is not None:
                 user_old["email_id"] = args.email
             if args.access is not None:
                 if args.access == 'enable':
                     user_old["access"] = 1
@@ -13992,15 +14064,15 @@
     args = tex()
     # args.service('kvm')
     # args.enabled(None)
     # args.port(None)
     # args.port2(7578)
     # args.sslenable(None)
     args.image(
-        'protocol://[root:inspur@2018@]100.2.28.203[:22]/data/nfs/server/CentOS-7-x86_64-Everything-1511')
+        'protocol://[root:test@2018@]100.2.28.203[:22]/data/nfs/server/CentOS-7-x86_64-Everything-1511')
     args.operatortype('Mount')
     # args.image(None)
     # res= com5.getproduct(client,args)
     # res= com5.getraid(client,args)
     # res= com5.getpdisk(client,args)
     # res= com5.getpcie(client,args)
     # res= com5.getpsu(client,args)
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6_41401.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM6_41401.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     else:
         result.State("Failure")
         result.Message([res.get('data')])
 
     for pd in ctrl_list_dict:
         ctrl_list_dict.get(pd).sort()
 
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             pdiskList = []
@@ -258,15 +258,15 @@
         result.State("Failure")
         result.Message([res.get('data')])
         return result
 
     for pd in ctrl_ld_list_dict:
         ctrl_ld_list_dict.get(pd).sort()
 
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
             raidDict['Controller Name'] = ctrl_id_name_dict.get(ctrlid)
             raidDict['Virtual Drive ID'] = ctrl_ld_list_dict.get(ctrl_id_name_dict.get(ctrlid))
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM6_4140a.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM6_4140a.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/CommonM7.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/CommonM7.py`

 * *Files 2% similar despite different names*

```diff
@@ -458,25 +458,26 @@
         # get
         # res=RestFunc.getAdapterByRest(client)
         res = RestFunc.getAdapterByRest(client)
         if res == {}:
             nicRes.State("Failure")
             nicRes.Message(["cannot get information"])
         elif res.get('code') == 0 and res.get('data') is not None:
-            port_status_dict = {0: "Not Linked", 1: "Linked", 2: "NA", "Unknown": "NA", 255: "NA"}
+            # port_status_dict = {0: "Not Linked", 1: "Linked", 2: "NA", "Unknown": "NA", 255: "NA"}
             nicRes.State("Success")
             PCIElist = []
             data = res.get('data')['sys_adapters']
             for ada in data:
                 PCIEinfo = NICBean()
                 PCIEinfo.CommonName(ada['location'])
                 PCIEinfo.Location("mainboard")
                 adapterinfo = NICController()
                 adapterinfo.Id(ada['id'])
-                adapterinfo.Location(ada['location'])
+                adapterinfo.Location(ada.get('location', 'NA'))
+                adapterinfo.PortType(ada.get('port_type', 'NA'))
                 if ada['vendor'] == "":
                     adapterinfo.Manufacturer(None)
                     PCIEinfo.Manufacturer(None)
                 else:
                     if "0x" in ada['vendor']:
                         maf = PCI_IDS_LIST.get(int(ada['vendor'], 16), ada['vendor'])
                         adapterinfo.Manufacturer(maf)
@@ -502,15 +503,16 @@
                 ports = ada.get('ports', [])
                 adapterinfo.PortCount(len(ports))
                 portlist = []
                 for port in ports:
                     portBean = NicPort()
                     portBean.Id(port['id'])
                     portBean.MACAddress(port['mac_addr'])
-                    portBean.LinkStatus(port_status_dict.get(port['status'], port['status']))
+                    # portBean.LinkStatus(port_status_dict.get(port['status'], port['status']))
+                    portBean.LinkStatus(port.get('LinkStatus', "N/A"))
                     portBean.MediaType(None)
                     portlist.append(portBean.dict)
                 adapterinfo.Port(portlist)
                 controllerList = []
                 controllerList.append(adapterinfo.dict)
                 # PCIEinfo.Serialnumber(ada['serial_num'])
                 if 'serial_num' in ada:
@@ -533,15 +535,15 @@
         else:
             nicRes.State("Failure")
             nicRes.Message(["get information error, error code " + str(res.get('code'))])
 
         RestFunc.logout(client)
         return nicRes
 
-    def getgpu(self, client, args):
+    def getgpu1(self, client, args):
         res = ResultBean()
         state = "Failure"
         gpu_device_class_type = ["DisplayController", "ProcessingAccelerator"]
         id_res = RedfishFunc.getChassisID(client)
         if id_res.get('code') == 0 and id_res.get('data') is not None:
             id_data = id_res.get('data')
             id_url = None
@@ -575,14 +577,36 @@
                 message = "No chassis id."
         else:
             message = "Cannot get chassis id."
         res.State(state)
         res.Message([message])
         return res
 
+    def getgpu(self, client, args):
+        headers = RestFunc.login_M6(client)
+        if headers == {}:
+            login_res = ResultBean()
+            login_res.State("Failure")
+            login_res.Message(["login error, please check username/password/host/port"])
+            return login_res
+        client.setHearder(headers)
+        res = ResultBean()
+
+        gpures = RestFunc.getgpu(client)
+        if gpures.get('code') == 0:
+            res.State('Success')
+            gpurawinfo = gpures.get('data')
+            res.Message([gpurawinfo])
+        else:
+            res.State('Failure')
+            res.Message(['get gpu information failed.' + str(gpures.get('date'))])
+        # logout
+        RestFunc.logout(client)
+        return res
+
     def setpowerbudget(self, client, args):
         import collections
 
         def getSuspend(start, end, week_str):
             if start is not None and end is not None and week_str is not None:
                 if start > 24 or start < 0:
                     value = 'Invalid start, start range from 0-24'
@@ -853,14 +877,17 @@
                     res.Message([""])
             except Exception as e:
                 res.State("Failure")
                 res.Message(["File content must be in json format."])
             return res
 
     def getbios(self, client, args):
+        #获取bios版本 放在args里面
+        self._get_bios_version(client, args)
+
         bios_result = ResultBean()
         login_header, login_id = RedfishFunc.login(client)
         if not login_header or not login_id or 'login error' in login_id:
             bios_result.State('Failure')
             bios_result.Message(['login session service failed, please check username/password/host/port'])
             return bios_result
         args.Attribute = None
@@ -958,17 +985,23 @@
                 index = int(user_key[-1:]) - 1
                 return value_map.get(origin_value[index], origin_value[index])
             else:
                 return [value_map.get(str(value), str(value)) for value in origin_value]
         elif isinstance(origin_value, dict):
             return {k: value_map.get(str(v), str(v)) for k, v in origin_value}
         else:
-            return value_map.get(str(origin_value), None)
+            if len(value_map) == 1:
+                return origin_value
+            else:
+                return value_map.get(str(origin_value), None)
 
     def setbios(self, client, args):
+        #获取bios版本 放在args里面
+        self._get_bios_version(client, args)
+
         res = ResultBean()
         attr_dict = {}
         # 读取映射文件
         mapper_result = self._get_xml_mapper(args, 'value', 'cmd')
         # args.list = False
         if mapper_result[0]:
             if 'list' in args and args.list:  # 打印信息
@@ -1014,15 +1047,15 @@
                 return res
             # 校验值并转换
             item_dict = attr_dict[key.lower().replace(" ","")]
             attr = item_dict['getter']
             attr_setter = item_dict['setter']
             attr_parent = item_dict['parent']
             #list的3种处理方式 {0:"x", 1:"y"} [x,y,...] x
-            if item_dict['type'] == 'list':
+            if item_dict.get('list') > 0:
                 if isinstance(value, dict):
                     for k, v in value.items():  # 根据目前支持的配置项，值统一处理为str
                         user_bios[attr + str(k)] = str(attr_setter[v])
                 elif isinstance(value, list):
                     for i in range(len(value)):
                         user_bios[attr + str(i)] = str(attr_setter[value[i]])
                 elif isinstance(value, str):
@@ -1038,23 +1071,44 @@
                             return res
                     elif "[" in value:
                         valueinlist = value[1:-1].split(",")
                         for i in range(len(valueinlist)):
                             user_bios[attr + str(i)] = str(attr_setter[valueinlist[i]])
 
             else:
-                if item_dict['match'] and value not in attr_setter:
-                    res.Message(['[{}] is invalid value for bios option [{}], and valid values are [{}].'
-                                .format(value, key, ', '.join(list(attr_setter.keys())))])
-                    res.State('Failure')
-                    return res
+                if len(attr_setter) == 1:
+                    #类型
+                    for valuerange in attr_setter.keys():
+                        if "-" in valuerange:
+                            min = int(valuerange.split("-")[0])
+                            max = int(valuerange.split("-")[1])
+                        elif "~" in valuerange:
+                            min = int(valuerange.split("~")[0])
+                            max = int(valuerange.split("~")[1])
+                        else:
+                            res.Message([
+                                            '[{}] is invalid range value for bios option [{}], range should be a~b or a-b.'
+                                        .format(valuerange, key)])
+                            res.State('Failure')
+                            return res
+                        if int(value) < min or int(value) > max:
+                            res.Message(
+                                ['[{}] is invalid value for bios option [{}], and valid values are [{}].'
+                                .format(value, key, valuerange)])
+                            res.State('Failure')
+                            return res
 
-                if item_dict['type'] == 'int':  # 根据目前支持的配置项，处理int、str两种类型
-                    user_bios[attr] = int(attr_setter.get(value, value))
+                        user_bios[attr] = int(value)
                 else:
+                    if item_dict['match'] and value not in attr_setter:
+                        res.Message(['[{}] is invalid value for bios option [{}], and valid values are [{}].'
+                                    .format(value, key, ', '.join(list(attr_setter.keys())))])
+                        res.State('Failure')
+                        return res
+
                     user_bios[attr] = str(attr_setter.get(value, value))
 
         # 调用接口设置
         login_header, login_id = RedfishFunc.login(client)
         if not login_header or not login_id or 'login error' in login_id:
             res.Message(['login session service failed, please check username/password/host/port'])
             res.State('Failure')
@@ -1137,45 +1191,81 @@
             res.State('Failure')
         RedfishFunc.logout(client, login_id, login_header)
         return res
 
     def formatBiosPatchBody(self, user_bios):
         return user_bios
 
-    def _get_xml_file(self):
+    def _get_bios_version(self, client, args):
+        biosversion = None
+        # login
+        headers = RestFunc.login_M6(client)
+        if headers == {}:
+            args.biosversion = biosversion
+            return biosversion
+        client.setHearder(headers)
+        # get
+        res = RestFunc.getFwVersion(client)
+        if res.get('code') == 0 and res.get('data') is not None:
+            data = res.get('data')
+
+            for fwinfo in data:
+                name_raw = fwinfo.get('dev_name')
+                if name_raw != "BIOS":
+                    continue
+                else:
+                    index_version = fwinfo.get('dev_version').find('(')
+                    if index_version == -1:
+                        biosversion = None if fwinfo.get('dev_version') == '' else fwinfo.get('dev_version')
+                    else:
+                        biosversion = None if fwinfo.get('dev_version') == '' else fwinfo.get('dev_version')[:index_version].strip()
+                    break
+        args.biosversion = biosversion
+        RestFunc.logout(client)
+        return biosversion
+
+    def _get_xml_file(self, args):
         xml_path = os.path.join(IpmiFunc.command_path, "bios") + os.path.sep
+        if args.biosversion:
+            #M7 5.10.00 开始 bios里面替换为 XCradle
+            b1=args.biosversion.split(".")[0]
+            b2=args.biosversion.split(".")[1]
+            b3=args.biosversion.split(".")[2]
+            biosformat = float(b1 + "." + b2 + b3)
+            if biosformat >= 5.1000:
+                return xml_path + 'M7_5.10.00.xml'
         return xml_path + 'M7.xml'
 
     def _get_xml_mapper(self, args, key, value):
         """
             {
                 'descriptionName': {
                     'description': 'descriptionName',
-                    'type': 'int/str/list/dict',
+                    'list': 64,
                     'match': True/False,
                     'parent': 'server_bios_parent_key',
                     'getter': 'server_bios_key',
                     'setter': {
                         'cmd': 'value' 或 'value': 'cmd' 根据参数确定
                     }
                 }
             }
         """
         try:
             #xml_filepath = sys.path[0] + '/mappers/bios/M7.xml'
-            xml_filepath = self._get_xml_file()
+            xml_filepath = self._get_xml_file(args)
             import xml.etree.ElementTree as ET
             tree = ET.parse(xml_filepath)
             server = tree.getroot()
             map_dict = {}
             for items in server:
                 for item in items:
                     map_dict[item.find('name').find('description').text.lower().replace(" ", "")] = {
                         'description': item.find('name').find('description').text,
-                        'type': 'str' if item.find('type') is None else item.find('type').text,
+                        'list': 0 if item.find('list') is None else int(item.find('list').text),
                         'match': True if item.find('match') is None else False if item.find(
                             'match').text == 'False' else True,
                         'parent': None if item.find('parent') is None else item.find('parent').text,
                         'getter': item.find('getter').text,
                         'setter': {
                             setter.find(key).text: setter.find(value).text for setter in item.find('setters')
                         },
@@ -1203,15 +1293,15 @@
                         'getter': 'cmd'
                     }
                 }
             }
         """
         try:
             #xml_filepath = sys.path[0] + '/mappers/bios/M7.xml'
-            xml_filepath = self._get_xml_file()
+            xml_filepath = self._get_xml_file(args)
             import xml.etree.ElementTree as ET
             tree = ET.parse(xml_filepath)
             server = tree.getroot()
             map_dict = {}
             for items in server:
                 for item in items:
                     map_dict[item.find('getter').text] = {
@@ -1257,17 +1347,30 @@
         condition_dict = {}
         # getter: description
         bios_dict = {}
         # getter: {cmd: value}
         bios_value_dict = {}
         errordict={}
         for bioskey, biosvalue in bios_set.items():
-            conditions = bios_all_info.get(bioskey).get("conditions")
+            conditions = bios_all_info.get(bioskey, {}).get("conditions", {})
             errorlist = []
             errorinfo = ""
+            #如果和当前值相等 不需要考虑condition
+            bioskeyparent = bios_all_info.get(bioskey, {}).get("parent")
+            if bioskeyparent:
+                if bioskeyparent == "FixedBootPriorities":
+                    #如果是启动项，可能获取方式有区别
+                    bioskeylistname = bioskey[0:-1]
+                    bioskeylistid = bioskey[-1]
+                    if bios_set.get(bioskey) == bios_cur.get(bioskeyparent, {}).get(bioskeylistname, [])[int(bioskeylistid)]:
+                        continue
+                else:
+                    if bios_cur.get(bioskeyparent, {}).get(bioskey) == bios_set.get(bioskey):
+                        continue
+
             for conditionkey,conditionvalue in conditions.items():
                 condition_bios_info = bios_all_info.get(conditionkey)
                 #condition 的 isrest 展示 key
                 conditionkeyshow = condition_bios_info.get("description")
                 #{bmc value: isrest value}
                 conditionvaluedict = condition_bios_info.get("setter")
                 conditionvalueshow = conditionvaluedict.get(conditionvalue, conditionvalue)
@@ -1294,14 +1397,15 @@
                     if conditonvalue_future:
                         if conditionvalue == conditonvalue_future:
                             continue
                         else:
                             errorlist.append(self.formatCondition(conditionkeyshow, conditionvalueshow, conditionvaluedict.get(conditonvalue_future), 2))
                             continue
                 #比较当前值
+                conditonvalue_current = None
                 if bios_cur.get(conditionkey):
                     conditonvalue_current = bios_cur.get(conditionkey)
                 elif bios_cur.get(conditionparent):
                     conditonvalue_current = bios_cur.get(conditionparent).get(conditionkey)
                 if conditonvalue_current:
                     if conditionvalue == conditonvalue_current:
                         continue
@@ -2484,17 +2588,19 @@
                         'Automatic' if mode.get('data').get('control_mode') == 'auto' else 'Manual')
                 else:
                     fan_Info.FanSpeedAdjustmentMode(None)
             # 通过sensor获取Fan_Power
             sensor = IpmiFunc.getSensorByNameByIpmi(client, 'Fan_Power')
             if sensor and sensor.get('code') == 0:
                 temp = sensor.get('data')[0].get('value')
-                fan_Info.FanTotalPowerWatts(float(temp) if (temp is not None and temp != 'na') else None)
-            else:
-                fan_Info.FanTotalPowerWatts(None)
+                if temp is not None and temp != 'na':
+                    fan_Info.FanTotalPowerWatts(float(temp))
+            #     fan_Info.FanTotalPowerWatts(float(temp) if (temp is not None and temp != 'na') else None)
+            # else:
+            #     fan_Info.FanTotalPowerWatts(None)
             fan_Info.FanManualModeTimeoutSeconds(None)
             fan_Info.Fan(list)
             result.State('Success')
             result.Message([fan_Info.dict])
         elif res.get('code') != 0 and res.get('data') is not None:
             result.State("Failure")
             result.Message(["get fan information error, " + res.get('data')])
@@ -4654,551 +4760,14 @@
         else:
             result.State("Failure")
             result.Message([set_res.get('data')])
 
         RestFunc.logout(client)
         return result
 
-    #2023年1月29日 大概是PFR专用 暂时删除
-    '''
-    def getldapgroup(self, client, args):
-        result = ResultBean()
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        res = RestFunc.getLDAPgroupM6(client)
-        if res.get('code') == 0 and res.get('data') is not None:
-            ldap_group = res.get('data')
-            ldap_group_list = []
-            for group in ldap_group:
-                ldap_res = collections.OrderedDict()
-                ldap_res['Id'] = group['id']
-                ldap_res['Name'] = group['role_group_name']
-                ldap_res['Domain'] = group['role_group_domain']
-                ldap_res['Privilege'] = group['role_group_withoem_privilege']
-                ldap_res['KVM Access'] = "Enabled" if group['role_group_kvm_privilege'] == 1 else "Disabled"
-                ldap_res['VMedia Access'] = "Enabled" if group['role_group_vmedia_privilege'] == 1 else "Disabled"
-                ldap_group_list.append(ldap_res)
-            result.State("Success")
-            result.Message([{"LDAPgroup": ldap_group_list}])
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def addldapgroup(self, client, args):
-        def checkGroupName(name):
-            # 角色组名称是一个64字母数字组成的字串。
-            # 允许特殊字符如连字符和下划线。
-            dn = '^[\da-zA-Z\-_]{1,64}$'
-            if re.search(dn, name, re.I):
-                return True
-            return False
-
-        def checkDoamin(s):
-            # 域名名称是一个64字母数字组成的字串。
-            # 开头字符必须是字母。
-            # 允许特殊字符如点(.)，逗号(,)，连字符(-)，下划线(_)，等于号(=)。
-            # 范例: cn=manager,ou=login, dc=domain,dc=com
-            dn = '^[a-zA-Z][a-zA-Z\-_\.\,\=]{4,64}$'
-            if re.search(dn, s, re.I):
-                return True
-            return False
-
-        result = ResultBean()
-
-        if args.name is not None:
-            if not checkGroupName(args.name):
-                result.State("Failure")
-                result.Message([
-                    'Group name is a string of less than 64 alpha-numeric characters, and hyphen and underscore are also allowed.'])
-                return result
-
-        if args.domain is not None:
-            if not checkDoamin(args.domain):
-                result.State("Failure")
-                result.Message([
-                    'Domain Name is a string of 4 to 64 alpha-numeric characters.It must start with an alphabetical character.Special Symbols like dot(.), comma(,), hyphen(-), underscore(_), equal-to(=) are allowed.Example: cn=manager,ou=login,dc=domain,dc=com'])
-                return result
-
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        name_exist_flag = False
-        add_flag = False
-        res = RestFunc.getLDAPgroupM6(client)
-        if res.get('code') == 0 and res.get('data') is not None:
-            for item in res.get('data'):
-                name = item.get('role_group_name', "unknown")
-                if name == args.name:
-                    name_exist_flag = True
-                    break
-                if name == "":
-                    add_flag = True
-                    args.id = item.get('id', 0)
-                    break
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if name_exist_flag:
-            result.State("Failure")
-            result.Message(['Group ' + args.name + ' is already exist.'])
-            RestFunc.logout(client)
-            return result
-
-        if not add_flag:
-            result.State("Failure")
-            result.Message(['LDAP role group is full.'])
-            RestFunc.logout(client)
-            return result
-
-        kvm_vm = {"enable": 1, "disable": 0}
-        # priv administrator user operator oem none
-        ldapgroup = {
-            'id': args.id,
-            'role_group_domain': args.domain,
-            'role_group_kvm_privilege': kvm_vm.get(args.kvm.lower()),
-            'role_group_name': args.name,
-            'role_group_withoem_privilege': args.pri,
-            'role_group_vmedia_privilege': kvm_vm.get(args.vm.lower()),
-            'role_group_privilege': "none"
-        }
-        # print(ldapgroup)
-        set_res = RestFunc.setLDAPgroupM6(client, ldapgroup)
-        if set_res.get('code') == 0 and set_res.get('data') is not None:
-            result.State("Success")
-            result.Message(["Add LDAP group success."])
-        else:
-            result.State("Failure")
-            result.Message([set_res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def setldapgroup(self, client, args):
-
-        def checkGroupName(name):
-            # 角色组名称是一个64字母数字组成的字串。
-            # 允许特殊字符如连字符和下划线。
-            dn = '^[\da-zA-Z\-_]{1,64}$'
-            if re.search(dn, name, re.I):
-                return True
-            return False
-
-        def checkDoamin(s):
-            # 域名名称是一个64字母数字组成的字串。
-            # 开头字符必须是字母。
-            # 允许特殊字符如点(.)，逗号(,)，连字符(-)，下划线(_)，等于号(=)。
-            # 范例: cn=manager,ou=login, dc=domain,dc=com
-            dn = '^[a-zA-Z][a-zA-Z\-_\.\,\=]{4,64}$'
-            if re.search(dn, s, re.I):
-                return True
-            return False
-
-        result = ResultBean()
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        name_exist_flag = False
-        res = RestFunc.getLDAPgroupM6(client)
-        ldapgroup = None
-        if res.get('code') == 0 and res.get('data') is not None:
-            for item in res.get('data'):
-                id = str(item.get('id', 0))
-                if id == args.id:
-                    ldapgroup = item
-                else:
-                    name = item.get('role_group_name', "unknown")
-                    if name == args.name:
-                        name_exist_flag = True
-                        break
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if name_exist_flag:
-            result.State("Failure")
-            result.Message(['Group ' + args.name + ' is already exist.'])
-            RestFunc.logout(client)
-            return result
-
-        if ldapgroup is None:
-            result.State("Failure")
-            result.Message(['Group id is not exist.' + res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if args.name is not None:
-            if checkGroupName(args.name):
-                ldapgroup['role_group_name'] = args.name
-            else:
-                result.State("Failure")
-                result.Message([
-                    'Group name is a string of less than 64 alpha-numeric characters, and hyphen and underscore are also allowed.'])
-                RestFunc.logout(client)
-                return result
-        if ldapgroup['role_group_name'] == "":
-            result.State("Failure")
-            result.Message(['Group name is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        if args.domain is not None:
-            if checkDoamin(args.domain):
-                ldapgroup['role_group_domain'] = args.domain
-            else:
-                result.State("Failure")
-                result.Message([
-                    'Domain Name is a string of 4 to 64 alpha-numeric characters.It must start with an alphabetical character.Special Symbols like dot(.), comma(,), hyphen(-), underscore(_), equal-to(=) are allowed.Example: cn=manager,ou=login,dc=domain,dc=com'])
-                RestFunc.logout(client)
-                return result
-        if ldapgroup['role_group_domain'] == "":
-            result.State("Failure")
-            result.Message(['Group domain is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        if args.pri is not None:
-            ldapgroup['role_group_withoem_privilege'] = args.pri
-        if ldapgroup['role_group_withoem_privilege'] == "":
-            result.State("Failure")
-            result.Message(['Group privilege is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        kvm_vm = {"enable": 1, "disable": 0}
-        if args.kvm is not None:
-            ldapgroup['role_group_kvm_privilege'] = kvm_vm.get(args.kvm.lower())
-
-        if args.vm is not None:
-            ldapgroup['role_group_vmedia_privilege'] = kvm_vm.get(args.vm.lower())
-
-        # print(ldapgroup)
-        set_res = RestFunc.setLDAPgroupM6(client, ldapgroup)
-        if set_res.get('code') == 0 and set_res.get('data') is not None:
-            result.State("Success")
-            result.Message(["Set LDAP group success."])
-        else:
-            result.State("Failure")
-            result.Message([set_res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def getadgroup(self, client, args):
-        result = ResultBean()
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        res = RestFunc.getADgroupM6(client)
-        if res.get('code') == 0 and res.get('data') is not None:
-            ldap_group = res.get('data')
-            ldap_group_list = []
-            for group in ldap_group:
-                ldap_res = collections.OrderedDict()
-                ldap_res['Id'] = group['id']
-                ldap_res['Name'] = group['role_group_name']
-                ldap_res['Domain'] = group['role_group_domain']
-                ldap_res['Privilege'] = group['role_group_withoem_privilege']
-                ldap_res['KVM Access'] = "Enabled" if group['role_group_kvm_privilege'] == 1 else "Disabled"
-                ldap_res['VMedia Access'] = "Enabled" if group['role_group_vmedia_privilege'] == 1 else "Disabled"
-                ldap_group_list.append(ldap_res)
-            result.State("Success")
-            result.Message([{"ADgroup": ldap_group_list}])
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def addadgroup(self, client, args):
-        def checkGroupName(name):
-            # 角色组名称是一个64字母数字组成的字串。
-            # 允许特殊字符如连字符和下划线。
-            dn = '^[\da-zA-Z\-_]{1,64}$'
-            if re.search(dn, name, re.I):
-                return True
-            return False
-
-        # def checkDoamin(s):
-        #     # 域名名称是一个64字母数字组成的字串。
-        #     # 开头字符必须是字母。
-        #     # 允许特殊字符如点(.)，逗号(,)，连字符(-)，下划线(_)，等于号(=)。
-        #     # 范例: cn=manager,ou=login, dc=domain,dc=com
-        #     dn = '^[a-zA-Z][a-zA-Z\-_\.\,\=]{4,64}$'
-        #     if re.search(dn, s, re.I):
-        #         return True
-        #     return False
-        def checkDoamin(s):
-            dn = '^([\da-zA-Z]+[\w\-]*\.)*([\da-zA-Z]+[\w\-]*)+\.([\da-zA-Z]+[\w\-]*)+$'
-            dnd = '^([\d]+\.)*[\d]+\.[\d]+$'
-            if re.search(dn, s, re.I) and not re.search(dnd, s, re.I):
-                return True
-            return False
-
-        result = ResultBean()
-        if args.name is not None:
-            if not checkGroupName(args.name):
-                result.State("Failure")
-                result.Message([
-                    'Group name is a string of less than 64 alpha-numeric characters, and hyphen and underscore are also allowed.'])
-                return result
-
-        if args.domain is not None:
-            if not checkDoamin(args.domain):
-                result.State("Failure")
-                result.Message([
-                    'Domain Name is a string of less than 255 alpha-numeric characters. '
-                    'It must start with an alphabetical character. '
-                    'Special Symbols like dot(.), hyphen(-), underscore(_) are allowed.'])
-                return result
-
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-        result = ResultBean()
-
-        id_exist_flag = False
-        name_exist_flag = False
-        # add_flag = False
-        res = RestFunc.getADgroupM6(client)
-        if res.get('code') == 0 and res.get('data') is not None:
-            for item in res.get('data'):
-                name = item.get('role_group_name', "unknown")
-                if name == args.name:
-                    name_exist_flag = True
-                    break
-                id = item.get('id', "unknown")
-                if str(id) == args.id and name != "":
-                    id_exist_flag = True
-                    break
-                # if name == "":
-                #     add_flag = True
-                #     args.id = item.get('id', 0)
-                #     break
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if id_exist_flag:
-            result.State("Failure")
-            result.Message(['the ID has group info already, please use "setADgroup" to edit it.'])
-            RestFunc.logout(client)
-            return result
-
-        if name_exist_flag:
-            result.State("Failure")
-            result.Message(['Group ' + args.name + ' is already exist.'])
-            RestFunc.logout(client)
-            return result
-
-        # if not add_flag:
-        #     result.State("Failure")
-        #     result.Message(['AD role group is full.'])
-        #     RestFunc.logout(client)
-        #     return result
-
-        kvm_vm = {"enable": 1, "disable": 0}
-        # priv administrator user operator none
-        adgroup = {
-            'id': args.id,
-            'role_group_domain': args.domain,
-            'role_group_kvm_privilege': kvm_vm.get(args.kvm.lower()),
-            'role_group_name': args.name,
-            'role_group_withoem_privilege': args.pri,
-            'role_group_vmedia_privilege': kvm_vm.get(args.vm.lower()),
-            'role_group_privilege': "none"
-        }
-        # print(adgroup)
-        set_res = RestFunc.setADgroupM6(client, adgroup)
-        if set_res.get('code') == 0 and set_res.get('data') is not None:
-            result.State("Success")
-            result.Message(["Add AD group success."])
-        else:
-            result.State("Failure")
-            result.Message([set_res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    def setadgroup(self, client, args):
-
-        def checkGroupName(name):
-            # 角色组名称是一个64字母数字组成的字串。
-            # 允许特殊字符如连字符和下划线。
-            dn = '^[\da-zA-Z\-_]{1,64}$'
-            if re.search(dn, name, re.I):
-                return True
-            return False
-
-        # def checkDoamin(s):
-        #     # 域名名称是一个64字母数字组成的字串。
-        #     # 开头字符必须是字母。
-        #     # 允许特殊字符如点(.)，逗号(,)，连字符(-)，下划线(_)，等于号(=)。
-        #     # 范例: cn=manager,ou=login, dc=domain,dc=com
-        #     dn = '^[a-zA-Z][a-zA-Z\-_\.\,\=]{4,64}$'
-        #     if re.search(dn, s, re.I):
-        #         return True
-        #     return False
-        def checkDoamin(s):
-            dn = '^([\da-zA-Z]+[\w\-]*\.)*([\da-zA-Z]+[\w\-]*)+\.([\da-zA-Z]+[\w\-]*)+$'
-            dnd = '^([\d]+\.)*[\d]+\.[\d]+$'
-            if re.search(dn, s, re.I) and not re.search(dnd, s, re.I):
-                return True
-            return False
-
-        result = ResultBean()
-        # login
-        headers = RestFunc.login_M6(client)
-        if headers == {}:
-            login_res = ResultBean()
-            login_res.State("Failure")
-            login_res.Message(["login error, please check username/password/host/port"])
-            return login_res
-        client.setHearder(headers)
-
-        name_exist_flag = False
-        id_not_exit_flag = False
-        res = RestFunc.getADgroupM6(client)
-        adgroup = None
-        if res.get('code') == 0 and res.get('data') is not None:
-            for item in res.get('data'):
-                id = str(item.get('id', 0))
-                if id == args.id:
-                    name = item.get('role_group_name', "unknown")
-                    if name == "":
-                        id_not_exit_flag = True
-                        break
-                    adgroup = item
-                else:
-                    name = item.get('role_group_name', "unknown")
-                    if name == args.name:
-                        name_exist_flag = True
-                        break
-        else:
-            result.State("Failure")
-            result.Message([res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if id_not_exit_flag:
-            result.State("Failure")
-            result.Message(['the ID has no group info yet, please use "addADgroup" to add it'])
-            RestFunc.logout(client)
-            return result
-
-        if name_exist_flag:
-            result.State("Failure")
-            result.Message(['Group ' + args.name + ' is already exist.'])
-            RestFunc.logout(client)
-            return result
-
-        if adgroup is None:
-            result.State("Failure")
-            result.Message(['Group id is not exist.' + res.get('data')])
-            RestFunc.logout(client)
-            return result
-
-        if args.name is not None:
-            if checkGroupName(args.name):
-                adgroup['role_group_name'] = args.name
-            else:
-                result.State("Failure")
-                result.Message([
-                    'Group name is a string of less than 64 alpha-numeric characters, and hyphen and underscore are also allowed.'])
-                RestFunc.logout(client)
-                return result
-        if adgroup['role_group_name'] == "":
-            result.State("Failure")
-            result.Message(['Group name is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        if args.domain is not None:
-            if checkDoamin(args.domain):
-                adgroup['role_group_domain'] = args.domain
-            else:
-                result.State("Failure")
-                result.Message([
-                    'Domain Name is a string of 4 to 64 alpha-numeric characters.It must start with an alphabetical character.Special Symbols like dot(.), comma(,), hyphen(-), underscore(_), equal-to(=) are allowed.Example: cn=manager,ou=login,dc=domain,dc=com'])
-                RestFunc.logout(client)
-                return result
-        if adgroup['role_group_domain'] == "":
-            result.State("Failure")
-            result.Message(['Group domain is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        if args.pri is not None:
-            adgroup['role_group_withoem_privilege'] = args.pri
-        if adgroup['role_group_withoem_privilege'] == "":
-            result.State("Failure")
-            result.Message(['Group privilege is needed.'])
-            RestFunc.logout(client)
-            return result
-
-        kvm_vm = {"enable": 1, "disable": 0}
-        if args.kvm is not None:
-            adgroup['role_group_kvm_privilege'] = kvm_vm.get(args.kvm.lower())
-
-        if args.vm is not None:
-            adgroup['role_group_vmedia_privilege'] = kvm_vm.get(args.vm.lower())
-
-        # print(adgroup)
-        set_res = RestFunc.setADgroupM6(client, adgroup)
-        if set_res.get('code') == 0 and set_res.get('data') is not None:
-            result.State("Success")
-            result.Message(["Set AD group success."])
-        else:
-            result.State("Failure")
-            result.Message([set_res.get('data')])
-
-        RestFunc.logout(client)
-        return result
-
-    '''
     def getmediainstance(self, client, args):
         result = ResultBean()
         # login
         headers = RestFunc.login_M6(client)
         if headers == {}:
             login_res = ResultBean()
             login_res.State("Failure")
@@ -5211,14 +4780,15 @@
             gs = res.get('data')
             media_instance = collections.OrderedDict()
             media_instance["CDNum"] = gs.get("num_cd")
             media_instance["HDNum"] = gs.get("num_hd")
             media_instance["KVMCDNum"] = gs.get("kvm_num_cd")
             media_instance["KVMHDNum"] = gs.get("kvm_num_hd")
             media_instance["SDMedia"] = "Enable" if gs.get("sd_media") == 1 else "Disable"
+            media_instance["SecureChannel"] = "Enable" if gs.get("secure_channel") == 1 else "Disable"
             media_instance["PowerSaveMode"] = "Enable" if gs.get("power_save_mode") == 1 else "Disable"
             result.State("Success")
             result.Message([{"Instance": media_instance}])
         else:
             result.State("Failure")
             result.Message([res.get('data')])
 
@@ -5298,27 +4868,50 @@
         else:
             result.State("Failure")
             result.Message(["Set media instance failed. " + set_res.get('data')])
 
         RestFunc.logout(client)
         return result
 
+    def resetkvm(self, client, args):
+        result = ResultBean()
+        # login
+        headers = RestFunc.login_M6(client)
+        if headers == {}:
+            login_res = ResultBean()
+            login_res.State("Failure")
+            login_res.Message(
+                ["login error, please check username/password/host/port"])
+            return login_res
+        client.setHearder(headers)
+
+        res = RestFunc.resetBMCM7(client, 'kvm')
+        if res.get('code') == 0 and res.get('data') is not None:
+            result.State("Success")
+            result.Message([res.get('data')])
+        else:
+            result.State("Failure")
+            result.Message([res.get('data')])
+
+        RestFunc.logout(client)
+        return result
+
     def resetbmc(self, client, args):
         result = ResultBean()
 
         headers = RestFunc.login_M6(client)
         if headers == {}:
             login_res = ResultBean()
             login_res.State("Failure")
             login_res.Message(["login error, please check username/password/host/port"])
             return login_res
         client.setHearder(headers)
 
         RestFunc.securityCheckByRest(client)
-        res = RestFunc.resetBMCM6(client, args.type)
+        res = RestFunc.resetBMCM7(client, 'bmc')
         if res.get('code') == 0 and res.get('data') is not None:
             result.State("Success")
             result.Message([res.get('data')])
         else:
             result.State("Failure")
             result.Message([res.get('data')])
 
@@ -5470,15 +5063,18 @@
                     psu_Info.OverallHealth('OK')
                 else:
                     psu_Info.OverallHealth(overalhealth.get('data').get('psu').capitalize())
             else:
                 psu_Info.OverallHealth(None)
             psu_allInfo = res.get('data')
             psu_Info.PsuPresentTotalPower(psu_allInfo.get('present_power_reading', None))
-            psu_Info.PsuRatedPower(psu_allInfo.get('rated_power', None))
+            # 2023年3月27日
+            rate_power = psu_allInfo.get('rated_power', 'N/A')
+            if rate_power != "N/A":
+                psu_Info.PsuRatedPower(psu_allInfo.get('rated_power', 'N/A'))
             psu_Info.PsuStatus(status_dict.get(psu_allInfo.get('power_supplies_redundant', 0)))
             temp = psu_allInfo.get('power_supplies', [])
             size = len(temp)
             Num = IpmiFunc.getM6DeviceNumByIpmi(client, '0x00')
             if Num and Num.get('code') == 0:
                 DevConfNum = Num.get('data').get('DevNum')
                 psu_Info.Maximum(DevConfNum)
@@ -5505,19 +5101,23 @@
                     psu.PowerInputWatts(temp[i].get('ps_in_power') if 'ps_in_power' in temp[i] else None)
                     psu.OutputAmperage(
                         temp[i].get('ps_out_current') if 'ps_out_current' in temp[i] else None)
                     psu.PartNumber(None if temp[i].get('part_num', None) == '' else temp[i].get('part_num', None))
                     psu.PowerSupplyType(temp[i].get('input_type', 'Unknown'))
                     psu.LineInputVoltage(temp[i].get('ps_in_volt') if 'ps_in_volt' in temp[i] else None)
                     # psu.PowerCapacityWatts(temp[i].get('ps_out_power_max', None))
-                    # 2023年3月27日 
+                    # 2023年3月27日
                     psu.PowerCapacityWatts(temp[i].get('rated_power', None))
                     psu.FirmwareVersion(None if temp[i].get('fw_ver', None) == '' else temp[i].get('fw_ver', None))
                     psu.SerialNumber(temp[i].get('serial_num', None))
-                    psu.Temperature(temp[i].get('ambient_temperature', None))
+
+                    if "temperature" in temp[i]:
+                        psu.Temperature(temp[i].get('temperature', None))
+                    else:
+                        psu.Temperature(temp[i].get('psu_max_temperature', None))
                     if 'status' in temp[i]:
                         psu.Health(
                             'OK' if temp[i].get('status').upper() == 'OK' else temp[i].get('status').capitalize())
                     else:
                         if 'power_status' in temp[i]:
                             psu.Health('OK' if temp[i].get('power_status') == 0 else 'Critical')
                         else:
@@ -5898,15 +5498,15 @@
             if pd['ControllerName'] not in ctrl_list_dict:
                 ctrl_list_dict[pd['ControllerName']] = []
             ctrl_list_dict[pd['ControllerName']].append(pd['DeviceID'])
     else:
         result.State("Failure")
         result.Message(['get physical disk information failed!' + res.get('data')])
         return result
-    if args.Info is not None:
+    if 'Info' in args and args.Info is not None:
         for pd in ctrl_list_dict:
             ctrl_list_dict.get(pd).sort()
         LSI_flag = False
         raidList = []
         for ctrlid in ctrl_id_name_dict:
             raidDict = collections.OrderedDict()
             raidDict['Controller ID'] = ctrlid
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/I24M6.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/I24M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/IBase.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/IBase.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5180M5.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5180M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5280M5.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5_435.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5280M5_435.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NF5280M5_436.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/NF5280M5_436.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/NS5160M6.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/NS5160M6.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/ResEntity.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/ResEntity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1727,14 +1727,20 @@
 
     def Id(self):
         return self.dict['Id']
 
     def Id(self, value):
         self.dict['Id'] = value
 
+    def PortType(self):
+        return self.dict['PortType']
+
+    def PortType(self, value):
+        self.dict['PortType'] = value
+
     def Manufacturer(self):
         return self.dict['Manufacturer']
 
     def Manufacturer(self, value):
         self.dict['Manufacturer'] = value
 
     def Model(self):
@@ -2113,14 +2119,38 @@
 
     def VendorID(self):
         return self.dict['VendorID']
 
     def VendorID(self, value):
         self.dict['VendorID'] = value
 
+    def DeviceName(self):
+        return self.dict['DeviceName']
+
+    def DeviceName(self, value):
+        self.dict['DeviceName'] = value
+
+    def VendorName(self):
+        return self.dict['VendorName']
+
+    def VendorName(self, value):
+        self.dict['VendorName'] = value
+
+    def SubDeviceID(self):
+        return self.dict['SubDeviceID']
+
+    def SubDeviceID(self, value):
+        self.dict['SubDeviceID'] = value
+
+    def SubVendorID(self):
+        return self.dict['SubVendorID']
+
+    def SubVendorID(self, value):
+        self.dict['SubVendorID'] = value
+
     def RatedLinkSpeed(self):
         return self.dict['RatedLinkSpeed']
 
     def RatedLinkSpeed(self, value):
         self.dict['RatedLinkSpeed'] = value
 
     def RatedLinkWidth(self):
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/interface/SA5212M5Impl.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/interface/SA5212M5Impl.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/util/HostTypeJudge.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/util/HostTypeJudge.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             result = {"State": "Failure", "Message": [
                 "Parameter is missing,please check -H <HOST> -U <USERNAME> -P <PASSWORD>"]}
             return result
         else:
             client = RequestClient.RequestClient()
             client.setself(host, username, passcode, port, "lanplus")
             productName = IpmiFunc.getProductNameByIpmi(client)
-            firmwareVersion = IpmiFunc.getFirmwareVersoinByIpmi(client)
+            firmwareVersion = IpmiFunc.getFirmwareVersoinByMcinfo(client)
             return productName, firmwareVersion
 
     # 从命令行参数利用IPMI fru命令验证远程主机的机型
     # 返回 机型、host、username、password
     # raw 0x3c 0x42 获取型号不通用，仅在Korea定制化使用。5288返回5280
 
     def getHostInfoByRaw(self, args):
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/util/RedfishClient.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/util/RedfishClient.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/util/RegularCheckUtil.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/util/RegularCheckUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/util/RequestClient.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/util/RequestClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,22 @@
         self.host = ''
         self.resthost = ''
         self.username = ''
         self.passcode = ''
         self.port = ''
         self.restport = 443
         self.lantype = ''
+        self.type = ''
 
         self.token = ''
         self.etag = ''
         self.headerhost = None
         self.auth = None
 
-    def setself(self, host, username, password, port=623, lantype="lanplus"):
+    def setself(self, host, username, password, type, port=623, lantype="lanplus"):
         """
         #=====================================================================
         #   @Method:  设置带内hos，port,username,password值
         #   @Param:
         #   @Return:
         #   @author:
         #=====================================================================
@@ -62,14 +63,15 @@
             resthost = '[' + host + ']'
         else:
             resthost = host
         self.host = host
         self.resthost = resthost
         self.username = username
         self.passcode = password
+        self.type = type
         if port is None:
             self.port = 623
         else:
             self.port = port
         if lantype is None:
             self.lantype = 'lanplus'
         else:
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/util/configUtil.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/util/configUtil.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # -*- coding:utf-8 -*-
 
 from __future__ import (absolute_import, division, print_function)
+
 __metaclass__ = type
 
 import copy
 import os
 import yaml
 import sys
 import xml.etree.ElementTree as ET
 
-routePath = os.path.join(
-    os.path.abspath(
-        os.path.dirname(
-            os.path.dirname(__file__))),
-    "route",
-    "route.yml")
+modelRoute = os.path.join(os.path.abspath(os.path.dirname(os.path.dirname(__file__))),
+                          "route", "modelRoute.yml")
+interfaceRoute = os.path.join(os.path.abspath(os.path.dirname(os.path.dirname(__file__))),
+                              "route", "interfaceRoute.yml")
 
 
 # get yaml config util,singleton type
 class configUtil():
     def __init__(self):
         pass
 
@@ -27,75 +26,72 @@
         if not hasattr(cls, "_instance"):
             if sys.version_info < (3, 0):
                 cls._instance = super(configUtil, cls).__new__(cls, *args, **kwargs)
             else:
                 cls._instance = super().__new__(cls, *args, **kwargs)
         return cls._instance
 
-    # get all configuration option
-    def getRouteConfig(self):
-        '''
-        get route configuration to dict
-        :return: all route  dict
-        '''
-        if os.path.exists(routePath):
-            with open(routePath, 'r') as f:
-                serverconfig = yaml.load(f.read())
-                return serverconfig
-
-    def getRouteOption(self, productName, bmcVersion):
-        # try:
-        yaml1 = open(routePath)
-        content = yaml.load(yaml1, Loader=yaml.BaseLoader)
-        yaml1.close()
-        if "G220-A" in productName.upper():
-            productName = "G220-A"
-        elif "G226-A" in productName.upper():
-            productName = "G226-A"
-        elif "S520-A" in productName.upper():
-            productName = "S520-A"
-        if content.get(productName.upper(), None):
-            model_info = content.get(productName.upper())
-            model_keys = copy.deepcopy(list(model_info.keys()))
-            model_keys.remove('common')
-            if (bmcVersion is None or len(bmcVersion) == 0 or len(model_keys) == 0) and model_info.get('common'):
-                return model_info.get("common")
-            elif len(model_keys) >= 1:
-                model_keys.sort()
-                # model_keys = map(eval, model_keys)
-                if float(bmcVersion) < float(model_keys[0]):
-                    return model_info.get("common")
-                if len(model_keys) > 1:
-                    for i in range(len(model_keys) - 1):
-                        if float(bmcVersion) >= float(model_keys[i]) and float(bmcVersion) < float(model_keys[i + 1]):
-                            return model_info.get(str(model_keys[i]))
-                return model_info.get(str(model_keys[len(model_keys) - 1]))
-            else:
-                return "Error: Not find interface of {0}".format(productName)
-        return "Error: sdk does not support {0} at present.".format(productName)
+    def getRouteOption(self, productName, bmcVersion=None):
+        # if True:
+        try:
+            with open(modelRoute, "r") as file:
+                modeldict = yaml.safe_load(file)
+
+            with open(interfaceRoute, "r") as file:
+                interfacedict = yaml.safe_load(file)
+            content = {}
+            for key, value in modeldict.items():
+                for productname in value:
+                    content[productname.upper()] = interfacedict.get(key)
+
+            if content.get(productName.upper(), None):
+                model_info = content.get(productName.upper())
+                platform = model_info["platform"]
+                model_keysV = copy.deepcopy(list(model_info.keys()))
+                model_keysV.remove("platform")
+                model_keysV.remove('common')
+                model_keys = []
+                for model_key in model_keysV:
+                    model_keys.append(model_key.replace("V", ""))
+                if (bmcVersion is None or len(model_keys) == 0) and model_info.get('common'):
+                    return model_info.get("common"), platform
+                elif len(model_keys) >= 1:
+                    model_keys.sort()
+
+                    if float(bmcVersion) < float(model_keys[0]):
+                        return model_info.get("common")
+                    if len(model_keys) > 1:
+                        for i in range(len(model_keys) - 1):
+                            if float(bmcVersion) >= float(model_keys[i]) and float(bmcVersion) < float(
+                                    model_keys[i + 1]):
+                                return model_info.get("V" + str(model_keys[i])), platform
+                    return model_info.get("V" + str(model_keys[len(model_keys) - 1])), platform
+                else:
+                    return "Error: Not find interface of {0}".format(productName), None
+            return "Error: sdk does not support {0} at present.".format(productName), None
+        except Exception as e:
+            return "Error: " + str(e), None
 
     def getModelSupport(self):
         # try:
-        yaml1 = open(routePath)
+        yaml1 = open(modelRoute)
         content = yaml.load(yaml1, Loader=yaml.BaseLoader)
         yaml1.close()
         return list(content.keys())
 
-
     # xmlfilepath 文件路径
-    def getSetOption(self,xmlfilepath):
+    def getSetOption(self, xmlfilepath):
 
         tree = ET.parse(xmlfilepath)  # 调用parse方法返回解析树
-        server = tree.getroot()     # 获取根节点
+        server = tree.getroot()  # 获取根节点
 
-        blongtoSet = set()   # 存储所有的分类
+        blongtoSet = set()  # 存储所有的分类
         descriptionList = []  # 存储所有的描述
         infoList = []  # 存储所有xml表示的数据 字典列表
 
-
         def sortByKey(obj):
             return obj['key']
 
         for cfgItems in server:
             for cfgItem in cfgItems:
 
                 info = {}  # 字典
@@ -107,63 +103,61 @@
                         blongto_text = belongto.text
                     for description in name.iter('description'):
                         description_text = str(description.text).replace(" ", "")
 
                 blongtoSet.add(blongto_text)
                 descriptionList.append(description_text)
 
-
                 # getter标签
-                getterCMD=''
+                getterCMD = ''
                 for getter in cfgItem.iter('getter'):
                     getterCMD = getter.text
 
                 # parent标签
-                parentKey=''
+                parentKey = ''
                 for getter in cfgItem.iter('parent'):
                     parentKey = getter.text
 
-
                 # condition 标签
                 predict = {}
                 for conditions in cfgItem:
                     if conditions.tag == "conditions":
                         for precon in conditions.iter('condition'):
                             for cmd in precon.iter('key'):
                                 # 将tab键替换，换行键替换
-                                prekey = cmd.text.replace("\\t","").replace("\\n","")
+                                prekey = cmd.text.replace("\\t", "").replace("\\n", "")
                             for value in precon.iter('value'):
                                 prevalue = value.text
-                            predict[prekey]=prevalue
+                            predict[prekey] = prevalue
 
                 # #setters标签
                 setterlist = []  # 后面嵌套了setOption，是一个字典列表，每一项都是一个字典，字典里面包含{cmd，value，validation}
                 sin = False
                 for setters in cfgItem.iter('setters'):
                     for setter in setters.iter('setter'):
                         setOption = {}
                         for cmd in setter.iter('cmd'):
                             # 将tab键替换，换行键替换
-                            setOption['cmd'] = cmd.text.replace("\\t","").replace("\\n","")
-                            #2021年9月13日 不再依赖validation字段判断是否为范围
-                            #改为通过看cmd里面是否有$in
+                            setOption['cmd'] = cmd.text.replace("\\t", "").replace("\\n", "")
+                            # 2021年9月13日 不再依赖validation字段判断是否为范围
+                            # 改为通过看cmd里面是否有$in
                             if "$in" in cmd.text:
                                 sin = True
                         for value in setter.iter('value'):
                             setOption['value'] = value.text
                         for validation in setter.iter('validation'):
                             setOption['validation'] = validation.text
                             sin = True
                         # condition 标签
                         for conditions in setter.iter('conditions'):
-                            cmdpredict={}
+                            cmdpredict = {}
                             for precon in conditions.iter('condition'):
                                 for cmd in precon.iter('key'):
                                     # 将tab键替换，换行键替换
-                                    prekey = cmd.text.replace("\\t","").replace("\\n","")
+                                    prekey = cmd.text.replace("\\t", "").replace("\\n", "")
                                 for value in precon.iter('value'):
                                     prevalue = value.text
                                 cmdpredict[prekey] = prevalue
                             setOption["condition"] = cmdpredict
                         setterlist.append(setOption)
 
                 info['getter'] = getterCMD
@@ -173,8 +167,15 @@
                 info['blongto'] = blongto_text
                 info['input'] = sin
                 info['setter'] = setterlist
                 info['parent'] = parentKey
                 infoList.append(info)
 
         # infoList=sorted(infoList,key=lambda i:i['key'])
-        return blongtoSet, descriptionList ,infoList
+        return blongtoSet, descriptionList, infoList
+
+
+if __name__ == '__main__':
+    fruclass = configUtil()
+    # print(fruclass.getRouteConfig().get("NF5180M5"))
+    abc = fruclass.getRouteOption("NF5280M7", "5.3.0")
+    print(abc)
```

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/util/fileUtil.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/util/fileUtil.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspur_sm_sdk/util/parameterConversion.py` & `inspursmsdk-2.2.0/inspur_sm_sdk/util/parameterConversion.py`

 * *Files identical despite different names*

### Comparing `inspursmsdk-2.1.6/inspursmsdk.egg-info/PKG-INFO` & `inspursmsdk-2.2.0/inspursmsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inspursmsdk
-Version: 2.1.6
+Version: 2.2.0
 Summary: inspur server manager api
 Home-page: https://github.com/ISIB-Group/inspursmsdk
 Author: Wangbaoshan
 Author-email: wangbaoshan@inspur.com
 License: Expat License
 Description: # inspursmsdk
         inspursmsdk is a support tool for ansible.inspur.sm
```

### Comparing `inspursmsdk-2.1.6/inspursmsdk.egg-info/SOURCES.txt` & `inspursmsdk-2.2.0/inspursmsdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,27 +20,23 @@
 inspur_sm_sdk/command/M5Log/showSensorDesc.py
 inspur_sm_sdk/command/bios/A7.xml
 inspur_sm_sdk/command/bios/M4.xml
 inspur_sm_sdk/command/bios/M5.xml
 inspur_sm_sdk/command/bios/M6-N.xml
 inspur_sm_sdk/command/bios/M6.xml
 inspur_sm_sdk/command/bios/M7.xml
+inspur_sm_sdk/command/bios/M7_5.10.00.xml
 inspur_sm_sdk/command/bios/NF3180A6.xml
 inspur_sm_sdk/command/bios/NF3280A6.xml
 inspur_sm_sdk/command/bios/NF5180M5.xml
 inspur_sm_sdk/command/bios/NF5280M5.xml
 inspur_sm_sdk/command/bios/NF5468A5.xml
 inspur_sm_sdk/command/bios/NF5488A5.xml
 inspur_sm_sdk/command/bios/SA5112M5.xml
 inspur_sm_sdk/command/bios/SA5212M5.xml
-inspur_sm_sdk/conf/NF5180M5.yml
-inspur_sm_sdk/conf/NF5280M5.yml
-inspur_sm_sdk/conf/SA5112M5.yml
-inspur_sm_sdk/conf/SA5212M5.yml
-inspur_sm_sdk/conf/__init__.py
 inspur_sm_sdk/interface/Base.py
 inspur_sm_sdk/interface/CommonA5.py
 inspur_sm_sdk/interface/CommonA6.py
 inspur_sm_sdk/interface/CommonA7.py
 inspur_sm_sdk/interface/CommonA7_11308.py
 inspur_sm_sdk/interface/CommonM5.py
 inspur_sm_sdk/interface/CommonM6.py
@@ -57,15 +53,16 @@
 inspur_sm_sdk/interface/NF5280M5_435.py
 inspur_sm_sdk/interface/NF5280M5_436.py
 inspur_sm_sdk/interface/NS5160M6.py
 inspur_sm_sdk/interface/ResEntity.py
 inspur_sm_sdk/interface/SA5212M5Impl.py
 inspur_sm_sdk/interface/__init__.py
 inspur_sm_sdk/route/__init__.py
-inspur_sm_sdk/route/route.yml
+inspur_sm_sdk/route/interfaceRoute.yml
+inspur_sm_sdk/route/modelRoute.yml
 inspur_sm_sdk/util/HostTypeJudge.py
 inspur_sm_sdk/util/RedfishClient.py
 inspur_sm_sdk/util/RegularCheckUtil.py
 inspur_sm_sdk/util/RequestClient.py
 inspur_sm_sdk/util/__init__.py
 inspur_sm_sdk/util/configUtil.py
 inspur_sm_sdk/util/fileUtil.py
```

### Comparing `inspursmsdk-2.1.6/ism.py` & `inspursmsdk-2.2.0/ism.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ImportError:
     ISM_EXIST = False
 sys.path.append(os.path.join(sys.path[0], "interface"))
 current_time = time.strftime(
     '%Y-%m-%d   %H:%M:%S',
     time.localtime(
         time.time()))
-__version__ = '2.1.6'
+__version__ = '2.2.0'
 
 
 ERR_dict = {
     'ERR_CODE_CMN_FAIL': 'data acquisition exception',
     'ERR_CODE_PARAM_NULL': 'parameter is null',
     'ERR_CODE_INPUT_ERROR': 'parameter error',
     'ERR_CODE_INTF_FAIL': 'create link exception',
@@ -34,14 +34,15 @@
     'ERR_CODE_ALLOC_MEM': 'allocated memory exception',
     'ERR_CODE_NETWORK_CONNECT_FAIL': 'network connection failed',
     'ERR_CODE_AUTH_NAME_OR_PWD_ERROR': 'incorrect user name or password',
     'ERR_CODE_USER_NOT_EXIST': 'user not exist'
 }
 
 
+
 def main(params):
 
     def logout(signum, frame):
         if hasattr(client, "header"):
             RestFunc.logout(client)
 
     signal.signal(signal.SIGINT, logout)
@@ -73,64 +74,62 @@
     elif productName in ERR_dict:
         res['State'] = "Failure"
         res['Message'] = [ERR_dict.get(productName)]
         return res
     if firmwareVersion is None:
         res['State'] = "Failure"
         res['Message'] = ["cannot get BMC version"]
-        return
-    args.hostPlatform = productName
+        return res
     configutil = configUtil.configUtil()
-    impl = configutil.getRouteOption(productName, firmwareVersion)
+    impl, platform = configutil.getRouteOption(productName, firmwareVersion)
+    args.productName = productName
+    args.platform = platform
     if 'Error' in impl:
         res['State'] = "Failure"
         res['Message'] = [impl]
         return res
-    # if 'M5' not in impl and 'M6' not in impl and 'A5' not in impl and 'A6' not in impl:
-    #     res['State'] = "Failure"
-    #     res['Message'] = ['Not Support']
-    #     return res
     module_impl = 'inspur_sm_sdk.interface.' + impl
     obj = import_module(module_impl)
     targetclass = getattr(obj, impl)
     obj = targetclass()
     if args.subcommand is None:
         res['State'] = "Failure"
         res['Message'] = ["please input a subcommand"]
         return res
     targetMed = getattr(obj, args.subcommand)
     client = RequestClient.RequestClient()
     client.setself(
         args.host,
         args.username,
         args.passcode,
+        platform,
         args.port,
         'lanplus')
     try:
         resultJson = targetMed(client, args)
     except Exception as e:
         # 保留日志
-        # import traceback
-        # utool_path = os.path.dirname(os.path.abspath(__file__))
-        # # print(utool_path)
-        # log_path = os.path.join(utool_path, "log")
-        # if not os.path.exists(log_path):
-        #     os.makedirs(log_path)
-        # # TIME
-        # localtime = time.localtime()
-        # f_localdate = time.strftime("%Y-%m-%d", localtime)
-        # f_localtime = time.strftime("%Y-%m-%dT%H:%M:%S ", localtime)
-        #
-        # log_file = os.path.join(log_path, f_localdate)
-        # args.items()
-        # res_info = "[" + args.subcommand + "]" + traceback.format_exc()
-        # with open(log_file, 'a+') as logfile:
-        #     utoollog = "[ERROR]" + f_localtime + res_info + json.dumps(param, default=lambda o: o.__dict__, indent=4, ensure_ascii=True)
-        #     logfile.write(utoollog)
-        #     logfile.write("\n")
+        import traceback
+        utool_path = os.path.dirname(os.path.abspath(__file__))
+        # print(utool_path)
+        log_path = os.path.join(utool_path, "log")
+        if not os.path.exists(log_path):
+            os.makedirs(log_path)
+        # TIME
+        localtime = time.localtime()
+        f_localdate = time.strftime("%Y-%m-%d", localtime)
+        f_localtime = time.strftime("%Y-%m-%dT%H:%M:%S ", localtime)
+
+        log_file = os.path.join(log_path, f_localdate)
+        args.items()
+        res_info = "[" + args.subcommand + "]" + traceback.format_exc()
+        with open(log_file, 'a+') as logfile:
+            utoollog = "[ERROR]" + f_localtime + res_info + json.dumps(param, default=lambda o: o.__dict__, indent=4, ensure_ascii=True)
+            logfile.write(utoollog)
+            logfile.write("\n")
 
         res['State'] = "Failure"
         res['Message'] = ["Error occurs, request failed..."]
         return res
     sortedRes = collections.OrderedDict()
     sortedRes["State"] = resultJson.State
     sortedRes["Message"] = resultJson.Message
```

### Comparing `inspursmsdk-2.1.6/setup.py` & `inspursmsdk-2.2.0/setup.py`

 * *Files identical despite different names*


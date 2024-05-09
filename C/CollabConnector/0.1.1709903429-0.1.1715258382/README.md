# Comparing `tmp/CollabConnector-0.1.1709903429.tar.gz` & `tmp/collabconnector-0.1.1715258382.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CollabConnector-0.1.1709903429.tar", last modified: Fri Mar  8 13:10:37 2024, max compression
+gzip compressed data, was "collabconnector-0.1.1715258382.tar", last modified: Thu May  9 12:39:54 2024, max compression
```

## Comparing `CollabConnector-0.1.1709903429.tar` & `collabconnector-0.1.1715258382.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.987079 CollabConnector-0.1.1709903429/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 CollabConnector-0.1.1709903429/LICENSE
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-03-08 13:10:37.986930 CollabConnector-0.1.1709903429/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 CollabConnector-0.1.1709903429/README.md
--rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 CollabConnector-0.1.1709903429/pyproject.toml
--rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-03-08 13:10:37.987915 CollabConnector-0.1.1709903429/setup.cfg
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.664298 CollabConnector-0.1.1709903429/src/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.674135 CollabConnector-0.1.1709903429/src/CollabConnector/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.678371 CollabConnector-0.1.1709903429/src/CollabConnector/CER/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CER/CER.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CER/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.680211 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.682637 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AST/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AST/AST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AST/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.688418 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/AXL.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.667369 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.696859 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.714440 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.739989 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.759916 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.822045 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.856642 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.863376 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/14.0/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.883637 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/7.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.890791 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.908471 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.925687 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.942482 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.956258 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/CDR/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/CDR/CDR.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/CDR/CDROnDemand.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/CDR/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/CUCM.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.957797 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/DIME/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/DIME/DIME.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/DIME/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.959223 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Logs/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Logs/Logs.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Logs/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.961031 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Phone/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.962299 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Risport/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Risport/Risport.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Risport/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.963585 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Serviceability/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Serviceability/Serviceability.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Serviceability/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.964722 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/UDS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/UDS/UDS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/UDS/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.965721 CollabConnector-0.1.1709903429/src/CollabConnector/CUCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCX/CUCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/CUCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.966919 CollabConnector-0.1.1709903429/src/CollabConnector/Expressway/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Expressway/Expressway.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Expressway/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.968392 CollabConnector-0.1.1709903429/src/CollabConnector/IOS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 CollabConnector-0.1.1709903429/src/CollabConnector/IOS/IOS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 CollabConnector-0.1.1709903429/src/CollabConnector/IOS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.970368 CollabConnector-0.1.1709903429/src/CollabConnector/PAWS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/PAWS/PAWS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/PAWS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.971969 CollabConnector-0.1.1709903429/src/CollabConnector/UCCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 CollabConnector-0.1.1709903429/src/CollabConnector/UCCX/UCCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/UCCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.973668 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.975945 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Connect/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Connect/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Connect/TXT.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      154 2023-09-29 19:33:18.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Connect/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.977312 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Consent/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Consent/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Consent/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.979446 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/ContactCenter/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    12799 2024-03-08 12:56:21.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/ContactCenter/OutputStyle.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       64 2024-03-08 13:04:39.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/ContactCenter/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.983727 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/Chat.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/Team.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/User.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.985275 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Phone/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    11357 2024-03-08 13:06:56.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Webex.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 CollabConnector-0.1.1709903429/src/CollabConnector/Webex/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 CollabConnector-0.1.1709903429/src/CollabConnector/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:10:37.986275 CollabConnector-0.1.1709903429/src/CollabConnector.egg-info/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-03-08 13:10:37.000000 CollabConnector-0.1.1709903429/src/CollabConnector.egg-info/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4476 2024-03-08 13:10:37.000000 CollabConnector-0.1.1709903429/src/CollabConnector.egg-info/SOURCES.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-03-08 13:10:37.000000 CollabConnector-0.1.1709903429/src/CollabConnector.egg-info/dependency_links.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-03-08 13:10:37.000000 CollabConnector-0.1.1709903429/src/CollabConnector.egg-info/requires.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-03-08 13:10:37.000000 CollabConnector-0.1.1709903429/src/CollabConnector.egg-info/top_level.txt
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.254366 collabconnector-0.1.1715258382/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 collabconnector-0.1.1715258382/LICENSE
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-09 12:39:54.253984 collabconnector-0.1.1715258382/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 collabconnector-0.1.1715258382/README.md
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 collabconnector-0.1.1715258382/pyproject.toml
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-05-09 12:39:54.255715 collabconnector-0.1.1715258382/setup.cfg
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.897223 collabconnector-0.1.1715258382/src/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.910558 collabconnector-0.1.1715258382/src/CollabConnector/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.915197 collabconnector-0.1.1715258382/src/CollabConnector/CER/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 collabconnector-0.1.1715258382/src/CollabConnector/CER/CER.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CER/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.917295 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.919227 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AST/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AST/AST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AST/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.924781 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/AXL.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.902959 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.934371 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.955865 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.976990 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:53.999228 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.039741 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.085896 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.093961 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/14.0/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.126468 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/7.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.134859 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.155128 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.170675 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.189659 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.212933 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/CDR/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/CDR/CDR.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/CDR/CDROnDemand.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/CDR/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/CUCM.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.214762 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/DIME/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/DIME/DIME.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/DIME/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.216618 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Logs/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Logs/Logs.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Logs/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.218964 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Phone/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.220868 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Risport/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Risport/Risport.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Risport/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.223163 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Serviceability/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Serviceability/Serviceability.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Serviceability/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.224850 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/UDS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/UDS/UDS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/UDS/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCM/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.226348 collabconnector-0.1.1715258382/src/CollabConnector/CUCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCX/CUCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/CUCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.227892 collabconnector-0.1.1715258382/src/CollabConnector/Expressway/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 collabconnector-0.1.1715258382/src/CollabConnector/Expressway/Expressway.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 collabconnector-0.1.1715258382/src/CollabConnector/Expressway/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.230157 collabconnector-0.1.1715258382/src/CollabConnector/IOS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 collabconnector-0.1.1715258382/src/CollabConnector/IOS/IOS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 collabconnector-0.1.1715258382/src/CollabConnector/IOS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.231833 collabconnector-0.1.1715258382/src/CollabConnector/PAWS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/PAWS/PAWS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/PAWS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.233818 collabconnector-0.1.1715258382/src/CollabConnector/UCCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 collabconnector-0.1.1715258382/src/CollabConnector/UCCX/UCCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/UCCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.235689 collabconnector-0.1.1715258382/src/CollabConnector/Webex/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.238423 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Connect/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Connect/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Connect/TXT.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      154 2023-09-29 19:33:18.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Connect/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.239938 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Consent/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Consent/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Consent/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.242295 collabconnector-0.1.1715258382/src/CollabConnector/Webex/ContactCenter/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    12799 2024-03-08 12:56:21.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/ContactCenter/OutputStyle.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       64 2024-03-08 13:04:39.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/ContactCenter/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.248060 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/Chat.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/Team.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/User.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.250813 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Phone/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    17562 2024-05-09 12:39:38.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/Webex.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 collabconnector-0.1.1715258382/src/CollabConnector/Webex/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 collabconnector-0.1.1715258382/src/CollabConnector/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:39:54.252272 collabconnector-0.1.1715258382/src/CollabConnector.egg-info/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-09 12:39:53.000000 collabconnector-0.1.1715258382/src/CollabConnector.egg-info/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4476 2024-05-09 12:39:53.000000 collabconnector-0.1.1715258382/src/CollabConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-05-09 12:39:53.000000 collabconnector-0.1.1715258382/src/CollabConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-05-09 12:39:53.000000 collabconnector-0.1.1715258382/src/CollabConnector.egg-info/requires.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-05-09 12:39:53.000000 collabconnector-0.1.1715258382/src/CollabConnector.egg-info/top_level.txt
```

### Comparing `CollabConnector-0.1.1709903429/LICENSE` & `collabconnector-0.1.1715258382/LICENSE`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/PKG-INFO` & `collabconnector-0.1.1715258382/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1709903429
+Version: 0.1.1715258382
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1709903429/README.md` & `collabconnector-0.1.1715258382/README.md`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/setup.cfg` & `collabconnector-0.1.1715258382/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CollabConnector
-version = 0.1.1709903429
+version = 0.1.1715258382
 author = Jon Snipes
 author_email = jsnipes@mycollablab.org
 description = An attempt at a simplified API collection for Cisco Collab products
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mycollablab/CollabConnector
 project_urls =
```

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CER/CER.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CER/CER.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AST/AST.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AST/AST.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/AXL.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/AXL.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/CDR/CDR.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/CDR/CDR.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/CDR/CDROnDemand.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/CDR/CDROnDemand.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/CUCM.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/CUCM.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/DIME/DIME.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/DIME/DIME.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Logs/Logs.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Logs/Logs.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Phone/Phone.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Risport/Risport.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Risport/Risport.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/Serviceability/Serviceability.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/Serviceability/Serviceability.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCM/UDS/UDS.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCM/UDS/UDS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/CUCX/CUCX.py` & `collabconnector-0.1.1715258382/src/CollabConnector/CUCX/CUCX.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Expressway/Expressway.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Expressway/Expressway.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/IOS/IOS.py` & `collabconnector-0.1.1715258382/src/CollabConnector/IOS/IOS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/PAWS/PAWS.py` & `collabconnector-0.1.1715258382/src/CollabConnector/PAWS/PAWS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/UCCX/UCCX.py` & `collabconnector-0.1.1715258382/src/CollabConnector/UCCX/UCCX.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Connect/REST.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Connect/REST.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Connect/TXT.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Connect/TXT.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Consent/REST.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Consent/REST.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Consent/__init__.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Consent/__init__.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/ContactCenter/ContactCenter.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/ContactCenter/ContactCenter.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/ContactCenter/OutputStyle.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/ContactCenter/OutputStyle.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/Chat.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/Chat.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/REST.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/REST.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/Team.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/Team.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Engage/User.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Engage/User.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Phone/Phone.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector/Webex/Webex.py` & `collabconnector-0.1.1715258382/src/CollabConnector/Webex/Webex.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,134 +1,218 @@
 import sys
 from collections import OrderedDict
 import requests
+import requests.packages.urllib3
 import json
 import time
-import urllib
+import urllib.parse
+import base64
+import codecs
+from typing import Self
 
 requests.packages.urllib3.disable_warnings()
 
 
 class Connect:
-    class Token(object):
+    class Token:
         import time
         import threading
 
-    access_token = None
-    refresh_token = None
-    refresh_interval = 0
-    client_id = None
-    client_secret = None
+        access_token = None
+        refresh_token = None
+        refresh_interval = 0
+        client_id = None
+        client_secret = None
+
+        def __init__(self,
+                     access_token: str = None,
+                     refresh_token: str = None,
+                     client_id: str = None,
+                     client_secret: str = None,
+                     auth_file: str = None
+                     ):
+            if auth_file:
+                with open("webex_key.json") as auth_file:
+                    webex_key = json.loads(auth_file.read())
+                    client_id = webex_key['client_id'] if "client_id" in webex_key.keys() and webex_key['client_id'] else None
+                    client_secret = webex_key['client_secret'] if "client_secret" in webex_key.keys() and webex_key['client_secret'] else None
+                    access_token = webex_key['access_token']
+                    refresh_token = webex_key['refresh_token'] if "refresh_token" in webex_key.keys() and webex_key['refresh_token'] else None
+            self.access_token = access_token
+            if refresh_token and client_id and client_secret:
+                import threading
+                import time
+
+                self.refresh_token = refresh_token
+                self.client_id = client_id
+                self.client_secret = client_secret
+
+                thread = threading.Thread(target=self.token_refresh, args=())
+                thread.daemon = True
+                thread.start()
+
+        def info(self) -> dict:
+            return {
+                "access_token": self.access_token,
+                "refresh_token": self.refresh_token,
+                "client_id": self.client_id,
+                "client_secret": self.client_secret,
+                "expires_in": self.refresh_interval
+            }
+
+        # refresh token
+        def token_refresh(self) -> None:
+            while True:
+                time.sleep(1)
+                self.refresh_interval -= 1
+                if self.refresh_interval <= 0:
+                    refresh_data = {
+                        "grant_type": "refresh_token",
+                        "client_id": self.client_id,
+                        "client_secret": self.client_secret,
+                        "refresh_token": self.refresh_token
+                    }
+                    try:
+                        new_token = self.get_token(refresh_data)
+                    except Exception as err:
+                        raise Exception(f"Not able to perform Webex Token Refresh: {err}")
+                    else:
+                        self.access_token = new_token['access_token']
+                        self.refresh_token = new_token['refresh_token']
+                        self.refresh_interval = int(new_token['expires_in']) - 1000
+
+        # basic REST POST
+        def get_token(self, data: dict) -> dict:
+            headers = {"Accept": "application/json",
+                       "Content-Type": "application/json",
+                       "Authorization": f"Bearer {self.access_token}"}
+
+            while True:  # loop for throttling
+                try:
+                    response = requests.post("https://webexapis.com/v1/access_token",
+                                             headers=headers,
+                                             data=json.dumps(data),
+                                             verify=False)
+
+                except Exception as err:
+                    raise Exception(f"Error sending Webex REST Token Refresh - {err}")
+
+                else:
+                    if response.status_code == 426:  # handle throttling
+                        time.sleep(int(response.headers['Retry-After']) + 1)
+                    elif response.status_code == 200 and response.json():
+                        return json.loads(response.text)
+                    else:
+                        raise Exception(f"Not able to perform Webex Token Refresh: REST response not valid.")
+
+    token = None
     org = None
+    tenant_id = None
     active_org = None
     profile = None
     id = None
     service_url = "https://webexapis.com"
     type = "wbx"
+    guest_info = {}
 
     # store token then fetch users orgId and save
     def __init__(self,
                  access_token: str = None,
                  org_id: str = None,
                  refresh_token: str = None,
                  client_id: str = None,
-                 client_secret: str = None
+                 client_secret: str = None,
+                 auth_file: str = None
                  ):
-        if not access_token:
+        if access_token is None and auth_file is None:
             raise Exception("Must pass API token for Admin API")
         else:
-            self.access_token = access_token
+            self.token = self.Token(access_token, refresh_token, client_id, client_secret, auth_file)
 
             try:
                 self.profile = self.get("/v1/people/me?callingData=true")
                 self.id = self.profile['id']
                 self.org = self.profile['orgId']
                 self.active_org = self.org
 
             except Exception as err:
                 if client_id is None:
                     raise Exception(f"Error with Token or getting Org")
                 else:
                     print("User profile not found. Assuming Service App!", file=sys.stderr)
 
-            if refresh_token and client_id and client_secret:
-                import threading
-                import time
-
-                self.refresh_token = refresh_token
-                self.client_id = client_id
-                self.client_secret = client_secret
-
-                thread = threading.Thread(target=self.token_refresh, args=())
-                thread.daemon = True
-                thread.start()
-
             if org_id:
                 self.org = org_id
+            if self.org:
+                self.tenant_id = codecs.decode(base64.b64decode(f"{self.org}==============")).split("/")[-1]
+
+    #  set headers
+    def headers(self, send: bool = False):
+        if send:
+            return {
+                "Accept": "application/json",
+                "Content-Type":  "application/json",
+                "Authorization": f"Bearer {self.token.access_token}"
+            }
+        else:
+            return {
+                "Accept": "application/json",
+                "Authorization": f"Bearer {self.token.access_token}"
+            }
 
     # parses out paging from response headers
     @staticmethod
     def find_next_page(call_response):
         if 'Link' in call_response.headers:
             return call_response.headers['Link'].split(";")[0].strip("<>")
         else:
             return False
 
-    # refresh token
-    def token_refresh(self):
-        while True:
-            time.sleep(1)
-            self.refresh_interval -= 1
-            if self.refresh_interval <= 0:
-                refresh_data = {
-                                   "grant_type": "refresh_token",
-                                   "client_id": self.client_id,
-                                   "client_secret": self.client_secret,
-                                   "refresh_token": self.refresh_token
-                                }
-                try:
-                    new_token = self.post("/v1/access_token", refresh_data)
-                except Exception as err:
-                    raise Exception(f"Not able to perform Webex Token Refresh: {err}")
-                else:
-                    self.access_token = new_token['access_token']
-                    self.refresh_token = new_token['refresh_token']
-                    self.refresh_interval = int(new_token['expires_in']) - 1000
+    # create guest user
+    def guest(self, subject: str, display_name: str = "") -> Self:
+        guest_info = {
+            "displayName": display_name,
+            "subject": subject
+        }
+        guest_auth = self.post("/v1/guests/token", guest_info)
+        guest_account = Connect(guest_auth['accessToken'])
+        guest_account.guest_info = guest_info
+
+        return guest_account
 
     # basic REST GET
-    def get(self, uri, data=None, limit=50000, debug=False):
+    def get(self, uri, data=None, limit=50000, debug=False) -> dict:
         # URL encode parameters for appending to URI if provided
         if data:
-            data = f"?{urllib.urlencode(data)}"
+            data = f"?{urllib.parse.urlencode(data)}"
         else:
             data = ""
 
-        headers = {"Accept": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}  # set auth header
-
         uri = f"{self.service_url}/{uri.strip('/')}{data}"
         return_values = {'items': []}
         # Loop while true to handled paged results and throttling
         while True:
             try:
                 # send request to Webex
-                response = requests.get(uri, headers=headers, verify=False)
+                response = requests.get(uri, headers=self.headers(), verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex REST GET - {uri} {err}")
 
             else:
                 if debug:
                     print("GET", uri, response.status_code, response.headers)
                 if 200 <= response.status_code <= 300 and response.json():
                     # create or add to return dict
                     response_data = response.json()
                     if isinstance(response_data, dict) and len(response_data) == 1:
                         key = list(response_data.keys())[0]
                         response_data['items'] = response_data[key]
+                    if not isinstance(response_data, dict) or not isinstance(response_data, list):
+                        return response_data
                     if 'items' in response_data:
                         return_values['items'].extend(response_data['items'])
                     else:
                         return response_data
 
                     # check for additional and loop until max (limit minimum is 50)
                     if len(return_values['items']) >= limit or self.find_next_page(response) is False:
@@ -156,22 +240,80 @@
 
                 elif response.status_code == 401:  # handle auth issues
                     raise Exception("Webex Admin token invalid.  Generate new token")
                 else:  # catch generic failures
                     print(f"Error sending GET to Webex - {uri}{data} {response}{response.text}", file=sys.stderr)
                     raise Exception(f"Error sending GET to Webex - {uri}{data} {response}{response.text}")
 
+    # basic REST HEAD
+    def head(self, uri: str, full: bool = False, debug: bool = False) -> dict:
+        uri = uri.replace(self.service_url, "")
+        uri = f"{self.service_url}/{uri.strip('/')}"
+        # Loop while true to handled paged results and throttling
+        while True:
+            try:
+                # send request to Webex
+                response = requests.head(uri, headers=self.headers(), verify=False)
+
+            except Exception as err:
+                raise Exception(f"Error sending Webex REST GET - {uri} {err}")
+
+            else:
+                if debug:
+                    print("GET", uri, response.status_code, response.headers)
+                if 200 <= response.status_code < 300:
+                    return dict(response.headers)
+
+                elif response.status_code == 429:  # handle throttling
+                    print(f"Request to {uri} throttled.  Doing it again in a bit.", file=sys.stderr)
+                    time.sleep(int(response.headers['Retry-After']) + 1)
+
+                elif response.status_code == 401:  # handle auth issues
+                    raise Exception("Webex Admin token invalid.  Generate new token")
+                else:  # catch generic failures
+                    print(f"Error sending HEAD to Webex - {uri} {response}", file=sys.stderr)
+                    raise Exception(f"Error sending HEAD to Webex - {uri} {response}")
+
+    # basic REST GET for bytes content
+    def get_content(self, uri: str, debug: bool = False) -> bytes:
+        uri = f"{self.service_url}/{uri.strip('/')}"
+        # Loop while true to handled paged results and throttling
+        while True:
+            try:
+                # send request to Webex
+                response = requests.get(uri, headers=self.headers(), verify=False)
+
+            except Exception as err:
+                raise Exception(f"Error sending Webex REST GET - {uri} {err}")
+
+            else:
+                if debug:
+                    print("GET", uri, response.status_code, response.headers)
+                if 200 <= response.status_code <= 300 and response.json():
+                    # test for non-json responces ie: images
+                    if response.headers['Content-type'].split("/")[0] not in ["video", "audio", "image"]:
+                        return response.content
+                    else:
+                        raise Exception(f"Non-bytes response for {uri} Try regular get.")
+
+                elif response.status_code == 429:  # handle throttling
+                    print(f"Request to {uri} throttled.  Doing it again in a bit.", file=sys.stderr)
+                    time.sleep(int(response.headers['Retry-After']) + 1)
+
+                elif response.status_code == 401:  # handle auth issues
+                    raise Exception("Webex Admin token invalid.  Generate new token")
+                else:  # catch generic failures
+                    print(f"Error sending GET to Webex - {uri} {response}", file=sys.stderr)
+                    raise Exception(f"Error sending GET to Webex - {uri} {response}")
+
     # basic REST DELETE
     def delete(self, uri, debug=False):
-        headers = {"Accept": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}
-
         while True:  # loop for throttling
             try:
-                response = requests.delete(f"{self.service_url}/{uri.strip('/')}", headers=headers, verify=False)
+                response = requests.delete(f"{self.service_url}/{uri.strip('/')}", headers=self.headers(), verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex REST DELETE - {uri} {err}")
 
             else:
                 if debug:
                     print("DELETE", uri, response.status_code, response.headers)
@@ -182,22 +324,18 @@
                 elif 200 < response.status_code < 300:
                     return True
                 else:
                     raise Exception(f"Error sending DELETE to Webex - {uri} {response}{response.text}")
 
     # basic REST POST
     def post(self, uri, data, debug=False):
-        headers = {"Accept": "application/json",
-                   "Content-Type": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}
-
         while True:  # loop for throttling
             try:
                 response = requests.post(f"{self.service_url}/{uri.strip('/')}",
-                                         headers=headers,
+                                         headers=self.headers(True),
                                          data=json.dumps(data),
                                          verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex REST POST - {uri} {err}")
 
             else:
@@ -210,22 +348,18 @@
                 elif 200 < response.status_code < 300:
                     return True
                 else:
                     raise Exception(f"Error sending POST to Webex - {uri} {response}{response.text}")
 
     # basic REST PUT
     def put(self, uri, data, debug=False):
-        headers = {"Accept": "application/json",
-                   "Content-Type": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}
-
         while True:  # loop for throttling\
             try:
                 response = requests.put(f"{self.service_url}/{uri.strip('/')}",
-                                        headers=headers,
+                                        headers=self.headers(True),
                                         data=json.dumps(data),
                                         verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex REST PUT - {uri} {err}")
 
             else:
@@ -238,22 +372,18 @@
                 elif 200 < response.status_code < 300:
                     return True
                 else:
                     raise Exception(f"Error sending PUT to Webex - {uri} {response}{response.text}")
 
     # basic REST patch
     def patch(self, uri, data, debug=False):
-        headers = {"Accept": "application/json",
-                   "Content-Type": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}
-
         while True:  # loop for throttling
             try:
                 response = requests.patch(f"{self.service_url}/{uri.strip('/')}",
-                                          headers=headers,
+                                          headers=self.headers(True),
                                           data=json.dumps(data),
                                           verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex REST PATCH - {uri} {err}")
 
             else:
```

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector.egg-info/PKG-INFO` & `collabconnector-0.1.1715258382/src/CollabConnector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1709903429
+Version: 0.1.1715258382
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1709903429/src/CollabConnector.egg-info/SOURCES.txt` & `collabconnector-0.1.1715258382/src/CollabConnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*


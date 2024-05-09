# Comparing `tmp/collabconnector-0.1.1715258612.tar.gz` & `tmp/collabconnector-0.1.1715283497.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collabconnector-0.1.1715258612.tar", last modified: Thu May  9 12:43:36 2024, max compression
+gzip compressed data, was "collabconnector-0.1.1715283497.tar", last modified: Thu May  9 19:38:23 2024, max compression
```

## Comparing `collabconnector-0.1.1715258612.tar` & `collabconnector-0.1.1715283497.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.797591 collabconnector-0.1.1715258612/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 collabconnector-0.1.1715258612/LICENSE
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-09 12:43:36.797344 collabconnector-0.1.1715258612/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 collabconnector-0.1.1715258612/README.md
--rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 collabconnector-0.1.1715258612/pyproject.toml
--rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-05-09 12:43:36.798550 collabconnector-0.1.1715258612/setup.cfg
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.474659 collabconnector-0.1.1715258612/src/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.484971 collabconnector-0.1.1715258612/src/CollabConnector/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.488663 collabconnector-0.1.1715258612/src/CollabConnector/CER/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 collabconnector-0.1.1715258612/src/CollabConnector/CER/CER.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CER/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.490280 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.492431 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AST/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AST/AST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AST/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.498800 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/AXL.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.478104 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.508142 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.531382 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.553876 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.589570 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.619110 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.660188 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.667807 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/14.0/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.686676 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/7.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.692976 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.712939 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.730285 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.748192 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.764749 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/CDR/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/CDR/CDR.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/CDR/CDROnDemand.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/CDR/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/CUCM.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.766600 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/DIME/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/DIME/DIME.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/DIME/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.767912 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Logs/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Logs/Logs.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Logs/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.769717 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Phone/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.771021 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Risport/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Risport/Risport.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Risport/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.772495 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Serviceability/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Serviceability/Serviceability.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Serviceability/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.774221 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/UDS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/UDS/UDS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/UDS/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCM/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.775776 collabconnector-0.1.1715258612/src/CollabConnector/CUCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCX/CUCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/CUCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.777000 collabconnector-0.1.1715258612/src/CollabConnector/Expressway/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 collabconnector-0.1.1715258612/src/CollabConnector/Expressway/Expressway.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 collabconnector-0.1.1715258612/src/CollabConnector/Expressway/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.778834 collabconnector-0.1.1715258612/src/CollabConnector/IOS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 collabconnector-0.1.1715258612/src/CollabConnector/IOS/IOS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 collabconnector-0.1.1715258612/src/CollabConnector/IOS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.781165 collabconnector-0.1.1715258612/src/CollabConnector/PAWS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/PAWS/PAWS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/PAWS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.782594 collabconnector-0.1.1715258612/src/CollabConnector/UCCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 collabconnector-0.1.1715258612/src/CollabConnector/UCCX/UCCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/UCCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.784367 collabconnector-0.1.1715258612/src/CollabConnector/Webex/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.787177 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Connect/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Connect/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Connect/TXT.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1108 2024-05-09 12:42:58.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Connect/WhatsApp.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      224 2024-05-09 12:43:27.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Connect/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.788177 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Consent/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Consent/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Consent/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.790099 collabconnector-0.1.1715258612/src/CollabConnector/Webex/ContactCenter/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    12799 2024-03-08 12:56:21.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/ContactCenter/OutputStyle.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       64 2024-03-08 13:04:39.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/ContactCenter/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.793276 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/Chat.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/REST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/Team.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/User.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.794730 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Phone/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    17562 2024-05-09 12:39:38.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/Webex.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 collabconnector-0.1.1715258612/src/CollabConnector/Webex/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 collabconnector-0.1.1715258612/src/CollabConnector/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 12:43:36.796122 collabconnector-0.1.1715258612/src/CollabConnector.egg-info/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-09 12:43:36.000000 collabconnector-0.1.1715258612/src/CollabConnector.egg-info/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4522 2024-05-09 12:43:36.000000 collabconnector-0.1.1715258612/src/CollabConnector.egg-info/SOURCES.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-05-09 12:43:36.000000 collabconnector-0.1.1715258612/src/CollabConnector.egg-info/dependency_links.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-05-09 12:43:36.000000 collabconnector-0.1.1715258612/src/CollabConnector.egg-info/requires.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-05-09 12:43:36.000000 collabconnector-0.1.1715258612/src/CollabConnector.egg-info/top_level.txt
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.403607 collabconnector-0.1.1715283497/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 collabconnector-0.1.1715283497/LICENSE
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-09 19:38:23.403356 collabconnector-0.1.1715283497/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 collabconnector-0.1.1715283497/README.md
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 collabconnector-0.1.1715283497/pyproject.toml
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      965 2024-05-09 19:38:23.404759 collabconnector-0.1.1715283497/setup.cfg
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:22.977678 collabconnector-0.1.1715283497/src/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.044395 collabconnector-0.1.1715283497/src/CollabConnector/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.079076 collabconnector-0.1.1715283497/src/CollabConnector/CER/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2586 2023-07-06 17:16:08.000000 collabconnector-0.1.1715283497/src/CollabConnector/CER/CER.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CER/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.080635 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.082517 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AST/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    10786 2023-08-29 12:33:53.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AST/AST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AST/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.085823 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   357792 2023-08-30 01:25:13.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/AXL.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2023-08-29 16:07:10.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:22.981698 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.109801 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.127331 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.152414 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.177347 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.206325 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.257395 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.269379 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/14.0/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.291697 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/7.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.299255 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.319418 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.333508 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.352791 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.366530 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/CDR/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20752 2023-08-03 20:55:28.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/CDR/CDR.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/CDR/CDROnDemand.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/CDR/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    13200 2023-08-30 01:25:13.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/CUCM.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.368176 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/DIME/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/DIME/DIME.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/DIME/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.369667 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Logs/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Logs/Logs.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Logs/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.371552 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    30953 2023-07-06 17:17:27.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Phone/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.373199 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Risport/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Risport/Risport.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Risport/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.374708 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Serviceability/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Serviceability/Serviceability.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Serviceability/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.376267 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/UDS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2102 2023-07-06 17:15:02.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/UDS/UDS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/UDS/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCM/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.377579 collabconnector-0.1.1715283497/src/CollabConnector/CUCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15091 2023-08-29 12:24:59.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCX/CUCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/CUCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.379168 collabconnector-0.1.1715283497/src/CollabConnector/Expressway/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3529 2023-07-06 17:16:00.000000 collabconnector-0.1.1715283497/src/CollabConnector/Expressway/Expressway.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 collabconnector-0.1.1715283497/src/CollabConnector/Expressway/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.381173 collabconnector-0.1.1715283497/src/CollabConnector/IOS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    22137 2023-08-15 19:43:30.000000 collabconnector-0.1.1715283497/src/CollabConnector/IOS/IOS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 collabconnector-0.1.1715283497/src/CollabConnector/IOS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.382710 collabconnector-0.1.1715283497/src/CollabConnector/PAWS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/PAWS/PAWS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/PAWS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.384565 collabconnector-0.1.1715283497/src/CollabConnector/UCCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8554 2023-07-06 17:17:13.000000 collabconnector-0.1.1715283497/src/CollabConnector/UCCX/UCCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/UCCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.386410 collabconnector-0.1.1715283497/src/CollabConnector/Webex/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.389926 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Connect/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5205 2023-09-29 22:42:01.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Connect/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2942 2023-09-29 22:55:16.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Connect/TXT.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1108 2024-05-09 12:42:58.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Connect/WhatsApp.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      224 2024-05-09 12:43:27.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Connect/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.391657 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Consent/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5425 2023-09-29 23:50:27.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Consent/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1011 2023-09-29 23:52:18.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Consent/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.394569 collabconnector-0.1.1715283497/src/CollabConnector/Webex/ContactCenter/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14945 2024-05-09 19:37:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/ContactCenter/ContactCenter.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/ContactCenter/OutputStyle.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       64 2024-03-08 13:04:39.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/ContactCenter/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.399433 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8235 2023-11-02 16:46:15.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/Chat.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5439 2023-09-29 14:23:57.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/REST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1354 2023-09-29 14:23:57.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/Team.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4817 2023-11-02 16:51:10.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/User.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      338 2023-09-29 14:23:57.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.401336 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3412 2024-03-08 12:53:56.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Phone/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    17562 2024-05-09 12:39:38.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/Webex.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2024-03-08 13:05:25.000000 collabconnector-0.1.1715283497/src/CollabConnector/Webex/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2024-03-08 13:05:58.000000 collabconnector-0.1.1715283497/src/CollabConnector/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2024-05-09 19:38:23.402480 collabconnector-0.1.1715283497/src/CollabConnector.egg-info/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3569 2024-05-09 19:38:22.000000 collabconnector-0.1.1715283497/src/CollabConnector.egg-info/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4522 2024-05-09 19:38:22.000000 collabconnector-0.1.1715283497/src/CollabConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2024-05-09 19:38:22.000000 collabconnector-0.1.1715283497/src/CollabConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       77 2024-05-09 19:38:22.000000 collabconnector-0.1.1715283497/src/CollabConnector.egg-info/requires.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2024-05-09 19:38:22.000000 collabconnector-0.1.1715283497/src/CollabConnector.egg-info/top_level.txt
```

### Comparing `collabconnector-0.1.1715258612/LICENSE` & `collabconnector-0.1.1715283497/LICENSE`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/PKG-INFO` & `collabconnector-0.1.1715283497/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1715258612
+Version: 0.1.1715283497
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `collabconnector-0.1.1715258612/README.md` & `collabconnector-0.1.1715283497/README.md`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/setup.cfg` & `collabconnector-0.1.1715283497/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CollabConnector
-version = 0.1.1715258612
+version = 0.1.1715283497
 author = Jon Snipes
 author_email = jsnipes@mycollablab.org
 description = An attempt at a simplified API collection for Cisco Collab products
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mycollablab/CollabConnector
 project_urls =
```

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CER/CER.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CER/CER.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AST/AST.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AST/AST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/AXL.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/AXL.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/CDR/CDR.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/CDR/CDR.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/CDR/CDROnDemand.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/CDR/CDROnDemand.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/CUCM.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/CUCM.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/DIME/DIME.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/DIME/DIME.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Logs/Logs.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Logs/Logs.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Phone/Phone.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Risport/Risport.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Risport/Risport.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/Serviceability/Serviceability.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/Serviceability/Serviceability.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCM/UDS/UDS.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCM/UDS/UDS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/CUCX/CUCX.py` & `collabconnector-0.1.1715283497/src/CollabConnector/CUCX/CUCX.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Expressway/Expressway.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Expressway/Expressway.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/IOS/IOS.py` & `collabconnector-0.1.1715283497/src/CollabConnector/IOS/IOS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/PAWS/PAWS.py` & `collabconnector-0.1.1715283497/src/CollabConnector/PAWS/PAWS.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/UCCX/UCCX.py` & `collabconnector-0.1.1715283497/src/CollabConnector/UCCX/UCCX.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Connect/REST.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Connect/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Connect/TXT.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Connect/TXT.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Connect/WhatsApp.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Connect/WhatsApp.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Consent/REST.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Consent/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Consent/__init__.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Consent/__init__.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/ContactCenter/ContactCenter.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/ContactCenter/ContactCenter.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,85 +6,149 @@
 import time
 import urllib
 
 requests.packages.urllib3.disable_warnings()
 
 
 class Connect:
-    access_token = None
-    refresh_token = None
-    refresh_interval = 0
-    client_id = None
-    client_secret = None
+    class Token:
+        import time
+        import threading
+
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
     org_id = None
 
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
-            TextStyle.error("Must pass API token for Admin API")
+        if access_token is None and auth_file is None:
+            raise Exception("Must pass API token for Admin API")
         else:
-            self.access_token = access_token
-            if org_id:
-                self.org_id = org_id
-            else:
-                try:
-                    self.org_id = self.get("/v1/subscriptions")['meta']['orgId']
+            self.token = self.Token(access_token, refresh_token, client_id, client_secret, auth_file)
 
-                except Exception as err:
-                    if client_id is None:
-                        raise Exception(f"Error with Token or getting Org")
-                    else:
-                        print("User profile not found. Assuming Service App!", file=sys.stderr)
+            try:
+                self.org_id = self.get("/v1/subscriptions")['meta']['orgId']
 
-                if refresh_token and client_id and client_secret:
-                    import threading
-                    import time
-
-                    self.refresh_token = refresh_token
-                    self.client_id = client_id
-                    self.client_secret = client_secret
-
-                    thread = threading.Thread(target=self.token_refresh, args=())
-                    thread.daemon = True
-                    thread.start()
+            except Exception as err:
+                Exception ("Error retrieving Org ID from token. If token valid?")
 
-                if org_id:
-                    self.org = org_id
+            if org_id:
+                self.org = org_id
 
     # get next page for large requests
     @staticmethod
     def find_next_page(call_response):
         return True
 
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
+    #  set headers
+    def headers(self, payload: bool = False):
+        if payload:
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
 
     # basic REST GET
     def get(self, uri, data={}, page_size=50, page=0):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
         elif uri.find("/v1/") > -1 and self.org_id is not None:
             data['orgId'] = self.org_id
@@ -93,23 +157,20 @@
             uri = uri.replace("/{orgid}/", f"/{self.org_id}/")
 
         if len(data) > 0:
             data = f"&{urllib.parse.urlencode(data)}"
         else:
             data = ""
 
-        headers = {"Accept": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}
-
         return_data = {'data': [], 'meta': {}}
         api_url = f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}?pageSize={page_size}&page={page}{data}"
         while True:  # loop for throttling
             try:
                 response = requests.get(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}?pageSize={page_size}&page={page}{data}",
-                                        headers=headers,
+                                        headers=self.headers(),
                                         verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex CC REST GET - {uri} {err}")
 
             else:
                 if response.status_code == 200 and response.json():
@@ -169,21 +230,18 @@
                     TextStyle.error(f"Error sending CC GET to Webex - {uri}{data} {response}{response.text}")
                     return False
 
     def delete(self, uri):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
-        headers = {"Accept": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}
-
         while True:  # loop for throttling
             try:
                 response = requests.delete(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
-                                           headers=headers,
+                                           headers=self.headers(),
                                            verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex CC REST DELETE - {uri} {err}")
 
             else:
                 if response.status_code == 429:  # handle throttling
@@ -196,22 +254,18 @@
                     TextStyle.error(f"Error sending CC DELETE to Webex - {uri} {response}{response.text}")
                     return False
 
     def post(self, uri, data):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
-        headers = {"Accept": "application/json",
-                   "Content-Type": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}
-
         while True:  # loop for throttling
             try:
                 response = requests.post(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
-                                         headers=headers,
+                                         headers=self.headers(payload =True),
                                          data=json.dumps(data),
                                          verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex CC REST POST - {uri} {err}")
 
             else:
@@ -225,22 +279,18 @@
                     TextStyle.error(f"Error sending POST to Webex - {uri} {response}{response.text}")
                     return False
 
     def put(self, uri, data):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
-        headers = {"Accept": "application/json",
-                   "Content-Type": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}
-
         while True:  # loop for throttling
             try:
                 response = requests.put(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
-                                        headers=headers,
+                                        headers=self.headers(payload =True),
                                         data=json.dumps(data),
                                         verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex CC REST PUT - {uri} {err}")
 
             else:
@@ -254,22 +304,18 @@
                     TextStyle.error(f"Error sending PUT to Webex - {uri} {response}{response.text}")
                     return False
 
     def patch(self, uri, data):
         if uri.find("organization//") > -1:  # add org ID for ease of use
             uri = uri.replace("//", f"/{self.org_id}/")
 
-        headers = {"Accept": "application/json",
-                   "Content-Type": "application/json",
-                   "Authorization": f"Bearer {self.access_token}"}
-
         while True:  # loop for throttling
             try:
                 response = requests.patch(f"https://api.wxcc-us1.cisco.com/{uri.strip('/')}",
-                                          headers=headers,
+                                          headers=self.headers(payload =True),
                                           data=json.dumps(data),
                                           verify=False)
 
             except Exception as err:
                 raise Exception(f"Error sending Webex CC REST PATCH - {uri} {err}")
 
             else:
```

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/ContactCenter/OutputStyle.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/ContactCenter/OutputStyle.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/Chat.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/Chat.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/REST.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/REST.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/Team.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/Team.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Engage/User.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Engage/User.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Phone/Phone.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector/Webex/Webex.py` & `collabconnector-0.1.1715283497/src/CollabConnector/Webex/Webex.py`

 * *Files identical despite different names*

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector.egg-info/PKG-INFO` & `collabconnector-0.1.1715283497/src/CollabConnector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1715258612
+Version: 0.1.1715283497
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `collabconnector-0.1.1715258612/src/CollabConnector.egg-info/SOURCES.txt` & `collabconnector-0.1.1715283497/src/CollabConnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*


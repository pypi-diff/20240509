# Comparing `tmp/Unified-python-sdk-0.21.9.tar.gz` & `tmp/Unified-python-sdk-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Unified-python-sdk-0.21.9.tar", last modified: Fri Apr 26 00:26:34 2024, max compression
+gzip compressed data, was "Unified-python-sdk-0.22.0.tar", last modified: Thu May  9 00:26:34 2024, max compression
```

## Comparing `Unified-python-sdk-0.21.9.tar` & `Unified-python-sdk-0.22.0.tar`

### file list

```diff
@@ -1,440 +1,448 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.152959 Unified-python-sdk-0.21.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    92722 2024-04-26 00:26:34.152959 Unified-python-sdk-0.21.9/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    53343 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 00:26:34.152959 Unified-python-sdk-0.21.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.084960 Unified-python-sdk-0.21.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.084960 Unified-python-sdk-0.21.9/src/Unified_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    92722 2024-04-26 00:26:33.000000 Unified-python-sdk-0.21.9/src/Unified_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21011 2024-04-26 00:26:34.000000 Unified-python-sdk-0.21.9/src/Unified_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 00:26:33.000000 Unified-python-sdk-0.21.9/src/Unified_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-26 00:26:33.000000 Unified-python-sdk-0.21.9/src/Unified_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-26 00:26:33.000000 Unified-python-sdk-0.21.9/src/Unified_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.096960 Unified-python-sdk-0.21.9/src/unified_to/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.096960 Unified-python-sdk-0.21.9/src/unified_to/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    19424 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/account.py
--rw-r--r--   0 runner    (1001) docker     (127)   101260 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/accounting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/apicall.py
--rw-r--r--   0 runner    (1001) docker     (127)    19296 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/applicationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)   139530 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/ats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/call.py
--rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    75778 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/commerce.py
--rw-r--r--   0 runner    (1001) docker     (127)    28048 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/company.py
--rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    56361 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)   111142 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/crm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/customer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/deal.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/document.py
--rw-r--r--   0 runner    (1001) docker     (127)    19171 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)    18942 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    18989 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    49530 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/hris.py
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/interview.py
--rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19424 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6320 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/issue.py
--rw-r--r--   0 runner    (1001) docker     (127)    19143 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/item.py
--rw-r--r--   0 runner    (1001) docker     (127)    18819 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/lead.py
--rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/link.py
--rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/list.py
--rw-r--r--   0 runner    (1001) docker     (127)    19374 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/login.py
--rw-r--r--   0 runner    (1001) docker     (127)    37788 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/martech.py
--rw-r--r--   0 runner    (1001) docker     (127)    19230 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/member.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.096960 Unified-python-sdk-0.21.9/src/unified_to/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.100960 Unified-python-sdk-0.21.9/src/unified_to/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.136959 Unified-python-sdk-0.21.9/src/unified_to/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)    21975 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createhrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createhrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createmartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createmartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createpassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createpaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createpaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createstoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/createunifiedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingorganization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatscompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/gethrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/gethrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/gethrispayslip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/gethristimeoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getmartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getmartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getpaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getpaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getpaymentpayout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getpaymentrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getstoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedapicall.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedintegrationauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedintegrationlogin.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingcontacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountinginvoices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingtaxrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsactivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsapplications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsapplicationstatuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatscandidates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatscompanies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsdocuments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsinterviews.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsjobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsscorecards.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcommercecollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcommerceinventories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcommerceitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcommercelocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmcompanies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmcontacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmdeals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmleads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmpipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listenrichcompanies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listenrichpeople.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listhrisemployees.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listhrisgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listhrispayslips.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listhristimeoffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listmartechlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listmartechmembers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpassthroughs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpaymentlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpaymentpayments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpaymentpayouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpaymentrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/liststoragefiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listticketingcustomers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listticketingnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listticketingtickets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listuccalls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listuccontacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedapicalls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedconnections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedintegrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedintegrationworkspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedissues.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedsupports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedwebhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchhrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchhrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchmartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchmartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchpassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchpaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchpaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchstoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchunifiedwebhooktrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removehrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removehrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removemartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removemartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removepassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removepaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removepaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removestoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeunifiedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatehrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatehrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatemartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatemartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatepassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatepaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatepaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatestoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateunifiedwebhooktrigger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.152959 Unified-python-sdk-0.21.9/src/unified_to/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingcontactpaymentmethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountinglineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingorganization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingtelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingtransactionlineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/apicall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsapplicationanswer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atscompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atscompensation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsjobquestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsscorecardquestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/atstelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/commercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitemmedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitemoption.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitemprice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitemvariant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/commercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmtelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichperson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichpersonworkhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichtelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrisemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrispayslip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrispayslipdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/hristelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/hristimeoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/integrationsupport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/issue.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/marketingemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/marketinglist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/marketingmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentlinklineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentpayout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_accountingcontact_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_accountingcontact_shipping_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_accountingorganization_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_atscandidate_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_atscompany_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_commercelocation_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_connection_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_connection_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_connection_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmcompany_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmcontact_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_meeting.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmlead_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_enrichcompany_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_enrichperson_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_hrisemployee_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_integration_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_integrationsupport_webhook_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_created.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_deleted.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_storagepermission_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_uccall_telephone.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/storagefile.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/storagepermission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingtelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/uccall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/uccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/ucemail.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/uctelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/undefined.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/models/shared/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16091 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/passthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)    49784 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/payout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/payslip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/person.py
--rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/scorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8660 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19089 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/taxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19308 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)    56813 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/ticketing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/timeoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/uc.py
--rw-r--r--   0 runner    (1001) docker     (127)    57984 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/unified.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 00:26:34.152959 Unified-python-sdk-0.21.9/src/unified_to/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-26 00:26:25.000000 Unified-python-sdk-0.21.9/src/unified_to/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.211010 Unified-python-sdk-0.22.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    93632 2024-05-09 00:26:34.211010 Unified-python-sdk-0.22.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53802 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:26:34.211010 Unified-python-sdk-0.22.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.147009 Unified-python-sdk-0.22.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.151009 Unified-python-sdk-0.22.0/src/Unified_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    93632 2024-05-09 00:26:33.000000 Unified-python-sdk-0.22.0/src/Unified_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21322 2024-05-09 00:26:34.000000 Unified-python-sdk-0.22.0/src/Unified_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:26:33.000000 Unified-python-sdk-0.22.0/src/Unified_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-09 00:26:33.000000 Unified-python-sdk-0.22.0/src/Unified_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 00:26:33.000000 Unified-python-sdk-0.22.0/src/Unified_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.159009 Unified-python-sdk-0.22.0/src/unified_to/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.159009 Unified-python-sdk-0.22.0/src/unified_to/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102700 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/accounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19396 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/apicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19566 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/applicationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141555 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/ats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19762 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76858 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/commerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28453 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19348 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57171 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112762 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/crm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19696 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/deal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19441 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/employee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19212 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19356 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19259 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50250 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/hris.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10010 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19448 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/interview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19715 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19089 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/lead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19356 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19644 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38328 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/martech.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19500 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.159009 Unified-python-sdk-0.22.0/src/unified_to/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.163009 Unified-python-sdk-0.22.0/src/unified_to/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.195010 Unified-python-sdk-0.22.0/src/unified_to/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)    22145 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/creategenaiprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createhrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createhrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createmartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createmartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createpassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createpaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createpaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createstoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/createunifiedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingorganization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatscompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/gethrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/gethrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/gethrispayslip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/gethristimeoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getmartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getmartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getpaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getpaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getpaymentpayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getpaymentrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getstoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedapicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedintegrationauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedintegrationlogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingcontacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountinginvoices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingtaxrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsactivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsapplications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsapplicationstatuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatscandidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatscompanies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsdocuments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsinterviews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsjobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsscorecards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcommercecollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcommerceinventories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcommerceitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcommercelocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmcompanies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmcontacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmdeals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmleads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmpipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listenrichcompanies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listenrichpeople.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listgenaimodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listhrisemployees.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listhrisgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listhrispayslips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listhristimeoffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listmartechlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listmartechmembers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpassthroughs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpaymentlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpaymentpayments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpaymentpayouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpaymentrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/liststoragefiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listticketingcustomers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listticketingnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listticketingtickets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listuccalls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listuccontacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedapicalls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedconnections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedintegrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedintegrationworkspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedissues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedsupports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedwebhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchhrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchhrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchmartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchmartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchpassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchpaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchpaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchstoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchunifiedwebhooktrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removehrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removehrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removemartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removemartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removepassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removepaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removepaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removestoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeunifiedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatehrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatehrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatemartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatemartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatepassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatepaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatepaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatestoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateunifiedwebhooktrigger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.211010 Unified-python-sdk-0.22.0/src/unified_to/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingcontactpaymentmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5628 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountinglineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingorganization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingtelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingtransactionlineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/apicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsapplicationanswer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atscompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atscompensation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsjobquestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsscorecardquestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/atstelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/commercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitemmedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitemoption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitemprice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitemvariant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/commercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmtelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichperson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichpersonworkhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichtelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/genaicontent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/genaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/genaiprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrisemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrispayslip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrispayslipdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/hristelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/hristimeoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/integrationsupport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/marketingemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/marketinglist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/marketingmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentlinklineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentpayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_accountingcontact_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_accountingcontact_shipping_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_accountingorganization_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_atscandidate_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_atscompany_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_commercelocation_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_connection_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_connection_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_connection_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmcompany_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmcontact_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_meeting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmlead_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_enrichcompany_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_enrichperson_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_hrisemployee_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_integration_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_integrationsupport_webhook_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_updated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_storagepermission_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_uccall_telephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/storagefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/storagepermission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingtelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/uccall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/uccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/ucemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/uctelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/undefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/models/shared/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19460 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16316 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/payout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/payslip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/scorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19359 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19689 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/taxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57623 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/ticketing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/timeoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19925 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/uc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58846 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/unified.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:26:34.211010 Unified-python-sdk-0.22.0/src/unified_to/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18801 2024-05-09 00:26:21.000000 Unified-python-sdk-0.22.0/src/unified_to/webhook.py
```

### Comparing `Unified-python-sdk-0.21.9/LICENSE.md` & `Unified-python-sdk-0.22.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/PKG-INFO` & `Unified-python-sdk-0.22.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Unified-python-sdk
-Version: 0.21.9
+Version: 0.22.0
 Summary: Python Client SDK for Unified.to
 Home-page: https://github.com/unified-to/unified-python-sdk.git
 Author: Unified API Inc
 License: UNKNOWN
 Description: <div align="left">
             <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
             <a href="https://github.com/unified-to/unified-python-sdk/actions"><img src="https://img.shields.io/github/actions/workflow/status/unified-to/unified-python-sdk/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
@@ -30,19 +30,17 @@
         
         s = unified_to.UnifiedTo(
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
+        res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
             connection_id='<value>',
-        )
-        
-        res = s.accounting.create_accounting_account(req)
+        ))
         
         if res.accounting_account is not None:
             # handle response
             pass
         
         ```
         <!-- End SDK Example Usage [usage] -->
@@ -417,14 +415,27 @@
         * [list_enrich_companies](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/enrich/README.md#list_enrich_companies) - Retrieve enrichment information for a company
         * [list_enrich_people](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/enrich/README.md#list_enrich_people) - Retrieve enrichment information for a person
         
         ### [person](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/person/README.md)
         
         * [list_enrich_people](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/person/README.md#list_enrich_people) - Retrieve enrichment information for a person
         
+        ### [genai](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/README.md)
+        
+        * [create_genai_prompt](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/README.md#create_genai_prompt) - Create a prompt
+        * [list_genai_models](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/README.md#list_genai_models) - List all models
+        
+        ### [model](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/model/README.md)
+        
+        * [list_genai_models](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/model/README.md#list_genai_models) - List all models
+        
+        ### [prompt](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/prompt/README.md)
+        
+        * [create_genai_prompt](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/prompt/README.md#create_genai_prompt) - Create a prompt
+        
         ### [hris](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md)
         
         * [create_hris_employee](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#create_hris_employee) - Create an employee
         * [create_hris_group](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#create_hris_group) - Create a group
         * [get_hris_employee](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#get_hris_employee) - Retrieve an employee
         * [get_hris_group](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#get_hris_group) - Retrieve a group
         * [get_hris_payslip](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#get_hris_payslip) - Retrieve a payslip
@@ -716,21 +727,19 @@
         
         s = unified_to.UnifiedTo(
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
-            connection_id='<value>',
-        )
-        
         res = None
         try:
-            res = s.accounting.create_accounting_account(req)
+            res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
+            connection_id='<value>',
+        ))
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
         if res.accounting_account is not None:
             # handle response
             pass
@@ -761,19 +770,17 @@
         s = unified_to.UnifiedTo(
             server_idx=1,
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
+        res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
             connection_id='<value>',
-        )
-        
-        res = s.accounting.create_accounting_account(req)
+        ))
         
         if res.accounting_account is not None:
             # handle response
             pass
         
         ```
         
@@ -788,19 +795,17 @@
         s = unified_to.UnifiedTo(
             server_url="https://api.unified.to",
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
+        res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
             connection_id='<value>',
-        )
-        
-        res = s.accounting.create_accounting_account(req)
+        ))
         
         if res.accounting_account is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -843,19 +848,17 @@
         
         s = unified_to.UnifiedTo(
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
+        res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
             connection_id='<value>',
-        )
-        
-        res = s.accounting.create_accounting_account(req)
+        ))
         
         if res.accounting_account is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
```

#### html2text {}

```diff
@@ -1,129 +1,129 @@
-Metadata-Version: 2.1 Name: Unified-python-sdk Version: 0.21.9 Summary: Python
+Metadata-Version: 2.1 Name: Unified-python-sdk Version: 0.22.0 Summary: Python
 Client SDK for Unified.to Home-page: https://github.com/unified-to/unified-
 python-sdk.git Author: Unified API Inc License: UNKNOWN Description:
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_u_n_i_f_i_e_d_-_t_o_/_u_n_i_f_i_e_d_-
 _p_y_t_h_o_n_-_s_d_k_/_s_p_e_a_k_e_a_s_y___s_d_k___g_e_n_e_r_a_t_i_o_n_._y_m_l_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 ## SDK Installation ```bash pip install Unified-python-sdk ``` ## SDK Example
 Usage ### Example ```python import unified_to from unified_to.models import
 operations, shared s = unified_to.UnifiedTo( security=shared.Security( jwt="",
-), ) req = operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ## Available Resources and Operations ###
-[accounting](https://github.com/unified-to/unified-python-sdk/blob/master/docs/
-sdks/accounting/README.md) * [create_accounting_account](https://github.com/
-unified-to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#create_accounting_account) - Create an account *
-[create_accounting_contact](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#create_accounting_contact) - Create
-a contact * [create_accounting_invoice](https://github.com/unified-to/unified-
+), ) res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ## Available
+Resources and Operations ### [accounting](https://github.com/unified-to/
+unified-python-sdk/blob/master/docs/sdks/accounting/README.md) *
+[create_accounting_account](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#create_accounting_account) - Create
+an account * [create_accounting_contact](https://github.com/unified-to/unified-
 python-sdk/blob/master/docs/sdks/accounting/
-README.md#create_accounting_invoice) - Create an invoice *
-[create_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#create_accounting_taxrate) - Create
-a taxrate * [create_accounting_transaction](https://github.com/unified-to/
+README.md#create_accounting_contact) - Create a contact *
+[create_accounting_invoice](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#create_accounting_invoice) - Create
+an invoice * [create_accounting_taxrate](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/
+README.md#create_accounting_taxrate) - Create a taxrate *
+[create_accounting_transaction](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#create_accounting_transaction) -
+Create a transaction * [get_accounting_account](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#create_accounting_transaction) - Create a transaction *
-[get_accounting_account](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/accounting/README.md#get_accounting_account) - Retrieve an
-account * [get_accounting_contact](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/README.md#get_accounting_contact) -
-Retrieve a contact * [get_accounting_invoice](https://github.com/unified-to/
+README.md#get_accounting_account) - Retrieve an account *
+[get_accounting_contact](https://github.com/unified-to/unified-python-sdk/blob/
+master/docs/sdks/accounting/README.md#get_accounting_contact) - Retrieve a
+contact * [get_accounting_invoice](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/README.md#get_accounting_invoice) -
+Retrieve an invoice * [get_accounting_organization](https://github.com/unified-
+to/unified-python-sdk/blob/master/docs/sdks/accounting/
+README.md#get_accounting_organization) - Retrieve an organization *
+[get_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/blob/
+master/docs/sdks/accounting/README.md#get_accounting_taxrate) - Retrieve a
+taxrate * [get_accounting_transaction](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/
+README.md#get_accounting_transaction) - Retrieve a transaction *
+[list_accounting_accounts](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#list_accounting_accounts) - List all
+accounts * [list_accounting_contacts](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/README.md#list_accounting_contacts)
+- List all contacts * [list_accounting_invoices](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#get_accounting_invoice) - Retrieve an invoice *
-[get_accounting_organization](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#get_accounting_organization) -
-Retrieve an organization * [get_accounting_taxrate](https://github.com/unified-
+README.md#list_accounting_invoices) - List all invoices *
+[list_accounting_organizations](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#list_accounting_organizations) -
+List all organizations * [list_accounting_taxrates](https://github.com/unified-
 to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#get_accounting_taxrate) - Retrieve a taxrate *
-[get_accounting_transaction](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#get_accounting_transaction) -
-Retrieve a transaction * [list_accounting_accounts](https://github.com/unified-
+README.md#list_accounting_taxrates) - List all taxrates *
+[list_accounting_transactions](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#list_accounting_transactions) -
+List all transactions * [patch_accounting_account](https://github.com/unified-
 to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#list_accounting_accounts) - List all accounts *
-[list_accounting_contacts](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#list_accounting_contacts) - List all
-contacts * [list_accounting_invoices](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/README.md#list_accounting_invoices)
-- List all invoices * [list_accounting_organizations](https://github.com/
-unified-to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#list_accounting_organizations) - List all organizations *
-[list_accounting_taxrates](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#list_accounting_taxrates) - List all
-taxrates * [list_accounting_transactions](https://github.com/unified-to/
-unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#list_accounting_transactions) - List all transactions *
-[patch_accounting_account](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#patch_accounting_account) - Update
-an account * [patch_accounting_contact](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/README.md#patch_accounting_contact)
-- Update a contact * [patch_accounting_invoice](https://github.com/unified-to/
+README.md#patch_accounting_account) - Update an account *
+[patch_accounting_contact](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#patch_accounting_contact) - Update a
+contact * [patch_accounting_invoice](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/README.md#patch_accounting_invoice)
+- Update an invoice * [patch_accounting_taxrate](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#patch_accounting_invoice) - Update an invoice *
-[patch_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#patch_accounting_taxrate) - Update a
-taxrate * [patch_accounting_transaction](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/
-README.md#patch_accounting_transaction) - Update a transaction *
-[remove_accounting_account](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#remove_accounting_account) - Remove
-an account * [remove_accounting_contact](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/
-README.md#remove_accounting_contact) - Remove a contact *
-[remove_accounting_invoice](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#remove_accounting_invoice) - Remove
-an invoice * [remove_accounting_taxrate](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/
-README.md#remove_accounting_taxrate) - Remove a taxrate *
-[remove_accounting_transaction](https://github.com/unified-to/unified-python-
-sdk/blob/master/docs/sdks/accounting/README.md#remove_accounting_transaction) -
-Remove a transaction * [update_accounting_account](https://github.com/unified-
+README.md#patch_accounting_taxrate) - Update a taxrate *
+[patch_accounting_transaction](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#patch_accounting_transaction) -
+Update a transaction * [remove_accounting_account](https://github.com/unified-
 to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#update_accounting_account) - Update an account *
-[update_accounting_contact](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#update_accounting_contact) - Update
-a contact * [update_accounting_invoice](https://github.com/unified-to/unified-
+README.md#remove_accounting_account) - Remove an account *
+[remove_accounting_contact](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#remove_accounting_contact) - Remove
+a contact * [remove_accounting_invoice](https://github.com/unified-to/unified-
 python-sdk/blob/master/docs/sdks/accounting/
-README.md#update_accounting_invoice) - Update an invoice *
-[update_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#update_accounting_taxrate) - Update
-a taxrate * [update_accounting_transaction](https://github.com/unified-to/
+README.md#remove_accounting_invoice) - Remove an invoice *
+[remove_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#remove_accounting_taxrate) - Remove
+a taxrate * [remove_accounting_transaction](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#update_accounting_transaction) - Update a transaction ### [account]
-(https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/
-account/README.md) * [create_accounting_account](https://github.com/unified-to/
+README.md#remove_accounting_transaction) - Remove a transaction *
+[update_accounting_account](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#update_accounting_account) - Update
+an account * [update_accounting_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/
+README.md#update_accounting_contact) - Update a contact *
+[update_accounting_invoice](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#update_accounting_invoice) - Update
+an invoice * [update_accounting_taxrate](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/
+README.md#update_accounting_taxrate) - Update a taxrate *
+[update_accounting_transaction](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#update_accounting_transaction) -
+Update a transaction ### [account](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/account/README.md) *
+[create_accounting_account](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/account/README.md#create_accounting_account) - Create an
+account * [get_accounting_account](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/account/README.md#get_accounting_account) -
+Retrieve an account * [list_accounting_accounts](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/account/
-README.md#create_accounting_account) - Create an account *
-[get_accounting_account](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/account/README.md#get_accounting_account) - Retrieve an
-account * [list_accounting_accounts](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/account/README.md#list_accounting_accounts) -
-List all accounts * [patch_accounting_account](https://github.com/unified-to/
+README.md#list_accounting_accounts) - List all accounts *
+[patch_accounting_account](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/account/README.md#patch_accounting_account) - Update an
+account * [remove_accounting_account](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/account/README.md#remove_accounting_account) -
+Remove an account * [update_accounting_account](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/account/
-README.md#patch_accounting_account) - Update an account *
-[remove_accounting_account](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/account/README.md#remove_accounting_account) - Remove an
-account * [update_accounting_account](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/account/README.md#update_accounting_account) -
-Update an account ### [contact](https://github.com/unified-to/unified-python-
-sdk/blob/master/docs/sdks/contact/README.md) * [create_accounting_contact]
-(https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/
-contact/README.md#create_accounting_contact) - Create a contact *
-[create_crm_contact](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/contact/README.md#create_crm_contact) - Create a contact *
-[create_uc_contact](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/contact/README.md#create_uc_contact) - Create a contact *
-[get_accounting_contact](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/contact/README.md#get_accounting_contact) - Retrieve a contact
-* [get_crm_contact](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/contact/README.md#get_crm_contact) - Retrieve a contact *
-[get_uc_contact](https://github.com/unified-to/unified-python-sdk/blob/master/
-docs/sdks/contact/README.md#get_uc_contact) - Retrieve a contact *
+README.md#update_accounting_account) - Update an account ### [contact](https://
+github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/contact/
+README.md) * [create_accounting_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/contact/README.md#create_accounting_contact) -
+Create a contact * [create_crm_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/contact/README.md#create_crm_contact) - Create
+a contact * [create_uc_contact](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/contact/README.md#create_uc_contact) - Create a
+contact * [get_accounting_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/contact/README.md#get_accounting_contact) -
+Retrieve a contact * [get_crm_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/contact/README.md#get_crm_contact) - Retrieve
+a contact * [get_uc_contact](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/contact/README.md#get_uc_contact) - Retrieve a contact *
 [list_accounting_contacts](https://github.com/unified-to/unified-python-sdk/
 blob/master/docs/sdks/contact/README.md#list_accounting_contacts) - List all
 contacts * [list_crm_contacts](https://github.com/unified-to/unified-python-
 sdk/blob/master/docs/sdks/contact/README.md#list_crm_contacts) - List all
 contacts * [list_uc_contacts](https://github.com/unified-to/unified-python-sdk/
 blob/master/docs/sdks/contact/README.md#list_uc_contacts) - List all contacts *
 [patch_accounting_contact](https://github.com/unified-to/unified-python-sdk/
@@ -659,17 +659,29 @@
 README.md#list_enrich_companies) - Retrieve enrichment information for a
 company * [list_enrich_people](https://github.com/unified-to/unified-python-
 sdk/blob/master/docs/sdks/enrich/README.md#list_enrich_people) - Retrieve
 enrichment information for a person ### [person](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/person/README.md) *
 [list_enrich_people](https://github.com/unified-to/unified-python-sdk/blob/
 master/docs/sdks/person/README.md#list_enrich_people) - Retrieve enrichment
-information for a person ### [hris](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/hris/README.md) * [create_hris_employee]
-(https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
+information for a person ### [genai](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/genai/README.md) * [create_genai_prompt]
+(https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/
+README.md#create_genai_prompt) - Create a prompt * [list_genai_models](https://
+github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/
+README.md#list_genai_models) - List all models ### [model](https://github.com/
+unified-to/unified-python-sdk/blob/master/docs/sdks/model/README.md) *
+[list_genai_models](https://github.com/unified-to/unified-python-sdk/blob/
+master/docs/sdks/model/README.md#list_genai_models) - List all models ###
+[prompt](https://github.com/unified-to/unified-python-sdk/blob/master/docs/
+sdks/prompt/README.md) * [create_genai_prompt](https://github.com/unified-to/
+unified-python-sdk/blob/master/docs/sdks/prompt/README.md#create_genai_prompt)
+- Create a prompt ### [hris](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/hris/README.md) * [create_hris_employee](https://
+github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
 README.md#create_hris_employee) - Create an employee * [create_hris_group]
 (https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
 README.md#create_hris_group) - Create a group * [get_hris_employee](https://
 github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
 README.md#get_hris_employee) - Retrieve an employee * [get_hris_group](https://
 github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
 README.md#get_hris_group) - Retrieve a group * [get_hris_payslip](https://
@@ -1097,58 +1109,59 @@
 README.md#update_unified_webhook_trigger) - Trigger webhook ## Error Handling
 Handling errors in this SDK should largely match your expectations. All
 operations return a response object or raise an error. If Error objects are
 specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 | Error Object | Status Code | Content Type | | --------------- | -------------
 -- | --------------- | | errors.SDKError | 4xx-5xx | */* | ### Example
 ```python import unified_to from unified_to.models import errors, operations,
-shared s = unified_to.UnifiedTo( security=shared.Security( jwt="", ), ) req =
-operations.CreateAccountingAccountRequest( connection_id='', ) res = None try:
-res = s.accounting.create_accounting_account(req) except errors.SDKError as e:
-# handle exception raise(e) if res.accounting_account is not None: # handle
-response pass ``` ## Server Selection ### Select Server by Index You can
-override the default server globally by passing a server index to the
-`server_idx: int` optional parameter when initializing the SDK client instance.
-The selected server will then be used as the default on the operations that use
-it. This table lists the indexes associated with the available servers: | # |
-Server | Variables | | - | ------ | --------- | | 0 | `https://api.unified.to`
-| None | | 1 | `https://api-eu.unified.to` | None | #### Example ```python
-import unified_to from unified_to.models import operations, shared s =
-unified_to.UnifiedTo( server_idx=1, security=shared.Security( jwt="", ), ) req
-= operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ### Override Server URL Per-Client The default
-server can also be overridden globally by passing a URL to the `server_url:
-str` optional parameter when initializing the SDK client instance. For example:
-```python import unified_to from unified_to.models import operations, shared s
-= unified_to.UnifiedTo( server_url="https://api.unified.to",
-security=shared.Security( jwt="", ), ) req =
-operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ## Custom HTTP Client The Python SDK makes API
-calls using the [requests](https://pypi.org/project/requests/) HTTP library. In
-order to provide a convenient way to configure timeouts, cookies, proxies,
-custom headers, and other low-level configuration, you can initialize the SDK
-client with a custom `requests.Session` object. For example, you could specify
-a header for every request that this sdk makes as follows: ```python import
-unified_to import requests http_client = requests.Session()
-http_client.headers.update({'x-custom-header': 'someValue'}) s =
-unified_to.UnifiedTo(client=http_client) ``` ## Authentication ### Per-Client
-Security Schemes This SDK supports the following security scheme globally: |
-Name | Type | Scheme | | ------- | ------- | ------- | | `jwt` | apiKey | API
-key | You can set the security parameters through the `security` optional
-parameter when initializing the SDK client instance. For example: ```python
-import unified_to from unified_to.models import operations, shared s =
-unified_to.UnifiedTo( security=shared.Security( jwt="", ), ) req =
-operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ### Maturity This SDK is in beta, and there
-may be breaking changes between versions without a major version update.
-Therefore, we recommend pinning usage to a specific package version. This way,
-you can install the same version each time without breaking changes unless you
-are intentionally looking for the latest version. ### Contributions While we
-value open-source contributions to this SDK, this library is generated
-programmatically. Feel free to open a PR or a Github issue as a proof of
-concept and we'll do our best to include it in a future release! ### SDK
-Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
-client-sdks) Platform: UNKNOWN Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: dev
+shared s = unified_to.UnifiedTo( security=shared.Security( jwt="", ), ) res =
+None try: res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) except
+errors.SDKError as e: # handle exception raise(e) if res.accounting_account is
+not None: # handle response pass ``` ## Server Selection ### Select Server by
+Index You can override the default server globally by passing a server index to
+the `server_idx: int` optional parameter when initializing the SDK client
+instance. The selected server will then be used as the default on the
+operations that use it. This table lists the indexes associated with the
+available servers: | # | Server | Variables | | - | ------ | --------- | | 0 |
+`https://api.unified.to` | None | | 1 | `https://api-eu.unified.to` | None |
+#### Example ```python import unified_to from unified_to.models import
+operations, shared s = unified_to.UnifiedTo( server_idx=1,
+security=shared.Security( jwt="", ), ) res =
+s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ### Override
+Server URL Per-Client The default server can also be overridden globally by
+passing a URL to the `server_url: str` optional parameter when initializing the
+SDK client instance. For example: ```python import unified_to from
+unified_to.models import operations, shared s = unified_to.UnifiedTo
+( server_url="https://api.unified.to", security=shared.Security( jwt="", ), )
+res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ## Custom HTTP
+Client The Python SDK makes API calls using the [requests](https://pypi.org/
+project/requests/) HTTP library. In order to provide a convenient way to
+configure timeouts, cookies, proxies, custom headers, and other low-level
+configuration, you can initialize the SDK client with a custom
+`requests.Session` object. For example, you could specify a header for every
+request that this sdk makes as follows: ```python import unified_to import
+requests http_client = requests.Session() http_client.headers.update({'x-
+custom-header': 'someValue'}) s = unified_to.UnifiedTo(client=http_client) ```
+## Authentication ### Per-Client Security Schemes This SDK supports the
+following security scheme globally: | Name | Type | Scheme | | ------- | ------
+- | ------- | | `jwt` | apiKey | API key | You can set the security parameters
+through the `security` optional parameter when initializing the SDK client
+instance. For example: ```python import unified_to from unified_to.models
+import operations, shared s = unified_to.UnifiedTo( security=shared.Security
+( jwt="", ), ) res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ### Maturity
+This SDK is in beta, and there may be breaking changes between versions without
+a major version update. Therefore, we recommend pinning usage to a specific
+package version. This way, you can install the same version each time without
+breaking changes unless you are intentionally looking for the latest version.
+### Contributions While we value open-source contributions to this SDK, this
+library is generated programmatically. Feel free to open a PR or a Github issue
+as a proof of concept and we'll do our best to include it in a future release!
+### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-
+speakeasy/client-sdks) Platform: UNKNOWN Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `Unified-python-sdk-0.21.9/README.md` & `Unified-python-sdk-0.22.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,17 @@
 
 s = unified_to.UnifiedTo(
     security=shared.Security(
         jwt="<YOUR_API_KEY_HERE>",
     ),
 )
 
-req = operations.CreateAccountingAccountRequest(
+res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
     connection_id='<value>',
-)
-
-res = s.accounting.create_accounting_account(req)
+))
 
 if res.accounting_account is not None:
     # handle response
     pass
 
 ```
 <!-- End SDK Example Usage [usage] -->
@@ -410,14 +408,27 @@
 * [list_enrich_companies](docs/sdks/enrich/README.md#list_enrich_companies) - Retrieve enrichment information for a company
 * [list_enrich_people](docs/sdks/enrich/README.md#list_enrich_people) - Retrieve enrichment information for a person
 
 ### [person](docs/sdks/person/README.md)
 
 * [list_enrich_people](docs/sdks/person/README.md#list_enrich_people) - Retrieve enrichment information for a person
 
+### [genai](docs/sdks/genai/README.md)
+
+* [create_genai_prompt](docs/sdks/genai/README.md#create_genai_prompt) - Create a prompt
+* [list_genai_models](docs/sdks/genai/README.md#list_genai_models) - List all models
+
+### [model](docs/sdks/model/README.md)
+
+* [list_genai_models](docs/sdks/model/README.md#list_genai_models) - List all models
+
+### [prompt](docs/sdks/prompt/README.md)
+
+* [create_genai_prompt](docs/sdks/prompt/README.md#create_genai_prompt) - Create a prompt
+
 ### [hris](docs/sdks/hris/README.md)
 
 * [create_hris_employee](docs/sdks/hris/README.md#create_hris_employee) - Create an employee
 * [create_hris_group](docs/sdks/hris/README.md#create_hris_group) - Create a group
 * [get_hris_employee](docs/sdks/hris/README.md#get_hris_employee) - Retrieve an employee
 * [get_hris_group](docs/sdks/hris/README.md#get_hris_group) - Retrieve a group
 * [get_hris_payslip](docs/sdks/hris/README.md#get_hris_payslip) - Retrieve a payslip
@@ -709,21 +720,19 @@
 
 s = unified_to.UnifiedTo(
     security=shared.Security(
         jwt="<YOUR_API_KEY_HERE>",
     ),
 )
 
-req = operations.CreateAccountingAccountRequest(
-    connection_id='<value>',
-)
-
 res = None
 try:
-    res = s.accounting.create_accounting_account(req)
+    res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
+    connection_id='<value>',
+))
 except errors.SDKError as e:
     # handle exception
     raise(e)
 
 if res.accounting_account is not None:
     # handle response
     pass
@@ -754,19 +763,17 @@
 s = unified_to.UnifiedTo(
     server_idx=1,
     security=shared.Security(
         jwt="<YOUR_API_KEY_HERE>",
     ),
 )
 
-req = operations.CreateAccountingAccountRequest(
+res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
     connection_id='<value>',
-)
-
-res = s.accounting.create_accounting_account(req)
+))
 
 if res.accounting_account is not None:
     # handle response
     pass
 
 ```
 
@@ -781,19 +788,17 @@
 s = unified_to.UnifiedTo(
     server_url="https://api.unified.to",
     security=shared.Security(
         jwt="<YOUR_API_KEY_HERE>",
     ),
 )
 
-req = operations.CreateAccountingAccountRequest(
+res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
     connection_id='<value>',
-)
-
-res = s.accounting.create_accounting_account(req)
+))
 
 if res.accounting_account is not None:
     # handle response
     pass
 
 ```
 <!-- End Server Selection [server] -->
@@ -836,19 +841,17 @@
 
 s = unified_to.UnifiedTo(
     security=shared.Security(
         jwt="<YOUR_API_KEY_HERE>",
     ),
 )
 
-req = operations.CreateAccountingAccountRequest(
+res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
     connection_id='<value>',
-)
-
-res = s.accounting.create_accounting_account(req)
+))
 
 if res.accounting_account is not None:
     # handle response
     pass
 
 ```
 <!-- End Authentication [security] -->
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_u_n_i_f_i_e_d_-_t_o_/_u_n_i_f_i_e_d_-
 _p_y_t_h_o_n_-_s_d_k_/_s_p_e_a_k_e_a_s_y___s_d_k___g_e_n_e_r_a_t_i_o_n_._y_m_l_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 ## SDK Installation ```bash pip install Unified-python-sdk ``` ## SDK Example
 Usage ### Example ```python import unified_to from unified_to.models import
 operations, shared s = unified_to.UnifiedTo( security=shared.Security( jwt="",
-), ) req = operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ## Available Resources and Operations ###
-[accounting](docs/sdks/accounting/README.md) * [create_accounting_account]
-(docs/sdks/accounting/README.md#create_accounting_account) - Create an account
-* [create_accounting_contact](docs/sdks/accounting/
+), ) res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ## Available
+Resources and Operations ### [accounting](docs/sdks/accounting/README.md) *
+[create_accounting_account](docs/sdks/accounting/
+README.md#create_accounting_account) - Create an account *
+[create_accounting_contact](docs/sdks/accounting/
 README.md#create_accounting_contact) - Create a contact *
 [create_accounting_invoice](docs/sdks/accounting/
 README.md#create_accounting_invoice) - Create an invoice *
 [create_accounting_taxrate](docs/sdks/accounting/
 README.md#create_accounting_taxrate) - Create a taxrate *
 [create_accounting_transaction](docs/sdks/accounting/
 README.md#create_accounting_transaction) - Create a transaction *
@@ -428,68 +429,74 @@
 [update_crm_pipeline](docs/sdks/pipeline/README.md#update_crm_pipeline) -
 Update a pipeline ### [enrich](docs/sdks/enrich/README.md) *
 [list_enrich_companies](docs/sdks/enrich/README.md#list_enrich_companies) -
 Retrieve enrichment information for a company * [list_enrich_people](docs/sdks/
 enrich/README.md#list_enrich_people) - Retrieve enrichment information for a
 person ### [person](docs/sdks/person/README.md) * [list_enrich_people](docs/
 sdks/person/README.md#list_enrich_people) - Retrieve enrichment information for
-a person ### [hris](docs/sdks/hris/README.md) * [create_hris_employee](docs/
-sdks/hris/README.md#create_hris_employee) - Create an employee *
-[create_hris_group](docs/sdks/hris/README.md#create_hris_group) - Create a
-group * [get_hris_employee](docs/sdks/hris/README.md#get_hris_employee) -
-Retrieve an employee * [get_hris_group](docs/sdks/hris/
-README.md#get_hris_group) - Retrieve a group * [get_hris_payslip](docs/sdks/
-hris/README.md#get_hris_payslip) - Retrieve a payslip * [get_hris_timeoff]
-(docs/sdks/hris/README.md#get_hris_timeoff) - Retrieve a timeoff *
-[list_hris_employees](docs/sdks/hris/README.md#list_hris_employees) - List all
-employees * [list_hris_groups](docs/sdks/hris/README.md#list_hris_groups) -
-List all groups * [list_hris_payslips](docs/sdks/hris/
-README.md#list_hris_payslips) - List all payslips * [list_hris_timeoffs](docs/
-sdks/hris/README.md#list_hris_timeoffs) - List all timeoffs *
-[patch_hris_employee](docs/sdks/hris/README.md#patch_hris_employee) - Update an
-employee * [patch_hris_group](docs/sdks/hris/README.md#patch_hris_group) -
-Update a group * [remove_hris_employee](docs/sdks/hris/
-README.md#remove_hris_employee) - Remove an employee * [remove_hris_group]
-(docs/sdks/hris/README.md#remove_hris_group) - Remove a group *
-[update_hris_employee](docs/sdks/hris/README.md#update_hris_employee) - Update
-an employee * [update_hris_group](docs/sdks/hris/README.md#update_hris_group) -
-Update a group ### [employee](docs/sdks/employee/README.md) *
-[create_hris_employee](docs/sdks/employee/README.md#create_hris_employee) -
-Create an employee * [get_hris_employee](docs/sdks/employee/
-README.md#get_hris_employee) - Retrieve an employee * [list_hris_employees]
-(docs/sdks/employee/README.md#list_hris_employees) - List all employees *
-[patch_hris_employee](docs/sdks/employee/README.md#patch_hris_employee) -
-Update an employee * [remove_hris_employee](docs/sdks/employee/
-README.md#remove_hris_employee) - Remove an employee * [update_hris_employee]
-(docs/sdks/employee/README.md#update_hris_employee) - Update an employee ###
-[group](docs/sdks/group/README.md) * [create_hris_group](docs/sdks/group/
-README.md#create_hris_group) - Create a group * [get_hris_group](docs/sdks/
-group/README.md#get_hris_group) - Retrieve a group * [list_hris_groups](docs/
-sdks/group/README.md#list_hris_groups) - List all groups * [patch_hris_group]
-(docs/sdks/group/README.md#patch_hris_group) - Update a group *
-[remove_hris_group](docs/sdks/group/README.md#remove_hris_group) - Remove a
-group * [update_hris_group](docs/sdks/group/README.md#update_hris_group) -
-Update a group ### [payslip](docs/sdks/payslip/README.md) * [get_hris_payslip]
-(docs/sdks/payslip/README.md#get_hris_payslip) - Retrieve a payslip *
-[list_hris_payslips](docs/sdks/payslip/README.md#list_hris_payslips) - List all
-payslips ### [timeoff](docs/sdks/timeoff/README.md) * [get_hris_timeoff](docs/
-sdks/timeoff/README.md#get_hris_timeoff) - Retrieve a timeoff *
-[list_hris_timeoffs](docs/sdks/timeoff/README.md#list_hris_timeoffs) - List all
-timeoffs ### [martech](docs/sdks/martech/README.md) * [create_martech_list]
-(docs/sdks/martech/README.md#create_martech_list) - Create a list *
-[create_martech_member](docs/sdks/martech/README.md#create_martech_member) -
-Create a member * [get_martech_list](docs/sdks/martech/
-README.md#get_martech_list) - Retrieve a list * [get_martech_member](docs/sdks/
-martech/README.md#get_martech_member) - Retrieve a member *
-[list_martech_lists](docs/sdks/martech/README.md#list_martech_lists) - List all
-lists * [list_martech_members](docs/sdks/martech/
-README.md#list_martech_members) - List all members * [patch_martech_list](docs/
-sdks/martech/README.md#patch_martech_list) - Update a list *
-[patch_martech_member](docs/sdks/martech/README.md#patch_martech_member) -
-Update a member * [remove_martech_list](docs/sdks/martech/
+a person ### [genai](docs/sdks/genai/README.md) * [create_genai_prompt](docs/
+sdks/genai/README.md#create_genai_prompt) - Create a prompt *
+[list_genai_models](docs/sdks/genai/README.md#list_genai_models) - List all
+models ### [model](docs/sdks/model/README.md) * [list_genai_models](docs/sdks/
+model/README.md#list_genai_models) - List all models ### [prompt](docs/sdks/
+prompt/README.md) * [create_genai_prompt](docs/sdks/prompt/
+README.md#create_genai_prompt) - Create a prompt ### [hris](docs/sdks/hris/
+README.md) * [create_hris_employee](docs/sdks/hris/
+README.md#create_hris_employee) - Create an employee * [create_hris_group]
+(docs/sdks/hris/README.md#create_hris_group) - Create a group *
+[get_hris_employee](docs/sdks/hris/README.md#get_hris_employee) - Retrieve an
+employee * [get_hris_group](docs/sdks/hris/README.md#get_hris_group) - Retrieve
+a group * [get_hris_payslip](docs/sdks/hris/README.md#get_hris_payslip) -
+Retrieve a payslip * [get_hris_timeoff](docs/sdks/hris/
+README.md#get_hris_timeoff) - Retrieve a timeoff * [list_hris_employees](docs/
+sdks/hris/README.md#list_hris_employees) - List all employees *
+[list_hris_groups](docs/sdks/hris/README.md#list_hris_groups) - List all groups
+* [list_hris_payslips](docs/sdks/hris/README.md#list_hris_payslips) - List all
+payslips * [list_hris_timeoffs](docs/sdks/hris/README.md#list_hris_timeoffs) -
+List all timeoffs * [patch_hris_employee](docs/sdks/hris/
+README.md#patch_hris_employee) - Update an employee * [patch_hris_group](docs/
+sdks/hris/README.md#patch_hris_group) - Update a group * [remove_hris_employee]
+(docs/sdks/hris/README.md#remove_hris_employee) - Remove an employee *
+[remove_hris_group](docs/sdks/hris/README.md#remove_hris_group) - Remove a
+group * [update_hris_employee](docs/sdks/hris/README.md#update_hris_employee) -
+Update an employee * [update_hris_group](docs/sdks/hris/
+README.md#update_hris_group) - Update a group ### [employee](docs/sdks/
+employee/README.md) * [create_hris_employee](docs/sdks/employee/
+README.md#create_hris_employee) - Create an employee * [get_hris_employee]
+(docs/sdks/employee/README.md#get_hris_employee) - Retrieve an employee *
+[list_hris_employees](docs/sdks/employee/README.md#list_hris_employees) - List
+all employees * [patch_hris_employee](docs/sdks/employee/
+README.md#patch_hris_employee) - Update an employee * [remove_hris_employee]
+(docs/sdks/employee/README.md#remove_hris_employee) - Remove an employee *
+[update_hris_employee](docs/sdks/employee/README.md#update_hris_employee) -
+Update an employee ### [group](docs/sdks/group/README.md) * [create_hris_group]
+(docs/sdks/group/README.md#create_hris_group) - Create a group *
+[get_hris_group](docs/sdks/group/README.md#get_hris_group) - Retrieve a group *
+[list_hris_groups](docs/sdks/group/README.md#list_hris_groups) - List all
+groups * [patch_hris_group](docs/sdks/group/README.md#patch_hris_group) -
+Update a group * [remove_hris_group](docs/sdks/group/
+README.md#remove_hris_group) - Remove a group * [update_hris_group](docs/sdks/
+group/README.md#update_hris_group) - Update a group ### [payslip](docs/sdks/
+payslip/README.md) * [get_hris_payslip](docs/sdks/payslip/
+README.md#get_hris_payslip) - Retrieve a payslip * [list_hris_payslips](docs/
+sdks/payslip/README.md#list_hris_payslips) - List all payslips ### [timeoff]
+(docs/sdks/timeoff/README.md) * [get_hris_timeoff](docs/sdks/timeoff/
+README.md#get_hris_timeoff) - Retrieve a timeoff * [list_hris_timeoffs](docs/
+sdks/timeoff/README.md#list_hris_timeoffs) - List all timeoffs ### [martech]
+(docs/sdks/martech/README.md) * [create_martech_list](docs/sdks/martech/
+README.md#create_martech_list) - Create a list * [create_martech_member](docs/
+sdks/martech/README.md#create_martech_member) - Create a member *
+[get_martech_list](docs/sdks/martech/README.md#get_martech_list) - Retrieve a
+list * [get_martech_member](docs/sdks/martech/README.md#get_martech_member) -
+Retrieve a member * [list_martech_lists](docs/sdks/martech/
+README.md#list_martech_lists) - List all lists * [list_martech_members](docs/
+sdks/martech/README.md#list_martech_members) - List all members *
+[patch_martech_list](docs/sdks/martech/README.md#patch_martech_list) - Update a
+list * [patch_martech_member](docs/sdks/martech/README.md#patch_martech_member)
+- Update a member * [remove_martech_list](docs/sdks/martech/
 README.md#remove_martech_list) - Remove a list * [remove_martech_member](docs/
 sdks/martech/README.md#remove_martech_member) - Remove a member *
 [update_martech_list](docs/sdks/martech/README.md#update_martech_list) - Update
 a list * [update_martech_member](docs/sdks/martech/
 README.md#update_martech_member) - Update a member ### [list](docs/sdks/list/
 README.md) * [create_martech_list](docs/sdks/list/
 README.md#create_martech_list) - Create a list * [get_martech_list](docs/sdks/
@@ -707,57 +714,58 @@
 webhook/README.md#update_unified_webhook_trigger) - Trigger webhook ## Error
 Handling Handling errors in this SDK should largely match your expectations.
 All operations return a response object or raise an error. If Error objects are
 specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 | Error Object | Status Code | Content Type | | --------------- | -------------
 -- | --------------- | | errors.SDKError | 4xx-5xx | */* | ### Example
 ```python import unified_to from unified_to.models import errors, operations,
-shared s = unified_to.UnifiedTo( security=shared.Security( jwt="", ), ) req =
-operations.CreateAccountingAccountRequest( connection_id='', ) res = None try:
-res = s.accounting.create_accounting_account(req) except errors.SDKError as e:
-# handle exception raise(e) if res.accounting_account is not None: # handle
-response pass ``` ## Server Selection ### Select Server by Index You can
-override the default server globally by passing a server index to the
-`server_idx: int` optional parameter when initializing the SDK client instance.
-The selected server will then be used as the default on the operations that use
-it. This table lists the indexes associated with the available servers: | # |
-Server | Variables | | - | ------ | --------- | | 0 | `https://api.unified.to`
-| None | | 1 | `https://api-eu.unified.to` | None | #### Example ```python
-import unified_to from unified_to.models import operations, shared s =
-unified_to.UnifiedTo( server_idx=1, security=shared.Security( jwt="", ), ) req
-= operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ### Override Server URL Per-Client The default
-server can also be overridden globally by passing a URL to the `server_url:
-str` optional parameter when initializing the SDK client instance. For example:
-```python import unified_to from unified_to.models import operations, shared s
-= unified_to.UnifiedTo( server_url="https://api.unified.to",
-security=shared.Security( jwt="", ), ) req =
-operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ## Custom HTTP Client The Python SDK makes API
-calls using the [requests](https://pypi.org/project/requests/) HTTP library. In
-order to provide a convenient way to configure timeouts, cookies, proxies,
-custom headers, and other low-level configuration, you can initialize the SDK
-client with a custom `requests.Session` object. For example, you could specify
-a header for every request that this sdk makes as follows: ```python import
-unified_to import requests http_client = requests.Session()
-http_client.headers.update({'x-custom-header': 'someValue'}) s =
-unified_to.UnifiedTo(client=http_client) ``` ## Authentication ### Per-Client
-Security Schemes This SDK supports the following security scheme globally: |
-Name | Type | Scheme | | ------- | ------- | ------- | | `jwt` | apiKey | API
-key | You can set the security parameters through the `security` optional
-parameter when initializing the SDK client instance. For example: ```python
-import unified_to from unified_to.models import operations, shared s =
-unified_to.UnifiedTo( security=shared.Security( jwt="", ), ) req =
-operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ### Maturity This SDK is in beta, and there
-may be breaking changes between versions without a major version update.
-Therefore, we recommend pinning usage to a specific package version. This way,
-you can install the same version each time without breaking changes unless you
-are intentionally looking for the latest version. ### Contributions While we
-value open-source contributions to this SDK, this library is generated
-programmatically. Feel free to open a PR or a Github issue as a proof of
-concept and we'll do our best to include it in a future release! ### SDK
-Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
-client-sdks)
+shared s = unified_to.UnifiedTo( security=shared.Security( jwt="", ), ) res =
+None try: res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) except
+errors.SDKError as e: # handle exception raise(e) if res.accounting_account is
+not None: # handle response pass ``` ## Server Selection ### Select Server by
+Index You can override the default server globally by passing a server index to
+the `server_idx: int` optional parameter when initializing the SDK client
+instance. The selected server will then be used as the default on the
+operations that use it. This table lists the indexes associated with the
+available servers: | # | Server | Variables | | - | ------ | --------- | | 0 |
+`https://api.unified.to` | None | | 1 | `https://api-eu.unified.to` | None |
+#### Example ```python import unified_to from unified_to.models import
+operations, shared s = unified_to.UnifiedTo( server_idx=1,
+security=shared.Security( jwt="", ), ) res =
+s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ### Override
+Server URL Per-Client The default server can also be overridden globally by
+passing a URL to the `server_url: str` optional parameter when initializing the
+SDK client instance. For example: ```python import unified_to from
+unified_to.models import operations, shared s = unified_to.UnifiedTo
+( server_url="https://api.unified.to", security=shared.Security( jwt="", ), )
+res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ## Custom HTTP
+Client The Python SDK makes API calls using the [requests](https://pypi.org/
+project/requests/) HTTP library. In order to provide a convenient way to
+configure timeouts, cookies, proxies, custom headers, and other low-level
+configuration, you can initialize the SDK client with a custom
+`requests.Session` object. For example, you could specify a header for every
+request that this sdk makes as follows: ```python import unified_to import
+requests http_client = requests.Session() http_client.headers.update({'x-
+custom-header': 'someValue'}) s = unified_to.UnifiedTo(client=http_client) ```
+## Authentication ### Per-Client Security Schemes This SDK supports the
+following security scheme globally: | Name | Type | Scheme | | ------- | ------
+- | ------- | | `jwt` | apiKey | API key | You can set the security parameters
+through the `security` optional parameter when initializing the SDK client
+instance. For example: ```python import unified_to from unified_to.models
+import operations, shared s = unified_to.UnifiedTo( security=shared.Security
+( jwt="", ), ) res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ### Maturity
+This SDK is in beta, and there may be breaking changes between versions without
+a major version update. Therefore, we recommend pinning usage to a specific
+package version. This way, you can install the same version each time without
+breaking changes unless you are intentionally looking for the latest version.
+### Contributions While we value open-source contributions to this SDK, this
+library is generated programmatically. Feel free to open a PR or a Github issue
+as a proof of concept and we'll do our best to include it in a future release!
+### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-
+speakeasy/client-sdks)
```

### Comparing `Unified-python-sdk-0.21.9/setup.py` & `Unified-python-sdk-0.22.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='Unified-python-sdk',
-    version='0.21.9',
+    version='0.22.0',
     author='Unified API Inc',
     description='Python Client SDK for Unified.to',
     url='https://github.com/unified-to/unified-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `Unified-python-sdk-0.21.9/src/Unified_python_sdk.egg-info/PKG-INFO` & `Unified-python-sdk-0.22.0/src/Unified_python_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Unified-python-sdk
-Version: 0.21.9
+Version: 0.22.0
 Summary: Python Client SDK for Unified.to
 Home-page: https://github.com/unified-to/unified-python-sdk.git
 Author: Unified API Inc
 License: UNKNOWN
 Description: <div align="left">
             <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
             <a href="https://github.com/unified-to/unified-python-sdk/actions"><img src="https://img.shields.io/github/actions/workflow/status/unified-to/unified-python-sdk/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
@@ -30,19 +30,17 @@
         
         s = unified_to.UnifiedTo(
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
+        res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
             connection_id='<value>',
-        )
-        
-        res = s.accounting.create_accounting_account(req)
+        ))
         
         if res.accounting_account is not None:
             # handle response
             pass
         
         ```
         <!-- End SDK Example Usage [usage] -->
@@ -417,14 +415,27 @@
         * [list_enrich_companies](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/enrich/README.md#list_enrich_companies) - Retrieve enrichment information for a company
         * [list_enrich_people](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/enrich/README.md#list_enrich_people) - Retrieve enrichment information for a person
         
         ### [person](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/person/README.md)
         
         * [list_enrich_people](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/person/README.md#list_enrich_people) - Retrieve enrichment information for a person
         
+        ### [genai](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/README.md)
+        
+        * [create_genai_prompt](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/README.md#create_genai_prompt) - Create a prompt
+        * [list_genai_models](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/README.md#list_genai_models) - List all models
+        
+        ### [model](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/model/README.md)
+        
+        * [list_genai_models](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/model/README.md#list_genai_models) - List all models
+        
+        ### [prompt](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/prompt/README.md)
+        
+        * [create_genai_prompt](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/prompt/README.md#create_genai_prompt) - Create a prompt
+        
         ### [hris](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md)
         
         * [create_hris_employee](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#create_hris_employee) - Create an employee
         * [create_hris_group](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#create_hris_group) - Create a group
         * [get_hris_employee](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#get_hris_employee) - Retrieve an employee
         * [get_hris_group](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#get_hris_group) - Retrieve a group
         * [get_hris_payslip](https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/README.md#get_hris_payslip) - Retrieve a payslip
@@ -716,21 +727,19 @@
         
         s = unified_to.UnifiedTo(
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
-            connection_id='<value>',
-        )
-        
         res = None
         try:
-            res = s.accounting.create_accounting_account(req)
+            res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
+            connection_id='<value>',
+        ))
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
         if res.accounting_account is not None:
             # handle response
             pass
@@ -761,19 +770,17 @@
         s = unified_to.UnifiedTo(
             server_idx=1,
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
+        res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
             connection_id='<value>',
-        )
-        
-        res = s.accounting.create_accounting_account(req)
+        ))
         
         if res.accounting_account is not None:
             # handle response
             pass
         
         ```
         
@@ -788,19 +795,17 @@
         s = unified_to.UnifiedTo(
             server_url="https://api.unified.to",
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
+        res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
             connection_id='<value>',
-        )
-        
-        res = s.accounting.create_accounting_account(req)
+        ))
         
         if res.accounting_account is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -843,19 +848,17 @@
         
         s = unified_to.UnifiedTo(
             security=shared.Security(
                 jwt="<YOUR_API_KEY_HERE>",
             ),
         )
         
-        req = operations.CreateAccountingAccountRequest(
+        res = s.accounting.create_accounting_account(request=operations.CreateAccountingAccountRequest(
             connection_id='<value>',
-        )
-        
-        res = s.accounting.create_accounting_account(req)
+        ))
         
         if res.accounting_account is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
```

#### html2text {}

```diff
@@ -1,129 +1,129 @@
-Metadata-Version: 2.1 Name: Unified-python-sdk Version: 0.21.9 Summary: Python
+Metadata-Version: 2.1 Name: Unified-python-sdk Version: 0.22.0 Summary: Python
 Client SDK for Unified.to Home-page: https://github.com/unified-to/unified-
 python-sdk.git Author: Unified API Inc License: UNKNOWN Description:
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_u_n_i_f_i_e_d_-_t_o_/_u_n_i_f_i_e_d_-
 _p_y_t_h_o_n_-_s_d_k_/_s_p_e_a_k_e_a_s_y___s_d_k___g_e_n_e_r_a_t_i_o_n_._y_m_l_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 ## SDK Installation ```bash pip install Unified-python-sdk ``` ## SDK Example
 Usage ### Example ```python import unified_to from unified_to.models import
 operations, shared s = unified_to.UnifiedTo( security=shared.Security( jwt="",
-), ) req = operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ## Available Resources and Operations ###
-[accounting](https://github.com/unified-to/unified-python-sdk/blob/master/docs/
-sdks/accounting/README.md) * [create_accounting_account](https://github.com/
-unified-to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#create_accounting_account) - Create an account *
-[create_accounting_contact](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#create_accounting_contact) - Create
-a contact * [create_accounting_invoice](https://github.com/unified-to/unified-
+), ) res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ## Available
+Resources and Operations ### [accounting](https://github.com/unified-to/
+unified-python-sdk/blob/master/docs/sdks/accounting/README.md) *
+[create_accounting_account](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#create_accounting_account) - Create
+an account * [create_accounting_contact](https://github.com/unified-to/unified-
 python-sdk/blob/master/docs/sdks/accounting/
-README.md#create_accounting_invoice) - Create an invoice *
-[create_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#create_accounting_taxrate) - Create
-a taxrate * [create_accounting_transaction](https://github.com/unified-to/
+README.md#create_accounting_contact) - Create a contact *
+[create_accounting_invoice](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#create_accounting_invoice) - Create
+an invoice * [create_accounting_taxrate](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/
+README.md#create_accounting_taxrate) - Create a taxrate *
+[create_accounting_transaction](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#create_accounting_transaction) -
+Create a transaction * [get_accounting_account](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#create_accounting_transaction) - Create a transaction *
-[get_accounting_account](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/accounting/README.md#get_accounting_account) - Retrieve an
-account * [get_accounting_contact](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/README.md#get_accounting_contact) -
-Retrieve a contact * [get_accounting_invoice](https://github.com/unified-to/
+README.md#get_accounting_account) - Retrieve an account *
+[get_accounting_contact](https://github.com/unified-to/unified-python-sdk/blob/
+master/docs/sdks/accounting/README.md#get_accounting_contact) - Retrieve a
+contact * [get_accounting_invoice](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/README.md#get_accounting_invoice) -
+Retrieve an invoice * [get_accounting_organization](https://github.com/unified-
+to/unified-python-sdk/blob/master/docs/sdks/accounting/
+README.md#get_accounting_organization) - Retrieve an organization *
+[get_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/blob/
+master/docs/sdks/accounting/README.md#get_accounting_taxrate) - Retrieve a
+taxrate * [get_accounting_transaction](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/
+README.md#get_accounting_transaction) - Retrieve a transaction *
+[list_accounting_accounts](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#list_accounting_accounts) - List all
+accounts * [list_accounting_contacts](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/README.md#list_accounting_contacts)
+- List all contacts * [list_accounting_invoices](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#get_accounting_invoice) - Retrieve an invoice *
-[get_accounting_organization](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#get_accounting_organization) -
-Retrieve an organization * [get_accounting_taxrate](https://github.com/unified-
+README.md#list_accounting_invoices) - List all invoices *
+[list_accounting_organizations](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#list_accounting_organizations) -
+List all organizations * [list_accounting_taxrates](https://github.com/unified-
 to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#get_accounting_taxrate) - Retrieve a taxrate *
-[get_accounting_transaction](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#get_accounting_transaction) -
-Retrieve a transaction * [list_accounting_accounts](https://github.com/unified-
+README.md#list_accounting_taxrates) - List all taxrates *
+[list_accounting_transactions](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#list_accounting_transactions) -
+List all transactions * [patch_accounting_account](https://github.com/unified-
 to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#list_accounting_accounts) - List all accounts *
-[list_accounting_contacts](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#list_accounting_contacts) - List all
-contacts * [list_accounting_invoices](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/README.md#list_accounting_invoices)
-- List all invoices * [list_accounting_organizations](https://github.com/
-unified-to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#list_accounting_organizations) - List all organizations *
-[list_accounting_taxrates](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#list_accounting_taxrates) - List all
-taxrates * [list_accounting_transactions](https://github.com/unified-to/
-unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#list_accounting_transactions) - List all transactions *
-[patch_accounting_account](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#patch_accounting_account) - Update
-an account * [patch_accounting_contact](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/README.md#patch_accounting_contact)
-- Update a contact * [patch_accounting_invoice](https://github.com/unified-to/
+README.md#patch_accounting_account) - Update an account *
+[patch_accounting_contact](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#patch_accounting_contact) - Update a
+contact * [patch_accounting_invoice](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/README.md#patch_accounting_invoice)
+- Update an invoice * [patch_accounting_taxrate](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#patch_accounting_invoice) - Update an invoice *
-[patch_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#patch_accounting_taxrate) - Update a
-taxrate * [patch_accounting_transaction](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/
-README.md#patch_accounting_transaction) - Update a transaction *
-[remove_accounting_account](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#remove_accounting_account) - Remove
-an account * [remove_accounting_contact](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/
-README.md#remove_accounting_contact) - Remove a contact *
-[remove_accounting_invoice](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#remove_accounting_invoice) - Remove
-an invoice * [remove_accounting_taxrate](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/accounting/
-README.md#remove_accounting_taxrate) - Remove a taxrate *
-[remove_accounting_transaction](https://github.com/unified-to/unified-python-
-sdk/blob/master/docs/sdks/accounting/README.md#remove_accounting_transaction) -
-Remove a transaction * [update_accounting_account](https://github.com/unified-
+README.md#patch_accounting_taxrate) - Update a taxrate *
+[patch_accounting_transaction](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#patch_accounting_transaction) -
+Update a transaction * [remove_accounting_account](https://github.com/unified-
 to/unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#update_accounting_account) - Update an account *
-[update_accounting_contact](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#update_accounting_contact) - Update
-a contact * [update_accounting_invoice](https://github.com/unified-to/unified-
+README.md#remove_accounting_account) - Remove an account *
+[remove_accounting_contact](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#remove_accounting_contact) - Remove
+a contact * [remove_accounting_invoice](https://github.com/unified-to/unified-
 python-sdk/blob/master/docs/sdks/accounting/
-README.md#update_accounting_invoice) - Update an invoice *
-[update_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/accounting/README.md#update_accounting_taxrate) - Update
-a taxrate * [update_accounting_transaction](https://github.com/unified-to/
+README.md#remove_accounting_invoice) - Remove an invoice *
+[remove_accounting_taxrate](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#remove_accounting_taxrate) - Remove
+a taxrate * [remove_accounting_transaction](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/accounting/
-README.md#update_accounting_transaction) - Update a transaction ### [account]
-(https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/
-account/README.md) * [create_accounting_account](https://github.com/unified-to/
+README.md#remove_accounting_transaction) - Remove a transaction *
+[update_accounting_account](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#update_accounting_account) - Update
+an account * [update_accounting_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/
+README.md#update_accounting_contact) - Update a contact *
+[update_accounting_invoice](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/accounting/README.md#update_accounting_invoice) - Update
+an invoice * [update_accounting_taxrate](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/accounting/
+README.md#update_accounting_taxrate) - Update a taxrate *
+[update_accounting_transaction](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/accounting/README.md#update_accounting_transaction) -
+Update a transaction ### [account](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/account/README.md) *
+[create_accounting_account](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/account/README.md#create_accounting_account) - Create an
+account * [get_accounting_account](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/account/README.md#get_accounting_account) -
+Retrieve an account * [list_accounting_accounts](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/account/
-README.md#create_accounting_account) - Create an account *
-[get_accounting_account](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/account/README.md#get_accounting_account) - Retrieve an
-account * [list_accounting_accounts](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/account/README.md#list_accounting_accounts) -
-List all accounts * [patch_accounting_account](https://github.com/unified-to/
+README.md#list_accounting_accounts) - List all accounts *
+[patch_accounting_account](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/account/README.md#patch_accounting_account) - Update an
+account * [remove_accounting_account](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/account/README.md#remove_accounting_account) -
+Remove an account * [update_accounting_account](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/account/
-README.md#patch_accounting_account) - Update an account *
-[remove_accounting_account](https://github.com/unified-to/unified-python-sdk/
-blob/master/docs/sdks/account/README.md#remove_accounting_account) - Remove an
-account * [update_accounting_account](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/account/README.md#update_accounting_account) -
-Update an account ### [contact](https://github.com/unified-to/unified-python-
-sdk/blob/master/docs/sdks/contact/README.md) * [create_accounting_contact]
-(https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/
-contact/README.md#create_accounting_contact) - Create a contact *
-[create_crm_contact](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/contact/README.md#create_crm_contact) - Create a contact *
-[create_uc_contact](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/contact/README.md#create_uc_contact) - Create a contact *
-[get_accounting_contact](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/contact/README.md#get_accounting_contact) - Retrieve a contact
-* [get_crm_contact](https://github.com/unified-to/unified-python-sdk/blob/
-master/docs/sdks/contact/README.md#get_crm_contact) - Retrieve a contact *
-[get_uc_contact](https://github.com/unified-to/unified-python-sdk/blob/master/
-docs/sdks/contact/README.md#get_uc_contact) - Retrieve a contact *
+README.md#update_accounting_account) - Update an account ### [contact](https://
+github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/contact/
+README.md) * [create_accounting_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/contact/README.md#create_accounting_contact) -
+Create a contact * [create_crm_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/contact/README.md#create_crm_contact) - Create
+a contact * [create_uc_contact](https://github.com/unified-to/unified-python-
+sdk/blob/master/docs/sdks/contact/README.md#create_uc_contact) - Create a
+contact * [get_accounting_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/contact/README.md#get_accounting_contact) -
+Retrieve a contact * [get_crm_contact](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/contact/README.md#get_crm_contact) - Retrieve
+a contact * [get_uc_contact](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/contact/README.md#get_uc_contact) - Retrieve a contact *
 [list_accounting_contacts](https://github.com/unified-to/unified-python-sdk/
 blob/master/docs/sdks/contact/README.md#list_accounting_contacts) - List all
 contacts * [list_crm_contacts](https://github.com/unified-to/unified-python-
 sdk/blob/master/docs/sdks/contact/README.md#list_crm_contacts) - List all
 contacts * [list_uc_contacts](https://github.com/unified-to/unified-python-sdk/
 blob/master/docs/sdks/contact/README.md#list_uc_contacts) - List all contacts *
 [patch_accounting_contact](https://github.com/unified-to/unified-python-sdk/
@@ -659,17 +659,29 @@
 README.md#list_enrich_companies) - Retrieve enrichment information for a
 company * [list_enrich_people](https://github.com/unified-to/unified-python-
 sdk/blob/master/docs/sdks/enrich/README.md#list_enrich_people) - Retrieve
 enrichment information for a person ### [person](https://github.com/unified-to/
 unified-python-sdk/blob/master/docs/sdks/person/README.md) *
 [list_enrich_people](https://github.com/unified-to/unified-python-sdk/blob/
 master/docs/sdks/person/README.md#list_enrich_people) - Retrieve enrichment
-information for a person ### [hris](https://github.com/unified-to/unified-
-python-sdk/blob/master/docs/sdks/hris/README.md) * [create_hris_employee]
-(https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
+information for a person ### [genai](https://github.com/unified-to/unified-
+python-sdk/blob/master/docs/sdks/genai/README.md) * [create_genai_prompt]
+(https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/
+README.md#create_genai_prompt) - Create a prompt * [list_genai_models](https://
+github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/genai/
+README.md#list_genai_models) - List all models ### [model](https://github.com/
+unified-to/unified-python-sdk/blob/master/docs/sdks/model/README.md) *
+[list_genai_models](https://github.com/unified-to/unified-python-sdk/blob/
+master/docs/sdks/model/README.md#list_genai_models) - List all models ###
+[prompt](https://github.com/unified-to/unified-python-sdk/blob/master/docs/
+sdks/prompt/README.md) * [create_genai_prompt](https://github.com/unified-to/
+unified-python-sdk/blob/master/docs/sdks/prompt/README.md#create_genai_prompt)
+- Create a prompt ### [hris](https://github.com/unified-to/unified-python-sdk/
+blob/master/docs/sdks/hris/README.md) * [create_hris_employee](https://
+github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
 README.md#create_hris_employee) - Create an employee * [create_hris_group]
 (https://github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
 README.md#create_hris_group) - Create a group * [get_hris_employee](https://
 github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
 README.md#get_hris_employee) - Retrieve an employee * [get_hris_group](https://
 github.com/unified-to/unified-python-sdk/blob/master/docs/sdks/hris/
 README.md#get_hris_group) - Retrieve a group * [get_hris_payslip](https://
@@ -1097,58 +1109,59 @@
 README.md#update_unified_webhook_trigger) - Trigger webhook ## Error Handling
 Handling errors in this SDK should largely match your expectations. All
 operations return a response object or raise an error. If Error objects are
 specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 | Error Object | Status Code | Content Type | | --------------- | -------------
 -- | --------------- | | errors.SDKError | 4xx-5xx | */* | ### Example
 ```python import unified_to from unified_to.models import errors, operations,
-shared s = unified_to.UnifiedTo( security=shared.Security( jwt="", ), ) req =
-operations.CreateAccountingAccountRequest( connection_id='', ) res = None try:
-res = s.accounting.create_accounting_account(req) except errors.SDKError as e:
-# handle exception raise(e) if res.accounting_account is not None: # handle
-response pass ``` ## Server Selection ### Select Server by Index You can
-override the default server globally by passing a server index to the
-`server_idx: int` optional parameter when initializing the SDK client instance.
-The selected server will then be used as the default on the operations that use
-it. This table lists the indexes associated with the available servers: | # |
-Server | Variables | | - | ------ | --------- | | 0 | `https://api.unified.to`
-| None | | 1 | `https://api-eu.unified.to` | None | #### Example ```python
-import unified_to from unified_to.models import operations, shared s =
-unified_to.UnifiedTo( server_idx=1, security=shared.Security( jwt="", ), ) req
-= operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ### Override Server URL Per-Client The default
-server can also be overridden globally by passing a URL to the `server_url:
-str` optional parameter when initializing the SDK client instance. For example:
-```python import unified_to from unified_to.models import operations, shared s
-= unified_to.UnifiedTo( server_url="https://api.unified.to",
-security=shared.Security( jwt="", ), ) req =
-operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ## Custom HTTP Client The Python SDK makes API
-calls using the [requests](https://pypi.org/project/requests/) HTTP library. In
-order to provide a convenient way to configure timeouts, cookies, proxies,
-custom headers, and other low-level configuration, you can initialize the SDK
-client with a custom `requests.Session` object. For example, you could specify
-a header for every request that this sdk makes as follows: ```python import
-unified_to import requests http_client = requests.Session()
-http_client.headers.update({'x-custom-header': 'someValue'}) s =
-unified_to.UnifiedTo(client=http_client) ``` ## Authentication ### Per-Client
-Security Schemes This SDK supports the following security scheme globally: |
-Name | Type | Scheme | | ------- | ------- | ------- | | `jwt` | apiKey | API
-key | You can set the security parameters through the `security` optional
-parameter when initializing the SDK client instance. For example: ```python
-import unified_to from unified_to.models import operations, shared s =
-unified_to.UnifiedTo( security=shared.Security( jwt="", ), ) req =
-operations.CreateAccountingAccountRequest( connection_id='', ) res =
-s.accounting.create_accounting_account(req) if res.accounting_account is not
-None: # handle response pass ``` ### Maturity This SDK is in beta, and there
-may be breaking changes between versions without a major version update.
-Therefore, we recommend pinning usage to a specific package version. This way,
-you can install the same version each time without breaking changes unless you
-are intentionally looking for the latest version. ### Contributions While we
-value open-source contributions to this SDK, this library is generated
-programmatically. Feel free to open a PR or a Github issue as a proof of
-concept and we'll do our best to include it in a future release! ### SDK
-Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
-client-sdks) Platform: UNKNOWN Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: dev
+shared s = unified_to.UnifiedTo( security=shared.Security( jwt="", ), ) res =
+None try: res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) except
+errors.SDKError as e: # handle exception raise(e) if res.accounting_account is
+not None: # handle response pass ``` ## Server Selection ### Select Server by
+Index You can override the default server globally by passing a server index to
+the `server_idx: int` optional parameter when initializing the SDK client
+instance. The selected server will then be used as the default on the
+operations that use it. This table lists the indexes associated with the
+available servers: | # | Server | Variables | | - | ------ | --------- | | 0 |
+`https://api.unified.to` | None | | 1 | `https://api-eu.unified.to` | None |
+#### Example ```python import unified_to from unified_to.models import
+operations, shared s = unified_to.UnifiedTo( server_idx=1,
+security=shared.Security( jwt="", ), ) res =
+s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ### Override
+Server URL Per-Client The default server can also be overridden globally by
+passing a URL to the `server_url: str` optional parameter when initializing the
+SDK client instance. For example: ```python import unified_to from
+unified_to.models import operations, shared s = unified_to.UnifiedTo
+( server_url="https://api.unified.to", security=shared.Security( jwt="", ), )
+res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ## Custom HTTP
+Client The Python SDK makes API calls using the [requests](https://pypi.org/
+project/requests/) HTTP library. In order to provide a convenient way to
+configure timeouts, cookies, proxies, custom headers, and other low-level
+configuration, you can initialize the SDK client with a custom
+`requests.Session` object. For example, you could specify a header for every
+request that this sdk makes as follows: ```python import unified_to import
+requests http_client = requests.Session() http_client.headers.update({'x-
+custom-header': 'someValue'}) s = unified_to.UnifiedTo(client=http_client) ```
+## Authentication ### Per-Client Security Schemes This SDK supports the
+following security scheme globally: | Name | Type | Scheme | | ------- | ------
+- | ------- | | `jwt` | apiKey | API key | You can set the security parameters
+through the `security` optional parameter when initializing the SDK client
+instance. For example: ```python import unified_to from unified_to.models
+import operations, shared s = unified_to.UnifiedTo( security=shared.Security
+( jwt="", ), ) res = s.accounting.create_accounting_account
+(request=operations.CreateAccountingAccountRequest( connection_id='', )) if
+res.accounting_account is not None: # handle response pass ``` ### Maturity
+This SDK is in beta, and there may be breaking changes between versions without
+a major version update. Therefore, we recommend pinning usage to a specific
+package version. This way, you can install the same version each time without
+breaking changes unless you are intentionally looking for the latest version.
+### Contributions While we value open-source contributions to this SDK, this
+library is generated programmatically. Feel free to open a PR or a Github issue
+as a proof of concept and we'll do our best to include it in a future release!
+### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-
+speakeasy/client-sdks) Platform: UNKNOWN Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: dev
```

### Comparing `Unified-python-sdk-0.21.9/src/Unified_python_sdk.egg-info/SOURCES.txt` & `Unified-python-sdk-0.22.0/src/Unified_python_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/unified_to/customer.py
 src/unified_to/deal.py
 src/unified_to/document.py
 src/unified_to/employee.py
 src/unified_to/enrich.py
 src/unified_to/event.py
 src/unified_to/file.py
+src/unified_to/genai.py
 src/unified_to/group.py
 src/unified_to/hris.py
 src/unified_to/integration.py
 src/unified_to/interview.py
 src/unified_to/inventory.py
 src/unified_to/invoice.py
 src/unified_to/issue.py
@@ -42,22 +43,24 @@
 src/unified_to/lead.py
 src/unified_to/link.py
 src/unified_to/list.py
 src/unified_to/location.py
 src/unified_to/login.py
 src/unified_to/martech.py
 src/unified_to/member.py
+src/unified_to/model.py
 src/unified_to/note.py
 src/unified_to/organization.py
 src/unified_to/passthrough.py
 src/unified_to/payment.py
 src/unified_to/payout.py
 src/unified_to/payslip.py
 src/unified_to/person.py
 src/unified_to/pipeline.py
+src/unified_to/prompt.py
 src/unified_to/refund.py
 src/unified_to/scorecard.py
 src/unified_to/sdk.py
 src/unified_to/sdkconfiguration.py
 src/unified_to/storage.py
 src/unified_to/taxrate.py
 src/unified_to/ticket.py
@@ -92,14 +95,15 @@
 src/unified_to/models/operations/createcommercelocation.py
 src/unified_to/models/operations/createcrmcompany.py
 src/unified_to/models/operations/createcrmcontact.py
 src/unified_to/models/operations/createcrmdeal.py
 src/unified_to/models/operations/createcrmevent.py
 src/unified_to/models/operations/createcrmlead.py
 src/unified_to/models/operations/createcrmpipeline.py
+src/unified_to/models/operations/creategenaiprompt.py
 src/unified_to/models/operations/createhrisemployee.py
 src/unified_to/models/operations/createhrisgroup.py
 src/unified_to/models/operations/createmartechlist.py
 src/unified_to/models/operations/createmartechmember.py
 src/unified_to/models/operations/createpassthrough.py
 src/unified_to/models/operations/createpaymentlink.py
 src/unified_to/models/operations/createpaymentpayment.py
@@ -177,14 +181,15 @@
 src/unified_to/models/operations/listcrmcontacts.py
 src/unified_to/models/operations/listcrmdeals.py
 src/unified_to/models/operations/listcrmevents.py
 src/unified_to/models/operations/listcrmleads.py
 src/unified_to/models/operations/listcrmpipelines.py
 src/unified_to/models/operations/listenrichcompanies.py
 src/unified_to/models/operations/listenrichpeople.py
+src/unified_to/models/operations/listgenaimodels.py
 src/unified_to/models/operations/listhrisemployees.py
 src/unified_to/models/operations/listhrisgroups.py
 src/unified_to/models/operations/listhrispayslips.py
 src/unified_to/models/operations/listhristimeoffs.py
 src/unified_to/models/operations/listmartechlists.py
 src/unified_to/models/operations/listmartechmembers.py
 src/unified_to/models/operations/listpassthroughs.py
@@ -360,14 +365,17 @@
 src/unified_to/models/shared/crmpipeline.py
 src/unified_to/models/shared/crmtelephone.py
 src/unified_to/models/shared/enrichcompany.py
 src/unified_to/models/shared/enrichemail.py
 src/unified_to/models/shared/enrichperson.py
 src/unified_to/models/shared/enrichpersonworkhistory.py
 src/unified_to/models/shared/enrichtelephone.py
+src/unified_to/models/shared/genaicontent.py
+src/unified_to/models/shared/genaimodel.py
+src/unified_to/models/shared/genaiprompt.py
 src/unified_to/models/shared/hrisemail.py
 src/unified_to/models/shared/hrisemployee.py
 src/unified_to/models/shared/hrisgroup.py
 src/unified_to/models/shared/hrispayslip.py
 src/unified_to/models/shared/hrispayslipdetail.py
 src/unified_to/models/shared/hristelephone.py
 src/unified_to/models/shared/hristimeoff.py
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/_hooks/sdkhooks.py` & `Unified-python-sdk-0.22.0/src/unified_to/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/_hooks/types.py` & `Unified-python-sdk-0.22.0/src/unified_to/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/account.py` & `Unified-python-sdk-0.22.0/src/unified_to/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingAccount])
                 res.accounting_account = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingAccount])
                 res.accounting_account = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingAccountsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingAccount]])
                 res.accounting_accounts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingAccount])
                 res.accounting_account = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingAccount])
                 res.accounting_account = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/accounting.py` & `Unified-python-sdk-0.22.0/src/unified_to/accounting.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingAccount])
                 res.accounting_account = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,14 +111,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingContact])
                 res.accounting_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -167,14 +169,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingInvoice])
                 res.accounting_invoice = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -224,14 +227,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTaxrate])
                 res.accounting_taxrate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -281,14 +285,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTransaction])
                 res.accounting_transaction = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -336,14 +341,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingAccount])
                 res.accounting_account = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -391,14 +397,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingContact])
                 res.accounting_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -446,14 +453,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingInvoice])
                 res.accounting_invoice = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -501,14 +509,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingOrganizationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingOrganization])
                 res.accounting_organization = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -556,14 +565,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTaxrate])
                 res.accounting_taxrate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -611,14 +621,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTransaction])
                 res.accounting_transaction = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -666,14 +677,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingAccountsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingAccount]])
                 res.accounting_accounts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -721,14 +733,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingContactsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingContact]])
                 res.accounting_contacts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -776,14 +789,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingInvoicesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingInvoice]])
                 res.accounting_invoices = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -831,14 +845,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingOrganizationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingOrganization]])
                 res.accounting_organizations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -886,14 +901,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingTaxratesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingTaxrate]])
                 res.accounting_taxrates = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -941,14 +957,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingTransaction]])
                 res.accounting_transactions = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -998,14 +1015,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingAccount])
                 res.accounting_account = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1055,14 +1073,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingContact])
                 res.accounting_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1112,14 +1131,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingInvoice])
                 res.accounting_invoice = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1169,14 +1189,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTaxrate])
                 res.accounting_taxrate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1226,14 +1247,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTransaction])
                 res.accounting_transaction = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1284,14 +1306,15 @@
         res = operations.RemoveAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1338,14 +1361,15 @@
         res = operations.RemoveAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1392,14 +1416,15 @@
         res = operations.RemoveAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1446,14 +1471,15 @@
         res = operations.RemoveAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1500,14 +1526,15 @@
         res = operations.RemoveAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1553,14 +1580,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingAccount])
                 res.accounting_account = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1610,14 +1638,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingContact])
                 res.accounting_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1667,14 +1696,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingInvoice])
                 res.accounting_invoice = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1724,14 +1754,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTaxrate])
                 res.accounting_taxrate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1781,14 +1812,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTransaction])
                 res.accounting_transaction = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/activity.py` & `Unified-python-sdk-0.22.0/src/unified_to/activity.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsActivity])
                 res.ats_activity = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsActivity])
                 res.ats_activity = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsActivitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsActivity]])
                 res.ats_activities = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsActivity])
                 res.ats_activity = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsActivity])
                 res.ats_activity = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/apicall.py` & `Unified-python-sdk-0.22.0/src/unified_to/apicall.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedApicallResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.APICall])
                 res.api_call = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -105,14 +106,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedApicallsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.APICall]])
                 res.api_calls = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/application.py` & `Unified-python-sdk-0.22.0/src/unified_to/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsApplication])
                 res.ats_application = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsApplication])
                 res.ats_application = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsApplicationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsApplication]])
                 res.ats_applications = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsApplication])
                 res.ats_application = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsApplication])
                 res.ats_application = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/applicationstatus.py` & `Unified-python-sdk-0.22.0/src/unified_to/applicationstatus.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsApplicationstatusesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsStatus]])
                 res.ats_statuses = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/ats.py` & `Unified-python-sdk-0.22.0/src/unified_to/ats.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsActivity])
                 res.ats_activity = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,14 +111,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsApplication])
                 res.ats_application = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -167,14 +169,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCandidate])
                 res.ats_candidate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -224,14 +227,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsDocument])
                 res.ats_document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -281,14 +285,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsInterview])
                 res.ats_interview = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -338,14 +343,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
                 res.ats_job = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -395,14 +401,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsScorecard])
                 res.ats_scorecard = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -450,14 +457,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsActivity])
                 res.ats_activity = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -505,14 +513,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsApplication])
                 res.ats_application = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -560,14 +569,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCandidate])
                 res.ats_candidate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -615,14 +625,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCompany])
                 res.ats_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -670,14 +681,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsDocument])
                 res.ats_document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -725,14 +737,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsInterview])
                 res.ats_interview = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -780,14 +793,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
                 res.ats_job = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -835,14 +849,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsScorecard])
                 res.ats_scorecard = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -890,14 +905,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsActivitiesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsActivity]])
                 res.ats_activities = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -945,14 +961,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsApplicationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsApplication]])
                 res.ats_applications = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1000,14 +1017,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsApplicationstatusesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsStatus]])
                 res.ats_statuses = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1055,14 +1073,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsCandidatesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsCandidate]])
                 res.ats_candidates = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1110,14 +1129,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsCompaniesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsCompany]])
                 res.ats_companies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1165,14 +1185,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsDocumentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsDocument]])
                 res.ats_documents = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1220,14 +1241,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsInterviewsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsInterview]])
                 res.ats_interviews = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1275,14 +1297,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsJobsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsJob]])
                 res.ats_jobs = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1330,14 +1353,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsScorecardsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsScorecard]])
                 res.ats_scorecards = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1387,14 +1411,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsActivity])
                 res.ats_activity = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1444,14 +1469,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsApplication])
                 res.ats_application = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1501,14 +1527,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCandidate])
                 res.ats_candidate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1558,14 +1585,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsDocument])
                 res.ats_document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1615,14 +1643,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsInterview])
                 res.ats_interview = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1672,14 +1701,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
                 res.ats_job = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1729,14 +1759,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsScorecard])
                 res.ats_scorecard = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1787,14 +1818,15 @@
         res = operations.RemoveAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1841,14 +1873,15 @@
         res = operations.RemoveAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1895,14 +1928,15 @@
         res = operations.RemoveAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1949,14 +1983,15 @@
         res = operations.RemoveAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2003,14 +2038,15 @@
         res = operations.RemoveAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2057,14 +2093,15 @@
         res = operations.RemoveAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2111,14 +2148,15 @@
         res = operations.RemoveAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2164,14 +2202,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsActivityResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsActivity])
                 res.ats_activity = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -2221,14 +2260,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsApplicationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsApplication])
                 res.ats_application = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -2278,14 +2318,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCandidate])
                 res.ats_candidate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -2335,14 +2376,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsDocument])
                 res.ats_document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -2392,14 +2434,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsInterview])
                 res.ats_interview = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -2449,14 +2492,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
                 res.ats_job = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -2506,14 +2550,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsScorecard])
                 res.ats_scorecard = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/auth.py` & `Unified-python-sdk-0.22.0/src/unified_to/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedIntegrationAuthResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'text/plain'):                
                 res.res = http_res.text
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedIntegrationLoginResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'text/plain'):                
                 res.res = http_res.text
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/call.py` & `Unified-python-sdk-0.22.0/src/unified_to/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUcCallsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.UcCall]])
                 res.uc_calls = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/candidate.py` & `Unified-python-sdk-0.22.0/src/unified_to/candidate.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCandidate])
                 res.ats_candidate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCandidate])
                 res.ats_candidate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsCandidatesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsCandidate]])
                 res.ats_candidates = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCandidate])
                 res.ats_candidate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsCandidateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCandidate])
                 res.ats_candidate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/collection.py` & `Unified-python-sdk-0.22.0/src/unified_to/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceCollection])
                 res.commerce_collection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceCollection])
                 res.commerce_collection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCommerceCollectionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CommerceCollection]])
                 res.commerce_collections = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceCollection])
                 res.commerce_collection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceCollection])
                 res.commerce_collection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/commerce.py` & `Unified-python-sdk-0.22.0/src/unified_to/commerce.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceCollection])
                 res.commerce_collection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,14 +111,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceInventory])
                 res.commerce_inventory = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -167,14 +169,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceItem])
                 res.commerce_item = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -224,14 +227,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceLocation])
                 res.commerce_location = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -279,14 +283,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceCollection])
                 res.commerce_collection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -334,14 +339,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceInventory])
                 res.commerce_inventory = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -389,14 +395,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceItem])
                 res.commerce_item = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -444,14 +451,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceLocation])
                 res.commerce_location = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -499,14 +507,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCommerceCollectionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CommerceCollection]])
                 res.commerce_collections = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -554,14 +563,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCommerceInventoriesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CommerceInventory]])
                 res.commerce_inventories = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -609,14 +619,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCommerceItemsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CommerceItem]])
                 res.commerce_items = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -664,14 +675,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCommerceLocationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CommerceLocation]])
                 res.commerce_locations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -721,14 +733,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceCollection])
                 res.commerce_collection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -778,14 +791,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceInventory])
                 res.commerce_inventory = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -835,14 +849,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceItem])
                 res.commerce_item = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -892,14 +907,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceLocation])
                 res.commerce_location = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -950,14 +966,15 @@
         res = operations.RemoveCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1004,14 +1021,15 @@
         res = operations.RemoveCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1058,14 +1076,15 @@
         res = operations.RemoveCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1112,14 +1131,15 @@
         res = operations.RemoveCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1165,14 +1185,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCommerceCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceCollection])
                 res.commerce_collection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1222,14 +1243,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceInventory])
                 res.commerce_inventory = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1279,14 +1301,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceItem])
                 res.commerce_item = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1336,14 +1359,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceLocation])
                 res.commerce_location = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/company.py` & `Unified-python-sdk-0.22.0/src/unified_to/company.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmCompany])
                 res.crm_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsCompany])
                 res.ats_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmCompany])
                 res.crm_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -218,14 +221,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsCompaniesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsCompany]])
                 res.ats_companies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -273,14 +277,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmCompaniesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmCompany]])
                 res.crm_companies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -328,14 +333,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListEnrichCompaniesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.EnrichCompany])
                 res.enrich_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -385,14 +391,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmCompany])
                 res.crm_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -443,14 +450,15 @@
         res = operations.RemoveCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -496,14 +504,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmCompany])
                 res.crm_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/connection.py` & `Unified-python-sdk-0.22.0/src/unified_to/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_unified_connection(self, request: Optional[shared.Connection]) -> operations.CreateUnifiedConnectionResponse:
+    def create_unified_connection(self, request: Optional[shared.Connection] = None) -> operations.CreateUnifiedConnectionResponse:
         r"""Create connection"""
         hook_ctx = HookContext(operation_id='createUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/unified/connection'
         
         if callable(self.sdk_configuration.security):
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -107,14 +108,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -162,14 +164,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedConnectionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Connection]])
                 res.connections = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -219,14 +222,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -277,14 +281,15 @@
         res = operations.RemoveUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -330,14 +335,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/contact.py` & `Unified-python-sdk-0.22.0/src/unified_to/contact.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingContact])
                 res.accounting_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,14 +111,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmContact])
                 res.crm_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -167,14 +169,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UcContact])
                 res.uc_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -222,14 +225,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingContact])
                 res.accounting_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -277,14 +281,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmContact])
                 res.crm_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -332,14 +337,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UcContact])
                 res.uc_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -387,14 +393,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingContactsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingContact]])
                 res.accounting_contacts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -442,14 +449,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmContactsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmContact]])
                 res.crm_contacts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -497,14 +505,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUcContactsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.UcContact]])
                 res.uc_contacts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -554,14 +563,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingContact])
                 res.accounting_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -611,14 +621,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmContact])
                 res.crm_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -668,14 +679,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UcContact])
                 res.uc_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -726,14 +738,15 @@
         res = operations.RemoveAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -780,14 +793,15 @@
         res = operations.RemoveCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -834,14 +848,15 @@
         res = operations.RemoveUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -887,14 +902,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingContact])
                 res.accounting_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -944,14 +960,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmContact])
                 res.crm_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1001,14 +1018,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UcContact])
                 res.uc_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/crm.py` & `Unified-python-sdk-0.22.0/src/unified_to/crm.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmCompany])
                 res.crm_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,14 +111,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmContact])
                 res.crm_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -167,14 +169,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmDeal])
                 res.crm_deal = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -224,14 +227,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmEvent])
                 res.crm_event = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -281,14 +285,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmLead])
                 res.crm_lead = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -338,14 +343,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmPipeline])
                 res.crm_pipeline = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -393,14 +399,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmCompany])
                 res.crm_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -448,14 +455,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmContact])
                 res.crm_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -503,14 +511,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmDeal])
                 res.crm_deal = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -558,14 +567,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmEvent])
                 res.crm_event = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -613,14 +623,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmLead])
                 res.crm_lead = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -668,14 +679,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmPipeline])
                 res.crm_pipeline = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -723,14 +735,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmCompaniesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmCompany]])
                 res.crm_companies = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -778,14 +791,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmContactsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmContact]])
                 res.crm_contacts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -833,14 +847,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmDealsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmDeal]])
                 res.crm_deals = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -888,14 +903,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmEventsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmEvent]])
                 res.crm_events = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -943,14 +959,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmLeadsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmLead]])
                 res.crm_leads = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -998,14 +1015,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmPipelinesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmPipeline]])
                 res.crm_pipelines = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1055,14 +1073,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmCompany])
                 res.crm_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1112,14 +1131,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmContact])
                 res.crm_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1169,14 +1189,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmDeal])
                 res.crm_deal = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1226,14 +1247,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmEvent])
                 res.crm_event = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1283,14 +1305,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmLead])
                 res.crm_lead = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1340,14 +1363,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmPipeline])
                 res.crm_pipeline = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1398,14 +1422,15 @@
         res = operations.RemoveCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1452,14 +1477,15 @@
         res = operations.RemoveCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1506,14 +1532,15 @@
         res = operations.RemoveCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1560,14 +1587,15 @@
         res = operations.RemoveCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1614,14 +1642,15 @@
         res = operations.RemoveCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1668,14 +1697,15 @@
         res = operations.RemoveCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1721,14 +1751,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmCompanyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmCompany])
                 res.crm_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1778,14 +1809,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmContact])
                 res.crm_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1835,14 +1867,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmDeal])
                 res.crm_deal = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1892,14 +1925,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmEvent])
                 res.crm_event = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1949,14 +1983,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmLead])
                 res.crm_lead = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -2006,14 +2041,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmPipeline])
                 res.crm_pipeline = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/customer.py` & `Unified-python-sdk-0.22.0/src/unified_to/customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingCustomer])
                 res.ticketing_customer = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingCustomer])
                 res.ticketing_customer = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTicketingCustomersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.TicketingCustomer]])
                 res.ticketing_customers = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingCustomer])
                 res.ticketing_customer = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingCustomer])
                 res.ticketing_customer = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/deal.py` & `Unified-python-sdk-0.22.0/src/unified_to/deal.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmDeal])
                 res.crm_deal = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmDeal])
                 res.crm_deal = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmDealsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmDeal]])
                 res.crm_deals = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmDeal])
                 res.crm_deal = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmDealResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmDeal])
                 res.crm_deal = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/document.py` & `Unified-python-sdk-0.22.0/src/unified_to/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsDocument])
                 res.ats_document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsDocument])
                 res.ats_document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsDocumentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsDocument]])
                 res.ats_documents = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsDocument])
                 res.ats_document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsDocumentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsDocument])
                 res.ats_document = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/employee.py` & `Unified-python-sdk-0.22.0/src/unified_to/employee.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisEmployee])
                 res.hris_employee = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisEmployee])
                 res.hris_employee = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListHrisEmployeesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.HrisEmployee]])
                 res.hris_employees = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisEmployee])
                 res.hris_employee = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisEmployee])
                 res.hris_employee = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/enrich.py` & `Unified-python-sdk-0.22.0/src/unified_to/enrich.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListEnrichCompaniesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.EnrichCompany])
                 res.enrich_company = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -106,14 +107,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListEnrichPeopleResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.EnrichPerson])
                 res.enrich_person = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/event.py` & `Unified-python-sdk-0.22.0/src/unified_to/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmEvent])
                 res.crm_event = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmEvent])
                 res.crm_event = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmEventsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmEvent]])
                 res.crm_events = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmEvent])
                 res.crm_event = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmEvent])
                 res.crm_event = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/file.py` & `Unified-python-sdk-0.22.0/src/unified_to/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.StorageFile])
                 res.storage_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.StorageFile])
                 res.storage_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListStorageFilesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.StorageFile]])
                 res.storage_files = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.StorageFile])
                 res.storage_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.StorageFile])
                 res.storage_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/group.py` & `Unified-python-sdk-0.22.0/src/unified_to/job.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import List, Optional
 from unified_to import utils
 from unified_to._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from unified_to.models import errors, operations, shared
 
-class Group:
+class Job:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_hris_group(self, request: operations.CreateHrisGroupRequest) -> operations.CreateHrisGroupResponse:
-        r"""Create a group"""
-        hook_ctx = HookContext(operation_id='createHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def create_ats_job(self, request: operations.CreateAtsJobRequest) -> operations.CreateAtsJobResponse:
+        r"""Create a job"""
+        hook_ctx = HookContext(operation_id='createAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/hris/{connection_id}/group', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateHrisGroupRequest, "hris_group", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsJobRequest, "ats_job", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -50,38 +50,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.CreateHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
-                res.hris_group = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
+                res.ats_job = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_hris_group(self, request: operations.GetHrisGroupRequest) -> operations.GetHrisGroupResponse:
-        r"""Retrieve a group"""
-        hook_ctx = HookContext(operation_id='getHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_ats_job(self, request: operations.GetAtsJobRequest) -> operations.GetAtsJobResponse:
+        r"""Retrieve a job"""
+        hook_ctx = HookContext(operation_id='getAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         query_params = { **utils.get_query_params(request), **query_params }
@@ -105,38 +106,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
-                res.hris_group = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
+                res.ats_job = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list_hris_groups(self, request: operations.ListHrisGroupsRequest) -> operations.ListHrisGroupsResponse:
-        r"""List all groups"""
-        hook_ctx = HookContext(operation_id='listHrisGroups', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def list_ats_jobs(self, request: operations.ListAtsJobsRequest) -> operations.ListAtsJobsResponse:
+        r"""List all jobs"""
+        hook_ctx = HookContext(operation_id='listAtsJobs', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/hris/{connection_id}/group', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         query_params = { **utils.get_query_params(request), **query_params }
@@ -160,45 +162,46 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.ListHrisGroupsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.ListAtsJobsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[shared.HrisGroup]])
-                res.hris_groups = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsJob]])
+                res.ats_jobs = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def patch_hris_group(self, request: operations.PatchHrisGroupRequest) -> operations.PatchHrisGroupResponse:
-        r"""Update a group"""
-        hook_ctx = HookContext(operation_id='patchHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def patch_ats_job(self, request: operations.PatchAtsJobRequest) -> operations.PatchAtsJobResponse:
+        r"""Update a job"""
+        hook_ctx = HookContext(operation_id='patchAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.PatchHrisGroupRequest, "hris_group", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsJobRequest, "ats_job", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -217,38 +220,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.PatchHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.PatchAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
-                res.hris_group = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
+                res.ats_job = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def remove_hris_group(self, request: operations.RemoveHrisGroupRequest) -> operations.RemoveHrisGroupResponse:
-        r"""Remove a group"""
-        hook_ctx = HookContext(operation_id='removeHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def remove_ats_job(self, request: operations.RemoveAtsJobRequest) -> operations.RemoveAtsJobResponse:
+        r"""Remove a job"""
+        hook_ctx = HookContext(operation_id='removeAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -271,45 +275,46 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.RemoveHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.RemoveAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def update_hris_group(self, request: operations.UpdateHrisGroupRequest) -> operations.UpdateHrisGroupResponse:
-        r"""Update a group"""
-        hook_ctx = HookContext(operation_id='updateHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def update_ats_job(self, request: operations.UpdateAtsJobRequest) -> operations.UpdateAtsJobResponse:
+        r"""Update a job"""
+        hook_ctx = HookContext(operation_id='updateAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateHrisGroupRequest, "hris_group", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsJobRequest, "ats_job", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -328,20 +333,21 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.UpdateHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
-                res.hris_group = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
+                res.ats_job = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/hris.py` & `Unified-python-sdk-0.22.0/src/unified_to/hris.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisEmployee])
                 res.hris_employee = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,14 +111,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
                 res.hris_group = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -165,14 +167,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisEmployee])
                 res.hris_employee = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
                 res.hris_group = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -275,14 +279,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetHrisPayslipResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisPayslip])
                 res.hris_payslip = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -330,14 +335,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetHrisTimeoffResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisTimeoff])
                 res.hris_timeoff = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -385,14 +391,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListHrisEmployeesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.HrisEmployee]])
                 res.hris_employees = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -440,14 +447,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListHrisGroupsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.HrisGroup]])
                 res.hris_groups = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -495,14 +503,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListHrisPayslipsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.HrisPayslip]])
                 res.hris_payslips = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -550,14 +559,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListHrisTimeoffsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.HrisTimeoff]])
                 res.hris_timeoffs = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -607,14 +617,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisEmployee])
                 res.hris_employee = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -664,14 +675,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
                 res.hris_group = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -722,14 +734,15 @@
         res = operations.RemoveHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -776,14 +789,15 @@
         res = operations.RemoveHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -829,14 +843,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateHrisEmployeeResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisEmployee])
                 res.hris_employee = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -886,14 +901,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
                 res.hris_group = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/integration.py` & `Unified-python-sdk-0.22.0/src/unified_to/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedIntegrationAuthResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'text/plain'):                
                 res.res = http_res.text
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -109,14 +110,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedIntegrationWorkspacesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Integration]])
                 res.integrations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -164,14 +166,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedIntegrationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Integration]])
                 res.integrations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/interview.py` & `Unified-python-sdk-0.22.0/src/unified_to/interview.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsInterview])
                 res.ats_interview = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsInterview])
                 res.ats_interview = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsInterviewsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsInterview]])
                 res.ats_interviews = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsInterview])
                 res.ats_interview = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsInterviewResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsInterview])
                 res.ats_interview = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/inventory.py` & `Unified-python-sdk-0.22.0/src/unified_to/inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceInventory])
                 res.commerce_inventory = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceInventory])
                 res.commerce_inventory = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCommerceInventoriesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CommerceInventory]])
                 res.commerce_inventories = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceInventory])
                 res.commerce_inventory = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCommerceInventoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceInventory])
                 res.commerce_inventory = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/invoice.py` & `Unified-python-sdk-0.22.0/src/unified_to/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingInvoice])
                 res.accounting_invoice = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingInvoice])
                 res.accounting_invoice = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingInvoicesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingInvoice]])
                 res.accounting_invoices = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingInvoice])
                 res.accounting_invoice = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingInvoiceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingInvoice])
                 res.accounting_invoice = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/issue.py` & `Unified-python-sdk-0.22.0/src/unified_to/issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedIssuesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Issue]])
                 res.issues = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -105,14 +106,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedSupportsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UndefinedT])
                 res.undefined = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/item.py` & `Unified-python-sdk-0.22.0/src/unified_to/item.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceItem])
                 res.commerce_item = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceItem])
                 res.commerce_item = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCommerceItemsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CommerceItem]])
                 res.commerce_items = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceItem])
                 res.commerce_item = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCommerceItemResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceItem])
                 res.commerce_item = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/job.py` & `Unified-python-sdk-0.22.0/src/unified_to/link.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import List, Optional
 from unified_to import utils
 from unified_to._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from unified_to.models import errors, operations, shared
 
-class Job:
+class Link:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_ats_job(self, request: operations.CreateAtsJobRequest) -> operations.CreateAtsJobResponse:
-        r"""Create a job"""
-        hook_ctx = HookContext(operation_id='createAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def create_payment_link(self, request: operations.CreatePaymentLinkRequest) -> operations.CreatePaymentLinkResponse:
+        r"""Create a link"""
+        hook_ctx = HookContext(operation_id='createPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/ats/{connection_id}/job', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsJobRequest, "ats_job", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreatePaymentLinkRequest, "payment_link", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -50,38 +50,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.CreateAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreatePaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
-                res.ats_job = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
+                res.payment_link = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_ats_job(self, request: operations.GetAtsJobRequest) -> operations.GetAtsJobResponse:
-        r"""Retrieve a job"""
-        hook_ctx = HookContext(operation_id='getAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_payment_link(self, request: operations.GetPaymentLinkRequest) -> operations.GetPaymentLinkResponse:
+        r"""Retrieve a link"""
+        hook_ctx = HookContext(operation_id='getPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         query_params = { **utils.get_query_params(request), **query_params }
@@ -105,38 +106,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetPaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
-                res.ats_job = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
+                res.payment_link = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list_ats_jobs(self, request: operations.ListAtsJobsRequest) -> operations.ListAtsJobsResponse:
-        r"""List all jobs"""
-        hook_ctx = HookContext(operation_id='listAtsJobs', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def list_payment_links(self, request: operations.ListPaymentLinksRequest) -> operations.ListPaymentLinksResponse:
+        r"""List all links"""
+        hook_ctx = HookContext(operation_id='listPaymentLinks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/ats/{connection_id}/job', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         query_params = { **utils.get_query_params(request), **query_params }
@@ -160,45 +162,46 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.ListAtsJobsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.ListPaymentLinksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsJob]])
-                res.ats_jobs = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[shared.PaymentLink]])
+                res.payment_links = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def patch_ats_job(self, request: operations.PatchAtsJobRequest) -> operations.PatchAtsJobResponse:
-        r"""Update a job"""
-        hook_ctx = HookContext(operation_id='patchAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def patch_payment_link(self, request: operations.PatchPaymentLinkRequest) -> operations.PatchPaymentLinkResponse:
+        r"""Update a link"""
+        hook_ctx = HookContext(operation_id='patchPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsJobRequest, "ats_job", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.PatchPaymentLinkRequest, "payment_link", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -217,38 +220,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.PatchAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.PatchPaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
-                res.ats_job = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
+                res.payment_link = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def remove_ats_job(self, request: operations.RemoveAtsJobRequest) -> operations.RemoveAtsJobResponse:
-        r"""Remove a job"""
-        hook_ctx = HookContext(operation_id='removeAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def remove_payment_link(self, request: operations.RemovePaymentLinkRequest) -> operations.RemovePaymentLinkResponse:
+        r"""Remove a link"""
+        hook_ctx = HookContext(operation_id='removePaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -271,45 +275,46 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.RemoveAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.RemovePaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def update_ats_job(self, request: operations.UpdateAtsJobRequest) -> operations.UpdateAtsJobResponse:
-        r"""Update a job"""
-        hook_ctx = HookContext(operation_id='updateAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def update_payment_link(self, request: operations.UpdatePaymentLinkRequest) -> operations.UpdatePaymentLinkResponse:
+        r"""Update a link"""
+        hook_ctx = HookContext(operation_id='updatePaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsJobRequest, "ats_job", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdatePaymentLinkRequest, "payment_link", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
@@ -328,20 +333,21 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.UpdateAtsJobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdatePaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.AtsJob])
-                res.ats_job = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
+                res.payment_link = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/lead.py` & `Unified-python-sdk-0.22.0/src/unified_to/lead.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmLead])
                 res.crm_lead = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmLead])
                 res.crm_lead = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmLeadsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmLead]])
                 res.crm_leads = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmLead])
                 res.crm_lead = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmLeadResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmLead])
                 res.crm_lead = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/link.py` & `Unified-python-sdk-0.22.0/src/unified_to/webhook.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,37 +3,40 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import List, Optional
 from unified_to import utils
 from unified_to._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from unified_to.models import errors, operations, shared
 
-class Link:
+class Webhook:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_payment_link(self, request: operations.CreatePaymentLinkRequest) -> operations.CreatePaymentLinkResponse:
-        r"""Create a link"""
-        hook_ctx = HookContext(operation_id='createPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def create_unified_webhook(self, request: operations.CreateUnifiedWebhookRequest) -> operations.CreateUnifiedWebhookResponse:
+        r"""Create webhook subscription
+        The data payload received by your server is described at https://docs.unified.to/unified/overview. The `interval` field can be set as low as 1 minute for paid accounts, and 60 minutes for free accounts.
+        """
+        hook_ctx = HookContext(operation_id='createUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/payment/{connection_id}/link', request)
+        url = base_url + '/unified/webhook'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreatePaymentLinkRequest, "payment_link", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateUnifiedWebhookRequest, "webhook", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -50,45 +53,45 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.CreatePaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateUnifiedWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
-                res.payment_link = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
+                res.webhook = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_payment_link(self, request: operations.GetPaymentLinkRequest) -> operations.GetPaymentLinkResponse:
-        r"""Retrieve a link"""
-        hook_ctx = HookContext(operation_id='getPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_unified_webhook(self, request: operations.GetUnifiedWebhookRequest) -> operations.GetUnifiedWebhookResponse:
+        r"""Retrieve webhook by its ID"""
+        hook_ctx = HookContext(operation_id='getUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -105,38 +108,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetPaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetUnifiedWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
-                res.payment_link = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
+                res.webhook = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list_payment_links(self, request: operations.ListPaymentLinksRequest) -> operations.ListPaymentLinksResponse:
-        r"""List all links"""
-        hook_ctx = HookContext(operation_id='listPaymentLinks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def list_unified_webhooks(self, request: operations.ListUnifiedWebhooksRequest) -> operations.ListUnifiedWebhooksResponse:
+        r"""Returns all registered webhooks"""
+        hook_ctx = HookContext(operation_id='listUnifiedWebhooks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/payment/{connection_id}/link', request)
+        url = base_url + '/unified/webhook'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         query_params = { **utils.get_query_params(request), **query_params }
@@ -160,53 +164,51 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.ListPaymentLinksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.ListUnifiedWebhooksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[shared.PaymentLink]])
-                res.payment_links = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[shared.Webhook]])
+                res.webhooks = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def patch_payment_link(self, request: operations.PatchPaymentLinkRequest) -> operations.PatchPaymentLinkResponse:
-        r"""Update a link"""
-        hook_ctx = HookContext(operation_id='patchPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def patch_unified_webhook_trigger(self, request: operations.PatchUnifiedWebhookTriggerRequest) -> operations.PatchUnifiedWebhookTriggerResponse:
+        r"""Trigger webhook"""
+        hook_ctx = HookContext(operation_id='patchUnifiedWebhookTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}/trigger', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.PatchPaymentLinkRequest, "payment_link", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -217,38 +219,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.PatchPaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.PatchUnifiedWebhookTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 200:
+        if http_res.status_code >= 200 and http_res.status_code < 300:
+            pass
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
-                res.payment_link = out
+                out = utils.unmarshal_json(http_res.text, Optional[str])
+                res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def remove_payment_link(self, request: operations.RemovePaymentLinkRequest) -> operations.RemovePaymentLinkResponse:
-        r"""Remove a link"""
-        hook_ctx = HookContext(operation_id='removePaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def remove_unified_webhook(self, request: operations.RemoveUnifiedWebhookRequest) -> operations.RemoveUnifiedWebhookResponse:
+        r"""Remove webhook subscription"""
+        hook_ctx = HookContext(operation_id='removeUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -271,53 +274,51 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.RemovePaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.RemoveUnifiedWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def update_payment_link(self, request: operations.UpdatePaymentLinkRequest) -> operations.UpdatePaymentLinkResponse:
-        r"""Update a link"""
-        hook_ctx = HookContext(operation_id='updatePaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def update_unified_webhook_trigger(self, request: operations.UpdateUnifiedWebhookTriggerRequest) -> operations.UpdateUnifiedWebhookTriggerResponse:
+        r"""Trigger webhook"""
+        hook_ctx = HookContext(operation_id='updateUnifiedWebhookTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}/trigger', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdatePaymentLinkRequest, "payment_link", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -328,25 +329,26 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.UpdatePaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateUnifiedWebhookTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code == 200:
+        if http_res.status_code >= 200 and http_res.status_code < 300:
+            pass
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
-                res.payment_link = out
+                out = utils.unmarshal_json(http_res.text, Optional[str])
+                res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/list.py` & `Unified-python-sdk-0.22.0/src/unified_to/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingList])
                 res.marketing_list = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingList])
                 res.marketing_list = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListMartechListsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.MarketingList]])
                 res.marketing_lists = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingList])
                 res.marketing_list = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingList])
                 res.marketing_list = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/location.py` & `Unified-python-sdk-0.22.0/src/unified_to/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceLocation])
                 res.commerce_location = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceLocation])
                 res.commerce_location = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCommerceLocationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CommerceLocation]])
                 res.commerce_locations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceLocation])
                 res.commerce_location = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCommerceLocationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CommerceLocation])
                 res.commerce_location = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/login.py` & `Unified-python-sdk-0.22.0/src/unified_to/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedIntegrationLoginResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'text/plain'):                
                 res.res = http_res.text
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/martech.py` & `Unified-python-sdk-0.22.0/src/unified_to/martech.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingList])
                 res.marketing_list = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,14 +111,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingMember])
                 res.marketing_member = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -165,14 +167,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingList])
                 res.marketing_list = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingMember])
                 res.marketing_member = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -275,14 +279,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListMartechListsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.MarketingList]])
                 res.marketing_lists = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -330,14 +335,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListMartechMembersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.MarketingMember]])
                 res.marketing_members = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -387,14 +393,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingList])
                 res.marketing_list = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -444,14 +451,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingMember])
                 res.marketing_member = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -502,14 +510,15 @@
         res = operations.RemoveMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -556,14 +565,15 @@
         res = operations.RemoveMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -609,14 +619,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateMartechListResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingList])
                 res.marketing_list = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -666,14 +677,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingMember])
                 res.marketing_member = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/member.py` & `Unified-python-sdk-0.22.0/src/unified_to/member.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingMember])
                 res.marketing_member = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingMember])
                 res.marketing_member = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListMartechMembersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.MarketingMember]])
                 res.marketing_members = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingMember])
                 res.marketing_member = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateMartechMemberResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MarketingMember])
                 res.marketing_member = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/errors/sdkerror.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/__init__.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .createcommercelocation import *
 from .createcrmcompany import *
 from .createcrmcontact import *
 from .createcrmdeal import *
 from .createcrmevent import *
 from .createcrmlead import *
 from .createcrmpipeline import *
+from .creategenaiprompt import *
 from .createhrisemployee import *
 from .createhrisgroup import *
 from .createmartechlist import *
 from .createmartechmember import *
 from .createpassthrough import *
 from .createpaymentlink import *
 from .createpaymentpayment import *
@@ -103,14 +104,15 @@
 from .listcrmcontacts import *
 from .listcrmdeals import *
 from .listcrmevents import *
 from .listcrmleads import *
 from .listcrmpipelines import *
 from .listenrichcompanies import *
 from .listenrichpeople import *
+from .listgenaimodels import *
 from .listhrisemployees import *
 from .listhrisgroups import *
 from .listhrispayslips import *
 from .listhristimeoffs import *
 from .listmartechlists import *
 from .listmartechmembers import *
 from .listpassthroughs import *
@@ -236,8 +238,8 @@
 from .updateticketingcustomer import *
 from .updateticketingnote import *
 from .updateticketingticket import *
 from .updateuccontact import *
 from .updateunifiedconnection import *
 from .updateunifiedwebhooktrigger import *
 
-__all__ = ["Categories","CreateAccountingAccountRequest","CreateAccountingAccountResponse","CreateAccountingContactRequest","CreateAccountingContactResponse","CreateAccountingInvoiceRequest","CreateAccountingInvoiceResponse","CreateAccountingTaxrateRequest","CreateAccountingTaxrateResponse","CreateAccountingTransactionRequest","CreateAccountingTransactionResponse","CreateAtsActivityRequest","CreateAtsActivityResponse","CreateAtsApplicationRequest","CreateAtsApplicationResponse","CreateAtsCandidateRequest","CreateAtsCandidateResponse","CreateAtsDocumentRequest","CreateAtsDocumentResponse","CreateAtsInterviewRequest","CreateAtsInterviewResponse","CreateAtsJobRequest","CreateAtsJobResponse","CreateAtsScorecardRequest","CreateAtsScorecardResponse","CreateCommerceCollectionRequest","CreateCommerceCollectionResponse","CreateCommerceInventoryRequest","CreateCommerceInventoryResponse","CreateCommerceItemRequest","CreateCommerceItemResponse","CreateCommerceLocationRequest","CreateCommerceLocationResponse","CreateCrmCompanyRequest","CreateCrmCompanyResponse","CreateCrmContactRequest","CreateCrmContactResponse","CreateCrmDealRequest","CreateCrmDealResponse","CreateCrmEventRequest","CreateCrmEventResponse","CreateCrmLeadRequest","CreateCrmLeadResponse","CreateCrmPipelineRequest","CreateCrmPipelineResponse","CreateHrisEmployeeRequest","CreateHrisEmployeeResponse","CreateHrisGroupRequest","CreateHrisGroupResponse","CreateMartechListRequest","CreateMartechListResponse","CreateMartechMemberRequest","CreateMartechMemberResponse","CreatePassthroughRequest","CreatePassthroughResponse","CreatePaymentLinkRequest","CreatePaymentLinkResponse","CreatePaymentPaymentRequest","CreatePaymentPaymentResponse","CreateStorageFileRequest","CreateStorageFileResponse","CreateTicketingCustomerRequest","CreateTicketingCustomerResponse","CreateTicketingNoteRequest","CreateTicketingNoteResponse","CreateTicketingTicketRequest","CreateTicketingTicketResponse","CreateUcContactRequest","CreateUcContactResponse","CreateUnifiedConnectionResponse","CreateUnifiedWebhookRequest","CreateUnifiedWebhookResponse","GetAccountingAccountRequest","GetAccountingAccountResponse","GetAccountingContactRequest","GetAccountingContactResponse","GetAccountingInvoiceRequest","GetAccountingInvoiceResponse","GetAccountingOrganizationRequest","GetAccountingOrganizationResponse","GetAccountingTaxrateRequest","GetAccountingTaxrateResponse","GetAccountingTransactionRequest","GetAccountingTransactionResponse","GetAtsActivityRequest","GetAtsActivityResponse","GetAtsApplicationRequest","GetAtsApplicationResponse","GetAtsCandidateRequest","GetAtsCandidateResponse","GetAtsCompanyRequest","GetAtsCompanyResponse","GetAtsDocumentRequest","GetAtsDocumentResponse","GetAtsInterviewRequest","GetAtsInterviewResponse","GetAtsJobRequest","GetAtsJobResponse","GetAtsScorecardRequest","GetAtsScorecardResponse","GetCommerceCollectionRequest","GetCommerceCollectionResponse","GetCommerceInventoryRequest","GetCommerceInventoryResponse","GetCommerceItemRequest","GetCommerceItemResponse","GetCommerceLocationRequest","GetCommerceLocationResponse","GetCrmCompanyRequest","GetCrmCompanyResponse","GetCrmContactRequest","GetCrmContactResponse","GetCrmDealRequest","GetCrmDealResponse","GetCrmEventRequest","GetCrmEventResponse","GetCrmLeadRequest","GetCrmLeadResponse","GetCrmPipelineRequest","GetCrmPipelineResponse","GetHrisEmployeeRequest","GetHrisEmployeeResponse","GetHrisGroupRequest","GetHrisGroupResponse","GetHrisPayslipRequest","GetHrisPayslipResponse","GetHrisTimeoffRequest","GetHrisTimeoffResponse","GetMartechListRequest","GetMartechListResponse","GetMartechMemberRequest","GetMartechMemberResponse","GetPaymentLinkRequest","GetPaymentLinkResponse","GetPaymentPaymentRequest","GetPaymentPaymentResponse","GetPaymentPayoutRequest","GetPaymentPayoutResponse","GetPaymentRefundRequest","GetPaymentRefundResponse","GetStorageFileRequest","GetStorageFileResponse","GetTicketingCustomerRequest","GetTicketingCustomerResponse","GetTicketingNoteRequest","GetTicketingNoteResponse","GetTicketingTicketRequest","GetTicketingTicketResponse","GetUcContactRequest","GetUcContactResponse","GetUnifiedApicallRequest","GetUnifiedApicallResponse","GetUnifiedConnectionRequest","GetUnifiedConnectionResponse","GetUnifiedIntegrationAuthRequest","GetUnifiedIntegrationAuthResponse","GetUnifiedIntegrationLoginRequest","GetUnifiedIntegrationLoginResponse","GetUnifiedWebhookRequest","GetUnifiedWebhookResponse","ListAccountingAccountsRequest","ListAccountingAccountsResponse","ListAccountingContactsRequest","ListAccountingContactsResponse","ListAccountingInvoicesRequest","ListAccountingInvoicesResponse","ListAccountingOrganizationsRequest","ListAccountingOrganizationsResponse","ListAccountingTaxratesRequest","ListAccountingTaxratesResponse","ListAccountingTransactionsRequest","ListAccountingTransactionsResponse","ListAtsActivitiesRequest","ListAtsActivitiesResponse","ListAtsApplicationsRequest","ListAtsApplicationsResponse","ListAtsApplicationstatusesRequest","ListAtsApplicationstatusesResponse","ListAtsCandidatesRequest","ListAtsCandidatesResponse","ListAtsCompaniesRequest","ListAtsCompaniesResponse","ListAtsDocumentsRequest","ListAtsDocumentsResponse","ListAtsInterviewsRequest","ListAtsInterviewsResponse","ListAtsJobsRequest","ListAtsJobsResponse","ListAtsScorecardsRequest","ListAtsScorecardsResponse","ListCommerceCollectionsRequest","ListCommerceCollectionsResponse","ListCommerceInventoriesRequest","ListCommerceInventoriesResponse","ListCommerceItemsRequest","ListCommerceItemsResponse","ListCommerceLocationsRequest","ListCommerceLocationsResponse","ListCrmCompaniesRequest","ListCrmCompaniesResponse","ListCrmContactsRequest","ListCrmContactsResponse","ListCrmDealsRequest","ListCrmDealsResponse","ListCrmEventsRequest","ListCrmEventsResponse","ListCrmLeadsRequest","ListCrmLeadsResponse","ListCrmPipelinesRequest","ListCrmPipelinesResponse","ListEnrichCompaniesRequest","ListEnrichCompaniesResponse","ListEnrichPeopleRequest","ListEnrichPeopleResponse","ListHrisEmployeesRequest","ListHrisEmployeesResponse","ListHrisGroupsRequest","ListHrisGroupsResponse","ListHrisPayslipsRequest","ListHrisPayslipsResponse","ListHrisTimeoffsRequest","ListHrisTimeoffsResponse","ListMartechListsRequest","ListMartechListsResponse","ListMartechMembersRequest","ListMartechMembersResponse","ListPassthroughsRequest","ListPassthroughsResponse","ListPaymentLinksRequest","ListPaymentLinksResponse","ListPaymentPaymentsRequest","ListPaymentPaymentsResponse","ListPaymentPayoutsRequest","ListPaymentPayoutsResponse","ListPaymentRefundsRequest","ListPaymentRefundsResponse","ListStorageFilesRequest","ListStorageFilesResponse","ListTicketingCustomersRequest","ListTicketingCustomersResponse","ListTicketingNotesRequest","ListTicketingNotesResponse","ListTicketingTicketsRequest","ListTicketingTicketsResponse","ListUcCallsRequest","ListUcCallsResponse","ListUcContactsRequest","ListUcContactsResponse","ListUnifiedApicallsRequest","ListUnifiedApicallsResponse","ListUnifiedConnectionsRequest","ListUnifiedConnectionsResponse","ListUnifiedIntegrationWorkspacesRequest","ListUnifiedIntegrationWorkspacesResponse","ListUnifiedIntegrationsQueryParamCategories","ListUnifiedIntegrationsRequest","ListUnifiedIntegrationsResponse","ListUnifiedIssuesRequest","ListUnifiedIssuesResponse","ListUnifiedSupportsResponse","ListUnifiedWebhooksRequest","ListUnifiedWebhooksResponse","PatchAccountingAccountRequest","PatchAccountingAccountResponse","PatchAccountingContactRequest","PatchAccountingContactResponse","PatchAccountingInvoiceRequest","PatchAccountingInvoiceResponse","PatchAccountingTaxrateRequest","PatchAccountingTaxrateResponse","PatchAccountingTransactionRequest","PatchAccountingTransactionResponse","PatchAtsActivityRequest","PatchAtsActivityResponse","PatchAtsApplicationRequest","PatchAtsApplicationResponse","PatchAtsCandidateRequest","PatchAtsCandidateResponse","PatchAtsDocumentRequest","PatchAtsDocumentResponse","PatchAtsInterviewRequest","PatchAtsInterviewResponse","PatchAtsJobRequest","PatchAtsJobResponse","PatchAtsScorecardRequest","PatchAtsScorecardResponse","PatchCommerceCollectionRequest","PatchCommerceCollectionResponse","PatchCommerceInventoryRequest","PatchCommerceInventoryResponse","PatchCommerceItemRequest","PatchCommerceItemResponse","PatchCommerceLocationRequest","PatchCommerceLocationResponse","PatchCrmCompanyRequest","PatchCrmCompanyResponse","PatchCrmContactRequest","PatchCrmContactResponse","PatchCrmDealRequest","PatchCrmDealResponse","PatchCrmEventRequest","PatchCrmEventResponse","PatchCrmLeadRequest","PatchCrmLeadResponse","PatchCrmPipelineRequest","PatchCrmPipelineResponse","PatchHrisEmployeeRequest","PatchHrisEmployeeResponse","PatchHrisGroupRequest","PatchHrisGroupResponse","PatchMartechListRequest","PatchMartechListResponse","PatchMartechMemberRequest","PatchMartechMemberResponse","PatchPassthroughRequest","PatchPassthroughResponse","PatchPaymentLinkRequest","PatchPaymentLinkResponse","PatchPaymentPaymentRequest","PatchPaymentPaymentResponse","PatchStorageFileRequest","PatchStorageFileResponse","PatchTicketingCustomerRequest","PatchTicketingCustomerResponse","PatchTicketingNoteRequest","PatchTicketingNoteResponse","PatchTicketingTicketRequest","PatchTicketingTicketResponse","PatchUcContactRequest","PatchUcContactResponse","PatchUnifiedConnectionRequest","PatchUnifiedConnectionResponse","PatchUnifiedWebhookTriggerRequest","PatchUnifiedWebhookTriggerResponse","QueryParamCategories","RemoveAccountingAccountRequest","RemoveAccountingAccountResponse","RemoveAccountingContactRequest","RemoveAccountingContactResponse","RemoveAccountingInvoiceRequest","RemoveAccountingInvoiceResponse","RemoveAccountingTaxrateRequest","RemoveAccountingTaxrateResponse","RemoveAccountingTransactionRequest","RemoveAccountingTransactionResponse","RemoveAtsActivityRequest","RemoveAtsActivityResponse","RemoveAtsApplicationRequest","RemoveAtsApplicationResponse","RemoveAtsCandidateRequest","RemoveAtsCandidateResponse","RemoveAtsDocumentRequest","RemoveAtsDocumentResponse","RemoveAtsInterviewRequest","RemoveAtsInterviewResponse","RemoveAtsJobRequest","RemoveAtsJobResponse","RemoveAtsScorecardRequest","RemoveAtsScorecardResponse","RemoveCommerceCollectionRequest","RemoveCommerceCollectionResponse","RemoveCommerceInventoryRequest","RemoveCommerceInventoryResponse","RemoveCommerceItemRequest","RemoveCommerceItemResponse","RemoveCommerceLocationRequest","RemoveCommerceLocationResponse","RemoveCrmCompanyRequest","RemoveCrmCompanyResponse","RemoveCrmContactRequest","RemoveCrmContactResponse","RemoveCrmDealRequest","RemoveCrmDealResponse","RemoveCrmEventRequest","RemoveCrmEventResponse","RemoveCrmLeadRequest","RemoveCrmLeadResponse","RemoveCrmPipelineRequest","RemoveCrmPipelineResponse","RemoveHrisEmployeeRequest","RemoveHrisEmployeeResponse","RemoveHrisGroupRequest","RemoveHrisGroupResponse","RemoveMartechListRequest","RemoveMartechListResponse","RemoveMartechMemberRequest","RemoveMartechMemberResponse","RemovePassthroughRequest","RemovePassthroughResponse","RemovePaymentLinkRequest","RemovePaymentLinkResponse","RemovePaymentPaymentRequest","RemovePaymentPaymentResponse","RemoveStorageFileRequest","RemoveStorageFileResponse","RemoveTicketingCustomerRequest","RemoveTicketingCustomerResponse","RemoveTicketingNoteRequest","RemoveTicketingNoteResponse","RemoveTicketingTicketRequest","RemoveTicketingTicketResponse","RemoveUcContactRequest","RemoveUcContactResponse","RemoveUnifiedConnectionRequest","RemoveUnifiedConnectionResponse","RemoveUnifiedWebhookRequest","RemoveUnifiedWebhookResponse","Scopes","UpdateAccountingAccountRequest","UpdateAccountingAccountResponse","UpdateAccountingContactRequest","UpdateAccountingContactResponse","UpdateAccountingInvoiceRequest","UpdateAccountingInvoiceResponse","UpdateAccountingTaxrateRequest","UpdateAccountingTaxrateResponse","UpdateAccountingTransactionRequest","UpdateAccountingTransactionResponse","UpdateAtsActivityRequest","UpdateAtsActivityResponse","UpdateAtsApplicationRequest","UpdateAtsApplicationResponse","UpdateAtsCandidateRequest","UpdateAtsCandidateResponse","UpdateAtsDocumentRequest","UpdateAtsDocumentResponse","UpdateAtsInterviewRequest","UpdateAtsInterviewResponse","UpdateAtsJobRequest","UpdateAtsJobResponse","UpdateAtsScorecardRequest","UpdateAtsScorecardResponse","UpdateCommerceCollectionRequest","UpdateCommerceCollectionResponse","UpdateCommerceInventoryRequest","UpdateCommerceInventoryResponse","UpdateCommerceItemRequest","UpdateCommerceItemResponse","UpdateCommerceLocationRequest","UpdateCommerceLocationResponse","UpdateCrmCompanyRequest","UpdateCrmCompanyResponse","UpdateCrmContactRequest","UpdateCrmContactResponse","UpdateCrmDealRequest","UpdateCrmDealResponse","UpdateCrmEventRequest","UpdateCrmEventResponse","UpdateCrmLeadRequest","UpdateCrmLeadResponse","UpdateCrmPipelineRequest","UpdateCrmPipelineResponse","UpdateHrisEmployeeRequest","UpdateHrisEmployeeResponse","UpdateHrisGroupRequest","UpdateHrisGroupResponse","UpdateMartechListRequest","UpdateMartechListResponse","UpdateMartechMemberRequest","UpdateMartechMemberResponse","UpdatePassthroughRequest","UpdatePassthroughResponse","UpdatePaymentLinkRequest","UpdatePaymentLinkResponse","UpdatePaymentPaymentRequest","UpdatePaymentPaymentResponse","UpdateStorageFileRequest","UpdateStorageFileResponse","UpdateTicketingCustomerRequest","UpdateTicketingCustomerResponse","UpdateTicketingNoteRequest","UpdateTicketingNoteResponse","UpdateTicketingTicketRequest","UpdateTicketingTicketResponse","UpdateUcContactRequest","UpdateUcContactResponse","UpdateUnifiedConnectionRequest","UpdateUnifiedConnectionResponse","UpdateUnifiedWebhookTriggerRequest","UpdateUnifiedWebhookTriggerResponse"]
+__all__ = ["Categories","CreateAccountingAccountRequest","CreateAccountingAccountResponse","CreateAccountingContactRequest","CreateAccountingContactResponse","CreateAccountingInvoiceRequest","CreateAccountingInvoiceResponse","CreateAccountingTaxrateRequest","CreateAccountingTaxrateResponse","CreateAccountingTransactionRequest","CreateAccountingTransactionResponse","CreateAtsActivityRequest","CreateAtsActivityResponse","CreateAtsApplicationRequest","CreateAtsApplicationResponse","CreateAtsCandidateRequest","CreateAtsCandidateResponse","CreateAtsDocumentRequest","CreateAtsDocumentResponse","CreateAtsInterviewRequest","CreateAtsInterviewResponse","CreateAtsJobRequest","CreateAtsJobResponse","CreateAtsScorecardRequest","CreateAtsScorecardResponse","CreateCommerceCollectionRequest","CreateCommerceCollectionResponse","CreateCommerceInventoryRequest","CreateCommerceInventoryResponse","CreateCommerceItemRequest","CreateCommerceItemResponse","CreateCommerceLocationRequest","CreateCommerceLocationResponse","CreateCrmCompanyRequest","CreateCrmCompanyResponse","CreateCrmContactRequest","CreateCrmContactResponse","CreateCrmDealRequest","CreateCrmDealResponse","CreateCrmEventRequest","CreateCrmEventResponse","CreateCrmLeadRequest","CreateCrmLeadResponse","CreateCrmPipelineRequest","CreateCrmPipelineResponse","CreateGenaiPromptRequest","CreateGenaiPromptResponse","CreateHrisEmployeeRequest","CreateHrisEmployeeResponse","CreateHrisGroupRequest","CreateHrisGroupResponse","CreateMartechListRequest","CreateMartechListResponse","CreateMartechMemberRequest","CreateMartechMemberResponse","CreatePassthroughRequest","CreatePassthroughResponse","CreatePaymentLinkRequest","CreatePaymentLinkResponse","CreatePaymentPaymentRequest","CreatePaymentPaymentResponse","CreateStorageFileRequest","CreateStorageFileResponse","CreateTicketingCustomerRequest","CreateTicketingCustomerResponse","CreateTicketingNoteRequest","CreateTicketingNoteResponse","CreateTicketingTicketRequest","CreateTicketingTicketResponse","CreateUcContactRequest","CreateUcContactResponse","CreateUnifiedConnectionResponse","CreateUnifiedWebhookRequest","CreateUnifiedWebhookResponse","GetAccountingAccountRequest","GetAccountingAccountResponse","GetAccountingContactRequest","GetAccountingContactResponse","GetAccountingInvoiceRequest","GetAccountingInvoiceResponse","GetAccountingOrganizationRequest","GetAccountingOrganizationResponse","GetAccountingTaxrateRequest","GetAccountingTaxrateResponse","GetAccountingTransactionRequest","GetAccountingTransactionResponse","GetAtsActivityRequest","GetAtsActivityResponse","GetAtsApplicationRequest","GetAtsApplicationResponse","GetAtsCandidateRequest","GetAtsCandidateResponse","GetAtsCompanyRequest","GetAtsCompanyResponse","GetAtsDocumentRequest","GetAtsDocumentResponse","GetAtsInterviewRequest","GetAtsInterviewResponse","GetAtsJobRequest","GetAtsJobResponse","GetAtsScorecardRequest","GetAtsScorecardResponse","GetCommerceCollectionRequest","GetCommerceCollectionResponse","GetCommerceInventoryRequest","GetCommerceInventoryResponse","GetCommerceItemRequest","GetCommerceItemResponse","GetCommerceLocationRequest","GetCommerceLocationResponse","GetCrmCompanyRequest","GetCrmCompanyResponse","GetCrmContactRequest","GetCrmContactResponse","GetCrmDealRequest","GetCrmDealResponse","GetCrmEventRequest","GetCrmEventResponse","GetCrmLeadRequest","GetCrmLeadResponse","GetCrmPipelineRequest","GetCrmPipelineResponse","GetHrisEmployeeRequest","GetHrisEmployeeResponse","GetHrisGroupRequest","GetHrisGroupResponse","GetHrisPayslipRequest","GetHrisPayslipResponse","GetHrisTimeoffRequest","GetHrisTimeoffResponse","GetMartechListRequest","GetMartechListResponse","GetMartechMemberRequest","GetMartechMemberResponse","GetPaymentLinkRequest","GetPaymentLinkResponse","GetPaymentPaymentRequest","GetPaymentPaymentResponse","GetPaymentPayoutRequest","GetPaymentPayoutResponse","GetPaymentRefundRequest","GetPaymentRefundResponse","GetStorageFileRequest","GetStorageFileResponse","GetTicketingCustomerRequest","GetTicketingCustomerResponse","GetTicketingNoteRequest","GetTicketingNoteResponse","GetTicketingTicketRequest","GetTicketingTicketResponse","GetUcContactRequest","GetUcContactResponse","GetUnifiedApicallRequest","GetUnifiedApicallResponse","GetUnifiedConnectionRequest","GetUnifiedConnectionResponse","GetUnifiedIntegrationAuthRequest","GetUnifiedIntegrationAuthResponse","GetUnifiedIntegrationLoginRequest","GetUnifiedIntegrationLoginResponse","GetUnifiedWebhookRequest","GetUnifiedWebhookResponse","ListAccountingAccountsRequest","ListAccountingAccountsResponse","ListAccountingContactsRequest","ListAccountingContactsResponse","ListAccountingInvoicesRequest","ListAccountingInvoicesResponse","ListAccountingOrganizationsRequest","ListAccountingOrganizationsResponse","ListAccountingTaxratesRequest","ListAccountingTaxratesResponse","ListAccountingTransactionsRequest","ListAccountingTransactionsResponse","ListAtsActivitiesRequest","ListAtsActivitiesResponse","ListAtsApplicationsRequest","ListAtsApplicationsResponse","ListAtsApplicationstatusesRequest","ListAtsApplicationstatusesResponse","ListAtsCandidatesRequest","ListAtsCandidatesResponse","ListAtsCompaniesRequest","ListAtsCompaniesResponse","ListAtsDocumentsRequest","ListAtsDocumentsResponse","ListAtsInterviewsRequest","ListAtsInterviewsResponse","ListAtsJobsRequest","ListAtsJobsResponse","ListAtsScorecardsRequest","ListAtsScorecardsResponse","ListCommerceCollectionsRequest","ListCommerceCollectionsResponse","ListCommerceInventoriesRequest","ListCommerceInventoriesResponse","ListCommerceItemsRequest","ListCommerceItemsResponse","ListCommerceLocationsRequest","ListCommerceLocationsResponse","ListCrmCompaniesRequest","ListCrmCompaniesResponse","ListCrmContactsRequest","ListCrmContactsResponse","ListCrmDealsRequest","ListCrmDealsResponse","ListCrmEventsRequest","ListCrmEventsResponse","ListCrmLeadsRequest","ListCrmLeadsResponse","ListCrmPipelinesRequest","ListCrmPipelinesResponse","ListEnrichCompaniesRequest","ListEnrichCompaniesResponse","ListEnrichPeopleRequest","ListEnrichPeopleResponse","ListGenaiModelsRequest","ListGenaiModelsResponse","ListHrisEmployeesRequest","ListHrisEmployeesResponse","ListHrisGroupsRequest","ListHrisGroupsResponse","ListHrisPayslipsRequest","ListHrisPayslipsResponse","ListHrisTimeoffsRequest","ListHrisTimeoffsResponse","ListMartechListsRequest","ListMartechListsResponse","ListMartechMembersRequest","ListMartechMembersResponse","ListPassthroughsRequest","ListPassthroughsResponse","ListPaymentLinksRequest","ListPaymentLinksResponse","ListPaymentPaymentsRequest","ListPaymentPaymentsResponse","ListPaymentPayoutsRequest","ListPaymentPayoutsResponse","ListPaymentRefundsRequest","ListPaymentRefundsResponse","ListStorageFilesRequest","ListStorageFilesResponse","ListTicketingCustomersRequest","ListTicketingCustomersResponse","ListTicketingNotesRequest","ListTicketingNotesResponse","ListTicketingTicketsRequest","ListTicketingTicketsResponse","ListUcCallsRequest","ListUcCallsResponse","ListUcContactsRequest","ListUcContactsResponse","ListUnifiedApicallsRequest","ListUnifiedApicallsResponse","ListUnifiedConnectionsRequest","ListUnifiedConnectionsResponse","ListUnifiedIntegrationWorkspacesRequest","ListUnifiedIntegrationWorkspacesResponse","ListUnifiedIntegrationsQueryParamCategories","ListUnifiedIntegrationsRequest","ListUnifiedIntegrationsResponse","ListUnifiedIssuesRequest","ListUnifiedIssuesResponse","ListUnifiedSupportsResponse","ListUnifiedWebhooksRequest","ListUnifiedWebhooksResponse","PatchAccountingAccountRequest","PatchAccountingAccountResponse","PatchAccountingContactRequest","PatchAccountingContactResponse","PatchAccountingInvoiceRequest","PatchAccountingInvoiceResponse","PatchAccountingTaxrateRequest","PatchAccountingTaxrateResponse","PatchAccountingTransactionRequest","PatchAccountingTransactionResponse","PatchAtsActivityRequest","PatchAtsActivityResponse","PatchAtsApplicationRequest","PatchAtsApplicationResponse","PatchAtsCandidateRequest","PatchAtsCandidateResponse","PatchAtsDocumentRequest","PatchAtsDocumentResponse","PatchAtsInterviewRequest","PatchAtsInterviewResponse","PatchAtsJobRequest","PatchAtsJobResponse","PatchAtsScorecardRequest","PatchAtsScorecardResponse","PatchCommerceCollectionRequest","PatchCommerceCollectionResponse","PatchCommerceInventoryRequest","PatchCommerceInventoryResponse","PatchCommerceItemRequest","PatchCommerceItemResponse","PatchCommerceLocationRequest","PatchCommerceLocationResponse","PatchCrmCompanyRequest","PatchCrmCompanyResponse","PatchCrmContactRequest","PatchCrmContactResponse","PatchCrmDealRequest","PatchCrmDealResponse","PatchCrmEventRequest","PatchCrmEventResponse","PatchCrmLeadRequest","PatchCrmLeadResponse","PatchCrmPipelineRequest","PatchCrmPipelineResponse","PatchHrisEmployeeRequest","PatchHrisEmployeeResponse","PatchHrisGroupRequest","PatchHrisGroupResponse","PatchMartechListRequest","PatchMartechListResponse","PatchMartechMemberRequest","PatchMartechMemberResponse","PatchPassthroughRequest","PatchPassthroughResponse","PatchPaymentLinkRequest","PatchPaymentLinkResponse","PatchPaymentPaymentRequest","PatchPaymentPaymentResponse","PatchStorageFileRequest","PatchStorageFileResponse","PatchTicketingCustomerRequest","PatchTicketingCustomerResponse","PatchTicketingNoteRequest","PatchTicketingNoteResponse","PatchTicketingTicketRequest","PatchTicketingTicketResponse","PatchUcContactRequest","PatchUcContactResponse","PatchUnifiedConnectionRequest","PatchUnifiedConnectionResponse","PatchUnifiedWebhookTriggerRequest","PatchUnifiedWebhookTriggerResponse","QueryParamCategories","RemoveAccountingAccountRequest","RemoveAccountingAccountResponse","RemoveAccountingContactRequest","RemoveAccountingContactResponse","RemoveAccountingInvoiceRequest","RemoveAccountingInvoiceResponse","RemoveAccountingTaxrateRequest","RemoveAccountingTaxrateResponse","RemoveAccountingTransactionRequest","RemoveAccountingTransactionResponse","RemoveAtsActivityRequest","RemoveAtsActivityResponse","RemoveAtsApplicationRequest","RemoveAtsApplicationResponse","RemoveAtsCandidateRequest","RemoveAtsCandidateResponse","RemoveAtsDocumentRequest","RemoveAtsDocumentResponse","RemoveAtsInterviewRequest","RemoveAtsInterviewResponse","RemoveAtsJobRequest","RemoveAtsJobResponse","RemoveAtsScorecardRequest","RemoveAtsScorecardResponse","RemoveCommerceCollectionRequest","RemoveCommerceCollectionResponse","RemoveCommerceInventoryRequest","RemoveCommerceInventoryResponse","RemoveCommerceItemRequest","RemoveCommerceItemResponse","RemoveCommerceLocationRequest","RemoveCommerceLocationResponse","RemoveCrmCompanyRequest","RemoveCrmCompanyResponse","RemoveCrmContactRequest","RemoveCrmContactResponse","RemoveCrmDealRequest","RemoveCrmDealResponse","RemoveCrmEventRequest","RemoveCrmEventResponse","RemoveCrmLeadRequest","RemoveCrmLeadResponse","RemoveCrmPipelineRequest","RemoveCrmPipelineResponse","RemoveHrisEmployeeRequest","RemoveHrisEmployeeResponse","RemoveHrisGroupRequest","RemoveHrisGroupResponse","RemoveMartechListRequest","RemoveMartechListResponse","RemoveMartechMemberRequest","RemoveMartechMemberResponse","RemovePassthroughRequest","RemovePassthroughResponse","RemovePaymentLinkRequest","RemovePaymentLinkResponse","RemovePaymentPaymentRequest","RemovePaymentPaymentResponse","RemoveStorageFileRequest","RemoveStorageFileResponse","RemoveTicketingCustomerRequest","RemoveTicketingCustomerResponse","RemoveTicketingNoteRequest","RemoveTicketingNoteResponse","RemoveTicketingTicketRequest","RemoveTicketingTicketResponse","RemoveUcContactRequest","RemoveUcContactResponse","RemoveUnifiedConnectionRequest","RemoveUnifiedConnectionResponse","RemoveUnifiedWebhookRequest","RemoveUnifiedWebhookResponse","Scopes","UpdateAccountingAccountRequest","UpdateAccountingAccountResponse","UpdateAccountingContactRequest","UpdateAccountingContactResponse","UpdateAccountingInvoiceRequest","UpdateAccountingInvoiceResponse","UpdateAccountingTaxrateRequest","UpdateAccountingTaxrateResponse","UpdateAccountingTransactionRequest","UpdateAccountingTransactionResponse","UpdateAtsActivityRequest","UpdateAtsActivityResponse","UpdateAtsApplicationRequest","UpdateAtsApplicationResponse","UpdateAtsCandidateRequest","UpdateAtsCandidateResponse","UpdateAtsDocumentRequest","UpdateAtsDocumentResponse","UpdateAtsInterviewRequest","UpdateAtsInterviewResponse","UpdateAtsJobRequest","UpdateAtsJobResponse","UpdateAtsScorecardRequest","UpdateAtsScorecardResponse","UpdateCommerceCollectionRequest","UpdateCommerceCollectionResponse","UpdateCommerceInventoryRequest","UpdateCommerceInventoryResponse","UpdateCommerceItemRequest","UpdateCommerceItemResponse","UpdateCommerceLocationRequest","UpdateCommerceLocationResponse","UpdateCrmCompanyRequest","UpdateCrmCompanyResponse","UpdateCrmContactRequest","UpdateCrmContactResponse","UpdateCrmDealRequest","UpdateCrmDealResponse","UpdateCrmEventRequest","UpdateCrmEventResponse","UpdateCrmLeadRequest","UpdateCrmLeadResponse","UpdateCrmPipelineRequest","UpdateCrmPipelineResponse","UpdateHrisEmployeeRequest","UpdateHrisEmployeeResponse","UpdateHrisGroupRequest","UpdateHrisGroupResponse","UpdateMartechListRequest","UpdateMartechListResponse","UpdateMartechMemberRequest","UpdateMartechMemberResponse","UpdatePassthroughRequest","UpdatePassthroughResponse","UpdatePaymentLinkRequest","UpdatePaymentLinkResponse","UpdatePaymentPaymentRequest","UpdatePaymentPaymentResponse","UpdateStorageFileRequest","UpdateStorageFileResponse","UpdateTicketingCustomerRequest","UpdateTicketingCustomerResponse","UpdateTicketingNoteRequest","UpdateTicketingNoteResponse","UpdateTicketingTicketRequest","UpdateTicketingTicketResponse","UpdateUcContactRequest","UpdateUcContactResponse","UpdateUnifiedConnectionRequest","UpdateUnifiedConnectionResponse","UpdateUnifiedWebhookTriggerRequest","UpdateUnifiedWebhookTriggerResponse"]
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountingaccount.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountingcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountinginvoice.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountingtaxrate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createaccountingtransaction.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsactivity.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsapplication.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatscandidate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsdocument.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsinterview.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsjob.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createatsscorecard.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcommercecollection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcommerceinventory.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcommerceitem.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcommercelocation.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmcompany.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmdeal.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmevent.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmlead.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createcrmpipeline.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createcrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createhrisemployee.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createhrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createhrisgroup.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createhrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createmartechlist.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createmartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createmartechmember.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createmartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createpassthrough.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createpassthrough.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createpaymentlink.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createpaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createpaymentpayment.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createpaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createstoragefile.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createstoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createticketingcustomer.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createticketingnote.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createticketingticket.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createuccontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createunifiedconnection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/createunifiedwebhook.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/createunifiedwebhook.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingaccount.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountinginvoice.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingorganization.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingorganization.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingtaxrate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getaccountingtransaction.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsactivity.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsapplication.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatscandidate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatscompany.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatscompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsdocument.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsinterview.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsjob.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getatsscorecard.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcommercecollection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcommerceinventory.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcommerceitem.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcommercelocation.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmcompany.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmdeal.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmevent.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmlead.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getcrmpipeline.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getcrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/gethrisemployee.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/gethrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/gethrisgroup.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/gethrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/gethrispayslip.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/gethrispayslip.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/gethristimeoff.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/gethristimeoff.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getmartechlist.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getmartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getmartechmember.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getmartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getpaymentlink.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getpaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getpaymentpayment.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getpaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getpaymentpayout.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getpaymentpayout.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getpaymentrefund.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getpaymentrefund.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getstoragefile.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getstoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getticketingcustomer.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getticketingnote.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getticketingticket.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getuccontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedapicall.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedapicall.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedconnection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedintegrationauth.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedintegrationauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,17 @@
     HRIS_PAYSLIP_WRITE = 'hris_payslip_write'
     HRIS_TIMEOFF_READ = 'hris_timeoff_read'
     HRIS_TIMEOFF_WRITE = 'hris_timeoff_write'
     UC_CALL_READ = 'uc_call_read'
     STORAGE_FILE_READ = 'storage_file_read'
     STORAGE_FILE_WRITE = 'storage_file_write'
     WEBHOOK = 'webhook'
+    GENAI_MODEL_READ = 'genai_model_read'
+    GENAI_PROMPT_READ = 'genai_prompt_read'
+    GENAI_PROMPT_WRITE = 'genai_prompt_write'
 
 
 @dataclasses.dataclass
 class GetUnifiedIntegrationAuthRequest:
     integration_type: str = dataclasses.field(metadata={'path_param': { 'field_name': 'integration_type', 'style': 'simple', 'explode': False }})
     r"""Type of the supported integration"""
     workspace_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'workspace_id', 'style': 'simple', 'explode': False }})
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedintegrationlogin.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedintegrationlogin.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/getunifiedwebhook.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/getunifiedwebhook.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingaccounts.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingaccounts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingcontacts.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingcontacts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountinginvoices.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountinginvoices.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingorganizations.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingorganizations.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingtaxrates.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingtaxrates.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listaccountingtransactions.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listaccountingtransactions.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsactivities.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsactivities.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsapplications.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsapplications.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsapplicationstatuses.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsapplicationstatuses.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatscandidates.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatscandidates.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatscompanies.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatscompanies.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsdocuments.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsdocuments.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsinterviews.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsinterviews.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsjobs.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsjobs.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listatsscorecards.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listatsscorecards.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcommercecollections.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcommercecollections.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcommerceinventories.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcommerceinventories.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcommerceitems.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcommerceitems.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcommercelocations.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcommercelocations.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmcompanies.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmcompanies.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmcontacts.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmcontacts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmdeals.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmdeals.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmevents.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmevents.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmleads.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmleads.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listcrmpipelines.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listcrmpipelines.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listenrichcompanies.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listenrichcompanies.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listenrichpeople.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listenrichpeople.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listhrisemployees.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listhrisemployees.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listhrisgroups.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listhrisgroups.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listhrispayslips.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listhrispayslips.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listhristimeoffs.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listhristimeoffs.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listmartechlists.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listmartechlists.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listmartechmembers.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listmartechmembers.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpassthroughs.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpassthroughs.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpaymentlinks.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpaymentlinks.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpaymentpayments.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpaymentpayments.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpaymentpayouts.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpaymentpayouts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listpaymentrefunds.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listpaymentrefunds.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/liststoragefiles.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/liststoragefiles.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listticketingcustomers.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listticketingcustomers.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listticketingnotes.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listticketingnotes.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listticketingtickets.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listticketingtickets.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listuccalls.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listuccalls.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listuccontacts.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listuccontacts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedapicalls.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedapicalls.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedconnections.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedconnections.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     MARTECH = 'martech'
     TICKETING = 'ticketing'
     UC = 'uc'
     ACCOUNTING = 'accounting'
     STORAGE = 'storage'
     COMMERCE = 'commerce'
     PAYMENT = 'payment'
+    GENAI = 'genai'
 
 
 @dataclasses.dataclass
 class ListUnifiedConnectionsRequest:
     categories: Optional[List[Categories]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'categories', 'style': 'form', 'explode': True }})
     r"""Filter the results on these categories"""
     env: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'env', 'style': 'form', 'explode': True }})
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedintegrations.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedintegrations.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     MARTECH = 'martech'
     TICKETING = 'ticketing'
     UC = 'uc'
     ACCOUNTING = 'accounting'
     STORAGE = 'storage'
     COMMERCE = 'commerce'
     PAYMENT = 'payment'
+    GENAI = 'genai'
 
 
 @dataclasses.dataclass
 class ListUnifiedIntegrationsRequest:
     active: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'active', 'style': 'form', 'explode': True }})
     r"""Filter the results for only the workspace's active integrations"""
     categories: Optional[List[ListUnifiedIntegrationsQueryParamCategories]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'categories', 'style': 'form', 'explode': True }})
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedintegrationworkspaces.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedintegrationworkspaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     MARTECH = 'martech'
     TICKETING = 'ticketing'
     UC = 'uc'
     ACCOUNTING = 'accounting'
     STORAGE = 'storage'
     COMMERCE = 'commerce'
     PAYMENT = 'payment'
+    GENAI = 'genai'
 
 
 @dataclasses.dataclass
 class ListUnifiedIntegrationWorkspacesRequest:
     workspace_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'workspace_id', 'style': 'simple', 'explode': False }})
     r"""The ID of the workspace"""
     active: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'active', 'style': 'form', 'explode': True }})
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedissues.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedissues.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedsupports.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedsupports.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/listunifiedwebhooks.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/listunifiedwebhooks.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountingaccount.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountingcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountinginvoice.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountingtaxrate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchaccountingtransaction.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsactivity.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsapplication.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatscandidate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsdocument.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsinterview.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsjob.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchatsscorecard.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcommercecollection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcommerceinventory.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcommerceitem.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcommercelocation.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmcompany.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmdeal.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmevent.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmlead.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchcrmpipeline.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchcrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchhrisemployee.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchhrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchhrisgroup.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchhrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchmartechlist.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchmartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchmartechmember.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchmartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchpassthrough.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchpassthrough.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchpaymentlink.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchpaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchpaymentpayment.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchpaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchstoragefile.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchstoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchticketingcustomer.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchticketingnote.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchticketingticket.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchuccontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchunifiedconnection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/patchunifiedwebhooktrigger.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/patchunifiedwebhooktrigger.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountingaccount.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountingcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountinginvoice.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountingtaxrate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeaccountingtransaction.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsactivity.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsapplication.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatscandidate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsdocument.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsinterview.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsjob.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeatsscorecard.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecommercecollection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecommerceinventory.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecommerceitem.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecommercelocation.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmcompany.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmdeal.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmevent.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmlead.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removecrmpipeline.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removecrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removehrisemployee.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removehrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removehrisgroup.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removehrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removemartechlist.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removemartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removemartechmember.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removemartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removepassthrough.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removepassthrough.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removepaymentlink.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removepaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removepaymentpayment.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removepaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removestoragefile.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removestoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeticketingcustomer.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeticketingnote.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeticketingticket.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeuccontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeunifiedconnection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/removeunifiedwebhook.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/removeunifiedwebhook.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountingaccount.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountingcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountinginvoice.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountingtaxrate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateaccountingtransaction.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsactivity.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsapplication.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatscandidate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsdocument.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsinterview.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsjob.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateatsscorecard.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecommercecollection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecommerceinventory.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecommerceitem.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecommercelocation.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmcompany.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmdeal.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmevent.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmlead.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatecrmpipeline.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatecrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatehrisemployee.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatehrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatehrisgroup.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatehrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatemartechlist.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatemartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatemartechmember.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatemartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatepassthrough.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatepassthrough.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatepaymentlink.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatepaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatepaymentpayment.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatepaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updatestoragefile.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updatestoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateticketingcustomer.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateticketingnote.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateticketingticket.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateuccontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateunifiedconnection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/operations/updateunifiedwebhooktrigger.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/operations/updateunifiedwebhooktrigger.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/__init__.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 from .crmpipeline import *
 from .crmtelephone import *
 from .enrichcompany import *
 from .enrichemail import *
 from .enrichperson import *
 from .enrichpersonworkhistory import *
 from .enrichtelephone import *
+from .genaicontent import *
+from .genaimodel import *
+from .genaiprompt import *
 from .hrisemail import *
 from .hrisemployee import *
 from .hrisgroup import *
 from .hrispayslip import *
 from .hrispayslipdetail import *
 from .hristelephone import *
 from .hristimeoff import *
@@ -106,8 +109,8 @@
 from .uccall import *
 from .uccontact import *
 from .ucemail import *
 from .uctelephone import *
 from .undefined import *
 from .webhook import *
 
-__all__ = ["APICall","APICallType","AccountingAccount","AccountingContact","AccountingContactPaymentMethod","AccountingContactPaymentMethodType","AccountingEmail","AccountingEmailType","AccountingInvoice","AccountingInvoiceStatus","AccountingLineitem","AccountingOrganization","AccountingTaxrate","AccountingTelephone","AccountingTelephoneType","AccountingTransaction","AccountingTransactionLineitem","AtsActivity","AtsActivityType","AtsAddress","AtsApplication","AtsApplicationAnswer","AtsApplicationStatus","AtsCandidate","AtsCompany","AtsCompensation","AtsCompensationType","AtsDocument","AtsDocumentType","AtsEmail","AtsEmailType","AtsInterview","AtsInterviewStatus","AtsJob","AtsJobQuestion","AtsJobQuestionType","AtsJobStatus","AtsScorecard","AtsScorecardQuestion","AtsStatus","AtsStatusStatus","AtsTelephone","AtsTelephoneType","CommerceCollection","CommerceCollectionType","CommerceInventory","CommerceItem","CommerceItemMedia","CommerceItemMediaType","CommerceItemOption","CommerceItemPrice","CommerceItemVariant","CommerceLocation","Connection","CrmCompany","CrmContact","CrmDeal","CrmEmail","CrmEmailType","CrmEvent","CrmEventType","CrmLead","CrmPipeline","CrmTelephone","CrmTelephoneType","EmploymentStatus","EmploymentType","EnrichCompany","EnrichEmail","EnrichEmailType","EnrichPerson","EnrichPersonWorkHistory","EnrichTelephone","EnrichTelephoneType","Event","Frequency","Gender","HrisEmail","HrisEmailType","HrisEmployee","HrisEmployeeEmploymentType","HrisEmployeeGender","HrisGroup","HrisGroupType","HrisPayslip","HrisPayslipDetail","HrisPayslipDetailType","HrisTelephone","HrisTelephoneType","HrisTimeoff","HrisTimeoffStatus","HrisTimeoffType","Integration","IntegrationSupport","Issue","IssueStatus","IssueType","MaritalStatus","MarketingEmail","MarketingEmailType","MarketingList","MarketingMember","ObjectType","Origin","PaymentCollectionMethod","PaymentLink","PaymentLinkLineitem","PaymentPayment","PaymentPayout","PaymentPayoutStatus","PaymentRefund","PaymentRefundStatus","PaymentType","PropertyAccountingContactBillingAddress","PropertyAccountingContactShippingAddress","PropertyAccountingOrganizationAddress","PropertyAtsCandidateAddress","PropertyAtsCompanyAddress","PropertyCommerceLocationAddress","PropertyConnectionAuth","PropertyConnectionCategories","PropertyConnectionPermissions","PropertyCrmCompanyAddress","PropertyCrmContactAddress","PropertyCrmEventCall","PropertyCrmEventEmail","PropertyCrmEventMeeting","PropertyCrmEventNote","PropertyCrmEventTask","PropertyCrmEventTaskStatus","PropertyCrmLeadAddress","PropertyEnrichCompanyAddress","PropertyEnrichPersonAddress","PropertyHrisEmployeeAddress","PropertyIntegrationCategories","PropertyIntegrationSupportWebhookEvents","PropertyPropertyIntegrationSupportWebhookEventsCreated","PropertyPropertyIntegrationSupportWebhookEventsDeleted","PropertyPropertyIntegrationSupportWebhookEventsUpdated","PropertyStoragePermissionRoles","PropertyUcCallTelephone","PropertyUcCallTelephoneType","Recommendation","Security","SizeUnit","Status","StorageFile","StorageFileType","StoragePermission","TaxExemption","TicketingCustomer","TicketingEmail","TicketingEmailType","TicketingNote","TicketingTelephone","TicketingTelephoneType","TicketingTicket","TicketingTicketStatus","Type","UcCall","UcContact","UcEmail","UcEmailType","UcTelephone","UcTelephoneType","UndefinedT","Webhook","WebhookType","WeightUnit"]
+__all__ = ["APICall","APICallType","AccountingAccount","AccountingContact","AccountingContactPaymentMethod","AccountingContactPaymentMethodType","AccountingEmail","AccountingEmailType","AccountingInvoice","AccountingInvoiceStatus","AccountingLineitem","AccountingOrganization","AccountingTaxrate","AccountingTelephone","AccountingTelephoneType","AccountingTransaction","AccountingTransactionLineitem","AtsActivity","AtsActivityType","AtsAddress","AtsApplication","AtsApplicationAnswer","AtsApplicationStatus","AtsCandidate","AtsCompany","AtsCompensation","AtsCompensationType","AtsDocument","AtsDocumentType","AtsEmail","AtsEmailType","AtsInterview","AtsInterviewStatus","AtsJob","AtsJobQuestion","AtsJobQuestionType","AtsJobStatus","AtsScorecard","AtsScorecardQuestion","AtsStatus","AtsStatusStatus","AtsTelephone","AtsTelephoneType","CommerceCollection","CommerceCollectionType","CommerceInventory","CommerceItem","CommerceItemMedia","CommerceItemMediaType","CommerceItemOption","CommerceItemPrice","CommerceItemVariant","CommerceLocation","Connection","CrmCompany","CrmContact","CrmDeal","CrmEmail","CrmEmailType","CrmEvent","CrmEventType","CrmLead","CrmPipeline","CrmTelephone","CrmTelephoneType","EmploymentStatus","EmploymentType","EnrichCompany","EnrichEmail","EnrichEmailType","EnrichPerson","EnrichPersonWorkHistory","EnrichTelephone","EnrichTelephoneType","Event","Frequency","GenaiContent","GenaiModel","GenaiPrompt","Gender","HrisEmail","HrisEmailType","HrisEmployee","HrisEmployeeEmploymentType","HrisEmployeeGender","HrisGroup","HrisGroupType","HrisPayslip","HrisPayslipDetail","HrisPayslipDetailType","HrisTelephone","HrisTelephoneType","HrisTimeoff","HrisTimeoffStatus","HrisTimeoffType","Integration","IntegrationSupport","Issue","IssueStatus","IssueType","MaritalStatus","MarketingEmail","MarketingEmailType","MarketingList","MarketingMember","ObjectType","Origin","PaymentCollectionMethod","PaymentLink","PaymentLinkLineitem","PaymentPayment","PaymentPayout","PaymentPayoutStatus","PaymentRefund","PaymentRefundStatus","PaymentType","PropertyAccountingContactBillingAddress","PropertyAccountingContactShippingAddress","PropertyAccountingOrganizationAddress","PropertyAtsCandidateAddress","PropertyAtsCompanyAddress","PropertyCommerceLocationAddress","PropertyConnectionAuth","PropertyConnectionCategories","PropertyConnectionPermissions","PropertyCrmCompanyAddress","PropertyCrmContactAddress","PropertyCrmEventCall","PropertyCrmEventEmail","PropertyCrmEventMeeting","PropertyCrmEventNote","PropertyCrmEventTask","PropertyCrmEventTaskStatus","PropertyCrmLeadAddress","PropertyEnrichCompanyAddress","PropertyEnrichPersonAddress","PropertyHrisEmployeeAddress","PropertyIntegrationCategories","PropertyIntegrationSupportWebhookEvents","PropertyPropertyIntegrationSupportWebhookEventsCreated","PropertyPropertyIntegrationSupportWebhookEventsDeleted","PropertyPropertyIntegrationSupportWebhookEventsUpdated","PropertyStoragePermissionRoles","PropertyUcCallTelephone","PropertyUcCallTelephoneType","Recommendation","Role","Security","SizeUnit","Status","StorageFile","StorageFileType","StoragePermission","TaxExemption","TicketingCustomer","TicketingEmail","TicketingEmailType","TicketingNote","TicketingTelephone","TicketingTelephoneType","TicketingTicket","TicketingTicketStatus","Type","UcCall","UcContact","UcEmail","UcEmailType","UcTelephone","UcTelephoneType","UndefinedT","Webhook","WebhookType","WeightUnit"]
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingaccount.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingcontactpaymentmethod.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingcontactpaymentmethod.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingemail.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountinginvoice.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountinglineitem.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountinglineitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingorganization.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingorganization.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingtaxrate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingtelephone.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingtelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingtransaction.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/accountingtransactionlineitem.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/accountingtransactionlineitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/apicall.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/apicall.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsactivity.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsaddress.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsaddress.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsapplication.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsapplicationanswer.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsapplicationanswer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atscandidate.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atscompany.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atscompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atscompensation.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atscompensation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsdocument.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsemail.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsinterview.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsjob.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsjobquestion.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsjobquestion.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsscorecard.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsscorecardquestion.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsscorecardquestion.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atsstatus.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atsstatus.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/atstelephone.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/atstelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/commercecollection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/commercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceinventory.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitem.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitemmedia.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitemmedia.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitemoption.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitemoption.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitemprice.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitemprice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/commerceitemvariant.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/commerceitemvariant.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/commercelocation.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/commercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/connection.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/connection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmcompany.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmcontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmdeal.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmemail.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmevent.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmlead.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmpipeline.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/crmtelephone.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/crmtelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichcompany.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichemail.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichperson.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichperson.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichpersonworkhistory.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichpersonworkhistory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/enrichtelephone.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/enrichtelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrisemail.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrisemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrisemployee.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrisgroup.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrispayslip.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrispayslip.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/hrispayslipdetail.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/hrispayslipdetail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/hristelephone.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/hristelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/hristimeoff.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/hristimeoff.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/integration.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/integration.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/integrationsupport.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/integrationsupport.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/issue.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/issue.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/marketingemail.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/marketingemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/marketinglist.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/marketinglist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/marketingmember.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/marketingmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentlink.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentlinklineitem.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentlinklineitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentpayment.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentpayout.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentpayout.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/paymentrefund.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/paymentrefund.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_accountingcontact_billing_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_accountingcontact_billing_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_accountingcontact_shipping_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_accountingcontact_shipping_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_accountingorganization_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_accountingorganization_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_atscandidate_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_atscandidate_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_atscompany_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_atscompany_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_commercelocation_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_commercelocation_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_connection_auth.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_connection_auth.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_connection_permissions.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_connection_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,7 +76,10 @@
     HRIS_PAYSLIP_WRITE = 'hris_payslip_write'
     HRIS_TIMEOFF_READ = 'hris_timeoff_read'
     HRIS_TIMEOFF_WRITE = 'hris_timeoff_write'
     UC_CALL_READ = 'uc_call_read'
     STORAGE_FILE_READ = 'storage_file_read'
     STORAGE_FILE_WRITE = 'storage_file_write'
     WEBHOOK = 'webhook'
+    GENAI_MODEL_READ = 'genai_model_read'
+    GENAI_PROMPT_READ = 'genai_prompt_read'
+    GENAI_PROMPT_WRITE = 'genai_prompt_write'
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmcompany_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmcompany_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmcontact_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmcontact_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_call.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_call.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_email.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_email.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_meeting.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_meeting.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_note.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_note.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmevent_task.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmevent_task.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_crmlead_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_crmlead_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_enrichcompany_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_enrichcompany_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_enrichperson_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_enrichperson_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_hrisemployee_address.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_hrisemployee_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_integrationsupport_webhook_events.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_integrationsupport_webhook_events.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/property_uccall_telephone.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/property_uccall_telephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/storagefile.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/storagefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/storagepermission.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/storagepermission.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingcustomer.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingemail.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingnote.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingtelephone.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingtelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/ticketingticket.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/ticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/uccall.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/uccall.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/uccontact.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/uccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/ucemail.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/ucemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/uctelephone.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/uctelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/undefined.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/undefined.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/models/shared/webhook.py` & `Unified-python-sdk-0.22.0/src/unified_to/models/shared/webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     TICKETING_TICKET = 'ticketing_ticket'
     TICKETING_CUSTOMER = 'ticketing_customer'
     UC_CONTACT = 'uc_contact'
     UC_CALL = 'uc_call'
     ENRICH_PERSON = 'enrich_person'
     ENRICH_COMPANY = 'enrich_company'
     STORAGE_FILE = 'storage_file'
+    GENAI_MODEL = 'genai_model'
+    GENAI_PROMPT = 'genai_prompt'
 
 class WebhookType(str, Enum):
     VIRTUAL = 'virtual'
     NATIVE = 'native'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/note.py` & `Unified-python-sdk-0.22.0/src/unified_to/note.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingNote])
                 res.ticketing_note = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingNote])
                 res.ticketing_note = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTicketingNotesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.TicketingNote]])
                 res.ticketing_notes = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingNote])
                 res.ticketing_note = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingNote])
                 res.ticketing_note = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/organization.py` & `Unified-python-sdk-0.22.0/src/unified_to/organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingOrganizationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingOrganization])
                 res.accounting_organization = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -106,14 +107,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingOrganizationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingOrganization]])
                 res.accounting_organizations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/passthrough.py` & `Unified-python-sdk-0.22.0/src/unified_to/passthrough.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreatePassthroughResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[Dict[str, Any]])
                 res.result = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -107,14 +108,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPassthroughsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[Dict[str, Any]])
                 res.result = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -164,14 +166,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchPassthroughResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[Dict[str, Any]])
                 res.result = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -218,14 +221,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.RemovePassthroughResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[Dict[str, Any]])
                 res.result = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -275,14 +279,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdatePassthroughResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[Dict[str, Any]])
                 res.result = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/payment.py` & `Unified-python-sdk-0.22.0/src/unified_to/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreatePaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
                 res.payment_link = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,14 +111,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreatePaymentPaymentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentPayment])
                 res.payment_payment = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -165,14 +167,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
                 res.payment_link = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPaymentPaymentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentPayment])
                 res.payment_payment = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -275,14 +279,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPaymentPayoutResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentPayout])
                 res.payment_payout = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -330,14 +335,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPaymentRefundResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentRefund])
                 res.payment_refund = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -385,14 +391,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPaymentLinksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.PaymentLink]])
                 res.payment_links = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -440,14 +447,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPaymentPaymentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.PaymentPayment]])
                 res.payment_payments = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -495,14 +503,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPaymentPayoutsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.PaymentPayout]])
                 res.payment_payouts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -550,14 +559,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPaymentRefundsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.PaymentRefund]])
                 res.payment_refunds = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -607,14 +617,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchPaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
                 res.payment_link = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -664,14 +675,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchPaymentPaymentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentPayment])
                 res.payment_payment = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -722,14 +734,15 @@
         res = operations.RemovePaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -776,14 +789,15 @@
         res = operations.RemovePaymentPaymentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -829,14 +843,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdatePaymentLinkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentLink])
                 res.payment_link = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -886,14 +901,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdatePaymentPaymentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentPayment])
                 res.payment_payment = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/payout.py` & `Unified-python-sdk-0.22.0/src/unified_to/payout.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPaymentPayoutResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentPayout])
                 res.payment_payout = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -106,14 +107,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPaymentPayoutsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.PaymentPayout]])
                 res.payment_payouts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/payslip.py` & `Unified-python-sdk-0.22.0/src/unified_to/payslip.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetHrisPayslipResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisPayslip])
                 res.hris_payslip = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -106,14 +107,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListHrisPayslipsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.HrisPayslip]])
                 res.hris_payslips = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/person.py` & `Unified-python-sdk-0.22.0/src/unified_to/person.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListEnrichPeopleResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.EnrichPerson])
                 res.enrich_person = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/pipeline.py` & `Unified-python-sdk-0.22.0/src/unified_to/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmPipeline])
                 res.crm_pipeline = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmPipeline])
                 res.crm_pipeline = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListCrmPipelinesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CrmPipeline]])
                 res.crm_pipelines = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmPipeline])
                 res.crm_pipeline = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateCrmPipelineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CrmPipeline])
                 res.crm_pipeline = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/refund.py` & `Unified-python-sdk-0.22.0/src/unified_to/refund.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPaymentRefundResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentRefund])
                 res.payment_refund = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -106,14 +107,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPaymentRefundsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.PaymentRefund]])
                 res.payment_refunds = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/scorecard.py` & `Unified-python-sdk-0.22.0/src/unified_to/scorecard.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsScorecard])
                 res.ats_scorecard = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsScorecard])
                 res.ats_scorecard = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAtsScorecardsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AtsScorecard]])
                 res.ats_scorecards = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsScorecard])
                 res.ats_scorecard = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAtsScorecardResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AtsScorecard])
                 res.ats_scorecard = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/sdk.py` & `Unified-python-sdk-0.22.0/src/unified_to/sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .customer import Customer
 from .deal import Deal
 from .document import Document
 from .employee import Employee
 from .enrich import Enrich
 from .event import Event
 from .file import File
+from .genai import Genai
 from .group import Group
 from .hris import Hris
 from .integration import Integration
 from .interview import Interview
 from .inventory import Inventory
 from .invoice import Invoice
 from .issue import Issue
@@ -36,22 +37,24 @@
 from .lead import Lead
 from .link import Link
 from .list import ListT
 from .location import Location
 from .login import Login
 from .martech import Martech
 from .member import Member
+from .model import Model
 from .note import Note
 from .organization import Organization
 from .passthrough import Passthrough
 from .payment import Payment
 from .payout import Payout
 from .payslip import Payslip
 from .person import Person
 from .pipeline import Pipeline
+from .prompt import Prompt
 from .refund import Refund
 from .scorecard import Scorecard
 from .sdkconfiguration import SDKConfiguration
 from .storage import Storage
 from .taxrate import Taxrate
 from .ticket import Ticket
 from .ticketing import Ticketing
@@ -93,14 +96,17 @@
     crm: Crm
     deal: Deal
     event: Event
     lead: Lead
     pipeline: Pipeline
     enrich: Enrich
     person: Person
+    genai: Genai
+    model: Model
+    prompt: Prompt
     hris: Hris
     employee: Employee
     group: Group
     payslip: Payslip
     timeoff: Timeoff
     martech: Martech
     list: ListT
@@ -207,14 +213,17 @@
         self.crm = Crm(self.sdk_configuration)
         self.deal = Deal(self.sdk_configuration)
         self.event = Event(self.sdk_configuration)
         self.lead = Lead(self.sdk_configuration)
         self.pipeline = Pipeline(self.sdk_configuration)
         self.enrich = Enrich(self.sdk_configuration)
         self.person = Person(self.sdk_configuration)
+        self.genai = Genai(self.sdk_configuration)
+        self.model = Model(self.sdk_configuration)
+        self.prompt = Prompt(self.sdk_configuration)
         self.hris = Hris(self.sdk_configuration)
         self.employee = Employee(self.sdk_configuration)
         self.group = Group(self.sdk_configuration)
         self.payslip = Payslip(self.sdk_configuration)
         self.timeoff = Timeoff(self.sdk_configuration)
         self.martech = Martech(self.sdk_configuration)
         self.list = ListT(self.sdk_configuration)
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/sdkconfiguration.py` & `Unified-python-sdk-0.22.0/src/unified_to/sdkconfiguration.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0'
-    sdk_version: str = '0.21.9'
-    gen_version: str = '2.314.0'
-    user_agent: str = 'speakeasy-sdk/python 0.21.9 2.314.0 1.0 Unified-python-sdk'
+    sdk_version: str = '0.22.0'
+    gen_version: str = '2.326.3'
+    user_agent: str = 'speakeasy-sdk/python 0.22.0 2.326.3 1.0 Unified-python-sdk'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/storage.py` & `Unified-python-sdk-0.22.0/src/unified_to/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.StorageFile])
                 res.storage_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.StorageFile])
                 res.storage_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListStorageFilesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.StorageFile]])
                 res.storage_files = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.StorageFile])
                 res.storage_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateStorageFileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.StorageFile])
                 res.storage_file = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/taxrate.py` & `Unified-python-sdk-0.22.0/src/unified_to/taxrate.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTaxrate])
                 res.accounting_taxrate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTaxrate])
                 res.accounting_taxrate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingTaxratesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingTaxrate]])
                 res.accounting_taxrates = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTaxrate])
                 res.accounting_taxrate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingTaxrateResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTaxrate])
                 res.accounting_taxrate = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/ticket.py` & `Unified-python-sdk-0.22.0/src/unified_to/ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingTicket])
                 res.ticketing_ticket = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingTicket])
                 res.ticketing_ticket = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTicketingTicketsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.TicketingTicket]])
                 res.ticketing_tickets = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingTicket])
                 res.ticketing_ticket = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingTicket])
                 res.ticketing_ticket = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/ticketing.py` & `Unified-python-sdk-0.22.0/src/unified_to/ticketing.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingCustomer])
                 res.ticketing_customer = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -110,14 +111,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingNote])
                 res.ticketing_note = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -167,14 +169,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingTicket])
                 res.ticketing_ticket = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -222,14 +225,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingCustomer])
                 res.ticketing_customer = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -277,14 +281,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingNote])
                 res.ticketing_note = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -332,14 +337,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingTicket])
                 res.ticketing_ticket = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -387,14 +393,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTicketingCustomersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.TicketingCustomer]])
                 res.ticketing_customers = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -442,14 +449,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTicketingNotesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.TicketingNote]])
                 res.ticketing_notes = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -497,14 +505,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTicketingTicketsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.TicketingTicket]])
                 res.ticketing_tickets = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -554,14 +563,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingCustomer])
                 res.ticketing_customer = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -611,14 +621,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingNote])
                 res.ticketing_note = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -668,14 +679,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingTicket])
                 res.ticketing_ticket = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -726,14 +738,15 @@
         res = operations.RemoveTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -780,14 +793,15 @@
         res = operations.RemoveTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -834,14 +848,15 @@
         res = operations.RemoveTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -887,14 +902,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateTicketingCustomerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingCustomer])
                 res.ticketing_customer = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -944,14 +960,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateTicketingNoteResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingNote])
                 res.ticketing_note = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1001,14 +1018,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateTicketingTicketResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TicketingTicket])
                 res.ticketing_ticket = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/timeoff.py` & `Unified-python-sdk-0.22.0/src/unified_to/timeoff.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetHrisTimeoffResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.HrisTimeoff])
                 res.hris_timeoff = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -106,14 +107,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListHrisTimeoffsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.HrisTimeoff]])
                 res.hris_timeoffs = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/transaction.py` & `Unified-python-sdk-0.22.0/src/unified_to/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTransaction])
                 res.accounting_transaction = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTransaction])
                 res.accounting_transaction = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountingTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.AccountingTransaction]])
                 res.accounting_transactions = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -220,14 +223,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTransaction])
                 res.accounting_transaction = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
         res = operations.RemoveAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateAccountingTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountingTransaction])
                 res.accounting_transaction = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/uc.py` & `Unified-python-sdk-0.22.0/src/unified_to/uc.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UcContact])
                 res.uc_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UcContact])
                 res.uc_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -163,14 +165,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUcCallsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.UcCall]])
                 res.uc_calls = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -218,14 +221,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUcContactsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.UcContact]])
                 res.uc_contacts = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -275,14 +279,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UcContact])
                 res.uc_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -333,14 +338,15 @@
         res = operations.RemoveUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -386,14 +392,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateUcContactResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UcContact])
                 res.uc_contact = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/unified.py` & `Unified-python-sdk-0.22.0/src/unified_to/unified.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_unified_connection(self, request: Optional[shared.Connection]) -> operations.CreateUnifiedConnectionResponse:
+    def create_unified_connection(self, request: Optional[shared.Connection] = None) -> operations.CreateUnifiedConnectionResponse:
         r"""Create connection"""
         hook_ctx = HookContext(operation_id='createUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/unified/connection'
         
         if callable(self.sdk_configuration.security):
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -113,14 +114,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateUnifiedWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
                 res.webhook = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -167,14 +169,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedApicallResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.APICall])
                 res.api_call = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -221,14 +224,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -278,14 +282,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedIntegrationAuthResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'text/plain'):                
                 res.res = http_res.text
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -331,14 +336,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUnifiedWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
                 res.webhook = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -386,14 +392,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedApicallsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.APICall]])
                 res.api_calls = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -441,14 +448,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedConnectionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Connection]])
                 res.connections = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -498,14 +506,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedIntegrationWorkspacesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Integration]])
                 res.integrations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -553,14 +562,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedIntegrationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Integration]])
                 res.integrations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -608,14 +618,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedIssuesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Issue]])
                 res.issues = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -662,14 +673,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedSupportsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UndefinedT])
                 res.undefined = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -717,14 +729,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUnifiedWebhooksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Webhook]])
                 res.webhooks = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -774,14 +787,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PatchUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -832,14 +846,15 @@
         res = operations.PatchUnifiedWebhookTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -886,14 +901,15 @@
         res = operations.RemoveUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -940,14 +956,15 @@
         res = operations.RemoveUnifiedWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -993,14 +1010,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateUnifiedConnectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Connection])
                 res.connection = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -1051,14 +1069,15 @@
         res = operations.UpdateUnifiedWebhookTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/utils/retries.py` & `Unified-python-sdk-0.22.0/src/unified_to/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/utils/utils.py` & `Unified-python-sdk-0.22.0/src/unified_to/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -904,14 +904,41 @@
 
 
 def bigintdecoder(val):
     if isinstance(val, float):
         raise ValueError(f"{val} is a float")
     return int(val)
 
+def integerstrencoder(optional: bool):
+    def integerstrencode(val: int):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return integerstrencode
+
+
+def integerstrdecoder(val):
+    if isinstance(val, float):
+        raise ValueError(f"{val} is a float")
+    return int(val)
+
+
+def numberstrencoder(optional: bool):
+    def numberstrencode(val: float):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return numberstrencode
+
+
+def numberstrdecoder(val):
+    return float(val)
+
 
 def decimalencoder(optional: bool, as_str: bool):
     def decimalencode(val: Decimal):
         if optional and val is None:
             return None
 
         if as_str:
```

### Comparing `Unified-python-sdk-0.21.9/src/unified_to/webhook.py` & `Unified-python-sdk-0.22.0/src/unified_to/group.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,40 +3,37 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from typing import List, Optional
 from unified_to import utils
 from unified_to._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from unified_to.models import errors, operations, shared
 
-class Webhook:
+class Group:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_unified_webhook(self, request: operations.CreateUnifiedWebhookRequest) -> operations.CreateUnifiedWebhookResponse:
-        r"""Create webhook subscription
-        The data payload received by your server is described at https://docs.unified.to/unified/overview. The `interval` field can be set as low as 1 minute for paid accounts, and 60 minutes for free accounts.
-        """
-        hook_ctx = HookContext(operation_id='createUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def create_hris_group(self, request: operations.CreateHrisGroupRequest) -> operations.CreateHrisGroupResponse:
+        r"""Create a group"""
+        hook_ctx = HookContext(operation_id='createHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/unified/webhook'
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateUnifiedWebhookRequest, "webhook", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateHrisGroupRequest, "hris_group", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -53,44 +50,46 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.CreateUnifiedWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
-                res.webhook = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
+                res.hris_group = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_unified_webhook(self, request: operations.GetUnifiedWebhookRequest) -> operations.GetUnifiedWebhookResponse:
-        r"""Retrieve webhook by its ID"""
-        hook_ctx = HookContext(operation_id='getUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_hris_group(self, request: operations.GetHrisGroupRequest) -> operations.GetHrisGroupResponse:
+        r"""Retrieve a group"""
+        hook_ctx = HookContext(operation_id='getHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/unified/webhook/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -107,38 +106,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetUnifiedWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Webhook])
-                res.webhook = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
+                res.hris_group = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def list_unified_webhooks(self, request: operations.ListUnifiedWebhooksRequest) -> operations.ListUnifiedWebhooksResponse:
-        r"""Returns all registered webhooks"""
-        hook_ctx = HookContext(operation_id='listUnifiedWebhooks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def list_hris_groups(self, request: operations.ListHrisGroupsRequest) -> operations.ListHrisGroupsResponse:
+        r"""List all groups"""
+        hook_ctx = HookContext(operation_id='listHrisGroups', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/unified/webhook'
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         query_params = { **utils.get_query_params(request), **query_params }
@@ -162,50 +162,54 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.ListUnifiedWebhooksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.ListHrisGroupsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[shared.Webhook]])
-                res.webhooks = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[shared.HrisGroup]])
+                res.hris_groups = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def patch_unified_webhook_trigger(self, request: operations.PatchUnifiedWebhookTriggerRequest) -> operations.PatchUnifiedWebhookTriggerResponse:
-        r"""Trigger webhook"""
-        hook_ctx = HookContext(operation_id='patchUnifiedWebhookTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def patch_hris_group(self, request: operations.PatchHrisGroupRequest) -> operations.PatchHrisGroupResponse:
+        r"""Update a group"""
+        hook_ctx = HookContext(operation_id='patchHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/unified/webhook/{id}/trigger', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, operations.PatchHrisGroupRequest, "hris_group", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -216,38 +220,39 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.PatchUnifiedWebhookTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.PatchHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code >= 200 and http_res.status_code < 300:
-            pass
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
+        if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[str])
-                res.string = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
+                res.hris_group = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def remove_unified_webhook(self, request: operations.RemoveUnifiedWebhookRequest) -> operations.RemoveUnifiedWebhookResponse:
-        r"""Remove webhook subscription"""
-        hook_ctx = HookContext(operation_id='removeUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def remove_hris_group(self, request: operations.RemoveHrisGroupRequest) -> operations.RemoveHrisGroupResponse:
+        r"""Remove a group"""
+        hook_ctx = HookContext(operation_id='removeHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/unified/webhook/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -270,50 +275,54 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.RemoveUnifiedWebhookResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.RemoveHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[str])
                 res.string = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def update_unified_webhook_trigger(self, request: operations.UpdateUnifiedWebhookTriggerRequest) -> operations.UpdateUnifiedWebhookTriggerResponse:
-        r"""Trigger webhook"""
-        hook_ctx = HookContext(operation_id='updateUnifiedWebhookTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def update_hris_group(self, request: operations.UpdateHrisGroupRequest) -> operations.UpdateHrisGroupResponse:
+        r"""Update a group"""
+        hook_ctx = HookContext(operation_id='updateHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/unified/webhook/{id}/trigger', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateHrisGroupRequest, "hris_group", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -324,25 +333,26 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.UpdateUnifiedWebhookTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateHrisGroupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
-        if http_res.status_code >= 200 and http_res.status_code < 300:
-            pass
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
+        if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[str])
-                res.string = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.HrisGroup])
+                res.hris_group = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
```


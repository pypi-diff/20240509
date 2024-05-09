# Comparing `tmp/speakeasy-client-sdk-python-5.7.1.tar.gz` & `tmp/speakeasy-client-sdk-python-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-5.7.1.tar", last modified: Sat May  4 00:13:59 2024, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-5.8.0.tar", last modified: Thu May  9 00:12:31 2024, max compression
```

## Comparing `speakeasy-client-sdk-python-5.7.1.tar` & `speakeasy-client-sdk-python-5.8.0.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.132623 speakeasy-client-sdk-python-5.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-05-04 00:13:59.132623 speakeasy-client-sdk-python-5.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:13:59.132623 speakeasy-client-sdk-python-5.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.116623 speakeasy-client-sdk-python-5.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.120623 speakeasy-client-sdk-python-5.7.1/src/speakeasy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.120623 speakeasy-client-sdk-python-5.7.1/src/speakeasy/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28727 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/apiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    24256 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13901 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    16531 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.120623 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.120623 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.120623 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.128623 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/deleteapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/deleteapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/deleteschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/deleteversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/downloadschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/downloadschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/findapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generateopenapispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generatepostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getallapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getallapiversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getchangesreportsignedurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getlintingreportsignedurl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getnamespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getrequestfromeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getrevisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getschemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/gettags.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getworkspaceaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getworkspaceeventsbytarget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getworkspacetargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/insertversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/posttags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/postworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/preflight.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/queryeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/registerschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/searchworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/uploadreport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/upsertapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/upsertapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.132623 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/accessdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/addtags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/api_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/apiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/apiendpoint_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/boundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/clievent.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/embedtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/filter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/generateopenapispecdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/getnamespacesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/getrevisionsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/gettagsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/interactiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/preflightrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/preflighttoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/requestmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/schemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/targetsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/unboundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/v2descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/versionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/versionmetadata_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28253 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.132623 speakeasy-client-sdk-python-5.7.1/src/speakeasy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-04 00:13:50.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:13:59.132623 speakeasy-client-sdk-python-5.7.1/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-05-04 00:13:58.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-04 00:13:59.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:13:58.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-04 00:13:58.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 00:13:58.000000 speakeasy-client-sdk-python-5.7.1/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.636888 speakeasy-client-sdk-python-5.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-05-09 00:12:31.636888 speakeasy-client-sdk-python-5.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14717 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:12:31.636888 speakeasy-client-sdk-python-5.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.616888 speakeasy-client-sdk-python-5.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.616888 speakeasy-client-sdk-python-5.8.0/src/speakeasy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.620888 speakeasy-client-sdk-python-5.8.0/src/speakeasy/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29402 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/apiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22156 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16846 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10843 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.620888 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.620888 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.620888 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.628888 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/deleteapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/deleteapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/deleteschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/deleteversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/downloadschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/downloadschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/findapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generateopenapispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generatepostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getallapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getallapiversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getchangesreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getlintingreportsignedurl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getnamespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getrevisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getschemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/gettags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getworkspaceaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getworkspaceeventsbytarget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getworkspacetargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/insertversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/posttags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/postworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/preflight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/queryeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/registerschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/searchworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/uploadreport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/upsertapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/upsertapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.632888 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/accessdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/addtags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/api_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/apiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/apiendpoint_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/boundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20535 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/clievent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/embedtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/getnamespacesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/getrevisionsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/gettagsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/interactiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/preflightrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/preflighttoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/requestmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/schemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/targetsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/unboundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/v2descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/versionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/versionmetadata_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11614 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28973 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.632888 speakeasy-client-sdk-python-5.8.0/src/speakeasy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-09 00:12:23.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:12:31.636888 speakeasy-client-sdk-python-5.8.0/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-05-09 00:12:31.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-09 00:12:31.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:12:31.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-09 00:12:31.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 00:12:31.000000 speakeasy-client-sdk-python-5.8.0/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-5.7.1/PKG-INFO` & `speakeasy-client-sdk-python-5.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.7.1
+Version: 5.8.0
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -24,20 +24,17 @@
         import speakeasy
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.GetApisRequest()
-        
-        res = s.apis.get_apis(req)
+        res = s.apis.get_apis(request=operations.GetApisRequest())
         
         if res.apis is not None:
             # handle response
             pass
         
         ```
         <!-- End SDK Example Usage [usage] -->
@@ -151,24 +148,21 @@
         import speakeasy
         from speakeasy.models import errors, operations, shared
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
-        )
-        
-        req = operations.GetWorkspaceEventsByTargetRequest(
-            target_id='<value>',
         )
         
         res = None
         try:
-            res = s.events.get_workspace_events_by_target(req)
+            res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
+            target_id='<value>',
+        ))
         except errors.Error as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -199,23 +193,20 @@
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             server="prod",
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.DeleteAPIRequest(
+        res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
-        )
-        
-        res = s.apis.delete_api(req)
+        ))
         
         if res is not None:
             # handle response
             pass
         
         ```
         
@@ -228,23 +219,20 @@
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             server_url="https://api.prod.speakeasyapi.dev",
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.DeleteAPIRequest(
+        res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
-        )
-        
-        res = s.apis.delete_api(req)
+        ))
         
         if res is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -286,23 +274,20 @@
         import speakeasy
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.DeleteAPIRequest(
+        res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
-        )
-        
-        res = s.apis.delete_api(req)
+        ))
         
         if res is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
@@ -330,22 +315,19 @@
         import speakeasy
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceEventsByTargetRequest(
+        res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
             target_id='<value>',
-        )
-        
-        res = s.events.get_workspace_events_by_target(req)
+        ))
         
         if res.cli_event_batch is not None:
             # handle response
             pass
         
         ```
         <!-- End Global Parameters [global-parameters] -->
@@ -361,20 +343,17 @@
         from speakeasy.models import operations, shared
         from speakeasy.utils import BackoffStrategy, RetryConfig
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceAccessRequest()
-        
-        res = s.auth.get_workspace_access(req,
+        res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest(),
             RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False))
         
         if res.access_details is not None:
             # handle response
             pass
         
         ```
@@ -386,20 +365,17 @@
         from speakeasy.utils import BackoffStrategy, RetryConfig
         
         s = speakeasy.Speakeasy(
             retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False),
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceAccessRequest()
-        
-        res = s.auth.get_workspace_access(req)
+        res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest())
         
         if res.access_details is not None:
             # handle response
             pass
         
         ```
         <!-- End Retries [retries] -->
```

### Comparing `speakeasy-client-sdk-python-5.7.1/README.md` & `speakeasy-client-sdk-python-5.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,17 @@
 import speakeasy
 from speakeasy.models import operations, shared
 
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
-    workspace_id='<value>',
 )
 
-req = operations.GetApisRequest()
-
-res = s.apis.get_apis(req)
+res = s.apis.get_apis(request=operations.GetApisRequest())
 
 if res.apis is not None:
     # handle response
     pass
 
 ```
 <!-- End SDK Example Usage [usage] -->
@@ -144,24 +141,21 @@
 import speakeasy
 from speakeasy.models import errors, operations, shared
 
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
-    workspace_id='<value>',
-)
-
-req = operations.GetWorkspaceEventsByTargetRequest(
-    target_id='<value>',
 )
 
 res = None
 try:
-    res = s.events.get_workspace_events_by_target(req)
+    res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
+    target_id='<value>',
+))
 except errors.Error as e:
     # handle exception
     raise(e)
 except errors.SDKError as e:
     # handle exception
     raise(e)
 
@@ -192,23 +186,20 @@
 from speakeasy.models import operations, shared
 
 s = speakeasy.Speakeasy(
     server="prod",
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
-    workspace_id='<value>',
 )
 
-req = operations.DeleteAPIRequest(
+res = s.apis.delete_api(request=operations.DeleteAPIRequest(
     api_id='<value>',
     version_id='<value>',
-)
-
-res = s.apis.delete_api(req)
+))
 
 if res is not None:
     # handle response
     pass
 
 ```
 
@@ -221,23 +212,20 @@
 from speakeasy.models import operations, shared
 
 s = speakeasy.Speakeasy(
     server_url="https://api.prod.speakeasyapi.dev",
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
-    workspace_id='<value>',
 )
 
-req = operations.DeleteAPIRequest(
+res = s.apis.delete_api(request=operations.DeleteAPIRequest(
     api_id='<value>',
     version_id='<value>',
-)
-
-res = s.apis.delete_api(req)
+))
 
 if res is not None:
     # handle response
     pass
 
 ```
 <!-- End Server Selection [server] -->
@@ -279,23 +267,20 @@
 import speakeasy
 from speakeasy.models import operations, shared
 
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
-    workspace_id='<value>',
 )
 
-req = operations.DeleteAPIRequest(
+res = s.apis.delete_api(request=operations.DeleteAPIRequest(
     api_id='<value>',
     version_id='<value>',
-)
-
-res = s.apis.delete_api(req)
+))
 
 if res is not None:
     # handle response
     pass
 
 ```
 <!-- End Authentication [security] -->
@@ -323,22 +308,19 @@
 import speakeasy
 from speakeasy.models import operations, shared
 
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
-    workspace_id='<value>',
 )
 
-req = operations.GetWorkspaceEventsByTargetRequest(
+res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
     target_id='<value>',
-)
-
-res = s.events.get_workspace_events_by_target(req)
+))
 
 if res.cli_event_batch is not None:
     # handle response
     pass
 
 ```
 <!-- End Global Parameters [global-parameters] -->
@@ -354,20 +336,17 @@
 from speakeasy.models import operations, shared
 from speakeasy.utils import BackoffStrategy, RetryConfig
 
 s = speakeasy.Speakeasy(
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
-    workspace_id='<value>',
 )
 
-req = operations.GetWorkspaceAccessRequest()
-
-res = s.auth.get_workspace_access(req,
+res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest(),
     RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False))
 
 if res.access_details is not None:
     # handle response
     pass
 
 ```
@@ -379,20 +358,17 @@
 from speakeasy.utils import BackoffStrategy, RetryConfig
 
 s = speakeasy.Speakeasy(
     retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False),
     security=shared.Security(
         api_key="<YOUR_API_KEY_HERE>",
     ),
-    workspace_id='<value>',
 )
 
-req = operations.GetWorkspaceAccessRequest()
-
-res = s.auth.get_workspace_access(req)
+res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest())
 
 if res.access_details is not None:
     # handle response
     pass
 
 ```
 <!-- End Retries [retries] -->
```

### Comparing `speakeasy-client-sdk-python-5.7.1/setup.py` & `speakeasy-client-sdk-python-5.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='speakeasy-client-sdk-python',
-    version='5.7.1',
+    version='5.8.0',
     author='Speakeasy',
     description='Speakeasy API Client SDK for Python',
     url='https://github.com/speakeasy-api/speakeasy-client-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/_hooks/registration.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/_hooks/sdkhooks.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/_hooks/types.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,35 +4,37 @@
 from .sdkconfiguration import SDKConfiguration
 from enum import Enum
 from speakeasy import utils
 from speakeasy._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from speakeasy.models import errors, operations, shared
 from typing import List, Optional
 
-class GeneratePostmanCollectionForApiEndpointAcceptEnum(str, Enum):
+class DownloadSchemaAcceptEnum(str, Enum):
     APPLICATION_JSON = "application/json"
-    APPLICATION_OCTET_STREAM = "application/octet-stream"
+    APPLICATION_X_YAML = "application/x-yaml"
 
-class APIEndpoints:
-    r"""REST APIs for managing ApiEndpoint entities"""
+class DownloadSchemaRevisionAcceptEnum(str, Enum):
+    APPLICATION_JSON = "application/json"
+    APPLICATION_X_YAML = "application/x-yaml"
+
+class Schemas:
+    r"""REST APIs for managing Schema entities"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def delete_api_endpoint(self, request: operations.DeleteAPIEndpointRequest) -> operations.DeleteAPIEndpointResponse:
-        r"""Delete an ApiEndpoint.
-        Delete an ApiEndpoint. This will also delete all associated Request Logs (if using a Postgres datastore).
-        """
-        hook_ctx = HookContext(operation_id='deleteApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def delete_schema(self, request: operations.DeleteSchemaRequest) -> operations.DeleteSchemaResponse:
+        r"""Delete a particular schema revision for an Api."""
+        hook_ctx = HookContext(operation_id='deleteSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -55,48 +57,49 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.DeleteAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DeleteSchemaResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def find_api_endpoint(self, request: operations.FindAPIEndpointRequest) -> operations.FindAPIEndpointResponse:
-        r"""Find an ApiEndpoint via its displayName.
-        Find an ApiEndpoint via its displayName (set by operationId from a registered OpenAPI schema).
-        This is useful for finding the ID of an ApiEndpoint to use in the /v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID} endpoints.
-        """
-        hook_ctx = HookContext(operation_id='findApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def download_schema(self, request: operations.DownloadSchemaRequest, accept_header_override: Optional[DownloadSchemaAcceptEnum] = None) -> operations.DownloadSchemaResponse:
+        r"""Download the latest schema for a particular apiID."""
+        hook_ctx = HookContext(operation_id='downloadSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/find/{displayName}', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/download', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = 'application/json'
+        if accept_header_override is not None:
+            headers['Accept'] = accept_header_override.value
+        else:
+            headers['Accept'] = 'application/json;q=1, application/x-yaml;q=0'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -112,53 +115,57 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.FindAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DownloadSchemaResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.APIEndpoint])
-                res.api_endpoint = out
+                res.two_hundred_application_json_schema = http_res
+            # pylint: disable=no-else-return
+            elif utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/x-yaml'):                
+                res.two_hundred_application_x_yaml_schema = http_res
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def generate_open_api_spec_for_api_endpoint(self, request: operations.GenerateOpenAPISpecForAPIEndpointRequest) -> operations.GenerateOpenAPISpecForAPIEndpointResponse:
-        r"""Generate an OpenAPI specification for a particular ApiEndpoint.
-        This endpoint will generate a new operation in any registered OpenAPI document if the operation does not already exist in the document.
-        Returns the original document and the newly generated document allowing a diff to be performed to see what has changed.
-        """
-        hook_ctx = HookContext(operation_id='generateOpenApiSpecForApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def download_schema_revision(self, request: operations.DownloadSchemaRevisionRequest, accept_header_override: Optional[DownloadSchemaRevisionAcceptEnum] = None) -> operations.DownloadSchemaRevisionResponse:
+        r"""Download a particular schema revision for an Api."""
+        hook_ctx = HookContext(operation_id='downloadSchemaRevision', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}/generate/openapi', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}/download', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = 'application/json'
+        if accept_header_override is not None:
+            headers['Accept'] = accept_header_override.value
+        else:
+            headers['Accept'] = 'application/json;q=1, application/x-yaml;q=0'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -174,55 +181,57 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GenerateOpenAPISpecForAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DownloadSchemaRevisionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.GenerateOpenAPISpecDiff])
-                res.generate_open_api_spec_diff = out
+                res.two_hundred_application_json_schema = http_res
+            # pylint: disable=no-else-return
+            elif utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/x-yaml'):                
+                res.two_hundred_application_x_yaml_schema = http_res
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def generate_postman_collection_for_api_endpoint(self, request: operations.GeneratePostmanCollectionForAPIEndpointRequest, accept_header_override: Optional[GeneratePostmanCollectionForApiEndpointAcceptEnum] = None) -> operations.GeneratePostmanCollectionForAPIEndpointResponse:
-        r"""Generate a Postman collection for a particular ApiEndpoint.
-        Generates a postman collection that allows the endpoint to be called from postman variables produced for any path/query/header parameters included in the OpenAPI document.
+    def get_schema(self, request: operations.GetSchemaRequest) -> operations.GetSchemaResponse:
+        r"""Get information about the latest schema.
+        Returns information about the last uploaded schema for a particular API version. 
+        This won't include the schema itself, that can be retrieved via the downloadSchema operation.
         """
-        hook_ctx = HookContext(operation_id='generatePostmanCollectionForApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='getSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}/generate/postman', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        if accept_header_override is not None:
-            headers['Accept'] = accept_header_override.value
-        else:
-            headers['Accept'] = 'application/json;q=1, application/octet-stream;q=0'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -238,42 +247,45 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GeneratePostmanCollectionForAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetSchemaResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/octet-stream'):                
-                res.postman_collection = http_res
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_all_api_endpoints(self, request: operations.GetAllAPIEndpointsRequest) -> operations.GetAllAPIEndpointsResponse:
-        r"""Get all Api endpoints for a particular apiID."""
-        hook_ctx = HookContext(operation_id='getAllApiEndpoints', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_schema_diff(self, request: operations.GetSchemaDiffRequest) -> operations.GetSchemaDiffResponse:
+        r"""Get a diff of two schema revisions for an Api."""
+        hook_ctx = HookContext(operation_id='getSchemaDiff', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/api_endpoints', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{baseRevisionID}/diff/{targetRevisionID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -296,43 +308,48 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetAllAPIEndpointsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetSchemaDiffResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[shared.APIEndpoint]])
-                res.api_endpoints = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.SchemaDiff])
+                res.schema_diff = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_all_for_version_api_endpoints(self, request: operations.GetAllForVersionAPIEndpointsRequest) -> operations.GetAllForVersionAPIEndpointsResponse:
-        r"""Get all ApiEndpoints for a particular apiID and versionID."""
-        hook_ctx = HookContext(operation_id='getAllForVersionApiEndpoints', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_schema_revision(self, request: operations.GetSchemaRevisionRequest) -> operations.GetSchemaRevisionResponse:
+        r"""Get information about a particular schema revision for an Api.
+        Returns information about the last uploaded schema for a particular schema revision. 
+        This won't include the schema itself, that can be retrieved via the downloadSchema operation.
+        """
+        hook_ctx = HookContext(operation_id='getSchemaRevision', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -355,43 +372,48 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetAllForVersionAPIEndpointsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetSchemaRevisionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[shared.APIEndpoint]])
-                res.api_endpoints = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_api_endpoint(self, request: operations.GetAPIEndpointRequest) -> operations.GetAPIEndpointResponse:
-        r"""Get an ApiEndpoint."""
-        hook_ctx = HookContext(operation_id='getApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_schemas(self, request: operations.GetSchemasRequest) -> operations.GetSchemasResponse:
+        r"""Get information about all schemas associated with a particular apiID.
+        Returns information the schemas associated with a particular apiID. 
+        This won't include the schemas themselves, they can be retrieved via the downloadSchema operation.
+        """
+        hook_ctx = HookContext(operation_id='getSchemas', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schemas', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -414,62 +436,65 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetSchemasResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.APIEndpoint])
-                res.api_endpoint = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[shared.Schema]])
+                res.classes = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def upsert_api_endpoint(self, request: operations.UpsertAPIEndpointRequest) -> operations.UpsertAPIEndpointResponse:
-        r"""Upsert an ApiEndpoint.
-        Upsert an ApiEndpoint. If the ApiEndpoint does not exist it will be created, otherwise it will be updated.
+    def register_schema(self, request: operations.RegisterSchemaRequest) -> operations.RegisterSchemaResponse:
+        r"""Register a schema.
+        Allows uploading a schema for a particular API version.
+        This will be used to populate ApiEndpoints and used as a base for any schema generation if present.
         """
-        hook_ctx = HookContext(operation_id='upsertApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='registerSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpsertAPIEndpointRequest, "api_endpoint", False, False, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.RegisterSchemaRequest, "request_body", False, False, 'multipart')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -480,26 +505,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.UpsertAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.RegisterSchemaResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.APIEndpoint])
-                res.api_endpoint = out
-            else:
-                content_type = http_res.headers.get('Content-Type')
-                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+            pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/apis.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         res = operations.DeleteAPIResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -115,23 +116,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GenerateOpenAPISpecResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GenerateOpenAPISpecDiff])
                 res.generate_open_api_spec_diff = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -179,22 +182,24 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GeneratePostmanCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/octet-stream'):                
                 res.postman_collection = http_res
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -241,23 +246,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAllAPIVersionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.API]])
                 res.apis = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -304,23 +311,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetApisResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.API]])
                 res.apis = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -371,23 +380,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpsertAPIResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.API])
                 res.api = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/artifacts.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/artifacts.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,22 +62,24 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetBlobResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/octet-stream'):                
                 res.blob = http_res
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -123,23 +125,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetManifestResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/vnd.oci.image.manifest.v1+json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Manifest])
                 res.manifest = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -182,23 +186,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetNamespacesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetNamespacesResponse])
                 res.get_namespaces_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -241,23 +247,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetRevisionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetRevisionsResponse])
                 res.get_revisions_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -299,23 +307,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTagsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetTagsResponse])
                 res.get_tags_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -365,26 +375,27 @@
         res = operations.PostTagsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def preflight(self, request: Optional[shared.PreflightRequest]) -> operations.PreflightResponse:
+    def preflight(self, request: Optional[shared.PreflightRequest] = None) -> operations.PreflightResponse:
         r"""Get access token for communicating with OCI distribution endpoints"""
         hook_ctx = HookContext(operation_id='preflight', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/v1/artifacts/preflight'
         
         if callable(self.sdk_configuration.security):
@@ -418,23 +429,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PreflightResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PreflightToken])
                 res.preflight_token = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/auth.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,23 +50,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccessTokenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccessToken])
                 res.access_token = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -109,23 +111,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetUserResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.User])
                 res.user = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -193,14 +197,15 @@
             '503'
         ]))
         
         
         res = operations.GetWorkspaceAccessResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccessDetails])
                 res.access_details = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -247,23 +252,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ValidateAPIKeyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.APIKeyDetails])
                 res.api_key_details = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/embeds.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,23 +55,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetEmbedAccessTokenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.EmbedAccessTokenResponse])
                 res.embed_access_token_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -114,23 +116,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetValidEmbedAccessTokensResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.EmbedToken]])
                 res.embed_tokens = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -177,14 +181,15 @@
         res = operations.RevokeEmbedAccessTokenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/events.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/events.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,23 +57,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetWorkspaceEventsByTargetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CliEvent]])
                 res.cli_event_batch = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 500 and http_res.status_code < 600:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -124,23 +126,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetWorkspaceTargetsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.TargetSDK]])
                 res.target_sdk_list = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 500 and http_res.status_code < 600:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -224,14 +228,15 @@
         res = operations.PostWorkspaceEventsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 500 and http_res.status_code < 600:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -282,23 +287,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.SearchWorkspaceEventsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.CliEvent]])
                 res.cli_event_batch = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 500 and http_res.status_code < 600:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         res = operations.DeleteVersionMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -105,23 +106,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetVersionMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.VersionMetadata]])
                 res.version_metadata = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -169,23 +172,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.InsertVersionMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.VersionMetadata])
                 res.version_metadata = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/errors/error.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/errors/sdkerror.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getaccesstoken.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getblob.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getblob.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getchangesreportsignedurl.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getchangesreportsignedurl.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getlintingreportsignedurl.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getlintingreportsignedurl.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getmanifest.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getnamespaces.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getnamespaces.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getorganizations.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getorganizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getrevisions.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getrevisions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/gettags.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/gettags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getuser.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getuser.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getworkspaceaccess.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getworkspaceaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getworkspaceeventsbytarget.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getworkspaceeventsbytarget.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/getworkspacetargets.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/getworkspacetargets.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/posttags.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/posttags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/postworkspaceevents.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/postworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/preflight.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/preflight.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/searchworkspaceevents.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/searchworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/uploadreport.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/uploadreport.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/upsertapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/operations/validateapikey.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/operations/validateapikey.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/accessdetails.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/accessdetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/accesstoken.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/accesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/addtags.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/addtags.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/annotations.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/annotations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/api_input.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/api_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/apiendpoint_input.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/apiendpoint_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/apikeydetails.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/apikeydetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/clievent.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/clievent.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     r"""The version of the customer's SDK that we just generated"""
     generate_config_pre_checksum: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_config_pre_checksum'), 'exclude': lambda f: f is None }})
     r"""Checksum of the configuration file (prior to generation)"""
     generate_config_pre_raw: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_config_pre_raw'), 'exclude': lambda f: f is None }})
     r"""Rendered configuration file (prior to generation)"""
     generate_config_pre_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_config_pre_version'), 'exclude': lambda f: f is None }})
     r"""The version of the customer's SDK before we generated"""
+    generate_eligible_features: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_eligible_features'), 'exclude': lambda f: f is None }})
+    r"""Eligible feature set during generation"""
     generate_gen_lock_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_gen_lock_id'), 'exclude': lambda f: f is None }})
     r"""gen.lock ID (expected to be a uuid)."""
     generate_gen_lock_post_features: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_gen_lock_post_features'), 'exclude': lambda f: f is None }})
     r"""Features post generation"""
     generate_gen_lock_pre_blob_digest: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_gen_lock_pre_blob_digest'), 'exclude': lambda f: f is None }})
     r"""Blob digest of the Previous Generation"""
     generate_gen_lock_pre_doc_checksum: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_gen_lock_pre_doc_checksum'), 'exclude': lambda f: f is None }})
@@ -83,28 +85,34 @@
     r"""Features prior to generation"""
     generate_gen_lock_pre_namespace_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_gen_lock_pre_namespace_name'), 'exclude': lambda f: f is None }})
     r"""Namespace name of the Previous Generation"""
     generate_gen_lock_pre_revision_digest: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_gen_lock_pre_revision_digest'), 'exclude': lambda f: f is None }})
     r"""Revision digest of the Previous Generation"""
     generate_gen_lock_pre_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_gen_lock_pre_version'), 'exclude': lambda f: f is None }})
     r"""Artifact version for the Previous Generation"""
+    generate_number_of_operations_ignored: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_number_of_operations_ignored'), 'exclude': lambda f: f is None }})
+    r"""The number of operations ignored in generation."""
+    generate_number_of_operations_used: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_number_of_operations_used'), 'exclude': lambda f: f is None }})
+    r"""The number of operations used in generation."""
     generate_output_tests: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_output_tests'), 'exclude': lambda f: f is None }})
     r"""Indicates whether tests were output."""
     generate_published: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_published'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the target was considered published."""
     generate_repo_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_repo_url'), 'exclude': lambda f: f is None }})
     r"""Expected Repo URL, for use in documentation generation."""
     generate_target: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_target'), 'exclude': lambda f: f is None }})
     r"""The target of the event."""
     generate_target_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_target_version'), 'exclude': lambda f: f is None }})
     r"""The version of the target."""
     generate_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_version'), 'exclude': lambda f: f is None }})
     r"""Version of the generation logic used."""
     gh_action_organization: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_organization'), 'exclude': lambda f: f is None }})
     r"""GitHub organization of the action."""
+    gh_action_ref: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_ref'), 'exclude': lambda f: f is None }})
+    r"""GitHub Action ref value."""
     gh_action_repository: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_repository'), 'exclude': lambda f: f is None }})
     r"""GitHub repository of the action."""
     gh_action_run_link: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_run_link'), 'exclude': lambda f: f is None }})
     r"""Link to the GitHub action run."""
     gh_action_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_version'), 'exclude': lambda f: f is None }})
     r"""Version of the GitHub action."""
     git_relative_cwd: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('git_relative_cwd'), 'exclude': lambda f: f is None }})
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/filter_.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/filter_.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/generateopenapispecdiff.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/generateopenapispecdiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/getrevisionsresponse.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/getrevisionsresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/manifest.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/manifest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/namespace.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/namespace.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/organization.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/organization.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/preflighttoken.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/preflighttoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/report.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/report.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/revision.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/revision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/security.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/tag.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/tag.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/targetsdk.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/targetsdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,26 +29,34 @@
     r"""Remote commit ID."""
     continuous_integration_environment: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('continuous_integration_environment'), 'exclude': lambda f: f is None }})
     r"""Name of the CI environment."""
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
     r"""Error message if the last event was not successful."""
     generate_config_post_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_config_post_version'), 'exclude': lambda f: f is None }})
     r"""Version of the generated target (post generation)"""
+    generate_eligible_features: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_eligible_features'), 'exclude': lambda f: f is None }})
+    r"""Eligible feature set during generation"""
     generate_gen_lock_pre_features: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_gen_lock_pre_features'), 'exclude': lambda f: f is None }})
     r"""Features prior to generation"""
     generate_gen_lock_pre_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_gen_lock_pre_version'), 'exclude': lambda f: f is None }})
     r"""Artifact version for the Previous Generation"""
+    generate_number_of_operations_ignored: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_number_of_operations_ignored'), 'exclude': lambda f: f is None }})
+    r"""The number of operations ignored in generation."""
+    generate_number_of_operations_used: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_number_of_operations_used'), 'exclude': lambda f: f is None }})
+    r"""The number of operations used in generation."""
     generate_published: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_published'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the target was considered published."""
     generate_target_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_target_name'), 'exclude': lambda f: f is None }})
     r"""The name of the target as defined by the user."""
     generate_target_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('generate_target_version'), 'exclude': lambda f: f is None }})
     r"""The version of the Speakeasy generator for this target eg v2 of the typescript generator."""
     gh_action_organization: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_organization'), 'exclude': lambda f: f is None }})
     r"""GitHub organization of the action."""
+    gh_action_ref: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_ref'), 'exclude': lambda f: f is None }})
+    r"""GitHub Action ref value."""
     gh_action_repository: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_repository'), 'exclude': lambda f: f is None }})
     r"""GitHub repository of the action."""
     gh_action_run_link: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_run_link'), 'exclude': lambda f: f is None }})
     r"""Link to the GitHub action run."""
     gh_action_version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gh_action_version'), 'exclude': lambda f: f is None }})
     r"""Version of the GitHub action."""
     git_relative_cwd: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('git_relative_cwd'), 'exclude': lambda f: f is None }})
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/user.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/v2descriptor.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/v2descriptor.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/versionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/models/shared/versionmetadata_input.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/models/shared/versionmetadata_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/organizations.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/organizations.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,23 +52,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetOrganizationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.Organization]])
                 res.organizations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/reports.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetChangesReportSignedURLResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetChangesReportSignedURLSignedAccess])
                 res.signed_access = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -105,14 +106,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetLintingReportSignedURLResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetLintingReportSignedURLSignedAccess])
                 res.signed_access = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -164,14 +166,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UploadReportResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UploadReportUploadedReport])
                 res.uploaded_report = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,22 +62,24 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GenerateRequestPostmanCollectionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/octet-stream'):                
                 res.postman_collection = http_res
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -120,23 +122,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetRequestFromEventLogResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UnboundedRequest])
                 res.unbounded_request = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -183,23 +187,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.QueryEventLogResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[shared.BoundedRequest]])
                 res.bounded_requests = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/apiendpoints.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,37 +4,35 @@
 from .sdkconfiguration import SDKConfiguration
 from enum import Enum
 from speakeasy import utils
 from speakeasy._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from speakeasy.models import errors, operations, shared
 from typing import List, Optional
 
-class DownloadSchemaAcceptEnum(str, Enum):
+class GeneratePostmanCollectionForApiEndpointAcceptEnum(str, Enum):
     APPLICATION_JSON = "application/json"
-    APPLICATION_X_YAML = "application/x-yaml"
+    APPLICATION_OCTET_STREAM = "application/octet-stream"
 
-class DownloadSchemaRevisionAcceptEnum(str, Enum):
-    APPLICATION_JSON = "application/json"
-    APPLICATION_X_YAML = "application/x-yaml"
-
-class Schemas:
-    r"""REST APIs for managing Schema entities"""
+class APIEndpoints:
+    r"""REST APIs for managing ApiEndpoint entities"""
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def delete_schema(self, request: operations.DeleteSchemaRequest) -> operations.DeleteSchemaResponse:
-        r"""Delete a particular schema revision for an Api."""
-        hook_ctx = HookContext(operation_id='deleteSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def delete_api_endpoint(self, request: operations.DeleteAPIEndpointRequest) -> operations.DeleteAPIEndpointResponse:
+        r"""Delete an ApiEndpoint.
+        Delete an ApiEndpoint. This will also delete all associated Request Logs (if using a Postgres datastore).
+        """
+        hook_ctx = HookContext(operation_id='deleteApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -57,48 +55,49 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.DeleteSchemaResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DeleteAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def download_schema(self, request: operations.DownloadSchemaRequest, accept_header_override: Optional[DownloadSchemaAcceptEnum] = None) -> operations.DownloadSchemaResponse:
-        r"""Download the latest schema for a particular apiID."""
-        hook_ctx = HookContext(operation_id='downloadSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def find_api_endpoint(self, request: operations.FindAPIEndpointRequest) -> operations.FindAPIEndpointResponse:
+        r"""Find an ApiEndpoint via its displayName.
+        Find an ApiEndpoint via its displayName (set by operationId from a registered OpenAPI schema).
+        This is useful for finding the ID of an ApiEndpoint to use in the /v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID} endpoints.
+        """
+        hook_ctx = HookContext(operation_id='findApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/download', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/find/{displayName}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        if accept_header_override is not None:
-            headers['Accept'] = accept_header_override.value
-        else:
-            headers['Accept'] = 'application/json;q=1, application/x-yaml;q=0'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -114,54 +113,55 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.DownloadSchemaResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.FindAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                res.two_hundred_application_json_schema = http_res
-            elif utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/x-yaml'):                
-                res.two_hundred_application_x_yaml_schema = http_res
+                out = utils.unmarshal_json(http_res.text, Optional[shared.APIEndpoint])
+                res.api_endpoint = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def download_schema_revision(self, request: operations.DownloadSchemaRevisionRequest, accept_header_override: Optional[DownloadSchemaRevisionAcceptEnum] = None) -> operations.DownloadSchemaRevisionResponse:
-        r"""Download a particular schema revision for an Api."""
-        hook_ctx = HookContext(operation_id='downloadSchemaRevision', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def generate_open_api_spec_for_api_endpoint(self, request: operations.GenerateOpenAPISpecForAPIEndpointRequest) -> operations.GenerateOpenAPISpecForAPIEndpointResponse:
+        r"""Generate an OpenAPI specification for a particular ApiEndpoint.
+        This endpoint will generate a new operation in any registered OpenAPI document if the operation does not already exist in the document.
+        Returns the original document and the newly generated document allowing a diff to be performed to see what has changed.
+        """
+        hook_ctx = HookContext(operation_id='generateOpenApiSpecForApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}/download', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}/generate/openapi', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        if accept_header_override is not None:
-            headers['Accept'] = accept_header_override.value
-        else:
-            headers['Accept'] = 'application/json;q=1, application/x-yaml;q=0'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -177,54 +177,57 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.DownloadSchemaRevisionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GenerateOpenAPISpecForAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                res.two_hundred_application_json_schema = http_res
-            elif utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/x-yaml'):                
-                res.two_hundred_application_x_yaml_schema = http_res
+                out = utils.unmarshal_json(http_res.text, Optional[shared.GenerateOpenAPISpecDiff])
+                res.generate_open_api_spec_diff = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_schema(self, request: operations.GetSchemaRequest) -> operations.GetSchemaResponse:
-        r"""Get information about the latest schema.
-        Returns information about the last uploaded schema for a particular API version. 
-        This won't include the schema itself, that can be retrieved via the downloadSchema operation.
+    def generate_postman_collection_for_api_endpoint(self, request: operations.GeneratePostmanCollectionForAPIEndpointRequest, accept_header_override: Optional[GeneratePostmanCollectionForApiEndpointAcceptEnum] = None) -> operations.GeneratePostmanCollectionForAPIEndpointResponse:
+        r"""Generate a Postman collection for a particular ApiEndpoint.
+        Generates a postman collection that allows the endpoint to be called from postman variables produced for any path/query/header parameters included in the OpenAPI document.
         """
-        hook_ctx = HookContext(operation_id='getSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='generatePostmanCollectionForApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}/generate/postman', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = 'application/json'
+        if accept_header_override is not None:
+            headers['Accept'] = accept_header_override.value
+        else:
+            headers['Accept'] = 'application/json;q=1, application/octet-stream;q=0'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -240,43 +243,44 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetSchemaResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GeneratePostmanCollectionForAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
-                res.schema = out
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/octet-stream'):                
+                res.postman_collection = http_res
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_schema_diff(self, request: operations.GetSchemaDiffRequest) -> operations.GetSchemaDiffResponse:
-        r"""Get a diff of two schema revisions for an Api."""
-        hook_ctx = HookContext(operation_id='getSchemaDiff', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_all_api_endpoints(self, request: operations.GetAllAPIEndpointsRequest) -> operations.GetAllAPIEndpointsResponse:
+        r"""Get all Api endpoints for a particular apiID."""
+        hook_ctx = HookContext(operation_id='getAllApiEndpoints', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{baseRevisionID}/diff/{targetRevisionID}', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/api_endpoints', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -299,46 +303,45 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetSchemaDiffResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetAllAPIEndpointsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.SchemaDiff])
-                res.schema_diff = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[shared.APIEndpoint]])
+                res.api_endpoints = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_schema_revision(self, request: operations.GetSchemaRevisionRequest) -> operations.GetSchemaRevisionResponse:
-        r"""Get information about a particular schema revision for an Api.
-        Returns information about the last uploaded schema for a particular schema revision. 
-        This won't include the schema itself, that can be retrieved via the downloadSchema operation.
-        """
-        hook_ctx = HookContext(operation_id='getSchemaRevision', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_all_for_version_api_endpoints(self, request: operations.GetAllForVersionAPIEndpointsRequest) -> operations.GetAllForVersionAPIEndpointsResponse:
+        r"""Get all ApiEndpoints for a particular apiID and versionID."""
+        hook_ctx = HookContext(operation_id='getAllForVersionApiEndpoints', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema/{revisionID}', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -361,46 +364,45 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetSchemaRevisionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetAllForVersionAPIEndpointsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
-                res.schema = out
+                out = utils.unmarshal_json(http_res.text, Optional[List[shared.APIEndpoint]])
+                res.api_endpoints = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def get_schemas(self, request: operations.GetSchemasRequest) -> operations.GetSchemasResponse:
-        r"""Get information about all schemas associated with a particular apiID.
-        Returns information the schemas associated with a particular apiID. 
-        This won't include the schemas themselves, they can be retrieved via the downloadSchema operation.
-        """
-        hook_ctx = HookContext(operation_id='getSchemas', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+    def get_api_endpoint(self, request: operations.GetAPIEndpointRequest) -> operations.GetAPIEndpointResponse:
+        r"""Get an ApiEndpoint."""
+        hook_ctx = HookContext(operation_id='getApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schemas', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -423,63 +425,64 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.GetSchemasResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[shared.Schema]])
-                res.classes = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.APIEndpoint])
+                res.api_endpoint = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def register_schema(self, request: operations.RegisterSchemaRequest) -> operations.RegisterSchemaResponse:
-        r"""Register a schema.
-        Allows uploading a schema for a particular API version.
-        This will be used to populate ApiEndpoints and used as a base for any schema generation if present.
+    def upsert_api_endpoint(self, request: operations.UpsertAPIEndpointRequest) -> operations.UpsertAPIEndpointResponse:
+        r"""Upsert an ApiEndpoint.
+        Upsert an ApiEndpoint. If the ApiEndpoint does not exist it will be created, otherwise it will be updated.
         """
-        hook_ctx = HookContext(operation_id='registerSchema', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        hook_ctx = HookContext(operation_id='upsertApiEndpoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/schema', request)
+        url = utils.generate_url(base_url, '/v1/apis/{apiID}/version/{versionID}/api_endpoints/{apiEndpointID}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        req_content_type, data, form = utils.serialize_request_body(request, operations.RegisterSchemaRequest, "request_body", False, False, 'multipart')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpsertAPIEndpointRequest, "api_endpoint", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -490,21 +493,28 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.RegisterSchemaResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpsertAPIEndpointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            pass
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[shared.APIEndpoint])
+                res.api_endpoint = out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.Error])
                 res.error = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/sdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/sdkconfiguration.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/sdkconfiguration.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server: Optional[str] = ''
     language: str = 'python'
     openapi_doc_version: str = '0.4.0 .'
-    sdk_version: str = '5.7.1'
-    gen_version: str = '2.322.5'
-    user_agent: str = 'speakeasy-sdk/python 5.7.1 2.322.5 0.4.0 . speakeasy-client-sdk-python'
+    sdk_version: str = '5.8.0'
+    gen_version: str = '2.326.3'
+    user_agent: str = 'speakeasy-sdk/python 5.8.0 2.326.3 0.4.0 . speakeasy-client-sdk-python'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.7.1
+Version: 5.8.0
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -24,20 +24,17 @@
         import speakeasy
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.GetApisRequest()
-        
-        res = s.apis.get_apis(req)
+        res = s.apis.get_apis(request=operations.GetApisRequest())
         
         if res.apis is not None:
             # handle response
             pass
         
         ```
         <!-- End SDK Example Usage [usage] -->
@@ -151,24 +148,21 @@
         import speakeasy
         from speakeasy.models import errors, operations, shared
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
-        )
-        
-        req = operations.GetWorkspaceEventsByTargetRequest(
-            target_id='<value>',
         )
         
         res = None
         try:
-            res = s.events.get_workspace_events_by_target(req)
+            res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
+            target_id='<value>',
+        ))
         except errors.Error as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
         
@@ -199,23 +193,20 @@
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             server="prod",
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.DeleteAPIRequest(
+        res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
-        )
-        
-        res = s.apis.delete_api(req)
+        ))
         
         if res is not None:
             # handle response
             pass
         
         ```
         
@@ -228,23 +219,20 @@
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             server_url="https://api.prod.speakeasyapi.dev",
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.DeleteAPIRequest(
+        res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
-        )
-        
-        res = s.apis.delete_api(req)
+        ))
         
         if res is not None:
             # handle response
             pass
         
         ```
         <!-- End Server Selection [server] -->
@@ -286,23 +274,20 @@
         import speakeasy
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.DeleteAPIRequest(
+        res = s.apis.delete_api(request=operations.DeleteAPIRequest(
             api_id='<value>',
             version_id='<value>',
-        )
-        
-        res = s.apis.delete_api(req)
+        ))
         
         if res is not None:
             # handle response
             pass
         
         ```
         <!-- End Authentication [security] -->
@@ -330,22 +315,19 @@
         import speakeasy
         from speakeasy.models import operations, shared
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceEventsByTargetRequest(
+        res = s.events.get_workspace_events_by_target(request=operations.GetWorkspaceEventsByTargetRequest(
             target_id='<value>',
-        )
-        
-        res = s.events.get_workspace_events_by_target(req)
+        ))
         
         if res.cli_event_batch is not None:
             # handle response
             pass
         
         ```
         <!-- End Global Parameters [global-parameters] -->
@@ -361,20 +343,17 @@
         from speakeasy.models import operations, shared
         from speakeasy.utils import BackoffStrategy, RetryConfig
         
         s = speakeasy.Speakeasy(
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceAccessRequest()
-        
-        res = s.auth.get_workspace_access(req,
+        res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest(),
             RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False))
         
         if res.access_details is not None:
             # handle response
             pass
         
         ```
@@ -386,20 +365,17 @@
         from speakeasy.utils import BackoffStrategy, RetryConfig
         
         s = speakeasy.Speakeasy(
             retry_config=RetryConfig('backoff', BackoffStrategy(1, 50, 1.1, 100), False),
             security=shared.Security(
                 api_key="<YOUR_API_KEY_HERE>",
             ),
-            workspace_id='<value>',
         )
         
-        req = operations.GetWorkspaceAccessRequest()
-        
-        res = s.auth.get_workspace_access(req)
+        res = s.auth.get_workspace_access(request=operations.GetWorkspaceAccessRequest())
         
         if res.access_details is not None:
             # handle response
             pass
         
         ```
         <!-- End Retries [retries] -->
```

### Comparing `speakeasy-client-sdk-python-5.7.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-5.8.0/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*


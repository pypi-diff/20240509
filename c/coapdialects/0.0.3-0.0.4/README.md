# Comparing `tmp/coapdialects-0.0.3.tar.gz` & `tmp/coapdialects-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coapdialects-0.0.3.tar", last modified: Thu May  9 17:21:10 2024, max compression
+gzip compressed data, was "coapdialects-0.0.4.tar", last modified: Thu May  9 17:24:57 2024, max compression
```

## Comparing `coapdialects-0.0.3.tar` & `coapdialects-0.0.4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.318352 coapdialects-0.0.3/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1086 2024-04-28 18:52:03.000000 coapdialects-0.0.3/LICENSE
--rw-r--r--   0 erikg     (1000) erikg     (1000)      789 2024-05-09 17:21:10.318352 coapdialects-0.0.3/PKG-INFO
--rw-rw-r--   0 erikg     (1000) erikg     (1000)       14 2024-04-28 18:52:03.000000 coapdialects-0.0.3/README.md
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      863 2024-05-09 17:20:45.000000 coapdialects-0.0.3/pyproject.toml
--rw-rw-r--   0 erikg     (1000) erikg     (1000)       38 2024-05-09 17:21:10.318352 coapdialects-0.0.3/setup.cfg
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.310348 coapdialects-0.0.3/src/
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.310348 coapdialects-0.0.3/src/coapdialects/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1075 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     4510 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/blockwise.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.314350 coapdialects-0.0.3/src/coapdialects/cli/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      515 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/cli/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17334 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/cli/client.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5538 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/cli/common.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2158 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/cli/defaults.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    14554 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/cli/fileserver.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     6283 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/cli/proxy.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    29388 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/cli/rd.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    12589 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/credentials.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7793 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/defaults.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7233 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/error.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    20509 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/interfaces.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    27717 2024-05-09 17:19:57.000000 coapdialects-0.0.3/src/coapdialects/message.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    21127 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/messagemanager.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      670 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/meta.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.314350 coapdialects-0.0.3/src/coapdialects/numbers/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1425 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/numbers/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5275 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/numbers/codes.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5795 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/numbers/constants.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    12199 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/numbers/contentformat.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5534 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/numbers/optionnumbers.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      575 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/numbers/types.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     9296 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/options.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     8207 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/optiontypes.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    80685 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/oscore.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     6275 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/oscore_sitewrapper.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    13282 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/pipe.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    46714 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/protocol.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.314350 coapdialects-0.0.3/src/coapdialects/proxy/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      242 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/proxy/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1615 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/proxy/client.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    15717 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/proxy/server.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17175 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/resource.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.314350 coapdialects-0.0.3/src/coapdialects/resourcedirectory/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      382 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/resourcedirectory/__init__.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.314350 coapdialects-0.0.3/src/coapdialects/resourcedirectory/client/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      304 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/resourcedirectory/client/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    13702 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/resourcedirectory/client/register.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    11199 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/tokenmanager.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.314350 coapdialects-0.0.3/src/coapdialects/transports/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      828 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2485 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/generic_udp.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    10545 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/oscore.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     8288 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/rfc8323common.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    11182 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/simple6.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7998 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/simplesocketserver.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    14842 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/tcp.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    14956 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/tinydtls.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    11343 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/tinydtls_server.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/tls.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    25068 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/udp6.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17659 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/transports/ws.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.314350 coapdialects-0.0.3/src/coapdialects/util/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5844 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/__init__.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.318352 coapdialects-0.0.3/src/coapdialects/util/asyncio/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      486 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/asyncio/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     4126 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/asyncio/getaddrinfo_addrconfig.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     6703 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/asyncio/recvmsg.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1972 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/asyncio/timeoutdict.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5687 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/cli.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/contenttype.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2503 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/cryptography_additions.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1412 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/linkformat.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1200 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/linkformat_pygments.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7029 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/prettyprint.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     4636 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/pyodide_websockets.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2126 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/socknumbers.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      832 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/uri.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.318352 coapdialects-0.0.3/src/coapdialects/util/vendored/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    12359 2024-02-04 01:58:32.000000 coapdialects-0.0.3/src/coapdialects/util/vendored/link_header.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:21:10.318352 coapdialects-0.0.3/src/coapdialects.egg-info/
--rw-r--r--   0 erikg     (1000) erikg     (1000)      789 2024-05-09 17:21:10.000000 coapdialects-0.0.3/src/coapdialects.egg-info/PKG-INFO
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2490 2024-05-09 17:21:10.000000 coapdialects-0.0.3/src/coapdialects.egg-info/SOURCES.txt
--rw-rw-r--   0 erikg     (1000) erikg     (1000)        1 2024-05-09 17:21:10.000000 coapdialects-0.0.3/src/coapdialects.egg-info/dependency_links.txt
--rw-rw-r--   0 erikg     (1000) erikg     (1000)       13 2024-05-09 17:21:10.000000 coapdialects-0.0.3/src/coapdialects.egg-info/top_level.txt
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.728000 coapdialects-0.0.4/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1086 2024-04-28 18:52:03.000000 coapdialects-0.0.4/LICENSE
+-rw-r--r--   0 erikg     (1000) erikg     (1000)      789 2024-05-09 17:24:57.728000 coapdialects-0.0.4/PKG-INFO
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)       14 2024-04-28 18:52:03.000000 coapdialects-0.0.4/README.md
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      863 2024-05-09 17:24:41.000000 coapdialects-0.0.4/pyproject.toml
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)       38 2024-05-09 17:24:57.728000 coapdialects-0.0.4/setup.cfg
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.715994 coapdialects-0.0.4/src/
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.719997 coapdialects-0.0.4/src/coapdialects/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1075 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     4510 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/blockwise.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.719997 coapdialects-0.0.4/src/coapdialects/cli/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      515 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/cli/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    17334 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/cli/client.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5538 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/cli/common.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2158 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/cli/defaults.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    14554 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/cli/fileserver.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     6283 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/cli/proxy.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    29388 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/cli/rd.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    12589 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/credentials.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7793 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/defaults.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7233 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/error.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    20509 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/interfaces.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    27714 2024-05-09 17:24:10.000000 coapdialects-0.0.4/src/coapdialects/message.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    21127 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/messagemanager.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      670 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/meta.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.723998 coapdialects-0.0.4/src/coapdialects/numbers/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1425 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/numbers/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5275 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/numbers/codes.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5795 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/numbers/constants.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    12199 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/numbers/contentformat.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5534 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/numbers/optionnumbers.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      575 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/numbers/types.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     9296 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/options.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     8207 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/optiontypes.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    80685 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/oscore.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     6275 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/oscore_sitewrapper.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    13282 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/pipe.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    46714 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/protocol.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.723998 coapdialects-0.0.4/src/coapdialects/proxy/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      242 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/proxy/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1615 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/proxy/client.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    15717 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/proxy/server.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    17175 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/resource.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.723998 coapdialects-0.0.4/src/coapdialects/resourcedirectory/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      382 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/resourcedirectory/__init__.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.723998 coapdialects-0.0.4/src/coapdialects/resourcedirectory/client/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      304 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/resourcedirectory/client/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    13702 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/resourcedirectory/client/register.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    11199 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/tokenmanager.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.728000 coapdialects-0.0.4/src/coapdialects/transports/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      828 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2485 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/generic_udp.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    10545 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/oscore.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     8288 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/rfc8323common.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    11182 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/simple6.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7998 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/simplesocketserver.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    14842 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/tcp.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    14956 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/tinydtls.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    11343 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/tinydtls_server.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/tls.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    25068 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/udp6.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    17659 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/transports/ws.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.728000 coapdialects-0.0.4/src/coapdialects/util/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5844 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/__init__.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.728000 coapdialects-0.0.4/src/coapdialects/util/asyncio/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      486 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/asyncio/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     4126 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/asyncio/getaddrinfo_addrconfig.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     6703 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/asyncio/recvmsg.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1972 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/asyncio/timeoutdict.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5687 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/cli.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/contenttype.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2503 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/cryptography_additions.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1412 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/linkformat.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1200 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/linkformat_pygments.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7029 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/prettyprint.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     4636 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/pyodide_websockets.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2126 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/socknumbers.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      832 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/uri.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.728000 coapdialects-0.0.4/src/coapdialects/util/vendored/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    12359 2024-02-04 01:58:32.000000 coapdialects-0.0.4/src/coapdialects/util/vendored/link_header.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 17:24:57.728000 coapdialects-0.0.4/src/coapdialects.egg-info/
+-rw-r--r--   0 erikg     (1000) erikg     (1000)      789 2024-05-09 17:24:57.000000 coapdialects-0.0.4/src/coapdialects.egg-info/PKG-INFO
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2490 2024-05-09 17:24:57.000000 coapdialects-0.0.4/src/coapdialects.egg-info/SOURCES.txt
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)        1 2024-05-09 17:24:57.000000 coapdialects-0.0.4/src/coapdialects.egg-info/dependency_links.txt
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)       13 2024-05-09 17:24:57.000000 coapdialects-0.0.4/src/coapdialects.egg-info/top_level.txt
```

### Comparing `coapdialects-0.0.3/LICENSE` & `coapdialects-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/PKG-INFO` & `coapdialects-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coapdialects
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python aiocoap dialects
 Author-email: Erik Gonzalez <erikglez_ipn@hotmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ErikGlz/coapdialects
 Keywords: coap,asyncio,iot
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `coapdialects-0.0.3/pyproject.toml` & `coapdialects-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools >= 66.0" ]
 build-backend = "setuptools.build_meta"
  
 [project]
 name = "coapdialects"
-version = "0.0.3"
+version = "0.0.4"
 description = "Python aiocoap dialects"
 readme = "README.md"
 authors = [
     { name = "Erik Gonzalez", email = "erikglez_ipn@hotmail.com" },
 ]
 license = { text = "MIT" }
 keywords = [ "coap", "asyncio", "iot" ]
```

### Comparing `coapdialects-0.0.3/src/coapdialects/__init__.py` & `coapdialects-0.0.4/src/coapdialects/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/blockwise.py` & `coapdialects-0.0.4/src/coapdialects/blockwise.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/cli/__init__.py` & `coapdialects-0.0.4/src/coapdialects/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/cli/client.py` & `coapdialects-0.0.4/src/coapdialects/cli/client.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/cli/common.py` & `coapdialects-0.0.4/src/coapdialects/cli/common.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/cli/defaults.py` & `coapdialects-0.0.4/src/coapdialects/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/cli/fileserver.py` & `coapdialects-0.0.4/src/coapdialects/cli/fileserver.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/cli/proxy.py` & `coapdialects-0.0.4/src/coapdialects/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/cli/rd.py` & `coapdialects-0.0.4/src/coapdialects/cli/rd.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/credentials.py` & `coapdialects-0.0.4/src/coapdialects/credentials.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/defaults.py` & `coapdialects-0.0.4/src/coapdialects/defaults.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/error.py` & `coapdialects-0.0.4/src/coapdialects/error.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/interfaces.py` & `coapdialects-0.0.4/src/coapdialects/interfaces.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/message.py` & `coapdialects-0.0.4/src/coapdialects/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
           literal or a host name in the unicast case if the Uri-Host option was
           not sent.
         * Properties like Message ID and token will differ if a proxy was
           involved.
         * Some options or even the payload may differ if a proxy was involved.
     """
 
-    def __init__(self, *, version = None, mtype=None, mid=None, code=None, payload=b'', token=b'', uri=None, transport_tuning=None, **kwargs):
+    def __init__(self, *, version = 1, mtype=None, mid=None, code=None, payload=b'', token=b'', uri=None, transport_tuning=None, **kwargs):
         self.version = version
         if mtype is None:
             # leave it unspecified for convenience, sending functions will know what to do
             self.mtype = None
         else:
             self.mtype = Type(mtype)
         self.mid = mid
```

### Comparing `coapdialects-0.0.3/src/coapdialects/messagemanager.py` & `coapdialects-0.0.4/src/coapdialects/messagemanager.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/meta.py` & `coapdialects-0.0.4/src/coapdialects/meta.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/numbers/__init__.py` & `coapdialects-0.0.4/src/coapdialects/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/numbers/codes.py` & `coapdialects-0.0.4/src/coapdialects/numbers/codes.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/numbers/constants.py` & `coapdialects-0.0.4/src/coapdialects/numbers/constants.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/numbers/contentformat.py` & `coapdialects-0.0.4/src/coapdialects/numbers/contentformat.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/numbers/optionnumbers.py` & `coapdialects-0.0.4/src/coapdialects/numbers/optionnumbers.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/numbers/types.py` & `coapdialects-0.0.4/src/coapdialects/numbers/types.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/options.py` & `coapdialects-0.0.4/src/coapdialects/options.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/optiontypes.py` & `coapdialects-0.0.4/src/coapdialects/optiontypes.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/oscore.py` & `coapdialects-0.0.4/src/coapdialects/oscore.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/oscore_sitewrapper.py` & `coapdialects-0.0.4/src/coapdialects/oscore_sitewrapper.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/pipe.py` & `coapdialects-0.0.4/src/coapdialects/pipe.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/protocol.py` & `coapdialects-0.0.4/src/coapdialects/protocol.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/proxy/client.py` & `coapdialects-0.0.4/src/coapdialects/proxy/client.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/proxy/server.py` & `coapdialects-0.0.4/src/coapdialects/proxy/server.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/resource.py` & `coapdialects-0.0.4/src/coapdialects/resource.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/resourcedirectory/client/register.py` & `coapdialects-0.0.4/src/coapdialects/resourcedirectory/client/register.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/tokenmanager.py` & `coapdialects-0.0.4/src/coapdialects/tokenmanager.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/__init__.py` & `coapdialects-0.0.4/src/coapdialects/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/generic_udp.py` & `coapdialects-0.0.4/src/coapdialects/transports/generic_udp.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/oscore.py` & `coapdialects-0.0.4/src/coapdialects/transports/oscore.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/rfc8323common.py` & `coapdialects-0.0.4/src/coapdialects/transports/rfc8323common.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/simple6.py` & `coapdialects-0.0.4/src/coapdialects/transports/simple6.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/simplesocketserver.py` & `coapdialects-0.0.4/src/coapdialects/transports/simplesocketserver.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/tcp.py` & `coapdialects-0.0.4/src/coapdialects/transports/tcp.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/tinydtls.py` & `coapdialects-0.0.4/src/coapdialects/transports/tinydtls.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/tinydtls_server.py` & `coapdialects-0.0.4/src/coapdialects/transports/tinydtls_server.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/tls.py` & `coapdialects-0.0.4/src/coapdialects/transports/tls.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/udp6.py` & `coapdialects-0.0.4/src/coapdialects/transports/udp6.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/transports/ws.py` & `coapdialects-0.0.4/src/coapdialects/transports/ws.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/__init__.py` & `coapdialects-0.0.4/src/coapdialects/util/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/asyncio/getaddrinfo_addrconfig.py` & `coapdialects-0.0.4/src/coapdialects/util/asyncio/getaddrinfo_addrconfig.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/asyncio/recvmsg.py` & `coapdialects-0.0.4/src/coapdialects/util/asyncio/recvmsg.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/asyncio/timeoutdict.py` & `coapdialects-0.0.4/src/coapdialects/util/asyncio/timeoutdict.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/cli.py` & `coapdialects-0.0.4/src/coapdialects/util/cli.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/contenttype.py` & `coapdialects-0.0.4/src/coapdialects/util/contenttype.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/cryptography_additions.py` & `coapdialects-0.0.4/src/coapdialects/util/cryptography_additions.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/linkformat.py` & `coapdialects-0.0.4/src/coapdialects/util/linkformat.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/linkformat_pygments.py` & `coapdialects-0.0.4/src/coapdialects/util/linkformat_pygments.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/prettyprint.py` & `coapdialects-0.0.4/src/coapdialects/util/prettyprint.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/pyodide_websockets.py` & `coapdialects-0.0.4/src/coapdialects/util/pyodide_websockets.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/socknumbers.py` & `coapdialects-0.0.4/src/coapdialects/util/socknumbers.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/uri.py` & `coapdialects-0.0.4/src/coapdialects/util/uri.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects/util/vendored/link_header.py` & `coapdialects-0.0.4/src/coapdialects/util/vendored/link_header.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.3/src/coapdialects.egg-info/PKG-INFO` & `coapdialects-0.0.4/src/coapdialects.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coapdialects
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python aiocoap dialects
 Author-email: Erik Gonzalez <erikglez_ipn@hotmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ErikGlz/coapdialects
 Keywords: coap,asyncio,iot
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `coapdialects-0.0.3/src/coapdialects.egg-info/SOURCES.txt` & `coapdialects-0.0.4/src/coapdialects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

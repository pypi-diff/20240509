# Comparing `tmp/coapdialects-0.0.1.tar.gz` & `tmp/coapdialects-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coapdialects-0.0.1.tar", last modified: Sun Apr 28 21:20:07 2024, max compression
+gzip compressed data, was "coapdialects-0.0.2.tar", last modified: Thu May  9 16:49:55 2024, max compression
```

## Comparing `coapdialects-0.0.1.tar` & `coapdialects-0.0.2.tar`

### file list

```diff
@@ -1,96 +1,85 @@
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.401364 coapdialects-0.0.1/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1086 2024-04-28 18:52:03.000000 coapdialects-0.0.1/LICENSE
--rw-r--r--   0 erikg     (1000) erikg     (1000)      789 2024-04-28 21:20:07.401364 coapdialects-0.0.1/PKG-INFO
--rw-rw-r--   0 erikg     (1000) erikg     (1000)       14 2024-04-28 18:52:03.000000 coapdialects-0.0.1/README.md
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      863 2024-04-28 18:53:29.000000 coapdialects-0.0.1/pyproject.toml
--rw-rw-r--   0 erikg     (1000) erikg     (1000)       38 2024-04-28 21:20:07.401364 coapdialects-0.0.1/setup.cfg
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.329364 coapdialects-0.0.1/src/
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.349364 coapdialects-0.0.1/src/coapdialects/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1075 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     4510 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/blockwise.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.349364 coapdialects-0.0.1/src/coapdialects/cli/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      515 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/cli/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17334 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/cli/client.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5538 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/cli/common.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2158 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/cli/defaults.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    14554 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/cli/fileserver.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     6283 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/cli/proxy.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    29388 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/cli/rd.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    12589 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/credentials.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7793 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/defaults.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7233 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/error.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    20509 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/interfaces.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    27693 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/message.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    27777 2024-04-28 19:37:23.000000 coapdialects-0.0.1/src/coapdialects/message_coapcpv.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    27700 2024-04-28 19:40:53.000000 coapdialects-0.0.1/src/coapdialects/message_coaprcs.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    27699 2024-04-28 19:21:23.000000 coapdialects-0.0.1/src/coapdialects/message_coapts.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    21127 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/messagemanager.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      670 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/meta.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.353364 coapdialects-0.0.1/src/coapdialects/numbers/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1425 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/numbers/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5275 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/numbers/codes.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5897 2024-04-28 19:34:22.000000 coapdialects-0.0.1/src/coapdialects/numbers/codes_coaprcs.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5795 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/numbers/constants.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    12199 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/numbers/contentformat.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5534 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/numbers/optionnumbers.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      575 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/numbers/types.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      574 2024-04-28 19:33:26.000000 coapdialects-0.0.1/src/coapdialects/numbers/types_coapts.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     9296 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/options.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     8207 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/optiontypes.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    80685 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/oscore.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     6275 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/oscore_sitewrapper.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    13282 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/pipe.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    46714 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/protocol.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    46721 2024-04-28 19:57:44.000000 coapdialects-0.0.1/src/coapdialects/protocol_coapcpv.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    46735 2024-04-28 20:01:58.000000 coapdialects-0.0.1/src/coapdialects/protocol_coaprcs.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    46720 2024-04-28 19:57:06.000000 coapdialects-0.0.1/src/coapdialects/protocol_coapts.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.353364 coapdialects-0.0.1/src/coapdialects/proxy/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      242 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/proxy/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1615 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/proxy/client.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    15717 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/proxy/server.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17175 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/resource.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17249 2024-04-28 19:40:04.000000 coapdialects-0.0.1/src/coapdialects/resource_coapcpv.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17292 2024-04-28 19:42:59.000000 coapdialects-0.0.1/src/coapdialects/resource_coaprcs.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17209 2024-04-28 19:44:23.000000 coapdialects-0.0.1/src/coapdialects/resource_coapts.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.353364 coapdialects-0.0.1/src/coapdialects/resourcedirectory/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      382 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/resourcedirectory/__init__.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.353364 coapdialects-0.0.1/src/coapdialects/resourcedirectory/client/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      304 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/resourcedirectory/client/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    13702 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/resourcedirectory/client/register.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    11199 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/tokenmanager.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.381364 coapdialects-0.0.1/src/coapdialects/transports/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      828 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2485 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/generic_udp.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    10545 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/oscore.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     8288 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/rfc8323common.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    11182 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/simple6.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7998 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/simplesocketserver.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    14842 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/tcp.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    14956 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/tinydtls.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    11343 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/tinydtls_server.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/tls.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    25068 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/udp6.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    17659 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/transports/ws.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.397364 coapdialects-0.0.1/src/coapdialects/util/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5844 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/__init__.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.401364 coapdialects-0.0.1/src/coapdialects/util/asyncio/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      486 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/asyncio/__init__.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     4126 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/asyncio/getaddrinfo_addrconfig.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     6703 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/asyncio/recvmsg.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1972 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/asyncio/timeoutdict.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     5687 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/cli.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/contenttype.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2503 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/cryptography_additions.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1412 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/linkformat.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     1200 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/linkformat_pygments.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     7029 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/prettyprint.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     4636 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/pyodide_websockets.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2126 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/socknumbers.py
--rw-rw-r--   0 erikg     (1000) erikg     (1000)      832 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/uri.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.401364 coapdialects-0.0.1/src/coapdialects/util/vendored/
--rw-rw-r--   0 erikg     (1000) erikg     (1000)    12359 2024-02-04 01:58:32.000000 coapdialects-0.0.1/src/coapdialects/util/vendored/link_header.py
-drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-04-28 21:20:07.401364 coapdialects-0.0.1/src/coapdialects.egg-info/
--rw-r--r--   0 erikg     (1000) erikg     (1000)      789 2024-04-28 21:20:07.000000 coapdialects-0.0.1/src/coapdialects.egg-info/PKG-INFO
--rw-rw-r--   0 erikg     (1000) erikg     (1000)     2900 2024-04-28 21:20:07.000000 coapdialects-0.0.1/src/coapdialects.egg-info/SOURCES.txt
--rw-rw-r--   0 erikg     (1000) erikg     (1000)        1 2024-04-28 21:20:07.000000 coapdialects-0.0.1/src/coapdialects.egg-info/dependency_links.txt
--rw-rw-r--   0 erikg     (1000) erikg     (1000)       13 2024-04-28 21:20:07.000000 coapdialects-0.0.1/src/coapdialects.egg-info/top_level.txt
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.069196 coapdialects-0.0.2/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1086 2024-04-28 18:52:03.000000 coapdialects-0.0.2/LICENSE
+-rw-r--r--   0 erikg     (1000) erikg     (1000)      789 2024-05-09 16:49:55.069196 coapdialects-0.0.2/PKG-INFO
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)       14 2024-04-28 18:52:03.000000 coapdialects-0.0.2/README.md
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      863 2024-05-09 16:48:24.000000 coapdialects-0.0.2/pyproject.toml
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)       38 2024-05-09 16:49:55.069196 coapdialects-0.0.2/setup.cfg
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.057190 coapdialects-0.0.2/src/
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.061192 coapdialects-0.0.2/src/coapdialects/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1075 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     4510 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/blockwise.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.065194 coapdialects-0.0.2/src/coapdialects/cli/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      515 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/cli/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    17334 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/cli/client.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5538 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/cli/common.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2158 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/cli/defaults.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    14554 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/cli/fileserver.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     6283 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/cli/proxy.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    29388 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/cli/rd.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    12589 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/credentials.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7793 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/defaults.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7233 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/error.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    20509 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/interfaces.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    27695 2024-05-09 16:48:05.000000 coapdialects-0.0.2/src/coapdialects/message.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    21127 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/messagemanager.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      670 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/meta.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.065194 coapdialects-0.0.2/src/coapdialects/numbers/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1425 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/numbers/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5275 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/numbers/codes.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5795 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/numbers/constants.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    12199 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/numbers/contentformat.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5534 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/numbers/optionnumbers.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      575 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/numbers/types.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     9296 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/options.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     8207 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/optiontypes.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    80685 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/oscore.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     6275 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/oscore_sitewrapper.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    13282 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/pipe.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    46714 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/protocol.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.065194 coapdialects-0.0.2/src/coapdialects/proxy/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      242 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/proxy/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1615 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/proxy/client.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    15717 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/proxy/server.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    17175 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/resource.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.065194 coapdialects-0.0.2/src/coapdialects/resourcedirectory/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      382 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/resourcedirectory/__init__.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.065194 coapdialects-0.0.2/src/coapdialects/resourcedirectory/client/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      304 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/resourcedirectory/client/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    13702 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/resourcedirectory/client/register.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    11199 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/tokenmanager.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.069196 coapdialects-0.0.2/src/coapdialects/transports/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      828 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2485 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/generic_udp.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    10545 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/oscore.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     8288 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/rfc8323common.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    11182 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/simple6.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7998 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/simplesocketserver.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    14842 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/tcp.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    14956 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/tinydtls.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    11343 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/tinydtls_server.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/tls.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    25068 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/udp6.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    17659 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/transports/ws.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.069196 coapdialects-0.0.2/src/coapdialects/util/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5844 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/__init__.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.069196 coapdialects-0.0.2/src/coapdialects/util/asyncio/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      486 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/asyncio/__init__.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     4126 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/asyncio/getaddrinfo_addrconfig.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     6703 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/asyncio/recvmsg.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1972 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/asyncio/timeoutdict.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     5687 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/cli.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1140 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/contenttype.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2503 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/cryptography_additions.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1412 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/linkformat.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     1200 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/linkformat_pygments.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     7029 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/prettyprint.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     4636 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/pyodide_websockets.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2126 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/socknumbers.py
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)      832 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/uri.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.069196 coapdialects-0.0.2/src/coapdialects/util/vendored/
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)    12359 2024-02-04 01:58:32.000000 coapdialects-0.0.2/src/coapdialects/util/vendored/link_header.py
+drwxrwxr-x   0 erikg     (1000) erikg     (1000)        0 2024-05-09 16:49:55.069196 coapdialects-0.0.2/src/coapdialects.egg-info/
+-rw-r--r--   0 erikg     (1000) erikg     (1000)      789 2024-05-09 16:49:55.000000 coapdialects-0.0.2/src/coapdialects.egg-info/PKG-INFO
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)     2490 2024-05-09 16:49:55.000000 coapdialects-0.0.2/src/coapdialects.egg-info/SOURCES.txt
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)        1 2024-05-09 16:49:55.000000 coapdialects-0.0.2/src/coapdialects.egg-info/dependency_links.txt
+-rw-rw-r--   0 erikg     (1000) erikg     (1000)       13 2024-05-09 16:49:55.000000 coapdialects-0.0.2/src/coapdialects.egg-info/top_level.txt
```

### Comparing `coapdialects-0.0.1/LICENSE` & `coapdialects-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/PKG-INFO` & `coapdialects-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coapdialects
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python aiocoap dialects
 Author-email: Erik Gonzalez <erikglez_ipn@hotmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ErikGlz/coapdialects
 Keywords: coap,asyncio,iot
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `coapdialects-0.0.1/pyproject.toml` & `coapdialects-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools >= 66.0" ]
 build-backend = "setuptools.build_meta"
  
 [project]
 name = "coapdialects"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python aiocoap dialects"
 readme = "README.md"
 authors = [
     { name = "Erik Gonzalez", email = "erikglez_ipn@hotmail.com" },
 ]
 license = { text = "MIT" }
 keywords = [ "coap", "asyncio", "iot" ]
```

### Comparing `coapdialects-0.0.1/src/coapdialects/__init__.py` & `coapdialects-0.0.2/src/coapdialects/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/blockwise.py` & `coapdialects-0.0.2/src/coapdialects/blockwise.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/cli/__init__.py` & `coapdialects-0.0.2/src/coapdialects/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/cli/client.py` & `coapdialects-0.0.2/src/coapdialects/cli/client.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/cli/common.py` & `coapdialects-0.0.2/src/coapdialects/cli/common.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/cli/defaults.py` & `coapdialects-0.0.2/src/coapdialects/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/cli/fileserver.py` & `coapdialects-0.0.2/src/coapdialects/cli/fileserver.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/cli/proxy.py` & `coapdialects-0.0.2/src/coapdialects/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/cli/rd.py` & `coapdialects-0.0.2/src/coapdialects/cli/rd.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/credentials.py` & `coapdialects-0.0.2/src/coapdialects/credentials.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/defaults.py` & `coapdialects-0.0.2/src/coapdialects/defaults.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/error.py` & `coapdialects-0.0.2/src/coapdialects/error.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/interfaces.py` & `coapdialects-0.0.2/src/coapdialects/interfaces.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/message.py` & `coapdialects-0.0.2/src/coapdialects/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,16 +234,16 @@
     def decode(cls, rawdata, remote=None):
         """Create Message object from binary representation of message."""
         try:
             (vttkl, code, mid) = struct.unpack('!BBH', rawdata[:4])
         except struct.error:
             raise error.UnparsableMessage("Incoming message too short for CoAP")
         version = (vttkl & 0xC0) >> 6
-        if version != 1:
-            raise error.UnparsableMessage("Fatal Error: Protocol Version must be 1")
+        #if version != 1:
+        #    raise error.UnparsableMessage("Fatal Error: Protocol Version must be 1")
         mtype = (vttkl & 0x30) >> 4
         token_length = (vttkl & 0x0F)
         msg = Message(mtype=mtype, mid=mid, code=code)
         msg.token = rawdata[4:4 + token_length]
         msg.payload = msg.opt.decode(rawdata[4 + token_length:])
         msg.remote = remote
         return msg
```

### Comparing `coapdialects-0.0.1/src/coapdialects/messagemanager.py` & `coapdialects-0.0.2/src/coapdialects/messagemanager.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/meta.py` & `coapdialects-0.0.2/src/coapdialects/meta.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/numbers/__init__.py` & `coapdialects-0.0.2/src/coapdialects/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/numbers/codes.py` & `coapdialects-0.0.2/src/coapdialects/numbers/codes.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/numbers/constants.py` & `coapdialects-0.0.2/src/coapdialects/numbers/constants.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/numbers/contentformat.py` & `coapdialects-0.0.2/src/coapdialects/numbers/contentformat.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/numbers/optionnumbers.py` & `coapdialects-0.0.2/src/coapdialects/numbers/optionnumbers.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/numbers/types.py` & `coapdialects-0.0.2/src/coapdialects/numbers/types.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/options.py` & `coapdialects-0.0.2/src/coapdialects/options.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/optiontypes.py` & `coapdialects-0.0.2/src/coapdialects/optiontypes.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/oscore.py` & `coapdialects-0.0.2/src/coapdialects/oscore.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/oscore_sitewrapper.py` & `coapdialects-0.0.2/src/coapdialects/oscore_sitewrapper.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/pipe.py` & `coapdialects-0.0.2/src/coapdialects/pipe.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/protocol.py` & `coapdialects-0.0.2/src/coapdialects/protocol.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/proxy/client.py` & `coapdialects-0.0.2/src/coapdialects/proxy/client.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/proxy/server.py` & `coapdialects-0.0.2/src/coapdialects/proxy/server.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/resource.py` & `coapdialects-0.0.2/src/coapdialects/resource.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/resource_coapcpv.py` & `coapdialects-0.0.2/src/coapdialects/transports/ws.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,432 +1,455 @@
 # SPDX-FileCopyrightText: Christian Amsüss and the aiocoap contributors
 #
 # SPDX-License-Identifier: MIT
 
-"""Basic resource implementations
-
-A resource in URL / CoAP / REST terminology is the thing identified by a URI.
-
-Here, a :class:`.Resource` is the place where server functionality is
-implemented. In many cases, there exists one persistent Resource object for a
-given resource (eg. a ``TimeResource()`` is responsible for serving the
-``/time`` location). On the other hand, an aiocoap server context accepts only
-one thing as its serversite, and that is a Resource too (typically of the
-:class:`Site` class).
-
-Resources are most easily implemented by deriving from :class:`.Resource` and
-implementing ``render_get``, ``render_post`` and similar coroutine methods.
-Those take a single request message object and must return a
-:class:`aiocoap.Message` object or raise an
-:class:`.error.RenderableError` (eg. ``raise UnsupportedMediaType()``).
-
-To serve more than one resource on a site, use the :class:`Site` class to
-dispatch requests based on the Uri-Path header.
 """
+This moduel implements a TokenInterface for `CoAP over WebSockets`_.
 
-import hashlib
-import warnings
-
-from .numbers import message_coapcpv
-from .numbers import meta
-from .numbers import error
-from .numbers import interfaces
-from .numbers import numbers
-from .pipe import Pipe
-
-def hashing_etag(request, response):
-    """Helper function for render_get handlers that allows them to use ETags based
-    on the payload's hash value
-
-    Run this on your request and response before returning from render_get; it is
-    safe to use this function with all kinds of responses, it will only act on
-    2.05 Content messages (and those with no code set, which defaults to that
-    for GET requests). The hash used are the first 8 bytes of the sha1 sum of
-    the payload.
-
-    Note that this method is not ideal from a server performance point of view
-    (a file server, for example, might want to hash only the stat() result of a
-    file instead of reading it in full), but it saves bandwith for the simple
-    cases.
-
-    >>> from aiocoap import *
-    >>> req = Message(code=GET)
-    >>> hash_of_hello = b'\\xaa\\xf4\\xc6\\x1d\\xdc\\xc5\\xe8\\xa2'
-    >>> req.opt.etags = [hash_of_hello]
-    >>> resp = Message(code=CONTENT)
-    >>> resp.payload = b'hello'
-    >>> hashing_etag(req, resp)
-    >>> resp                                            # doctest: +ELLIPSIS
-    <aiocoap.Message at ... 2.03 Valid ... 1 option(s)>
-    """
-
-    if response.code != numbers.codes.CONTENT and response.code is not None:
-        return
-
-    response.opt.etag = hashlib.sha1(response.payload).digest()[:8]
-    if request.opt.etags is not None and response.opt.etag in request.opt.etags:
-        response.code = numbers.codes.VALID
-        response.payload = b''
-
-class _ExposesWellknownAttributes:
-    def get_link_description(self):
-        # FIXME which formats are acceptable, and how much escaping and
-        # list-to-separated-string conversion needs to happen here
-        ret = {}
-        if hasattr(self, 'ct'):
-            ret['ct'] = str(self.ct)
-        if hasattr(self, 'rt'):
-            ret['rt'] = self.rt
-        if hasattr(self, 'if_'):
-            ret['if'] = self.if_
-        return ret
-
-class Resource(_ExposesWellknownAttributes, interfaces.Resource):
-    """Simple base implementation of the :class:`interfaces.Resource`
-    interface
-
-    The render method delegates content creation to ``render_$method`` methods
-    (``render_get``, ``render_put`` etc), and responds appropriately to
-    unsupported methods. Those messages may return messages without a response
-    code, the default render method will set an appropriate successful code
-    ("Content" for GET/FETCH, "Deleted" for DELETE, "Changed" for anything
-    else). The render method will also fill in the request's no_response code
-    into the response (see :meth:`.interfaces.Resource.render`) if none was
-    set.
-
-    Moreover, this class provides a ``get_link_description`` method as used by
-    .well-known/core to expose a resource's ``.ct``, ``.rt`` and ``.if_``
-    (alternative name for ``if`` as that's a Python keyword) attributes.
-    Details can be added by overriding the method to return a more
-    comprehensive dictionary, and resources can be hidden completely by
-    returning None.
-    """
-
-    async def needs_blockwise_assembly(self, request):
-        return True
-
-    async def render(self, request):
-        if not request.code.is_request():
-            raise error.UnsupportedMethod()
-        m = getattr(self, 'render_%s' % str(request.code).lower(), None)
-        if not m:
-            raise error.UnallowedMethod()
-
-        response = await m(request)
-
-        if response is message_coapcpv.NoResponse:
-            warnings.warn("Returning NoResponse is deprecated, please return a"
-                          " regular response with a no_response option set.",
-                          DeprecationWarning)
-            response = message_coapcpv.Message(no_response=26)
-
-        if response.code is None:
-            if request.code in (numbers.codes.GET, numbers.codes.FETCH):
-                response_default = numbers.codes.CONTENT
-            elif request.code == numbers.codes.DELETE:
-                response_default = numbers.codes.DELETED
-            else:
-                response_default = numbers.codes.CHANGED
-            response.code = response_default
-
-        if response.opt.no_response is None:
-            response.opt.no_response = request.opt.no_response
-
-        return response
-
-    async def render_to_pipe(self, request: Pipe):
-        # Silence the deprecation warning
-        if isinstance(self, interfaces.ObservableResource):
-            # See interfaces.Resource.render_to_pipe
-            return await interfaces.ObservableResource._render_to_pipe(self, request)
-        return await interfaces.Resource._render_to_pipe(self, request)
-
-class ObservableResource(Resource, interfaces.ObservableResource):
-    def __init__(self):
-        super(ObservableResource, self).__init__()
-        self._observations = set()
-
-    async def add_observation(self, request, serverobservation):
-        self._observations.add(serverobservation)
-        def _cancel(self=self, obs=serverobservation):
-            self._observations.remove(serverobservation)
-            self.update_observation_count(len(self._observations))
-        serverobservation.accept(_cancel)
-        self.update_observation_count(len(self._observations))
-
-    def update_observation_count(self, newcount):
-        """Hook into this method to be notified when the number of observations
-        on the resource changes."""
-
-    def updated_state(self, response=None):
-        """Call this whenever the resource was updated, and a notification
-        should be sent to observers."""
+.. _`CoAP over WebSockets`: https://tools.ietf.org/html/rfc8323#section-4
 
-        for o in self._observations:
-            o.trigger(response)
+As with CoAP-over-TCP, while the transport distinguishes a connection initiator
+("WebSocket (and TCP) client") and a receiver ("WebSocket (and TCP) server"),
+both sides can take both roles in CoAP (ie. as a CoAP server and a CoAP
+client). As the WebSocket client can not possibly be connected to (even by the
+same server -- once the connection is closed, it's gone and even a new one
+likely has a different port), aiocoap does not allow expressing their addresses
+in URIs (given they wouldn't serve their purpose as URLs and don't provide any
+stability either). Requests to a CoAP-over-WS client can be made by assigning
+the remote to an outgoing request.
+
+Port choice
+-----------
+
+Unlike the other transports, CoAP-over-WS is specified with a privileged port
+(port 80) as the default port. This is impractical for aiocoap servers for two
+reasons:
+
+    * Unless explicitly configured, aiocoap is typically run as an unprivileged
+      user (and has no provisions in place to receive a socket by other means
+      than opening it).
+
+    * Where a CoAP-over-WS proxy is run, there is often a "proper" website
+      running on the same port on a full HTTP server. That server is usually
+      capable of forwarding requests, whereas the ``websockets`` module used by
+      aiocoap is in no position to either serve websites nor to proxy to an
+      underlying server.
+
+The recommended setup is therefore to run a full web server at port 80, and
+configure it to proxy incoming requests for WebSockets at `/.well-known/coap`
+to aiocoap's server, which defaults to binding to port 8683.
+
+The port choice of outgoing connections, or the interpretation of the
+protocol's default port (ie. the port implied by ``coap+ws://hostname/``) is of
+course unaffected by this.
+
+.. warning::
+
+  Due to a shortcoming of aiocoap's way of specifying ports to bind
+  to, if a port is explicitly stated to bind to, CoAP-over-WS will bind to that
+  port plus 3000 (resulting in the abovementioned 8683 for 5683). If TLS server
+  keys are given, the TLS server is launched on the next port after the HTTP
+  server (typically 8684).
+
+Using on pyodide_
+-----------------
+
+When use  on pyodide_,
+instead of using the ``websockets`` module,
+a simplified client-only back-end is used,
+which utilizes the browser's WebSocket API.
 
-    def get_link_description(self):
-        link = super(ObservableResource, self).get_link_description()
-        link['obs'] = None
-        return link
+.. _pyodide: https://pyodide.org/
+"""
 
-    async def render_to_pipe(self, request: Pipe):
-        # Silence the deprecation warning
-        return await interfaces.ObservableResource._render_to_pipe(self, request)
+from __future__ import annotations
 
-def link_format_to_message(request, linkformat,
-        default_ct=numbers.ContentFormat.LINKFORMAT):
-    """Given a LinkFormat object, render it to a response message, picking a
-    suitable conent format from a given request.
+from typing import Dict, List
+from collections import namedtuple
+import asyncio
+import functools
+import http
+import weakref
+
+from aiocoap import Message, interfaces, ABORT, util, error
+from aiocoap.transports import rfc8323common
+from ..util.asyncio import py38args
+from ..defaults import is_pyodide
+
+if is_pyodide:
+    import aiocoap.util.pyodide_websockets as websockets
+else:
+    import websockets
+
+def _decode_message(data: bytes) -> Message:
+    codeoffset = 1
+    tokenoffset = 2
+
+    tkl = data[0]
+    if tkl > 8:
+        raise error.UnparsableMessage("Overly long token")
+    code = data[codeoffset]
+    token = data[tokenoffset:tokenoffset + tkl]
+
+    msg = Message(code=code, token=token)
+
+    msg.payload = msg.opt.decode(data[tokenoffset + tkl:])
+
+    return msg
+
+def _serialize(msg: Message) -> bytes:
+    tkl = len(msg.token)
+    if tkl > 8:
+        raise ValueError("Overly long token")
+
+    data = [
+            bytes((tkl, msg.code,)),
+            msg.token,
+            msg.opt.encode(),
+            ]
+    if msg.payload:
+        data += [b'\xff', msg.payload]
+
+    return b"".join(data)
+
+PoolKey = namedtuple("PoolKey", ("scheme", "hostinfo"))
+
+class WSRemote(rfc8323common.RFC8323Remote, interfaces.EndpointAddress):
+    _connection: websockets.WebSocketCommonProtocol
+    # Only used to ensure that remotes are associated to the right pool -- not
+    # that there'd be any good reason to have multiple of those.
+    _pool: weakref.ReferenceType[WSPool]
+
+    scheme = None # Override property -- it's per instance here
+
+    def __init__(self, pool, connection, loop, log, *, scheme, local_hostinfo=None, remote_hostinfo=None):
+        super().__init__()
+        self._pool = weakref.ref(pool)
+        self._connection = connection
+        self.loop = loop
+        self.log = log
 
-    It returns a Not Acceptable response if something unsupported was queried.
+        self._local_is_server = isinstance(connection, websockets.WebSocketServerProtocol)
 
-    It makes no attempt to modify the URI reference literals encoded in the
-    LinkFormat object; they have to be suitably prepared by the caller."""
+        if local_hostinfo is None:
+            self._local_hostinfo = self._connection.local_address[:2]
+        else:
+            self._local_hostinfo = local_hostinfo
+        if remote_hostinfo is None:
+            self._remote_hostinfo = self._connection.remote_address[:2]
+        else:
+            self._remote_hostinfo = remote_hostinfo
 
-    ct = request.opt.accept
-    if ct is None:
-        ct = default_ct
+        self.scheme = scheme
 
-    if ct == numbers.ContentFormat.LINKFORMAT:
-        payload = str(linkformat).encode('utf8')
-    else:
-        return message_coapcpv.Message(code=numbers.NOT_ACCEPTABLE)
+        # Goes both for client and for server ends; on the server end, it
+        # ensures that role reversal URIs can be used even when passed as URIs
+        # and not as remotes (although that's of course only possible locally).
+        self._poolkey = PoolKey(self.scheme, self.hostinfo)
+
+    # Necessary for RFC8323Remote
+
+    def _abort_with(self, msg, *, close_code=1002):
+        # Like _send_message, this may take actual time -- but unlike there,
+        # there's no need to regulate back-pressure
+        self.loop.create_task(
+                self._abort_with_waiting(msg, close_code=close_code),
+                **py38args(name="Abortion WebSocket sonnection with %r" % msg)
+                )
+
+    # Unlike _send_message, this is pulled out of the the _abort_with function
+    # as it's also used in _run_recv_loop
+    async def _abort_with_waiting(self, msg, *, close_code):
+        self.log.debug("Aborting with message: %r", msg)
+        try:
+            await self._connection.send(_serialize(msg))
+        except Exception as e:
+            self.log.error("Sending to a WebSocket should not raise errors", exc_info=e)
+        await self._connection.close(code=close_code)
+
+    def _send_message(self, msg):
+        # FIXME overhaul back-pressure model
+        async def send():
+            self.log.debug("Sending message: %r", msg)
+            try:
+                await self._connection.send(_serialize(msg))
+            except Exception as e:
+                self.log.error("Sending to a WebSocket should not raise errors", exc_info=e)
+        self.loop.create_task(
+                send(),
+                **py38args(name="WebSocket sending of %r" % msg)
+                )
 
-    return message_coapcpv.Message(payload=payload, content_format=ct)
+    async def release(self):
+        await super().release()
+        try:
+            await self._connection.wait_closed()
+        except asyncio.CancelledError:
+            self.log.warning(
+                    "Connection %s was not closed by peer in time after release",
+                    self
+                    )
+
+class WSPool(interfaces.TokenInterface):
+    _outgoing_starting: Dict[PoolKey, asyncio.Task]
+    _pool: Dict[PoolKey, WSRemote]
+
+    _servers: List[websockets.WebSocketServer]
+
+    def __init__(self, tman, log, loop):
+        self.loop = loop
+
+        self._pool = {}
+        self._outgoing_starting = {}
+
+        self._servers = []
+
+        # See where it is used for documentation, remove when not needed any more
+        self._in_shutdown = False
+
+        self._tokenmanager = tman
+        self.log = log
+
+    @classmethod
+    async def create_transport(cls, tman: interfaces.TokenManager, log, loop, *, client_credentials, server_bind=None, server_context=None):
+        self = cls(tman, log, loop)
+
+        self._client_credentials = client_credentials
+
+        if server_bind:
+            host, port = server_bind
+            if port is None:
+                port = 8683
+            elif port != 0:
+                # FIXME see module documentation
+                port = port + 3000
+
+            server = await websockets.serve(
+                    functools.partial(self._new_connection, scheme='coap+ws'),
+                    host, port,
+                    subprotocols=['coap'],
+                    process_request=self._process_request,
+                    ping_interval=None, # "SHOULD NOT be used"
+                    )
+            self._servers.append(server)
+
+            if server_context is not None:
+                server = await websockets.serve(
+                        functools.partial(self._new_connection, scheme='coaps+ws'),
+                        host, port + 1,
+                        subprotocols=['coap'],
+                        process_request=self._process_request,
+                        ping_interval=None, # "SHOULD NOT be used"
+                        ssl=server_context,
+                        )
+                self._servers.append(server)
+
+        return self
+
+    # Helpers for WebScoket server
+
+    async def _new_connection(self, websocket, path=None, *, scheme):
+        # ignoring path: Already checked in _process_request
+        #
+        # (path is present up to 10.0 and absent in 10.1; keeping it around to
+        # stay compatible with different versions).
+
+        hostheader = websocket.request_headers['Host']
+        if hostheader.count(':') > 1 and '[' not in hostheader:
+            # Workaround for websockets version before
+            # https://github.com/aaugustin/websockets/issues/802
+            #
+            # To be removed once a websockets version with this fix can be
+            # depended on
+            hostheader = '[' + hostheader[:hostheader.rfind(':')] + ']' + hostheader[hostheader.rfind(':'):]
+        local_hostinfo = util.hostportsplit(hostheader)
+
+        remote = WSRemote(self, websocket, self.loop, self.log, scheme=scheme, local_hostinfo=local_hostinfo)
+        self._pool[remote._poolkey] = remote
+
+        await self._run_recv_loop(remote)
+
+    @staticmethod
+    async def _process_request(path, request_headers):
+        if path != '/.well-known/coap':
+            return (http.HTTPStatus.NOT_FOUND, [], b"")
+        # Continue with WebSockets
+        return None
+
+    # Helpers for WebScoket client
+
+    def _connect(self, key: PoolKey):
+        self._outgoing_starting[key] = self.loop.create_task(
+                self._connect_task(key),
+                **py38args(name="WebSocket connection opening to %r" % (key,))
+                )
 
-# Convenience attribute to set as ct on resources that use
-# link_format_to_message as their final step in the request handler
-link_format_to_message.supported_ct = " ".join(str(int(x)) for x in (
-        numbers.ContentFormat.LINKFORMAT,
-        ))
+    async def _connect_task(self, key: PoolKey):
+        try:
+            ssl_context = self._client_credentials.ssl_client_context(key.scheme, key.hostinfo)
 
-class WKCResource(Resource):
-    """Read-only dynamic resource list, suitable as .well-known/core.
+            hostinfo_split = util.hostportsplit(key.hostinfo)
 
-    This resource renders a link_header.LinkHeader object (which describes a
-    collection of resources) as application/link-format (RFC 6690).
+            ws_scheme = {'coap+ws': 'ws', 'coaps+ws': 'wss'}[key.scheme]
 
-    The list to be rendered is obtained from a function passed into the
-    constructor; typically, that function would be a bound
-    Site.get_resources_as_linkheader() method.
+            if ws_scheme == 'ws' and ssl_context is not None:
+                raise ValueError("An SSL context was provided for a remote accessed via a plaintext websockets.")
+            if ws_scheme == 'wss':
+                if is_pyodide:
+                    if ssl_context is not None:
+                        raise ValueError("The pyodide websocket implementation can't be configured with a non-default context -- connections created in a browser will always use the browser's CA set.")
+                else:
+                    if ssl_context is None:
+                        # Like with TLSClient, we need to pass in a default
+                        # context and can't rely on the websocket library to
+                        # use a default one when wss is requested (it doesn't)
+                        import ssl
+                        ssl_context = ssl.create_default_context()
+
+            websocket = await websockets.connect("%s://%s/.well-known/coap" % (
+                ws_scheme, key.hostinfo),
+                subprotocols=['coap'],
+                ping_interval=None,
+                ssl=ssl_context,
+                )
+
+            remote = WSRemote(self, websocket, self.loop, self.log, scheme=key.scheme, remote_hostinfo=hostinfo_split)
+            assert remote._poolkey == key, "Pool key construction is inconsistent"
+            self._pool[key] = remote
+
+            self.loop.create_task(
+                    self._run_recv_loop(remote),
+                    **py38args(name="WebSocket receive loop for %r" % (key,))
+                    )
+
+            return remote
+        finally:
+            del self._outgoing_starting[key]
+
+    # Implementation of TokenInterface
+
+    async def fill_or_recognize_remote(self, message):
+        if isinstance(message.remote, WSRemote) and \
+                message.remote._pool() is self:
+            return True
 
-    This resource also provides server `implementation information link`_;
-    server authors are invited to override this by passing an own URI as the
-    `impl_info` parameter, and can disable it by passing None.
+        if message.requested_scheme in ('coap+ws', 'coaps+ws'):
+            key = PoolKey(message.requested_scheme, message.remote.hostinfo)
 
-    .. _`implementation information link`: https://tools.ietf.org/html/draft-bormann-t2trg-rel-impl-00"""
+            if key in self._pool:
+                message.remote = self._pool[key]
+                if message.remote._connection.open:
+                    return True
+                # else try opening a new one
+
+            if key not in self._outgoing_starting:
+                self._connect(key)
+            # It's a bit unorthodox to wait for an (at least partially)
+            # established connection in fill_or_recognize_remote, but it's
+            # not completely off off either, and it makes it way easier to
+            # not have partially initialized remotes around
+            message.remote = await self._outgoing_starting[key]
+            return True
 
-    ct = link_format_to_message.supported_ct
+        return False
 
-    def __init__(self, listgenerator, impl_info=meta.library_uri, **kwargs):
-        super().__init__(**kwargs)
-        self.listgenerator = listgenerator
-        self.impl_info = impl_info
+    def send_message(self, message, messageerror_monitor):
+        # Ignoring messageerror_monitor: CoAP over reliable transports has no
+        # way of indicating that a particular message was bad, it always shuts
+        # down the complete connection
+
+        if message.code.is_response():
+            no_response = (message.opt.no_response or 0) & (1 << message.code.class_ - 1) != 0
+            if no_response:
+                return
+
+        message.opt.no_response = None
+
+        message.remote._send_message(message)
+
+    async def shutdown(self):
+        self._in_shutdown = True
+        self.log.debug("Shutting down any connections on %r", self)
+
+        client_shutdowns = [
+            asyncio.create_task(
+                c.release(),
+                **py38args(name="Close connection %s" % c)
+            )
+            for c in self._pool.values()]
+
+        server_shutdowns = []
+        while self._servers:
+            s = self._servers.pop()
+            # We could do something like
+            # >>> for websocket in s.websockets:
+            # >>>     del websocket.logger.extra['websocket']
+            # to reduce the reference loops
+            # (websocket.logger.extra['websocket'] == websocket), but as the
+            # tests actually do run a GC collection once and that gets broken
+            # up, it's not worth adding fragilty here
+            s.close()
+            server_shutdowns.append(asyncio.create_task(
+                s.wait_closed(),
+                **py38args(name="Close server %s" % s)))
+
+        # Placing client shutdowns before server shutdowns to give them a
+        # chance to send out Abort messages; the .close() method could be more
+        # helpful here by stopping new connections but letting us finish off
+        # the old ones
+        shutdowns = client_shutdowns + server_shutdowns
+        if shutdowns:
+            # wait is documented to require a non-empty set
+            await asyncio.wait(shutdowns)
 
-    async def render_get(self, request):
-        links = self.listgenerator()
+    # Incoming message processing
 
-        if self.impl_info is not None:
-            from .util.linkformat import Link
-            links.links = links.links + [Link(href=self.impl_info, rel="impl-info")]
+    async def _run_recv_loop(self, remote):
+        remote._send_initial_csm()
 
-        filters = []
-        for q in request.opt.uri_query:
+        while True:
             try:
-                k, v = q.split('=', 1)
-            except ValueError:
-                continue # no =, not a relevant filter
-
-            if v.endswith('*'):
-                def matchexp(x, v=v):
-                    return x.startswith(v[:-1])
-            else:
-                def matchexp(x, v=v):
-                    return x == v
-
-            if k in ('rt', 'if', 'ct'):
-                filters.append(lambda link: any(matchexp(part) for part in (" ".join(getattr(link, k, ()))).split(" ")))
-            elif k in ('href',): # x.href is single valued
-                filters.append(lambda link: matchexp(getattr(link, k)))
-            else:
-                filters.append(lambda link: any(matchexp(part) for part in getattr(link, k, ())))
-
-        while filters:
-            links.links = filter(filters.pop(), links.links)
-        links.links = list(links.links)
-
-        response = link_format_to_message(request, links)
-
-        if request.opt.uri_query and not links.links and \
-                request.remote.is_multicast_locally:
-            if request.opt.no_response is None:
-                # If the filter does not match, multicast requests should not
-                # be responded to -- that's equivalent to a "no_response on
-                # 2.xx" option.
-                response.opt.no_response = 0x02
-
-        return response
-
-class PathCapable:
-    """Class that indicates that a resource promises to parse the uri_path
-    option, and can thus be given requests for :meth:`.render`-ing that
-    contain a uri_path"""
-
-class Site(interfaces.ObservableResource, PathCapable):
-    """Typical root element that gets passed to a :class:`Context` and contains
-    all the resources that can be found when the endpoint gets accessed as a
-    server.
-
-    This provides easy registration of statical resources. Add resources at
-    absolute locations using the :meth:`.add_resource` method.
-
-    For example, the site at
-
-    >>> site = Site()
-    >>> site.add_resource(["hello"], Resource())
-
-    will have requests to </hello> rendered by the new resource.
-
-    You can add another Site (or another instance of :class:`PathCapable`) as
-    well, those will be nested and integrally reported in a WKCResource. The
-    path of a site should not end with an empty string (ie. a slash in the URI)
-    -- the child site's own root resource will then have the trailing slash
-    address.  Subsites can not have link-header attributes on their own (eg.
-    `rt`) and will never respond to a request that does not at least contain a
-    single slash after the the given path part.
-
-    For example,
-
-    >>> batch = Site()
-    >>> batch.add_resource(["light1"], Resource())
-    >>> batch.add_resource(["light2"], Resource())
-    >>> batch.add_resource([], Resource())
-    >>> s = Site()
-    >>> s.add_resource(["batch"], batch)
-
-    will have the three created resources rendered at </batch/light1>,
-    </batch/light2> and </batch/>.
-
-    If it is necessary to respond to requests to </batch> or report its
-    attributes in .well-known/core in addition to the above, a non-PathCapable
-    resource can be added with the same path. This is usually considered an odd
-    design, not fully supported, and for example doesn't support removal of
-    resources from the site.
-    """
-
-    def __init__(self):
-        self._resources = {}
-        self._subsites = {}
-
-    async def needs_blockwise_assembly(self, request):
-        try:
-            child, subrequest = self._find_child_and_pathstripped_message(request)
-        except KeyError:
-            return True
-        else:
-            return await child.needs_blockwise_assembly(subrequest)
-
-    def _find_child_and_pathstripped_message(self, request):
-        """Given a request, find the child that will handle it, and strip all
-        path components from the request that are covered by the child's
-        position within the site. Returns the child and a request with a path
-        shortened by the components in the child's path, or raises a
-        KeyError.
-
-        While producing stripped messages, this adds a ._original_request_uri
-        attribute to the messages which holds the request URI before the
-        stripping is started. That allows internal components to access the
-        original URI until there is a variation of the request API that allows
-        accessing this in a better usable way."""
-
-        original_request_uri = getattr(request, '_original_request_uri',
-                request.get_request_uri(local_is_server=True))
-
-        if request.opt.uri_path in self._resources:
-            stripped = request.copy(uri_path=())
-            stripped._original_request_uri = original_request_uri
-            return self._resources[request.opt.uri_path], stripped
-
-        if not request.opt.uri_path:
-            raise KeyError()
-
-        remainder = [request.opt.uri_path[-1]]
-        path = request.opt.uri_path[:-1]
-        while path:
-            if path in self._subsites:
-                res = self._subsites[path]
-                if remainder == [""]:
-                    # sub-sites should see their root resource like sites
-                    remainder = []
-                stripped = request.copy(uri_path=remainder)
-                stripped._original_request_uri = original_request_uri
-                return res, stripped
-            remainder.insert(0, path[-1])
-            path = path[:-1]
-        raise KeyError()
-
-    async def render(self, request):
-        try:
-            child, subrequest = self._find_child_and_pathstripped_message(request)
-        except KeyError:
-            raise error.NotFound()
-        else:
-            return await child.render(subrequest)
-
-    async def add_observation(self, request, serverobservation):
-        try:
-            child, subrequest = self._find_child_and_pathstripped_message(request)
-        except KeyError:
-            return
+                received = await remote._connection.recv()
+            except websockets.exceptions.ConnectionClosed:
+                # This check is purely needed to silence the warning printed
+                # from tokenmanager, "Internal shutdown sequence msismatch:
+                # error dispatched through tokenmanager after shutdown" -- and
+                # is a symptom of https://github.com/chrysn/aiocoap/issues/284
+                # and of the odd circumstance that we can't easily cancel the
+                # _run_recv_loop tasks (as we should while that issue is
+                # unresolved) in the shutdown handler.
+                if not self._in_shutdown:
+                    # FIXME if deposited somewhere, mark that as stale?
+                    self._tokenmanager.dispatch_error(error.RemoteServerShutdown("Peer closed connection"), remote)
+                return
+
+            if not isinstance(received, bytes):
+                await remote._abort_with_waiting(Message(code=ABORT, payload=b"Text frame received"), close_code=1003)
+                return
 
-        try:
-            await child.add_observation(subrequest, serverobservation)
-        except AttributeError:
-            pass
-
-    def add_resource(self, path, resource):
-        if isinstance(path, str):
-            raise ValueError("Paths should be tuples or lists of strings")
-        if isinstance(resource, PathCapable):
-            self._subsites[tuple(path)] = resource
-        else:
-            self._resources[tuple(path)] = resource
-
-    def remove_resource(self, path):
-        try:
-            del self._subsites[tuple(path)]
-        except KeyError:
-            del self._resources[tuple(path)]
-
-    def get_resources_as_linkheader(self):
-        from .util.linkformat import Link, LinkFormat
-
-        links = []
-
-        for path, resource in self._resources.items():
-            if hasattr(resource, "get_link_description"):
-                details = resource.get_link_description()
-            else:
-                details = {}
-            if details is None:
+            try:
+                msg = _decode_message(received)
+            except error.UnparsableMessage:
+                await remote._abort_with_waiting(Message(code=ABORT, payload=b"Message parsing error"), close_code=1007)
+                return
+
+            msg.remote = remote
+
+            if msg.code.is_signalling():
+                try:
+                    remote._process_signaling(msg)
+                except rfc8323common.CloseConnection as e:
+                    self._tokenmanager.dispatch_error(e.args[0], msg.remote)
+                    self._pool.pop(remote._poolkey)
+                    await remote._connection.close()
                 continue
-            lh = Link('/' + '/'.join(path), **details)
 
-            links.append(lh)
-
-        for path, resource in self._subsites.items():
-            if hasattr(resource, "get_resources_as_linkheader"):
-                for l in resource.get_resources_as_linkheader().links:
-                    links.append(Link('/' + '/'.join(path) + l.href, l.attr_pairs))
-        return LinkFormat(links)
-
-    async def render_to_pipe(self, request: Pipe):
-        try:
-            child, subrequest = self._find_child_and_pathstripped_message(request.request)
-        except KeyError:
-            raise error.NotFound()
-        else:
-            # FIXME consider carefully whether this switching-around is good.
-            # It probably is.
-            request.request = subrequest
-            return await child.render_to_pipe(request)
+            if remote._remote_settings is None:
+                remote.abort("No CSM received")
+                return
+
+            if msg.code.is_response():
+                self._tokenmanager.process_response(msg)
+                # ignoring the return value; unexpected responses can be the
+                # asynchronous result of cancelled observations
+            else:
+                self._tokenmanager.process_request(msg)
```

### Comparing `coapdialects-0.0.1/src/coapdialects/resourcedirectory/client/register.py` & `coapdialects-0.0.2/src/coapdialects/resourcedirectory/client/register.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/tokenmanager.py` & `coapdialects-0.0.2/src/coapdialects/tokenmanager.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/__init__.py` & `coapdialects-0.0.2/src/coapdialects/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/generic_udp.py` & `coapdialects-0.0.2/src/coapdialects/transports/generic_udp.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/oscore.py` & `coapdialects-0.0.2/src/coapdialects/transports/oscore.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/rfc8323common.py` & `coapdialects-0.0.2/src/coapdialects/transports/rfc8323common.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/simple6.py` & `coapdialects-0.0.2/src/coapdialects/transports/simple6.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/simplesocketserver.py` & `coapdialects-0.0.2/src/coapdialects/transports/simplesocketserver.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/tcp.py` & `coapdialects-0.0.2/src/coapdialects/transports/tcp.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/tinydtls.py` & `coapdialects-0.0.2/src/coapdialects/transports/tinydtls.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/tinydtls_server.py` & `coapdialects-0.0.2/src/coapdialects/transports/tinydtls_server.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/tls.py` & `coapdialects-0.0.2/src/coapdialects/transports/tls.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/transports/udp6.py` & `coapdialects-0.0.2/src/coapdialects/transports/udp6.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/__init__.py` & `coapdialects-0.0.2/src/coapdialects/util/__init__.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/asyncio/getaddrinfo_addrconfig.py` & `coapdialects-0.0.2/src/coapdialects/util/asyncio/getaddrinfo_addrconfig.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/asyncio/recvmsg.py` & `coapdialects-0.0.2/src/coapdialects/util/asyncio/recvmsg.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/asyncio/timeoutdict.py` & `coapdialects-0.0.2/src/coapdialects/util/asyncio/timeoutdict.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/cli.py` & `coapdialects-0.0.2/src/coapdialects/util/cli.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/contenttype.py` & `coapdialects-0.0.2/src/coapdialects/util/contenttype.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/cryptography_additions.py` & `coapdialects-0.0.2/src/coapdialects/util/cryptography_additions.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/linkformat.py` & `coapdialects-0.0.2/src/coapdialects/util/linkformat.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/linkformat_pygments.py` & `coapdialects-0.0.2/src/coapdialects/util/linkformat_pygments.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/prettyprint.py` & `coapdialects-0.0.2/src/coapdialects/util/prettyprint.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/pyodide_websockets.py` & `coapdialects-0.0.2/src/coapdialects/util/pyodide_websockets.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/socknumbers.py` & `coapdialects-0.0.2/src/coapdialects/util/socknumbers.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/uri.py` & `coapdialects-0.0.2/src/coapdialects/util/uri.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects/util/vendored/link_header.py` & `coapdialects-0.0.2/src/coapdialects/util/vendored/link_header.py`

 * *Files identical despite different names*

### Comparing `coapdialects-0.0.1/src/coapdialects.egg-info/PKG-INFO` & `coapdialects-0.0.2/src/coapdialects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coapdialects
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python aiocoap dialects
 Author-email: Erik Gonzalez <erikglez_ipn@hotmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ErikGlz/coapdialects
 Keywords: coap,asyncio,iot
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
```

### Comparing `coapdialects-0.0.1/src/coapdialects.egg-info/SOURCES.txt` & `coapdialects-0.0.2/src/coapdialects.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,52 +4,41 @@
 src/coapdialects/__init__.py
 src/coapdialects/blockwise.py
 src/coapdialects/credentials.py
 src/coapdialects/defaults.py
 src/coapdialects/error.py
 src/coapdialects/interfaces.py
 src/coapdialects/message.py
-src/coapdialects/message_coapcpv.py
-src/coapdialects/message_coaprcs.py
-src/coapdialects/message_coapts.py
 src/coapdialects/messagemanager.py
 src/coapdialects/meta.py
 src/coapdialects/options.py
 src/coapdialects/optiontypes.py
 src/coapdialects/oscore.py
 src/coapdialects/oscore_sitewrapper.py
 src/coapdialects/pipe.py
 src/coapdialects/protocol.py
-src/coapdialects/protocol_coapcpv.py
-src/coapdialects/protocol_coaprcs.py
-src/coapdialects/protocol_coapts.py
 src/coapdialects/resource.py
-src/coapdialects/resource_coapcpv.py
-src/coapdialects/resource_coaprcs.py
-src/coapdialects/resource_coapts.py
 src/coapdialects/tokenmanager.py
 src/coapdialects.egg-info/PKG-INFO
 src/coapdialects.egg-info/SOURCES.txt
 src/coapdialects.egg-info/dependency_links.txt
 src/coapdialects.egg-info/top_level.txt
 src/coapdialects/cli/__init__.py
 src/coapdialects/cli/client.py
 src/coapdialects/cli/common.py
 src/coapdialects/cli/defaults.py
 src/coapdialects/cli/fileserver.py
 src/coapdialects/cli/proxy.py
 src/coapdialects/cli/rd.py
 src/coapdialects/numbers/__init__.py
 src/coapdialects/numbers/codes.py
-src/coapdialects/numbers/codes_coaprcs.py
 src/coapdialects/numbers/constants.py
 src/coapdialects/numbers/contentformat.py
 src/coapdialects/numbers/optionnumbers.py
 src/coapdialects/numbers/types.py
-src/coapdialects/numbers/types_coapts.py
 src/coapdialects/proxy/__init__.py
 src/coapdialects/proxy/client.py
 src/coapdialects/proxy/server.py
 src/coapdialects/resourcedirectory/__init__.py
 src/coapdialects/resourcedirectory/client/__init__.py
 src/coapdialects/resourcedirectory/client/register.py
 src/coapdialects/transports/__init__.py
```


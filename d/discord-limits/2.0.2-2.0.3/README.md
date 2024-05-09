# Comparing `tmp/discord_limits-2.0.2.tar.gz` & `tmp/discord_limits-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_limits-2.0.2.tar", last modified: Fri Apr 26 04:25:56 2024, max compression
+gzip compressed data, was "discord_limits-2.0.3.tar", last modified: Thu May  9 17:03:59 2024, max compression
```

## Comparing `discord_limits-2.0.2.tar` & `discord_limits-2.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 04:25:56.969343 discord_limits-2.0.2/
--rw-rw-rw-   0        0        0     1088 2022-05-06 09:44:00.000000 discord_limits-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     1143 2024-04-26 04:25:56.968842 discord_limits-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      819 2024-04-26 04:24:19.000000 discord_limits-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 04:25:56.927230 discord_limits-2.0.2/discord_limits/
--rw-rw-rw-   0        0        0      191 2024-04-26 04:24:51.000000 discord_limits-2.0.2/discord_limits/__init__.py
--rw-rw-rw-   0        0        0     9715 2024-04-26 04:23:53.000000 discord_limits-2.0.2/discord_limits/client.py
--rw-rw-rw-   0        0        0      863 2024-04-26 02:09:02.000000 discord_limits-2.0.2/discord_limits/errors.py
--rw-rw-rw-   0        0        0     1283 2024-04-26 03:33:26.000000 discord_limits-2.0.2/discord_limits/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-26 04:25:56.967340 discord_limits-2.0.2/discord_limits/paths/
--rw-rw-rw-   0        0        0      499 2024-04-10 17:52:46.000000 discord_limits-2.0.2/discord_limits/paths/__init__.py
--rw-rw-rw-   0        0        0    10829 2024-04-26 00:13:39.000000 discord_limits-2.0.2/discord_limits/paths/applicationPaths.py
--rw-rw-rw-   0        0        0     1735 2024-04-25 13:16:04.000000 discord_limits-2.0.2/discord_limits/paths/auditPaths.py
--rw-rw-rw-   0        0        0     3884 2024-04-25 13:16:29.000000 discord_limits-2.0.2/discord_limits/paths/autoModerationPaths.py
--rw-rw-rw-   0        0        0    38917 2024-04-26 04:23:53.000000 discord_limits-2.0.2/discord_limits/paths/channelPaths.py
--rw-rw-rw-   0        0        0     3856 2024-04-26 02:49:01.000000 discord_limits-2.0.2/discord_limits/paths/emojiPaths.py
--rw-rw-rw-   0        0        0    54345 2024-04-25 13:52:49.000000 discord_limits-2.0.2/discord_limits/paths/guildPaths.py
--rw-rw-rw-   0        0        0     9702 2024-04-25 14:47:20.000000 discord_limits-2.0.2/discord_limits/paths/interationsPaths.py
--rw-rw-rw-   0        0        0     2318 2024-04-25 14:43:34.000000 discord_limits-2.0.2/discord_limits/paths/invitePaths.py
--rw-rw-rw-   0        0        0     5059 2024-04-25 14:45:12.000000 discord_limits-2.0.2/discord_limits/paths/paths.py
--rw-rw-rw-   0        0        0     3457 2024-04-25 14:47:56.000000 discord_limits-2.0.2/discord_limits/paths/stagePaths.py
--rw-rw-rw-   0        0        0     4512 2024-04-25 14:51:36.000000 discord_limits-2.0.2/discord_limits/paths/stickerPaths.py
--rw-rw-rw-   0        0        0     5247 2024-04-26 00:13:14.000000 discord_limits-2.0.2/discord_limits/paths/userPaths.py
--rw-rw-rw-   0        0        0    13305 2024-04-26 00:13:01.000000 discord_limits-2.0.2/discord_limits/paths/webhookPaths.py
--rw-rw-rw-   0        0        0     1826 2024-04-26 04:23:53.000000 discord_limits-2.0.2/discord_limits/rate_limits.py
-drwxrwxrwx   0        0        0        0 2024-04-26 04:25:56.952787 discord_limits-2.0.2/discord_limits.egg-info/
--rw-rw-rw-   0        0        0     1143 2024-04-26 04:25:56.000000 discord_limits-2.0.2/discord_limits.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      873 2024-04-26 04:25:56.000000 discord_limits-2.0.2/discord_limits.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 04:25:56.000000 discord_limits-2.0.2/discord_limits.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-26 04:25:56.000000 discord_limits-2.0.2/discord_limits.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-26 04:25:56.000000 discord_limits-2.0.2/discord_limits.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       89 2024-04-26 03:43:46.000000 discord_limits-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 04:25:56.969843 discord_limits-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      699 2024-04-26 04:24:43.000000 discord_limits-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:03:59.426303 discord_limits-2.0.3/
+-rw-rw-rw-   0        0        0     1088 2022-05-06 09:44:00.000000 discord_limits-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1208 2024-05-09 17:03:59.422861 discord_limits-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      819 2024-05-09 16:56:38.000000 discord_limits-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 17:03:59.323145 discord_limits-2.0.3/discord_limits/
+-rw-rw-rw-   0        0        0      191 2024-05-09 16:55:41.000000 discord_limits-2.0.3/discord_limits/__init__.py
+-rw-rw-rw-   0        0        0     9688 2024-05-09 16:55:27.000000 discord_limits-2.0.3/discord_limits/client.py
+-rw-rw-rw-   0        0        0      863 2024-04-26 02:09:02.000000 discord_limits-2.0.3/discord_limits/errors.py
+-rw-rw-rw-   0        0        0     1283 2024-04-26 03:33:26.000000 discord_limits-2.0.3/discord_limits/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:03:59.416666 discord_limits-2.0.3/discord_limits/paths/
+-rw-rw-rw-   0        0        0      499 2024-04-10 17:52:46.000000 discord_limits-2.0.3/discord_limits/paths/__init__.py
+-rw-rw-rw-   0        0        0    10829 2024-04-26 00:13:39.000000 discord_limits-2.0.3/discord_limits/paths/applicationPaths.py
+-rw-rw-rw-   0        0        0     1735 2024-04-25 13:16:04.000000 discord_limits-2.0.3/discord_limits/paths/auditPaths.py
+-rw-rw-rw-   0        0        0     3884 2024-04-25 13:16:29.000000 discord_limits-2.0.3/discord_limits/paths/autoModerationPaths.py
+-rw-rw-rw-   0        0        0    38917 2024-04-26 04:23:53.000000 discord_limits-2.0.3/discord_limits/paths/channelPaths.py
+-rw-rw-rw-   0        0        0     3856 2024-04-26 02:49:01.000000 discord_limits-2.0.3/discord_limits/paths/emojiPaths.py
+-rw-rw-rw-   0        0        0    54345 2024-04-25 13:52:49.000000 discord_limits-2.0.3/discord_limits/paths/guildPaths.py
+-rw-rw-rw-   0        0        0     9702 2024-04-25 14:47:20.000000 discord_limits-2.0.3/discord_limits/paths/interationsPaths.py
+-rw-rw-rw-   0        0        0     2318 2024-04-25 14:43:34.000000 discord_limits-2.0.3/discord_limits/paths/invitePaths.py
+-rw-rw-rw-   0        0        0     5059 2024-04-25 14:45:12.000000 discord_limits-2.0.3/discord_limits/paths/paths.py
+-rw-rw-rw-   0        0        0     3457 2024-04-25 14:47:56.000000 discord_limits-2.0.3/discord_limits/paths/stagePaths.py
+-rw-rw-rw-   0        0        0     4512 2024-04-25 14:51:36.000000 discord_limits-2.0.3/discord_limits/paths/stickerPaths.py
+-rw-rw-rw-   0        0        0     5247 2024-04-26 00:13:14.000000 discord_limits-2.0.3/discord_limits/paths/userPaths.py
+-rw-rw-rw-   0        0        0    13305 2024-04-26 00:13:01.000000 discord_limits-2.0.3/discord_limits/paths/webhookPaths.py
+-rw-rw-rw-   0        0        0     1826 2024-04-26 04:23:53.000000 discord_limits-2.0.3/discord_limits/rate_limits.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:03:59.419967 discord_limits-2.0.3/discord_limits.egg-info/
+-rw-rw-rw-   0        0        0     1208 2024-05-09 17:03:59.000000 discord_limits-2.0.3/discord_limits.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      873 2024-05-09 17:03:59.000000 discord_limits-2.0.3/discord_limits.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 17:03:59.000000 discord_limits-2.0.3/discord_limits.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-09 17:03:59.000000 discord_limits-2.0.3/discord_limits.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 17:03:59.000000 discord_limits-2.0.3/discord_limits.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       89 2024-04-26 03:43:46.000000 discord_limits-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 17:03:59.427325 discord_limits-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      699 2024-05-09 17:03:44.000000 discord_limits-2.0.3/setup.py
```

### Comparing `discord_limits-2.0.2/LICENSE` & `discord_limits-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/PKG-INFO` & `discord_limits-2.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: discord_limits
-Version: 2.0.2
+Version: 2.0.3
 Summary: Make Discord API calls without having to worry about ratelimits.
 Home-page: https://github.com/ninjafella/discord-API-limits
 Author: ninjafella
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiolimiter==1.1.0
+Requires-Dist: aiohttp==3.9.5
 
 [![Documentation Status]](https://discord-limits.readthedocs.io/en/latest/?badge=latest)
-[![Version](https://img.shields.io/badge/Version-v2.0.2-blue)](https://img.shields.io/badge/Version-v2.0.2-blue)
+[![Version](https://img.shields.io/badge/Version-v2.0.3-blue)](https://img.shields.io/badge/Version-v2.0.3-blue)
 
 # discord_limits
 
 ### A simple library to asynchronously make API requests to Discord without having to worry about ratelimits.
 
 <br>
```

### Comparing `discord_limits-2.0.2/README.md` & `discord_limits-2.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Documentation Status]](https://discord-limits.readthedocs.io/en/latest/?badge=latest)
-[![Version](https://img.shields.io/badge/Version-v2.0.2-blue)](https://img.shields.io/badge/Version-v2.0.2-blue)
+[![Version](https://img.shields.io/badge/Version-v2.0.3-blue)](https://img.shields.io/badge/Version-v2.0.3-blue)
 
 # discord_limits
 
 ### A simple library to asynchronously make API requests to Discord without having to worry about ratelimits.
 
 <br>
```

### Comparing `discord_limits-2.0.2/discord_limits/client.py` & `discord_limits-2.0.3/discord_limits/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import warnings
 import datetime
 from sys import version_info as python_version
 
 from aiohttp import ClientResponse, ClientSession
 from aiohttp import __version__ as aiohttp_version
 from aiolimiter import AsyncLimiter
-from requests import head
 
 from . import __version__
 from .errors import *
 from .paths import Paths
 from .rate_limits import BucketHandler, ClientRateLimits
 
 from typing import Optional
```

### Comparing `discord_limits-2.0.2/discord_limits/errors.py` & `discord_limits-2.0.3/discord_limits/errors.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/helpers.py` & `discord_limits-2.0.3/discord_limits/helpers.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/applicationPaths.py` & `discord_limits-2.0.3/discord_limits/paths/applicationPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/auditPaths.py` & `discord_limits-2.0.3/discord_limits/paths/auditPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/autoModerationPaths.py` & `discord_limits-2.0.3/discord_limits/paths/autoModerationPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/channelPaths.py` & `discord_limits-2.0.3/discord_limits/paths/channelPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/emojiPaths.py` & `discord_limits-2.0.3/discord_limits/paths/emojiPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/guildPaths.py` & `discord_limits-2.0.3/discord_limits/paths/guildPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/interationsPaths.py` & `discord_limits-2.0.3/discord_limits/paths/interationsPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/invitePaths.py` & `discord_limits-2.0.3/discord_limits/paths/invitePaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/paths.py` & `discord_limits-2.0.3/discord_limits/paths/paths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/stagePaths.py` & `discord_limits-2.0.3/discord_limits/paths/stagePaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/stickerPaths.py` & `discord_limits-2.0.3/discord_limits/paths/stickerPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/userPaths.py` & `discord_limits-2.0.3/discord_limits/paths/userPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/paths/webhookPaths.py` & `discord_limits-2.0.3/discord_limits/paths/webhookPaths.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits/rate_limits.py` & `discord_limits-2.0.3/discord_limits/rate_limits.py`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/discord_limits.egg-info/PKG-INFO` & `discord_limits-2.0.3/discord_limits.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
-Name: discord-limits
-Version: 2.0.2
+Name: discord_limits
+Version: 2.0.3
 Summary: Make Discord API calls without having to worry about ratelimits.
 Home-page: https://github.com/ninjafella/discord-API-limits
 Author: ninjafella
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiolimiter==1.1.0
+Requires-Dist: aiohttp==3.9.5
 
 [![Documentation Status]](https://discord-limits.readthedocs.io/en/latest/?badge=latest)
-[![Version](https://img.shields.io/badge/Version-v2.0.2-blue)](https://img.shields.io/badge/Version-v2.0.2-blue)
+[![Version](https://img.shields.io/badge/Version-v2.0.3-blue)](https://img.shields.io/badge/Version-v2.0.3-blue)
 
 # discord_limits
 
 ### A simple library to asynchronously make API requests to Discord without having to worry about ratelimits.
 
 <br>
```

### Comparing `discord_limits-2.0.2/discord_limits.egg-info/SOURCES.txt` & `discord_limits-2.0.3/discord_limits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord_limits-2.0.2/setup.py` & `discord_limits-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name="discord_limits",
     packages=find_packages(
         include=["discord_limits", "discord_limits.paths", "discord_limits.objects"]
     ),
-    version="2.0.2",
+    version="2.0.3",
     description="Make Discord API calls without having to worry about ratelimits.",
     author="ninjafella",
     license="MIT",
     install_requires=["aiolimiter==1.1.0", "aiohttp==3.9.5"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ninjafella/discord-API-limits",
```


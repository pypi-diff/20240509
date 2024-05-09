# Comparing `tmp/icemedia-0.1.3.tar.gz` & `tmp/icemedia-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icemedia-0.1.3.tar", last modified: Sat May  4 21:38:19 2024, max compression
+gzip compressed data, was "icemedia-0.1.4.tar", last modified: Thu May  9 09:34:02 2024, max compression
```

## Comparing `icemedia-0.1.3.tar` & `icemedia-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-04 21:38:19.803892 icemedia-0.1.3/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    26526 2024-04-05 18:14:06.000000 icemedia-0.1.3/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8929 2024-05-04 21:38:19.803892 icemedia-0.1.3/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     8373 2024-05-04 21:37:29.000000 icemedia-0.1.3/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-04 21:38:19.803892 icemedia-0.1.3/icemedia/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-05 18:15:47.000000 icemedia-0.1.3/icemedia/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9616 2024-04-10 05:25:46.000000 icemedia-0.1.3/icemedia/iceflow.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    44440 2024-05-04 21:30:35.000000 icemedia-0.1.3/icemedia/iceflow_server.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     7016 2024-04-05 23:26:04.000000 icemedia-0.1.3/icemedia/jack_client_subprocess.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    36703 2024-04-10 05:33:55.000000 icemedia-0.1.3/icemedia/jack_tools.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    20538 2024-04-10 05:33:09.000000 icemedia-0.1.3/icemedia/jsonrpyc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-11 23:13:16.000000 icemedia-0.1.3/icemedia/py.typed
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    24337 2024-04-06 02:27:57.000000 icemedia-0.1.3/icemedia/python_mpv_jsonipc.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    22473 2024-04-14 01:55:10.000000 icemedia-0.1.3/icemedia/sound_player.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-04 21:38:19.803892 icemedia-0.1.3/icemedia.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8929 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      495 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       21 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2024-05-04 21:38:19.000000 icemedia-0.1.3/icemedia.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-05-04 21:38:19.803892 icemedia-0.1.3/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      892 2024-05-04 21:36:44.000000 icemedia-0.1.3/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-04 21:38:19.803892 icemedia-0.1.3/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-11-08 06:36:16.000000 icemedia-0.1.3/tests/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3037 2024-04-06 01:34:27.000000 icemedia-0.1.3/tests/testGstStability.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      938 2024-04-06 01:34:27.000000 icemedia-0.1.3/tests/testJack.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      231 2024-04-06 02:25:55.000000 icemedia-0.1.3/tests/test_sound_player.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-09 09:34:02.711137 icemedia-0.1.4/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    26526 2024-04-05 18:14:06.000000 icemedia-0.1.4/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8929 2024-05-09 09:34:02.710137 icemedia-0.1.4/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8373 2024-05-04 21:37:29.000000 icemedia-0.1.4/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-09 09:34:02.708137 icemedia-0.1.4/icemedia/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-05 18:15:47.000000 icemedia-0.1.4/icemedia/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10291 2024-05-09 09:21:45.000000 icemedia-0.1.4/icemedia/iceflow.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    44586 2024-05-09 08:57:02.000000 icemedia-0.1.4/icemedia/iceflow_server.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     7016 2024-04-05 23:26:04.000000 icemedia-0.1.4/icemedia/jack_client_subprocess.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    36703 2024-04-10 05:33:55.000000 icemedia-0.1.4/icemedia/jack_tools.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    20538 2024-04-10 05:33:09.000000 icemedia-0.1.4/icemedia/jsonrpyc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2024-04-11 23:13:16.000000 icemedia-0.1.4/icemedia/py.typed
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    24337 2024-04-06 02:27:57.000000 icemedia-0.1.4/icemedia/python_mpv_jsonipc.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    22473 2024-04-14 01:55:10.000000 icemedia-0.1.4/icemedia/sound_player.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-09 09:34:02.710137 icemedia-0.1.4/icemedia.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8929 2024-05-09 09:34:02.000000 icemedia-0.1.4/icemedia.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      495 2024-05-09 09:34:02.000000 icemedia-0.1.4/icemedia.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-05-09 09:34:02.000000 icemedia-0.1.4/icemedia.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       21 2024-05-09 09:34:02.000000 icemedia-0.1.4/icemedia.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2024-05-09 09:34:02.000000 icemedia-0.1.4/icemedia.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-05-09 09:34:02.711137 icemedia-0.1.4/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      892 2024-05-09 09:33:48.000000 icemedia-0.1.4/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-05-09 09:34:02.710137 icemedia-0.1.4/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-11-08 06:36:16.000000 icemedia-0.1.4/tests/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3037 2024-04-06 01:34:27.000000 icemedia-0.1.4/tests/testGstStability.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      938 2024-04-06 01:34:27.000000 icemedia-0.1.4/tests/testJack.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      231 2024-04-06 02:25:55.000000 icemedia-0.1.4/tests/test_sound_player.py
```

### Comparing `icemedia-0.1.3/LICENSE` & `icemedia-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.3/PKG-INFO` & `icemedia-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icemedia
-Version: 0.1.3
+Version: 0.1.4
 Summary: A GStreamer wrapper with JACK connection management
 Home-page: https://github.com/EternityForest/iceflow
 Author: Daniel Dunn
 Author-email: dannydunn@eternityforest.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `icemedia-0.1.3/README.md` & `icemedia-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.3/icemedia/iceflow.py` & `icemedia-0.1.4/icemedia/iceflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,21 +5,45 @@
 import time
 import sys
 import functools
 import base64
 import os
 import threading
 import weakref
+import logging
 from typing import Optional
 from subprocess import PIPE, STDOUT
 from subprocess import Popen
 from scullery import workers
 from .jsonrpyc import RPC
 
 
+# Truly an awefullehaccken
+# Break out of venv to get to gstreamer
+# It's just that one package.  Literally everything else
+# Is perfectly fine. GStreamer doesn't do pip so we do this.
+
+try:
+    if os.environ.get("VIRTUAL_ENV"):
+        en = os.environ["VIRTUAL_ENV"]
+        p = os.path.join(
+            en,
+            "lib",
+            "python" + ".".join(sys.version.split(".")[:2]),
+            "site-packages",
+            "gi",
+        )
+        s = "/usr/lib/python3/dist-packages/gi"
+
+        if os.path.exists(s) and (not os.path.exists(p)):
+            os.symlink(s, p)
+except Exception:
+    logging.exception("Failed to do the gstreamer hack")
+
+
 def close_fds(p: Popen):
     try:
         p.stdin.close()
     except Exception:
         pass
     try:
         p.stdout.close()
```

### Comparing `icemedia-0.1.3/icemedia/iceflow_server.py` & `icemedia-0.1.4/icemedia/iceflow_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,17 @@
                 unref = True
                 if not b:
                     raise RuntimeError("B has no pad named sink and A is a pad")
             if not a.link(b) == Gst.PadLinkReturn.OK:
                 raise RuntimeError("Could not link: " + str(a) + str(b))
 
         else:
+            if a.srcpads and b.sinkpads:
+                if a.srcpads[0].peer == b.sinkpads[0]:
+                    raise RuntimeError("Elements already linked.")
             x = a.link(b)
 
             if not x:
                 raise RuntimeError(
                     "Could not link" + str(a) + str(b) + " reason " + str(x)
                 )
     finally:
@@ -470,15 +473,15 @@
         self.realtime = realtime
         self._stopped = True
         self.sync_stop = False
         self.pipeline = Gst.Pipeline()
         self.thread_started = False
         self.weakrefs = weakref.WeakValueDictionary()
 
-        self.proxyToElement = weakref.WeakValueDictionary()
+        self.proxies_to_elements = {}
 
         # This WeakValueDictionary is mostly for testing purposes
         pipes[id(self)] = self
 
         # Thread puts something in this so we know we exited
         self.exitSignal = []
 
@@ -1221,15 +1224,15 @@
                 self.sidechainElements.append(e)
 
             self.namedElements[name] = e
 
             self.lastElementType = t
             p = weakref.proxy(e)
 
-            self.proxyToElement[id(p)] = e
+            self.proxies_to_elements[id(p)] = p
             # List it under the proxy as well
             self.elementTypesById[id(p)] = t
             elementsByShortId[id(p)] = e
 
         # Mark as a JACK user so we can stop if needed for JACK
         # Stuff
         if t.startswith("jackaudio"):
```

### Comparing `icemedia-0.1.3/icemedia/jack_client_subprocess.py` & `icemedia-0.1.4/icemedia/jack_client_subprocess.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.3/icemedia/jack_tools.py` & `icemedia-0.1.4/icemedia/jack_tools.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.3/icemedia/jsonrpyc.py` & `icemedia-0.1.4/icemedia/jsonrpyc.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.3/icemedia/python_mpv_jsonipc.py` & `icemedia-0.1.4/icemedia/python_mpv_jsonipc.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.3/icemedia/sound_player.py` & `icemedia-0.1.4/icemedia/sound_player.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.3/icemedia.egg-info/PKG-INFO` & `icemedia-0.1.4/icemedia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icemedia
-Version: 0.1.3
+Version: 0.1.4
 Summary: A GStreamer wrapper with JACK connection management
 Home-page: https://github.com/EternityForest/iceflow
 Author: Daniel Dunn
 Author-email: dannydunn@eternityforest.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `icemedia-0.1.3/setup.py` & `icemedia-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="icemedia",
-    version="0.1.3",
+    version="0.1.4",
     author="Daniel Dunn",
     author_email="dannydunn@eternityforest.com",
     description="A GStreamer wrapper with JACK connection management",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EternityForest/iceflow",
     packages=setuptools.find_packages(),
```

### Comparing `icemedia-0.1.3/tests/testGstStability.py` & `icemedia-0.1.4/tests/testGstStability.py`

 * *Files identical despite different names*

### Comparing `icemedia-0.1.3/tests/testJack.py` & `icemedia-0.1.4/tests/testJack.py`

 * *Files identical despite different names*


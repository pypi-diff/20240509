# Comparing `tmp/ansar_connect-0.1.235.tar.gz` & `tmp/ansar_connect-0.1.236.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.235.tar", last modified: Thu May  9 02:23:31 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.236.tar", last modified: Thu May  9 12:40:43 2024, max compression
```

## Comparing `ansar_connect-0.1.235.tar` & `ansar_connect-0.1.236.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.235/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.235/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-09 01:14:47.000000 ansar_connect-0.1.235/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-09 01:14:38.000000 ansar_connect-0.1.235/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.215453 ansar_connect-0.1.235/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.215453 ansar_connect-0.1.235/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.215453 ansar_connect-0.1.235/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.235/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.235/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.235/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.235/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-09 02:23:28.000000 ansar_connect-0.1.235/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.235/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.235/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.235/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.235/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.235/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.235/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.235/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.235/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.235/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34886 2024-05-07 19:48:13.000000 ansar_connect-0.1.235/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.235/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.235/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.235/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.235/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.235/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.235/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.235/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.235/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 12:40:43.220940 ansar_connect-0.1.236/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.236/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 12:40:43.220940 ansar_connect-0.1.236/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.236/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-09 12:39:56.000000 ansar_connect-0.1.236/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-09 12:40:43.220940 ansar_connect-0.1.236/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-09 12:39:45.000000 ansar_connect-0.1.236/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 12:40:43.220940 ansar_connect-0.1.236/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 12:40:43.220940 ansar_connect-0.1.236/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 12:40:43.220940 ansar_connect-0.1.236/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.236/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.236/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.236/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.236/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 12:40:43.220940 ansar_connect-0.1.236/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2999 2024-05-09 12:40:40.000000 ansar_connect-0.1.236/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.236/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.236/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.236/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.236/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.236/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12383 2024-05-09 06:40:17.000000 ansar_connect-0.1.236/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.236/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.236/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.236/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8453 2024-05-09 12:04:12.000000 ansar_connect-0.1.236/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.236/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.236/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.236/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.236/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.236/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.236/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.236/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.236/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 12:40:43.220940 ansar_connect-0.1.236/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 12:40:43.000000 ansar_connect-0.1.236/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-09 12:40:43.000000 ansar_connect-0.1.236/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-09 12:40:43.000000 ansar_connect-0.1.236/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-09 12:40:43.000000 ansar_connect-0.1.236/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-09 12:40:43.000000 ansar_connect-0.1.236/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-09 12:40:43.000000 ansar_connect-0.1.236/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.235/LICENSE` & `ansar_connect-0.1.236/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/PKG-INFO` & `ansar_connect-0.1.236/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.235
+Version: 0.1.236
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.82
+Requires-Dist: ansar-create>=0.1.83
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
 messaging into the asynchronous model of execution. The result of this approach is that sending
```

### Comparing `ansar_connect-0.1.235/README.md` & `ansar_connect-0.1.236/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/pyproject.toml` & `ansar_connect-0.1.236/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries"
 ]
 dynamic = ["description", "version", "scripts"]
 dependencies = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.82"
+    "ansar-create>=0.1.83"
 ]
 
 [project.urls]
 Documentation = "https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html"
```

### Comparing `ansar_connect-0.1.235/setup.py` & `ansar_connect-0.1.236/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 with open("DOC_LATEST_LINK", "r", encoding="utf-8") as f:
     d = f.read()
 DOC_LINK = d[:-1]
 
 REQUIRES = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.82",
+    "ansar-create>=0.1.83",
 ]
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="Scott Woods",
     author_email="scott.18.ansar@gmail.com.com",
```

### Comparing `ansar_connect-0.1.235/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.236/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.236/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.236/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.236/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/__init__.py` & `ansar_connect-0.1.236/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: d0946f454fbf36f7253dd247af0632ebdb9be90b
-Version: 0.1.234 (2024-05-09@14:23:28+NZST)
+Commit: 4e2adc74f04ec76aa1fcb1a0d458a01a939d4acc
+Version: 0.1.235 (2024-05-10@00:40:40+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
 
@@ -56,15 +56,15 @@
 from .directory import publish, subscribe
 from .directory import clear, retract
 from .directory import key_service
 
 from .networking_if import UseAddress, NoAddress, GlareTimer
 from .networking import ConnectToAddress, ListenAtAddress
 from .networking import SubscribeToListing, PublishAListing, SubscribeToSearch
-from .grouping import GroupTable, GroupUpdate, AddressGroup, GroupTimer, GroupObject
+from .grouping import GroupTable, GroupUpdate, AddressGroup, GroupTimer
 
 from .node import NodeSettings, node_settings
 from .node import node_passing, sub_node_passing
 from .node import create_node, NodeProperties
 
 from .moving import overlay, mirror
```

### Comparing `ansar_connect-0.1.235/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.236/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/directory.py` & `ansar_connect-0.1.236/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.236/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.236/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/group_if.py` & `ansar_connect-0.1.236/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/grouping.py` & `ansar_connect-0.1.236/src/ansar/connect/grouping.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from .plumbing import *
 from .networking_if import *
 
 __all__ = [
 	'GroupTable',
 	'GroupUpdate',
 	'AddressGroup',
-	'GroupObject',
 ]
 
 # The specification.
 class GroupTable(object):
 	def __init__(self, **member_frame):
 		if 'member_frame' in member_frame or 'create' in member_frame or 'update' in member_frame:
 			raise ValueError('names of members would hide GroupTable methods')
@@ -421,61 +420,7 @@
 	),
 	CLEARING: (
 		(ar.Completed,), ()
 	),
 }
 
 ar.bind(AddressGroup, ADDRESS_GROUP_DISPATCH)
-
-# A shim object between create_object() and the application object.
-# This is the most concise way to run an object with the support
-# of one or more runtime objects, e.g. a connection to a service.
-class GroupObject(ar.Point, ar.StateMachine):
-	def __init__(self, *args_plus_2, get_ready=None, resident_code=False, until_stopped=False):
-		ar.Point.__init__(self)
-		ar.StateMachine.__init__(self, INITIAL)
-		# Need to trampoline a variable list of settings, input and variables
-		# onto the receiving function, i.e. group_args.
-		self.args = args_plus_2[:-2]
-		self.session = args_plus_2[-2]
-		self.group_args = args_plus_2[-1]
-		self.get_ready = get_ready
-		self.resident_code = resident_code
-		self.until_stopped = until_stopped
-
-		self.group = None
-		self.created = None
-		self.closing = None
-
-def GroupObject_INITIAL_Start(self, message):
-	# Convert settings, input and variables into args and
-	# kw suitable for the session object. This is all about
-	# converting the "command-line" info its most useful
-	# form.
-	self.group, args, kv = self.group_args(*self.args)
-
-	# Create a session factory.
-	session = CreateFrame(self.session, *args, **kv)
-
-	# Real work done by AddressGroup.
-	# Create the group passing the factory for those moments
-	# when the group goes ready.
-	self.created = self.group.create(self, session=session, resident_code=self.resident_code, get_ready=self.get_ready, until_stopped=self.until_stopped)
-	return RUNNING
-
-def GroupObject_RUNNING_Completed(self, message):
-	self.complete(message.value)
-
-def GroupObject_RUNNING_Stop(self, message):
-	self.send(message, self.created)
-	return RUNNING
-
-GROUP_SESSION_DISPATCH = {
-	INITIAL: (
-		(ar.Start,), ()
-	),
-	RUNNING: (
-		(ar.Completed, ar.Stop), ()
-	),
-}
-
-ar.bind(GroupObject, GROUP_SESSION_DISPATCH)
```

### Comparing `ansar_connect-0.1.235/src/ansar/connect/moving.py` & `ansar_connect-0.1.236/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/networking.py` & `ansar_connect-0.1.236/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.236/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.236/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/procedure.py` & `ansar_connect-0.1.236/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/product.py` & `ansar_connect-0.1.236/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/socketry.py` & `ansar_connect-0.1.236/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/standard.py` & `ansar_connect-0.1.236/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/transporting.py` & `ansar_connect-0.1.236/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.236/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar/connect/wan.py` & `ansar_connect-0.1.236/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.235/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.236/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.235
+Version: 0.1.236
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi>=1.16.0
 Requires-Dist: PyNaCl>=1.5.0
-Requires-Dist: ansar-create>=0.1.82
+Requires-Dist: ansar-create>=0.1.83
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
 messaging into the asynchronous model of execution. The result of this approach is that sending
```

### Comparing `ansar_connect-0.1.235/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.236/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*


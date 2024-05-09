# Comparing `tmp/ansar_connect-0.1.223.tar.gz` & `tmp/ansar_connect-0.1.232.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.223.tar", last modified: Wed May  8 01:37:47 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.232.tar", last modified: Wed May  8 22:13:05 2024, max compression
```

## Comparing `ansar_connect-0.1.223.tar` & `ansar_connect-0.1.232.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:37:47.146972 ansar_connect-0.1.223/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.223/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-08 01:37:47.146972 ansar_connect-0.1.223/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.223/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-08 01:35:22.000000 ansar_connect-0.1.223/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-08 01:37:47.146972 ansar_connect-0.1.223/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-08 01:35:12.000000 ansar_connect-0.1.223/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:37:47.142972 ansar_connect-0.1.223/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:37:47.142972 ansar_connect-0.1.223/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:37:47.142972 ansar_connect-0.1.223/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.223/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3206 2024-04-18 00:04:05.000000 ansar_connect-0.1.223/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.223/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8819 2024-04-18 00:04:05.000000 ansar_connect-0.1.223/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:37:47.142972 ansar_connect-0.1.223/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-08 01:37:43.000000 ansar_connect-0.1.223/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.223/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87388 2024-05-07 01:18:28.000000 ansar_connect-0.1.223/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.223/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.223/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.223/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.223/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.223/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.223/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.223/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34886 2024-05-07 19:48:13.000000 ansar_connect-0.1.223/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.223/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.223/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.223/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    39924 2024-05-07 04:34:09.000000 ansar_connect-0.1.223/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.223/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.223/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.223/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.223/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 01:37:47.142972 ansar_connect-0.1.223/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-08 01:37:47.000000 ansar_connect-0.1.223/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-08 01:37:47.000000 ansar_connect-0.1.223/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-08 01:37:47.000000 ansar_connect-0.1.223/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-08 01:37:47.000000 ansar_connect-0.1.223/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-08 01:37:47.000000 ansar_connect-0.1.223/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-08 01:37:47.000000 ansar_connect-0.1.223/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 22:13:05.276826 ansar_connect-0.1.232/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.232/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-08 22:13:05.276826 ansar_connect-0.1.232/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.232/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-08 19:43:40.000000 ansar_connect-0.1.232/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-08 22:13:05.276826 ansar_connect-0.1.232/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-08 19:43:31.000000 ansar_connect-0.1.232/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 22:13:05.272827 ansar_connect-0.1.232/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 22:13:05.272827 ansar_connect-0.1.232/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 22:13:05.272827 ansar_connect-0.1.232/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.232/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.232/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.232/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.232/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 22:13:05.276826 ansar_connect-0.1.232/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-08 22:13:02.000000 ansar_connect-0.1.232/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.232/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87388 2024-05-07 01:18:28.000000 ansar_connect-0.1.232/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.232/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.232/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.232/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.232/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.232/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.232/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.232/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34886 2024-05-07 19:48:13.000000 ansar_connect-0.1.232/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.232/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.232/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.232/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38933 2024-05-08 22:09:06.000000 ansar_connect-0.1.232/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.232/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.232/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.232/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.232/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-08 22:13:05.276826 ansar_connect-0.1.232/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-08 22:13:05.000000 ansar_connect-0.1.232/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-08 22:13:05.000000 ansar_connect-0.1.232/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-08 22:13:05.000000 ansar_connect-0.1.232/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-08 22:13:05.000000 ansar_connect-0.1.232/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-08 22:13:05.000000 ansar_connect-0.1.232/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-08 22:13:05.000000 ansar_connect-0.1.232/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.223/LICENSE` & `ansar_connect-0.1.232/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/PKG-INFO` & `ansar_connect-0.1.232/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.223
+Version: 0.1.232
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
-Requires-Dist: ansar-create>=0.1.77
+Requires-Dist: ansar-create>=0.1.81
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
 messaging into the asynchronous model of execution. The result of this approach is that sending
```

### Comparing `ansar_connect-0.1.223/README.md` & `ansar_connect-0.1.232/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/pyproject.toml` & `ansar_connect-0.1.232/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -20,12 +20,12 @@
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries"
 ]
 dynamic = ["description", "version", "scripts"]
 dependencies = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.77"
+    "ansar-create>=0.1.81"
 ]
 
 [project.urls]
 Documentation = "https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html"
```

### Comparing `ansar_connect-0.1.223/setup.py` & `ansar_connect-0.1.232/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 with open("DOC_LATEST_LINK", "r", encoding="utf-8") as f:
     d = f.read()
 DOC_LINK = d[:-1]
 
 REQUIRES = [
     "cffi>=1.16.0",
     "PyNaCl>=1.5.0",
-    "ansar-create>=0.1.77",
+    "ansar-create>=0.1.81",
 ]
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="Scott Woods",
     author_email="scott.18.ansar@gmail.com.com",
```

### Comparing `ansar_connect-0.1.223/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.232/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.232/src/ansar/command/ansar_directory.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 '''.
 
 .
 '''
 import ansar.connect as ar
+from ansar.connect.standard import *
 from ansar.create.object import decoration_store
 
 __all__ = [
 	'main',
 ]
 
 #
@@ -89,15 +90,16 @@
 
 ar.bind(directory)
 
 #
 #
 factory_settings = Settings(
 	directory_scope=ar.ScopeOfService.HOST,
-	connect_above=ar.HostPort('192.168.1.176', 32176)
+	accept_below=ANSAR_LOCAL_DEDICATED,
+	connect_above=ar.HostPort(),
 )
 
 #
 #
 def main():
     ar.create_object(directory, factory_settings=factory_settings)
```

### Comparing `ansar_connect-0.1.223/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.232/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.232/src/ansar/command/shared_directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 Rather than a unique network address (IP + port) per directory, this
 process uses a single address while managing multiple directories. Multiple
 deployments of different products or different instances of the same
 product can be supported.
 '''
 import ansar.connect as ar
+from ansar.connect.standard import *
 from ansar.connect.wan import *
 from ansar.connect.product import *
 from ansar.connect.directory import find_overlap
 
 __all__ = [
 	'main',
 ]
@@ -288,15 +289,15 @@
 }
 
 ar.bind(Settings, object_schema=SETTINGS_SCHEMA)
 
 #
 #
 factory_settings = Settings(directory_scope=ar.ScopeOfService.HOST,
-	public_access=ar.LocalPort(32177))
+	public_access=ANSAR_LOCAL_SHARED)
 
 #
 #
 def main():
     ar.create_object(ProductDirectory, factory_settings=factory_settings)
 
 # The standard entry point. Needed for IDEs
```

### Comparing `ansar_connect-0.1.223/src/ansar/connect/__init__.py` & `ansar_connect-0.1.232/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 711219c3ee00d26e0301c1aa33414ab8e374fd74
-Version: 0.1.222 (2024-05-08@13:37:43+NZST)
+Commit: eed9d7c5947895460669afcc45d5ed7ecaa34058
+Version: 0.1.231 (2024-05-09@10:13:02+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.223/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.232/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/directory.py` & `ansar_connect-0.1.232/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.232/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.232/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/group_if.py` & `ansar_connect-0.1.232/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/grouping.py` & `ansar_connect-0.1.232/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/moving.py` & `ansar_connect-0.1.232/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/networking.py` & `ansar_connect-0.1.232/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.232/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/node.py` & `ansar_connect-0.1.232/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.232/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/procedure.py` & `ansar_connect-0.1.232/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/product.py` & `ansar_connect-0.1.232/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/socketry.py` & `ansar_connect-0.1.232/src/ansar/connect/socketry.py`

 * *Files 5% similar despite different names*

```diff
@@ -341,94 +341,85 @@
 }
 
 ar.bind(Relay, object_schema=RELAY_SCHEMA)
 
 class StreamingIn(object):
 	def __init__(self):
 		self.analysis_state = 1
-		self.size_digits = bytearray()
-		self.jump_size = 0
-		self.byte_header = bytearray()
-		self.byte_body = bytearray()
-		self.byte_space = bytearray()
-		self.byte_part = self.byte_header
+		self.size_byte = bytearray()
+		self.size_len = []
+		self.frame_size = 0
+		self.frame_byte = bytearray()
 
 		def s1(c):
-			if c in b'0123456789':
-				nd = len(self.size_digits)
+			if c in b'0123456789,':
+				nd = len(self.size_byte)
 				if nd < NUMBER_OF_DIGITS:
-					self.size_digits += c
+					self.size_byte.append(c)
 					return 1
 				raise OverflowError(f'unlikely frame size with {nd} digits')
 			elif c == b'\n':
-				d = self.size_digits.decode('utf-8')
-				self.jump_size = int(d)
+				a = self.size_byte.split(b',')
+				if len(a) != 3:
+					raise ValueError(f'unexpected dimension')
+				for b in a:
+					if not b or not b.isdigit():
+						raise ValueError(f'mangled frame dimensions')
+				self.size_len = [int(b) for b in a]
+				self.jump_size = self.size_len[-1]
 				if self.jump_size > GIANT_FRAME:
 					raise OverflowError(f'oversize frame of {self.jump_size} bytes')
 				elif self.jump_size == 0:
 					return 3
 				return 2
-			d = c.decode('utf8')
-			raise ValueError(f'frame with unexpected byte {d} in digits')
+			raise ValueError(f'frame with unexpected {c} in digits')
 
 		def s2(c):
-			self.byte_part += c
+			self.frame_byte.append(c)
 			self.jump_size -= 1
 			if self.jump_size == 0:
 				return 3
 			return 2
 
 		def s3(c):
 			if c == b'\n':
 				return 0
-			d = c.decode('utf8')
-			raise ValueError(f'unexpected byte {d} at end-of-frame')
+			raise ValueError(f'unexpected {c} at end-of-frame')
 
 		self.shift = {
 			1: s1,
 			2: s2,
 			3: s3,
 		}
 
 	def header_body(self, received):
-		r = len(received)
-		for i in range(r):
-			c = received[i:i+1]
+		for c in received:
 			next = self.shift[self.analysis_state](c)
 			if next:
 				self.analysis_state = next
 				continue
-			if self.byte_part is self.byte_header:
-				self.analysis_state = 1
-				self.size_digits.clear()
-				self.jump_size = 0
-				self.byte_part = self.byte_body
-				continue
-			if self.byte_part is self.byte_body:
-				self.analysis_state = 1
-				self.size_digits.clear()
-				self.jump_size = 0
-				self.byte_part = self.byte_space
-				continue
+
+			# Completed frame.
+			f = bytes(self.frame_byte)
 			if self.key_box:
-				h = self.key_box.decrypt(bytes(self.byte_header))
-				b_ = self.key_box.decrypt(bytes(self.byte_body))
-				s = self.key_box.decrypt(bytes(self.byte_space))
-				yield bytearray(h), bytearray(b_), bytearray(s)
-			else:
-				yield self.byte_header, self.byte_body, self.byte_space
+				f = self.key_box.decrypt(f)
+
+			# Breakout.
+			n0 = self.size_len[0]
+			n1 = self.size_len[1]
+			b2 = n0 + n1
+			yield f[0:n0], f[n0:b2], f[b2:]
+
+			# Restart.
 			self.analysis_state = 1
-			self.size_digits.clear()
-			self.jump_size = 0
-			# Ownership passed with yield. Make new
-			# ones.
-			self.byte_header = bytearray()
-			self.byte_body = bytearray()
-			self.byte_space = bytearray()
-			self.byte_part = self.byte_header
+			self.size_byte = bytearray()
+			self.size_len = []
+			self.frame_size = 0
+			self.frame_byte = bytearray()
+
 
 class StreamingOut(object):
 	def __init__(self):
 		self.pending = []		   # Messages not yet in the loop.
 		self.lock = thr.RLock()	 # Safe sharing and empty detection.
 		self.messages_to_encode = ar.deque()
 
@@ -454,84 +445,73 @@
 
 	def best_block(self, encoded_bytes, codec):
 		while len(encoded_bytes) < TCP_SEND:
 			if len(self.messages_to_encode) == 0:
 				added = self.drain(self.messages_to_encode)
 				if added == 0:
 					break
+			# The message and to-return addresses.
 			m, t, r = self.messages_to_encode.popleft()
 			f = False
 			key_box = self.key_box
-			if isinstance(m, Diffie):
+
+			# Types significant to streaming.
+			# Be nice to move DH detection elsewhere.
+			if isinstance(m, Blob):
+				f = True
+			elif isinstance(m, Diffie):
 				self.private_key = PrivateKey.generate()
 				public_bytes = self.private_key.public_key.encode()
 				m.public_key = bytearray(public_bytes)
 			elif isinstance(m, Hellman):
 				self.private_key = PrivateKey.generate()
 				shared_bytes = bytes(m.public_key)
 				shared_key = PublicKey(shared_bytes)
 				self.key_box = Box(self.private_key, shared_key)
 				public_bytes = self.private_key.public_key.encode()
 				m.public_key = bytearray(public_bytes)
-			elif isinstance(m, Blob):
-				f = True
+
+			# Bring the parts together.
+			# 1. Header
 			h = Header(t, r, f)
 			e = codec.encode(h, HEADING)
-			e = e.encode('utf-8')
-			if key_box:
-				e = key_box.encrypt(e)
-			n = len(e)
-			# Stream the header
-			encoded_bytes += str(n).encode('ascii')
-			encoded_bytes += b'\n'
-			encoded_bytes += e
-			encoded_bytes += b'\n'
-			# Then a tunnelled bock, relay or normal message.
+			b0 = e.encode('utf-8')
+			n0 = len(b0)
+
+			# 2. Message body.
 			if f:
-				e = m.block
-				if key_box:
-					e = key_box.encrypt(e)
-				n = len(e)
-				encoded_bytes += str(n).encode('ascii')
-				encoded_bytes += b'\n'
-				encoded_bytes += e
-				encoded_bytes += b'\n'
-				# Tunnel block contains no addresses
-				# Could just assign '[]' (an empty JSON list)
+				b1 = m.block
+				n1 = len(b1)
 				s = codec.encode([], SPACE)
 			elif isinstance(m, Relay):
-				e = m.block
-				if key_box:
-					e = key_box.encrypt(e)
-				n = len(e)
-				encoded_bytes += str(n).encode('ascii')
-				encoded_bytes += b'\n'
-				encoded_bytes += e
-				encoded_bytes += b'\n'
+				b1 = m.block
+				n1 = len(b1)
 				s = codec.encode(m.space, SPACE)
 			else:
 				space = []
 				e = codec.encode(m, ar.Any(), space=space)
-				e = e.encode('utf-8')
-				if key_box:
-					e = key_box.encrypt(e)
-				n = len(e)
-				encoded_bytes += str(n).encode('ascii')
-				encoded_bytes += b'\n'
-				encoded_bytes += e
-				encoded_bytes += b'\n'
+				b1 = e.encode('utf-8')
+				n1 = len(b1)
 				s = codec.encode(space, SPACE)
-			# And lastly, the mutated section.
-			e = s.encode('utf-8')
+
+			# 3. Mutated addresses.
+			b2 = s.encode('utf-8')
+
+			# Combine into 1 and optionally encrypt.
+			b0 += b1
+			b0 += b2
 			if key_box:
-				e = key_box.encrypt(e)
-			n = len(e)
-			encoded_bytes += str(n).encode('ascii')
+				b0 = key_box.encrypt(b0)
+			n3 = len(b0)
+
+			# Put frame on the stream.
+			n = f'{n0},{n1},{n3}'
+			encoded_bytes += n.encode('ascii')
 			encoded_bytes += b'\n'
-			encoded_bytes += e
+			encoded_bytes += b0
 			encoded_bytes += b'\n'
 		return len(encoded_bytes)
 
 class TcpStream(StreamingIn, StreamingOut):
 	def __init__(self, parent, controller_address, upgrade, opened):
 		StreamingIn.__init__(self)
 		StreamingOut.__init__(self)
```

### Comparing `ansar_connect-0.1.223/src/ansar/connect/standard.py` & `ansar_connect-0.1.232/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/transporting.py` & `ansar_connect-0.1.232/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.232/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar/connect/wan.py` & `ansar_connect-0.1.232/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.223/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.232/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.223
+Version: 0.1.232
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
-Requires-Dist: ansar-create>=0.1.77
+Requires-Dist: ansar-create>=0.1.81
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
 messaging into the asynchronous model of execution. The result of this approach is that sending
```

### Comparing `ansar_connect-0.1.223/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.232/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*


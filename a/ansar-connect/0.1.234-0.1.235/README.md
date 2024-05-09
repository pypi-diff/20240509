# Comparing `tmp/ansar_connect-0.1.234.tar.gz` & `tmp/ansar_connect-0.1.235.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.234.tar", last modified: Thu May  9 01:15:02 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.235.tar", last modified: Thu May  9 02:23:31 2024, max compression
```

## Comparing `ansar_connect-0.1.234.tar` & `ansar_connect-0.1.235.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 01:15:02.693429 ansar_connect-0.1.234/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.234/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 01:15:02.693429 ansar_connect-0.1.234/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.234/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-09 01:14:47.000000 ansar_connect-0.1.234/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-09 01:15:02.693429 ansar_connect-0.1.234/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-09 01:14:38.000000 ansar_connect-0.1.234/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 01:15:02.689429 ansar_connect-0.1.234/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 01:15:02.689429 ansar_connect-0.1.234/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 01:15:02.689429 ansar_connect-0.1.234/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.234/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.234/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.234/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.234/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 01:15:02.693429 ansar_connect-0.1.234/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-09 01:14:59.000000 ansar_connect-0.1.234/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.234/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    87388 2024-05-07 01:18:28.000000 ansar_connect-0.1.234/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.234/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.234/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.234/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.234/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.234/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.234/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.234/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34886 2024-05-07 19:48:13.000000 ansar_connect-0.1.234/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.234/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.234/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.234/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.234/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.234/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.234/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.234/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.234/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 01:15:02.693429 ansar_connect-0.1.234/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 01:15:02.000000 ansar_connect-0.1.234/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-09 01:15:02.000000 ansar_connect-0.1.234/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-09 01:15:02.000000 ansar_connect-0.1.234/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-09 01:15:02.000000 ansar_connect-0.1.234/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-09 01:15:02.000000 ansar_connect-0.1.234/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-09 01:15:02.000000 ansar_connect-0.1.234/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.235/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.235/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-09 01:14:47.000000 ansar_connect-0.1.235/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-09 01:14:38.000000 ansar_connect-0.1.235/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.215453 ansar_connect-0.1.235/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.215453 ansar_connect-0.1.235/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.215453 ansar_connect-0.1.235/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.235/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3259 2024-05-08 21:30:23.000000 ansar_connect-0.1.235/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.235/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8855 2024-05-08 21:32:04.000000 ansar_connect-0.1.235/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-09 02:23:28.000000 ansar_connect-0.1.235/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.235/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    87458 2024-05-09 02:23:09.000000 ansar_connect-0.1.235/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     8445 2024-05-07 03:55:37.000000 ansar_connect-0.1.235/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.235/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.235/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.235/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.235/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21090 2024-05-07 01:18:28.000000 ansar_connect-0.1.235/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.235/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34886 2024-05-07 19:48:13.000000 ansar_connect-0.1.235/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.235/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    32864 2024-04-19 03:56:52.000000 ansar_connect-0.1.235/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.235/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    38992 2024-05-09 00:38:31.000000 ansar_connect-0.1.235/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.235/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2063 2024-05-07 01:18:28.000000 ansar_connect-0.1.235/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.235/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.235/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-09 02:23:31.219453 ansar_connect-0.1.235/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-09 02:23:31.000000 ansar_connect-0.1.235/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.234/LICENSE` & `ansar_connect-0.1.235/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/PKG-INFO` & `ansar_connect-0.1.235/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.234
+Version: 0.1.235
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.234/README.md` & `ansar_connect-0.1.235/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/pyproject.toml` & `ansar_connect-0.1.235/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/setup.py` & `ansar_connect-0.1.235/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.235/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.235/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.235/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.235/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/__init__.py` & `ansar_connect-0.1.235/src/ansar/connect/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: c0759d1887fea27be6b254d97cf360b5dd51304b
-Version: 0.1.233 (2024-05-09@13:14:59+NZST)
+Commit: d0946f454fbf36f7253dd247af0632ebdb9be90b
+Version: 0.1.234 (2024-05-09@14:23:28+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.234/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.235/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/directory.py` & `ansar_connect-0.1.235/src/ansar/connect/directory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1207,15 +1207,15 @@
 
 # Methods of termination;
 ### PS-pub-8 Loop terminates by session completion.
 def PublisherLoop_LOOPED_Completed(self, message):
 	if self.created_session and self.return_address == self.created_session:
 		cleared = Cleared(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, value=message.value)
+			route_key=self.route.route_key, value=message.value)
 		self.forward(cleared, self.publisher_address, self.origin_address)
 		self.send(CloseLoop(self.route_key), self.remote_loop)
 		self.close_route()
 		self.complete(ar.Aborted())
 	self.warning('Unexpected termination')
 	return LOOPED
 
@@ -1226,28 +1226,28 @@
 	if self.created_session:
 		self.send(ar.Stop(), self.created_session)
 		return CLEARING
 	self.close_route()
 
 	cleared = Cleared(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, value=message.value)
+		route_key=self.route.route_key, value=message.value)
 	self.forward(cleared, self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
 
 ### PS-pub-8 Loop terminates by remote close.
 def PublisherLoop_LOOPED_CloseLoop(self, message):
 	if self.created_session:
 		self.send(ar.Stop(), self.created_session)
 		return CLEARING
 	self.close_route()
 
 	dropped = Dropped(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason='abandoned by remote')
+		route_key=self.route.route_key, reason='abandoned by remote')
 	self.forward(dropped, self.publisher_address, self.origin_address)
 	self.complete(ar.Aborted())
 
 ### PS-pub-8 Loop terminates by local exit.
 def PublisherLoop_LOOPED_Stop(self, message):
 	self.send(CloseLoop(self.route_key), self.remote_loop)
 	if self.created_session:
@@ -1267,20 +1267,20 @@
 
 	self.create_session = None
 	self.close_route()
 
 	if self.closing:
 		cleared = Cleared(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, value=self.value)
+			route_key=self.route.route_key, value=self.value)
 		self.forward(cleared, self.publisher_address, self.origin_address)
 	else:
 		dropped = Dropped(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, reason='aborted')
+			route_key=self.route.route_key, reason='aborted')
 		self.forward(dropped, self.publisher_address, self.origin_address)
 
 	self.complete(ar.Aborted())
 
 PUBLISHER_LOOP_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
@@ -1719,15 +1719,15 @@
 		# about "origin_address".
 		s = address_to_text(self.subscriber_address)
 		p = address_to_text(self.origin_address)
 		self.trace(f'Loop opened between subscriber [{s}] and publisher [{p}]')
 		opened_at = ar.world_now()
 		available = Available(matched_search=self.route.matched_search, matched_name=self.route.matched_name,
 			matched_scope=self.route.matched_scope, opened_at=opened_at,
-			route_key=message.route_key, agent_address=self.parent_address)
+			route_key=self.route.route_key, agent_address=self.parent_address)
 		self.forward(available, self.subscriber_address, self.origin_address)
 		self.send(hand, self.latch)
 		# LATCH MUST CONTINUE FOR THOSE MESSAGES THAT WERE
 		# SITTING IN THE QUEUE AFTER THE HANDOVER MESSAGE
 	
 	def latch_loop(self):
 		j = self.address_job.pop(self.latch, None)
@@ -1796,54 +1796,54 @@
 # Stop -> application
 def SubscriberLoop_LOOPED_Completed(self, message):
 	d = self.debrief()
 	# 0) Latch, 1) Session, *) Unknown
 	if d == 1:
 		cleared = Cleared(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, value=message.value)
+			route_key=self.route.route_key, value=message.value)
 		self.forward(cleared, self.subscriber_address, self.origin_address)
 	else:
 		f = ar.Faulted('Loop management', f'unexpected completion {d}')
 		self.warning(str(f))
 		cleared = Cleared(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, value=f)
+			route_key=self.route.route_key, value=f)
 		cleared = Cleared(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, value=f)
+			route_key=self.route.route_key, value=f)
 		self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 # Local termination.
 def SubscriberLoop_LOOPED_Close(self, message):
 	cleared = Cleared(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, value=message.value)
+		route_key=self.route.route_key, value=message.value)
 	self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 # Remote termination.
 def SubscriberLoop_LOOPED_CloseLoop(self, message):
 	dropped = Dropped(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason='abandoned by remote')
+		route_key=self.route.route_key, reason='abandoned by remote')
 	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
@@ -1869,15 +1869,15 @@
 	return CONNECTION_LOOPING
 
 def SubscriberLoop_CONNECTION_PEERING_NotPeered(self, message):
 	name = key_service(message.route_key)
 	self.trace(f'Cannot loop to {name} ({message.reason})')
 	na = NotAvailable(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason=message.reason,
+		route_key=self.route.route_key, reason=message.reason,
 		agent_address=self.parent_address)
 	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -1888,15 +1888,15 @@
 def SubscriberLoop_CONNECTION_PEERING_T2(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot loop to {name} ({reason})')
 	na = NotAvailable(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason=message.reason,
+		route_key=self.route.route_key, reason=message.reason,
 		agent_address=self.parent_address)
 	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -1920,15 +1920,15 @@
 def SubscriberLoop_CONNECTION_LOOPING_T1(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'timed out on loop'
 	self.trace(f'Cannot loop to {name} ({reason})')
 	na = NotAvailable(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason=message.reason,
+		route_key=self.route.route_key, reason=reason,
 		agent_address=self.parent_address)
 	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_loop()
 	self.close_peer()
 
 	if self.working():
@@ -1953,65 +1953,65 @@
 
 def SubscriberLoop_CONNECTION_LOOPED_Completed(self, message):
 	d = self.debrief()
 	# 0) Latch, 1) Session, *) Unknown
 	if d == 1:
 		cleared = Cleared(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, value=ar.Aborted())
+			route_key=self.route.route_key, value=ar.Aborted())
 		self.forward(cleared, self.subscriber_address, self.origin_address)
 	else:
 		f = ar.Faulted('Loop management', f'unexpected completion {d}')
 		self.warning(str(f))
 		cleared = Cleared(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, value=f)
+			route_key=self.route.route_key, value=f)
 		self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_peer()
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 def SubscriberLoop_CONNECTION_LOOPED_Close(self, message):
 	cleared = Cleared(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, value=message.value)
+		route_key=self.route.route_key, value=message.value)
 	self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = True
 		return CLEARING
 	self.complete(True)
 
 def SubscriberLoop_CONNECTION_LOOPED_CloseLoop(self, message):
 	dropped = Dropped(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason='abandoned by remote')
+		route_key=self.route.route_key, reason='abandoned by remote')
 	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
 
 def SubscriberLoop_CONNECTION_LOOPED_PeerLost(self, message):
 	dropped = Dropped(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason='abandoned by remote')
+		route_key=self.route.route_key, reason='abandoned by remote')
 	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
@@ -2058,15 +2058,15 @@
 def SubscriberLoop_RELAY_PEERING_T2(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'timed out on peer'
 	self.trace(f'Cannot relay to {name} ({reason})')
 	na = NotAvailable(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason=message.reason,
+		route_key=self.route.route_key, reason=message.reason,
 		agent_address=self.parent_address)
 	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -2090,15 +2090,15 @@
 def SubscriberLoop_RELAY_LOOPING_T1(self, message):
 	route_key = self.route.route_key
 	name = key_service(route_key)
 	reason = 'loop time exceeded'
 	self.trace(f'Cannot relay to {name} ({reason})')
 	na = NotAvailable(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason=message.reason,
+		route_key=self.route.route_key, reason=message.reason,
 		agent_address=self.parent_address)
 	self.forward(na, self.subscriber_address, self.address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
@@ -2125,22 +2125,22 @@
 
 def SubscriberLoop_RELAY_LOOPED_Completed(self, message):
 	d = self.debrief()
 	# 0) Latch, 1) Session, *) Unknown
 	if d == 1:
 		cleared = Cleared(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, value=message.value)
+			route_key=self.route.route_key, value=message.value)
 		self.forward(cleared, self.subscriber_address, self.origin_address)
 	else:
 		f = ar.Faulted('Loop management', f'unexpected completion {d}')
 		self.warning(str(f))
 		cleared = Cleared(matched_search=self.route.matched_search,
 			matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-			route_key=message.route_key, value=f)
+			route_key=self.route.route_key, value=f)
 		self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
@@ -2149,15 +2149,15 @@
 		return CLEARING
 	self.complete(True)
 
 # Local termination.
 def SubscriberLoop_RELAY_LOOPED_Close(self, message):
 	cleared = Cleared(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, value=message.value)
+		route_key=self.route.route_key, value=message.value)
 	self.forward(cleared, self.subscriber_address, self.origin_address)
 
 	self.close_loop()
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
@@ -2166,15 +2166,15 @@
 		return CLEARING
 	self.complete(True)
 
 # Remote termination.
 def SubscriberLoop_RELAY_LOOPED_CloseLoop(self, message):
 	dropped = Dropped(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason='abandoned by remote')
+		route_key=self.route.route_key, reason='abandoned by remote')
 	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	self.close_relay()
 	self.close_peer()
 
 	if self.working():
 		self.abort()
@@ -2182,15 +2182,15 @@
 		return CLEARING
 	self.complete(False)
 
 # Termination by loss of peer.
 def SubscriberLoop_RELAY_LOOPED_PeerLost(self, message):
 	dropped = Dropped(matched_search=self.route.matched_search,
 		matched_name=self.route.matched_name, matched_scope=self.route.matched_scope,
-		route_key=message.route_key, reason='abandoned by peer')
+		route_key=self.route.route_key, reason='abandoned by peer')
 	self.forward(dropped, self.subscriber_address, self.origin_address)
 
 	if self.working():
 		self.abort()
 		self.clearing_value = False
 		return CLEARING
 	self.complete(False)
```

### Comparing `ansar_connect-0.1.234/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.235/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.235/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/group_if.py` & `ansar_connect-0.1.235/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/grouping.py` & `ansar_connect-0.1.235/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/moving.py` & `ansar_connect-0.1.235/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/networking.py` & `ansar_connect-0.1.235/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.235/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/node.py` & `ansar_connect-0.1.235/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.235/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/procedure.py` & `ansar_connect-0.1.235/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/product.py` & `ansar_connect-0.1.235/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/socketry.py` & `ansar_connect-0.1.235/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/standard.py` & `ansar_connect-0.1.235/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/transporting.py` & `ansar_connect-0.1.235/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.235/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar/connect/wan.py` & `ansar_connect-0.1.235/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.234/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.235/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.234
+Version: 0.1.235
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.234/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.235/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*


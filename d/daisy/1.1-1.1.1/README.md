# Comparing `tmp/daisy-1.1.tar.gz` & `tmp/daisy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daisy-1.1.tar", last modified: Mon Mar 18 22:30:40 2024, max compression
+gzip compressed data, was "daisy-1.1.1.tar", last modified: Thu May  9 21:29:51 2024, max compression
```

## Comparing `daisy-1.1.tar` & `daisy-1.1.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:30:40.461687 daisy-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-18 22:30:34.000000 daisy-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-03-18 22:30:40.461687 daisy-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-03-18 22:30:34.000000 daisy-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:30:40.453687 daisy-1.1/daisy/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-18 22:30:34.000000 daisy-1.1/daisy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-03-18 22:30:34.000000 daisy-1.1/daisy/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-03-18 22:30:34.000000 daisy-1.1/daisy/block_bookkeeper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14350 2024-03-18 22:30:34.000000 daisy-1.1/daisy/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-03-18 22:30:34.000000 daisy-1.1/daisy/cl_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-03-18 22:30:34.000000 daisy-1.1/daisy/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-18 22:30:34.000000 daisy-1.1/daisy/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-18 22:30:34.000000 daisy-1.1/daisy/convenience.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-18 22:30:34.000000 daisy-1.1/daisy/coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25530 2024-03-18 22:30:34.000000 daisy-1.1/daisy/dependency_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-18 22:30:34.000000 daisy-1.1/daisy/freezable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-18 22:30:34.000000 daisy-1.1/daisy/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:30:40.457687 daisy-1.1/daisy/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-18 22:30:34.000000 daisy-1.1/daisy/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-18 22:30:34.000000 daisy-1.1/daisy/messages/acquire_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-18 22:30:34.000000 daisy-1.1/daisy/messages/block_failed.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-18 22:30:34.000000 daisy-1.1/daisy/messages/client_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-18 22:30:34.000000 daisy-1.1/daisy/messages/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-18 22:30:34.000000 daisy-1.1/daisy/messages/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-18 22:30:34.000000 daisy-1.1/daisy/messages/release_block.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-18 22:30:34.000000 daisy-1.1/daisy/messages/request_shutdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-18 22:30:34.000000 daisy-1.1/daisy/messages/send_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-18 22:30:34.000000 daisy-1.1/daisy/processing_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-03-18 22:30:34.000000 daisy-1.1/daisy/ready_surface.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-18 22:30:34.000000 daisy-1.1/daisy/roi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-03-18 22:30:34.000000 daisy-1.1/daisy/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8628 2024-03-18 22:30:34.000000 daisy-1.1/daisy/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-18 22:30:34.000000 daisy-1.1/daisy/server_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-03-18 22:30:34.000000 daisy-1.1/daisy/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-18 22:30:34.000000 daisy-1.1/daisy/task_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-18 22:30:34.000000 daisy-1.1/daisy/task_worker_pools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:30:40.457687 daisy-1.1/daisy/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-18 22:30:34.000000 daisy-1.1/daisy/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-18 22:30:34.000000 daisy-1.1/daisy/tcp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-18 22:30:34.000000 daisy-1.1/daisy/tcp/internal_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-18 22:30:34.000000 daisy-1.1/daisy/tcp/io_looper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-03-18 22:30:34.000000 daisy-1.1/daisy/tcp/tcp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-03-18 22:30:34.000000 daisy-1.1/daisy/tcp/tcp_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-03-18 22:30:34.000000 daisy-1.1/daisy/tcp/tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-03-18 22:30:34.000000 daisy-1.1/daisy/tcp/tcp_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-03-18 22:30:34.000000 daisy-1.1/daisy/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-03-18 22:30:34.000000 daisy-1.1/daisy/worker_pool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:30:40.457687 daisy-1.1/daisy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-03-18 22:30:40.000000 daisy-1.1/daisy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-18 22:30:40.000000 daisy-1.1/daisy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 22:30:40.000000 daisy-1.1/daisy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-18 22:30:40.000000 daisy-1.1/daisy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-18 22:30:40.000000 daisy-1.1/daisy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-18 22:30:34.000000 daisy-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 22:30:40.461687 daisy-1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 22:30:40.457687 daisy-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-18 22:30:34.000000 daisy-1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-18 22:30:34.000000 daisy-1.1/tests/test_clients_close.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-03-18 22:30:34.000000 daisy-1.1/tests/test_dependency_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-03-18 22:30:34.000000 daisy-1.1/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-18 22:30:34.000000 daisy-1.1/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-03-18 22:30:34.000000 daisy-1.1/tests/test_tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:51.769839 daisy-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 21:29:47.000000 daisy-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-09 21:29:51.769839 daisy-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-05-09 21:29:47.000000 daisy-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:51.761839 daisy-1.1.1/daisy/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/block_bookkeeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14350 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/cl_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25530 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/dependency_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/freezable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:51.765839 daisy-1.1.1/daisy/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/messages/acquire_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/messages/block_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/messages/client_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/messages/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/messages/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/messages/release_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/messages/request_shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/messages/send_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/processing_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/ready_surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/roi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/server_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/task_worker_pools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:51.765839 daisy-1.1.1/daisy/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/tcp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/tcp/internal_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/tcp/io_looper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/tcp/tcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/tcp/tcp_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/tcp/tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/tcp/tcp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-09 21:29:47.000000 daisy-1.1.1/daisy/worker_pool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:51.769839 daisy-1.1.1/daisy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-09 21:29:51.000000 daisy-1.1.1/daisy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-09 21:29:51.000000 daisy-1.1.1/daisy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 21:29:51.000000 daisy-1.1.1/daisy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 21:29:51.000000 daisy-1.1.1/daisy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 21:29:51.000000 daisy-1.1.1/daisy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-09 21:29:47.000000 daisy-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 21:29:51.769839 daisy-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 21:29:51.769839 daisy-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-09 21:29:47.000000 daisy-1.1.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-09 21:29:47.000000 daisy-1.1.1/tests/test_clients_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-09 21:29:47.000000 daisy-1.1.1/tests/test_dependency_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-05-09 21:29:47.000000 daisy-1.1.1/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 21:29:47.000000 daisy-1.1.1/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-09 21:29:47.000000 daisy-1.1.1/tests/test_tcp.py
```

### Comparing `daisy-1.1/LICENSE` & `daisy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `daisy-1.1/PKG-INFO` & `daisy-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daisy
-Version: 1.1
+Version: 1.1.1
 Summary: Blockwise task scheduler for processing large volumetric data.
 Author-email: William Patton <pattonw@hhmi.org>, Jan Funke <funkej@janelia.hhmi.org>, "Tri M. Nguyen" <tri_nguyen@hms.harvard.edu>, Caroline Malin-Mayor <malinmayorc@janelia.hhmi.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `daisy-1.1/README.md` & `daisy-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/__init__.py` & `daisy-1.1.1/daisy/__init__.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/block.py` & `daisy-1.1.1/daisy/block.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/block_bookkeeper.py` & `daisy-1.1.1/daisy/block_bookkeeper.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/blocks.py` & `daisy-1.1.1/daisy/blocks.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/cl_monitor.py` & `daisy-1.1.1/daisy/cl_monitor.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/client.py` & `daisy-1.1.1/daisy/client.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/context.py` & `daisy-1.1.1/daisy/context.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/convenience.py` & `daisy-1.1.1/daisy/convenience.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/dependency_graph.py` & `daisy-1.1.1/daisy/dependency_graph.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/logging.py` & `daisy-1.1.1/daisy/logging.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/processing_queue.py` & `daisy-1.1.1/daisy/processing_queue.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/ready_surface.py` & `daisy-1.1.1/daisy/ready_surface.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/scheduler.py` & `daisy-1.1.1/daisy/scheduler.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/server.py` & `daisy-1.1.1/daisy/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,14 +145,20 @@
 
                 logger.debug(
                     "No more pending blocks for task %s, terminating " "client",
                     message.task_id,
                 )
 
                 self._send_client_message(message.stream, RequestShutdown())
+                # in the case that the scheduler skips all blocks for a task
+                # because that task has previously been recruited, we now
+                # have tasks available to start that will hang forever unless
+                # started now since no more blocks are available for the existing
+                # task and no workers are running.
+                self._recruit_workers()
 
                 return
 
             # there are more blocks for this task, but none of them has its
             # dependencies fullfilled
             logger.debug(
                 "No currently ready blocks for task %s, delaying " "request",
```

### Comparing `daisy-1.1/daisy/server_observer.py` & `daisy-1.1.1/daisy/server_observer.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/task.py` & `daisy-1.1.1/daisy/task.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/task_state.py` & `daisy-1.1.1/daisy/task_state.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/task_worker_pools.py` & `daisy-1.1.1/daisy/task_worker_pools.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/tcp/internal_messages.py` & `daisy-1.1.1/daisy/tcp/internal_messages.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/tcp/io_looper.py` & `daisy-1.1.1/daisy/tcp/io_looper.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/tcp/tcp_client.py` & `daisy-1.1.1/daisy/tcp/tcp_client.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/tcp/tcp_server.py` & `daisy-1.1.1/daisy/tcp/tcp_server.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/tcp/tcp_stream.py` & `daisy-1.1.1/daisy/tcp/tcp_stream.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/worker.py` & `daisy-1.1.1/daisy/worker.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy/worker_pool.py` & `daisy-1.1.1/daisy/worker_pool.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/daisy.egg-info/PKG-INFO` & `daisy-1.1.1/daisy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daisy
-Version: 1.1
+Version: 1.1.1
 Summary: Blockwise task scheduler for processing large volumetric data.
 Author-email: William Patton <pattonw@hhmi.org>, Jan Funke <funkej@janelia.hhmi.org>, "Tri M. Nguyen" <tri_nguyen@hms.harvard.edu>, Caroline Malin-Mayor <malinmayorc@janelia.hhmi.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `daisy-1.1/daisy.egg-info/SOURCES.txt` & `daisy-1.1.1/daisy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `daisy-1.1/pyproject.toml` & `daisy-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "daisy"
 description = "Blockwise task scheduler for processing large volumetric data."
-version = "1.1"
+version = "1.1.1"
 license = {text = "MIT"}
 readme = "README.md"
 authors = [
   {name = "William Patton", email = "pattonw@hhmi.org"},
   {name = "Jan Funke", email = "funkej@janelia.hhmi.org"},
   {name = "Tri M. Nguyen", email = "tri_nguyen@hms.harvard.edu"},
   {name = "Caroline Malin-Mayor", email = "malinmayorc@janelia.hhmi.org"}
```

### Comparing `daisy-1.1/tests/test_client.py` & `daisy-1.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/tests/test_clients_close.py` & `daisy-1.1.1/tests/test_clients_close.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/tests/test_dependency_graph.py` & `daisy-1.1.1/tests/test_dependency_graph.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/tests/test_scheduler.py` & `daisy-1.1.1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/tests/test_server.py` & `daisy-1.1.1/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `daisy-1.1/tests/test_tcp.py` & `daisy-1.1.1/tests/test_tcp.py`

 * *Files identical despite different names*


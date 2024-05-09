# Comparing `tmp/esdbclient-1.1b1.tar.gz` & `tmp/esdbclient-1.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esdbclient-1.1b1.tar", max compression
+gzip compressed data, was "esdbclient-1.1b2.tar", max compression
```

## Comparing `esdbclient-1.1b1.tar` & `esdbclient-1.1b2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-1.1b1/LICENSE
--rw-r--r--   0        0        0   146551 2024-05-07 17:49:34.578510 esdbclient-1.1b1/README.md
--rw-r--r--   0        0        0      665 2024-04-29 21:28:03.270446 esdbclient-1.1b1/esdbclient/__init__.py
--rw-r--r--   0        0        0    61816 2024-05-07 17:49:33.437999 esdbclient-1.1b1/esdbclient/asyncio_client.py
--rw-r--r--   0        0        0    68114 2024-05-07 17:49:33.438828 esdbclient-1.1b1/esdbclient/client.py
--rw-r--r--   0        0        0    11967 2024-05-07 17:49:33.439565 esdbclient-1.1b1/esdbclient/common.py
--rw-r--r--   0        0        0     3819 2024-05-07 17:49:33.440928 esdbclient-1.1b1/esdbclient/connection.py
--rw-r--r--   0        0        0    10170 2024-03-20 01:14:49.708462 esdbclient-1.1b1/esdbclient/connection_spec.py
--rw-r--r--   0        0        0     3284 2024-04-29 21:27:57.792242 esdbclient-1.1b1/esdbclient/events.py
--rw-r--r--   0        0        0     5948 2024-04-26 00:35:12.280754 esdbclient-1.1b1/esdbclient/exceptions.py
--rw-r--r--   0        0        0     5532 2024-04-04 00:22:38.215558 esdbclient-1.1b1/esdbclient/gossip.py
--rw-r--r--   0        0        0    82861 2024-04-29 22:32:08.972569 esdbclient-1.1b1/esdbclient/persistent.py
--rw-r--r--   0        0        0    27488 2024-05-07 17:49:33.442344 esdbclient-1.1b1/esdbclient/projections.py
--rw-r--r--   0        0        0    14166 2024-05-02 13:49:41.020003 esdbclient-1.1b1/esdbclient/protos/Grpc/cluster_pb2.py
--rw-r--r--   0        0        0    37958 2024-05-02 13:49:41.275519 esdbclient-1.1b1/esdbclient/protos/Grpc/cluster_pb2.pyi
--rw-r--r--   0        0        0    19336 2024-05-02 13:49:40.865930 esdbclient-1.1b1/esdbclient/protos/Grpc/cluster_pb2_grpc.py
--rw-r--r--   0        0        0     1916 2024-05-02 13:49:40.420076 esdbclient-1.1b1/esdbclient/protos/Grpc/code_pb2.py
--rw-r--r--   0        0        0    13555 2024-05-02 13:49:40.538653 esdbclient-1.1b1/esdbclient/protos/Grpc/code_pb2.pyi
--rw-r--r--   0        0        0      158 2024-05-02 13:49:40.389375 esdbclient-1.1b1/esdbclient/protos/Grpc/code_pb2_grpc.py
--rw-r--r--   0        0        0     3030 2024-05-02 13:49:40.543509 esdbclient-1.1b1/esdbclient/protos/Grpc/gossip_pb2.py
--rw-r--r--   0        0        0     5524 2024-05-02 13:49:40.640362 esdbclient-1.1b1/esdbclient/protos/Grpc/gossip_pb2.pyi
--rw-r--r--   0        0        0     2752 2024-05-02 13:49:40.532290 esdbclient-1.1b1/esdbclient/protos/Grpc/gossip_pb2_grpc.py
--rw-r--r--   0        0        0    23846 2024-05-02 13:49:41.404767 esdbclient-1.1b1/esdbclient/protos/Grpc/persistent_pb2.py
--rw-r--r--   0        0        0    73220 2024-05-02 13:49:41.830902 esdbclient-1.1b1/esdbclient/protos/Grpc/persistent_pb2.pyi
--rw-r--r--   0        0        0    15771 2024-05-02 13:49:40.799320 esdbclient-1.1b1/esdbclient/protos/Grpc/persistent_pb2_grpc.py
--rw-r--r--   0        0        0    10621 2024-05-07 17:49:33.443252 esdbclient-1.1b1/esdbclient/protos/Grpc/projections_pb2.py
--rw-r--r--   0        0        0    25437 2024-05-07 17:49:33.443914 esdbclient-1.1b1/esdbclient/protos/Grpc/projections_pb2.pyi
--rw-r--r--   0        0        0    18841 2024-05-07 17:49:33.444347 esdbclient-1.1b1/esdbclient/protos/Grpc/projections_pb2_grpc.py
--rw-r--r--   0        0        0     4187 2024-05-02 13:49:40.665078 esdbclient-1.1b1/esdbclient/protos/Grpc/shared_pb2.py
--rw-r--r--   0        0        0     9874 2024-05-02 13:49:40.801616 esdbclient-1.1b1/esdbclient/protos/Grpc/shared_pb2.pyi
--rw-r--r--   0        0        0      158 2024-05-02 13:49:40.534944 esdbclient-1.1b1/esdbclient/protos/Grpc/shared_pb2_grpc.py
--rw-r--r--   0        0        0     1813 2024-05-02 13:49:40.593327 esdbclient-1.1b1/esdbclient/protos/Grpc/status_pb2.py
--rw-r--r--   0        0        0     2838 2024-05-02 13:49:40.608113 esdbclient-1.1b1/esdbclient/protos/Grpc/status_pb2.pyi
--rw-r--r--   0        0        0      158 2024-05-02 13:49:40.550725 esdbclient-1.1b1/esdbclient/protos/Grpc/status_pb2_grpc.py
--rw-r--r--   0        0        0    21622 2024-05-02 13:49:41.325300 esdbclient-1.1b1/esdbclient/protos/Grpc/streams_pb2.py
--rw-r--r--   0        0        0    72778 2024-05-02 13:49:41.844782 esdbclient-1.1b1/esdbclient/protos/Grpc/streams_pb2.pyi
--rw-r--r--   0        0        0     9787 2024-05-02 13:49:40.788920 esdbclient-1.1b1/esdbclient/protos/Grpc/streams_pb2_grpc.py
--rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-1.1b1/esdbclient/py.typed
--rw-r--r--   0        0        0    52257 2024-04-29 21:31:01.778647 esdbclient-1.1b1/esdbclient/streams.py
--rw-r--r--   0        0        0     2778 2024-05-07 17:49:33.446041 esdbclient-1.1b1/pyproject.toml
--rw-r--r--   0        0        0   147589 1970-01-01 00:00:00.000000 esdbclient-1.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1520 2022-06-23 14:19:18.317032 esdbclient-1.1b2/LICENSE
+-rw-r--r--   0        0        0   147009 2024-05-09 16:08:18.286706 esdbclient-1.1b2/README.md
+-rw-r--r--   0        0        0      665 2024-05-09 12:30:42.655858 esdbclient-1.1b2/esdbclient/__init__.py
+-rw-r--r--   0        0        0    60668 2024-05-09 15:19:09.242192 esdbclient-1.1b2/esdbclient/asyncio_client.py
+-rw-r--r--   0        0        0    66978 2024-05-09 15:19:09.232635 esdbclient-1.1b2/esdbclient/client.py
+-rw-r--r--   0        0        0    12402 2024-05-09 13:51:54.783176 esdbclient-1.1b2/esdbclient/common.py
+-rw-r--r--   0        0        0     3819 2024-05-09 12:30:42.661945 esdbclient-1.1b2/esdbclient/connection.py
+-rw-r--r--   0        0        0    10170 2024-05-09 12:30:42.663682 esdbclient-1.1b2/esdbclient/connection_spec.py
+-rw-r--r--   0        0        0     3422 2024-05-09 12:30:42.664490 esdbclient-1.1b2/esdbclient/events.py
+-rw-r--r--   0        0        0     6117 2024-05-09 13:25:45.934297 esdbclient-1.1b2/esdbclient/exceptions.py
+-rw-r--r--   0        0        0     5532 2024-05-09 12:30:42.667329 esdbclient-1.1b2/esdbclient/gossip.py
+-rw-r--r--   0        0        0    82861 2024-05-09 12:30:42.668861 esdbclient-1.1b2/esdbclient/persistent.py
+-rw-r--r--   0        0        0    24972 2024-05-09 15:21:18.742508 esdbclient-1.1b2/esdbclient/projections.py
+-rw-r--r--   0        0        0    14166 2024-05-09 12:30:42.671328 esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2.py
+-rw-r--r--   0        0        0    37958 2024-05-02 13:49:41.275519 esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2.pyi
+-rw-r--r--   0        0        0    19336 2024-05-02 13:49:40.865930 esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2_grpc.py
+-rw-r--r--   0        0        0     1916 2024-05-09 12:30:42.672190 esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2.py
+-rw-r--r--   0        0        0    13555 2024-05-02 13:49:40.538653 esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-02 13:49:40.389375 esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2_grpc.py
+-rw-r--r--   0        0        0     3030 2024-05-09 12:30:42.672780 esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2.py
+-rw-r--r--   0        0        0     5524 2024-05-02 13:49:40.640362 esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2.pyi
+-rw-r--r--   0        0        0     2752 2024-05-02 13:49:40.532290 esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2_grpc.py
+-rw-r--r--   0        0        0    23846 2024-05-09 12:30:42.673979 esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2.py
+-rw-r--r--   0        0        0    73220 2024-05-02 13:49:41.830902 esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2.pyi
+-rw-r--r--   0        0        0    15771 2024-05-02 13:49:40.799320 esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2_grpc.py
+-rw-r--r--   0        0        0    10621 2024-05-09 12:30:42.674904 esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2.py
+-rw-r--r--   0        0        0    25437 2024-05-09 12:30:42.675584 esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2.pyi
+-rw-r--r--   0        0        0    18841 2024-05-09 12:30:42.676247 esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2_grpc.py
+-rw-r--r--   0        0        0     4187 2024-05-09 12:30:42.677057 esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2.py
+-rw-r--r--   0        0        0     9874 2024-05-02 13:49:40.801616 esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-02 13:49:40.534944 esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2_grpc.py
+-rw-r--r--   0        0        0     1813 2024-05-09 12:30:42.677868 esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2.py
+-rw-r--r--   0        0        0     2838 2024-05-02 13:49:40.608113 esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2.pyi
+-rw-r--r--   0        0        0      158 2024-05-02 13:49:40.550725 esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2_grpc.py
+-rw-r--r--   0        0        0    21622 2024-05-09 12:30:42.678599 esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2.py
+-rw-r--r--   0        0        0    72778 2024-05-09 12:30:42.679517 esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2.pyi
+-rw-r--r--   0        0        0     9787 2024-05-02 13:49:40.788920 esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2022-06-23 14:19:18.321130 esdbclient-1.1b2/esdbclient/py.typed
+-rw-r--r--   0        0        0    52319 2024-05-09 12:30:42.680251 esdbclient-1.1b2/esdbclient/streams.py
+-rw-r--r--   0        0        0     2778 2024-05-09 16:44:18.274739 esdbclient-1.1b2/pyproject.toml
+-rw-r--r--   0        0        0   148047 1970-01-01 00:00:00.000000 esdbclient-1.1b2/PKG-INFO
```

### Comparing `esdbclient-1.1b1/LICENSE` & `esdbclient-1.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/README.md` & `esdbclient-1.1b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -239,18 +239,18 @@
   * [Replay parked events](#replay-parked-events)
   * [Get subscription info](#get-subscription-info)
   * [List subscriptions](#list-subscriptions)
   * [List subscriptions to stream](#list-subscriptions-to-stream)
   * [Delete subscription](#delete-subscription)
 * [Projections](#projections)
   * [Create projection](#create-projection)
-  * [Update projection](#update-projection)
-  * [Get projection statistics](#get-projection-statistics)
   * [Get projection state](#get-projection-state)
   * [Get projection result](#get-projection-result)
+  * [Get projection statistics](#get-projection-statistics)
+  * [Update projection](#update-projection)
   * [Enable projection](#enable-projection)
   * [Disable projection](#disable-projection)
   * [Reset projection](#reset-projection)
   * [Delete projection](#delete-projection)
   * [Restart projections subsystem](#restart-projections-subsystem)
 * [Call credentials](#call-credentials)
   * [Construct call credentials](#construct-call-credentials)
@@ -2830,52 +2830,58 @@
     stream_name=stream_name2,
 )
 ```
 
 
 ## Projections<a id="projections"></a>
 
+Please refer to the [EventStoreDB documentation](https://developers.eventstore.com/server/v23.10/projections.html)
+for more information on projections in EventStoreDB.
+
 ### Create projection<a id="create-projection"></a>
 
 The `create_projection()` method can be used to create a projection.
 
-This method has a required `query` argument, which is a Python `str` that
-defines what the projection will do.
+This method has two required arguments, `name` and `query`.
+
+This required `name` argument is a Python `str` that specifies the name of the projection.
 
-This method also has six optional arguments, `name`, `continuous`, `emit_enabled`,
-`track_emitted_streams`, `timeout`, and `credentials`.
+This required `query` argument is a Python `str` that defines what the projection will do.
 
-The optional `name` argument is a Python `str` which specifies the name of the projection.
-If a name is provided, the projection will either be a "transient" or a "continuous"
-projection. Otherwise, the projection will be a "one time" projection.
-
-The optional `continuous` argument is a Python `bool` which specifies whether a
-projection will be a "continuous" projection. If a `True` value is specified, the
-projection will be a "continuous" projection, otherwise the projection will be a
-"transient" projection. The default value of `continuous` is `False`.
+This method also has four optional arguments, `emit_enabled`,
+`track_emitted_streams`, `timeout`, and `credentials`.
 
 The optional `emit_enabled` argument is a Python `bool` which specifies whether a
 projection will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events, otherwise the projection will not be able to emit events.
 The default value of `emit_enabled` is `False`.
 
+Please note, if your projection query includes a call to `emit()` then `emit_enabled`
+must be `True`, otherwise the projection will not run.
+
 The optional `track_emitted_streams` argument is a Python `bool` which specifies whether
 a projection will have its emitted streams tracked. If a `True` value is specified, the
 projection will have its emitted streams tracked, otherwise the projection will not
 have its emitted streams tracked. The default value of `track_emitted_streams` is `False`.
 
+The purpose of tracking emitted streams is that they can optionally be deleted when
+a projection is deleted (see the `delete_projection()` method for more details).
+
+Please note, if you set `track_emitted_streams` to `True`, then you must also set
+`emit_enabled` to `True`, otherwise an error will be raised by this method.
+
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
-In the example below, a continuous projection is created that processes
-events appended to `stream_name2`. The "state" of the projection is
-initialised to have a "count" that is incremented once for each event.
+In the example below, a projection is created that processes events appended to
+`stream_name2`. The "state" of the projection is initialised to have a "count" that
+is incremented once for each event.
 
 ```python
 projection_name = str(uuid.uuid4())
 
 projection_query = """fromStream('%s')
 .when({
   $init: function(){
@@ -2895,18 +2901,25 @@
 })
 .outputState()
 """  % stream_name2
 
 client.create_projection(
     name=projection_name,
     query=projection_query,
-    continuous=True,
 )
 ```
 
+Please note, the `outputState()` call is optional, and causes the state of the
+projection to be persisted in a "result" stream. The default name of the result stream
+is `$projections-{projection_name}-result`, and this name can be used to read from and
+subscribe to the results stream with the `get_stream()`, `read_stream()`,
+`subscribe_stream()`, `create_subscription_to_stream()` and `read_subscription_to_stream()`
+methods.
+
+
 ### Get projection state<a id="get-projection-state"></a>
 
 The `get_projection_state()` method can be used to get a projection's state.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of a projection.
 
@@ -2937,15 +2950,15 @@
 The `get_projection_result()` method can be used to get a projection's result.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of a projection.
 
 This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
 
-The optional `partition` argument is a Python `str` which specifies a partition...
+The optional `partition` argument is a Python `str` which specifies a partition.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -2958,40 +2971,30 @@
 assert projection_result.value == {'count': 3}
 ```
 
 ### Get projection statistics<a id="get-projection-statistics"></a>
 
 The `get_projection_statistucs()` method can be used to get projection statistics.
 
-This method also has seven optional arguments, `name`, `all`, `transient`,
-`continuous`, `one_time`, `timeout`, and `credentials`.
-
-The optional `name` argument is a Python `str` that specifies the name of a
-projection. If the name of a projection is specified, this method will return
-a single `ProjectionStatistics` object that represents that projection. Otherwise
-this method will return a sequence of `ProjectionStatistics` objects.
-
-The optional `all` argument is Python `bool` that can be used to request statistics
-for all projections.
+This method has a required `name` argument, which is a Python `str` that specifies the
+name of a projection.
 
-The optional `transient` argument is Python `bool` that can be used to request
-statistics for all "transient" projections.
-
-The optional `continuous` argument is Python `bool` that can be used to request
-statistics for all "continuous" projections.
+This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
 
-The optional `one_time` argument is Python `bool` that can be used to request
-statistics for all "one time" projections.
+The optional `partition` argument is a Python `str` which specifies a partition.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
+This method returns a `ProjectionStatistics` object that represents
+the named projection.
+
 ```python
 statistics = client.get_projection_statistics(name=projection_name)
 ```
 
 A `ProjectionStatistics` object is returned. The attributes of this object
 have values that represent the progress of the projection.
 
@@ -3007,15 +3010,20 @@
 The required `query` argument is a Python `str` which defines what the projection will do.
 
 This method also has three optional arguments, `emit_enabled`, `timeout`, and `credentials`.
 
 The optional `emit_enabled` argument is a Python `bool` which specifies whether a
 projection will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events. If a `False` value is specified, the projection will not
-be able to emit events. The default value of `emit_enabled` is `None`.
+be able to emit events. The default value of `emit_enabled` is `False`.
+
+Please note, if your projection query includes a call to `emit()` then `emit_enabled`
+must be `True`, otherwise the projection will not run.
+
+Please note, it is not possible to update `track_emitted_streams` via the gRPC API.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -3025,15 +3033,15 @@
 
 ### Enable projection<a id="enable-projection"></a>
 
 The `enable_projection()` method can be used to enable a projection that was previously
 disabled.
 
 This method has a required `name` argument, which is a Python `str` that
-specifies the name of the projection to be disabled.
+specifies the name of the projection to be enabled.
 
 This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
@@ -3097,15 +3105,18 @@
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be deleted.
 
 This method also has five optional arguments, `delete_emitted_streams`,
 `delete_state_stream`, `delete_checkpoint_stream`, `timeout`, and `credentials`.
 
-The optional `delete_emitted_streams` argument is a Python `bool` which...
+The optional `delete_emitted_streams` argument is a Python `bool` which specifies
+that the emitted streams will be deleted. For emitted streams to be deleted, they
+must have been tracked (see the `track_emitted_streams` argument of the `create_projection()`
+method.)
 
 The optional `delete_state_stream` argument is a Python `bool` which...
 
 The optional `delete_checkpoint_stream` argument is a Python `bool` which...
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
```

#### html2text {}

```diff
@@ -115,23 +115,23 @@
 consumer) * [Update subscription to all](#update-subscription-to-all) * [Create
 subscription to stream](#create-subscription-to-stream) * [Read subscription to
 stream](#read-subscription-to-stream) * [Update subscription to stream]
 (#update-subscription-to-stream) * [Replay parked events](#replay-parked-
 events) * [Get subscription info](#get-subscription-info) * [List
 subscriptions](#list-subscriptions) * [List subscriptions to stream](#list-
 subscriptions-to-stream) * [Delete subscription](#delete-subscription) *
-[Projections](#projections) * [Create projection](#create-projection) * [Update
-projection](#update-projection) * [Get projection statistics](#get-projection-
-statistics) * [Get projection state](#get-projection-state) * [Get projection
-result](#get-projection-result) * [Enable projection](#enable-projection) *
-[Disable projection](#disable-projection) * [Reset projection](#reset-
-projection) * [Delete projection](#delete-projection) * [Restart projections
-subsystem](#restart-projections-subsystem) * [Call credentials](#call-
-credentials) * [Construct call credentials](#construct-call-credentials) *
-[Connection](#connection) * [Reconnect](#reconnect) * [Close](#close) *
+[Projections](#projections) * [Create projection](#create-projection) * [Get
+projection state](#get-projection-state) * [Get projection result](#get-
+projection-result) * [Get projection statistics](#get-projection-statistics) *
+[Update projection](#update-projection) * [Enable projection](#enable-
+projection) * [Disable projection](#disable-projection) * [Reset projection]
+(#reset-projection) * [Delete projection](#delete-projection) * [Restart
+projections subsystem](#restart-projections-subsystem) * [Call credentials]
+(#call-credentials) * [Construct call credentials](#construct-call-credentials)
+* [Connection](#connection) * [Reconnect](#reconnect) * [Close](#close) *
 [Asyncio client](#asyncio-client) * [Synopsis](#synopsis-1) * [Notes](#notes) *
 [Regular expression filters](#regular-expression-filters) * [Reconnect and
 retry method decorators](#reconnect-and-retry-method-decorators) *
 [Contributors](#contributors) * [Install Poetry](#install-poetry) * [Setup for
 PyCharm users](#setup-for-pycharm-users) * [Setup from command line](#setup-
 from-command-line) * [Project Makefile commands](#project-makefile-commands) ##
 Install package It is recommended to install Python packages into a Python
@@ -1490,115 +1490,119 @@
 `credentials` argument, which can be used to override call credentials derived
 from the connection string URI. The example below deletes the persistent
 subscription `group_name1` which was created by calling
 `create_subscription_to_all()`. ```python client.delete_subscription
 ( group_name=group_name1, ) ``` The example below deleted the persistent
 subscription `group_name2` on `stream_name2` which was created by calling
 `create_subscription_to_stream()`. ```python client.delete_subscription
-( group_name=group_name2, stream_name=stream_name2, ) ``` ## Projections ###
-Create projection The `create_projection()` method can be used to create a
-projection. This method has a required `query` argument, which is a Python
-`str` that defines what the projection will do. This method also has six
-optional arguments, `name`, `continuous`, `emit_enabled`,
-`track_emitted_streams`, `timeout`, and `credentials`. The optional `name`
-argument is a Python `str` which specifies the name of the projection. If a
-name is provided, the projection will either be a "transient" or a "continuous"
-projection. Otherwise, the projection will be a "one time" projection. The
-optional `continuous` argument is a Python `bool` which specifies whether a
-projection will be a "continuous" projection. If a `True` value is specified,
-the projection will be a "continuous" projection, otherwise the projection will
-be a "transient" projection. The default value of `continuous` is `False`. The
-optional `emit_enabled` argument is a Python `bool` which specifies whether a
-projection will be able to emit events. If a `True` value is specified, the
-projection will be able to emit events, otherwise the projection will not be
-able to emit events. The default value of `emit_enabled` is `False`. The
+( group_name=group_name2, stream_name=stream_name2, ) ``` ## Projections Please
+refer to the [EventStoreDB documentation](https://developers.eventstore.com/
+server/v23.10/projections.html) for more information on projections in
+EventStoreDB. ### Create projection The `create_projection()` method can be
+used to create a projection. This method has two required arguments, `name` and
+`query`. This required `name` argument is a Python `str` that specifies the
+name of the projection. This required `query` argument is a Python `str` that
+defines what the projection will do. This method also has four optional
+arguments, `emit_enabled`, `track_emitted_streams`, `timeout`, and
+`credentials`. The optional `emit_enabled` argument is a Python `bool` which
+specifies whether a projection will be able to emit events. If a `True` value
+is specified, the projection will be able to emit events, otherwise the
+projection will not be able to emit events. The default value of `emit_enabled`
+is `False`. Please note, if your projection query includes a call to `emit()`
+then `emit_enabled` must be `True`, otherwise the projection will not run. The
 optional `track_emitted_streams` argument is a Python `bool` which specifies
 whether a projection will have its emitted streams tracked. If a `True` value
 is specified, the projection will have its emitted streams tracked, otherwise
 the projection will not have its emitted streams tracked. The default value of
-`track_emitted_streams` is `False`. The optional `timeout` argument is a Python
-`float` which sets a maximum duration, in seconds, for the completion of the
-gRPC operation. The optional `credentials` argument can be used to override
-call credentials derived from the connection string URI. In the example below,
-a continuous projection is created that processes events appended to
-`stream_name2`. The "state" of the projection is initialised to have a "count"
-that is incremented once for each event. ```python projection_name = str
-(uuid.uuid4()) projection_query = """fromStream('%s') .when({ $init: function()
-{ return { count: 0 }; }, OrderCreated: function(s,e){ s.count += 1; },
-OrderUpdated: function(s,e){ s.count += 1; }, OrderDeleted: function(s,e)
-{ s.count += 1; } }) .outputState() """ % stream_name2 client.create_projection
-( name=projection_name, query=projection_query, continuous=True, ) ``` ### Get
-projection state The `get_projection_state()` method can be used to get a
-projection's state. This method has a required `name` argument, which is a
-Python `str` that specifies the name of a projection. This method also has
-three optional arguments, `partition`, `timeout`, and `credentials`. The
-optional `partition` argument is a Python `str` which specifies a partition...
-The optional `timeout` argument is a Python `float` which sets a maximum
-duration, in seconds, for the completion of the gRPC operation. The optional
-`credentials` argument can be used to override call credentials derived from
-the connection string URI. In the example below, after sleeping for 1 second to
-allow the projection to process all the recorded events, the projection "state"
-is obtained. We can see that the projection has processed three events.
-```python sleep(1) # allow time for projection to process recorded events
-projection_state = client.get_projection_state(name=projection_name) assert
-projection_state.value == {'count': 3} ``` ### Get projection result The
-`get_projection_result()` method can be used to get a projection's result. This
+`track_emitted_streams` is `False`. The purpose of tracking emitted streams is
+that they can optionally be deleted when a projection is deleted (see the
+`delete_projection()` method for more details). Please note, if you set
+`track_emitted_streams` to `True`, then you must also set `emit_enabled` to
+`True`, otherwise an error will be raised by this method. The optional
+`timeout` argument is a Python `float` which sets a maximum duration, in
+seconds, for the completion of the gRPC operation. The optional `credentials`
+argument can be used to override call credentials derived from the connection
+string URI. In the example below, a projection is created that processes events
+appended to `stream_name2`. The "state" of the projection is initialised to
+have a "count" that is incremented once for each event. ```python
+projection_name = str(uuid.uuid4()) projection_query = """fromStream('%s')
+.when({ $init: function(){ return { count: 0 }; }, OrderCreated: function(s,e)
+{ s.count += 1; }, OrderUpdated: function(s,e){ s.count += 1; }, OrderDeleted:
+function(s,e){ s.count += 1; } }) .outputState() """ % stream_name2
+client.create_projection( name=projection_name, query=projection_query, ) ```
+Please note, the `outputState()` call is optional, and causes the state of the
+projection to be persisted in a "result" stream. The default name of the result
+stream is `$projections-{projection_name}-result`, and this name can be used to
+read from and subscribe to the results stream with the `get_stream()`,
+`read_stream()`, `subscribe_stream()`, `create_subscription_to_stream()` and
+`read_subscription_to_stream()` methods. ### Get projection state The
+`get_projection_state()` method can be used to get a projection's state. This
 method has a required `name` argument, which is a Python `str` that specifies
 the name of a projection. This method also has three optional arguments,
 `partition`, `timeout`, and `credentials`. The optional `partition` argument is
 a Python `str` which specifies a partition... The optional `timeout` argument
 is a Python `float` which sets a maximum duration, in seconds, for the
 completion of the gRPC operation. The optional `credentials` argument can be
 used to override call credentials derived from the connection string URI. In
-the example below, the projection "result" is obtained. We can see that the
-projection has processed three events. ```python projection_result =
+the example below, after sleeping for 1 second to allow the projection to
+process all the recorded events, the projection "state" is obtained. We can see
+that the projection has processed three events. ```python sleep(1) # allow time
+for projection to process recorded events projection_state =
+client.get_projection_state(name=projection_name) assert projection_state.value
+== {'count': 3} ``` ### Get projection result The `get_projection_result()`
+method can be used to get a projection's result. This method has a required
+`name` argument, which is a Python `str` that specifies the name of a
+projection. This method also has three optional arguments, `partition`,
+`timeout`, and `credentials`. The optional `partition` argument is a Python
+`str` which specifies a partition. The optional `timeout` argument is a Python
+`float` which sets a maximum duration, in seconds, for the completion of the
+gRPC operation. The optional `credentials` argument can be used to override
+call credentials derived from the connection string URI. In the example below,
+the projection "result" is obtained. We can see that the projection has
+processed three events. ```python projection_result =
 client.get_projection_result(name=projection_name) assert
 projection_result.value == {'count': 3} ``` ### Get projection statistics The
 `get_projection_statistucs()` method can be used to get projection statistics.
-This method also has seven optional arguments, `name`, `all`, `transient`,
-`continuous`, `one_time`, `timeout`, and `credentials`. The optional `name`
-argument is a Python `str` that specifies the name of a projection. If the name
-of a projection is specified, this method will return a single
-`ProjectionStatistics` object that represents that projection. Otherwise this
-method will return a sequence of `ProjectionStatistics` objects. The optional
-`all` argument is Python `bool` that can be used to request statistics for all
-projections. The optional `transient` argument is Python `bool` that can be
-used to request statistics for all "transient" projections. The optional
-`continuous` argument is Python `bool` that can be used to request statistics
-for all "continuous" projections. The optional `one_time` argument is Python
-`bool` that can be used to request statistics for all "one time" projections.
+This method has a required `name` argument, which is a Python `str` that
+specifies the name of a projection. This method also has three optional
+arguments, `partition`, `timeout`, and `credentials`. The optional `partition`
+argument is a Python `str` which specifies a partition. The optional `timeout`
+argument is a Python `float` which sets a maximum duration, in seconds, for the
+completion of the gRPC operation. The optional `credentials` argument can be
+used to override call credentials derived from the connection string URI. This
+method returns a `ProjectionStatistics` object that represents the named
+projection. ```python statistics = client.get_projection_statistics
+(name=projection_name) ``` A `ProjectionStatistics` object is returned. The
+attributes of this object have values that represent the progress of the
+projection. ### Update projection The `update_projection()` method can be used
+to update a projection. This method has two required arguments, `name` and
+`query`. The required `name` argument is a Python `str` which specifies the
+name of the projection to be updated. The required `query` argument is a Python
+`str` which defines what the projection will do. This method also has three
+optional arguments, `emit_enabled`, `timeout`, and `credentials`. The optional
+`emit_enabled` argument is a Python `bool` which specifies whether a projection
+will be able to emit events. If a `True` value is specified, the projection
+will be able to emit events. If a `False` value is specified, the projection
+will not be able to emit events. The default value of `emit_enabled` is
+`False`. Please note, if your projection query includes a call to `emit()` then
+`emit_enabled` must be `True`, otherwise the projection will not run. Please
+note, it is not possible to update `track_emitted_streams` via the gRPC API.
 The optional `timeout` argument is a Python `float` which sets a maximum
 duration, in seconds, for the completion of the gRPC operation. The optional
 `credentials` argument can be used to override call credentials derived from
-the connection string URI. ```python statistics =
-client.get_projection_statistics(name=projection_name) ``` A
-`ProjectionStatistics` object is returned. The attributes of this object have
-values that represent the progress of the projection. ### Update projection The
-`update_projection()` method can be used to update a projection. This method
-has two required arguments, `name` and `query`. The required `name` argument is
-a Python `str` which specifies the name of the projection to be updated. The
-required `query` argument is a Python `str` which defines what the projection
-will do. This method also has three optional arguments, `emit_enabled`,
-`timeout`, and `credentials`. The optional `emit_enabled` argument is a Python
-`bool` which specifies whether a projection will be able to emit events. If a
-`True` value is specified, the projection will be able to emit events. If a
-`False` value is specified, the projection will not be able to emit events. The
-default value of `emit_enabled` is `None`. The optional `timeout` argument is a
-Python `float` which sets a maximum duration, in seconds, for the completion of
-the gRPC operation. The optional `credentials` argument can be used to override
-call credentials derived from the connection string URI. ```python
-client.update_projection(name=projection_name, query=projection_query) ``` ###
-Enable projection The `enable_projection()` method can be used to enable a
-projection that was previously disabled. This method has a required `name`
-argument, which is a Python `str` that specifies the name of the projection to
-be disabled. This method also has two optional arguments, `timeout` and
-`credentials`. The optional `timeout` argument is a Python `float` which sets a
-maximum duration, in seconds, for the completion of the gRPC operation. The
-optional `credentials` argument can be used to override call credentials
-derived from the connection string URI. ```python client.enable_projection
+the connection string URI. ```python client.update_projection
+(name=projection_name, query=projection_query) ``` ### Enable projection The
+`enable_projection()` method can be used to enable a projection that was
+previously disabled. This method has a required `name` argument, which is a
+Python `str` that specifies the name of the projection to be enabled. This
+method also has two optional arguments, `timeout` and `credentials`. The
+optional `timeout` argument is a Python `float` which sets a maximum duration,
+in seconds, for the completion of the gRPC operation. The optional
+`credentials` argument can be used to override call credentials derived from
+the connection string URI. ```python client.enable_projection
 (name=projection_name) ``` ### Disable projection The `disable_projection()`
 method can be used to disable a projection. This method has a required `name`
 argument, which is a Python `str` that specifies the name of the projection to
 be disabled. This method also has three optional arguments, `write_checkpoint`,
 `timeout`, and `credentials`. The optional `write_checkpoint` argument is a
 Python `bool` which specifies whether a checkpoint will be written when the
 projection is disabled. If `write_checkpoint` is `True` a checkpoint will be
@@ -1621,26 +1625,29 @@
 argument can be used to override call credentials derived from the connection
 string URI. ```python client.reset_projection(name=projection_name) ``` ###
 Delete projection The `delete_projection()` method can be used to delete a
 projection. This method has a required `name` argument, which is a Python `str`
 that specifies the name of the projection to be deleted. This method also has
 five optional arguments, `delete_emitted_streams`, `delete_state_stream`,
 `delete_checkpoint_stream`, `timeout`, and `credentials`. The optional
-`delete_emitted_streams` argument is a Python `bool` which... The optional
-`delete_state_stream` argument is a Python `bool` which... The optional
-`delete_checkpoint_stream` argument is a Python `bool` which... The optional
-`timeout` argument is a Python `float` which sets a maximum duration, in
-seconds, for the completion of the gRPC operation. The optional `credentials`
-argument can be used to override call credentials derived from the connection
-string URI. ```python client.delete_projection(name=projection_name) ``` ###
-Restart projections subsystem The `restart_projections_subsystem()` method can
-be used to restart the projections subsystem. This method also has two optional
-arguments, `timeout` and `credentials`. The optional `timeout` argument is a
-Python `float` which sets a maximum duration, in seconds, for the completion of
-the gRPC operation. The optional `credentials` argument can be used to override
+`delete_emitted_streams` argument is a Python `bool` which specifies that the
+emitted streams will be deleted. For emitted streams to be deleted, they must
+have been tracked (see the `track_emitted_streams` argument of the
+`create_projection()` method.) The optional `delete_state_stream` argument is a
+Python `bool` which... The optional `delete_checkpoint_stream` argument is a
+Python `bool` which... The optional `timeout` argument is a Python `float`
+which sets a maximum duration, in seconds, for the completion of the gRPC
+operation. The optional `credentials` argument can be used to override call
+credentials derived from the connection string URI. ```python
+client.delete_projection(name=projection_name) ``` ### Restart projections
+subsystem The `restart_projections_subsystem()` method can be used to restart
+the projections subsystem. This method also has two optional arguments,
+`timeout` and `credentials`. The optional `timeout` argument is a Python
+`float` which sets a maximum duration, in seconds, for the completion of the
+gRPC operation. The optional `credentials` argument can be used to override
 call credentials derived from the connection string URI. ```python
 client.restart_projections_subsystem() ``` ## Call credentials Default call
 credentials are derived by the client from the user info part of the connection
 string URI. Many of the client methods described above have an optional
 `credentials` argument, which can be used to set call credentials for an
 individual method call that override those derived from the connection string
 URI. ### Construct call credentials The client method
```

### Comparing `esdbclient-1.1b1/esdbclient/__init__.py` & `esdbclient-1.1b2/esdbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/asyncio_client.py` & `esdbclient-1.1b2/esdbclient/asyncio_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1389,46 +1389,44 @@
         )
 
     @retrygrpc
     @autoreconnect
     async def create_projection(
         self,
         *,
+        name: str,
         query: str,
-        name: str = "",
-        continuous: bool = False,
         emit_enabled: bool = False,
         track_emitted_streams: bool = False,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         """
         Creates a projection.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         await self._connection.projections.create(
             query=query,
             name=name,
-            continuous=continuous,
             emit_enabled=emit_enabled,
             track_emitted_streams=track_emitted_streams,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     async def update_projection(
         self,
         name: str,
         *,
         query: str,
-        emit_enabled: Optional[bool] = None,
+        emit_enabled: bool = False,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         """
         Updates a projection.
         """
         timeout = timeout if timeout is not None else self._default_deadline
@@ -1465,65 +1463,30 @@
             delete_state_stream=delete_state_stream,
             delete_checkpoint_stream=delete_checkpoint_stream,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
-    @overload
-    async def get_projection_statistics(
-        self,
-        *,
-        name: str,
-        timeout: Optional[float] = None,
-        credentials: Optional[grpc.CallCredentials] = None,
-    ) -> ProjectionStatistics:
-        """
-        Signature for returning statistics for named projection.
-        """
-
-    @overload
-    async def get_projection_statistics(
-        self,
-        *,
-        all: bool = False,
-        transient: bool = False,
-        continuous: bool = False,
-        one_time: bool = False,
-        timeout: Optional[float] = None,
-        credentials: Optional[grpc.CallCredentials] = None,
-    ) -> Sequence[ProjectionStatistics]:
-        """
-        Signature for returning collection of projection statistics.
-        """
-
     @retrygrpc
     @autoreconnect
     async def get_projection_statistics(
         self,
         *,
-        name: Optional[str] = None,
-        all: bool = False,
-        transient: bool = False,
-        continuous: bool = False,
-        one_time: bool = False,
+        name: str,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
-    ) -> Union[ProjectionStatistics, Sequence[ProjectionStatistics]]:
+    ) -> ProjectionStatistics:
         """
         Gets projection statistics.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         return await self._connection.projections.get_projection_statistics(
             name=name,
-            all=all,
-            transient=transient,
-            continuous=continuous,
-            one_time=one_time,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
```

### Comparing `esdbclient-1.1b1/esdbclient/client.py` & `esdbclient-1.1b2/esdbclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1589,46 +1589,44 @@
         )
 
     @retrygrpc
     @autoreconnect
     def create_projection(
         self,
         *,
+        name: str,
         query: str,
-        name: str = "",
-        continuous: bool = False,
         emit_enabled: bool = False,
         track_emitted_streams: bool = False,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         """
         Creates a projection.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         self._esdb.projections.create(
             query=query,
             name=name,
-            continuous=continuous,
             emit_enabled=emit_enabled,
             track_emitted_streams=track_emitted_streams,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
     def update_projection(
         self,
         name: str,
         *,
         query: str,
-        emit_enabled: Optional[bool] = None,
+        emit_enabled: bool = False,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         """
         Updates a projection.
         """
         timeout = timeout if timeout is not None else self._default_deadline
@@ -1665,65 +1663,30 @@
             delete_state_stream=delete_state_stream,
             delete_checkpoint_stream=delete_checkpoint_stream,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
-    @overload
-    def get_projection_statistics(
-        self,
-        *,
-        name: str,
-        timeout: Optional[float] = None,
-        credentials: Optional[grpc.CallCredentials] = None,
-    ) -> ProjectionStatistics:
-        """
-        Signature for returning statistics for named projection.
-        """
-
-    @overload
-    def get_projection_statistics(
-        self,
-        *,
-        all: bool = False,
-        transient: bool = False,
-        continuous: bool = False,
-        one_time: bool = False,
-        timeout: Optional[float] = None,
-        credentials: Optional[grpc.CallCredentials] = None,
-    ) -> Sequence[ProjectionStatistics]:
-        """
-        Signature for returning collection of projection statistics.
-        """
-
     @retrygrpc
     @autoreconnect
     def get_projection_statistics(
         self,
         *,
-        name: Optional[str] = None,
-        all: bool = False,
-        transient: bool = False,
-        continuous: bool = False,
-        one_time: bool = False,
+        name: str,
         timeout: Optional[float] = None,
         credentials: Optional[grpc.CallCredentials] = None,
-    ) -> Union[ProjectionStatistics, Sequence[ProjectionStatistics]]:
+    ) -> ProjectionStatistics:
         """
         Gets projection statistics.
         """
         timeout = timeout if timeout is not None else self._default_deadline
 
         return self._esdb.projections.get_projection_statistics(
             name=name,
-            all=all,
-            transient=transient,
-            continuous=continuous,
-            one_time=one_time,
             timeout=timeout,
             metadata=self._call_metadata,
             credentials=credentials or self._call_credentials,
         )
 
     @retrygrpc
     @autoreconnect
```

### Comparing `esdbclient-1.1b1/esdbclient/common.py` & `esdbclient-1.1b2/esdbclient/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     FailedPrecondition,
     GrpcDeadlineExceeded,
     GrpcError,
     InternalError,
     MaximumSubscriptionsReached,
     NodeIsNotLeader,
     NotFound,
+    OperationFailed,
     ServiceUnavailable,
     SSLError,
     UnknownError,
 )
 from esdbclient.protos.Grpc import persistent_pb2, streams_pb2
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -181,14 +182,20 @@
                 return NotFound(e)
             elif (
                 "Envelope callback expected ProjectionResult, received NotFound instead"
                 in details
             ):
                 # Projections.Result does this....
                 return NotFound(e)
+            elif (
+                "Envelope callback expected Updated, received OperationFailed instead"
+                in details
+            ):
+                # Projections.Delete does this....
+                return OperationFailed(e)
             else:  # pragma: no cover
                 return UnknownError(e)
         elif e.code() == grpc.StatusCode.ABORTED:
             details = str(e.details())
             if isinstance(details, str) and "Consumer too slow" in details:
                 return ConsumerTooSlow()
             else:
@@ -323,14 +330,15 @@
             type=link.metadata.get("type", ""),
             data=link.data,
             metadata=link.custom_metadata,
             content_type=link.metadata.get("content-type", ""),
             stream_name=link.stream_identifier.stream_name.decode("utf8"),
             stream_position=link.stream_revision,
             commit_position=None if ignore_commit_position else link.commit_position,
+            prepare_position=None if ignore_commit_position else link.prepare_position,
             retry_count=retry_count,
             recorded_at=recorded_at,
         )
 
     try:
         recorded_at = datetime.datetime.fromtimestamp(
             int(event.metadata.get("created", "")) / 10000000.0,
@@ -344,12 +352,13 @@
         type=event.metadata.get("type", ""),
         data=event.data,
         metadata=event.custom_metadata,
         content_type=event.metadata.get("content-type", ""),
         stream_name=event.stream_identifier.stream_name.decode("utf8"),
         stream_position=event.stream_revision,
         commit_position=None if ignore_commit_position else event.commit_position,
+        prepare_position=None if ignore_commit_position else event.prepare_position,
         retry_count=retry_count,
         link=recorded_event_link,
         recorded_at=recorded_at,
     )
     return recorded_event
```

### Comparing `esdbclient-1.1b1/esdbclient/connection.py` & `esdbclient-1.1b2/esdbclient/connection.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/connection_spec.py` & `esdbclient-1.1b2/esdbclient/connection_spec.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/events.py` & `esdbclient-1.1b2/esdbclient/events.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     data: bytes
     metadata: bytes
     content_type: str
     id: UUID
     stream_name: str
     stream_position: int
     commit_position: Optional[int]
+    prepare_position: Optional[int]
     recorded_at: Optional[datetime] = None
     link: Optional["RecordedEvent"] = None
     retry_count: Optional[int] = None
 
     @property
     def ack_id(self) -> UUID:
         if self.link is not None:
@@ -75,24 +76,25 @@
     #     return False
 
 
 @dataclass(frozen=True)
 class Checkpoint(RecordedEvent):
     CHECKPOINT_ID = UUID("00000000-0000-0000-0000-000000000000")
 
-    def __init__(self, commit_position: int) -> None:
+    def __init__(self, commit_position: int, prepare_position: int) -> None:
         super().__init__(
             id=Checkpoint.CHECKPOINT_ID,
             type="",
             data=b"",
             content_type="",
             metadata=b"",
             stream_name="",
             stream_position=0,
             commit_position=commit_position,
+            prepare_position=prepare_position,
         )
 
     @property
     def is_checkpoint(self) -> bool:
         return True
 
 
@@ -106,14 +108,15 @@
             type="",
             data=b"",
             content_type="",
             metadata=b"",
             stream_name="",
             stream_position=0,
             commit_position=0,
+            prepare_position=0,
         )
 
     @property
     def is_caught_up(self) -> bool:
         return True
```

### Comparing `esdbclient-1.1b1/esdbclient/exceptions.py` & `esdbclient-1.1b2/esdbclient/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             return f"{host}:{port}"
         else:
             return None
 
 
 class NotFound(EventStoreDBClientException):
     """
-    Raised when stream or subscription is not found.
+    Raised when stream or subscription or projection is not found.
     """
 
 
 class AlreadyExists(EventStoreDBClientException):
     """
     Raised when creating something, e.g. a persistent subscription, that already exists.
     """
@@ -162,14 +162,20 @@
 
 class InvalidTransactionError(EventStoreDBClientException):
     """
     Raised when append operation fails with an "invalid transaction" error.
     """
 
 
+class OperationFailed(EventStoreDBClientException):
+    """
+    Raised when an operation fails (e.g. deleting a projection that isn't disabled).
+    """
+
+
 class MaximumAppendSizeExceededError(EventStoreDBClientException):
     """
     Raised when append operation fails with a "maximum append size exceeded" error.
     """
 
 
 class BadRequestError(EventStoreDBClientException):
```

### Comparing `esdbclient-1.1b1/esdbclient/gossip.py` & `esdbclient-1.1b2/esdbclient/gossip.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/persistent.py` & `esdbclient-1.1b2/esdbclient/persistent.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/projections.py` & `esdbclient-1.1b2/esdbclient/projections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 from dataclasses import dataclass
-from typing import Any, List, Optional, Sequence, Union
+from typing import Any, Optional, Union
 
 import grpc
 import grpc.aio
 from google.protobuf import struct_pb2
 
 from esdbclient.common import (
     AsyncGrpcStreamers,
     ESDBService,
     Metadata,
     SyncGrpcStreamers,
     TGrpcStreamers,
     handle_rpc_error,
 )
 from esdbclient.connection_spec import ConnectionSpec
+from esdbclient.exceptions import EventStoreDBClientException
 from esdbclient.protos.Grpc import projections_pb2, projections_pb2_grpc, shared_pb2
 
 
 @dataclass(frozen=True)
 class ProjectionStatistics:
     core_processing_time: int
     version: int
@@ -61,63 +62,40 @@
         super().__init__(connection_spec=connection_spec, grpc_streamers=grpc_streamers)
         self._stub = projections_pb2_grpc.ProjectionsStub(channel)
 
     @staticmethod
     def _construct_create_req(
         query: str,
         name: str,
-        continuous: bool,
         emit_enabled: bool,
         track_emitted_streams: bool,
     ) -> projections_pb2.CreateReq:
-        # Decide "mode".
-        if not name:
-            options = projections_pb2.CreateReq.Options(
-                one_time=shared_pb2.Empty(),
-                query=query,
-            )
-        elif not continuous:
-            options = projections_pb2.CreateReq.Options(
-                transient=projections_pb2.CreateReq.Options.Transient(
-                    name=name,
-                ),
-                query=query,
-            )
-        else:
-            options = projections_pb2.CreateReq.Options(
-                continuous=projections_pb2.CreateReq.Options.Continuous(
-                    name=name,
-                    emit_enabled=emit_enabled,
-                    track_emitted_streams=track_emitted_streams,
-                ),
-                query=query,
-            )
-
+        options = projections_pb2.CreateReq.Options(
+            continuous=projections_pb2.CreateReq.Options.Continuous(
+                name=name,
+                emit_enabled=emit_enabled,
+                track_emitted_streams=track_emitted_streams,
+            ),
+            query=query,
+        )
         return projections_pb2.CreateReq(options=options)
 
     @staticmethod
     def _construct_update_req(
         name: str,
         query: str,
-        emit_enabled: Optional[bool],
+        emit_enabled: bool,
     ) -> projections_pb2.UpdateReq:
-        # Decide "emit_option".
-        if emit_enabled is None:
-            options = projections_pb2.UpdateReq.Options(
-                name=name,
-                query=query,
-                no_emit_options=shared_pb2.Empty(),
-            )
-        else:
-            options = projections_pb2.UpdateReq.Options(
+        return projections_pb2.UpdateReq(
+            options=projections_pb2.UpdateReq.Options(
                 name=name,
                 query=query,
                 emit_enabled=emit_enabled,
             )
-        return projections_pb2.UpdateReq(options=options)
+        )
 
     @staticmethod
     def _construct_delete_req(
         name: str,
         delete_emitted_streams: bool,
         delete_state_stream: bool,
         delete_checkpoint_stream: bool,
@@ -129,39 +107,18 @@
                 delete_state_stream=delete_state_stream,
                 delete_checkpoint_stream=delete_checkpoint_stream,
             ),
         )
 
     @staticmethod
     def _construct_statistics_req(
-        name: Optional[str],
-        all: bool,
-        transient: bool,
-        continuous: bool,
-        one_time: bool,
+        name: str,
     ) -> projections_pb2.StatisticsReq:
-        # Decide "mode".
-        if name:
-            options = projections_pb2.StatisticsReq.Options(name=name)
-        # elif all:
-        #     options = projections_pb2.StatisticsReq.Options(all=shared_pb2.Empty())
-        elif transient:  # pragma: no cover
-            options = projections_pb2.StatisticsReq.Options(
-                transient=shared_pb2.Empty()
-            )
-        elif continuous:
-            options = projections_pb2.StatisticsReq.Options(
-                continuous=shared_pb2.Empty()
-            )
-        elif one_time:
-            options = projections_pb2.StatisticsReq.Options(one_time=shared_pb2.Empty())
-        else:
-            options = projections_pb2.StatisticsReq.Options(all=shared_pb2.Empty())
         return projections_pb2.StatisticsReq(
-            options=options,
+            options=projections_pb2.StatisticsReq.Options(name=name),
         )
 
     @staticmethod
     def _construct_disable_req(
         name: str,
         write_checkpoint: bool,
     ) -> projections_pb2.DisableReq:
@@ -279,25 +236,23 @@
 
 
 class AsyncioProjectionsService(BaseProjectionsService[AsyncGrpcStreamers]):
     async def create(
         self,
         query: str,
         name: str,
-        continuous: bool,
         emit_enabled: bool,
         track_emitted_streams: bool,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         create_req = self._construct_create_req(
             query=query,
             name=name,
-            continuous=continuous,
             emit_enabled=emit_enabled,
             track_emitted_streams=track_emitted_streams,
         )
         try:
             create_resp = await self._stub.Create(
                 create_req,
                 timeout=timeout,
@@ -308,15 +263,15 @@
             raise handle_rpc_error(e) from None
         assert isinstance(create_resp, projections_pb2.CreateResp)
 
     async def update(
         self,
         name: str,
         query: str,
-        emit_enabled: Optional[bool],
+        emit_enabled: bool,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         update_req = self._construct_update_req(
             name=name,
             query=query,
@@ -358,50 +313,39 @@
             )
         except grpc.RpcError as e:
             raise handle_rpc_error(e) from None
         assert isinstance(delete_resp, projections_pb2.DeleteResp)
 
     async def get_projection_statistics(
         self,
-        name: Optional[str],
-        all: bool,
-        transient: bool,
-        continuous: bool,
-        one_time: bool,
+        name: str,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
-    ) -> Union[ProjectionStatistics, Sequence[ProjectionStatistics]]:
-        statistics_req = self._construct_statistics_req(
-            name=name,
-            all=all,
-            transient=transient,
-            continuous=continuous,
-            one_time=one_time,
-        )
+    ) -> ProjectionStatistics:
+        statistics_req = self._construct_statistics_req(name=name)
         try:
             statistics_resps = self._stub.Statistics(
                 statistics_req,
                 timeout=timeout,
                 metadata=self._metadata(metadata, requires_leader=True),
                 credentials=credentials,
             )
-            projection_statistics_list: List[ProjectionStatistics] = []
             async for statistics_resp in statistics_resps:
                 assert isinstance(
                     statistics_resp, projections_pb2.StatisticsResp
                 ), statistics_resp
                 projection_statistics = self._construct_projection_statistics(
                     statistics_resp
                 )
-                if name is not None:
-                    return projection_statistics
-                else:  # pragma: no cover
-                    projection_statistics_list.append(projection_statistics)
-            return tuple(projection_statistics_list)  # pragma: no cover
+                return projection_statistics
+            else:  # pragma: no cover
+                raise EventStoreDBClientException(
+                    "Statistics request didn't return any statistics"
+                )
         except grpc.RpcError as e:
             raise handle_rpc_error(e) from None
 
     async def disable(
         self,
         name: str,
         write_checkpoint: bool,
@@ -541,25 +485,23 @@
     Encapsulates the 'gossip.Projections' gRPC service.
     """
 
     def create(
         self,
         query: str,
         name: str,
-        continuous: bool,
         emit_enabled: bool,
         track_emitted_streams: bool,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         create_req = self._construct_create_req(
             query=query,
             name=name,
-            continuous=continuous,
             emit_enabled=emit_enabled,
             track_emitted_streams=track_emitted_streams,
         )
         try:
             create_resp = self._stub.Create(
                 create_req,
                 timeout=timeout,
@@ -570,15 +512,15 @@
             raise handle_rpc_error(e) from None
         assert isinstance(create_resp, projections_pb2.CreateResp)
 
     def update(
         self,
         name: str,
         query: str,
-        emit_enabled: Optional[bool],
+        emit_enabled: bool,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
     ) -> None:
         update_req = self._construct_update_req(
             name=name,
             query=query,
@@ -620,50 +562,39 @@
             )
         except grpc.RpcError as e:
             raise handle_rpc_error(e) from None
         assert isinstance(delete_resp, projections_pb2.DeleteResp)
 
     def get_projection_statistics(
         self,
-        name: Optional[str],
-        all: bool,
-        transient: bool,
-        continuous: bool,
-        one_time: bool,
+        name: str,
         timeout: Optional[float] = None,
         metadata: Optional[Metadata] = None,
         credentials: Optional[grpc.CallCredentials] = None,
-    ) -> Union[ProjectionStatistics, Sequence[ProjectionStatistics]]:
-        statistics_req = self._construct_statistics_req(
-            name=name,
-            all=all,
-            transient=transient,
-            continuous=continuous,
-            one_time=one_time,
-        )
+    ) -> ProjectionStatistics:
+        statistics_req = self._construct_statistics_req(name=name)
         try:
             statistics_resps = self._stub.Statistics(
                 statistics_req,
                 timeout=timeout,
                 metadata=self._metadata(metadata, requires_leader=True),
                 credentials=credentials,
             )
-            projection_statistics_list: List[ProjectionStatistics] = []
             for statistics_resp in statistics_resps:
                 assert isinstance(
                     statistics_resp, projections_pb2.StatisticsResp
                 ), statistics_resp
                 projection_statistics = self._construct_projection_statistics(
                     statistics_resp
                 )
-                if name is not None:
-                    return projection_statistics
-                else:  # pragma: no cover
-                    projection_statistics_list.append(projection_statistics)
-            return tuple(projection_statistics_list)  # pragma: no cover
+                return projection_statistics
+            else:  # pragma: no cover
+                raise EventStoreDBClientException(
+                    "Statistics request didn't return any statistics"
+                )
         except grpc.RpcError as e:
             raise handle_rpc_error(e) from None
 
     def disable(
         self,
         name: str,
         write_checkpoint: bool,
```

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/cluster_pb2.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/cluster_pb2.pyi` & `esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/cluster_pb2_grpc.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/cluster_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/code_pb2.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/code_pb2.pyi` & `esdbclient-1.1b2/esdbclient/protos/Grpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/gossip_pb2.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/gossip_pb2.pyi` & `esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/gossip_pb2_grpc.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/gossip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/persistent_pb2.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/persistent_pb2.pyi` & `esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/persistent_pb2_grpc.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/persistent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/projections_pb2.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/projections_pb2.pyi` & `esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/projections_pb2_grpc.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/projections_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/shared_pb2.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/shared_pb2.pyi` & `esdbclient-1.1b2/esdbclient/protos/Grpc/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/status_pb2.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/status_pb2.pyi` & `esdbclient-1.1b2/esdbclient/protos/Grpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/streams_pb2.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/streams_pb2.pyi` & `esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2.pyi`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/protos/Grpc/streams_pb2_grpc.py` & `esdbclient-1.1b2/esdbclient/protos/Grpc/streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `esdbclient-1.1b1/esdbclient/streams.py` & `esdbclient-1.1b2/esdbclient/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
             raise NotFound(f"Stream {self._stream_name!r} not found")
         elif content_oneof == "event":
             return construct_recorded_event(read_resp.event)
         elif content_oneof == "checkpoint":
             checkpoint = read_resp.checkpoint
             return Checkpoint(
                 commit_position=checkpoint.commit_position,
+                prepare_position=checkpoint.prepare_position,
             )
         elif content_oneof == "caught_up":  # pragma: no cover
             return CaughtUp()
         # elif content_oneof == "fell_behind":  # pragma: no cover
         #     return FellBehind()
         else:  # pragma: no cover
             return None
```

### Comparing `esdbclient-1.1b1/pyproject.toml` & `esdbclient-1.1b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esdbclient"
-version = "1.1b1"
+version = "1.1b2"
 
 description = "Python gRPC Client for EventStoreDB"
 authors = [
     "John Bywater <john.bywater@appropriatesoftware.net>",
 ]
 license = "BSD 3-Clause"
 classifiers = [
```

### Comparing `esdbclient-1.1b1/PKG-INFO` & `esdbclient-1.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esdbclient
-Version: 1.1b1
+Version: 1.1b2
 Summary: Python gRPC Client for EventStoreDB
 Home-page: https://github.com/pyeventsourcing/esdbclient
 License: BSD 3-Clause
 Author: John Bywater
 Author-email: john.bywater@appropriatesoftware.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -265,18 +265,18 @@
   * [Replay parked events](#replay-parked-events)
   * [Get subscription info](#get-subscription-info)
   * [List subscriptions](#list-subscriptions)
   * [List subscriptions to stream](#list-subscriptions-to-stream)
   * [Delete subscription](#delete-subscription)
 * [Projections](#projections)
   * [Create projection](#create-projection)
-  * [Update projection](#update-projection)
-  * [Get projection statistics](#get-projection-statistics)
   * [Get projection state](#get-projection-state)
   * [Get projection result](#get-projection-result)
+  * [Get projection statistics](#get-projection-statistics)
+  * [Update projection](#update-projection)
   * [Enable projection](#enable-projection)
   * [Disable projection](#disable-projection)
   * [Reset projection](#reset-projection)
   * [Delete projection](#delete-projection)
   * [Restart projections subsystem](#restart-projections-subsystem)
 * [Call credentials](#call-credentials)
   * [Construct call credentials](#construct-call-credentials)
@@ -2856,52 +2856,58 @@
     stream_name=stream_name2,
 )
 ```
 
 
 ## Projections<a id="projections"></a>
 
+Please refer to the [EventStoreDB documentation](https://developers.eventstore.com/server/v23.10/projections.html)
+for more information on projections in EventStoreDB.
+
 ### Create projection<a id="create-projection"></a>
 
 The `create_projection()` method can be used to create a projection.
 
-This method has a required `query` argument, which is a Python `str` that
-defines what the projection will do.
+This method has two required arguments, `name` and `query`.
+
+This required `name` argument is a Python `str` that specifies the name of the projection.
 
-This method also has six optional arguments, `name`, `continuous`, `emit_enabled`,
-`track_emitted_streams`, `timeout`, and `credentials`.
+This required `query` argument is a Python `str` that defines what the projection will do.
 
-The optional `name` argument is a Python `str` which specifies the name of the projection.
-If a name is provided, the projection will either be a "transient" or a "continuous"
-projection. Otherwise, the projection will be a "one time" projection.
-
-The optional `continuous` argument is a Python `bool` which specifies whether a
-projection will be a "continuous" projection. If a `True` value is specified, the
-projection will be a "continuous" projection, otherwise the projection will be a
-"transient" projection. The default value of `continuous` is `False`.
+This method also has four optional arguments, `emit_enabled`,
+`track_emitted_streams`, `timeout`, and `credentials`.
 
 The optional `emit_enabled` argument is a Python `bool` which specifies whether a
 projection will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events, otherwise the projection will not be able to emit events.
 The default value of `emit_enabled` is `False`.
 
+Please note, if your projection query includes a call to `emit()` then `emit_enabled`
+must be `True`, otherwise the projection will not run.
+
 The optional `track_emitted_streams` argument is a Python `bool` which specifies whether
 a projection will have its emitted streams tracked. If a `True` value is specified, the
 projection will have its emitted streams tracked, otherwise the projection will not
 have its emitted streams tracked. The default value of `track_emitted_streams` is `False`.
 
+The purpose of tracking emitted streams is that they can optionally be deleted when
+a projection is deleted (see the `delete_projection()` method for more details).
+
+Please note, if you set `track_emitted_streams` to `True`, then you must also set
+`emit_enabled` to `True`, otherwise an error will be raised by this method.
+
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
-In the example below, a continuous projection is created that processes
-events appended to `stream_name2`. The "state" of the projection is
-initialised to have a "count" that is incremented once for each event.
+In the example below, a projection is created that processes events appended to
+`stream_name2`. The "state" of the projection is initialised to have a "count" that
+is incremented once for each event.
 
 ```python
 projection_name = str(uuid.uuid4())
 
 projection_query = """fromStream('%s')
 .when({
   $init: function(){
@@ -2921,18 +2927,25 @@
 })
 .outputState()
 """  % stream_name2
 
 client.create_projection(
     name=projection_name,
     query=projection_query,
-    continuous=True,
 )
 ```
 
+Please note, the `outputState()` call is optional, and causes the state of the
+projection to be persisted in a "result" stream. The default name of the result stream
+is `$projections-{projection_name}-result`, and this name can be used to read from and
+subscribe to the results stream with the `get_stream()`, `read_stream()`,
+`subscribe_stream()`, `create_subscription_to_stream()` and `read_subscription_to_stream()`
+methods.
+
+
 ### Get projection state<a id="get-projection-state"></a>
 
 The `get_projection_state()` method can be used to get a projection's state.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of a projection.
 
@@ -2963,15 +2976,15 @@
 The `get_projection_result()` method can be used to get a projection's result.
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of a projection.
 
 This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
 
-The optional `partition` argument is a Python `str` which specifies a partition...
+The optional `partition` argument is a Python `str` which specifies a partition.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -2984,40 +2997,30 @@
 assert projection_result.value == {'count': 3}
 ```
 
 ### Get projection statistics<a id="get-projection-statistics"></a>
 
 The `get_projection_statistucs()` method can be used to get projection statistics.
 
-This method also has seven optional arguments, `name`, `all`, `transient`,
-`continuous`, `one_time`, `timeout`, and `credentials`.
-
-The optional `name` argument is a Python `str` that specifies the name of a
-projection. If the name of a projection is specified, this method will return
-a single `ProjectionStatistics` object that represents that projection. Otherwise
-this method will return a sequence of `ProjectionStatistics` objects.
-
-The optional `all` argument is Python `bool` that can be used to request statistics
-for all projections.
+This method has a required `name` argument, which is a Python `str` that specifies the
+name of a projection.
 
-The optional `transient` argument is Python `bool` that can be used to request
-statistics for all "transient" projections.
-
-The optional `continuous` argument is Python `bool` that can be used to request
-statistics for all "continuous" projections.
+This method also has three optional arguments, `partition`, `timeout`, and `credentials`.
 
-The optional `one_time` argument is Python `bool` that can be used to request
-statistics for all "one time" projections.
+The optional `partition` argument is a Python `str` which specifies a partition.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
+This method returns a `ProjectionStatistics` object that represents
+the named projection.
+
 ```python
 statistics = client.get_projection_statistics(name=projection_name)
 ```
 
 A `ProjectionStatistics` object is returned. The attributes of this object
 have values that represent the progress of the projection.
 
@@ -3033,15 +3036,20 @@
 The required `query` argument is a Python `str` which defines what the projection will do.
 
 This method also has three optional arguments, `emit_enabled`, `timeout`, and `credentials`.
 
 The optional `emit_enabled` argument is a Python `bool` which specifies whether a
 projection will be able to emit events. If a `True` value is specified, the projection
 will be able to emit events. If a `False` value is specified, the projection will not
-be able to emit events. The default value of `emit_enabled` is `None`.
+be able to emit events. The default value of `emit_enabled` is `False`.
+
+Please note, if your projection query includes a call to `emit()` then `emit_enabled`
+must be `True`, otherwise the projection will not run.
+
+Please note, it is not possible to update `track_emitted_streams` via the gRPC API.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
 override call credentials derived from the connection string URI.
 
@@ -3051,15 +3059,15 @@
 
 ### Enable projection<a id="enable-projection"></a>
 
 The `enable_projection()` method can be used to enable a projection that was previously
 disabled.
 
 This method has a required `name` argument, which is a Python `str` that
-specifies the name of the projection to be disabled.
+specifies the name of the projection to be enabled.
 
 This method also has two optional arguments, `timeout` and `credentials`.
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
 
 The optional `credentials` argument can be used to
@@ -3123,15 +3131,18 @@
 
 This method has a required `name` argument, which is a Python `str` that
 specifies the name of the projection to be deleted.
 
 This method also has five optional arguments, `delete_emitted_streams`,
 `delete_state_stream`, `delete_checkpoint_stream`, `timeout`, and `credentials`.
 
-The optional `delete_emitted_streams` argument is a Python `bool` which...
+The optional `delete_emitted_streams` argument is a Python `bool` which specifies
+that the emitted streams will be deleted. For emitted streams to be deleted, they
+must have been tracked (see the `track_emitted_streams` argument of the `create_projection()`
+method.)
 
 The optional `delete_state_stream` argument is a Python `bool` which...
 
 The optional `delete_checkpoint_stream` argument is a Python `bool` which...
 
 The optional `timeout` argument is a Python `float` which sets a
 maximum duration, in seconds, for the completion of the gRPC operation.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: esdbclient Version: 1.1b1 Summary: Python gRPC
+Metadata-Version: 2.1 Name: esdbclient Version: 1.1b2 Summary: Python gRPC
 Client for EventStoreDB Home-page: https://github.com/pyeventsourcing/
 esdbclient License: BSD 3-Clause Author: John Bywater Author-email:
 john.bywater@appropriatesoftware.net Requires-Python: >=3.7,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: License :: OSI Approved :: BSD
 License Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
@@ -129,23 +129,23 @@
 consumer) * [Update subscription to all](#update-subscription-to-all) * [Create
 subscription to stream](#create-subscription-to-stream) * [Read subscription to
 stream](#read-subscription-to-stream) * [Update subscription to stream]
 (#update-subscription-to-stream) * [Replay parked events](#replay-parked-
 events) * [Get subscription info](#get-subscription-info) * [List
 subscriptions](#list-subscriptions) * [List subscriptions to stream](#list-
 subscriptions-to-stream) * [Delete subscription](#delete-subscription) *
-[Projections](#projections) * [Create projection](#create-projection) * [Update
-projection](#update-projection) * [Get projection statistics](#get-projection-
-statistics) * [Get projection state](#get-projection-state) * [Get projection
-result](#get-projection-result) * [Enable projection](#enable-projection) *
-[Disable projection](#disable-projection) * [Reset projection](#reset-
-projection) * [Delete projection](#delete-projection) * [Restart projections
-subsystem](#restart-projections-subsystem) * [Call credentials](#call-
-credentials) * [Construct call credentials](#construct-call-credentials) *
-[Connection](#connection) * [Reconnect](#reconnect) * [Close](#close) *
+[Projections](#projections) * [Create projection](#create-projection) * [Get
+projection state](#get-projection-state) * [Get projection result](#get-
+projection-result) * [Get projection statistics](#get-projection-statistics) *
+[Update projection](#update-projection) * [Enable projection](#enable-
+projection) * [Disable projection](#disable-projection) * [Reset projection]
+(#reset-projection) * [Delete projection](#delete-projection) * [Restart
+projections subsystem](#restart-projections-subsystem) * [Call credentials]
+(#call-credentials) * [Construct call credentials](#construct-call-credentials)
+* [Connection](#connection) * [Reconnect](#reconnect) * [Close](#close) *
 [Asyncio client](#asyncio-client) * [Synopsis](#synopsis-1) * [Notes](#notes) *
 [Regular expression filters](#regular-expression-filters) * [Reconnect and
 retry method decorators](#reconnect-and-retry-method-decorators) *
 [Contributors](#contributors) * [Install Poetry](#install-poetry) * [Setup for
 PyCharm users](#setup-for-pycharm-users) * [Setup from command line](#setup-
 from-command-line) * [Project Makefile commands](#project-makefile-commands) ##
 Install package It is recommended to install Python packages into a Python
@@ -1504,115 +1504,119 @@
 `credentials` argument, which can be used to override call credentials derived
 from the connection string URI. The example below deletes the persistent
 subscription `group_name1` which was created by calling
 `create_subscription_to_all()`. ```python client.delete_subscription
 ( group_name=group_name1, ) ``` The example below deleted the persistent
 subscription `group_name2` on `stream_name2` which was created by calling
 `create_subscription_to_stream()`. ```python client.delete_subscription
-( group_name=group_name2, stream_name=stream_name2, ) ``` ## Projections ###
-Create projection The `create_projection()` method can be used to create a
-projection. This method has a required `query` argument, which is a Python
-`str` that defines what the projection will do. This method also has six
-optional arguments, `name`, `continuous`, `emit_enabled`,
-`track_emitted_streams`, `timeout`, and `credentials`. The optional `name`
-argument is a Python `str` which specifies the name of the projection. If a
-name is provided, the projection will either be a "transient" or a "continuous"
-projection. Otherwise, the projection will be a "one time" projection. The
-optional `continuous` argument is a Python `bool` which specifies whether a
-projection will be a "continuous" projection. If a `True` value is specified,
-the projection will be a "continuous" projection, otherwise the projection will
-be a "transient" projection. The default value of `continuous` is `False`. The
-optional `emit_enabled` argument is a Python `bool` which specifies whether a
-projection will be able to emit events. If a `True` value is specified, the
-projection will be able to emit events, otherwise the projection will not be
-able to emit events. The default value of `emit_enabled` is `False`. The
+( group_name=group_name2, stream_name=stream_name2, ) ``` ## Projections Please
+refer to the [EventStoreDB documentation](https://developers.eventstore.com/
+server/v23.10/projections.html) for more information on projections in
+EventStoreDB. ### Create projection The `create_projection()` method can be
+used to create a projection. This method has two required arguments, `name` and
+`query`. This required `name` argument is a Python `str` that specifies the
+name of the projection. This required `query` argument is a Python `str` that
+defines what the projection will do. This method also has four optional
+arguments, `emit_enabled`, `track_emitted_streams`, `timeout`, and
+`credentials`. The optional `emit_enabled` argument is a Python `bool` which
+specifies whether a projection will be able to emit events. If a `True` value
+is specified, the projection will be able to emit events, otherwise the
+projection will not be able to emit events. The default value of `emit_enabled`
+is `False`. Please note, if your projection query includes a call to `emit()`
+then `emit_enabled` must be `True`, otherwise the projection will not run. The
 optional `track_emitted_streams` argument is a Python `bool` which specifies
 whether a projection will have its emitted streams tracked. If a `True` value
 is specified, the projection will have its emitted streams tracked, otherwise
 the projection will not have its emitted streams tracked. The default value of
-`track_emitted_streams` is `False`. The optional `timeout` argument is a Python
-`float` which sets a maximum duration, in seconds, for the completion of the
-gRPC operation. The optional `credentials` argument can be used to override
-call credentials derived from the connection string URI. In the example below,
-a continuous projection is created that processes events appended to
-`stream_name2`. The "state" of the projection is initialised to have a "count"
-that is incremented once for each event. ```python projection_name = str
-(uuid.uuid4()) projection_query = """fromStream('%s') .when({ $init: function()
-{ return { count: 0 }; }, OrderCreated: function(s,e){ s.count += 1; },
-OrderUpdated: function(s,e){ s.count += 1; }, OrderDeleted: function(s,e)
-{ s.count += 1; } }) .outputState() """ % stream_name2 client.create_projection
-( name=projection_name, query=projection_query, continuous=True, ) ``` ### Get
-projection state The `get_projection_state()` method can be used to get a
-projection's state. This method has a required `name` argument, which is a
-Python `str` that specifies the name of a projection. This method also has
-three optional arguments, `partition`, `timeout`, and `credentials`. The
-optional `partition` argument is a Python `str` which specifies a partition...
-The optional `timeout` argument is a Python `float` which sets a maximum
-duration, in seconds, for the completion of the gRPC operation. The optional
-`credentials` argument can be used to override call credentials derived from
-the connection string URI. In the example below, after sleeping for 1 second to
-allow the projection to process all the recorded events, the projection "state"
-is obtained. We can see that the projection has processed three events.
-```python sleep(1) # allow time for projection to process recorded events
-projection_state = client.get_projection_state(name=projection_name) assert
-projection_state.value == {'count': 3} ``` ### Get projection result The
-`get_projection_result()` method can be used to get a projection's result. This
+`track_emitted_streams` is `False`. The purpose of tracking emitted streams is
+that they can optionally be deleted when a projection is deleted (see the
+`delete_projection()` method for more details). Please note, if you set
+`track_emitted_streams` to `True`, then you must also set `emit_enabled` to
+`True`, otherwise an error will be raised by this method. The optional
+`timeout` argument is a Python `float` which sets a maximum duration, in
+seconds, for the completion of the gRPC operation. The optional `credentials`
+argument can be used to override call credentials derived from the connection
+string URI. In the example below, a projection is created that processes events
+appended to `stream_name2`. The "state" of the projection is initialised to
+have a "count" that is incremented once for each event. ```python
+projection_name = str(uuid.uuid4()) projection_query = """fromStream('%s')
+.when({ $init: function(){ return { count: 0 }; }, OrderCreated: function(s,e)
+{ s.count += 1; }, OrderUpdated: function(s,e){ s.count += 1; }, OrderDeleted:
+function(s,e){ s.count += 1; } }) .outputState() """ % stream_name2
+client.create_projection( name=projection_name, query=projection_query, ) ```
+Please note, the `outputState()` call is optional, and causes the state of the
+projection to be persisted in a "result" stream. The default name of the result
+stream is `$projections-{projection_name}-result`, and this name can be used to
+read from and subscribe to the results stream with the `get_stream()`,
+`read_stream()`, `subscribe_stream()`, `create_subscription_to_stream()` and
+`read_subscription_to_stream()` methods. ### Get projection state The
+`get_projection_state()` method can be used to get a projection's state. This
 method has a required `name` argument, which is a Python `str` that specifies
 the name of a projection. This method also has three optional arguments,
 `partition`, `timeout`, and `credentials`. The optional `partition` argument is
 a Python `str` which specifies a partition... The optional `timeout` argument
 is a Python `float` which sets a maximum duration, in seconds, for the
 completion of the gRPC operation. The optional `credentials` argument can be
 used to override call credentials derived from the connection string URI. In
-the example below, the projection "result" is obtained. We can see that the
-projection has processed three events. ```python projection_result =
+the example below, after sleeping for 1 second to allow the projection to
+process all the recorded events, the projection "state" is obtained. We can see
+that the projection has processed three events. ```python sleep(1) # allow time
+for projection to process recorded events projection_state =
+client.get_projection_state(name=projection_name) assert projection_state.value
+== {'count': 3} ``` ### Get projection result The `get_projection_result()`
+method can be used to get a projection's result. This method has a required
+`name` argument, which is a Python `str` that specifies the name of a
+projection. This method also has three optional arguments, `partition`,
+`timeout`, and `credentials`. The optional `partition` argument is a Python
+`str` which specifies a partition. The optional `timeout` argument is a Python
+`float` which sets a maximum duration, in seconds, for the completion of the
+gRPC operation. The optional `credentials` argument can be used to override
+call credentials derived from the connection string URI. In the example below,
+the projection "result" is obtained. We can see that the projection has
+processed three events. ```python projection_result =
 client.get_projection_result(name=projection_name) assert
 projection_result.value == {'count': 3} ``` ### Get projection statistics The
 `get_projection_statistucs()` method can be used to get projection statistics.
-This method also has seven optional arguments, `name`, `all`, `transient`,
-`continuous`, `one_time`, `timeout`, and `credentials`. The optional `name`
-argument is a Python `str` that specifies the name of a projection. If the name
-of a projection is specified, this method will return a single
-`ProjectionStatistics` object that represents that projection. Otherwise this
-method will return a sequence of `ProjectionStatistics` objects. The optional
-`all` argument is Python `bool` that can be used to request statistics for all
-projections. The optional `transient` argument is Python `bool` that can be
-used to request statistics for all "transient" projections. The optional
-`continuous` argument is Python `bool` that can be used to request statistics
-for all "continuous" projections. The optional `one_time` argument is Python
-`bool` that can be used to request statistics for all "one time" projections.
+This method has a required `name` argument, which is a Python `str` that
+specifies the name of a projection. This method also has three optional
+arguments, `partition`, `timeout`, and `credentials`. The optional `partition`
+argument is a Python `str` which specifies a partition. The optional `timeout`
+argument is a Python `float` which sets a maximum duration, in seconds, for the
+completion of the gRPC operation. The optional `credentials` argument can be
+used to override call credentials derived from the connection string URI. This
+method returns a `ProjectionStatistics` object that represents the named
+projection. ```python statistics = client.get_projection_statistics
+(name=projection_name) ``` A `ProjectionStatistics` object is returned. The
+attributes of this object have values that represent the progress of the
+projection. ### Update projection The `update_projection()` method can be used
+to update a projection. This method has two required arguments, `name` and
+`query`. The required `name` argument is a Python `str` which specifies the
+name of the projection to be updated. The required `query` argument is a Python
+`str` which defines what the projection will do. This method also has three
+optional arguments, `emit_enabled`, `timeout`, and `credentials`. The optional
+`emit_enabled` argument is a Python `bool` which specifies whether a projection
+will be able to emit events. If a `True` value is specified, the projection
+will be able to emit events. If a `False` value is specified, the projection
+will not be able to emit events. The default value of `emit_enabled` is
+`False`. Please note, if your projection query includes a call to `emit()` then
+`emit_enabled` must be `True`, otherwise the projection will not run. Please
+note, it is not possible to update `track_emitted_streams` via the gRPC API.
 The optional `timeout` argument is a Python `float` which sets a maximum
 duration, in seconds, for the completion of the gRPC operation. The optional
 `credentials` argument can be used to override call credentials derived from
-the connection string URI. ```python statistics =
-client.get_projection_statistics(name=projection_name) ``` A
-`ProjectionStatistics` object is returned. The attributes of this object have
-values that represent the progress of the projection. ### Update projection The
-`update_projection()` method can be used to update a projection. This method
-has two required arguments, `name` and `query`. The required `name` argument is
-a Python `str` which specifies the name of the projection to be updated. The
-required `query` argument is a Python `str` which defines what the projection
-will do. This method also has three optional arguments, `emit_enabled`,
-`timeout`, and `credentials`. The optional `emit_enabled` argument is a Python
-`bool` which specifies whether a projection will be able to emit events. If a
-`True` value is specified, the projection will be able to emit events. If a
-`False` value is specified, the projection will not be able to emit events. The
-default value of `emit_enabled` is `None`. The optional `timeout` argument is a
-Python `float` which sets a maximum duration, in seconds, for the completion of
-the gRPC operation. The optional `credentials` argument can be used to override
-call credentials derived from the connection string URI. ```python
-client.update_projection(name=projection_name, query=projection_query) ``` ###
-Enable projection The `enable_projection()` method can be used to enable a
-projection that was previously disabled. This method has a required `name`
-argument, which is a Python `str` that specifies the name of the projection to
-be disabled. This method also has two optional arguments, `timeout` and
-`credentials`. The optional `timeout` argument is a Python `float` which sets a
-maximum duration, in seconds, for the completion of the gRPC operation. The
-optional `credentials` argument can be used to override call credentials
-derived from the connection string URI. ```python client.enable_projection
+the connection string URI. ```python client.update_projection
+(name=projection_name, query=projection_query) ``` ### Enable projection The
+`enable_projection()` method can be used to enable a projection that was
+previously disabled. This method has a required `name` argument, which is a
+Python `str` that specifies the name of the projection to be enabled. This
+method also has two optional arguments, `timeout` and `credentials`. The
+optional `timeout` argument is a Python `float` which sets a maximum duration,
+in seconds, for the completion of the gRPC operation. The optional
+`credentials` argument can be used to override call credentials derived from
+the connection string URI. ```python client.enable_projection
 (name=projection_name) ``` ### Disable projection The `disable_projection()`
 method can be used to disable a projection. This method has a required `name`
 argument, which is a Python `str` that specifies the name of the projection to
 be disabled. This method also has three optional arguments, `write_checkpoint`,
 `timeout`, and `credentials`. The optional `write_checkpoint` argument is a
 Python `bool` which specifies whether a checkpoint will be written when the
 projection is disabled. If `write_checkpoint` is `True` a checkpoint will be
@@ -1635,26 +1639,29 @@
 argument can be used to override call credentials derived from the connection
 string URI. ```python client.reset_projection(name=projection_name) ``` ###
 Delete projection The `delete_projection()` method can be used to delete a
 projection. This method has a required `name` argument, which is a Python `str`
 that specifies the name of the projection to be deleted. This method also has
 five optional arguments, `delete_emitted_streams`, `delete_state_stream`,
 `delete_checkpoint_stream`, `timeout`, and `credentials`. The optional
-`delete_emitted_streams` argument is a Python `bool` which... The optional
-`delete_state_stream` argument is a Python `bool` which... The optional
-`delete_checkpoint_stream` argument is a Python `bool` which... The optional
-`timeout` argument is a Python `float` which sets a maximum duration, in
-seconds, for the completion of the gRPC operation. The optional `credentials`
-argument can be used to override call credentials derived from the connection
-string URI. ```python client.delete_projection(name=projection_name) ``` ###
-Restart projections subsystem The `restart_projections_subsystem()` method can
-be used to restart the projections subsystem. This method also has two optional
-arguments, `timeout` and `credentials`. The optional `timeout` argument is a
-Python `float` which sets a maximum duration, in seconds, for the completion of
-the gRPC operation. The optional `credentials` argument can be used to override
+`delete_emitted_streams` argument is a Python `bool` which specifies that the
+emitted streams will be deleted. For emitted streams to be deleted, they must
+have been tracked (see the `track_emitted_streams` argument of the
+`create_projection()` method.) The optional `delete_state_stream` argument is a
+Python `bool` which... The optional `delete_checkpoint_stream` argument is a
+Python `bool` which... The optional `timeout` argument is a Python `float`
+which sets a maximum duration, in seconds, for the completion of the gRPC
+operation. The optional `credentials` argument can be used to override call
+credentials derived from the connection string URI. ```python
+client.delete_projection(name=projection_name) ``` ### Restart projections
+subsystem The `restart_projections_subsystem()` method can be used to restart
+the projections subsystem. This method also has two optional arguments,
+`timeout` and `credentials`. The optional `timeout` argument is a Python
+`float` which sets a maximum duration, in seconds, for the completion of the
+gRPC operation. The optional `credentials` argument can be used to override
 call credentials derived from the connection string URI. ```python
 client.restart_projections_subsystem() ``` ## Call credentials Default call
 credentials are derived by the client from the user info part of the connection
 string URI. Many of the client methods described above have an optional
 `credentials` argument, which can be used to set call credentials for an
 individual method call that override those derived from the connection string
 URI. ### Construct call credentials The client method
```


# Comparing `tmp/era_5g_relay_network_application-1.4.0.tar.gz` & `tmp/era_5g_relay_network_application-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_relay_network_application-1.4.0.tar", last modified: Mon Apr 29 08:58:11 2024, max compression
+gzip compressed data, was "era_5g_relay_network_application-1.5.0.tar", last modified: Thu May  9 08:57:30 2024, max compression
```

## Comparing `era_5g_relay_network_application-1.4.0.tar` & `era_5g_relay_network_application-1.5.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/MANIFEST.in
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      431 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/PKG-INFO
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/backend_shim.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.473980 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      353 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    16864 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/client.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2128 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/point_cloud_msg_conv.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2028 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/rosbridge_action_loader.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/data/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/data/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/py.typed
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    19727 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/server.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5643 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/utils.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1402 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_clock.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1374 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_image_publisher.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3401 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_image_subscriber.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5741 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_publisher.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6841 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_service.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4654 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_service_server.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1537 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_socketio.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1087 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_socketio_server.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6609 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_subscriber.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1213 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_tf.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.473980 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      431 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/PKG-INFO
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     1390 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      150 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/requires.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       33 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/top_level.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/setup.cfg
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1224 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-09 08:57:30.602085 era_5g_relay_network_application-1.5.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      431 2024-05-09 08:57:30.598086 era_5g_relay_network_application-1.5.0/PKG-INFO
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/backend_shim.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-09 08:57:30.590086 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      904 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    17227 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/client.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-09 08:57:30.598086 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/compatibility/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/compatibility/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2128 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/compatibility/point_cloud_msg_conv.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2028 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/compatibility/rosbridge_action_loader.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-09 08:57:30.598086 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/data/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/data/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1696 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/data/service.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4588 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/data/topic.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/py.typed
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    14793 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/server.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5643 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/utils.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1402 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_clock.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1168 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_commands.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1374 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_image_publisher.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3592 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_image_subscriber.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5715 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_publisher.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6841 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_service.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4654 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_service_server.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1537 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_socketio.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1313 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_socketio_server.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6916 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_subscriber.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1262 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_tf.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-05-09 08:57:30.594086 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      431 2024-05-09 08:57:30.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     1538 2024-05-09 08:57:30.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-05-09 08:57:30.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-05-09 08:57:30.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      150 2024-05-09 08:57:30.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       33 2024-05-09 08:57:30.000000 era_5g_relay_network_application-1.5.0/era_5g_relay_network_application.egg-info/top_level.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-05-09 08:57:30.602085 era_5g_relay_network_application-1.5.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1224 2024-05-09 08:57:29.000000 era_5g_relay_network_application-1.5.0/setup.py
```

### Comparing `era_5g_relay_network_application-1.4.0/backend_shim.py` & `era_5g_relay_network_application-1.5.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/client.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from rclpy.qos import QoSHistoryPolicy, QoSProfile, QoSReliabilityPolicy  # pants: no-infer-dep
 
 from era_5g_client.client import NetAppClient
 from era_5g_client.client_base import NetAppClientBase
 from era_5g_client.dataclasses import MiddlewareInfo
 from era_5g_client.exceptions import FailedToConnect
 from era_5g_interface.channels import CallbackInfoClient, Channels, ChannelType
-from era_5g_relay_network_application import SendFunctionProtocol
+from era_5g_relay_network_application import SendFunctionProtocol, can_be_dropped_from_qos, queue_len_from_qos
 from era_5g_relay_network_application.utils import (
     IMAGE_CHANNEL_TYPES,
     ActionServiceVariant,
     ActionTopicVariant,
     EntityConfig,
     get_channel_type,
     load_entities_list,
@@ -64,15 +64,14 @@
 # middleware robot id (robot id)
 MIDDLEWARE_ROBOT_ID = os.getenv("MIDDLEWARE_ROBOT_ID", "00000000-0000-0000-0000-000000000000")
 
 
 USE_SIM_TIME = os.getenv("USE_SIM_TIME", "false").lower() in ("true", "1", "t")
 
 QUEUE_LENGTH_TOPICS = int(os.getenv("QUEUE_LENGTH_TOPICS", 1))
-QUEUE_LENGTH_SERVICES = int(os.getenv("QUEUE_LENGTH_SERVICES", 1))
 QUEUE_LENGTH_TF = int(os.getenv("QUEUE_LENGTH_TF", 1))
 
 EXTENDED_MEASURING = bool(os.getenv("EXTENDED_MEASURING", False))
 
 bridge = CvBridge()
 client: Optional[NetAppClientBase] = None
 
@@ -94,47 +93,53 @@
     """Executed when new JSON data is received from the relay server.
 
     Args:
         data (Dict[str, Any]): JSON data received from the relay server.
         queue (Queue):  The queue to pass the data to the publisher.
     """
 
+    assert node
+
     try:
         queue.put_nowait((data, Channels.get_timestamp_from_data(data)))
     except Full:
-        return
+        node.get_logger().warning("client: JSON queue full!")
 
 
 def image_callback(data: Dict[str, Any], queue: Queue):
     """Executed when new image data is received from the relay server.
 
     Args:
         data (Dict[str, Any]): The image data received from the relay server in the format {"frame": <image_data>,
             "timestamp": <timestamp>}.
         queue (Queue): The queue to pass the data to the publisher.
     """
 
+    assert node
+
     try:
         queue.put_nowait((data["frame"], data["timestamp"]))
     except Full:
-        return
+        node.get_logger().warning("client: image queue full!")
 
 
 def service_callback(data: Dict[str, Any], response_queue: Queue):
     """Executed when new service response is received from the relay server.
 
     Args:
         data (Dict[str, Any]): Service response received from the relay server.
         response_queue (Queue): The queue to pass the data to the service server.
     """
 
+    assert node
+
     try:
         response_queue.put_nowait(data)
     except Full:
-        return
+        node.get_logger().warning("client: service response queue full!")
 
 
 def send_image(data: Tuple, event: str, client: NetAppClientBase, channel_type: ChannelType, can_be_dropped=False):
     """Sends image data to the relay server.
 
     Args:
         data (Tuple): The image data in the format (timestamp, image_data).
@@ -156,16 +161,16 @@
     qos: Optional[QoSProfile] = None,
     action_service_variant: ActionServiceVariant = ActionServiceVariant.NONE,
 ):
     """Create a service server to listen to local service calls."""
 
     global services_workers
 
-    request_q: Queue = Queue(QUEUE_LENGTH_SERVICES)
-    response_q: Queue = Queue(QUEUE_LENGTH_SERVICES)
+    request_q: Queue = Queue(1)
+    response_q: Queue = Queue(1)
     service_worker = WorkerServiceServer(
         service_name, service_type, request_q, response_q, node, qos, action_service_variant
     )
     services_workers[service_worker.service_name] = service_worker
 
     # The service is bidirectional, so we need to create callback for the response from the relay server
     callback = partial(
@@ -262,15 +267,15 @@
             "The relay network application should be already deployed. I will try to connect with following settings:"
         )
         logger.info(f"{NETAPP_ADDRESS=}")
 
     callbacks_info = dict()
     # Create publishers and collect callbacks info for all topics to be received from the relay server
     for topic_in in topics_incoming_list:
-        queue: Queue = Queue(QUEUE_LENGTH_TOPICS)
+        queue: Queue = Queue(queue_len_from_qos(QUEUE_LENGTH_TOPICS, topic_in.qos))
         channel_type = get_channel_type(topic_in.compression, topic_in.type)
         worker: WorkerPublisher
         if channel_type in IMAGE_CHANNEL_TYPES:
             callback = partial(
                 image_callback,
                 queue=queue,
             )
@@ -337,45 +342,51 @@
             )
             worker_clock = WorkerClock(send_function_clock, node)
             worker_clock.daemon = True
             worker_clock.start()
 
         # create socketio workers for all topics and services to be sent to the relay server
         for topic_out in topics_outgoing_list:
-            subscriber_queue: Queue = Queue(QUEUE_LENGTH_TOPICS)
+            subscriber_queue: Queue = Queue(queue_len_from_qos(QUEUE_LENGTH_TOPICS, topic_out.qos))
             channel_type = get_channel_type(topic_out.compression, topic_out.type)
             w: Union[WorkerImageSubscriber, WorkerSubscriber]
+
+            can_be_dropped = can_be_dropped_from_qos(topic_out.qos)
+
             if channel_type in IMAGE_CHANNEL_TYPES:
                 w = WorkerImageSubscriber(
                     topic_out.name,
                     topic_out.type,
                     node,
                     subscriber_queue,
                     topic_out.qos,
                     extended_measuring=EXTENDED_MEASURING,
                 )
                 send_function: SendFunctionProtocol = partial(
                     send_image,
                     event=f"topic/{topic_out.name}",
                     client=client,
                     channel_type=channel_type,
-                    can_be_dropped=True,
+                    can_be_dropped=can_be_dropped,
                 )
             else:
                 w = WorkerSubscriber(
                     topic_out.name,
                     topic_out.type,
                     node,
                     subscriber_queue,
                     topic_out.compression,
                     topic_out.qos,
                     extended_measuring=EXTENDED_MEASURING,
                 )
                 send_function: SendFunctionProtocol = partial(  # type: ignore  # deals with "name already defined"
-                    client.send_data, event=f"topic/{topic_out.name}", channel_type=channel_type, can_be_dropped=True
+                    client.send_data,
+                    event=f"topic/{topic_out.name}",
+                    channel_type=channel_type,
+                    can_be_dropped=can_be_dropped,
                 )
 
             if w.memory is not None:
                 for msg in w.memory:
                     send_function(msg)
             worker_socketio = WorkerSocketIO(subscriber_queue, send_function)
             worker_socketio.daemon = True
```

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/point_cloud_msg_conv.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/compatibility/point_cloud_msg_conv.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/rosbridge_action_loader.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/compatibility/rosbridge_action_loader.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/server.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,60 @@
 import logging
 import os
 import sys
 import threading
 from functools import partial
 from multiprocessing import Queue
 from queue import Full
-from typing import Any, Dict, Optional, Tuple, Union
+from typing import Any, Dict, Optional, Tuple
 
 import rclpy  # pants: no-infer-dep
 from rclpy.parameter import Parameter  # pants: no-infer-dep
-from rclpy.qos import QoSProfile  # pants: no-infer-dep
 
 from era_5g_interface.channels import CallbackInfoServer, Channels, ChannelType
 from era_5g_interface.dataclasses.control_command import ControlCmdType, ControlCommand
 from era_5g_interface.utils.locked_set import LockedSet
+from era_5g_relay_network_application import can_be_dropped_from_qos
+from era_5g_relay_network_application.data.service import RelayService
+from era_5g_relay_network_application.data.topic import RelayTopicIncoming, RelayTopicOutgoing
 from era_5g_relay_network_application.utils import (
     IMAGE_CHANNEL_TYPES,
     ActionServiceVariant,
     ActionSubscribers,
     ActionTopicVariant,
-    Compressions,
     EntityConfig,
     get_channel_type,
     load_entities_list,
     load_transform_list,
 )
-from era_5g_relay_network_application.worker_image_publisher import WorkerImagePublisher
-from era_5g_relay_network_application.worker_image_subscriber import WorkerImageSubscriber
-from era_5g_relay_network_application.worker_publisher import WorkerPublisher
-from era_5g_relay_network_application.worker_service import ServiceData, WorkerService
+from era_5g_relay_network_application.worker_commands import WorkerCommands
 from era_5g_relay_network_application.worker_socketio import WorkerSocketIO
 from era_5g_relay_network_application.worker_socketio_server import WorkerSocketIOServer
-from era_5g_relay_network_application.worker_subscriber import WorkerSubscriber
 from era_5g_relay_network_application.worker_tf import WorkerTF
 from era_5g_server.server import NetworkApplicationServer
 
 logging.basicConfig(stream=sys.stdout, level=logging.INFO)
 logger = logging.getLogger("relay server python")
 
 # port of the netapp's server
 NETAPP_PORT = int(os.getenv("NETAPP_PORT", 5896))
 
-QUEUE_LENGTH_TOPICS = int(os.getenv("QUEUE_LENGTH_TOPICS", 1))
-QUEUE_LENGTH_SERVICES = int(os.getenv("QUEUE_LENGTH_SERVICES", 1))
 QUEUE_LENGTH_TF = int(os.getenv("QUEUE_LENGTH_TF", 1))
 USE_SIM_TIME = os.getenv("USE_SIM_TIME", "false").lower() in ("true", "1", "t")
 EXTENDED_MEASURING = bool(os.getenv("EXTENDED_MEASURING", False))
 
 
-class RelayTopic:
-    """Base class that holds information about topic and its type."""
-
-    def __init__(
-        self,
-        topic_name: str,
-        topic_type: str,
-        channel_type: ChannelType,
-        compression: Optional[Compressions] = None,
-        qos: Optional[QoSProfile] = None,
-    ):
-        self.topic_name = topic_name
-        self.topic_type = topic_type
-        self.compression = compression
-        self.qos = qos
-        self.channel_type = channel_type
-        self.channel_name = f"topic/{self.topic_name}"
-        self.queue: Queue[Any] = Queue(QUEUE_LENGTH_TOPICS)
-
-
-class RelayTopicIncoming(RelayTopic):
-    """Class that holds information about incoming topic (i.e. topic that is received from the relay client and is
-    published here), its type and related publisher."""
-
-    def __init__(
-        self,
-        topic_name: str,
-        topic_type: str,
-        channel_type: ChannelType,
-        node,
-        compression: Optional[Compressions] = None,
-        qos: Optional[QoSProfile] = None,
-    ):
-        super().__init__(topic_name, topic_type, channel_type, compression, qos)
-
-        # this sucks, the classes should have some common ancestor or there should be two properties
-        self.worker: Union[WorkerImagePublisher, WorkerPublisher]
-
-        if self.channel_type in IMAGE_CHANNEL_TYPES:
-            self.worker = WorkerImagePublisher(
-                self.queue,
-                self.topic_name,
-                self.topic_type,
-                compression=compression,
-                node=node,
-                extended_measuring=EXTENDED_MEASURING,
-            )
-        else:
-            self.worker = WorkerPublisher(
-                self.queue,
-                self.topic_name,
-                self.topic_type,
-                node,
-                self.compression,
-                self.qos,
-                extended_measuring=EXTENDED_MEASURING,
-            )
-        self.worker.daemon = True
-        self.worker.start()
-
-
-class RelayTopicOutgoing(RelayTopic):
-    """Class that holds information about outgoing topic (i.e. topic that is subscribed to be sent to the relay client),
-    its type and related subscriber."""
-
-    def __init__(
-        self,
-        topic_name: str,
-        topic_type: str,
-        channel_type: ChannelType,
-        node: rclpy.node.Node,
-        compression: Optional[Compressions] = None,
-        qos: Optional[QoSProfile] = None,
-        action_topic_variant: ActionTopicVariant = ActionTopicVariant.NONE,
-        action_subscribers: Optional[ActionSubscribers] = None,
-    ):
-        super().__init__(topic_name, topic_type, channel_type, compression, qos)
-
-        self.action_topic_variant = action_topic_variant
-
-        # this sucks, the classes should have some common ancestor or there should be two properties
-        self.worker: Union[WorkerImageSubscriber, WorkerSubscriber]
-
-        if self.channel_type in IMAGE_CHANNEL_TYPES:
-            self.worker = WorkerImageSubscriber(
-                topic_name, topic_type, node, self.queue, extended_measuring=EXTENDED_MEASURING
-            )
-        else:
-            self.worker = WorkerSubscriber(
-                topic_name,
-                topic_type,
-                node,
-                self.queue,
-                compression,
-                qos,
-                action_topic_variant,
-                action_subscribers,
-                extended_measuring=EXTENDED_MEASURING,
-            )
-            # Topic name may be changed in case of action-related topics
-            self.channel_name = f"topic/{self.worker.topic_name}"
-            self.topic_name = self.worker.topic_name
-
-
-class RelayService:
-    """Class that holds information about incoming service (i.e. service that is called from relay client), its type and
-    related worker."""
-
-    def __init__(
-        self,
-        service_name: str,
-        service_type: str,
-        node: rclpy.node.Node,
-        qos: Optional[QoSProfile] = None,
-        action_service_variant: ActionServiceVariant = ActionServiceVariant.NONE,
-        action_subscribers: Optional[ActionSubscribers] = None,
-    ):
-        self.service_type = service_type
-
-        self.queue_request: Queue[ServiceData] = Queue(QUEUE_LENGTH_SERVICES)
-        self.queue_response: Queue[ServiceData] = Queue(QUEUE_LENGTH_SERVICES)
-
-        self.worker = WorkerService(
-            service_name,
-            service_type,
-            self.queue_request,
-            self.queue_response,
-            node,
-            qos,
-            action_service_variant,
-            action_subscribers,
-        )
-
-        # Service name can be changed by worker in case of action-related services
-        self.service_name = self.worker.service_name
-        self.channel_name_request = f"service_request/{self.service_name}"
-        self.channel_name_response = f"service_response/{self.service_name}"
-
-        self.worker.daemon = True
-        self.worker.start()
-
-
 class RelayServer(NetworkApplicationServer):
     def __init__(
         self,
         port: int,
         topics_incoming: Dict[str, RelayTopicIncoming],  # topics that are received from the relay client
         topics_outgoing: Dict[str, RelayTopicOutgoing],  # topics that are subscribed to be sent to the relay client
         services_incoming: Dict[str, RelayService],
+        command_queue: Queue,
         *args,
         tf_queue: Optional[Queue] = None,
         host: str = "0.0.0.0",
         **kwargs,
     ) -> None:
         self.callbacks_info: Dict[str, CallbackInfoServer] = dict()
         self.workers_outgoing: Dict[str, WorkerSocketIO] = dict()
@@ -236,42 +90,44 @@
 
         # callback_info needs to be passed to the parent class
         super().__init__(port, self.callbacks_info, *args, command_callback=self.command_callback, host=host, **kwargs)
         self.result_subscribers = LockedSet()  # contains data namespace SIDs of clients that want to receive results
 
         # collects info about topics that are subscribed to be sent to the relay client
         for topic_out in topics_outgoing.values():
+            can_be_dropped = can_be_dropped_from_qos(topic_out.qos)
+
             if topic_out.channel_type in [ChannelType.JSON, ChannelType.JSON_LZ4]:
                 send_function = partial(
                     self.send_data,
                     event=topic_out.channel_name,
                     channel_type=topic_out.channel_type,
-                    can_be_dropped=True,
+                    can_be_dropped=can_be_dropped,
                 )
             else:
                 send_function = partial(
                     self.send_image_data,
                     event=topic_out.channel_name,
                     channel_type=topic_out.channel_type,
-                    can_be_dropped=True,
+                    can_be_dropped=can_be_dropped,
                 )
 
             if topic_out.action_topic_variant == ActionTopicVariant.ACTION_FEEDBACK:
                 # Action feedback is not sent to everyone, but to a specific sid
                 send_function = partial(self.send_data_with_sid, event=topic_out.channel_name)
                 worker = WorkerSocketIO(topic_out.queue, send_function)
             else:
                 worker = WorkerSocketIOServer(topic_out.queue, self.result_subscribers, send_function)
 
             self.workers_outgoing[topic_out.topic_name] = worker
 
         if tf_queue:
             send_function = partial(self.send_data, event="topic//tf")
             self.workers_outgoing["/tf"] = WorkerSocketIOServer(tf_queue, self.result_subscribers, send_function)
-
+        self.command_queue = command_queue
         self.topics_outgoing = topics_outgoing
         self.topics_incoming = topics_incoming
 
     def send_data_with_sid(self, data: Tuple[str, Dict], event: str) -> None:
         """Sends response to the relay client.
 
         This is intended mainly for sending service response and action feedback.
@@ -312,65 +168,62 @@
             data (Dict[str, Any]): The image data in format {"frame": <image_data>, "timestamp": <timestamp>}.
             queue (Queue): The queue to pass the data to the publisher worker.
         """
 
         try:
             queue.put_nowait((data["frame"], data["timestamp"]))
         except Full:
-            pass
+            logger.warning("image queue full")
 
     def json_callback(self, sid: str, data: Dict, queue: Queue):
         """Allows to receive json data using the websocket transport.
 
         Args:
             sid (str): Data namespace SID of the client that sent the data.
             data (Dict): The json data.
             queue (Queue): The queue to pass the data to the publisher worker.
         """
         try:
             queue.put_nowait((data, Channels.get_timestamp_from_data(data)))
         except Full:
-            pass
+            logger.warning("JSON queue full")
 
     def service_callback(self, sid: str, data: Dict, queue: Queue):
         """Allows to receive service request using the websocket transport.
 
         Args:
             sid (str): Data namespace SID of the client that sent the data.
             data (Dict): The service request.
             queue (Queue): The queue to pass the data to the service worker.
         """
 
         try:
             queue.put_nowait((sid, data))
         except Full:
-            pass
+            logger.warning("service queue full")
 
     def command_callback(self, command: ControlCommand, sid: str) -> Tuple[bool, str]:
         """Processes the received control command.
 
         Args:
             command (ControlCommand): The control command.
             sid (str): Control namespace SID of the client that sent the command.
 
         Returns:
             Tuple[bool, str]: Confirmation that the command was processed.
         """
-
         if command and command.cmd_type == ControlCmdType.INIT:
             args = command.data
             if args:
                 sr = args.get("subscribe_results")
                 if sr:
                     sid = self.get_sid_of_data(self.get_eio_sid_of_control(sid))
                     self.result_subscribers.add(sid)
-                    for topic_out in self.topics_outgoing.values():
-                        if topic_out.worker.memory is not None:
-                            for msg in topic_out.worker.memory:
-                                self.send_data_with_sid((sid, msg), topic_out.channel_name)
+                    # notify all worker subscribers so they send cached messages to the newly connected client
+                    self.command_queue.put_nowait((sid, command))
         return True, ""
 
     def disconnect_callback(self, eio_sid):
         """Removes the client from the list of result subscribers."""
         self.result_subscribers.discard(eio_sid)
 
 
@@ -463,22 +316,27 @@
 
     # create worker for TFs
     tf_queue: Optional[Queue] = None
     if transforms_to_listen:
         tf_queue = Queue(QUEUE_LENGTH_TF)
         WorkerTF(transforms_to_listen, tf_queue, node)
 
+    command_queue: Queue = Queue(10)
+    worker_command = WorkerCommands(command_queue, topics_outgoing)
+    worker_command.daemon = True
+    worker_command.start()
     # create relay server
     socketio_process = RelayServer(
         NETAPP_PORT,
         topics_incoming,
         topics_outgoing,
         services_incoming,
         tf_queue=tf_queue,
         extended_measuring=EXTENDED_MEASURING,
+        command_queue=command_queue,
     )
 
     # TODO: An exception in callbacks of executor nodes does not terminate the application!
     #  This should be fixed!
 
     socketio_process.start()
     socketio_process.join()
```

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/utils.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/utils.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_clock.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_clock.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_image_publisher.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_image_publisher.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_image_subscriber.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_image_subscriber.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,21 +72,24 @@
                 "before_callback_timestamp": 0,
                 "after_callback_timestamp": 0,
             },
             enabled=self._extended_measuring,
             filename_prefix="subscription-" + self.topic_name.replace("/", ""),
         )
 
+    def flush_memory(self, sid: str) -> None:
+        pass  # TODO: implement latch support for images as well
+
     def callback(self, data: Any):
         before_callback_timestamp = time.perf_counter_ns()
         cv_image: Image = self.bridge.imgmsg_to_cv2(data, desired_encoding="bgr8")
         if cv_image is None:
             print("Empty image received!")
             return
         timestamp = Time.from_msg(data.header.stamp).nanoseconds
         try:
             self.queue.put_nowait((timestamp, cv_image))
         except Full:
-            pass
+            self.node.get_logger().warning(f"{self.topic_name} worker image subs: queue full!")
         self._measuring.log_measuring(timestamp, "before_callback_timestamp", before_callback_timestamp)
         self._measuring.log_timestamp(timestamp, "after_callback_timestamp")
         self._measuring.store_measuring(timestamp)
```

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_publisher.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             self.topic_name = f"{action_name}/_action/status"
             self.topic_type_class = action_type_class.Impl.GoalStatusMessage
 
             assert qos is None, "QoS should not be set for action status"
 
             # Status topic must have different qos profile
             # This is necessary for action to be recognized as being available by wait_for_server() call
-            qos = QoSProfile(durability=QoSDurabilityPolicy.RMW_QOS_POLICY_DURABILITY_TRANSIENT_LOCAL, depth=10)
+            qos = QoSProfile(durability=QoSDurabilityPolicy.TRANSIENT_LOCAL, depth=10)
 
         # Create publisher
         self.pub = node.create_publisher(self.topic_type_class, self.topic_name, qos if qos is not None else 10)
 
         self._extended_measuring = extended_measuring
         self._measuring = Measuring(
             measuring_items={
```

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_service.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_service.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_service_server.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_service_server.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_socketio.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_socketio.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_socketio_server.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_socketio_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 
     def __init__(self, queue: Queue, subscribers, send_function: Optional[SendFunctionProtocol], **kw):
         super().__init__(queue, send_function, **kw)
         self.subscribers = subscribers
 
     def send_data(self, data: Any):
         assert self.send_function
-
-        for s in self.subscribers:
-            try:
-                self.send_function(data, sid=s)
-            except BackPressureException:
-                logging.warning("Backpressure applied.")
-            except BadNamespaceError:
-                logging.warning("Trying to send data while not connected to the network application")
+        if isinstance(data, tuple):  # if the data is tupple, it contains the sid of the intended receiver
+            sid, msg = data
+            self.send_function(data=msg, sid=sid)
+        else:
+            for s in self.subscribers:
+                try:
+                    self.send_function(data, sid=s)
+                except BackPressureException:
+                    logging.warning("Backpressure applied.")
+                except BadNamespaceError:
+                    logging.warning("Trying to send data while not connected to the network application")
```

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_subscriber.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_subscriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,21 @@
                 "before_callback_timestamp": 0,
                 "after_callback_timestamp": 0,
             },
             enabled=self._extended_measuring,
             filename_prefix="subscription-" + self.topic_name.replace("/", ""),
         )
 
-    def callback(self, data: Any):
+    def flush_memory(self, sid: str) -> None:
+        """Send the content of the cache to the client with defined sid."""
+        if self.memory:
+            for msg in self.memory:
+                self.queue.put_nowait((sid, msg))
+
+    def callback(self, data: Any) -> None:
         before_callback_timestamp = time.perf_counter_ns()
 
         msg = extract_values(data)
         timestamp = Channels.get_timestamp_from_data(msg)
 
         if isinstance(data, PointCloud2) and self.compression == Compressions.DRACO:
             np_arr = read_points_numpy(data, field_names=["x", "y", "z"], skip_nans=True)  # drop intensity, etc....
@@ -143,11 +149,12 @@
                 self.queue.put_nowait((sid, msg))
             else:
                 if self.memory is not None:
                     self.memory.append(msg)
                 self.queue.put_nowait(msg)
 
         except Full:
-            pass
+            self.node.get_logger().debug(f"{self.topic_name} worker: full queue")
+
         self._measuring.log_measuring(timestamp, "before_callback_timestamp", before_callback_timestamp)
         self._measuring.log_timestamp(timestamp, "after_callback_timestamp")
         self._measuring.store_measuring(timestamp)
```

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_tf.py` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application/worker_tf.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,8 +25,8 @@
             tf_republisher.subscribe_transform(*tr)
 
     def tf_callback(self, transforms: List[TransformStamped]) -> None:
         if transforms:
             try:
                 self.queue.put_nowait(extract_values(TFMessage(transforms=transforms)))
             except Full:
-                pass
+                self.node.get_logger().debug("TF worker: full queue")
```

### Comparing `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/SOURCES.txt` & `era_5g_relay_network_application-1.5.0/era_5g_relay_network_application.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 era_5g_relay_network_application/__init__.py
 era_5g_relay_network_application/client.py
 era_5g_relay_network_application/py.typed
 era_5g_relay_network_application/server.py
 era_5g_relay_network_application/utils.py
 era_5g_relay_network_application/worker_clock.py
+era_5g_relay_network_application/worker_commands.py
 era_5g_relay_network_application/worker_image_publisher.py
 era_5g_relay_network_application/worker_image_subscriber.py
 era_5g_relay_network_application/worker_publisher.py
 era_5g_relay_network_application/worker_service.py
 era_5g_relay_network_application/worker_service_server.py
 era_5g_relay_network_application/worker_socketio.py
 era_5g_relay_network_application/worker_socketio_server.py
@@ -21,8 +22,10 @@
 era_5g_relay_network_application.egg-info/dependency_links.txt
 era_5g_relay_network_application.egg-info/namespace_packages.txt
 era_5g_relay_network_application.egg-info/requires.txt
 era_5g_relay_network_application.egg-info/top_level.txt
 era_5g_relay_network_application/compatibility/__init__.py
 era_5g_relay_network_application/compatibility/point_cloud_msg_conv.py
 era_5g_relay_network_application/compatibility/rosbridge_action_loader.py
-era_5g_relay_network_application/data/__init__.py
+era_5g_relay_network_application/data/__init__.py
+era_5g_relay_network_application/data/service.py
+era_5g_relay_network_application/data/topic.py
```

### Comparing `era_5g_relay_network_application-1.4.0/setup.py` & `era_5g_relay_network_application-1.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,9 +34,9 @@
     },
     'packages': (
         'era_5g_relay_network_application',
         'era_5g_relay_network_application.compatibility',
         'era_5g_relay_network_application.data',
     ),
     'python_requires': '>=3.8',
-    'version': '1.4.0',
+    'version': '1.5.0',
 })
```


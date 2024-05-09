# Comparing `tmp/dm_aiomqtt-0.4.7.tar.gz` & `tmp/dm_aiomqtt-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm_aiomqtt-0.4.7.tar", last modified: Tue Apr 23 07:35:53 2024, max compression
+gzip compressed data, was "dm_aiomqtt-0.4.8.tar", last modified: Thu May  9 18:04:25 2024, max compression
```

## Comparing `dm_aiomqtt-0.4.7.tar` & `dm_aiomqtt-0.4.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-23 07:35:42.000000 dm_aiomqtt-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/dm_aiomqtt/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 07:35:42.000000 dm_aiomqtt-0.4.7/dm_aiomqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-23 07:35:42.000000 dm_aiomqtt-0.4.7/dm_aiomqtt/dm_aiomqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-23 07:35:42.000000 dm_aiomqtt-0.4.7/dm_aiomqtt/message_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 07:35:53.833395 dm_aiomqtt-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-23 07:35:53.000000 dm_aiomqtt-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:04:25.486096 dm_aiomqtt-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-09 18:04:25.486096 dm_aiomqtt-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-09 18:04:17.000000 dm_aiomqtt-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:04:25.482096 dm_aiomqtt-0.4.8/dm_aiomqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 18:04:17.000000 dm_aiomqtt-0.4.8/dm_aiomqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-05-09 18:04:17.000000 dm_aiomqtt-0.4.8/dm_aiomqtt/dm_aiomqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-09 18:04:17.000000 dm_aiomqtt-0.4.8/dm_aiomqtt/message_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:04:25.482096 dm_aiomqtt-0.4.8/dm_aiomqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-09 18:04:25.000000 dm_aiomqtt-0.4.8/dm_aiomqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 18:04:25.000000 dm_aiomqtt-0.4.8/dm_aiomqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:04:25.000000 dm_aiomqtt-0.4.8/dm_aiomqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 18:04:25.000000 dm_aiomqtt-0.4.8/dm_aiomqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 18:04:25.000000 dm_aiomqtt-0.4.8/dm_aiomqtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:04:25.486096 dm_aiomqtt-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-09 18:04:25.000000 dm_aiomqtt-0.4.8/setup.py
```

### Comparing `dm_aiomqtt-0.4.7/PKG-INFO` & `dm_aiomqtt-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.7
+Version: 0.4.8
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dm_aiomqtt-0.4.7/README.md` & `dm_aiomqtt-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `dm_aiomqtt-0.4.7/dm_aiomqtt/dm_aiomqtt_client.py` & `dm_aiomqtt-0.4.8/dm_aiomqtt/dm_aiomqtt_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,39 +16,55 @@
         https://github.com/DIMKA4621/dm-aiomqtt
     """
     _SUBSCRIBE_CALLBACK_TYPE = Callable[["DMAioMqttClient.publish", str, str], Coroutine]
     _TEMP_CALLBACK_TYPE = Callable[["DMAioMqttClient.publish"], Coroutine]
     _LOG_FN_TYPE = Callable[[str], None]
     _QOS_TYPE = Literal[0, 1, 2]
 
+    __protocol_versions = {3: aiomqtt.ProtocolVersion.V31,
+                           4: aiomqtt.ProtocolVersion.V311,
+                           5: aiomqtt.ProtocolVersion.V5}
+    __default_version = 4
     __logger = None
 
     def __init__(
         self,
         host: str,
         port: int,
         username: str = "",
         password: str = "",
+        version: int = 4,  # 3 => v3.1;  4 => v3.1.1;  5 => v5
         ca_crt: str = "",
         client_crt: str = "",
         client_key: str = "",
         keepalive: int = 5,
         identifier: str = None,
-        clean_session: bool = True,
+        clean_session: Optional[bool] = None,  # not supported for v5 (for v5 by default => CLEAN_START=FIRST_ONLY)
         resend_not_success_messages: bool = False
     ) -> None:
         if self.__logger is None:
             self.__logger = DMLogger(f"DMAioMqttClient-{host}:{port}")
 
         self.__mqtt_config = {
             "hostname": host,
             "port": port,
             "keepalive": keepalive,
             "clean_session": clean_session
         }
+        if version not in self.__protocol_versions:
+            default_protocol = self.__protocol_versions[self.__default_version]
+            self.__mqtt_config["protocol"] = default_protocol
+            self.__logger.warning(f"Invalid protocol version: '{version}'! "
+                                  f"Used default version: {self.__default_version} ({default_protocol})")
+        else:
+            self.__mqtt_config["protocol"] = self.__protocol_versions[version]
+
+        if self.__mqtt_config["protocol"] == aiomqtt.ProtocolVersion.V5:
+            self.__mqtt_config["clean_session"] = None
+
         if identifier:
             self.__mqtt_config["identifier"] = identifier
         if username or password:
             self.__mqtt_config["username"] = username
             self.__mqtt_config["password"] = password
         self.__mqtt_config["tls_context"] = self.__get_tls_context(ca_crt, client_crt, client_key)
 
@@ -103,15 +119,15 @@
             async def test_topic_handler(publish: DMAioMqttClient.publish, topic: str, payload: str) -> None:
                print(f"Received message from {topic}: {payload}")
                publish("test/success", payload=True)
         """
         new_item = {"cb": callback, "qos": qos}
         self.__subscribes[topic] = new_item
 
-        if re.search(r"[+#]", topic):
+        if re.search(r"[+#$]", topic):
             self.__pattern_subscribes[topic] = new_item
 
     def publish(
         self,
         topic: str,
         payload: Union[str, int, float, dict, list, bool, None],
         qos: _QOS_TYPE = 0,
@@ -150,14 +166,16 @@
         messages = await self.__message_db.get_all()
         for topic, payload, qos in messages:
             self.publish(topic, payload, qos)
 
     def __get_callbacks_from_pattern_subscribes(self, current_topic: str) -> List[Callable]:
         callbacks = []
         for topic, params in self.__pattern_subscribes.items():
+            if topic[0] == "$":
+                topic = "/".join(topic.split("/")[2:])
             pattern = topic.replace("+", "[^/]+?")
             pattern = pattern.replace("/#", "(/.+)*")
             if re.search(pattern, current_topic):
                 callbacks.append(params["cb"])
         return callbacks
 
     async def __subscribe(self) -> None:
```

### Comparing `dm_aiomqtt-0.4.7/dm_aiomqtt/message_db.py` & `dm_aiomqtt-0.4.8/dm_aiomqtt/message_db.py`

 * *Files identical despite different names*

### Comparing `dm_aiomqtt-0.4.7/dm_aiomqtt.egg-info/PKG-INFO` & `dm_aiomqtt-0.4.8/dm_aiomqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-aiomqtt
-Version: 0.4.7
+Version: 0.4.8
 Summary: This is my custom aiomqtt client
 Home-page: https://pypi.org/project/dm-aiomqtt
 Author: dimka4621
 Author-email: mismartconfig@gmail.com
 Project-URL: GitHub, https://github.com/DIMKA4621/dm-aiomqtt
 Keywords: dm aiomqtt
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dm_aiomqtt-0.4.7/setup.py` & `dm_aiomqtt-0.4.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='dm-aiomqtt',
-    version='v0.4.7',
+    version='v0.4.8',
     author='dimka4621',
     author_email='mismartconfig@gmail.com',
     description='This is my custom aiomqtt client',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://pypi.org/project/dm-aiomqtt',
     packages=find_packages(),
```


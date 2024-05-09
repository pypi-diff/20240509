# Comparing `tmp/datalogd-0.3.7.tar.gz` & `tmp/datalogd-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalogd-0.3.7.tar", last modified: Wed Mar 29 05:56:19 2023, max compression
+gzip compressed data, was "datalogd-0.4.0.tar", last modified: Thu May  9 01:45:50 2024, max compression
```

## Comparing `datalogd-0.3.7.tar` & `datalogd-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,48 @@
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-03-29 05:56:19.418148 datalogd-0.3.7/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1059 2022-09-21 01:44:17.000000 datalogd-0.3.7/LICENSE.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3655 2023-03-29 05:56:19.414815 datalogd-0.3.7/PKG-INFO
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3025 2023-03-29 05:33:48.000000 datalogd-0.3.7/README.rst
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-03-29 05:56:19.414815 datalogd-0.3.7/datalogd/
--rw-r--r--   0 patrick   (1000) patrick   (1000)    16514 2023-03-29 04:40:48.000000 datalogd-0.3.7/datalogd/__init__.py
--rwxr-xr-x   0 patrick   (1000) patrick   (1000)       82 2022-09-21 01:44:17.000000 datalogd-0.3.7/datalogd/__main__.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-03-29 05:56:19.414815 datalogd-0.3.7/datalogd/plugins/
--rw-r--r--   0 patrick   (1000) patrick   (1000)      460 2022-09-21 01:44:17.000000 datalogd-0.3.7/datalogd/plugins/__init__.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3482 2022-09-21 01:44:17.000000 datalogd-0.3.7/datalogd/plugins/aggregator_datafilter.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     5436 2023-03-23 02:24:23.000000 datalogd-0.3.7/datalogd/plugins/coolingpower_datafilter.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2897 2022-11-17 04:09:23.000000 datalogd-0.3.7/datalogd/plugins/csv_datafilter.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4820 2022-10-10 07:23:33.000000 datalogd-0.3.7/datalogd/plugins/file_datasink.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3214 2022-11-17 04:09:23.000000 datalogd-0.3.7/datalogd/plugins/flowsensorcalibration_datafilter.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     9702 2022-10-21 00:59:38.000000 datalogd-0.3.7/datalogd/plugins/influxdb2_datasink.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4478 2022-10-10 07:17:07.000000 datalogd-0.3.7/datalogd/plugins/influxdb_datasink.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)      864 2022-09-21 01:44:17.000000 datalogd-0.3.7/datalogd/plugins/join_datafilter.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2947 2022-10-10 07:44:49.000000 datalogd-0.3.7/datalogd/plugins/keyval_datafilter.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3871 2022-10-21 01:05:53.000000 datalogd-0.3.7/datalogd/plugins/libsensors_datasource.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1181 2022-09-21 01:44:17.000000 datalogd-0.3.7/datalogd/plugins/logging_datasink.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2220 2022-10-06 05:19:15.000000 datalogd-0.3.7/datalogd/plugins/matplotlib_datasink.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    10598 2023-02-22 01:49:37.000000 datalogd-0.3.7/datalogd/plugins/picotc08_datasource.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     4953 2022-10-17 06:23:05.000000 datalogd-0.3.7/datalogd/plugins/polynomialfunction_datafilter.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)      745 2022-09-21 01:44:17.000000 datalogd-0.3.7/datalogd/plugins/print_datasink.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    12976 2023-01-04 03:35:06.000000 datalogd-0.3.7/datalogd/plugins/pyqtgraph_datasink.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     2133 2022-10-06 05:10:41.000000 datalogd-0.3.7/datalogd/plugins/randomwalk_datasource.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     8172 2023-02-21 08:09:43.000000 datalogd-0.3.7/datalogd/plugins/serial_datasource.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)    11078 2023-03-29 05:52:46.000000 datalogd-0.3.7/datalogd/plugins/socket_datafilter.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     7436 2023-03-29 03:08:20.000000 datalogd-0.3.7/datalogd/plugins/thorlabspm100_datasource.py
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1029 2022-09-21 01:44:17.000000 datalogd-0.3.7/datalogd/plugins/timestamp_datafilter.py
-drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2023-03-29 05:56:19.414815 datalogd-0.3.7/datalogd.egg-info/
--rw-r--r--   0 patrick   (1000) patrick   (1000)     3655 2023-03-29 05:56:19.000000 datalogd-0.3.7/datalogd.egg-info/PKG-INFO
--rw-r--r--   0 patrick   (1000) patrick   (1000)     1142 2023-03-29 05:56:19.000000 datalogd-0.3.7/datalogd.egg-info/SOURCES.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)        1 2023-03-29 05:56:19.000000 datalogd-0.3.7/datalogd.egg-info/dependency_links.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       43 2023-03-29 05:56:19.000000 datalogd-0.3.7/datalogd.egg-info/entry_points.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       24 2023-03-29 05:56:19.000000 datalogd-0.3.7/datalogd.egg-info/requires.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)        9 2023-03-29 05:56:19.000000 datalogd-0.3.7/datalogd.egg-info/top_level.txt
--rw-r--r--   0 patrick   (1000) patrick   (1000)       38 2023-03-29 05:56:19.418148 datalogd-0.3.7/setup.cfg
--rwxr-xr-x   0 patrick   (1000) patrick   (1000)     5825 2023-03-29 05:56:11.000000 datalogd-0.3.7/setup.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-09 01:45:50.166521 datalogd-0.4.0/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1059 2022-09-21 01:44:17.000000 datalogd-0.4.0/LICENSE.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3715 2024-05-09 01:45:50.166521 datalogd-0.4.0/PKG-INFO
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2995 2023-03-29 06:42:26.000000 datalogd-0.4.0/README.rst
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-09 01:45:50.163187 datalogd-0.4.0/datalogd/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    16517 2024-05-09 01:37:45.000000 datalogd-0.4.0/datalogd/__init__.py
+-rwxr-xr-x   0 patrick   (1000) patrick   (1000)       82 2022-09-21 01:44:17.000000 datalogd-0.4.0/datalogd/__main__.py
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-09 01:45:50.166521 datalogd-0.4.0/datalogd/plugins/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)      460 2022-09-21 01:44:17.000000 datalogd-0.4.0/datalogd/plugins/__init__.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3482 2022-09-21 01:44:17.000000 datalogd-0.4.0/datalogd/plugins/aggregator_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     5436 2023-03-23 02:24:23.000000 datalogd-0.4.0/datalogd/plugins/coolingpower_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2897 2022-11-17 04:09:23.000000 datalogd-0.4.0/datalogd/plugins/csv_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     4820 2022-10-10 07:23:33.000000 datalogd-0.4.0/datalogd/plugins/file_datasink.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3215 2024-05-09 01:35:05.000000 datalogd-0.4.0/datalogd/plugins/flowsensorcalibration_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2163 2023-08-01 07:13:02.000000 datalogd-0.4.0/datalogd/plugins/heartbeat_datasource.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     9947 2024-05-09 01:23:34.000000 datalogd-0.4.0/datalogd/plugins/influxdb2_datasink.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     4493 2023-06-05 05:08:01.000000 datalogd-0.4.0/datalogd/plugins/influxdb_datasink.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)      864 2022-09-21 01:44:17.000000 datalogd-0.4.0/datalogd/plugins/join_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2947 2022-10-10 07:44:49.000000 datalogd-0.4.0/datalogd/plugins/keyval_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3886 2023-06-05 05:08:01.000000 datalogd-0.4.0/datalogd/plugins/libsensors_datasource.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1181 2022-09-21 01:44:17.000000 datalogd-0.4.0/datalogd/plugins/logging_datasink.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1458 2023-06-26 05:08:45.000000 datalogd-0.4.0/datalogd/plugins/logwidget.ui
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2235 2023-06-05 05:08:01.000000 datalogd-0.4.0/datalogd/plugins/matplotlib_datasink.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    12519 2023-06-05 05:08:01.000000 datalogd-0.4.0/datalogd/plugins/picotc08_datasource.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     5560 2024-05-09 01:35:04.000000 datalogd-0.4.0/datalogd/plugins/polynomialfunction_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)      745 2022-09-21 01:44:17.000000 datalogd-0.4.0/datalogd/plugins/print_datasink.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    13129 2023-06-05 05:09:30.000000 datalogd-0.4.0/datalogd/plugins/pyqtgraph_datasink.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2133 2022-10-06 05:10:41.000000 datalogd-0.4.0/datalogd/plugins/randomwalk_datasource.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    37126 2023-07-04 07:41:34.000000 datalogd-0.4.0/datalogd/plugins/resources_rc.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    14283 2024-05-09 01:23:34.000000 datalogd-0.4.0/datalogd/plugins/sensoridentifierdatafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    25730 2024-05-09 01:23:34.000000 datalogd-0.4.0/datalogd/plugins/sensorpaneldatafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3676 2023-08-04 00:36:00.000000 datalogd-0.4.0/datalogd/plugins/sensorpaneldatafilter_demo.ui
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     8034 2023-06-05 05:09:30.000000 datalogd-0.4.0/datalogd/plugins/sensorwidget.ui
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    14132 2024-05-09 01:23:34.000000 datalogd-0.4.0/datalogd/plugins/serial_datasource.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1552 2024-05-09 01:23:34.000000 datalogd-0.4.0/datalogd/plugins/sinktimer_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)    11260 2024-05-09 01:35:04.000000 datalogd-0.4.0/datalogd/plugins/socket_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     9688 2024-05-09 01:23:34.000000 datalogd-0.4.0/datalogd/plugins/thorlabspm100_datasource.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1030 2024-05-09 01:35:03.000000 datalogd-0.4.0/datalogd/plugins/timestamp_datafilter.py
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     2470 2023-06-05 05:09:30.000000 datalogd-0.4.0/datalogd/plugins/watchdogwidget.ui
+drwxr-xr-x   0 patrick   (1000) patrick   (1000)        0 2024-05-09 01:45:50.166521 datalogd-0.4.0/datalogd.egg-info/
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     3715 2024-05-09 01:45:50.000000 datalogd-0.4.0/datalogd.egg-info/PKG-INFO
+-rw-r--r--   0 patrick   (1000) patrick   (1000)     1491 2024-05-09 01:45:50.000000 datalogd-0.4.0/datalogd.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)        1 2024-05-09 01:45:50.000000 datalogd-0.4.0/datalogd.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       43 2024-05-09 01:45:50.000000 datalogd-0.4.0/datalogd.egg-info/entry_points.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       30 2024-05-09 01:45:50.000000 datalogd-0.4.0/datalogd.egg-info/requires.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)        9 2024-05-09 01:45:50.000000 datalogd-0.4.0/datalogd.egg-info/top_level.txt
+-rw-r--r--   0 patrick   (1000) patrick   (1000)       38 2024-05-09 01:45:50.166521 datalogd-0.4.0/setup.cfg
+-rwxr-xr-x   0 patrick   (1000) patrick   (1000)     5889 2024-05-09 01:26:53.000000 datalogd-0.4.0/setup.py
```

### Comparing `datalogd-0.3.7/LICENSE.txt` & `datalogd-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/PKG-INFO` & `datalogd-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: datalogd
-Version: 0.3.7
+Version: 0.4.0
 Summary: A data logging daemon, easily customisable using a flexible plugin system.
 Home-page: https://gitlab.com/ptapping/datalogd
 Author: Patrick Tapping
 Author-email: mail@patricktapping.com
 Project-URL: Documentation, https://datalogd.readthedocs.io/
 Project-URL: Source, https://gitlab.com/ptapping/datalogd
 Project-URL: Tracker, https://gitlab.com/ptapping/datalogd/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE.txt
+Requires-Dist: wheel
+Requires-Dist: pluginlib
+Requires-Dist: pydot
+Requires-Dist: appdirs
 
 datalogd - A Data Logging Daemon
 ================================
 
 datalogd is a data logging daemon service which uses a source/filter/sink plugin architecture to
 allow extensive customisation and maximum flexibility. There are no strict specifications or
 requirements for data types, but typical examples would be readings from environmental sensors such
 as temperature, humidity, voltage or the like.
 
 The user guide and API documentation can be read online at `Read the Docs
 <https://datalogd.readthedocs.io/>`_. Source code is available on `GitLab
 <https://gitlab.com/ptapping/datalogd>`_.
 
 Custom data sources, filters, or sinks can be created simply by extending an existing
-``~datalogd.DataSource``, ``~datalogd.DataFilter``, or ``~datalogd.DataSink`` python
-class and placing it in a plugin directory.
+``DataSource``, ``DataFilter``, or ``DataSink`` python class and placing it in a plugin directory.
 
 Data sources, filters, and sinks can be arbitrarily connected together with a connection digraph
 described using the `DOT graph description language
 <https://en.wikipedia.org/wiki/DOT_(graph_description_language)>`_.
 
 Provided data source plugins include:
   * ``LibSensorsDataSource`` - (Linux) computer motherboard sensors for temperature, fan speed,
```

### Comparing `datalogd-0.3.7/README.rst` & `datalogd-0.4.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 as temperature, humidity, voltage or the like.
 
 The user guide and API documentation can be read online at `Read the Docs
 <https://datalogd.readthedocs.io/>`_. Source code is available on `GitLab
 <https://gitlab.com/ptapping/datalogd>`_.
 
 Custom data sources, filters, or sinks can be created simply by extending an existing
-``~datalogd.DataSource``, ``~datalogd.DataFilter``, or ``~datalogd.DataSink`` python
-class and placing it in a plugin directory.
+``DataSource``, ``DataFilter``, or ``DataSink`` python class and placing it in a plugin directory.
 
 Data sources, filters, and sinks can be arbitrarily connected together with a connection digraph
 described using the `DOT graph description language
 <https://en.wikipedia.org/wiki/DOT_(graph_description_language)>`_.
 
 Provided data source plugins include:
   * ``LibSensorsDataSource`` - (Linux) computer motherboard sensors for temperature, fan speed,
```

### Comparing `datalogd-0.3.7/datalogd/__init__.py` & `datalogd-0.4.0/datalogd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
         if plugindirs: plugin_paths.extend(plugindirs)
 
         # Show lists of available plugins
         try:
             loader = pluginlib.PluginLoader(group="datalogd", library="datalogd", paths=plugin_paths)
         except Exception as ex:
             raise RuntimeError(f"Error loading plugins: {ex.__name__}: {ex}")
-
         self.log.info(f"Detected source plugins: {', '.join(list(loader.plugins['DataSource']))}")
         self.log.info(f"Detected filter plugins: {', '.join(list(loader.plugins['DataFilter']))}")
         self.log.info(f"Detected sink plugins: {', '.join(list(loader.plugins['DataSink']))}")
 
         # Attempt to load connection graph=
         dot = graph_dot if graph_dot else config.get(appname, "connection_graph").strip()
         try:
@@ -116,15 +115,15 @@
             # Find the plugin from class name and initialise it
             try:
                 nc = loader.get_plugin("Data" + nodeclass.rpartition("Data")[2], nodeclass)
                 if nc is None:
                     raise RuntimeError(f"Error reading DOT connection graph. Can't find plugin for class {n.get_name()}:{nodeclass}.")
                 self.nodes[n.get_name()] = nc(*args, **kwargs)
             except Exception as ex:
-                raise RuntimeError(f"Unable to initialse node {n.get_name()}:{nodeclass} using args={args}, kwargs={kwargs}\n{ex}")
+                self.log.error(f"Unable to initialse node {n.get_name()}:{nodeclass} using args={args}, kwargs={kwargs}\n{ex}")
 
         # Ensure at least one node was initialised
         if not self.nodes:
             raise RuntimeError(f"No plugin nodes were initialised. Connection graph was:\n{dot}")
 
         # Make data connections from graph edges
         for e in graph.get_edges():
@@ -269,15 +268,15 @@
         if len(value) > 1 and value[0] == value[-1] and value[0] in "'\"":
             value = value[1:-1]
     return value
 
 
 @pluginlib.Parent(group="datalogd")
 class DataSource():
-    """
+    r"""
     The base class for all data sink plugins.
 
     :class:`~datalogd.DataSource` implements methods for connecting or
     disconnecting sinks, and for sending data to connected sinks. It has no
     intrinsic functionality (it does not actually produce any data) and is not
     itself considered a plugin, so can't be instantiated using the connection
     graph.
@@ -288,24 +287,24 @@
     """
     def __init__(self, sinks=[]):
         self.sinks = []
         if sinks: self.connect_sinks(sinks)
         self.log = logging.getLogger("DataSource")
 
     def send(self, data):
-        """
+        r"""
         Send the provided ``data`` to all connected :class:`DataSink`\ s.
 
         :param data: Data to send to :class:`DataSink`\ s.
         """
         for s in self.sinks:
             s.receive(data)
 
     def connect_sinks(self, sinks):
-        """
+        r"""
         Register the provided :class:`DataSink` as a receiver of data produced
         by this :class:`~datalogd.DataSource`. A list of sinks may also be
         provided.
 
         :param sinks: :class:`~datalogd.DataSink` or list of
             :class:`~datalogd.DataSink`\ s.
         """
@@ -321,15 +320,15 @@
                         self.sinks.append(s)
                     else:
                         raise AttributeError
                 except AttributeError:
                     self.log.warning(f"Skipping invalid sink: The {type(s).__name__} \"{s}\" does not have a receive() method.")
 
     def disconnect_sinks(self, sinks):
-        """
+        r"""
         Unregister the provided :class:`~datalogd.DataSink` so that it no longer
         receives data produced by this :class:`~datalogd.DataSource`. A list of
         sinks may also be provided. It is not an error to provide a sink that is
         not currently connected.
 
         :param sinks: :class:`~datalogd.DataSink` or list of
             :class:`~datalogd.DataSink`\ s.
@@ -355,15 +354,15 @@
     using the connection graph, although it provides no additional
     functionality.
     """
 
 
 @pluginlib.Parent(group="datalogd")
 class DataSink():
-    """
+    r"""
     The base class for all data sink plugins.
 
     :class:`~datalogd.DataSink`\ s have a :meth:`receive` method which accepts
     data from connected :class:`~datalogd.DataSource`\ s.
     """
     def receive(self, data):
         """
@@ -386,31 +385,31 @@
     Unlike the base :class:`~datalogd.DataSink`, this can be instantiated using
     the connection graph, although it provides no additional functionality.
     """
 
 
 @pluginlib.Parent(group="datalogd")
 class DataFilter(DataSource, DataSink):
-    """
+    r"""
     The base class for all data filter plugins.
 
     :class:`~datalogd.DataFilter`\ s are subclasses of both
     :class:`~datalogd.DataSource`\ s and :class:`~datalogd.DataSink`\ s, thus
     are capable of both sending and receiving data. Typically, they are used to
     sit between a :class:`~datalogd.DataSource` and a
     :class:`~datalogd.DataSink` (or other :class:`~datalogd.DataFilter`\ s) in
     order to modify the data flowing between them in some way.
     """
 
 
 class NullDataFilter(DataFilter):
-    """
+    r"""
     A :class:`~datalogd.DataFilter` which accepts data and passes it unchanged
     to any connected :class:`~datalogd.DataSink`\ s.
     """
     def receive(self, data):
-        """
+        r"""
         Pass ``data`` unchanged to all connected :class:`~datalogd.DataSink`\ s.
 
         :param data: Data received by this filter.
         """
         self.send(data)
```

### Comparing `datalogd-0.3.7/datalogd/plugins/aggregator_datafilter.py` & `datalogd-0.4.0/datalogd/plugins/aggregator_datafilter.py`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/datalogd/plugins/coolingpower_datafilter.py` & `datalogd-0.4.0/datalogd/plugins/coolingpower_datafilter.py`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/datalogd/plugins/csv_datafilter.py` & `datalogd-0.4.0/datalogd/plugins/csv_datafilter.py`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/datalogd/plugins/file_datasink.py` & `datalogd-0.4.0/datalogd/plugins/file_datasink.py`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/datalogd/plugins/flowsensorcalibration_datafilter.py` & `datalogd-0.4.0/datalogd/plugins/flowsensorcalibration_datafilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from  math import exp
 
 from datalogd import DataFilter, listify
 
 class FlowSensorCalibrationDataFilter(DataFilter):
-    """
+    r"""
     Use a pulse counter's counts per second to compute a liquid flow rate in litres per minute using
     an experimentally determined calibration function.
 
     A flow sensor has a spinning turbine and outputs pulses due to the flow rate of the liquid.
     However, the pulse rate will not be directly proportional to the flow rate (each pulse does not
     correspond to a fixed volume of liquid). A calibration curve can be constructed by measuring the
     number of pulses emitted over time for a given volume of liquid at a range of different flow
```

### Comparing `datalogd-0.3.7/datalogd/plugins/influxdb2_datasink.py` & `datalogd-0.4.0/datalogd/plugins/influxdb2_datasink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from datetime import datetime, timezone
 
 from datalogd import DataSink, listify
 
 try:
     from influxdb_client import InfluxDBClient
-    from influxdb_client.client.write_api import SYNCHRONOUS
-except ModuleNotFoundError:
+    #from influxdb_client.client.write_api import SYNCHRONOUS
+except (ModuleNotFoundError, ImportError):
     log = logging.getLogger(__name__.rpartition(".")[2])
     log.warning("influxdb_client module not found. Install it with \"pip install influxdb_client\" or similar.")
 else:
     # Required modules present, continue loading rest of this module
 
     class InfluxDB2DataSink(DataSink):
         """
@@ -69,15 +69,15 @@
         """
         def __init__(self, url="http://localhost:8086", token="", org="default", bucket="default", measurement="measurement", run_id=None, field_key=None, field_value=None):
             self.log = logging.getLogger("InfluxDB2DataSink")
             try:
                 self.client = InfluxDBClient(url, token=token, org=org)
             except Exception as ex:
                 self.log.exception("Unable to make connection to InfluxDB database.")
-            self.write_api = self.client.write_api(write_options=SYNCHRONOUS)
+            self.write_api = self.client.write_api()
             self.org = org
             self.bucket = bucket
             self.measurement = measurement
             if run_id is None:
                 self.run_id = datetime.now(timezone.utc).astimezone().strftime("%Y%m%d-%H%M%S")
             else:
                 self.run_id = run_id
@@ -117,18 +117,24 @@
 
             A timestamp for the commit will be generated using the current system clock if a
             "timestamp" field does not already exist.
 
             :param data: Data to commit to the database.
             """
             if data is None or data == []: return
+            if not self.client.ping():
+                self.log.debug("No database connection, data won't be stored.")
+                return
             data = listify(data)
 
             # Loop through each element in data list
             for d in data:
+                if type(d) == dict:
+                    # Don't modify the original dict data
+                    d = d.copy()
 
                 # Start building the structure to enter into database
                 datapoint = {
                     "measurement": self.measurement,
                     "tags": {"run_id": self.run_id},
                     "fields": {},
                 }
@@ -173,14 +179,14 @@
                 datapoint["tags"].update(d)
                 
                 # Send data point out to database
                 try:
                     self.log.debug(f"Committing: {datapoint}")
                     self.write_api.write(self.bucket, self.org, datapoint)
                 except Exception as ex:
-                    self.log.warning("Unable to commit data to InfluxDB database.", exc_info=True)
+                    self.log.warning("Unable to commit data to InfluxDB database.")
 
         def close(self):
             """
             Close the connection to the database.
             """
             self.client.close()
```

### Comparing `datalogd-0.3.7/datalogd/plugins/influxdb_datasink.py` & `datalogd-0.4.0/datalogd/plugins/influxdb_datasink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from datetime import datetime, timezone
 
 from datalogd import DataSink, listify
 
 try:
     from influxdb import InfluxDBClient
-except ModuleNotFoundError:
+except (ModuleNotFoundError, ImportError):
     log = logging.getLogger(__name__.rpartition(".")[2])
     log.warning("influxdb module not found. To use the InfluxDBDataSink, install the module with \"pip install influxdb\" or similar.")
 else:
     # Required modules present, continue loading rest of this module
 
     class InfluxDBDataSink(DataSink):
         """
```

### Comparing `datalogd-0.3.7/datalogd/plugins/join_datafilter.py` & `datalogd-0.4.0/datalogd/plugins/join_datafilter.py`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/datalogd/plugins/keyval_datafilter.py` & `datalogd-0.4.0/datalogd/plugins/keyval_datafilter.py`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/datalogd/plugins/libsensors_datasource.py` & `datalogd-0.4.0/datalogd/plugins/libsensors_datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 from enum import Enum
 
 from datalogd import DataSource
 
 try:
     import sensors
-except ModuleNotFoundError:
+except (ModuleNotFoundError, ImportError):
     log = logging.getLogger(__name__.rpartition(".")[2])
     log.warning("sensors module not found. Install it with \"pip install PySensors\" or similar.")
 else:
     # Required modules present, continue loading rest of this module
 
     class LibSensorsDataSource(DataSource):
         """
```

### Comparing `datalogd-0.3.7/datalogd/plugins/logging_datasink.py` & `datalogd-0.4.0/datalogd/plugins/logging_datasink.py`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/datalogd/plugins/matplotlib_datasink.py` & `datalogd-0.4.0/datalogd/plugins/matplotlib_datasink.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 
 from datalogd import DataSink, listify
 
 try:
     import matplotlib as mpl
     import matplotlib.pyplot as plt
-except ModuleNotFoundError:
+except (ModuleNotFoundError, ImportError):
     log = logging.getLogger(__name__.rpartition(".")[2])
     log.warning("matplotlib module not found. Install it with \"pip install matplotlib\" or similar.")
 else:
     # Required modules present, continue loading rest of this module
 
     class MatplotlibDataSink(DataSink):
         """
```

### Comparing `datalogd-0.3.7/datalogd/plugins/picotc08_datasource.py` & `datalogd-0.4.0/datalogd/plugins/picotc08_datasource.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,66 @@
 from ctypes import c_int8, c_int16, c_int32, c_float, byref
 from datetime import datetime, timezone, timedelta
 
 from datalogd import DataSource
 
 try:
     from picosdk.usbtc08 import usbtc08 as tc08
-except ModuleNotFoundError:
+except (ModuleNotFoundError, ImportError):
     log = logging.getLogger(__name__.rpartition(".")[2])
     log.warning("picosdk module not found. Install it with \"pip install picosdk\" or similar.")
 else:
     class PicoTC08DataSource(DataSource):
         """
         Obtain readings from a Pico Technologies TC-08 USB data logging device.
 
         The drivers and libraries (such as libusbtc08.so on Linux, usbtc08.dll on Windows) from
         PicoTech must be installed into a system library directory, and the ``picosdk`` python
         wrappers package must be on the system (with ``pip install picosdk`` or similar).
 
+        On Linux, read/write permissions to the USB device must be granted. This can be done with a
+        udev rule such as:
+
+        .. code-block:: none
+            :caption: ``/etc/udev/rules.d/51-picotc08.rules``
+
+            # PicoTech TC-08
+            SUBSYSTEMS=="usb", ACTION=="add", ATTRS{idVendor}=="0ce9, ATTRS{idProduct}=="1000", OWNER="root", GROUP="usbusers", MODE="0664"
+
+        where the ``idVendor`` and ``idProduct`` fields should match that listed from running
+        ``lsusb``. The ``usbusers`` group must be created and the user added to it:
+
+        .. code-block:: bash
+
+            groupadd usbusers
+            usermod -aG usbusers yourusername
+        
+        A reboot will then ensure permissions are set and the user is a part of the group (or use ``udevadm control --reload`` and re-login).
+        To check the permissions have been set correctly, get the USB bus and device numbers from the output of ``lsusb``. For example
+
+        .. code-block:: none
+            :caption: ``lsusb``
+        
+            Bus 001 Device 009: ID 0ce9:1000 Pico Technology 
+        
+        the bus ID is 001 and device ID is 009. Then list the device using ``ls -l /dev/bus/usb/[bus ID]/[device ID]``
+
+        .. code-block:: none
+            :caption: ``ls /dev/bus/usb/001/009 -l``
+
+            crw-rw-r-- 1 root usbusers 189, 9 Mar 29 13:19 /dev/bus/usb/001/009
+        
+        The middle "rw" and the "usbusers" indicates read-write permissions enabled to any user in
+        the usbusers group. You can check which groups your current user is in using the ``groups``
+        command.
+
+        Note that you may also allow read-write access to any user (without having to make a
+        usbusers group) by changing the lines in the udev rule to ``MODE="0666"`` and removing the
+        ``GROUP="usbusers"`` part.
+
         The ``interval`` parameter determines how often data will be obtained from the sensors, in
         seconds. The minimum interval time is about 0.2 s for a single probe and 0.9 s for all
         eight.
 
         The ``mains_rejection`` parameter filters out either 50 Hz or 60 Hz interference from mains
         power. The frequency is selected as either ``"50Hz"`` or ``"60Hz"``.
 
@@ -62,15 +102,15 @@
             self._handle = 0
             # Dictionary describing configured probes
             self._probes = {}
             # Configured sampling time interval, in seconds
             self._interval = self._req_interval
             # Get reference to event loop and schedule task (note loop probably hasn't started yet)
             self._loop = asyncio.get_event_loop()
-            self._connection_task = self._loop.create_task(self._connect_tc08(), name="PicoTC08DataSource Connector")
+            self._connection_task = self._loop.create_task(self._connect_tc08())  # For python 3.8+: , name="PicoTC08DataSource Connector")
             self._acquisition_task = None
 
 
         async def _connect_tc08(self):
             """
             Coroutine to attempt to find and connect to device over serial port.
             """
@@ -121,15 +161,15 @@
                         self._handle = 0
                     else:
                         self._log.debug("Starting TC-08 acquisition.")
                         # Everything seems OK, start the acquisition coroutine
                         self._interval = interval/1000
                         # Record local time of acquisition start
                         self._time_start = datetime.now(timezone.utc).astimezone()
-                        self._acquistion_task = self._loop.create_task(self._acquire_data(), name="PicoTC08DataSource Acquisition")
+                        self._acquistion_task = self._loop.create_task(self._acquire_data())  # For python 3.8+: , name="PicoTC08DataSource Acquisition")
                         return True
                 # No unit found, device busy, error opening device etc. Wait a bit before retrying
                 self._log.debug("No TC-08 units found or configured successfully, will retry.")
                 try:
                     await asyncio.sleep(5.0)
                 except asyncio.CancelledError:
                     return True
@@ -155,15 +195,15 @@
                         "CFKR".index(probe["units"]) if probe["units"] in "CFKR" else 0,
                         1)
                     if count < 0:
                         self._log.warning("Error acquiring data from Pico TC-08, will retry connection.")
                         # Closing sometimes seems to trigger a segfailt in the PicoTech library...
                         #tc08.usb_tc08_close_unit(self._handle)
                         self._handle = 0
-                        self._connection_task = self._loop.create_task(self._connect_tc08(), name="PicoTC08DataSource Connector")
+                        self._connection_task = self._loop.create_task(self._connect_tc08())  # For python 3.8+: , name="PicoTC08DataSource Connector")
                         return False
                     # Loop through each record
                     for i in range(count):
                         data.append({
                             "timestamp" : (self._time_start + timedelta(milliseconds=times[i])).isoformat(),
                             "type" : "analog" if probe["type"] == "X" else "temperature",
                             "source" : "TC-08",
```

### Comparing `datalogd-0.3.7/datalogd/plugins/polynomialfunction_datafilter.py` & `datalogd-0.4.0/datalogd/plugins/polynomialfunction_datafilter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,100 +1,108 @@
-import re
 
-import numpy as np
+import logging
 
-from datalogd import DataFilter, listify
-
-class PolynomialFunctionDataFilter(DataFilter):
-    """
-    Select data based on key--value pairs, then apply a polynomial function to a value.
-
-    Any data which matches all of the ``match_keyvals`` key--value pairs will be processed. The
-    format of the ``match_keyvals`` parameter is a list in the form ``[[key, value], [key2,
-    value2]...]``. For example, ``match_keyvals=[["type", "temperature"], ["id", "123"]]`` will
-    process any data which has a ``"type"`` field of ``"temperature"`` and an ``"id"`` field of
-    ``"123"``. A ``value`` of the python special ``NotImplemented`` will match any value for the
-    given key. In the case that values are strings, they will be matched as regular expressions, for
-    example ``".*"`` will match any string.
-
-    Once a data item is matched, a value will be selected to apply the polynomial function to,
-    selected by the ``value`` parameter. By default this is the value stored under the ``"value"`` key.
-
-    The polynomial function is defined by a set of coefficients, given by the ``coeffs`` parameter.
-    This is an array of :math:`n` coefficients, :math:`c_n`, which forms the function
-    :math:`x^\prime = \sum_n c_n x^{(n-1)} \equiv c_0 + c_1x + c_2x^2 \ldots c_nx^n`. For example,
-    ``coeffs=[1.23, 1.0]`` would add 1.23 to a value, while ``coeffs=[0, 10]`` would multiply a
-    value by 10. Specifying additional coefficients include quadratic, cubic terms etc.
-
-    Rounding may be applied to the result by supplying the number of decimal places in the
-    ``rounding`` parameter. Rounding behaviour is determined by the numpy ``around()`` function.
-    Negative numbers specify positions to the left of the decimal point.
-
-    The value of the data entry's ``"units"`` field can be modified or created using the ``units``
-    parameter. For example, ``units="V"`` might be used to indicate that an analogue measurement in
-    arbitrary units now equates to voltage, determined by the polynomial function calibration curve.
-
-    :param match_keyvals: Key--value pairs to match to data items.
-    :param value: Key from data item containing the value to modify.
-    :param coeffs: Coefficients of the polynomial function to apply.
-    :param rounding: Number of decimal places to round the result.
-    :param units: New value of units field for the modified data item.
-    """
-    def __init__(self, sinks=[], match_keyvals=[["type", ".*"], ["id", ".*"]], value="value", coeffs=[0.0, 1.0], rounding=None, units=None):
-        super().__init__(sinks=sinks)
-        self._keyvals = match_keyvals
-        self._value = value
-        self._coeffs = coeffs
-        self._rounding = rounding
-        self._units = units
-
-
-    def receive(self, data):
-        """
-        Accept the provided ``data``, select based on key/value pairs, apply function, and pass
-        onto connected sinks.
-
-        The selection is based upon the parameters provided to the constructor of this
-        :class:`~datalogd.plugins.polynomialfunction_datafilter.PolynomialFunctionDataFilter`.
-
-        :param data: Data to correct.
+try:
+    import numpy as np
+except (ModuleNotFoundError, ImportError):
+    log = logging.getLogger(__name__.rpartition(".")[2])
+    log.warning("numpy module not found. Install it with \"pip install numpy\" or similar.")
+else:
+    # OK, continue loading rest of module
+    import re
+    
+    from datalogd import DataFilter, listify
+
+    class PolynomialFunctionDataFilter(DataFilter):
+        r"""
+        Select data based on key--value pairs, then apply a polynomial function to a value.
+
+        Any data which matches all of the ``match_keyvals`` key--value pairs will be processed. The
+        format of the ``match_keyvals`` parameter is a list in the form ``[[key, value], [key2,
+        value2]...]``. For example, ``match_keyvals=[["type", "temperature"], ["id", "123"]]`` will
+        process any data which has a ``"type"`` field of ``"temperature"`` and an ``"id"`` field of
+        ``"123"``. A ``value`` of the python special ``NotImplemented`` will match any value for the
+        given key. In the case that values are strings, they will be matched as regular expressions, for
+        example ``".*"`` will match any string.
+
+        Once a data item is matched, a value will be selected to apply the polynomial function to,
+        selected by the ``value`` parameter. By default this is the value stored under the ``"value"`` key.
+
+        The polynomial function is defined by a set of coefficients, given by the ``coeffs`` parameter.
+        This is an array of :math:`n` coefficients, :math:`c_n`, which forms the function
+        :math:`x^\prime = \sum_n c_n x^{(n-1)} \equiv c_0 + c_1x + c_2x^2 \ldots c_nx^n`. For example,
+        ``coeffs=[1.23, 1.0]`` would add 1.23 to a value, while ``coeffs=[0, 10]`` would multiply a
+        value by 10. Specifying additional coefficients include quadratic, cubic terms etc.
+
+        Rounding may be applied to the result by supplying the number of decimal places in the
+        ``rounding`` parameter. Rounding behaviour is determined by the numpy ``around()`` function.
+        Negative numbers specify positions to the left of the decimal point.
+
+        The value of the data entry's ``"units"`` field can be modified or created using the ``units``
+        parameter. For example, ``units="V"`` might be used to indicate that an analogue measurement in
+        arbitrary units now equates to voltage, determined by the polynomial function calibration curve.
+
+        :param match_keyvals: Key--value pairs to match to data items.
+        :param value: Key from data item containing the value to modify.
+        :param coeffs: Coefficients of the polynomial function to apply.
+        :param rounding: Number of decimal places to round the result.
+        :param units: New value of units field for the modified data item.
         """
-        data = listify(data)
-        for d in data:
-            try:
-                # Look for matches to all key/value pairs
-                match = True
-                for kv_k, kv_v in self._keyvals:
-                    # Try looking for this key in this data entry
-                    v = d[kv_k]
-                    # This key exists, check its value
-                    if kv_v == v or ((type(kv_v) == type(v) == str) and re.fullmatch(kv_v, v)) or kv_v is NotImplemented:
-                        # Value matches, keep checking any remaining keyval pairs
-                        continue
-                    else:
-                        # Value doesn't match, can stop checking now
-                        match = False
-                        break
-                if match:
-                    # Retrieve specified value to correct
-                    x = d[self._value]
-                    # Allow correcting numpy arrays
-                    if isinstance(x, np.ndarray):
-                        y = np.zeros_like(x)
-                    else:
-                        y = 0
-                    # Apply polynomial function
-                    for n, c in enumerate(self._coeffs):
-                        y += c*x**n
-                    # Apply rounding if requested
-                    if self._rounding is not None:
-                        y = np.round(y, int(self._rounding))
-                    d[self._value] = y
-                    # Change or add new units to the data if given
-                    if self._units is not None:
-                        d["units"] = self._units
-            except (IndexError, KeyError, ValueError):
-                # An exception means we couldn't match this data entry, or find specified value
-                pass
-        self.send(data)
+        def __init__(self, sinks=[], match_keyvals=[["type", ".*"], ["id", ".*"]], value="value", coeffs=[0.0, 1.0], rounding=None, units=None):
+            super().__init__(sinks=sinks)
+            self._keyvals = match_keyvals
+            self._value = value
+            self._coeffs = coeffs
+            self._rounding = rounding
+            self._units = units
+
+
+        def receive(self, data):
+            """
+            Accept the provided ``data``, select based on key/value pairs, apply function, and pass
+            onto connected sinks.
+
+            The selection is based upon the parameters provided to the constructor of this
+            :class:`~datalogd.plugins.polynomialfunction_datafilter.PolynomialFunctionDataFilter`.
+
+            :param data: Data to correct.
+            """
+            data = listify(data)
+            for d in data:
+                try:
+                    # Look for matches to all key/value pairs
+                    match = True
+                    for kv_k, kv_v in self._keyvals:
+                        # Try looking for this key in this data entry
+                        v = d[kv_k]
+                        # This key exists, check its value
+                        if kv_v == v or ((type(kv_v) == type(v) == str) and re.fullmatch(kv_v, v)) or kv_v is NotImplemented:
+                            # Value matches, keep checking any remaining keyval pairs
+                            continue
+                        else:
+                            # Value doesn't match, can stop checking now
+                            match = False
+                            break
+                    if match:
+                        # Retrieve specified value to correct
+                        x = d[self._value]
+                        # Allow correcting numpy arrays
+                        if isinstance(x, np.ndarray):
+                            y = np.zeros_like(x)
+                        else:
+                            y = 0
+                        # Apply polynomial function
+                        for n, c in enumerate(self._coeffs):
+                            y += c*x**n
+                        # Apply rounding if requested
+                        if self._rounding is not None:
+                            y = np.round(y, int(self._rounding))
+                        d[self._value] = y
+                        # Change or add new units to the data if given
+                        if self._units is not None:
+                            d["units"] = self._units
+                except (IndexError, KeyError, ValueError):
+                    # An exception means we couldn't match this data entry, or find specified value
+                    pass
+            self.send(data)
```

### Comparing `datalogd-0.3.7/datalogd/plugins/print_datasink.py` & `datalogd-0.4.0/datalogd/plugins/print_datasink.py`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/datalogd/plugins/pyqtgraph_datasink.py` & `datalogd-0.4.0/datalogd/plugins/pyqtgraph_datasink.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,21 @@
 from queue import Empty
 
 from datalogd import DataSink, listify
 
 try:
     from PySide6 import QtCore
     from PySide6 import QtWidgets
-
+    import numpy as np
     import pyqtgraph as pg
-except ModuleNotFoundError:
+except (ModuleNotFoundError, ImportError):
     log = logging.getLogger(__name__.rpartition(".")[2])
-    log.warning("pyqtgraph module not found. Install it with \"pip install pyqtgraph pyside6\" or similar.")
+    log.warning("pyqtgraph module not found. Install it with \"pip install numpy pyqtgraph pyside6\" or similar.")
 else:
     # Required modules present, continue loading rest of this module
-    import numpy as np
-
 
     class PyqtgraphDataSink(DataSink):
         """
         Plot data in realtime in a pyqtgraph window.
 
         Multiple plot areas may be defined which will be stacked in rows with (by default) linked
         time axes. Each plot area may itself have multiple traces contained within. The complete
@@ -82,15 +80,14 @@
         :param title: String for title of the plot window.
         :param size: Tuple of (height, width) of the plot window.
         :param plotlayout: Data structure describing the plot layout and traces.
         :param xlink: Boolean, link the time axes of the plots.
         :param crosshair: Boolean, show the crosshair under the mouse pointer.
         """
         def __init__(self, **kwargs):
-            
             self.q = Queue()
             kwargs.update({"data_queue": self.q})
             self.appprocess = Process(target=self._exec_qt_app, kwargs=kwargs, name="PlotWindow")
             self.appprocess.start()
 
         def close(self):
             """
@@ -180,14 +177,20 @@
 
             if not self.data_queue is None:
                 self.timer = QtCore.QTimer()
                 self.timer.timeout.connect(self._update_plot)
                 self.timer.start(15)
 
 
+        def closeEvent(self, event):
+            # Don't close window, wait for parent to terminate our process instead
+            event.ignore()
+            self.showMinimized()
+
+
         def _mouse_moved(self, pos):
             for plot, traces, (hline, vline) in self.plots:
                 legend = plot.addLegend()
                 if plot.sceneBoundingRect().contains(pos):
                     point = plot.getViewBox().mapSceneToView(pos)
                     vline.show()
                     hline.show()
@@ -234,15 +237,15 @@
             }
 
 
         def _update_plot(self):
             while not self.data_queue.empty():
                 try:
                     data = self.data_queue.get(timeout=0.05)
-                except queue.Empty:
+                except Queue.Empty:
                     return
                 for d in data:
                     # Look through plot trace selector criteria looking for matching data
                     for p in self.plots:
                         for trace, traceaxis, tracedata, selectors in p[1]:
                             # Start by assuming data matches the selection criteria
                             match = True
@@ -257,22 +260,19 @@
                                         continue
                                     else:
                                         # Value doesn't match this trace, can stop checking now
                                         match = False
                                         break
                             except (IndexError, KeyError, ValueError) as ex:
                                 # An exception means we couldn't match this data entry to this trace
-                                print(ex)
                                 match = False
                             if match and "value" in d:
                                 # This data entry matched the selection criteria for this trace, update it
                                 tracedata[0:-1] = tracedata[1:]
                                 tracedata[-1] = d["value"]
                                 # Get timestamp from data, or create one if it doesn't exist
                                 traceaxis[0:-1] = traceaxis[1:]
                                 try:
                                     traceaxis[-1] = d["timestamp"].timestamp()
-                                except:
+                                except KeyError:
                                     traceaxis[-1] = datetime.now().timestamp()
                                 trace.setData(x=traceaxis, y=tracedata)
-
-
```

### Comparing `datalogd-0.3.7/datalogd/plugins/randomwalk_datasource.py` & `datalogd-0.4.0/datalogd/plugins/randomwalk_datasource.py`

 * *Files identical despite different names*

### Comparing `datalogd-0.3.7/datalogd/plugins/socket_datafilter.py` & `datalogd-0.4.0/datalogd/plugins/socket_datafilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import logging
 import json
 
 from datalogd import DataFilter
 
 class SocketDataFilter(DataFilter):
-    """
+    r"""
     Send and receive data over a network socket.
 
     The SocketDataFilter bridges data over a network socket. The other end of the connection may be
     another SocketDataFilter, but can be any application that uses the correct message encoding and
     structure. The connected sockets don't have to be on remote computers, and may be used to
     perform inter-process communications within a single machine.
 
@@ -82,18 +82,18 @@
             self._structure_type = structure_type
         else:
             self._log.warning("Data structure_type not supported.")
             self._structure_type = None
         # Get reference to event loop and schedule task (but loop probably isn't started yet)
         self.loop = asyncio.get_event_loop()
         if role == "server":
-            self._connection_task = self.loop.create_task(self._start_server(), name="SocketDataFilter Server Connector")
+            self._connection_task = self.loop.create_task(self._start_server())  # For python 3.8+: , name="SocketDataFilter Server Connector")
         else:
             role = "client"
-            self._connection_task = self.loop.create_task(self._start_client(), name="SocketDataFilter Client Connector")
+            self._connection_task = self.loop.create_task(self._start_client())  # For python 3.8+: , name="SocketDataFilter Client Connector")
 
 
     async def _start_server(self):
         """
         Coroutine to attempt to start the socket server.
         """
         self._server = None
@@ -125,15 +125,15 @@
                 await asyncio.sleep(5.0)
             else:
                 await self._handle_data(reader, writer)
 
 
     async def _handle_data(self, reader, writer):
         peer_name = writer.get_extra_info('peername')
-        self._log.info(f"Connection established to {peer_name}.")
+        self._log.info(f"Connection established with {peer_name}.")
         self._connections.append(writer)
         while True:
             try:
                 if self._message_delimiter:
                     # Multiple messages are expected, separated by a some delimiter bytes                
                     self._log.debug(f"Waiting for data block from {peer_name} delimited by {self._message_delimiter}")
                     data_bytes = await reader.readuntil(separator=self._message_delimiter)
@@ -145,17 +145,17 @@
                 # Stream limit exceeded, message may be incomplete
                 self._log.warning(f"Data block from {peer_name} exceeded buffer size.")
                 data_bytes = await reader.read(self._buffer_size)
                 # TODO: handle this better, could buffer and continue reading
             except asyncio.IncompleteReadError as ex:
                 # Connection closed before message completed
                 data_bytes = ex.partial
-                self._log.info("Connection to {} closed{}".format(peer_name, f" (read {len(data_bytes)} bytes)." if len(data_bytes) else "."))
-            except ConnectionResetError:
-                self._log.info(f"Connection to {peer_name} closed.")
+                self._log.info("Connection with {} closed{}".format(peer_name, f" (read {len(data_bytes)} bytes)." if len(data_bytes) else "."))
+            except (ConnectionResetError, BrokenPipeError, OSError):
+                self._log.info(f"Connection with {peer_name} closed.")
                 break
             if len(data_bytes) == 0:
                 break
             # Remove delimiter suffix if present
             if data_bytes[-len(self._message_delimiter):] == self._message_delimiter:
                 data_bytes = data_bytes[:-len(self._message_delimiter)]
             # If a message encoding given, attempt to decode
@@ -178,16 +178,16 @@
         # Close the connection
         self._connections.remove(writer)
         try:
             writer.write_eof()
             await writer.drain()
             writer.close()
             await writer.wait_closed()
-        except ConnectionResetError:
-            pass
+        except (ConnectionResetError, BrokenPipeError, OSError):
+            self._log.debug("Exception when closing connection, broken or already closed?")
 
 
     def receive(self, data):
         """
         Accept the provided data and output it to any connected sockets.
 
         :param data: Data to send to connected sockets.
```

### Comparing `datalogd-0.3.7/datalogd/plugins/thorlabspm100_datasource.py` & `datalogd-0.4.0/datalogd/plugins/thorlabspm100_datasource.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from enum import Enum
 
 from datalogd import DataSource
 
 try:
     import pyvisa
     from ThorlabsPM100 import ThorlabsPM100
-except ModuleNotFoundError:
+except (ModuleNotFoundError, ImportError):
     log = logging.getLogger(__name__.rpartition(".")[2])
     log.warning("ThorlabsPM100 and/or visa module not found. Install it with \"pip install pyvisa pyvisa-py pyusb ThorlabsPM100\" or similar. A VISA backend must also be present, use pyvisa-py if the native NI libraries are not installed.")
 else:
     # Required modules present, continue loading rest of this module
 
     class ThorlabsPMDataSource(DataSource):
         """
@@ -20,106 +20,137 @@
         This uses the VISA protocol over USB. On Linux, read/write permissions to the power meter
         device must be granted. This can be done with a udev rule such as:
 
         .. code-block:: none
             :caption: ``/etc/udev/rules.d/52-thorlabs-pm.rules``
 
             # Thorlabs PM100D
-            SUBSYSTEMS=="usb", ACTION=="add", ATTRS{idVendor}=="1313", ATTRS{idProduct}=="8078", OWNER="root", GROUP="usbusers", MODE="0664"
+            SUBSYSTEMS=="usb", ACTION=="add", ATTRS{idVendor}=="1313", ATTRS{idProduct}=="8078", OWNER="root", GROUP="plugdev", MODE="0664"
             # Thorlabs PM400
-            SUBSYSTEMS=="usb", ACTION=="add", ATTRS{idVendor}=="1313", ATTRS{idProduct}=="8075", OWNER="root", GROUP="usbusers", MODE="0664"
+            SUBSYSTEMS=="usb", ACTION=="add", ATTRS{idVendor}=="1313", ATTRS{idProduct}=="8075", OWNER="root", GROUP="plugdev", MODE="0664"
+            # Thorlabs PM16 Series
+            SUBSYSTEMS=="usb", ACTION=="add", ATTRS{idVendor}=="1313", ATTRS{idProduct}=="807c", OWNER="root", GROUP="plugdev", MODE="0664"
 
 
         where the ``idVendor`` and ``idProduct`` fields should match that listed from running
-        ``lsusb``. The ``usbusers`` group must be created and the user added to it:
+        ``lsusb``. The ``plugdev`` group must be created and the user added to it:
 
         .. code-block:: bash
 
-            groupadd usbusers
-            usermod -aG usbusers yourusername
+            groupadd plugdev
+            usermod -aG plugdev yourusername
 
         A reboot will then ensure permissions are set and the user is a part of the group (or use ``udevadm control --reload`` and re-login).
         To check the permissions have been set correctly, get the USB bus and device numbers from the output of ``lsusb``. For example
 
         .. code-block:: none
             :caption: ``lsusb``
         
             Bus 001 Device 010: ID 1313:8075 ThorLabs PM400 Handheld Optical Power/Energy Meter
         
         the bus ID is 001 and device ID is 010. Then list the device using ``ls -l /dev/bus/usb/[bus ID]/[device ID]``
 
         .. code-block:: none
             :caption: ``ls /dev/bus/usb/001/010 -l``
 
-            crw-rw-r-- 1 root usbusers 189, 9 Mar 29 13:19 /dev/bus/usb/001/010
+            crw-rw-r-- 1 root plugdev 189, 9 Mar 29 13:19 /dev/bus/usb/001/010
         
-        The middle "rw" and the "usbusers" indicates read-write permissions enabled to any user in
-        the usbusers group. You can check which groups your current user is in using the ``groups``
+        The middle "rw" and the "plugdev" indicates read-write permissions enabled to any user in
+        the plugdev group. You can check which groups your current user is in using the ``groups``
         command.
 
-        Note that you may also allow read-write access to any user (without having to make a
-        usbusers group) by changing the lines in the udev rule to ``MODE="0666"`` and removing the
-        ``GROUP="usbusers"`` part.
+        Note that you may also allow read-write access to any user (without having to use/create a
+        plugdev group) by changing the lines in the udev rule to ``MODE="0666"`` and removing the
+        ``GROUP="plugdev"`` part.
 
         :param serial_number: Serial number of power meter to use. If ``None``, will use the first device found.
         :param usb_vid: USB vendor ID (0x1313 or 4883 for Thorlabs).
         :param usb_pid: USB product ID (0x8078 for PM100D, 0x8075 for PM400).
         :param interval: How often to poll the sensors, in seconds.
         """
         def __init__(self, sinks=[], serial_number=None, usb_vid="0x1313", usb_pid="0x8078", interval=1.0):
             super().__init__(sinks=sinks)
-            self.log = logging.getLogger("ThorlabsPMDataSource")
+            self._log = logging.getLogger("ThorlabsPMDataSource")
             self.interval = interval
-            self.rm = pyvisa.ResourceManager()
-            if self.rm.visalib.library_path in ("py", "unset"):
-                # Native python VISA library, USB VID and PID in decimal, has extra field
-                # Here, 4883 == vendorID == 0x1313, 32888 == productID == 0x8078
-                try:
-                    usb_vid = int(usb_vid, 16)
-                    usb_pid = int(usb_pid, 16)
-                except Exception as ex:
-                    pass
-                res = self.rm.list_resources("USB0::{}::{}::{}::0::INSTR".format(usb_vid, usb_pid, serial_number if serial_number else "?*"))
-            else:
-                # NI VISA library (probably) in use, USB VID and PID are in hex, also extra field missing
-                res = self.rm.list_resources("USB0::{}::{}::{}::INSTR".format(usb_vid, usb_pid, serial_number if serial_number else "?*"))
-            if len(res) == 0:
-                self.log.warning("Could not find a Thorlabs PM device{}. Check USB device permissions and usb_pid parameter.".format(f" with serial {serial_number}" if serial_number else ""))
-                self.inst = None
-                self.pm = None
-                self.serial_number = None
-            else:
-                try:
-                    self.inst = self.rm.open_resource(res[0])
-                    self.pm = ThorlabsPM100(self.inst)
-                    self.serial_number = self.inst.resource_info.resource_name.split("::")[3]
-                    self.log.info(f"Initialised Thorlabs PM device: {self.serial_number}.")
-                    # Queue first call of update routine
-                    asyncio.get_event_loop().call_soon(self._read_power)
-                except Exception as ex:
-                    self.log.warning("Could not initialise Thorlabs PM device: {}".format(ex))
+
+            self._serial_number = serial_number
+            self._usb_vid = usb_vid
+            self._usb_pid = usb_pid
+
+            self._inst = None
+            self._pm = None
+            self._serial_number = None
+
+            self._loop = asyncio.get_event_loop()
+            self._connection_task = self._loop.create_task(self._connect_pm()) # python 3.8+: , name="ThorlabsPMDataSource Connector")
+
+
+        async def _connect_pm(self):
+            """
+            Coroutine to attempt connection to a Thorlabs power meter.
+            """
+            self._log.info("Searching for Thorlabs PM device...")
+            self._rm = pyvisa.ResourceManager()
+            while True:
+                if self._rm.visalib.library_path in ("py", "unset"):
+                    # Native python VISA library, USB VID and PID in decimal, has extra field
+                    # Here, 4883 == vendorID == 0x1313, 32888 == productID == 0x8078
+                    try:
+                        vid = int(self._usb_vid, 16)
+                        pid = int(self._usb_pid, 16)
+                    except ValueError as ex:
+                        pass
+                    device_string = f"USB0::{vid}::{pid}::{self._serial_number if self._serial_number else '?*'}::0::INSTR"
+                else:
+                    # NI VISA library (probably) in use, USB VID and PID are in hex, also extra field missing
+                    device_string = f"USB0::{vid}::{pid}::{self._serial_number if self._serial_number else '?*'}::INSTR"
+                self._log.debug(f"Looking for VISA device: {device_string}")
+                res = self._rm.list_resources(device_string)
+                if len(res) == 0:
+                    self._log.debug("Could not find a Thorlabs PM device{}. Check USB device permissions and usb_pid parameter.".format(f" with serial {self._serial_number}" if self._serial_number else ""))
+                    self._inst = None
+                    self._pm = None
+                    self._serial_number = None
+                else:
+                    try:
+                        self._inst = self._rm.open_resource(res[0])
+                        self._pm = ThorlabsPM100(self._inst)
+                        self._serial_number = self._inst.resource_info.resource_name.split("::")[3]
+                        self._log.info(f"Initialised Thorlabs PM device: {self._serial_number}.")
+                        # Queue first call of update routine and break out of connect loop
+                        self._loop.create_task(self._read_power())
+                        break
+                    except Exception as ex:
+                        self._log.warning("Could not initialise Thorlabs PM device: {}".format(ex))
+                # No device, try again in a little while
+                await asyncio.sleep(5)
+        
 
         def close(self):
             """
             Close the connection to the power meter.
             """
-            self.rm.close()
+            if self._rm is not None:
+                self._rm.close()
+
 
-        def _read_power(self):
+        async def _read_power(self):
             """
-            Read power and send data to any connected sinks.
+            Coroutine to read power and send data to any connected sinks.
             """
-            loop = asyncio.get_event_loop()
-            try:
-                data = {"type": "power", "source": "ThorlabsPM", "id": self.serial_number, "value": self.pm.read}
-                self.send(data)
-            except Exception as ex:
-                self.log.warning("Could not read power from Thorlabs PM device.")
-            # Reschedule next update
-            loop.call_later(self.interval, self._read_power)
+            while True:
+                try:
+                    data = {"type": "power", "source": "ThorlabsPM", "id": self._serial_number, "value": self._pm.read}
+                    self.send(data)
+                except Exception as ex:
+                    self._log.warning("Could not read power from Thorlabs PM device. Will attempt to reconnect.")
+                    await asyncio.sleep(2)
+                    self._loop.create_task(self._connect_pm()) # python 3.8+: , name="ThorlabsPMDataSource Connector")
+                    return
+                await asyncio.sleep(self.interval)
 
 
     class ThorlabsPM100DataSource(ThorlabsPMDataSource):
         """
         Provide data from a Thorlabs PM100 laser power meter.
 
         This is a wrapper around
@@ -145,8 +176,25 @@
         for accessing the USB device.
 
         :param serial_number: Serial number of power meter to use. If ``None``, will use the first
             device found.
         :param interval: How often to poll the sensors, in seconds.
         """
         def __init__(self, sinks=[], serial_number=None, interval=1.0):
-            super().__init__(sinks=sinks, usb_vid="0x1313", usb_pid="0x8075", serial_number=serial_number, interval=interval)
+            super().__init__(sinks=sinks, usb_vid="0x1313", usb_pid="0x8075", serial_number=serial_number, interval=interval)
+
+
+    class ThorlabsPM16DataSource(ThorlabsPMDataSource):
+        """
+        Provide data from a Thorlabs PM16 laser power meter.
+
+        This is a wrapper around
+        :class:`~datalogd.plugins.thorlabspm100_datasource.ThorlabsPMDataSource` with the
+        appropriate USB PID (0x807c) used as default. See its documentation regarding configuring permissions
+        for accessing the USB device.
+
+        :param serial_number: Serial number of power meter to use. If ``None``, will use the first
+            device found.
+        :param interval: How often to poll the sensors, in seconds.
+        """
+        def __init__(self, sinks=[], serial_number=None, interval=1.0):
+            super().__init__(sinks=sinks, usb_vid="0x1313", usb_pid="0x807c", serial_number=serial_number, interval=interval)
```

### Comparing `datalogd-0.3.7/datalogd/plugins/timestamp_datafilter.py` & `datalogd-0.4.0/datalogd/plugins/timestamp_datafilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datalogd import DataFilter, listify
 
 class TimeStampDataFilter(DataFilter):
     """
     Add or update a timestamp field to data using the current system clock.
     """
     def receive(self, data):
-        """
+        r"""
         Accept the provided ``data`` and add a timestamp field.
 
         If ``data``, or elements in the ``data`` list are ``dict``\ s, then a
         "timestamp" field will be added. Otherwise, the data entries will be
         converted to a ``dict`` with the old entry stored under a "value" field.
 
         :param data: Data to add a timestamp to.
```

### Comparing `datalogd-0.3.7/datalogd.egg-info/PKG-INFO` & `datalogd-0.4.0/datalogd.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: datalogd
-Version: 0.3.7
+Version: 0.4.0
 Summary: A data logging daemon, easily customisable using a flexible plugin system.
 Home-page: https://gitlab.com/ptapping/datalogd
 Author: Patrick Tapping
 Author-email: mail@patricktapping.com
 Project-URL: Documentation, https://datalogd.readthedocs.io/
 Project-URL: Source, https://gitlab.com/ptapping/datalogd
 Project-URL: Tracker, https://gitlab.com/ptapping/datalogd/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE.txt
+Requires-Dist: wheel
+Requires-Dist: pluginlib
+Requires-Dist: pydot
+Requires-Dist: appdirs
 
 datalogd - A Data Logging Daemon
 ================================
 
 datalogd is a data logging daemon service which uses a source/filter/sink plugin architecture to
 allow extensive customisation and maximum flexibility. There are no strict specifications or
 requirements for data types, but typical examples would be readings from environmental sensors such
 as temperature, humidity, voltage or the like.
 
 The user guide and API documentation can be read online at `Read the Docs
 <https://datalogd.readthedocs.io/>`_. Source code is available on `GitLab
 <https://gitlab.com/ptapping/datalogd>`_.
 
 Custom data sources, filters, or sinks can be created simply by extending an existing
-``~datalogd.DataSource``, ``~datalogd.DataFilter``, or ``~datalogd.DataSink`` python
-class and placing it in a plugin directory.
+``DataSource``, ``DataFilter``, or ``DataSink`` python class and placing it in a plugin directory.
 
 Data sources, filters, and sinks can be arbitrarily connected together with a connection digraph
 described using the `DOT graph description language
 <https://en.wikipedia.org/wiki/DOT_(graph_description_language)>`_.
 
 Provided data source plugins include:
   * ``LibSensorsDataSource`` - (Linux) computer motherboard sensors for temperature, fan speed,
```

### Comparing `datalogd-0.3.7/datalogd.egg-info/SOURCES.txt` & `datalogd-0.4.0/datalogd.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,23 +11,32 @@
 datalogd.egg-info/top_level.txt
 datalogd/plugins/__init__.py
 datalogd/plugins/aggregator_datafilter.py
 datalogd/plugins/coolingpower_datafilter.py
 datalogd/plugins/csv_datafilter.py
 datalogd/plugins/file_datasink.py
 datalogd/plugins/flowsensorcalibration_datafilter.py
+datalogd/plugins/heartbeat_datasource.py
 datalogd/plugins/influxdb2_datasink.py
 datalogd/plugins/influxdb_datasink.py
 datalogd/plugins/join_datafilter.py
 datalogd/plugins/keyval_datafilter.py
 datalogd/plugins/libsensors_datasource.py
 datalogd/plugins/logging_datasink.py
+datalogd/plugins/logwidget.ui
 datalogd/plugins/matplotlib_datasink.py
 datalogd/plugins/picotc08_datasource.py
 datalogd/plugins/polynomialfunction_datafilter.py
 datalogd/plugins/print_datasink.py
 datalogd/plugins/pyqtgraph_datasink.py
 datalogd/plugins/randomwalk_datasource.py
+datalogd/plugins/resources_rc.py
+datalogd/plugins/sensoridentifierdatafilter.py
+datalogd/plugins/sensorpaneldatafilter.py
+datalogd/plugins/sensorpaneldatafilter_demo.ui
+datalogd/plugins/sensorwidget.ui
 datalogd/plugins/serial_datasource.py
+datalogd/plugins/sinktimer_datafilter.py
 datalogd/plugins/socket_datafilter.py
 datalogd/plugins/thorlabspm100_datasource.py
-datalogd/plugins/timestamp_datafilter.py
+datalogd/plugins/timestamp_datafilter.py
+datalogd/plugins/watchdogwidget.ui
```

### Comparing `datalogd-0.3.7/setup.py` & `datalogd-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Description=Data Logging Daemon
 
 [Service]
 Type=simple
 ExecStart=/usr/bin/datalogd
 
 [Install]
-WantedBy=multi-user.target
+WantedBy=default.target
 """
 
 
 """
 Implements the distutils 'install' command to install service startup files.
 """
 from setuptools.command.install import install
@@ -132,15 +132,15 @@
             try:
                 os.system("systemctl --user daemon-reload > /dev/null 2>&1")
             except: pass
 
 
 setuptools.setup(
     name="datalogd",
-    version="0.3.7",
+    version="0.4.0",
     author="Patrick Tapping",
     author_email="mail@patricktapping.com",
     description="A data logging daemon, easily customisable using a flexible plugin system.",
     long_description=long_description,
     url="https://gitlab.com/ptapping/datalogd",
     project_urls={
         "Documentation": "https://datalogd.readthedocs.io/",
@@ -149,20 +149,24 @@
     },
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=[
+        "wheel",
         "pluginlib",
         "pydot",
         "appdirs",
     ],
+    package_data={
+        "": [ "*.ui" ],
+    },
     entry_points={
         "console_scripts": [
             "datalogd = datalogd:main",
         ],
     },
     cmdclass={
         'install': CustomInstallCommand,
```


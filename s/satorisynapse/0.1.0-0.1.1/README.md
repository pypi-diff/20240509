# Comparing `tmp/satorisynapse-0.1.0.tar.gz` & `tmp/satorisynapse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satorisynapse-0.1.0.tar", last modified: Sun May  5 15:53:08 2024, max compression
+gzip compressed data, was "satorisynapse-0.1.1.tar", last modified: Wed May  8 22:44:04 2024, max compression
```

## Comparing `satorisynapse-0.1.0.tar` & `satorisynapse-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/satorisynapse/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/satorisynapse/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/satorisynapse/synapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/synapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13961 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/synapse/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)    13238 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/satorisynapse/synapse/threaded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/satorisynapse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 15:53:08.000000 satorisynapse-0.1.0/satorisynapse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 15:53:08.075050 satorisynapse-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-05 15:53:01.000000 satorisynapse-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:04.184211 satorisynapse-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-08 22:44:04.184211 satorisynapse-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:04.180211 satorisynapse-0.1.1/satorisynapse/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:04.184211 satorisynapse-0.1.1/satorisynapse/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/lib/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/lib/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:04.184211 satorisynapse-0.1.1/satorisynapse/synapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/synapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/synapse/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/satorisynapse/synapse/threaded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:44:04.180211 satorisynapse-0.1.1/satorisynapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-08 22:44:04.000000 satorisynapse-0.1.1/satorisynapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 22:44:04.000000 satorisynapse-0.1.1/satorisynapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 22:44:04.000000 satorisynapse-0.1.1/satorisynapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 22:44:04.000000 satorisynapse-0.1.1/satorisynapse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 22:44:04.000000 satorisynapse-0.1.1/satorisynapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:44:04.184211 satorisynapse-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-08 22:43:55.000000 satorisynapse-0.1.1/setup.py
```

### Comparing `satorisynapse-0.1.0/LICENSE` & `satorisynapse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.1.0/PKG-INFO` & `satorisynapse-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.1.0
+Version: 0.1.1
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.1.0/satorisynapse/lib/domain.py` & `satorisynapse-0.1.1/satorisynapse/lib/domain.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.1.0/satorisynapse/lib/requests.py` & `satorisynapse-0.1.1/satorisynapse/lib/requests.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.1.0/satorisynapse/run.py` & `satorisynapse-0.1.1/satorisynapse/run.py`

 * *Files identical despite different names*

### Comparing `satorisynapse-0.1.0/satorisynapse/synapse/asynchronous.py` & `satorisynapse-0.1.1/satorisynapse/synapse/asynchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                     subprocess.Popen((
                         'docker run --rm -it --name satorineuron '
                         '-p 24601:24601 '
                         f'-v {os.path.join(self.installDir, "wallet")}:/Satori/Neuron/wallet '
                         f'-v {os.path.join(self.installDir, "config")}:/Satori/Neuron/config '
                         f'-v {os.path.join(self.installDir, "data")}:/Satori/Neuron/data '
                         f'-v {os.path.join(self.installDir, "models")}:/Satori/Neuron/models '
-                        '--env SATORI_RUN_MODE=prod '
+                        '--env ENV=prod '
                         f'satorinet/satorineuron:{self.version} ./start.sh'),)
             if msg.vesicle.shutdown:
                 greyPrint('shutting down Satori Neuron...')
                 self.broke.set()
                 subprocess.Popen('docker stop satorineuron')
                 time.sleep(30)
                 # exit()
```

### Comparing `satorisynapse-0.1.0/satorisynapse/synapse/threaded.py` & `satorisynapse-0.1.1/satorisynapse/synapse/threaded.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
                     subprocess.Popen((
                         'docker run --rm -it --name satorineuron '
                         '-p 24601:24601 '
                         f'-v {os.path.join(self.installDir, "wallet")}:/Satori/Neuron/wallet '
                         f'-v {os.path.join(self.installDir, "config")}:/Satori/Neuron/config '
                         f'-v {os.path.join(self.installDir, "data")}:/Satori/Neuron/data '
                         f'-v {os.path.join(self.installDir, "models")}:/Satori/Neuron/models '
-                        '--env SATORI_RUN_MODE=prod '
+                        '--env ENV=prod '
                         f'satorinet/satorineuron:{self.version} ./start.sh'),)
                     raise Exception('restarting neuron...')
             if signal.shutdown:
                 greyPrint('shutting down Satori Neuron...')
                 subprocess.Popen('docker stop satorineuron')
                 time.sleep(30)
                 self.shutdown()
```

### Comparing `satorisynapse-0.1.0/satorisynapse.egg-info/PKG-INFO` & `satorisynapse-0.1.1/satorisynapse.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satorisynapse
-Version: 0.1.0
+Version: 0.1.1
 Summary: satorisynapse contains domain model and apis for the Satori Network
 Home-page: https://github.com/SatoriNetwork/satorisynapse
 Download-URL: https://github.com/SatoriNetwork/satorisynapse
 Author: Jordan Miller
 Author-email: jordan@satorinet.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `satorisynapse-0.1.0/setup.py` & `satorisynapse-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 def get_name():
     return 'satorisynapse'
 
 
 def get_version():
-    return '0.1.0'
+    return '0.1.1'
 
 
 def get_requirements():
     requirements = get_here('requirements.txt')
     if os.path.isfile(requirements):
         with open(requirements, 'r') as f:
             return f.read().splitlines()
```


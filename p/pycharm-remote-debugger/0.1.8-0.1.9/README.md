# Comparing `tmp/pycharm_remote_debugger-0.1.8.tar.gz` & `tmp/pycharm_remote_debugger-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycharm_remote_debugger-0.1.8.tar", last modified: Thu Jun 17 18:02:58 2021, max compression
+gzip compressed data, was "pycharm_remote_debugger-0.1.9.tar", last modified: Sun Jun 20 19:36:41 2021, max compression
```

## Comparing `pycharm_remote_debugger-0.1.8.tar` & `pycharm_remote_debugger-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 elior     (1000) elior     (1000)        0 2021-06-17 18:02:58.349580 pycharm_remote_debugger-0.1.8/
--rw-r--r--   0 elior     (1000) elior     (1000)       65 2021-06-16 18:17:15.000000 pycharm_remote_debugger-0.1.8/MANIFEST.in
--rw-rw-r--   0 elior     (1000) elior     (1000)     2435 2021-06-17 18:02:58.349580 pycharm_remote_debugger-0.1.8/PKG-INFO
--rw-r--r--   0 elior     (1000) elior     (1000)     1316 2021-06-17 18:01:23.000000 pycharm_remote_debugger-0.1.8/README.md
--rw-r--r--   0 elior     (1000) elior     (1000)       22 2021-06-16 18:26:14.000000 pycharm_remote_debugger-0.1.8/requirements.txt
--rw-rw-r--   0 elior     (1000) elior     (1000)       38 2021-06-17 18:02:58.349580 pycharm_remote_debugger-0.1.8/setup.cfg
--rw-r--r--   0 elior     (1000) elior     (1000)     1637 2021-06-16 18:24:05.000000 pycharm_remote_debugger-0.1.8/setup.py
-drwxrwxr-x   0 elior     (1000) elior     (1000)        0 2021-06-17 18:02:58.348580 pycharm_remote_debugger-0.1.8/src/
-drwxrwxr-x   0 elior     (1000) elior     (1000)        0 2021-06-17 18:02:58.348580 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger/
--rw-r--r--   0 elior     (1000) elior     (1000)      119 2021-06-17 17:50:41.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger/__init__.py
--rw-r--r--   0 elior     (1000) elior     (1000)     1472 2021-06-17 17:44:28.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger/__main__.py
--rw-r--r--   0 elior     (1000) elior     (1000)     1054 2021-06-17 17:00:51.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger/_logger.py
--rw-r--r--   0 elior     (1000) elior     (1000)     2821 2021-06-17 17:59:23.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger/_pycharm_remote_debugger.py
-drwxrwxr-x   0 elior     (1000) elior     (1000)        0 2021-06-17 18:02:58.349580 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger.egg-info/
--rw-rw-r--   0 elior     (1000) elior     (1000)     2435 2021-06-17 18:02:58.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger.egg-info/PKG-INFO
--rw-rw-r--   0 elior     (1000) elior     (1000)      542 2021-06-17 18:02:58.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger.egg-info/SOURCES.txt
--rw-rw-r--   0 elior     (1000) elior     (1000)        1 2021-06-17 18:02:58.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger.egg-info/dependency_links.txt
--rw-rw-r--   0 elior     (1000) elior     (1000)       75 2021-06-17 18:02:58.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger.egg-info/entry_points.txt
--rw-rw-r--   0 elior     (1000) elior     (1000)       23 2021-06-17 18:02:58.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger.egg-info/requires.txt
--rw-rw-r--   0 elior     (1000) elior     (1000)       24 2021-06-17 18:02:58.000000 pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger.egg-info/top_level.txt
--rw-r--r--   0 elior     (1000) elior     (1000)       17 2021-06-17 18:02:58.000000 pycharm_remote_debugger-0.1.8/version.txt
+drwxrwxr-x   0 elior     (1000) elior     (1000)        0 2021-06-20 19:36:41.028788 pycharm_remote_debugger-0.1.9/
+-rw-r--r--   0 elior     (1000) elior     (1000)       65 2021-06-16 18:17:15.000000 pycharm_remote_debugger-0.1.9/MANIFEST.in
+-rw-rw-r--   0 elior     (1000) elior     (1000)     2466 2021-06-20 19:36:41.027788 pycharm_remote_debugger-0.1.9/PKG-INFO
+-rw-r--r--   0 elior     (1000) elior     (1000)     1331 2021-06-20 19:35:34.000000 pycharm_remote_debugger-0.1.9/README.md
+-rw-r--r--   0 elior     (1000) elior     (1000)       22 2021-06-16 18:26:14.000000 pycharm_remote_debugger-0.1.9/requirements.txt
+-rw-rw-r--   0 elior     (1000) elior     (1000)       38 2021-06-20 19:36:41.028788 pycharm_remote_debugger-0.1.9/setup.cfg
+-rw-r--r--   0 elior     (1000) elior     (1000)     1637 2021-06-16 18:24:05.000000 pycharm_remote_debugger-0.1.9/setup.py
+drwxrwxr-x   0 elior     (1000) elior     (1000)        0 2021-06-20 19:36:41.026788 pycharm_remote_debugger-0.1.9/src/
+drwxrwxr-x   0 elior     (1000) elior     (1000)        0 2021-06-20 19:36:41.027788 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger/
+-rw-r--r--   0 elior     (1000) elior     (1000)      119 2021-06-17 17:50:41.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger/__init__.py
+-rw-r--r--   0 elior     (1000) elior     (1000)     1436 2021-06-20 19:34:33.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger/__main__.py
+-rw-r--r--   0 elior     (1000) elior     (1000)     1054 2021-06-17 17:00:51.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger/_logger.py
+-rw-r--r--   0 elior     (1000) elior     (1000)     2821 2021-06-17 17:59:23.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger/_pycharm_remote_debugger.py
+drwxrwxr-x   0 elior     (1000) elior     (1000)        0 2021-06-20 19:36:41.027788 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger.egg-info/
+-rw-rw-r--   0 elior     (1000) elior     (1000)     2466 2021-06-20 19:36:40.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger.egg-info/PKG-INFO
+-rw-rw-r--   0 elior     (1000) elior     (1000)      542 2021-06-20 19:36:40.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger.egg-info/SOURCES.txt
+-rw-rw-r--   0 elior     (1000) elior     (1000)        1 2021-06-20 19:36:40.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger.egg-info/dependency_links.txt
+-rw-rw-r--   0 elior     (1000) elior     (1000)       75 2021-06-20 19:36:40.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger.egg-info/entry_points.txt
+-rw-rw-r--   0 elior     (1000) elior     (1000)       23 2021-06-20 19:36:40.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger.egg-info/requires.txt
+-rw-rw-r--   0 elior     (1000) elior     (1000)       24 2021-06-20 19:36:40.000000 pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger.egg-info/top_level.txt
+-rw-r--r--   0 elior     (1000) elior     (1000)       17 2021-06-20 19:36:40.000000 pycharm_remote_debugger-0.1.9/version.txt
```

### Comparing `pycharm_remote_debugger-0.1.8/PKG-INFO` & `pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pycharm_remote_debugger
-Version: 0.1.8
+Name: pycharm-remote-debugger
+Version: 0.1.9
 Summary: Easily debug your remote project
 Home-page: https://github.com/eliorerz/pycharm-remote-debugger
 Author: Elior Erez
 Author-email: elior123@gmail.com
 License: MIT
 Description: # Pycharm Remote Debugger
         
@@ -40,14 +40,16 @@
            - Use the command line: 
            ```shell
            python -m pycharm_remote_debugger -r 10.2.55.1 -p 6789 -m my_module_name -k module_arg1 -s -k module_arg2
            ```
         6. Start debugger on pycharm
         7. Debug your program :) 
         
+        ## Arguments:
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pycharm_remote_debugger-0.1.8/README.md` & `pycharm_remote_debugger-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,7 +31,9 @@
    ```
    - Use the command line: 
    ```shell
    python -m pycharm_remote_debugger -r 10.2.55.1 -p 6789 -m my_module_name -k module_arg1 -s -k module_arg2
    ```
 6. Start debugger on pycharm
 7. Debug your program :) 
+
+## Arguments:
```

### Comparing `pycharm_remote_debugger-0.1.8/setup.py` & `pycharm_remote_debugger-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger/__main__.py` & `pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,28 +8,28 @@
     parser.add_argument("-r", "--remote", help="Remote machine address", type=str)
     parser.add_argument("-p", "--port", help="Remote debugger port", type=int)
     parser.add_argument("-o", "--optional", help="Continue if not able to connect to the remote debugger", nargs='?',
                         default=False, type=bool, const=True)
     parser.add_argument("-t", "--timeout", help="Connection timeout", type=int,
                         default=PycharmRemoteDebugger.DEFAULT_CONNECTION_TIMEOUT)
     parser.add_argument("-m", "--module", help="Module to run", type=str, nargs="...")
-    parser.add_argument("-f", "--file", help="Python script to run", type=str, nargs="...")
+    parser.add_argument("script", nargs="...")
     args = parser.parse_args()
 
     if not args.port or not args.remote:
         raise ValueError("Missing remote IDE arguments - try: remote_debugger -r <remote_address> -p <port> ... ")
 
-    if args.port is None and args.module is None:
-        raise ValueError("Missing script or module to execute")
+    if args.script is None and args.module is None:
+        raise ValueError("Missing script path or module to execute")
 
     return args
 
 
 def main():
     args = get_args()
     code_type = CodeType.MODULE if args.module else CodeType.FILE
-    debugger = PycharmRemoteDebugger(args.remote, args.port, code_type, args.module or args.file, args.optional)
+    debugger = PycharmRemoteDebugger(args.remote, args.port, code_type, args.module or args.script, args.optional)
     debugger.debug(args.timeout)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger/_logger.py` & `pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger/_logger.py`

 * *Files identical despite different names*

### Comparing `pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger/_pycharm_remote_debugger.py` & `pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger/_pycharm_remote_debugger.py`

 * *Files identical despite different names*

### Comparing `pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger.egg-info/PKG-INFO` & `pycharm_remote_debugger-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pycharm-remote-debugger
-Version: 0.1.8
+Name: pycharm_remote_debugger
+Version: 0.1.9
 Summary: Easily debug your remote project
 Home-page: https://github.com/eliorerz/pycharm-remote-debugger
 Author: Elior Erez
 Author-email: elior123@gmail.com
 License: MIT
 Description: # Pycharm Remote Debugger
         
@@ -40,14 +40,16 @@
            - Use the command line: 
            ```shell
            python -m pycharm_remote_debugger -r 10.2.55.1 -p 6789 -m my_module_name -k module_arg1 -s -k module_arg2
            ```
         6. Start debugger on pycharm
         7. Debug your program :) 
         
+        ## Arguments:
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pycharm_remote_debugger-0.1.8/src/pycharm_remote_debugger.egg-info/SOURCES.txt` & `pycharm_remote_debugger-0.1.9/src/pycharm_remote_debugger.egg-info/SOURCES.txt`

 * *Files identical despite different names*


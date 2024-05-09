# Comparing `tmp/automvs-0.0.8.tar.gz` & `tmp/automvs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automvs-0.0.8.tar", last modified: Mon May  6 05:44:27 2024, max compression
+gzip compressed data, was "automvs-0.0.9.tar", last modified: Thu May  9 18:41:28 2024, max compression
```

## Comparing `automvs-0.0.8.tar` & `automvs-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-06 05:44:27.421794 automvs-0.0.8/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.8/LICENSE
--rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-06 05:44:27.421794 automvs-0.0.8/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.8/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-06 05:44:27.421794 automvs-0.0.8/automvs/
--rw-rw-r--   0 phil      (1000) phil      (1000)    35123 2024-05-06 05:43:46.000000 automvs-0.0.8/automvs/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-06 05:44:27.421794 automvs-0.0.8/automvs.egg-info/
--rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-06 05:44:27.000000 automvs-0.0.8/automvs.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-06 05:44:27.000000 automvs-0.0.8/automvs.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-06 05:44:27.000000 automvs-0.0.8/automvs.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-06 05:44:27.000000 automvs-0.0.8/automvs.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-06 05:44:27.421794 automvs-0.0.8/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-06 05:43:56.000000 automvs-0.0.8/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 18:41:28.519063 automvs-0.0.9/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.9/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-09 18:41:28.519063 automvs-0.0.9/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.9/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 18:41:28.519063 automvs-0.0.9/automvs/
+-rw-rw-r--   0 phil      (1000) phil      (1000)    37822 2024-05-09 18:38:08.000000 automvs-0.0.9/automvs/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-09 18:41:28.519063 automvs-0.0.9/automvs.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-09 18:41:28.000000 automvs-0.0.9/automvs.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-09 18:41:28.000000 automvs-0.0.9/automvs.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-09 18:41:28.000000 automvs-0.0.9/automvs.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-09 18:41:28.000000 automvs-0.0.9/automvs.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-09 18:41:28.519063 automvs-0.0.9/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-09 17:45:56.000000 automvs-0.0.9/setup.py
```

### Comparing `automvs-0.0.8/LICENSE` & `automvs-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `automvs-0.0.8/PKG-INFO` & `automvs-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.8/README.md` & `automvs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `automvs-0.0.8/automvs/__init__.py` & `automvs-0.0.9/automvs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     fashion. This can be used for deploying XMI files, pushing out updates, 
     building software, creating custom MVS deployments.
 
     Using this library requires a hercules SDL and MVS/CE for MVS/CE and/or
     TK4-/TK5 for those MVS3.8j.
 """
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 __author__ = 'Philip Young'
 __license__ = "GPL"
 
 # Copyright (c) 2021, Philip Young
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -496,14 +496,60 @@
                 return
 
             except queue.Empty:
                 #self.logger.debug("Empty Queue")
                 continue
             
 
+    def wait_for_strings(self, strings_to_waitfor, stderr=False, timeout=False):
+        '''
+           Reads stdout queue waiting for expected response, default is
+           to check STDOUT queue, set stderr=True to check stderr queue instead
+           default timeout is 30 minutes.and
+
+           Unlike wait_for_string() this function takes a list of strings
+           and returns when any of the strings in the list are found. 
+        '''
+        time_started = time.time()
+
+        if not timeout and self.timeout:
+            timeout=self.timeout
+
+        if not timeout:
+            timeout = TIMEOUT
+
+        self.logger.debug("[AUTOMATION: MVS/CE] Waiting {} seconds for string to appear in hercules log: {}".format(timeout,strings_to_waitfor))
+
+        while True:
+            if time.time() > time_started + timeout:
+                exception = "Waiting for one of '{}' timed out after {} seconds".format(strings_to_waitfor, timeout)
+                print("[AUTOMATION: MVS/CE] {}".format(exception))
+                raise Exception(exception)
+
+            try:
+                if stderr:
+                    line = self.stderr_q.get(False).strip()
+                else:
+                    line = self.stdout_q.get(False).strip()
+                while not any(word in line for word in strings_to_waitfor):
+                    if stderr:
+                        line = self.stderr_q.get(False).strip()
+                    else:
+                        line = self.stdout_q.get(False).strip()
+                    continue
+                for word in strings_to_waitfor:
+                    if word in line:
+                        break
+                return word
+
+            except queue.Empty:
+                #self.logger.debug("Empty Queue")
+                continue
+            
+
     def ipl(self, step_text='', clpa=False):
         self.logger.debug(step_text)
         self.reset_hercules(clpa=clpa)
         #self.wait_for_string("0:0151 CKD")
 
         if clpa:
             self.send_herc("ipl 150")
@@ -670,14 +716,36 @@
                 raise Exception(exception)
 
             new_lines = self.read_log_lines()
             for line in new_lines:
                 if string_to_waitfor in line:
                     return
 
+
+
+    def wait_for_strings(self,strings_to_waitfor):
+        '''
+        Unlike string to wait for this function 
+        '''
+        self.logger.debug(f"[AUTOMATION: {self.system}] Waiting for any of these strings '{strings_to_waitfor}' in {self.logfile}")
+        time_started = time.time()
+
+        self.logger.debug(f"[AUTOMATION: {self.system}] Waiting {self.timeout} seconds for strings to appear in hercules log: {strings_to_waitfor}")
+
+        while True:
+            if time.time() > time_started + self.timeout:
+                exception = f"Waiting for any of the strings timed out after {self.timeout} seconds"
+                print("[ERR] {}".format(exception))
+                raise Exception(exception)
+
+            new_lines = self.read_log_lines()
+            for line in new_lines:
+                if any(word in line for word in strings_to_waitfor):
+                    return
+
     def wait_for_job(self, jobname):
         self.wait_for_string("HASP250 {:<8} IS PURGED".format(jobname))
 
     def change_punchcard_output(self,path):
         self.logger.debug(f"[AUTOMATION: {self.system}] Changing 3525 Punchcard output location to: '{path}'")
         if not os.path.exists(os.path.dirname(path)): 
             self.logger.debug(f"[AUTOMATION: {self.system}] Punchcard folder '{path}' does not exist")
```

### Comparing `automvs-0.0.8/automvs.egg-info/PKG-INFO` & `automvs-0.0.9/automvs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.8/setup.py` & `automvs-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='automvs',
-    version='0.0.8',    
+    version='0.0.9',    
     description='Python library for MVS/CE automation',
     url='https://github.com/MVS-sysgen/automvs',
     author='Philip Young',
     author_email='mainframed767@gmail.com',
     license='MIT',
     packages=['automvs'],
     install_requires=[],
```


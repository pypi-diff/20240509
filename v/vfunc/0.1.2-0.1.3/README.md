# Comparing `tmp/vfunc-0.1.2.tar.gz` & `tmp/vfunc-0.1.3.tar.gz`

## Comparing `vfunc-0.1.2.tar` & `vfunc-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 vfunc-0.1.2/src/vfunc/__init__.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 vfunc-0.1.2/src/vfunc/_vfunc.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 vfunc-0.1.2/LICENSE
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 vfunc-0.1.2/README.md
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 vfunc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 vfunc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 vfunc-0.1.3/src/vfunc/__init__.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 vfunc-0.1.3/src/vfunc/_vfunc.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 vfunc-0.1.3/LICENSE
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 vfunc-0.1.3/README.md
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 vfunc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 vfunc-0.1.3/PKG-INFO
```

### Comparing `vfunc-0.1.2/src/vfunc/_vfunc.py` & `vfunc-0.1.3/src/vfunc/_vfunc.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,59 +3,66 @@
 
 if sys.platform == "win32":
     timer = time.perf_counter
 else:
     timer = time.time
 
 
-def conv(data, mode="speed"):
+def convert(data, mode="speed"):
     if mode == "speed":
         if data > 1000000:
             result = str(round(data / 1000000, 2)) + " M/S"
         elif data > 1000:
             result = str(round(data / 1000, 2)) + " K/S"
         else:
-            result = str(round(data, 2)) + "/s"
+            result = str(int(data)) + "/s"
     elif mode == "elapsed":
-        if data > 0.001:
-            result = str(round(data, 3)) + "s"
-        elif data > 1e-6:
-            result = str(int(data * 1e6)) + "ms"
+        if data >= 1:
+            result = str(round(data, 2)) + "s"
+        if data >= 1e-3:
+            result = str(round(data * 1e3, 1)) + "ms"
+        elif data >= 1e-6:
+            result = str(round(data * 1e6, 1)) + "us"
         else:
-            result = str(int(data * 1e9)) + "ns"
+            result = str(round(data * 1e9, 1)) + "ns"
     return result
 
 
-def vfunc(func, args, mode="speed"):
-    stat = []
+def vfunc(func, args=(), mode="speed"):
+
+    if mode not in ["speed", "elapsed"]:
+        print("'mode' parameter can only value as 'speed' or 'elapsed'.")
+        return False
 
-    for i in range(10):
-        count = pow(10, i)
+    try:
         start_time = timer()
-        for i in range(count):
-            func(*args)
+        func(*args)
         run_time = timer() - start_time
+    except:
+        print("Errors found in the function under test.")
+        return False
+
+    try:
+        count = int(1 / run_time) + 1
+    except ZeroDivisionError:
+        count = 1e9
 
-        if run_time > 0.01:
-            if run_time > 1:
-                count = 1
-            else:
-                count = int(1 / run_time * count)
-            break
+    stat = []
 
     while True:
         start_time = timer()
         for i in range(count):
             func(*args)
-
         run_time = timer() - start_time
 
         if mode == "speed":
             stat.append(count / run_time)
         else:
             stat.append(run_time / count)
 
-        result = conv(sum(stat) / len(stat), mode)
+        result = convert(stat[-1], mode)
+        avg = convert(sum(stat) / len(stat), mode)
 
         print(" " * 45, end="\r")
         print(result)
-        print("repeat: {}  ".format(len(stat)), "avg = {}".format(result), end="\r")
+        print("repeat: {}  ".format(len(stat)), "average = {}".format(avg), end="\r")
+
```

### Comparing `vfunc-0.1.2/LICENSE` & `vfunc-0.1.3/LICENSE`

 * *Files identical despite different names*


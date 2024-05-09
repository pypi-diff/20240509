# Comparing `tmp/taguchi-1.0.0.tar.gz` & `tmp/taguchi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taguchi-1.0.0.tar", last modified: Thu May  9 03:01:09 2024, max compression
+gzip compressed data, was "taguchi-1.0.1.tar", last modified: Thu May  9 03:36:10 2024, max compression
```

## Comparing `taguchi-1.0.0.tar` & `taguchi-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:01:09.253557 taguchi-1.0.0/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-09 03:01:09.252557 taguchi-1.0.0/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      587 2024-05-04 04:32:49.000000 taguchi-1.0.0/README.md
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.0.0/pyproject.toml
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-09 03:01:09.255557 taguchi-1.0.0/setup.cfg
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:01:09.250557 taguchi-1.0.0/taguchi/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-09 02:43:51.000000 taguchi-1.0.0/taguchi/__init__.py
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     2648 2024-05-09 02:59:55.000000 taguchi-1.0.0/taguchi/__main__.py
-drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:01:09.252557 taguchi-1.0.0/taguchi.egg-info/
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)     1016 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/PKG-INFO
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)      262 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/entry_points.txt
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.0.0/taguchi.egg-info/not-zip-safe
--rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-09 03:01:09.000000 taguchi-1.0.0/taguchi.egg-info/top_level.txt
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:36:10.919045 taguchi-1.0.1/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-09 03:36:10.918045 taguchi-1.0.1/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     3786 2024-05-09 03:35:22.000000 taguchi-1.0.1/README.md
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      103 2024-05-04 04:45:54.000000 taguchi-1.0.1/pyproject.toml
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      757 2024-05-09 03:36:10.921045 taguchi-1.0.1/setup.cfg
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:36:10.917045 taguchi-1.0.1/taguchi/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       17 2024-05-09 03:20:19.000000 taguchi-1.0.1/taguchi/__init__.py
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     2721 2024-05-09 03:20:06.000000 taguchi-1.0.1/taguchi/__main__.py
+drwxr-xr-x   0 jcranney  (1000) jcranney  (1000)        0 2024-05-09 03:36:10.918045 taguchi-1.0.1/taguchi.egg-info/
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)     4216 2024-05-09 03:36:10.000000 taguchi-1.0.1/taguchi.egg-info/PKG-INFO
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)      262 2024-05-09 03:36:10.000000 taguchi-1.0.1/taguchi.egg-info/SOURCES.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-09 03:36:10.000000 taguchi-1.0.1/taguchi.egg-info/dependency_links.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)       54 2024-05-09 03:36:10.000000 taguchi-1.0.1/taguchi.egg-info/entry_points.txt
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        1 2024-05-04 04:46:44.000000 taguchi-1.0.1/taguchi.egg-info/not-zip-safe
+-rw-r--r--   0 jcranney  (1000) jcranney  (1000)        8 2024-05-09 03:36:10.000000 taguchi-1.0.1/taguchi.egg-info/top_level.txt
```

### Comparing `taguchi-1.0.0/setup.cfg` & `taguchi-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `taguchi-1.0.0/taguchi/__main__.py` & `taguchi-1.0.1/taguchi/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,17 +60,21 @@
 for experiment in array:
     for param,state in zip(params,experiment):
         os.environ[param] = str(a[param][state])
         if verbose:
             print(param,state)
     proc = subprocess.Popen(command, stdout=subprocess.PIPE, shell=True)
     (out, err) = proc.communicate()
+    if err is not None:
+        print(err.decode())
+        exit(1)
     if verbose > 1:
         print(out.decode())
         print(err)
+    
     out = out.decode().split("\n")
     result = None
     for o in out:
         try:
             result = float(o)
             if verbose:
                 print(f"{result=}\n")
```


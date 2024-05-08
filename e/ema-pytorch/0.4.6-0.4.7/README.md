# Comparing `tmp/ema_pytorch-0.4.6.tar.gz` & `tmp/ema_pytorch-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ema_pytorch-0.4.6.tar", last modified: Mon May  6 14:35:42 2024, max compression
+gzip compressed data, was "ema_pytorch-0.4.7.tar", last modified: Wed May  8 22:12:18 2024, max compression
```

## Comparing `ema_pytorch-0.4.6.tar` & `ema_pytorch-0.4.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/ema_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/ema_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/ema_pytorch/ema_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/ema_pytorch/post_hoc_ema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/ema_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 14:35:42.000000 ema_pytorch-0.4.6/ema_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:35:42.609905 ema_pytorch-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-06 14:35:36.000000 ema_pytorch-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:12:18.072430 ema_pytorch-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 22:12:14.000000 ema_pytorch-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-08 22:12:18.068430 ema_pytorch-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-08 22:12:14.000000 ema_pytorch-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:12:18.068430 ema_pytorch-0.4.7/ema_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-08 22:12:14.000000 ema_pytorch-0.4.7/ema_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8326 2024-05-08 22:12:14.000000 ema_pytorch-0.4.7/ema_pytorch/ema_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-08 22:12:14.000000 ema_pytorch-0.4.7/ema_pytorch/post_hoc_ema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:12:18.068430 ema_pytorch-0.4.7/ema_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-08 22:12:18.000000 ema_pytorch-0.4.7/ema_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-08 22:12:18.000000 ema_pytorch-0.4.7/ema_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:12:18.000000 ema_pytorch-0.4.7/ema_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 22:12:18.000000 ema_pytorch-0.4.7/ema_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 22:12:18.000000 ema_pytorch-0.4.7/ema_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:12:18.072430 ema_pytorch-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-08 22:12:14.000000 ema_pytorch-0.4.7/setup.py
```

### Comparing `ema_pytorch-0.4.6/LICENSE` & `ema_pytorch-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ema_pytorch-0.4.6/PKG-INFO` & `ema_pytorch-0.4.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ema-pytorch
-Version: 0.4.6
+Version: 0.4.7
 Summary: Easy way to keep track of exponential moving average version of your pytorch module
 Home-page: https://github.com/lucidrains/ema-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,exponential moving average
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ema_pytorch-0.4.6/README.md` & `ema_pytorch-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `ema_pytorch-0.4.6/ema_pytorch/ema_pytorch.py` & `ema_pytorch-0.4.7/ema_pytorch/ema_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,16 @@
             try:
                 self.ema_model = deepcopy(model)
             except Exception as e:
                 print(f'Error: While trying to deepcopy model: {e}')
                 print('Your model was not copyable. Please make sure you are not using any LazyLinear')
                 exit()
 
-        self.ema_model.requires_grad_(False)
+        for p in self.ema_model.parameters():
+            p.detach_()
 
         # parameter and buffer names
 
         self.parameter_names = {name for name, param in self.ema_model.named_parameters() if torch.is_floating_point(param) or torch.is_complex(param)}
         self.buffer_names = {name for name, buffer in self.ema_model.named_buffers() if torch.is_floating_point(buffer) or torch.is_complex(buffer)}
 
         # tensor update functions
```

### Comparing `ema_pytorch-0.4.6/ema_pytorch/post_hoc_ema.py` & `ema_pytorch-0.4.7/ema_pytorch/post_hoc_ema.py`

 * *Files identical despite different names*

### Comparing `ema_pytorch-0.4.6/ema_pytorch.egg-info/PKG-INFO` & `ema_pytorch-0.4.7/ema_pytorch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ema-pytorch
-Version: 0.4.6
+Version: 0.4.7
 Summary: Easy way to keep track of exponential moving average version of your pytorch module
 Home-page: https://github.com/lucidrains/ema-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,exponential moving average
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ema_pytorch-0.4.6/setup.py` & `ema_pytorch-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ema-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.4.6',
+  version = '0.4.7',
   license='MIT',
   description = 'Easy way to keep track of exponential moving average version of your pytorch module',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ema-pytorch',
   keywords = [
```


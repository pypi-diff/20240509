# Comparing `tmp/flameengine-0.0.4.tar.gz` & `tmp/flameengine-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flameengine-0.0.4.tar", last modified: Tue May  7 17:51:04 2024, max compression
+gzip compressed data, was "flameengine-0.0.4.1.tar", last modified: Wed May  8 11:55:09 2024, max compression
```

## Comparing `flameengine-0.0.4.tar` & `flameengine-0.0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 17:51:04.005786 flameengine-0.0.4/
--rw-rw-rw-   0        0        0      618 2024-05-07 17:51:04.004996 flameengine-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 17:51:03.998296 flameengine-0.0.4/flameEngine/
--rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4/flameEngine/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4/flameEngine/example.py
--rw-rw-rw-   0        0        0    43279 2024-05-07 17:16:46.000000 flameengine-0.0.4/flameEngine/flame.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:51:04.003276 flameengine-0.0.4/flameEngine.egg-info/
--rw-rw-rw-   0        0        0      618 2024-05-07 17:51:03.000000 flameengine-0.0.4/flameEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-07 17:51:03.000000 flameengine-0.0.4/flameEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 17:51:03.000000 flameengine-0.0.4/flameEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-07 17:51:03.000000 flameengine-0.0.4/flameEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4/license.txt
--rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 17:51:04.005786 flameengine-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      943 2024-05-07 17:50:59.000000 flameengine-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:55:09.896280 flameengine-0.0.4.1/
+-rw-rw-rw-   0        0        0      620 2024-05-08 11:55:09.895279 flameengine-0.0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 11:55:09.887759 flameengine-0.0.4.1/flameEngine/
+-rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.1/flameEngine/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.1/flameEngine/example.py
+-rw-rw-rw-   0        0        0    43212 2024-05-08 11:54:29.000000 flameengine-0.0.4.1/flameEngine/flame.py
+drwxrwxrwx   0        0        0        0 2024-05-08 11:55:09.894278 flameengine-0.0.4.1/flameEngine.egg-info/
+-rw-rw-rw-   0        0        0      620 2024-05-08 11:55:09.000000 flameengine-0.0.4.1/flameEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-08 11:55:09.000000 flameengine-0.0.4.1/flameEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 11:55:09.000000 flameengine-0.0.4.1/flameEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-08 11:55:09.000000 flameengine-0.0.4.1/flameEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.1/license.txt
+-rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 11:55:09.896280 flameengine-0.0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      945 2024-05-08 11:54:55.000000 flameengine-0.0.4.1/setup.py
```

### Comparing `flameengine-0.0.4/PKG-INFO` & `flameengine-0.0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4/flameEngine/example.py` & `flameengine-0.0.4.1/flameEngine/example.py`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4/flameEngine/flame.py` & `flameengine-0.0.4.1/flameEngine/flame.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,20 +361,18 @@
 
         return torch.clamp(torch.stack((red, green, blue), dim=2), 0, 255), self.alpha
 
     # w1(x) = w0(x) + dt * f(x,t)
     # Dynamic fuel_density addition
     def add_fuel_density(self, x, x0, dt, step):
         # TODO: add fuel density with outside predefined fuel_density structure and behavior
-        if step < 500:
-            x0[self.idx,self.idy] += (1.808 + 2.48)  # Note :  propane + butane kg/m3
-            x[self.idx,self.idy] += \
-                dt * x0[self.idx,self.idy]
-        else:
-            pass
+
+        x0[self.idx,self.idy] += (1.808 + 2.48)  # Note :  propane + butane kg/m3
+        x[self.idx,self.idy] += \
+            dt * x0[self.idx,self.idy]
         return x, x0
 
     def add_oxidiser_density(self, x, x0, dt, step):
         # air density 1.225 kg/m3
         xmean = x0[self.N_boundary:self.grid_size_x - self.N_boundary,
                 self.N_boundary:self.grid_size_y - self.N_boundary].mean()
         # xx = torch.zeros_like(x0[N_boundary:grid_size_x, N_boundary:grid_size_y],device=device)
```

### Comparing `flameengine-0.0.4/flameEngine.egg-info/PKG-INFO` & `flameengine-0.0.4.1/flameEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4/license.txt` & `flameengine-0.0.4.1/license.txt`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4/setup.py` & `flameengine-0.0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.4.1'
 DESCRIPTION = 'Flame simulation package'
 LONG_DESCRIPTION = 'Simulation engine implementation of stable fluids with extra steps for dataset generation in neural network env and test'
 
 setup(
     name="flameEngine",
     version=VERSION,
     author="Piotr Mikolajczyk",
```


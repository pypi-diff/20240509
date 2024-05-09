# Comparing `tmp/flameengine-0.0.4.33.tar.gz` & `tmp/flameengine-0.0.4.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flameengine-0.0.4.33.tar", last modified: Thu May  9 11:45:34 2024, max compression
+gzip compressed data, was "flameengine-0.0.4.34.tar", last modified: Thu May  9 11:47:00 2024, max compression
```

## Comparing `flameengine-0.0.4.33.tar` & `flameengine-0.0.4.34.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:45:34.449864 flameengine-0.0.4.33/
--rw-rw-rw-   0        0        0      621 2024-05-09 11:45:34.448610 flameengine-0.0.4.33/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.33/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 11:45:34.442104 flameengine-0.0.4.33/flameEngine/
--rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.33/flameEngine/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.33/flameEngine/example.py
--rw-rw-rw-   0        0        0    47303 2024-05-09 11:43:51.000000 flameengine-0.0.4.33/flameEngine/flame.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:45:34.447610 flameengine-0.0.4.33/flameEngine.egg-info/
--rw-rw-rw-   0        0        0      621 2024-05-09 11:45:34.000000 flameengine-0.0.4.33/flameEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-09 11:45:34.000000 flameengine-0.0.4.33/flameEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:45:34.000000 flameengine-0.0.4.33/flameEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 11:45:34.000000 flameengine-0.0.4.33/flameEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.33/license.txt
--rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.33/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 11:45:34.450868 flameengine-0.0.4.33/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-05-09 11:45:18.000000 flameengine-0.0.4.33/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:47:00.926597 flameengine-0.0.4.34/
+-rw-rw-rw-   0        0        0      621 2024-05-09 11:47:00.925533 flameengine-0.0.4.34/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.34/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 11:47:00.919261 flameengine-0.0.4.34/flameEngine/
+-rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.34/flameEngine/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.34/flameEngine/example.py
+-rw-rw-rw-   0        0        0    47303 2024-05-09 11:46:29.000000 flameengine-0.0.4.34/flameEngine/flame.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:47:00.924388 flameengine-0.0.4.34/flameEngine.egg-info/
+-rw-rw-rw-   0        0        0      621 2024-05-09 11:47:00.000000 flameengine-0.0.4.34/flameEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-09 11:47:00.000000 flameengine-0.0.4.34/flameEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 11:47:00.000000 flameengine-0.0.4.34/flameEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 11:47:00.000000 flameengine-0.0.4.34/flameEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.34/license.txt
+-rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.34/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 11:47:00.926597 flameengine-0.0.4.34/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-05-09 11:46:54.000000 flameengine-0.0.4.34/setup.py
```

### Comparing `flameengine-0.0.4.33/PKG-INFO` & `flameengine-0.0.4.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.33
+Version: 0.0.4.34
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.33/flameEngine/example.py` & `flameengine-0.0.4.34/flameEngine/example.py`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.33/flameEngine/flame.py` & `flameengine-0.0.4.34/flameEngine/flame.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,13 +849,13 @@
                 self.update_grid(self.fuel_density, self.fuel_density_prev,
                                  self.oxidizer_density, self.oxidizer_density_prev,
                                  self.product_density, self.product_density_prev, self.u,
                                  self.u_prev, self.v,
                                  self.v_prev, self.pressure, self.temperature, self.temperature_prev,
                                  self.mass_fuel, self.mass_oxidizer, self.mass_product,
                                  self.poisson_v_term, self.dt,
-                                 self.viscosity, self.diff, i)
+                                 self.viscosity, self.diff, 0)
         torch.cuda.empty_cache()
         import sys
         sys.modules[__name__].__dict__.clear()
         import gc
         gc.collect()
```

### Comparing `flameengine-0.0.4.33/flameEngine.egg-info/PKG-INFO` & `flameengine-0.0.4.34/flameEngine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.33
+Version: 0.0.4.34
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.33/license.txt` & `flameengine-0.0.4.34/license.txt`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.33/setup.py` & `flameengine-0.0.4.34/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4.33'
+VERSION = '0.0.4.34'
 DESCRIPTION = 'Flame simulation package'
 LONG_DESCRIPTION = 'Simulation engine implementation of stable fluids with extra steps for dataset generation in neural network env and test'
 
 setup(
     name="flameEngine",
     version=VERSION,
     author="Piotr Mikolajczyk",
```


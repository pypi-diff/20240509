# Comparing `tmp/flameengine-0.0.4.2.tar.gz` & `tmp/flameengine-0.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flameengine-0.0.4.2.tar", last modified: Thu May  9 09:51:19 2024, max compression
+gzip compressed data, was "flameengine-0.0.4.3.tar", last modified: Thu May  9 10:59:15 2024, max compression
```

## Comparing `flameengine-0.0.4.2.tar` & `flameengine-0.0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 09:51:19.963622 flameengine-0.0.4.2/
--rw-rw-rw-   0        0        0      620 2024-05-09 09:51:19.962013 flameengine-0.0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 09:51:19.953905 flameengine-0.0.4.2/flameEngine/
--rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.2/flameEngine/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.2/flameEngine/example.py
--rw-rw-rw-   0        0        0    43372 2024-05-09 09:50:45.000000 flameengine-0.0.4.2/flameEngine/flame.py
-drwxrwxrwx   0        0        0        0 2024-05-09 09:51:19.961021 flameengine-0.0.4.2/flameEngine.egg-info/
--rw-rw-rw-   0        0        0      620 2024-05-09 09:51:19.000000 flameengine-0.0.4.2/flameEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-09 09:51:19.000000 flameengine-0.0.4.2/flameEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 09:51:19.000000 flameengine-0.0.4.2/flameEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 09:51:19.000000 flameengine-0.0.4.2/flameEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.2/license.txt
--rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 09:51:19.963622 flameengine-0.0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      945 2024-05-09 09:51:07.000000 flameengine-0.0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:59:15.383227 flameengine-0.0.4.3/
+-rw-rw-rw-   0        0        0      620 2024-05-09 10:59:15.382228 flameengine-0.0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 10:59:15.375843 flameengine-0.0.4.3/flameEngine/
+-rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.3/flameEngine/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.3/flameEngine/example.py
+-rw-rw-rw-   0        0        0    43514 2024-05-09 10:57:44.000000 flameengine-0.0.4.3/flameEngine/flame.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:59:15.381228 flameengine-0.0.4.3/flameEngine.egg-info/
+-rw-rw-rw-   0        0        0      620 2024-05-09 10:59:15.000000 flameengine-0.0.4.3/flameEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-09 10:59:15.000000 flameengine-0.0.4.3/flameEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 10:59:15.000000 flameengine-0.0.4.3/flameEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 10:59:15.000000 flameengine-0.0.4.3/flameEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.3/license.txt
+-rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 10:59:15.383227 flameengine-0.0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      945 2024-05-09 10:58:44.000000 flameengine-0.0.4.3/setup.py
```

### Comparing `flameengine-0.0.4.2/PKG-INFO` & `flameengine-0.0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.2
+Version: 0.0.4.3
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.2/flameEngine/example.py` & `flameengine-0.0.4.3/flameEngine/example.py`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.2/flameEngine/flame.py` & `flameengine-0.0.4.3/flameEngine/flame.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         self.PE_fuel_oxidizer_butane = 2657 * 1e3 / self.avogardo
         self.PE_total = (self.PE_fuel_oxidizer_propane + self.PE_fuel_oxidizer_butane) / 2
 
         self.Su_propane_butane_burning_velocity = 38.3 * 1e-2
         self.grid_unit_volume = 1
 
         self.igni_time = 75
+        self.fuel_cut_off_time = int(self.no_frames/2)
         self.d_low_fuel = d_low_fuel_c
         self.d_high_fuel = d_high_fuel_c
         self.d_low_oxidizer = d_low_oxidizer_c
         self.d_high_oxidizer = d_high_oxidizer_c
         self.th_point_c = th_point_c  # KELVINS
 
         self.d_low_product_r_c = d_low_product_r_c
@@ -366,18 +367,20 @@
 
         return torch.clamp(torch.stack((red, green, blue), dim=2), 0, 255), self.alpha
 
     # w1(x) = w0(x) + dt * f(x,t)
     # Dynamic fuel_density addition
     def add_fuel_density(self, x, x0, dt, step):
         # TODO: add fuel density with outside predefined fuel_density structure and behavior
-
-        x0[self.idx,self.idy] += self.fuel_density_m3*self.fuel_dens_modifier
-        x[self.idx,self.idy] += \
-            dt * x0[self.idx,self.idy]
+        if step < self.fuel_cut_off_time:
+            x0[self.idx,self.idy] += self.fuel_density_m3*self.fuel_dens_modifier
+            x[self.idx,self.idy] += \
+                dt * x0[self.idx,self.idy]
+        else:
+            pass
         return x, x0
 
     def add_oxidiser_density(self, x, x0, dt, step):
         # air density 1.225 kg/m3
         xmean = x0[self.N_boundary:self.grid_size_x - self.N_boundary,
                 self.N_boundary:self.grid_size_y - self.N_boundary].mean()
         # xx = torch.zeros_like(x0[N_boundary:grid_size_x, N_boundary:grid_size_y],device=device)
```

### Comparing `flameengine-0.0.4.2/flameEngine.egg-info/PKG-INFO` & `flameengine-0.0.4.3/flameEngine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.2
+Version: 0.0.4.3
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.2/license.txt` & `flameengine-0.0.4.3/license.txt`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.2/setup.py` & `flameengine-0.0.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4.2'
+VERSION = '0.0.4.3'
 DESCRIPTION = 'Flame simulation package'
 LONG_DESCRIPTION = 'Simulation engine implementation of stable fluids with extra steps for dataset generation in neural network env and test'
 
 setup(
     name="flameEngine",
     version=VERSION,
     author="Piotr Mikolajczyk",
```


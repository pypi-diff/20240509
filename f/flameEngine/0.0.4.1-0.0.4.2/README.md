# Comparing `tmp/flameengine-0.0.4.1.tar.gz` & `tmp/flameengine-0.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flameengine-0.0.4.1.tar", last modified: Wed May  8 11:55:09 2024, max compression
+gzip compressed data, was "flameengine-0.0.4.2.tar", last modified: Thu May  9 09:51:19 2024, max compression
```

## Comparing `flameengine-0.0.4.1.tar` & `flameengine-0.0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 11:55:09.896280 flameengine-0.0.4.1/
--rw-rw-rw-   0        0        0      620 2024-05-08 11:55:09.895279 flameengine-0.0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 11:55:09.887759 flameengine-0.0.4.1/flameEngine/
--rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.1/flameEngine/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.1/flameEngine/example.py
--rw-rw-rw-   0        0        0    43212 2024-05-08 11:54:29.000000 flameengine-0.0.4.1/flameEngine/flame.py
-drwxrwxrwx   0        0        0        0 2024-05-08 11:55:09.894278 flameengine-0.0.4.1/flameEngine.egg-info/
--rw-rw-rw-   0        0        0      620 2024-05-08 11:55:09.000000 flameengine-0.0.4.1/flameEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-08 11:55:09.000000 flameengine-0.0.4.1/flameEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 11:55:09.000000 flameengine-0.0.4.1/flameEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-08 11:55:09.000000 flameengine-0.0.4.1/flameEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.1/license.txt
--rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 11:55:09.896280 flameengine-0.0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      945 2024-05-08 11:54:55.000000 flameengine-0.0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:51:19.963622 flameengine-0.0.4.2/
+-rw-rw-rw-   0        0        0      620 2024-05-09 09:51:19.962013 flameengine-0.0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 09:51:19.953905 flameengine-0.0.4.2/flameEngine/
+-rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.2/flameEngine/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.2/flameEngine/example.py
+-rw-rw-rw-   0        0        0    43372 2024-05-09 09:50:45.000000 flameengine-0.0.4.2/flameEngine/flame.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:51:19.961021 flameengine-0.0.4.2/flameEngine.egg-info/
+-rw-rw-rw-   0        0        0      620 2024-05-09 09:51:19.000000 flameengine-0.0.4.2/flameEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-09 09:51:19.000000 flameengine-0.0.4.2/flameEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 09:51:19.000000 flameengine-0.0.4.2/flameEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 09:51:19.000000 flameengine-0.0.4.2/flameEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.2/license.txt
+-rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 09:51:19.963622 flameengine-0.0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      945 2024-05-09 09:51:07.000000 flameengine-0.0.4.2/setup.py
```

### Comparing `flameengine-0.0.4.1/PKG-INFO` & `flameengine-0.0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.1
+Version: 0.0.4.2
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.1/flameEngine/example.py` & `flameengine-0.0.4.2/flameEngine/example.py`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.1/flameEngine/flame.py` & `flameengine-0.0.4.2/flameEngine/flame.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,16 @@
                  th_point_c=273. + 400.,
                  d_low_product_r_c=1e-3,
                  d_high_product_r_c=1e1,
                  th_point_r_c=273. + 200.,
                  d_low_product_r_h=1e1,
                  d_high_product_r_h=20.,
                  th_point_r_h=273. + 400.):
+
+
         torch.cuda.synchronize()
         matplotlib.use('TkAgg')
         plt.style.use('dark_background')
         # CUDA_LAUNCH_BLOCKING = 1
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.no_frames = no_frames
         self.frame_skip = frame_skip
@@ -66,23 +68,26 @@
         self.no_of_carbon_dioxide_butane = 4
         self.no_of_h2o_propane = 4
         self.no_of_h2o_butane = 5
         self.no_of_co2 = self.no_of_carbon_dioxide_propane + self.no_of_carbon_dioxide_butane
         self.no_oxygen = self.no_of_oxygn_in_the_reaction_for_propane + self.no_of_oxygn_in_the_reaction_for_butane
         self.no_of_h2o = self.no_of_h2o_propane + self.no_of_h2o_butane
         self.fuel_molecular_mass = self.propane_molecular_mass + self.butane_molecular_mass
+        self.fuel_density_m3 = (1.808 + 2.48)  # Note :  propane + butane kg/m3
+        self.fuel_dens_modifier = 1.
         self.oxidizer_molecular_mass = 2 * self.oxygen_molecular_mass * self.no_oxygen
         self.product_molecular_mass = self.co2_molecular_mass * self.no_of_co2 + self.h2o_molecular_mass * self.no_of_h2o
         self.PE_fuel_oxidizer_propane = 2219.9 * 1e3 / self.avogardo
         self.PE_fuel_oxidizer_butane = 2657 * 1e3 / self.avogardo
         self.PE_total = (self.PE_fuel_oxidizer_propane + self.PE_fuel_oxidizer_butane) / 2
 
         self.Su_propane_butane_burning_velocity = 38.3 * 1e-2
         self.grid_unit_volume = 1
 
+        self.igni_time = 75
         self.d_low_fuel = d_low_fuel_c
         self.d_high_fuel = d_high_fuel_c
         self.d_low_oxidizer = d_low_oxidizer_c
         self.d_high_oxidizer = d_high_oxidizer_c
         self.th_point_c = th_point_c  # KELVINS
 
         self.d_low_product_r_c = d_low_product_r_c
@@ -211,15 +216,15 @@
         zero_mask = numerator_mask & denominator_mask
         result = torch.zeros_like(numerator, device=self.device)
         result[~zero_mask] = numerator[~zero_mask] / denominator[~zero_mask]
         return result
 
     def ignite(self, temperature, step):
         ignite_temp = 273. + 10300.  # Note: lighter temperature (273. + 1300.)
-        if step > 75:
+        if step > self.igni_time:
             pass
         else:
             temperature[self.idx,self.idy] = ignite_temp
         return temperature
 
     def combustion(self, fuel_density, oxidizer_density, product_density,
                    u, v, temperature, step):
@@ -362,15 +367,15 @@
         return torch.clamp(torch.stack((red, green, blue), dim=2), 0, 255), self.alpha
 
     # w1(x) = w0(x) + dt * f(x,t)
     # Dynamic fuel_density addition
     def add_fuel_density(self, x, x0, dt, step):
         # TODO: add fuel density with outside predefined fuel_density structure and behavior
 
-        x0[self.idx,self.idy] += (1.808 + 2.48)  # Note :  propane + butane kg/m3
+        x0[self.idx,self.idy] += self.fuel_density_m3*self.fuel_dens_modifier
         x[self.idx,self.idy] += \
             dt * x0[self.idx,self.idy]
         return x, x0
 
     def add_oxidiser_density(self, x, x0, dt, step):
         # air density 1.225 kg/m3
         xmean = x0[self.N_boundary:self.grid_size_x - self.N_boundary,
```

### Comparing `flameengine-0.0.4.1/flameEngine.egg-info/PKG-INFO` & `flameengine-0.0.4.2/flameEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.1
+Version: 0.0.4.2
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.1/license.txt` & `flameengine-0.0.4.2/license.txt`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.1/setup.py` & `flameengine-0.0.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4.1'
+VERSION = '0.0.4.2'
 DESCRIPTION = 'Flame simulation package'
 LONG_DESCRIPTION = 'Simulation engine implementation of stable fluids with extra steps for dataset generation in neural network env and test'
 
 setup(
     name="flameEngine",
     version=VERSION,
     author="Piotr Mikolajczyk",
```


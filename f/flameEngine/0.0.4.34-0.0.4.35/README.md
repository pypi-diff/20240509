# Comparing `tmp/flameengine-0.0.4.34.tar.gz` & `tmp/flameengine-0.0.4.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flameengine-0.0.4.34.tar", last modified: Thu May  9 11:47:00 2024, max compression
+gzip compressed data, was "flameengine-0.0.4.35.tar", last modified: Thu May  9 12:13:57 2024, max compression
```

## Comparing `flameengine-0.0.4.34.tar` & `flameengine-0.0.4.35.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:47:00.926597 flameengine-0.0.4.34/
--rw-rw-rw-   0        0        0      621 2024-05-09 11:47:00.925533 flameengine-0.0.4.34/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.34/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 11:47:00.919261 flameengine-0.0.4.34/flameEngine/
--rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.34/flameEngine/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.34/flameEngine/example.py
--rw-rw-rw-   0        0        0    47303 2024-05-09 11:46:29.000000 flameengine-0.0.4.34/flameEngine/flame.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:47:00.924388 flameengine-0.0.4.34/flameEngine.egg-info/
--rw-rw-rw-   0        0        0      621 2024-05-09 11:47:00.000000 flameengine-0.0.4.34/flameEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-09 11:47:00.000000 flameengine-0.0.4.34/flameEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:47:00.000000 flameengine-0.0.4.34/flameEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 11:47:00.000000 flameengine-0.0.4.34/flameEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.34/license.txt
--rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.34/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 11:47:00.926597 flameengine-0.0.4.34/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-05-09 11:46:54.000000 flameengine-0.0.4.34/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:13:57.642161 flameengine-0.0.4.35/
+-rw-rw-rw-   0        0        0      621 2024-05-09 12:13:57.641120 flameengine-0.0.4.35/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.35/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 12:13:57.634768 flameengine-0.0.4.35/flameEngine/
+-rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.35/flameEngine/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.35/flameEngine/example.py
+-rw-rw-rw-   0        0        0    47376 2024-05-09 12:13:28.000000 flameengine-0.0.4.35/flameEngine/flame.py
+drwxrwxrwx   0        0        0        0 2024-05-09 12:13:57.640224 flameengine-0.0.4.35/flameEngine.egg-info/
+-rw-rw-rw-   0        0        0      621 2024-05-09 12:13:57.000000 flameengine-0.0.4.35/flameEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-09 12:13:57.000000 flameengine-0.0.4.35/flameEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 12:13:57.000000 flameengine-0.0.4.35/flameEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 12:13:57.000000 flameengine-0.0.4.35/flameEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.35/license.txt
+-rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.35/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 12:13:57.642161 flameengine-0.0.4.35/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-05-09 12:13:43.000000 flameengine-0.0.4.35/setup.py
```

### Comparing `flameengine-0.0.4.34/PKG-INFO` & `flameengine-0.0.4.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.34
+Version: 0.0.4.35
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.34/flameEngine/example.py` & `flameengine-0.0.4.35/flameEngine/example.py`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.34/flameEngine/flame.py` & `flameengine-0.0.4.35/flameEngine/flame.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                  d_high_product_r_c=1e1,
                  th_point_r_c=273. + 200.,
                  d_low_product_r_h=1e1,
                  d_high_product_r_h=20.,
                  th_point_r_h=273. + 400.):
 
 
+
         torch.cuda.synchronize()
         matplotlib.use('TkAgg')
         plt.style.use('dark_background')
         # CUDA_LAUNCH_BLOCKING = 1
         self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.no_frames = no_frames
         self.frame_skip = frame_skip
@@ -82,14 +83,15 @@
         self.PE_fuel_oxidizer_butane = 2657 * 1e3 / self.avogardo
         self.PE_total = (self.PE_fuel_oxidizer_propane + self.PE_fuel_oxidizer_butane) / 2
 
         self.Su_propane_butane_burning_velocity = 38.3 * 1e-2
         self.grid_unit_volume = 1
 
         self.igni_time = 75
+        self.ignition_temp = 273. + 10300.  # Note: lighter temperature (273. + 1300.)
         self.fuel_cut_off_time = int(self.no_frames/2)
         self.d_low_fuel = d_low_fuel_c
         self.d_high_fuel = d_high_fuel_c
         self.d_low_oxidizer = d_low_oxidizer_c
         self.d_high_oxidizer = d_high_oxidizer_c
         self.th_point_c = th_point_c  # KELVINS
 
@@ -218,19 +220,18 @@
         denominator_mask = torch.abs(denominator) <= eps
         zero_mask = numerator_mask & denominator_mask
         result = torch.zeros_like(numerator, device=self.device)
         result[~zero_mask] = numerator[~zero_mask] / denominator[~zero_mask]
         return result
 
     def ignite(self, temperature, step):
-        ignite_temp = 273. + 10300.  # Note: lighter temperature (273. + 1300.)
         if step > self.igni_time:
             pass
         else:
-            temperature[self.idx,self.idy] = ignite_temp
+            temperature[self.idx,self.idy] = self.ignition_temp
         return temperature
 
     def combustion(self, fuel_density, oxidizer_density, product_density,
                    u, v, temperature, step):
         temperature += self.ignite(temperature, step)
         density_treshold_unburned_fuel = ((fuel_density >= self.d_low_fuel) & (fuel_density <= self.d_high_fuel))
         density_treshold_unburned_oxizdizer = (
@@ -649,15 +650,15 @@
             temperature, temperature_prev, \
             mass_fuel, mass_oxidizer, mass_product, \
             poisson_v_term, rgb, alpha
 
     def save_results(self, step, save_v=0, save_u=0, save_vu_mag=0, save_fuel=0, save_oxidizer=0,
                      save_product=0, save_pressure=0, save_temperature=0, save_rgb=0, save_alpha=0,delete_data=0):
         if step % self.frame_skip == 0 or step == 0:
-            meta_data = torch.tensor([step,self.fuel_initial_speed,self.grid_size_x,self.grid_size_y,self.N_boundary,self.size_x,
+            meta_data = torch.tensor([step,self.fuel_initial_speed,self.fuel_cut_off_time,self.igni_time,self.ignition_temp,self.grid_size_x,self.grid_size_y,self.N_boundary,self.size_x,
                           self.size_y,self.dx,self.dy,self.dt,self.degrees_of_freedom,
                           self.viscosity,self.diff,self.gravity,self.gravity_divider,
                           self.fuel_molecular_mass,self.oxidizer_molecular_mass,self.product_molecular_mass,
                           self.grid_unit_volume,self.d_low_fuel,self.d_high_fuel,self.d_low_oxidizer,
                           self.d_high_oxidizer,self.th_point_c,self.d_low_product_r_c,self.d_high_product_r_c,self.th_point_r_c,
                           self.d_low_product_r_h,self.d_high_product_r_h,self.th_point_r_h,self.low_alpha,self.high_alpha,self.alpha_decay])
             if save_v == 1:
```

### Comparing `flameengine-0.0.4.34/flameEngine.egg-info/PKG-INFO` & `flameengine-0.0.4.35/flameEngine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.34
+Version: 0.0.4.35
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.34/license.txt` & `flameengine-0.0.4.35/license.txt`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.34/setup.py` & `flameengine-0.0.4.35/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4.34'
+VERSION = '0.0.4.35'
 DESCRIPTION = 'Flame simulation package'
 LONG_DESCRIPTION = 'Simulation engine implementation of stable fluids with extra steps for dataset generation in neural network env and test'
 
 setup(
     name="flameEngine",
     version=VERSION,
     author="Piotr Mikolajczyk",
```


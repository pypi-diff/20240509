# Comparing `tmp/flameengine-0.0.4.31.tar.gz` & `tmp/flameengine-0.0.4.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flameengine-0.0.4.31.tar", last modified: Thu May  9 11:27:52 2024, max compression
+gzip compressed data, was "flameengine-0.0.4.32.tar", last modified: Thu May  9 11:30:36 2024, max compression
```

## Comparing `flameengine-0.0.4.31.tar` & `flameengine-0.0.4.32.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:27:52.201154 flameengine-0.0.4.31/
--rw-rw-rw-   0        0        0      621 2024-05-09 11:27:52.200154 flameengine-0.0.4.31/PKG-INFO
--rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.31/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 11:27:52.191456 flameengine-0.0.4.31/flameEngine/
--rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.31/flameEngine/__init__.py
--rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.31/flameEngine/example.py
--rw-rw-rw-   0        0        0    45250 2024-05-09 11:26:21.000000 flameengine-0.0.4.31/flameEngine/flame.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:27:52.198148 flameengine-0.0.4.31/flameEngine.egg-info/
--rw-rw-rw-   0        0        0      621 2024-05-09 11:27:52.000000 flameengine-0.0.4.31/flameEngine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-05-09 11:27:52.000000 flameengine-0.0.4.31/flameEngine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:27:52.000000 flameengine-0.0.4.31/flameEngine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 11:27:52.000000 flameengine-0.0.4.31/flameEngine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.31/license.txt
--rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.31/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 11:27:52.201154 flameengine-0.0.4.31/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-05-09 11:26:51.000000 flameengine-0.0.4.31/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:30:36.950718 flameengine-0.0.4.32/
+-rw-rw-rw-   0        0        0      621 2024-05-09 11:30:36.949718 flameengine-0.0.4.32/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-05-05 17:14:33.000000 flameengine-0.0.4.32/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 11:30:36.943291 flameengine-0.0.4.32/flameEngine/
+-rw-rw-rw-   0        0        0       39 2024-05-05 17:55:36.000000 flameengine-0.0.4.32/flameEngine/__init__.py
+-rw-rw-rw-   0        0        0     1078 2024-05-06 16:11:10.000000 flameengine-0.0.4.32/flameEngine/example.py
+-rw-rw-rw-   0        0        0    45462 2024-05-09 11:30:13.000000 flameengine-0.0.4.32/flameEngine/flame.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:30:36.948552 flameengine-0.0.4.32/flameEngine.egg-info/
+-rw-rw-rw-   0        0        0      621 2024-05-09 11:30:36.000000 flameengine-0.0.4.32/flameEngine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2024-05-09 11:30:36.000000 flameengine-0.0.4.32/flameEngine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 11:30:36.000000 flameengine-0.0.4.32/flameEngine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-09 11:30:36.000000 flameengine-0.0.4.32/flameEngine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2489 2024-05-05 16:37:14.000000 flameengine-0.0.4.32/license.txt
+-rw-rw-rw-   0        0        0       88 2024-05-05 17:13:41.000000 flameengine-0.0.4.32/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 11:30:36.950718 flameengine-0.0.4.32/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-05-09 11:30:32.000000 flameengine-0.0.4.32/setup.py
```

### Comparing `flameengine-0.0.4.31/PKG-INFO` & `flameengine-0.0.4.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.31
+Version: 0.0.4.32
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.31/flameEngine/example.py` & `flameengine-0.0.4.32/flameEngine/example.py`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.31/flameEngine/flame.py` & `flameengine-0.0.4.32/flameEngine/flame.py`

 * *Files 2% similar despite different names*

```diff
@@ -647,125 +647,125 @@
             product_density, product_density_prev, \
             u, v, u_prev, v_prev, velocity_magnitude, pressure, \
             temperature, temperature_prev, \
             mass_fuel, mass_oxidizer, mass_product, \
             poisson_v_term, rgb, alpha
 
     def save_results(self, step, save_v=0, save_u=0, save_vu_mag=0, save_fuel=0, save_oxidizer=0,
-                     save_product=0, save_pressure=0, save_temperature=0, save_rgb=0, save_alpha=0):
+                     save_product=0, save_pressure=0, save_temperature=0, save_rgb=0, save_alpha=0,delete_data=0):
         if step % self.frame_skip == 0 or step == 0:
             meta_data = torch.tensor([step,self.fuel_initial_speed,self.grid_size_x,self.grid_size_y,self.N_boundary,self.size_x,
                           self.size_y,self.dx,self.dy,self.dt,self.degrees_of_freedom,
                           self.viscosity,self.diff,self.gravity,self.gravity_divider,
                           self.fuel_molecular_mass,self.oxidizer_molecular_mass,self.product_molecular_mass,
                           self.grid_unit_volume,self.d_low_fuel,self.d_high_fuel,self.d_low_oxidizer,
                           self.d_high_oxidizer,self.th_point_c,self.d_low_product_r_c,self.d_high_product_r_c,self.th_point_r_c,
                           self.d_low_product_r_h,self.d_high_product_r_h,self.th_point_r_h,self.low_alpha,self.high_alpha,self.alpha_decay])
             if save_v == 1:
                 my_folder = 'v'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.v}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'v'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
             if save_u == 1:
                 my_folder = 'u'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.u}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'u'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
             if save_vu_mag == 1:
                 my_folder = 'velocity_magnitude'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.velocity_magnitude}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'velocity_magnitude'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
             if save_fuel == 1:
                 my_folder = 'fuel_density'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.fuel_density}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'fuel_density'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
             if save_oxidizer == 1:
                 my_folder = 'oxidizer_density'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.oxidizer_density}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'oxidizer_density'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
             if save_product == 1:
                 my_folder = 'product_density'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.product_density}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'product_density'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
             if save_pressure == 1:
                 my_folder = 'pressure'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.pressure}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'pressure'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
             if save_temperature == 1:
                 my_folder = 'temperature'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.temperature}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'temperature'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
             if save_rgb == 1:
                 my_folder = 'rgb'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.rgb}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'rgb'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
             if save_alpha == 1:
                 my_folder = 'alpha'
                 Path(my_folder).mkdir(parents=True, exist_ok=True)
                 torch.save({"metadata":meta_data,"data":self.alpha}, f"{my_folder}/t{step}.pt")
             else:
                 my_folder = 'alpha'
-                if os.path.exists(f"{my_folder}"):
+                if os.path.exists(f"{my_folder}") and delete_data:
                     shutil.rmtree(f"{my_folder}")
                 else:
                     pass
 
-    def simulate(self, plot=0, save_animation=0, save_v=0, save_u=0, save_vu_mag=0, save_fuel=0,save_oxidizer=0,save_product=0, save_pressure=0, save_temperature=0, save_rgb=0, save_alpha=0):
+    def simulate(self, plot=0, save_animation=0, save_v=0, save_u=0, save_vu_mag=0, save_fuel=0,save_oxidizer=0,save_product=0, save_pressure=0, save_temperature=0, save_rgb=0, save_alpha=0,delete_data=0):
         if self.idx is None or self.idy is None:
             self.structure_example()
         else:
             pass
         if plot == 1:
             # Create animation
             fig = plt.figure(figsize=(10, 6))
@@ -794,15 +794,15 @@
             ax9.set_title('RGB', size=font_title_size)
             ims = []
 
         for i in range(self.no_frames):
             self.save_results(i, save_v=save_v, save_u=save_u, save_vu_mag=save_vu_mag, save_fuel=save_fuel,
                               save_oxidizer=save_oxidizer,
                               save_product=save_product, save_pressure=save_pressure, save_temperature=save_temperature,
-                              save_rgb=save_rgb, save_alpha=save_alpha)
+                              save_rgb=save_rgb, save_alpha=save_alpha,delete_data=delete_data)
             self.fuel_density, self.fuel_density_prev, \
                 self.oxidizer_density, self.oxidizer_density_prev, \
                 self.product_density, self.product_density_prev, \
                 self.u, self.v, self.u_prev, self.v_prev, \
                 self.pressure, self.velocity_magnitude, self.temperature, self.temperature_prev, \
                 self.mass_fuel, self.mass_oxidizer, self.mass_product, \
                 self.poisson_v_term, self.rgb, self.alpha = \
```

### Comparing `flameengine-0.0.4.31/flameEngine.egg-info/PKG-INFO` & `flameengine-0.0.4.32/flameEngine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flameEngine
-Version: 0.0.4.31
+Version: 0.0.4.32
 Summary: Flame simulation package
 Author: Piotr Mikolajczyk
 Author-email: <pio.mikolajczyk@email.com>
 Keywords: python,flameEngine package,flameEngine,flameEngine
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flameengine-0.0.4.31/license.txt` & `flameengine-0.0.4.32/license.txt`

 * *Files identical despite different names*

### Comparing `flameengine-0.0.4.31/setup.py` & `flameengine-0.0.4.32/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4.31'
+VERSION = '0.0.4.32'
 DESCRIPTION = 'Flame simulation package'
 LONG_DESCRIPTION = 'Simulation engine implementation of stable fluids with extra steps for dataset generation in neural network env and test'
 
 setup(
     name="flameEngine",
     version=VERSION,
     author="Piotr Mikolajczyk",
```


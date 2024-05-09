# Comparing `tmp/pykan-0.0.3.tar.gz` & `tmp/pykan-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykan-0.0.3.tar", last modified: Tue May  7 01:20:49 2024, max compression
+gzip compressed data, was "pykan-0.0.5.tar", last modified: Thu May  9 10:41:55 2024, max compression
```

## Comparing `pykan-0.0.3.tar` & `pykan-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:20:49.091100 pykan-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 01:20:39.000000 pykan-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-07 01:20:49.091100 pykan-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12963 2024-05-07 01:20:39.000000 pykan-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:20:49.091100 pykan-0.0.3/kan/
--rw-r--r--   0 runner    (1001) docker     (127)    51213 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/KAN.py
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/LBFGS.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/Symbolic_KANLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/spline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-07 01:20:39.000000 pykan-0.0.3/kan/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:20:49.091100 pykan-0.0.3/pykan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-07 01:20:49.000000 pykan-0.0.3/pykan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 01:20:49.000000 pykan-0.0.3/pykan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:20:49.000000 pykan-0.0.3/pykan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-07 01:20:49.000000 pykan-0.0.3/pykan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:20:49.091100 pykan-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-07 01:20:39.000000 pykan-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:41:55.771645 pykan-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 10:41:52.000000 pykan-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-09 10:41:55.771645 pykan-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12963 2024-05-09 10:41:52.000000 pykan-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:41:55.771645 pykan-0.0.5/kan/
+-rw-r--r--   0 runner    (1001) docker     (127)    51976 2024-05-09 10:41:52.000000 pykan-0.0.5/kan/KAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15263 2024-05-09 10:41:52.000000 pykan-0.0.5/kan/KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17384 2024-05-09 10:41:52.000000 pykan-0.0.5/kan/LBFGS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-05-09 10:41:52.000000 pykan-0.0.5/kan/Symbolic_KANLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 10:41:52.000000 pykan-0.0.5/kan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-09 10:41:52.000000 pykan-0.0.5/kan/spline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-09 10:41:52.000000 pykan-0.0.5/kan/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:41:55.771645 pykan-0.0.5/pykan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-09 10:41:55.000000 pykan-0.0.5/pykan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-09 10:41:55.000000 pykan-0.0.5/pykan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:41:55.000000 pykan-0.0.5/pykan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 10:41:55.000000 pykan-0.0.5/pykan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:41:55.771645 pykan-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-09 10:41:52.000000 pykan-0.0.5/setup.py
```

### Comparing `pykan-0.0.3/LICENSE` & `pykan-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pykan-0.0.3/PKG-INFO` & `pykan-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykan
-Version: 0.0.3
+Version: 0.0.5
 Summary: Kolmogorov Arnold Networks
 Author: Ziming Liu
 Author-email: zmliu@mit.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pykan-0.0.3/README.md` & `pykan-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pykan-0.0.3/kan/KAN.py` & `pykan-0.0.5/kan/KAN.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,27 +186,27 @@
         >>> print(model_fine.act_fun[0].coef[0][0].data)
         >>> x = torch.normal(0,1,size=(100,2))
         >>> model_fine.initialize_from_another_model(model_coarse, x);
         >>> print(model_fine.act_fun[0].coef[0][0].data)
         tensor(-0.0030)
         tensor(0.0506)
         '''
-        another_model(x)  # get activations
+        another_model(x.to(another_model.device))  # get activations
         batch = x.shape[0]
 
-        self.initialize_grid_from_another_model(another_model, x)
+        self.initialize_grid_from_another_model(another_model, x.to(another_model.device))
 
         for l in range(self.depth):
             spb = self.act_fun[l]
             spb_parent = another_model.act_fun[l]
 
             # spb = spb_parent
             preacts = another_model.spline_preacts[l]
             postsplines = another_model.spline_postsplines[l]
-            self.act_fun[l].coef.data = curve2coef(preacts.reshape(batch, spb.size).permute(1, 0), postsplines.reshape(batch, spb.size).permute(1, 0), spb.grid, k=spb.k)
+            self.act_fun[l].coef.data = curve2coef(preacts.reshape(batch, spb.size).permute(1, 0), postsplines.reshape(batch, spb.size).permute(1, 0), spb.grid, k=spb.k, device=self.device)
             spb.scale_base.data = spb_parent.scale_base.data
             spb.scale_sp.data = spb_parent.scale_sp.data
             spb.mask.data = spb_parent.mask.data
             # print(spb.mask.data, self.act_fun[l].mask.data)
 
         for l in range(self.depth):
             self.biases[l].weight.data = another_model.biases[l].weight.data
@@ -1154,28 +1154,30 @@
                         print(f'skipping ({l},{i},{j}) since already symbolic')
                     else:
                         name, fun, r2 = self.suggest_symbolic(l, i, j, a_range=a_range, b_range=b_range, lib=lib, verbose=False)
                         self.fix_symbolic(l, i, j, name, verbose=verbose > 1)
                         if verbose >= 1:
                             print(f'fixing ({l},{i},{j}) with {name}, r2={r2}')
 
-    def symbolic_formula(self, floating_digit=2, var=None, normalizer=None, simplify=False):
+    def symbolic_formula(self, floating_digit=2, var=None, normalizer=None, simplify=False, output_normalizer = None ):
         '''
         obtain the symbolic formula
         
         Args:
         -----
             floating_digit : int
                 the number of digits to display
             var : list of str
                 the name of variables (if not provided, by default using ['x_1', 'x_2', ...])
             normalizer : [mean array (floats), varaince array (floats)]
                 the normalization applied to inputs
             simplify : bool
                 If True, simplify the equation at each step (usually quite slow), so set up False by default.
+            output_normalizer: [mean array (floats), varaince array (floats)]
+                the normalization applied to outputs
             
         Returns:
         --------
             symbolic formula : sympy function
         
         Example
         -------
@@ -1232,14 +1234,27 @@
                     y.append(sympy.simplify(yj + self.biases[l].weight.data[0, j]))
                 else:
                     y.append(yj + self.biases[l].weight.data[0, j])
 
             x = y
             symbolic_acts.append(x)
 
+        if output_normalizer != None:
+            output_layer = symbolic_acts[-1]
+            means = output_normalizer[0]
+            stds = output_normalizer[1]
+
+            assert len(output_layer) == len(means), 'output_normalizer does not match the output layer'
+            assert len(output_layer) == len(stds), 'output_normalizer does not match the output layer'
+            
+            output_layer = [(output_layer[i] * stds[i] + means[i]) for i in range(len(output_layer))]
+            symbolic_acts[-1] = output_layer
+
+
+
         self.symbolic_acts = [[ex_round(symbolic_acts[l][i]) for i in range(len(symbolic_acts[l]))] for l in range(len(symbolic_acts))]
 
         out_dim = len(symbolic_acts[-1])
         return [ex_round(symbolic_acts[-1][i]) for i in range(len(symbolic_acts[-1]))], x0
 
     def clear_ckpts(self, folder='./model_ckpt'):
         '''
```

### Comparing `pykan-0.0.3/kan/KANLayer.py` & `pykan-0.0.5/kan/KANLayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         noises = (torch.rand(size, self.grid.shape[1]) - 1 / 2) * noise_scale / num
         noises = noises.to(device)
         # shape: (size, coef)
         self.coef = torch.nn.Parameter(curve2coef(self.grid, noises, self.grid, k, device))
         if isinstance(scale_base, float):
             self.scale_base = torch.nn.Parameter(torch.ones(size, device=device) * scale_base).requires_grad_(sb_trainable)  # make scale trainable
         else:
-            self.scale_base = torch.nn.Parameter(torch.FloatTensor(scale_base).cuda()).requires_grad_(sb_trainable)
+            self.scale_base = torch.nn.Parameter(torch.FloatTensor(scale_base).to(device)).requires_grad_(sb_trainable)
         self.scale_sp = torch.nn.Parameter(torch.ones(size, device=device) * scale_sp).requires_grad_(sp_trainable)  # make scale trainable
         self.base_fun = base_fun
 
         self.mask = torch.nn.Parameter(torch.ones(size, device=device)).requires_grad_(False)
         self.grid_eps = grid_eps
         self.weight_sharing = torch.arange(size)
         self.lock_counter = 0
@@ -245,16 +245,16 @@
         tensor([[-1.0000, -0.8000, -0.6000, -0.4000, -0.2000,  0.0000,  0.2000,  0.4000,
           0.6000,  0.8000,  1.0000]])
         '''
         batch = x.shape[0]
         # preacts: shape (batch, in_dim) => shape (size, batch) (size = out_dim * in_dim)
         x_eval = torch.einsum('ij,k->ikj', x, torch.ones(self.out_dim, ).to(self.device)).reshape(batch, self.size).permute(1, 0)
         x_pos = parent.grid
-        sp2 = KANLayer(in_dim=1, out_dim=self.size, k=1, num=x_pos.shape[1] - 1, scale_base=0.).to(self.device)
-        sp2.coef.data = curve2coef(sp2.grid, x_pos, sp2.grid, k=1)
+        sp2 = KANLayer(in_dim=1, out_dim=self.size, k=1, num=x_pos.shape[1] - 1, scale_base=0., device=self.device)
+        sp2.coef.data = curve2coef(sp2.grid, x_pos, sp2.grid, k=1, device=self.device)
         y_eval = coef2curve(x_eval, parent.grid, parent.coef, parent.k, device=self.device)
         percentile = torch.linspace(-1, 1, self.num + 1).to(self.device)
         self.grid.data = sp2(percentile.unsqueeze(dim=1))[0].permute(1, 0)
         self.coef.data = curve2coef(x_eval, y_eval, self.grid, self.k, self.device)
 
     def get_subset(self, in_id, out_id):
         '''
```

### Comparing `pykan-0.0.3/kan/LBFGS.py` & `pykan-0.0.5/kan/LBFGS.py`

 * *Files identical despite different names*

### Comparing `pykan-0.0.3/kan/Symbolic_KANLayer.py` & `pykan-0.0.5/kan/Symbolic_KANLayer.py`

 * *Files identical despite different names*

### Comparing `pykan-0.0.3/kan/spline.py` & `pykan-0.0.5/kan/spline.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,16 @@
     >>> grids = torch.einsum('i,j->ij', torch.ones(num_spline,), torch.linspace(-1,1,steps=num_grid_interval+1))
     >>> coef = torch.normal(0,1,size=(num_spline, num_grid_interval+k))
     >>> coef2curve(x_eval, grids, coef, k=k).shape
     torch.Size([5, 100])
     '''
     # x_eval: (size, batch), grid: (size, grid), coef: (size, coef)
     # coef: (size, coef), B_batch: (size, coef, batch), summer over coef
+    if coef.dtype != x_eval.dtype:
+        coef = coef.to(x_eval.dtype)
     y_eval = torch.einsum('ij,ijk->ik', coef, B_batch(x_eval, grid, k, device=device))
     return y_eval
 
 
 def curve2coef(x_eval, y_eval, grid, k, device="cpu"):
     '''
     converting B-spline curves to B-spline coefficients using least squares.
```

### Comparing `pykan-0.0.3/kan/utils.py` & `pykan-0.0.5/kan/utils.py`

 * *Files identical despite different names*

### Comparing `pykan-0.0.3/pykan.egg-info/PKG-INFO` & `pykan-0.0.5/pykan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykan
-Version: 0.0.3
+Version: 0.0.5
 Summary: Kolmogorov Arnold Networks
 Author: Ziming Liu
 Author-email: zmliu@mit.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pykan-0.0.3/setup.py` & `pykan-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Load the long_description from README.md
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pykan",
-    version="0.0.3",
+    version="0.0.5",
     author="Ziming Liu",
     author_email="zmliu@mit.edu",
     description="Kolmogorov Arnold Networks",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/kindxiaoming/",
     packages=setuptools.find_packages(),
```


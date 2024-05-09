# Comparing `tmp/sdoclust-0.1.tar.gz` & `tmp/sdoclust-0.2.tar.gz`

## Comparing `sdoclust-0.1.tar` & `sdoclust-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 sdoclust-0.1/src/sdoclust/__init__.py
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 sdoclust-0.1/src/sdoclust/clust/__init__.py
--rw-r--r--   0        0        0   133670 2020-02-02 00:00:00.000000 sdoclust-0.1/tests/sdo.png
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 sdoclust-0.1/tests/sdo_example.py
--rw-r--r--   0        0        0   131786 2020-02-02 00:00:00.000000 sdoclust-0.1/tests/sdoclust.png
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 sdoclust-0.1/tests/sdoclust_example.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 sdoclust-0.1/LICENSE
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 sdoclust-0.1/README.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 sdoclust-0.1/pyproject.toml
--rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 sdoclust-0.1/PKG-INFO
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 sdoclust-0.2/src/sdoclust/__init__.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 sdoclust-0.2/src/sdoclust/clust/__init__.py
+-rw-r--r--   0        0        0   133670 2020-02-02 00:00:00.000000 sdoclust-0.2/tests/sdo.png
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 sdoclust-0.2/tests/sdo_example.py
+-rw-r--r--   0        0        0   131786 2020-02-02 00:00:00.000000 sdoclust-0.2/tests/sdoclust.png
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 sdoclust-0.2/tests/sdoclust_example.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 sdoclust-0.2/LICENSE
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 sdoclust-0.2/README.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 sdoclust-0.2/pyproject.toml
+-rw-r--r--   0        0        0     6664 2020-02-02 00:00:00.000000 sdoclust-0.2/PKG-INFO
```

### Comparing `sdoclust-0.1/src/sdoclust/__init__.py` & `sdoclust-0.2/src/sdoclust/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,16 @@
 		    Xp = pca.fit_transform(Xt)
 		    sigma = np.std(Xp)
 		    if sigma<1:
 			    sigma=1
 		    error = 0.1*np.std(Xp);
 		    self.k = sample_size( m, sigma, error )
 		    k = self.k
+	    else:
+		    k = self.k
 
 	    chunksize = self.chunksize
 	    if chunksize is None:
 	        chunksize = m
 
 	    np.random.seed(self.rseed)
 	    index = np.random.permutation(m)
@@ -217,14 +219,17 @@
 
         ind, count = np.unique(ol, return_counts=True)
         toremove = np.zeros(len(O))
         for i in ind:
             if count[i] <= self.e:
                 toremove[ol==i]=1
 
+        if np.sum(toremove) == len(O):
+            toremove = np.zeros(len(O))
+
         O = O[toremove==0,:]
         ol = ol[toremove==0] 
 
         nl = np.copy(ol)
         for i,l in enumerate(np.unique(ol)):
             nl[ol==l]=i
         ol = nl
```

### Comparing `sdoclust-0.1/src/sdoclust/clust/__init__.py` & `sdoclust-0.2/src/sdoclust/clust/__init__.py`

 * *Files identical despite different names*

### Comparing `sdoclust-0.1/tests/sdo.png` & `sdoclust-0.2/tests/sdo.png`

 * *Files identical despite different names*

### Comparing `sdoclust-0.1/tests/sdoclust.png` & `sdoclust-0.2/tests/sdoclust.png`

 * *Files identical despite different names*

### Comparing `sdoclust-0.1/LICENSE` & `sdoclust-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdoclust-0.1/README.md` & `sdoclust-0.2/README.md`

 * *Files identical despite different names*

### Comparing `sdoclust-0.1/pyproject.toml` & `sdoclust-0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sdoclust"
-version = "0.1"
+version = "0.2"
 authors = [
   { name="Félix Iglesias Vázquez", email="felix.iglesias@tuwien.ac.at" },
 ]
 description = "outlier detection and clustering based on sparse data observers"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `sdoclust-0.1/PKG-INFO` & `sdoclust-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sdoclust
-Version: 0.1
+Version: 0.2
 Summary: outlier detection and clustering based on sparse data observers
 Project-URL: Homepage, https://github.com/CN-TU/pysdoclust
 Author-email: Félix Iglesias Vázquez <felix.iglesias@tuwien.ac.at>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```


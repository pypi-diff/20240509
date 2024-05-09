# Comparing `tmp/ParametricSpectralClustering-0.0.2.tar.gz` & `tmp/ParametricSpectralClustering-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ParametricSpectralClustering-0.0.2.tar", last modified: Fri Apr 19 11:26:39 2024, max compression
+gzip compressed data, was "dist/ParametricSpectralClustering-0.0.3.tar", last modified: Wed May  1 04:16:15 2024, max compression
```

## Comparing `ParametricSpectralClustering-0.0.2.tar` & `ParametricSpectralClustering-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.451058 ParametricSpectralClustering-0.0.2/
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.446065 ParametricSpectralClustering-0.0.2/JSS_Experiments/
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.446372 ParametricSpectralClustering-0.0.2/JSS_Experiments/Firewall_table4/
--rw-r--r--   0 ivychang   (501) staff       (20)    14281 2024-04-03 04:53:46.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/Firewall_table4/main.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.446716 ParametricSpectralClustering-0.0.2/JSS_Experiments/NIDS_table5/
--rw-r--r--   0 ivychang   (501) staff       (20)     7449 2024-04-03 04:53:22.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/NIDS_table5/main.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.447334 ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/
--rw-r--r--   0 ivychang   (501) staff       (20)    10399 2024-04-19 11:08:05.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/figure1.py
--rw-r--r--   0 ivychang   (501) staff       (20)     6588 2024-02-08 08:49:22.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/figure2.py
--rw-r--r--   0 ivychang   (501) staff       (20)     2000 2024-04-19 11:23:25.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/run.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.447584 ParametricSpectralClustering-0.0.2/JSS_Experiments/table_3/
--rw-r--r--   0 ivychang   (501) staff       (20)     9400 2024-04-03 04:54:58.000000 ParametricSpectralClustering-0.0.2/JSS_Experiments/table_3/main.py
--rw-r--r--   0 ivychang   (501) staff       (20)     1066 2023-08-21 09:34:30.000000 ParametricSpectralClustering-0.0.2/LICENSE.txt
--rw-r--r--   0 ivychang   (501) staff       (20)       44 2023-08-21 09:45:35.000000 ParametricSpectralClustering-0.0.2/MANIFEST.in
--rw-r--r--   0 ivychang   (501) staff       (20)     4376 2024-04-19 11:26:39.450887 ParametricSpectralClustering-0.0.2/PKG-INFO
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.448151 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering/
--rw-r--r--   0 ivychang   (501) staff       (20)       47 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering/__init__.py
--rw-r--r--   0 ivychang   (501) staff       (20)    15151 2024-03-26 10:00:23.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering/psc.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.449102 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/
--rw-r--r--   0 ivychang   (501) staff       (20)     4376 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/PKG-INFO
--rw-r--r--   0 ivychang   (501) staff       (20)      813 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/SOURCES.txt
--rw-r--r--   0 ivychang   (501) staff       (20)        1 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/dependency_links.txt
--rw-r--r--   0 ivychang   (501) staff       (20)        1 2024-01-30 05:57:05.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/not-zip-safe
--rw-r--r--   0 ivychang   (501) staff       (20)      113 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/requires.txt
--rw-r--r--   0 ivychang   (501) staff       (20)       29 2024-04-19 11:26:39.000000 ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/top_level.txt
--rw-r--r--   0 ivychang   (501) staff       (20)     3591 2024-04-19 11:14:38.000000 ParametricSpectralClustering-0.0.2/README.md
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.449492 ParametricSpectralClustering-0.0.2/bin/
--rw-r--r--   0 ivychang   (501) staff       (20)     2566 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.2/bin/clustering.py
--rw-r--r--   0 ivychang   (501) staff       (20)     3276 2024-02-11 14:01:58.000000 ParametricSpectralClustering-0.0.2/bin/run.py
--rw-r--r--   0 ivychang   (501) staff       (20)     1641 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.2/bin/train_psc.py
--rw-r--r--   0 ivychang   (501) staff       (20)       38 2024-04-19 11:26:39.451114 ParametricSpectralClustering-0.0.2/setup.cfg
--rw-r--r--   0 ivychang   (501) staff       (20)     1348 2024-04-19 11:25:51.000000 ParametricSpectralClustering-0.0.2/setup.py
-drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-04-19 11:26:39.450489 ParametricSpectralClustering-0.0.2/tests/
--rw-r--r--   0 ivychang   (501) staff       (20)        0 2023-08-22 05:19:40.000000 ParametricSpectralClustering-0.0.2/tests/__init__.py
--rw-r--r--   0 ivychang   (501) staff       (20)      948 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.2/tests/test_Accuracy.py
--rw-r--r--   0 ivychang   (501) staff       (20)      716 2024-01-07 05:49:34.000000 ParametricSpectralClustering-0.0.2/tests/test_Four_layer_FNN.py
--rw-r--r--   0 ivychang   (501) staff       (20)     2864 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.2/tests/test_PSC.py
--rw-r--r--   0 ivychang   (501) staff       (20)     1435 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.2/tests/test_error_handling.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.025985 ParametricSpectralClustering-0.0.3/
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.019704 ParametricSpectralClustering-0.0.3/JSS_Experiments/
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.020157 ParametricSpectralClustering-0.0.3/JSS_Experiments/Firewall_table4/
+-rw-r--r--   0 ivychang   (501) staff       (20)    14551 2024-04-26 14:13:39.000000 ParametricSpectralClustering-0.0.3/JSS_Experiments/Firewall_table4/main.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.020538 ParametricSpectralClustering-0.0.3/JSS_Experiments/NIDS_table5/
+-rw-r--r--   0 ivychang   (501) staff       (20)     7751 2024-04-26 13:53:43.000000 ParametricSpectralClustering-0.0.3/JSS_Experiments/NIDS_table5/main.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.021378 ParametricSpectralClustering-0.0.3/JSS_Experiments/Synthesis_dataset/
+-rw-r--r--   0 ivychang   (501) staff       (20)    10480 2024-04-26 13:53:43.000000 ParametricSpectralClustering-0.0.3/JSS_Experiments/Synthesis_dataset/figure1.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     6657 2024-04-26 13:53:43.000000 ParametricSpectralClustering-0.0.3/JSS_Experiments/Synthesis_dataset/figure2.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     2001 2024-04-26 14:51:19.000000 ParametricSpectralClustering-0.0.3/JSS_Experiments/run.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.021871 ParametricSpectralClustering-0.0.3/JSS_Experiments/table_3/
+-rw-r--r--   0 ivychang   (501) staff       (20)    11113 2024-04-26 13:53:43.000000 ParametricSpectralClustering-0.0.3/JSS_Experiments/table_3/main.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     1066 2023-08-21 09:34:30.000000 ParametricSpectralClustering-0.0.3/LICENSE.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)       44 2023-08-21 09:45:35.000000 ParametricSpectralClustering-0.0.3/MANIFEST.in
+-rw-r--r--   0 ivychang   (501) staff       (20)     4449 2024-05-01 04:16:15.025802 ParametricSpectralClustering-0.0.3/PKG-INFO
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.022466 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering/
+-rw-r--r--   0 ivychang   (501) staff       (20)       47 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering/__init__.py
+-rw-r--r--   0 ivychang   (501) staff       (20)    15151 2024-03-26 10:00:23.000000 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering/psc.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.023669 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering.egg-info/
+-rw-r--r--   0 ivychang   (501) staff       (20)     4449 2024-05-01 04:16:14.000000 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering.egg-info/PKG-INFO
+-rw-r--r--   0 ivychang   (501) staff       (20)      813 2024-05-01 04:16:14.000000 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering.egg-info/SOURCES.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)        1 2024-05-01 04:16:14.000000 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering.egg-info/dependency_links.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)        1 2024-01-30 05:57:05.000000 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering.egg-info/not-zip-safe
+-rw-r--r--   0 ivychang   (501) staff       (20)      131 2024-05-01 04:16:14.000000 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering.egg-info/requires.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)       29 2024-05-01 04:16:14.000000 ParametricSpectralClustering-0.0.3/ParametricSpectralClustering.egg-info/top_level.txt
+-rw-r--r--   0 ivychang   (501) staff       (20)     3616 2024-05-01 04:13:53.000000 ParametricSpectralClustering-0.0.3/README.md
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.024092 ParametricSpectralClustering-0.0.3/bin/
+-rw-r--r--   0 ivychang   (501) staff       (20)     2566 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.3/bin/clustering.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     3276 2024-02-11 14:01:58.000000 ParametricSpectralClustering-0.0.3/bin/run.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     1641 2024-01-29 17:16:13.000000 ParametricSpectralClustering-0.0.3/bin/train_psc.py
+-rw-r--r--   0 ivychang   (501) staff       (20)       38 2024-05-01 04:16:15.026055 ParametricSpectralClustering-0.0.3/setup.cfg
+-rw-r--r--   0 ivychang   (501) staff       (20)     1373 2024-05-01 04:16:06.000000 ParametricSpectralClustering-0.0.3/setup.py
+drwxr-xr-x   0 ivychang   (501) staff       (20)        0 2024-05-01 04:16:15.025195 ParametricSpectralClustering-0.0.3/tests/
+-rw-r--r--   0 ivychang   (501) staff       (20)        0 2023-08-22 05:19:40.000000 ParametricSpectralClustering-0.0.3/tests/__init__.py
+-rw-r--r--   0 ivychang   (501) staff       (20)      948 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.3/tests/test_Accuracy.py
+-rw-r--r--   0 ivychang   (501) staff       (20)      716 2024-01-07 05:49:34.000000 ParametricSpectralClustering-0.0.3/tests/test_Four_layer_FNN.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     2864 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.3/tests/test_PSC.py
+-rw-r--r--   0 ivychang   (501) staff       (20)     1435 2024-02-08 07:46:41.000000 ParametricSpectralClustering-0.0.3/tests/test_error_handling.py
```

### Comparing `ParametricSpectralClustering-0.0.2/JSS_Experiments/Firewall_table4/main.py` & `ParametricSpectralClustering-0.0.3/JSS_Experiments/Firewall_table4/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 import time
 import datetime
 import argparse
 import warnings
 import sklearn
 from sklearn.cluster import SpectralClustering, KMeans
 from ParametricSpectralClustering import PSC, Accuracy
+from pathlib import Path
+import random
+import torch
+
+r = 72
+rng = np.random.RandomState(r)
+torch.manual_seed(0)
+random.seed(int(r))
+np.random.seed(0)
+
+ROOT = Path("JSS_Experiments").parent.absolute()
 
 warnings.filterwarnings("ignore")
 
 parser = argparse.ArgumentParser()
 parser.add_argument("-datasize", "--size", type=int, help="data size used for training")
 parser.add_argument(
     "-methods",
@@ -33,22 +44,22 @@
             nn.Linear(32, 4),
         )
 
     def forward(self, x):
         return self.model(x)
 
 
-df = pd.read_csv("JSS_Experiments/datasets/firewall.csv")
+df = pd.read_csv(ROOT / "datasets" / "firewall.csv")
 action = {"allow": 1, "deny": 2, "drop": 3, "reset-both": 4}
 df["Action"] = df["Action"].map(action)
 y_tmp = df["Action"].values
 x_tmp = df.drop(["Action"], axis=1).values
 
 
-f = open("JSS_Experiments/Firewall_table4/log.txt", "a+")
+f = open(ROOT / "Firewall_table4" / "log.txt", "a+")
 now = str(datetime.datetime.now())
 f.write("======" + now + "======\n")
 
 if args.size == -1:
     f.write("input data size: all\n")
     x_data = x_tmp
     y = y_tmp
@@ -73,23 +84,24 @@
 psc_acc_1_60000 = []
 psc_acc_15001_60000 = []
 psc_time_1_15000 = []
 psc_time_1_30000 = []
 psc_time_1_45000 = []
 psc_time_1_60000 = []
 
-result = pd.read_csv("JSS_Experiments/Firewall_table4/result.csv")
+result = pd.read_csv(ROOT / "Firewall_table4" / "result.csv")
 
 for _ in range(10):
     if "sc" in methods:
         spectral_clustering = SpectralClustering(
             n_clusters=4,
             eigen_solver="arpack",
             affinity="nearest_neighbors",
             assign_labels="kmeans",
+            random_state=rng,
         )
 
         # measure time spent
         start_time = round(time.time() * 1000)
         sc_index = spectral_clustering.fit_predict(x)
         end_time = round(time.time() * 1000)
 
@@ -111,22 +123,24 @@
     # fixed_n_wo_sampling_ratio.py --size 60000 --method
     if "psc" in methods:
         kmeans = KMeans(
             n_clusters=4,
             init="random",
             n_init="auto",
             algorithm="elkan",
+            random_state=rng,
         )
         psc = PSC(
             model=Net(),
             clustering_method=kmeans,
             sampling_ratio=0,
             n_components=4,
             n_neighbor=4,
             batch_size_data=args.size,
+            random_state=rng,
         )
 
         # measure training time spent
         train_start_time = round(time.time() * 1000)
         psc.fit(x[:15000])
         psc_index = psc.predict(x[:15000])
         train_end_time = round(time.time() * 1000)
@@ -273,22 +287,22 @@
         "[1:n] acc: "
         + str(psc_acc_1_15000_mean)
         + "±"
         + str(psc_acc_1_15000_std)
         + "\n"
     )
     f.write(
-        "[n+1:m] acc: "
+        "[n+1:n+m] acc: "
         + str(psc_acc_1_15000_mean)
         + "±"
         + str(psc_acc_1_15000_std)
         + "\n"
     )
     f.write(
-        "[1:m] acc: "
+        "all acc: "
         + str(psc_acc_1_15000_mean)
         + "±"
         + str(psc_acc_1_15000_std)
         + "\n\n"
     )
     f.write("data size: 30000\n")
     f.write(
@@ -302,22 +316,22 @@
         "[1:n] acc: "
         + str(psc_acc_1_15000_mean)
         + "±"
         + str(psc_acc_1_15000_std)
         + "\n"
     )
     f.write(
-        "[n+1:m] acc: "
+        "[n+1:n+m] acc: "
         + str(psc_acc_15001_30000_mean)
         + "±"
         + str(psc_acc_15001_30000_std)
         + "\n"
     )
     f.write(
-        "[1:m] acc: "
+        "all acc: "
         + str(psc_acc_1_30000_mean)
         + "±"
         + str(psc_acc_1_30000_std)
         + "\n\n"
     )
     f.write("data size: 45000\n")
     f.write(
@@ -331,22 +345,22 @@
         "[1:n] acc: "
         + str(psc_acc_1_15000_mean)
         + "±"
         + str(psc_acc_1_15000_std)
         + "\n"
     )
     f.write(
-        "[n+1:m] acc: "
+        "[n+1:n+m] acc: "
         + str(psc_acc_15001_45000_mean)
         + "±"
         + str(psc_acc_15001_45000_std)
         + "\n"
     )
     f.write(
-        "[1:n] acc: "
+        "all acc: "
         + str(psc_acc_1_45000_mean)
         + "±"
         + str(psc_acc_1_45000_std)
         + "\n\n"
     )
     f.write("data size: 60000\n")
     f.write(
@@ -360,22 +374,22 @@
         "[1:n] acc: "
         + str(psc_acc_1_15000_mean)
         + "±"
         + str(psc_acc_1_15000_std)
         + "\n"
     )
     f.write(
-        "[n+1:m] acc: "
+        "[n+1:n+m] acc: "
         + str(psc_acc_15001_60000_mean)
         + "±"
         + str(psc_acc_15001_60000_std)
         + "\n"
     )
     f.write(
-        "[1:n] acc: "
+        "all acc: "
         + str(psc_acc_1_60000_mean)
         + "±"
         + str(psc_acc_1_60000_std)
         + "\n\n"
     )
 
     # write result into result.csv
@@ -392,43 +406,43 @@
     result.at[1, "Accuracy.3"] = (
         str(psc_acc_1_15000_mean) + "±" + str(psc_acc_1_15000_std)
     )
     result.at[2, "Time.1"] = (
         str(psc_time_1_30000_mean) + "±" + str(psc_time_1_30000_std)
     )
     result.at[2, "Accuracy.1"] = (
-        str(psc_acc_1_15000_mean) + "±" + str(psc_acc_1_15000_std)
+        str(psc_acc_1_30000_mean) + "±" + str(psc_acc_1_30000_std)
     )
     result.at[2, "Accuracy.2"] = (
-        str(psc_acc_15001_30000_mean) + "±" + str(psc_acc_15001_30000_std)
+        str(psc_acc_1_15000_mean) + "±" + str(psc_acc_1_15000_std)
     )
     result.at[2, "Accuracy.3"] = (
-        str(psc_acc_1_30000_mean) + "±" + str(psc_acc_1_30000_std)
+        str(psc_acc_15001_30000_mean) + "±" + str(psc_acc_15001_30000_std)
     )
     result.at[3, "Time.1"] = (
         str(psc_time_1_45000_mean) + "±" + str(psc_time_1_45000_std)
     )
     result.at[3, "Accuracy.1"] = (
-        str(psc_acc_1_15000_mean) + "±" + str(psc_acc_1_15000_std)
+        str(psc_acc_1_45000_mean) + "±" + str(psc_acc_1_45000_std)
     )
     result.at[3, "Accuracy.2"] = (
-        str(psc_acc_15001_45000_mean) + "±" + str(psc_acc_15001_45000_std)
+        str(psc_acc_1_15000_mean) + "±" + str(psc_acc_1_15000_std)
     )
     result.at[3, "Accuracy.3"] = (
-        str(psc_acc_1_45000_mean) + "±" + str(psc_acc_1_45000_std)
+        str(psc_acc_15001_45000_mean) + "±" + str(psc_acc_15001_45000_std)
     )
     result.at[4, "Time.1"] = (
         str(psc_time_1_60000_mean) + "±" + str(psc_time_1_60000_std)
     )
     result.at[4, "Accuracy.1"] = (
-        str(psc_acc_1_15000_mean) + "±" + str(psc_acc_1_15000_std)
+        str(psc_acc_1_60000_mean) + "±" + str(psc_acc_1_60000_std)
     )
     result.at[4, "Accuracy.2"] = (
-        str(psc_acc_15001_60000_mean) + "±" + str(psc_acc_15001_60000_std)
+        str(psc_acc_1_15000_mean) + "±" + str(psc_acc_1_15000_std)
     )
     result.at[4, "Accuracy.3"] = (
-        str(psc_acc_1_60000_mean) + "±" + str(psc_acc_1_60000_std)
+        str(psc_acc_15001_60000_mean) + "±" + str(psc_acc_15001_60000_std)
     )
 
 
 f.close()
-result.to_csv("JSS_Experiments/Firewall_table4/result.csv", index=False)
+result.to_csv(ROOT / "Firewall_table4" / "result.csv", index=False)
```

### Comparing `ParametricSpectralClustering-0.0.2/JSS_Experiments/NIDS_table5/main.py` & `ParametricSpectralClustering-0.0.3/JSS_Experiments/NIDS_table5/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 from sklearn.cluster import SpectralClustering, KMeans
 from ParametricSpectralClustering import PSC, Accuracy
 import time
 import datetime
 import argparse
 import warnings
 import numpy as np
+from pathlib import Path
+import random
+import torch
+
+r = 72
+rng = np.random.RandomState(r)
+torch.manual_seed(0)
+random.seed(int(r))
+np.random.seed(0)
+
+ROOT = Path("JSS_Experiments").parent.absolute()
 
 warnings.filterwarnings("ignore")
 
 parser = argparse.ArgumentParser()
 parser.add_argument("-datasize", "--size", type=int, help="data size used for training")
 parser.add_argument("-methods", "--methods", nargs="+", help="which method to test")
 parser.add_argument("-sampling_ratio", "--ratio", type=float, help="sampling ratio")
@@ -33,15 +44,15 @@
         x = self.fc2(x)
         x = self.fc3(x)
         x = self.fc4(x)
         x = self.output_layer(x)
         return x
 
 
-df = pd.read_csv("JSS_Experiments/datasets/NF-UQ-NIDS-v2.csv", nrows=1040000)
+df = pd.read_csv(ROOT / "datasets" / "NF-UQ-NIDS-v2.csv", nrows=1040000)
 Class = {
     "Benign": 1,
     "DDoS": 2,
     "DoS": 3,
     "scanning": 4,
     "Reconnaissance": 4,
     "xss": 4,
@@ -63,15 +74,15 @@
 }
 df["Attack"] = df["Attack"].map(Class)
 print(df.drop(["Attack", "IPV4_SRC_ADDR", "IPV4_DST_ADDR", "Dataset"], axis=1).info())
 
 y_tmp = df["Attack"].values
 x_tmp = df.drop(["Attack", "IPV4_SRC_ADDR", "IPV4_DST_ADDR", "Dataset"], axis=1).values
 
-f = open("JSS_Experiments/NIDS_table5/log.txt", "a+")
+f = open(ROOT / "NIDS_table5" / "log.txt", "a+")
 now = str(datetime.datetime.now())
 f.write("======" + now + "======\n")
 if args.size == -1:
     f.write("input data size: all\n")
     x_data = x_tmp
     y = y_tmp
 else:
@@ -84,24 +95,25 @@
 methods = args.methods
 
 total_acc = []
 total_time = []
 total_ari = []
 total_ami = []
 
-result = pd.read_csv("JSS_Experiments/NIDS_table5/result.csv", index_col=0)
+result = pd.read_csv(ROOT / "NIDS_table5" / "result.csv", index_col=0)
 
 for i in range(10):
     # --------Spectral Clustering--------
     if "sc" in methods:
         spectral_clustering = SpectralClustering(
             n_clusters=10,
             eigen_solver="arpack",
             affinity="nearest_neighbors",
             assign_labels="kmeans",
+            random_state=rng,
         )
 
         # measure time spent
         start_time = round(time.time() * 1000)
         sc_index = spectral_clustering.fit_predict(x)
         end_time = round(time.time() * 1000)
 
@@ -118,15 +130,15 @@
         f.write("acc rate: " + str(sc_accRate) + "\n")
         f.write("ari: " + str(sc_ari) + "\n")
         f.write("ami: " + str(sc_ami) + "\n")
         f.write("time spent: " + str(end_time - start_time) + "\n\n")
 
     # --------kmeans--------
     if "kmeans" in methods:
-        kmeans = KMeans(n_clusters=10, init="random", n_init="auto", algorithm="elkan")
+        kmeans = KMeans(n_clusters=10, init="random", n_init="auto", algorithm="elkan", random_state=rng,)
 
         # measure time spent
         start_time = round(time.time() * 1000)
         kmeans_index = kmeans.fit_predict(x)
         end_time = round(time.time() * 1000)
 
         # calculate acc, ari, ami
@@ -143,32 +155,34 @@
         f.write("ari: " + str(kmeans_ari) + "\n")
         f.write("ami: " + str(kmeans_ami) + "\n")
         f.write("time spent: " + str(end_time - start_time) + "\n\n")
 
     # --------Parametric Spectral Clustering--------
     if "psc" in methods:
         model = Net_emb()
-        kmeans = KMeans(n_clusters=10, init="random", n_init="auto", algorithm="elkan")
+        kmeans = KMeans(n_clusters=10, init="random", n_init="auto", algorithm="elkan", random_state=rng)
         psc = PSC(
             model=model,
             clustering_method=kmeans,
             sampling_ratio=args.ratio,
             n_components=10,
             n_neighbor=10,
             batch_size_data=args.size,
+            random_state=rng,
         )
 
         # measure time spent
         start_time = round(time.time() * 1000)
         psc.fit(x)
         psc_index = psc.predict(x)
         end_time = round(time.time() * 1000)
 
+        file_name = "psc_model" + str(i + 1) + ".pkl"
         # save model
-        psc.save_model("JSS_Experiments/NIDS_table5/psc_model" + str(i + 1) + ".pkl")
+        psc.save_model(ROOT / "NIDS_table5" / file_name)
 
         # calculate acc, ari, ami
         acc = Accuracy(y_true=y, y_pred=psc_index)
         psc_accRate, psc_ari, psc_ami = acc.acc_report()
         total_acc.append(psc_accRate)
         total_ari.append(psc_ari)
         total_ami.append(psc_ami)
@@ -215,8 +229,8 @@
 if "sc" in methods:
     result.at[str(args), "SC"] = str(time_mean) + "±" + str(time_std)
     result.at[str(args), "SC.1"] = str(acc_mean) + "±" + str(acc_std)
     result.at[str(args), "SC.2"] = str(ari_mean) + "±" + str(ari_std)
     result.at[str(args), "SC.3"] = str(ami_mean) + "±" + str(ami_std)
 
 f.close()
-df.to_csv("JSS_Experiments/NIDS_table5/result.csv")
+df.to_csv(ROOT / "NIDS_table5" / "result.csv")
```

### Comparing `ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/figure1.py` & `ParametricSpectralClustering-0.0.3/JSS_Experiments/Synthesis_dataset/figure1.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 import torch.nn as nn
 import random
 import argparse
 from sklearn import cluster, datasets, mixture
 from sklearn.neighbors import kneighbors_graph
 from sklearn.preprocessing import StandardScaler
 from itertools import cycle, islice
-
+from pathlib import Path
 from ParametricSpectralClustering.psc import PSC
 
+ROOT = Path("JSS_Experiments").parent.absolute()
+
 parser = argparse.ArgumentParser()
 parser.add_argument(
     "-dataset",
     "--dataset",
     type=str,
     help="the dataset used in this single experiment",
 )
@@ -356,10 +358,11 @@
         plt.scatter(X[:, 0], X[:, 1], s=10, color=colors[y_pred])
 
         plt.xlim(-2.5, 2.5)
         plt.ylim(-2.5, 2.5)
         plt.xticks(())
         plt.yticks(())
         plot_num += 1
-fig_name = "JSS_Experiments/Synthesis_dataset/Figure1-" + str(fig_num) + ".pdf"
+name = "Figure1-" + str(fig_num) + ".pdf"
+fig_name = ROOT / "Synthesis_dataset" / name
 plt.savefig(fig_name, format="pdf", bbox_inches="tight")
 # f.close()
```

### Comparing `ParametricSpectralClustering-0.0.2/JSS_Experiments/Synthesis_dataset/figure2.py` & `ParametricSpectralClustering-0.0.3/JSS_Experiments/Synthesis_dataset/figure2.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import torch.nn as nn
 
 from sklearn import cluster, datasets
 from sklearn.preprocessing import StandardScaler
+from pathlib import Path
 
+ROOT = Path("JSS_Experiments").parent.absolute()
 
 class KMedian:
     def __init__(self, n_clusters, max_iters=100) -> None:
         self.n_clusters = n_clusters
         self.max_iters = max_iters
         self.cluseter_centers_ = None
 
@@ -228,11 +230,11 @@
         plt.xticks(())
         plt.yticks(())
 
         plot_num += 1
 
 
 plt.savefig(
-    "JSS_Experiments/Synthesis_dataset/Figure2_custom_clustering_KMedian.pdf",
+    ROOT / "Synthesis_dataset" / "Figure2_custom_clustering_KMedian.pdf",
     format="pdf",
 )
 plt.show()
```

### Comparing `ParametricSpectralClustering-0.0.2/JSS_Experiments/run.py` & `ParametricSpectralClustering-0.0.3/JSS_Experiments/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,21 @@
         subprocess.run(command, check=True)
     except subprocess.CalledProcessError as e:
         print("An error occurred while executing:", " ".join(command))
         print(e)
 
 
 # Experiment for table 3
-datasets_table3 = ["Pendigits", "Letter"]
+datasets_table3 = ["Firewall", "Letter"]
 for dataset in datasets_table3:
     run_command(
         [
             "python",
             "table_3/main.py",
-            "--method",
+            "--methods",
             "sc",
             "psc",
             "kmeans",
             "--dataset",
             dataset,
             "--size",
             "-1",
@@ -61,15 +61,15 @@
         [
             "python",
             "NIDS_table5/main.py",
             "--methods",
             "psc",
             "--size",
             data_size_table5,
-            "--rate",
+            "--ratio",
             "0.9",
         ]
     )
     run_command(
         ["python", "NIDS_table5/main.py", "--methods", "sc", "--size", data_size_table5]
     )
```

### Comparing `ParametricSpectralClustering-0.0.2/JSS_Experiments/table_3/main.py` & `ParametricSpectralClustering-0.0.3/JSS_Experiments/table_3/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,25 @@
 import datetime
 import argparse
 import warnings
 import sklearn
 from sklearn.cluster import SpectralClustering, KMeans
 from ParametricSpectralClustering import PSC, Accuracy
 from scipy.io import arff
+from pathlib import Path
+import random
+import torch
+
+r = 72
+rng = np.random.RandomState(r)
+torch.manual_seed(0)
+random.seed(int(r))
+np.random.seed(0)
+
+ROOT = Path("JSS_Experiments").parent.absolute()
 
 warnings.filterwarnings("ignore")
 
 parser = argparse.ArgumentParser()
 parser.add_argument("-datasize", "--size", type=int, help="data size used for training")
 parser.add_argument(
     "-methods",
@@ -26,38 +37,54 @@
     type=str,
     help="choose Letter dataset or Pendigits dataset in this experiment",
 )
 
 args = parser.parse_args()
 
 
-class Net(nn.Module):
+class Net_Letter(nn.Module):
     def __init__(self) -> None:
-        super(Net, self).__init__()
+        super(Net_Letter, self).__init__()
+
+        self.model = nn.Sequential(
+            nn.Linear(16, 32),
+            nn.Linear(32, 64),
+            nn.Linear(64, 32),
+            nn.Linear(32, 26),
+        )
+
+    def forward(self, x):
+        return self.model(x)
+
 
+class Net_Firewall(nn.Module):
+    def __init__(self) -> None:
+        super(Net_Firewall, self).__init__()
         self.model = nn.Sequential(
             nn.Linear(11, 32),
             nn.Linear(32, 64),
             nn.Linear(64, 32),
             nn.Linear(32, 4),
         )
 
     def forward(self, x):
         return self.model(x)
 
 
 dataset = args.dataset
 
-if "Pendigits" in dataset:
-    pendigits = pd.read_csv("JSS_Experiments/datasets/Pendigits.csv")
-    y_tmp = pendigits["class"].values
-    x_tmp = pendigits.drop(columns=["id", "class"]).values
+if "Firewall" in dataset:
+    firewall = pd.read_csv(ROOT / "datasets" / "firewall.csv")
+    action = {"allow": 1, "deny": 2, "drop": 3, "reset-both": 4}
+    firewall["Action"] = firewall["Action"].map(action)
+    y_tmp = firewall["Action"].values
+    x_tmp = firewall.drop(["Action"], axis=1).values
 
 elif "Letter" in dataset:
-    letter_arff = arff.loadarff("JSS_Experiments/datasets/dataset_6_letter.arff")
+    letter_arff = arff.loadarff(ROOT / "datasets" / "dataset_6_letter.arff")
     letter = pd.DataFrame(letter_arff[0])
     letter["class"] = letter["class"].astype(str)
 
     Class = {
         "A": 1,
         "B": 2,
         "C": 3,
@@ -89,15 +116,15 @@
     letter["class"] = letter["class"].map(Class)
     y_tmp = letter["class"].values
     x_data_tmp = letter.drop(["class"], axis=1).values
 
     scaler = sklearn.preprocessing.StandardScaler().fit(x_data_tmp)
     x_tmp = scaler.transform(x_data_tmp)
 
-f = open("JSS_Experiments/table_3/log.txt", "a+")
+f = open(ROOT / "table_3" / "log.txt", "a+")
 now = str(datetime.datetime.now())
 f.write("======" + now + "======\n")
 f.write("dataset: " + str(args.dataset) + "\n")
 
 if args.size == -1:
     f.write("input data size: all\n")
     x_data = x_tmp
@@ -120,25 +147,34 @@
 sc_total_ari = []
 sc_total_ami = []
 
 psc_total_acc = []
 psc_total_ari = []
 psc_total_ami = []
 
-result = pd.read_csv("JSS_Experiments/table_3/result.csv", index_col=[0, 1])
+result = pd.read_csv(ROOT / "table_3" / "result.csv", index_col=[0, 1])
 
 for _ in range(10):
     if "sc" in methods:
-        spectral_clustering = SpectralClustering(
-            n_clusters=4,
-            eigen_solver="arpack",
-            affinity="nearest_neighbors",
-            assign_labels="kmeans",
-        )
-
+        if "Firewall" in dataset:
+            spectral_clustering = SpectralClustering(
+                n_clusters=4,
+                eigen_solver="arpack",
+                affinity="nearest_neighbors",
+                assign_labels="kmeans",
+                random_state=rng,
+            )
+        elif "Letter" in dataset:
+            spectral_clustering = SpectralClustering(
+                n_clusters=26,
+                eigen_solver="arpack",
+                affinity="nearest_neighbors",
+                assign_labels="kmeans",
+                random_state=rng,
+            )
         # measure time spent
         start_time = round(time.time() * 1000)
         sc_index = spectral_clustering.fit_predict(x)
         end_time = round(time.time() * 1000)
 
         # calculate accuracy, ari, ami
         acc = Accuracy(y_true=y, y_pred=sc_index)
@@ -152,22 +188,34 @@
         f.write("time spent: " + str(end_time - start_time) + "\n\n")
         sc_total_acc.append(sc_accRate)
         sc_total_ami.append(sc_ami)
         sc_total_ari.append(sc_ari)
 
     if "psc" in methods:
         kmeans = KMeans(n_clusters=4, init="random", n_init="auto", algorithm="elkan")
-        psc = PSC(
-            model=Net(),
-            clustering_method=kmeans,
-            sampling_ratio=0,
-            n_components=4,
-            n_neighbor=4,
-            batch_size_data=args.size,
-        )
+        if "Firewall" in dataset:
+            psc = PSC(
+                model=Net_Firewall(),
+                clustering_method=kmeans,
+                sampling_ratio=0,
+                n_components=4,
+                n_neighbor=4,
+                batch_size_data=args.size,
+                random_state=rng,
+            )
+        elif "Letter" in dataset:
+            psc = PSC(
+                model=Net_Letter(),
+                clustering_method=kmeans,
+                sampling_ratio=0,
+                n_components=26,
+                n_neighbor=4,
+                batch_size_data=args.size,
+                random_state=rng,
+            )
 
         # measure total time spent
         start_time = round(time.time() * 1000)
         psc.fit(x)
         psc_index = psc.predict(x)
         end_time = round(time.time() * 1000)
 
@@ -181,16 +229,22 @@
         f.write("time spent: " + str(end_time - start_time) + "\n\n")
 
         psc_total_acc.append(psc_accRate)
         psc_total_ari.append(psc_ari)
         psc_total_ami.append(psc_ami)
 
     if "kmeans" in methods:
-        kmeans = KMeans(n_clusters=4, init="random", n_init="auto", algorithm="elkan")
-
+        if "Firewall" in dataset:
+            kmeans = KMeans(
+                n_clusters=4, init="random", n_init="auto", algorithm="elkan", random_state=rng,
+            )
+        elif "Letter" in dataset:
+            kmeans = KMeans(
+                n_clusters=26, init="random", n_init="auto", algorithm="elkan", random_state=rng,
+            )
         start_time = round(time.time() * 1000)
         kmeans_index = kmeans.fit_predict(x)
         end_time = round(time.time() * 1000)
 
         acc = Accuracy(y_true=y, y_pred=kmeans_index)
         kmeans_accRate, kmeans_ari, kmeans_ami = acc.acc_report()
 
@@ -272,8 +326,8 @@
     result.at[("KMeans", "ClusterAcc"), args.dataset] = (
         str(acc_mean) + "±" + str(acc_std)
     )
     result.at[("KMeans", "ARI"), args.dataset] = str(ari_mean) + "±" + str(ari_std)
     result.at[("KMeans", "AMI"), args.dataset] = str(ami_mean) + "±" + str(ami_std)
 
 f.close()
-result.to_csv("JSS_Experiments/table_3/result.csv")
+result.to_csv(ROOT / "table_3" / "result.csv")
```

### Comparing `ParametricSpectralClustering-0.0.2/LICENSE.txt` & `ParametricSpectralClustering-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.2/PKG-INFO` & `ParametricSpectralClustering-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParametricSpectralClustering
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for users to use parametric spectral clustering
 Home-page: 
 Author: Ivy Chang, Hsin Ju Tai
 Author-email: ivy900403@gmail.com, luludai020127@gmail.com
 License: MIT
 Keywords: Spectral Clustering,Incremental Clustering,Online Clustering,Non-linear clustering
 Classifier: Development Status :: 3 - Alpha
@@ -32,14 +32,15 @@
 
 -   Python (>= 3.8)
 -   NumPy (>= 1.26.4)
 -   SciPy (>= 1.13.0)
 -   PyTorch (>= 2.2.2)
 -   scikit-learn (>= 1.4.2)
 -   Pandas (>= 2.2.2)
+-   Matplotlib (3.8.4)
 
 ---
 
 <!-- INSTALLATION -->
 
 ## User installation
 
@@ -105,15 +106,15 @@
 
 -   NIDS Dataset: https://www.kaggle.com/datasets/aryashah2k/nfuqnidsv2-network-intrusion-detection-dataset
 
 Please place the downloaded datasets in the ‘JSS_Experiments/datasets’ directory. Ensure the datasets are correctly located before running the scripts.
 
 ```sh
 cd JSS_Experiments
-bash run.sh
+python run.py
 ```
 
 <!-- Test -->
 
 # Test
 
 To run the test, use the following command:
@@ -144,7 +145,9 @@
 
 2024/03/26
 First published
 
 2024/04/19
 Update requirements
 
+2024/05/01
+Update requirements (add Matplotlib)
```

### Comparing `ParametricSpectralClustering-0.0.2/ParametricSpectralClustering/psc.py` & `ParametricSpectralClustering-0.0.3/ParametricSpectralClustering/psc.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/PKG-INFO` & `ParametricSpectralClustering-0.0.3/ParametricSpectralClustering.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParametricSpectralClustering
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for users to use parametric spectral clustering
 Home-page: 
 Author: Ivy Chang, Hsin Ju Tai
 Author-email: ivy900403@gmail.com, luludai020127@gmail.com
 License: MIT
 Keywords: Spectral Clustering,Incremental Clustering,Online Clustering,Non-linear clustering
 Classifier: Development Status :: 3 - Alpha
@@ -32,14 +32,15 @@
 
 -   Python (>= 3.8)
 -   NumPy (>= 1.26.4)
 -   SciPy (>= 1.13.0)
 -   PyTorch (>= 2.2.2)
 -   scikit-learn (>= 1.4.2)
 -   Pandas (>= 2.2.2)
+-   Matplotlib (3.8.4)
 
 ---
 
 <!-- INSTALLATION -->
 
 ## User installation
 
@@ -105,15 +106,15 @@
 
 -   NIDS Dataset: https://www.kaggle.com/datasets/aryashah2k/nfuqnidsv2-network-intrusion-detection-dataset
 
 Please place the downloaded datasets in the ‘JSS_Experiments/datasets’ directory. Ensure the datasets are correctly located before running the scripts.
 
 ```sh
 cd JSS_Experiments
-bash run.sh
+python run.py
 ```
 
 <!-- Test -->
 
 # Test
 
 To run the test, use the following command:
@@ -144,7 +145,9 @@
 
 2024/03/26
 First published
 
 2024/04/19
 Update requirements
 
+2024/05/01
+Update requirements (add Matplotlib)
```

### Comparing `ParametricSpectralClustering-0.0.2/ParametricSpectralClustering.egg-info/SOURCES.txt` & `ParametricSpectralClustering-0.0.3/ParametricSpectralClustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.2/README.md` & `ParametricSpectralClustering-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 -   Python (>= 3.8)
 -   NumPy (>= 1.26.4)
 -   SciPy (>= 1.13.0)
 -   PyTorch (>= 2.2.2)
 -   scikit-learn (>= 1.4.2)
 -   Pandas (>= 2.2.2)
+-   Matplotlib (3.8.4)
 
 ---
 
 <!-- INSTALLATION -->
 
 ## User installation
 
@@ -87,15 +88,15 @@
 
 -   NIDS Dataset: https://www.kaggle.com/datasets/aryashah2k/nfuqnidsv2-network-intrusion-detection-dataset
 
 Please place the downloaded datasets in the ‘JSS_Experiments/datasets’ directory. Ensure the datasets are correctly located before running the scripts.
 
 ```sh
 cd JSS_Experiments
-bash run.sh
+python run.py
 ```
 
 <!-- Test -->
 
 # Test
 
 To run the test, use the following command:
```

### Comparing `ParametricSpectralClustering-0.0.2/bin/clustering.py` & `ParametricSpectralClustering-0.0.3/bin/clustering.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.2/bin/run.py` & `ParametricSpectralClustering-0.0.3/bin/run.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.2/bin/train_psc.py` & `ParametricSpectralClustering-0.0.3/bin/train_psc.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.2/setup.py` & `ParametricSpectralClustering-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "scipy>=1.13.0",
     "torch>=2.2.2",
     "torchaudio>=2.2.2",
     "torchvision>=0.17.2",
     "scikit-learn>=1.4.2",
     "pandas>=2.2.2",
     "numpy==1.26.4",
+    "matplotlib>=3.8.4",
 ]
 
 scripts = [
     "bin/clustering.py",
     "bin/train_psc.py",
     "bin/run.py",
 ]
@@ -29,15 +30,15 @@
     "Incremental Clustering",
     "Online Clustering",
     "Non-linear clustering",
 ]
 
 setup(
     name="ParametricSpectralClustering",
-    version="0.0.2",
+    version="0.0.3",
     description="A library for users to use parametric spectral clustering",
     long_description=open("README.md").read() + "\n\n" + open("CHANGELOG.txt").read(),
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["tests*"]),
     classifiers=classifiers,
     keywords=keywords,
     url="",
```

### Comparing `ParametricSpectralClustering-0.0.2/tests/test_Accuracy.py` & `ParametricSpectralClustering-0.0.3/tests/test_Accuracy.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.2/tests/test_Four_layer_FNN.py` & `ParametricSpectralClustering-0.0.3/tests/test_Four_layer_FNN.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.2/tests/test_PSC.py` & `ParametricSpectralClustering-0.0.3/tests/test_PSC.py`

 * *Files identical despite different names*

### Comparing `ParametricSpectralClustering-0.0.2/tests/test_error_handling.py` & `ParametricSpectralClustering-0.0.3/tests/test_error_handling.py`

 * *Files identical despite different names*


# Comparing `tmp/tse_motion-0.1.4.tar.gz` & `tmp/tse_motion-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tse_motion-0.1.4.tar", last modified: Thu May  9 05:21:39 2024, max compression
+gzip compressed data, was "tse_motion-0.1.5.tar", last modified: Thu May  9 05:52:35 2024, max compression
```

## Comparing `tse_motion-0.1.4.tar` & `tse_motion-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jinghangli   (501) staff       (20)        0 2024-05-09 05:21:39.037778 tse_motion-0.1.4/
--rw-r--r--   0 jinghangli   (501) staff       (20)     1068 2024-05-09 04:15:48.000000 tse_motion-0.1.4/LICENSE
--rw-r--r--   0 jinghangli   (501) staff       (20)      540 2024-05-09 05:21:39.037571 tse_motion-0.1.4/PKG-INFO
--rw-r--r--   0 jinghangli   (501) staff       (20)       12 2024-05-09 04:15:48.000000 tse_motion-0.1.4/README.md
--rw-r--r--   0 jinghangli   (501) staff       (20)       38 2024-05-09 05:21:39.037828 tse_motion-0.1.4/setup.cfg
--rw-r--r--   0 jinghangli   (501) staff       (20)      820 2024-05-09 05:20:36.000000 tse_motion-0.1.4/setup.py
-drwxr-xr-x   0 jinghangli   (501) staff       (20)        0 2024-05-09 05:21:39.036723 tse_motion-0.1.4/tse_motion.egg-info/
--rw-r--r--   0 jinghangli   (501) staff       (20)      540 2024-05-09 05:21:38.000000 tse_motion-0.1.4/tse_motion.egg-info/PKG-INFO
--rw-r--r--   0 jinghangli   (501) staff       (20)      304 2024-05-09 05:21:39.000000 tse_motion-0.1.4/tse_motion.egg-info/SOURCES.txt
--rw-r--r--   0 jinghangli   (501) staff       (20)        1 2024-05-09 05:21:38.000000 tse_motion-0.1.4/tse_motion.egg-info/dependency_links.txt
--rw-r--r--   0 jinghangli   (501) staff       (20)       66 2024-05-09 05:21:38.000000 tse_motion-0.1.4/tse_motion.egg-info/entry_points.txt
--rw-r--r--   0 jinghangli   (501) staff       (20)       32 2024-05-09 05:21:38.000000 tse_motion-0.1.4/tse_motion.egg-info/requires.txt
--rw-r--r--   0 jinghangli   (501) staff       (20)       11 2024-05-09 05:21:38.000000 tse_motion-0.1.4/tse_motion.egg-info/top_level.txt
-drwxr-xr-x   0 jinghangli   (501) staff       (20)        0 2024-05-09 05:21:39.037232 tse_motion-0.1.4/tse_rating/
--rw-r--r--   0 jinghangli   (501) staff       (20)       50 2024-05-09 04:27:43.000000 tse_motion-0.1.4/tse_rating/__init__.py
--rw-r--r--   0 jinghangli   (501) staff       (20)     1206 2024-05-09 05:20:29.000000 tse_motion-0.1.4/tse_rating/artifact_rating.py
--rw-r--r--   0 jinghangli   (501) staff       (20)      159 2024-05-09 05:16:59.000000 tse_motion-0.1.4/tse_rating/test.py
+drwxr-xr-x   0 jinghangli   (501) staff       (20)        0 2024-05-09 05:52:35.777680 tse_motion-0.1.5/
+-rw-r--r--   0 jinghangli   (501) staff       (20)     1068 2024-05-09 04:15:48.000000 tse_motion-0.1.5/LICENSE
+-rw-r--r--   0 jinghangli   (501) staff       (20)      748 2024-05-09 05:52:35.777459 tse_motion-0.1.5/PKG-INFO
+-rw-r--r--   0 jinghangli   (501) staff       (20)      221 2024-05-09 05:29:46.000000 tse_motion-0.1.5/README.md
+-rw-r--r--   0 jinghangli   (501) staff       (20)       38 2024-05-09 05:52:35.777743 tse_motion-0.1.5/setup.cfg
+-rw-r--r--   0 jinghangli   (501) staff       (20)      820 2024-05-09 05:52:04.000000 tse_motion-0.1.5/setup.py
+drwxr-xr-x   0 jinghangli   (501) staff       (20)        0 2024-05-09 05:52:35.776455 tse_motion-0.1.5/tse_motion.egg-info/
+-rw-r--r--   0 jinghangli   (501) staff       (20)      748 2024-05-09 05:52:35.000000 tse_motion-0.1.5/tse_motion.egg-info/PKG-INFO
+-rw-r--r--   0 jinghangli   (501) staff       (20)      304 2024-05-09 05:52:35.000000 tse_motion-0.1.5/tse_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 jinghangli   (501) staff       (20)        1 2024-05-09 05:52:35.000000 tse_motion-0.1.5/tse_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 jinghangli   (501) staff       (20)       66 2024-05-09 05:52:35.000000 tse_motion-0.1.5/tse_motion.egg-info/entry_points.txt
+-rw-r--r--   0 jinghangli   (501) staff       (20)       32 2024-05-09 05:52:35.000000 tse_motion-0.1.5/tse_motion.egg-info/requires.txt
+-rw-r--r--   0 jinghangli   (501) staff       (20)       11 2024-05-09 05:52:35.000000 tse_motion-0.1.5/tse_motion.egg-info/top_level.txt
+drwxr-xr-x   0 jinghangli   (501) staff       (20)        0 2024-05-09 05:52:35.777082 tse_motion-0.1.5/tse_rating/
+-rw-r--r--   0 jinghangli   (501) staff       (20)       50 2024-05-09 04:27:43.000000 tse_motion-0.1.5/tse_rating/__init__.py
+-rw-r--r--   0 jinghangli   (501) staff       (20)     1181 2024-05-09 05:29:46.000000 tse_motion-0.1.5/tse_rating/artifact_rating.py
+-rw-r--r--   0 jinghangli   (501) staff       (20)      167 2024-05-09 05:25:31.000000 tse_motion-0.1.5/tse_rating/test.py
```

### Comparing `tse_motion-0.1.4/LICENSE` & `tse_motion-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tse_motion-0.1.4/setup.py` & `tse_motion-0.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tse_motion',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         'torch',
         'monai',
         'nibabel',
         'torchvision'
     ],
```

### Comparing `tse_motion-0.1.4/tse_rating/artifact_rating.py` & `tse_motion-0.1.5/tse_rating/artifact_rating.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import nibabel as nib
 from torchvision.transforms import CenterCrop
 from monai.networks.nets import DenseNet121
 
 def rate_motion_artifact(input_path):
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
     model = DenseNet121(spatial_dims=2, in_channels=1, out_channels=5)
-    model.load_state_dict(torch.load('/Users/jinghangli/tse-score/checkpoint/weight_20.pth', map_location=device))
+    model.load_state_dict(torch.load('../checkpoint/weight_20.pth', map_location=device))
     model = model.to(device)
     model.eval()
 
     transform = CenterCrop((512, 512))
     imgs = torch.tensor(nib.load(input_path).get_fdata()).permute(-1, 0, 1).to(device).float()
     imgs = torch.stack([img/img.max() for img in imgs])
     ratings = []
```


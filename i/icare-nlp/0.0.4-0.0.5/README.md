# Comparing `tmp/icare_nlp-0.0.4.tar.gz` & `tmp/icare_nlp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icare_nlp-0.0.4.tar", last modified: Wed May  8 06:54:50 2024, max compression
+gzip compressed data, was "icare_nlp-0.0.5.tar", last modified: Thu May  9 08:57:18 2024, max compression
```

## Comparing `icare_nlp-0.0.4.tar` & `icare_nlp-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/
--rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/PKG-INFO
--rw-rw-r--   0 yi        (1000) yi        (1000)      327 2024-05-02 05:18:30.000000 icare_nlp-0.0.4/README.md
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/icare_nlp/
--rw-rw-r--   0 yi        (1000) yi        (1000)       49 2024-05-01 13:47:31.000000 icare_nlp-0.0.4/icare_nlp/__init__.py
--rw-rw-r--   0 yi        (1000) yi        (1000)     2803 2024-05-06 06:31:01.000000 icare_nlp-0.0.4/icare_nlp/object_desc.py
--rw-rw-r--   0 yi        (1000) yi        (1000)     7433 2024-05-06 06:49:59.000000 icare_nlp-0.0.4/icare_nlp/object_qa.py
--rw-rw-r--   0 yi        (1000) yi        (1000)      650 2024-05-08 06:52:37.000000 icare_nlp-0.0.4/icare_nlp/receipt_desc.py
--rw-rw-r--   0 yi        (1000) yi        (1000)      459 2024-05-08 06:52:37.000000 icare_nlp-0.0.4/icare_nlp/receipt_qa.py
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/icare_nlp/resources/
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-05-02 04:39:47.000000 icare_nlp-0.0.4/icare_nlp/resources/__init__.py
--rw-rw-r--   0 yi        (1000) yi        (1000)   247000 2024-04-30 13:33:50.000000 icare_nlp-0.0.4/icare_nlp/resources/category_emb_tensor.pt
--rw-rw-r--   0 yi        (1000) yi        (1000)    15275 2024-05-02 05:01:02.000000 icare_nlp-0.0.4/icare_nlp/resources/category_tactile_description.json
--rw-rw-r--   0 yi        (1000) yi        (1000)     6623 2024-05-06 04:31:11.000000 icare_nlp-0.0.4/icare_nlp/resources/desc_words.json
--rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 12:13:21.000000 icare_nlp-0.0.4/icare_nlp/resources/inv_yolo_obj_class_def.json
--rw-rw-r--   0 yi        (1000) yi        (1000)      261 2024-04-30 12:07:36.000000 icare_nlp-0.0.4/icare_nlp/resources/invert.py
--rw-rw-r--   0 yi        (1000) yi        (1000)    11708 2024-04-30 13:50:11.000000 icare_nlp-0.0.4/icare_nlp/resources/object_types.py
--rw-rw-r--   0 yi        (1000) yi        (1000)     3529 2024-04-30 13:33:44.000000 icare_nlp-0.0.4/icare_nlp/resources/rev_yolo_obj_class_def.json
--rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 13:35:28.000000 icare_nlp-0.0.4/icare_nlp/resources/yolo_obj_class_def.json
--rw-rw-r--   0 yi        (1000) yi        (1000)     2999 2024-05-06 06:31:39.000000 icare_nlp-0.0.4/icare_nlp/utils.py
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/icare_nlp.egg-info/
--rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-08 06:54:50.000000 icare_nlp-0.0.4/icare_nlp.egg-info/PKG-INFO
--rw-rw-r--   0 yi        (1000) yi        (1000)      660 2024-05-08 06:54:50.000000 icare_nlp-0.0.4/icare_nlp.egg-info/SOURCES.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-08 06:54:50.000000 icare_nlp-0.0.4/icare_nlp.egg-info/dependency_links.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)       10 2024-05-08 06:54:50.000000 icare_nlp-0.0.4/icare_nlp.egg-info/top_level.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)       38 2024-05-08 06:54:50.577597 icare_nlp-0.0.4/setup.cfg
--rw-rw-r--   0 yi        (1000) yi        (1000)      438 2024-05-08 06:53:03.000000 icare_nlp-0.0.4/setup.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-09 08:57:18.752493 icare_nlp-0.0.5/
+-rw-r--r--   0 yi        (1000) yi        (1000)     5904 2024-05-09 08:57:18.752493 icare_nlp-0.0.5/PKG-INFO
+-rw-rw-r--   0 yi        (1000) yi        (1000)     5696 2024-05-09 08:14:45.000000 icare_nlp-0.0.5/README.md
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-09 08:57:18.752493 icare_nlp-0.0.5/icare_nlp/
+-rw-rw-r--   0 yi        (1000) yi        (1000)       29 2024-05-02 04:42:22.000000 icare_nlp-0.0.5/icare_nlp/MANIFEST.in
+-rw-rw-r--   0 yi        (1000) yi        (1000)       49 2024-05-01 13:47:31.000000 icare_nlp-0.0.5/icare_nlp/__init__.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     2803 2024-05-06 06:31:01.000000 icare_nlp-0.0.5/icare_nlp/object_desc.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     7433 2024-05-06 06:49:59.000000 icare_nlp-0.0.5/icare_nlp/object_qa.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)      650 2024-05-08 06:52:37.000000 icare_nlp-0.0.5/icare_nlp/receipt_desc.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     3295 2024-05-08 13:49:06.000000 icare_nlp-0.0.5/icare_nlp/receipt_qa.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-09 08:57:18.752493 icare_nlp-0.0.5/icare_nlp/resources/
+-rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-05-02 04:39:47.000000 icare_nlp-0.0.5/icare_nlp/resources/__init__.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)   247000 2024-04-30 13:33:50.000000 icare_nlp-0.0.5/icare_nlp/resources/category_emb_tensor.pt
+-rw-rw-r--   0 yi        (1000) yi        (1000)    15275 2024-05-02 05:01:02.000000 icare_nlp-0.0.5/icare_nlp/resources/category_tactile_description.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     6623 2024-05-06 04:31:11.000000 icare_nlp-0.0.5/icare_nlp/resources/desc_words.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 12:13:21.000000 icare_nlp-0.0.5/icare_nlp/resources/inv_yolo_obj_class_def.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)      261 2024-04-30 12:07:36.000000 icare_nlp-0.0.5/icare_nlp/resources/invert.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)    11708 2024-04-30 13:50:11.000000 icare_nlp-0.0.5/icare_nlp/resources/object_types.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     3529 2024-04-30 13:33:44.000000 icare_nlp-0.0.5/icare_nlp/resources/rev_yolo_obj_class_def.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 13:35:28.000000 icare_nlp-0.0.5/icare_nlp/resources/yolo_obj_class_def.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     4027 2024-05-09 07:12:33.000000 icare_nlp-0.0.5/icare_nlp/task_disp.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     2999 2024-05-06 06:31:39.000000 icare_nlp-0.0.5/icare_nlp/utils.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-09 08:57:18.752493 icare_nlp-0.0.5/icare_nlp.egg-info/
+-rw-r--r--   0 yi        (1000) yi        (1000)     5904 2024-05-09 08:57:18.000000 icare_nlp-0.0.5/icare_nlp.egg-info/PKG-INFO
+-rw-rw-r--   0 yi        (1000) yi        (1000)      705 2024-05-09 08:57:18.000000 icare_nlp-0.0.5/icare_nlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-09 08:57:18.000000 icare_nlp-0.0.5/icare_nlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)       10 2024-05-09 08:57:18.000000 icare_nlp-0.0.5/icare_nlp.egg-info/top_level.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)       38 2024-05-09 08:57:18.752493 icare_nlp-0.0.5/setup.cfg
+-rw-rw-r--   0 yi        (1000) yi        (1000)      616 2024-05-09 08:56:31.000000 icare_nlp-0.0.5/setup.py
```

### Comparing `icare_nlp-0.0.4/icare_nlp/object_desc.py` & `icare_nlp-0.0.5/icare_nlp/object_desc.py`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/object_qa.py` & `icare_nlp-0.0.5/icare_nlp/object_qa.py`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/receipt_desc.py` & `icare_nlp-0.0.5/icare_nlp/receipt_desc.py`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/resources/category_emb_tensor.pt` & `icare_nlp-0.0.5/icare_nlp/resources/category_emb_tensor.pt`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/resources/category_tactile_description.json` & `icare_nlp-0.0.5/icare_nlp/resources/category_tactile_description.json`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/resources/desc_words.json` & `icare_nlp-0.0.5/icare_nlp/resources/desc_words.json`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/resources/inv_yolo_obj_class_def.json` & `icare_nlp-0.0.5/icare_nlp/resources/inv_yolo_obj_class_def.json`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/resources/object_types.py` & `icare_nlp-0.0.5/icare_nlp/resources/object_types.py`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/resources/rev_yolo_obj_class_def.json` & `icare_nlp-0.0.5/icare_nlp/resources/rev_yolo_obj_class_def.json`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/resources/yolo_obj_class_def.json` & `icare_nlp-0.0.5/icare_nlp/resources/yolo_obj_class_def.json`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp/utils.py` & `icare_nlp-0.0.5/icare_nlp/utils.py`

 * *Files identical despite different names*

### Comparing `icare_nlp-0.0.4/icare_nlp.egg-info/SOURCES.txt` & `icare_nlp-0.0.5/icare_nlp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 README.md
 setup.py
+icare_nlp/MANIFEST.in
 icare_nlp/__init__.py
 icare_nlp/object_desc.py
 icare_nlp/object_qa.py
 icare_nlp/receipt_desc.py
 icare_nlp/receipt_qa.py
+icare_nlp/task_disp.py
 icare_nlp/utils.py
 icare_nlp.egg-info/PKG-INFO
 icare_nlp.egg-info/SOURCES.txt
 icare_nlp.egg-info/dependency_links.txt
 icare_nlp.egg-info/top_level.txt
 icare_nlp/resources/__init__.py
 icare_nlp/resources/category_emb_tensor.pt
```


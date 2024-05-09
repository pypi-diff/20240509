# Comparing `tmp/hedge_lab_ct-0.1.3.tar.gz` & `tmp/hedge_lab_ct-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedge_lab_ct-0.1.3.tar", last modified: Wed May  8 15:57:42 2024, max compression
+gzip compressed data, was "hedge_lab_ct-0.1.4.tar", last modified: Thu May  9 01:13:40 2024, max compression
```

## Comparing `hedge_lab_ct-0.1.3.tar` & `hedge_lab_ct-0.1.4.tar`

### file list

```diff
@@ -1,49 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:57:42.973615 hedge_lab_ct-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 15:57:42.969615 hedge_lab_ct-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:57:42.965615 hedge_lab_ct-0.1.3/cv-lab-aurct/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:57:42.969615 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/1.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/10.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/11.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/14.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/15.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/4.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/5.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/6.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/7.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/8.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/9.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex10.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex2a.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex2c.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex4.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex5a.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex5b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex5c.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex6.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex7.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex8.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex81.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/ex9.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/kalman.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/cv-lab-aurct/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:57:42.969615 hedge_lab_ct-0.1.3/hedge_lab_ct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 15:57:42.000000 hedge_lab_ct-0.1.3/hedge_lab_ct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 15:57:42.000000 hedge_lab_ct-0.1.3/hedge_lab_ct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:57:42.000000 hedge_lab_ct-0.1.3/hedge_lab_ct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 15:57:42.000000 hedge_lab_ct-0.1.3/hedge_lab_ct.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:57:42.973615 hedge_lab_ct-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-08 15:57:36.000000 hedge_lab_ct-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:13:40.319169 hedge_lab_ct-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 01:13:40.319169 hedge_lab_ct-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:13:40.315169 hedge_lab_ct-0.1.4/cv-lab-aurct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:13:40.319169 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/9.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19575 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/cv-lab-aurct/ex/tesla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:13:40.319169 hedge_lab_ct-0.1.4/hedge_lab_ct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 01:13:40.000000 hedge_lab_ct-0.1.4/hedge_lab_ct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-09 01:13:40.000000 hedge_lab_ct-0.1.4/hedge_lab_ct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:13:40.000000 hedge_lab_ct-0.1.4/hedge_lab_ct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 01:13:40.000000 hedge_lab_ct-0.1.4/hedge_lab_ct.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 01:13:40.319169 hedge_lab_ct-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-09 01:13:36.000000 hedge_lab_ct-0.1.4/setup.py
```

### Comparing `hedge_lab_ct-0.1.3/LICENSE` & `hedge_lab_ct-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/1.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/1.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/10.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/9.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/11.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/10.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/12.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/11.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/13.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/12.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/14.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/13.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/15.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/15.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/2.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/2.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/4.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/3.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/5.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/4.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/8.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/7.py`

 * *Files identical despite different names*

### Comparing `hedge_lab_ct-0.1.3/cv-lab-aurct/ex/9.py` & `hedge_lab_ct-0.1.4/cv-lab-aurct/ex/8.py`

 * *Files identical despite different names*


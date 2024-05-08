# Comparing `tmp/grader_helper-0.1.5.tar.gz` & `tmp/grader_helper-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grader_helper-0.1.5.tar", max compression
+gzip compressed data, was "grader_helper-0.1.6.tar", max compression
```

## Comparing `grader_helper-0.1.5.tar` & `grader_helper-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      794 2024-05-06 22:37:50.633298 grader_helper-0.1.5/grader_helper/__init__.py
--rw-r--r--   0        0        0     1607 2024-05-06 19:47:00.017889 grader_helper-0.1.5/grader_helper/distribute_feedback_sheets.py
--rw-r--r--   0        0        0     2592 2024-05-06 19:47:00.030900 grader_helper-0.1.5/grader_helper/distribute_graders_groups.py
--rw-r--r--   0        0        0     1967 2024-05-06 19:46:59.931883 grader_helper-0.1.5/grader_helper/distribute_graders_individual.py
--rw-r--r--   0        0        0     1483 2024-05-06 19:47:00.070903 grader_helper-0.1.5/grader_helper/import_brightspace_classlist.py
--rw-r--r--   0        0        0      644 2024-05-06 20:26:06.293171 grader_helper-0.1.5/grader_helper/load_graders.py
--rw-r--r--   0        0        0     4817 2024-05-06 23:29:36.953441 grader_helper-0.1.5/grader_helper/rename_folders.py
--rw-r--r--   0        0        0     1604 2024-05-06 22:39:35.413885 grader_helper-0.1.5/grader_helper/save_distributed_graders.py
--rw-r--r--   0        0        0     2189 2024-05-06 19:47:00.142422 grader_helper-0.1.5/grader_helper/save_grader_sheets.py
--rw-r--r--   0        0        0      441 2024-05-06 23:30:00.726720 grader_helper-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 20:05:58.335712 grader_helper-0.1.5/README.md
--rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 grader_helper-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      794 2024-05-06 22:37:50.633298 grader_helper-0.1.6/grader_helper/__init__.py
+-rw-r--r--   0        0        0     1607 2024-05-06 19:47:00.017889 grader_helper-0.1.6/grader_helper/distribute_feedback_sheets.py
+-rw-r--r--   0        0        0     2592 2024-05-06 19:47:00.030900 grader_helper-0.1.6/grader_helper/distribute_graders_groups.py
+-rw-r--r--   0        0        0     1967 2024-05-06 19:46:59.931883 grader_helper-0.1.6/grader_helper/distribute_graders_individual.py
+-rw-r--r--   0        0        0     1483 2024-05-06 19:47:00.070903 grader_helper-0.1.6/grader_helper/import_brightspace_classlist.py
+-rw-r--r--   0        0        0      644 2024-05-06 20:26:06.293171 grader_helper-0.1.6/grader_helper/load_graders.py
+-rw-r--r--   0        0        0     4817 2024-05-06 23:29:36.953441 grader_helper-0.1.6/grader_helper/rename_folders.py
+-rw-r--r--   0        0        0     1604 2024-05-06 22:39:35.413885 grader_helper-0.1.6/grader_helper/save_distributed_graders.py
+-rw-r--r--   0        0        0     2189 2024-05-06 19:47:00.142422 grader_helper-0.1.6/grader_helper/save_grader_sheets.py
+-rw-r--r--   0        0        0      462 2024-05-08 22:40:43.966485 grader_helper-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      731 2024-05-07 10:51:10.000000 grader_helper-0.1.6/README.md
+-rw-r--r--   0        0        0     1237 1970-01-01 00:00:00.000000 grader_helper-0.1.6/PKG-INFO
```

### Comparing `grader_helper-0.1.5/grader_helper/__init__.py` & `grader_helper-0.1.6/grader_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.5/grader_helper/distribute_feedback_sheets.py` & `grader_helper-0.1.6/grader_helper/distribute_feedback_sheets.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.5/grader_helper/distribute_graders_groups.py` & `grader_helper-0.1.6/grader_helper/distribute_graders_groups.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.5/grader_helper/distribute_graders_individual.py` & `grader_helper-0.1.6/grader_helper/distribute_graders_individual.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.5/grader_helper/import_brightspace_classlist.py` & `grader_helper-0.1.6/grader_helper/import_brightspace_classlist.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.5/grader_helper/load_graders.py` & `grader_helper-0.1.6/grader_helper/load_graders.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.5/grader_helper/rename_folders.py` & `grader_helper-0.1.6/grader_helper/rename_folders.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.5/grader_helper/save_distributed_graders.py` & `grader_helper-0.1.6/grader_helper/save_distributed_graders.py`

 * *Files identical despite different names*

### Comparing `grader_helper-0.1.5/grader_helper/save_grader_sheets.py` & `grader_helper-0.1.6/grader_helper/save_grader_sheets.py`

 * *Files identical despite different names*


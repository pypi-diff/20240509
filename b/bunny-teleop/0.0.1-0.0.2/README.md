# Comparing `tmp/bunny_teleop-0.0.1-py3-none-any.whl.zip` & `tmp/bunny_teleop-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6556 bytes, number of entries: 10
--rw-rw-r--  2.0 unx       22 b- defN 24-Apr-27 01:32 bunny_teleop/__init__.py
--rw-rw-r--  2.0 unx     4455 b- defN 24-May-06 05:38 bunny_teleop/bimanual_teleop_client.py
--rw-rw-r--  2.0 unx     3504 b- defN 24-May-06 05:38 bunny_teleop/bimanual_teleop_server.py
--rw-rw-r--  2.0 unx     3491 b- defN 24-Apr-27 01:26 bunny_teleop/init_config.py
--rw-rw-r--  2.0 unx     1090 b- defN 24-May-06 08:29 bunny_teleop-0.0.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1233 b- defN 24-May-06 08:29 bunny_teleop-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-06 08:29 bunny_teleop-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 24-May-06 08:29 bunny_teleop-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 24-May-06 08:29 bunny_teleop-0.0.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      855 b- defN 24-May-06 08:29 bunny_teleop-0.0.1.dist-info/RECORD
-10 files, 14756 bytes uncompressed, 5078 bytes compressed:  65.6%
+Zip file size: 7500 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       22 b- defN 24-May-09 06:02 bunny_teleop/__init__.py
+-rw-r--r--  2.0 unx     4455 b- defN 24-May-09 06:02 bunny_teleop/bimanual_teleop_client.py
+-rw-r--r--  2.0 unx     3504 b- defN 24-May-09 06:02 bunny_teleop/bimanual_teleop_server.py
+-rw-r--r--  2.0 unx     3491 b- defN 24-May-09 06:02 bunny_teleop/init_config.py
+-rw-r--r--  2.0 unx     1090 b- defN 24-May-09 06:02 bunny_teleop-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3811 b- defN 24-May-09 06:02 bunny_teleop-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 06:02 bunny_teleop-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-09 06:02 bunny_teleop-0.0.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-09 06:02 bunny_teleop-0.0.2.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      855 b- defN 24-May-09 06:02 bunny_teleop-0.0.2.dist-info/RECORD
+10 files, 17334 bytes uncompressed, 6022 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: bunny_teleop/bimanual_teleop_server.py
 Comment: 
 
 Filename: bunny_teleop/init_config.py
 Comment: 
 
-Filename: bunny_teleop-0.0.1.dist-info/LICENSE
+Filename: bunny_teleop-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: bunny_teleop-0.0.1.dist-info/METADATA
+Filename: bunny_teleop-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: bunny_teleop-0.0.1.dist-info/WHEEL
+Filename: bunny_teleop-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: bunny_teleop-0.0.1.dist-info/top_level.txt
+Filename: bunny_teleop-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: bunny_teleop-0.0.1.dist-info/zip-safe
+Filename: bunny_teleop-0.0.2.dist-info/zip-safe
 Comment: 
 
-Filename: bunny_teleop-0.0.1.dist-info/RECORD
+Filename: bunny_teleop-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bunny_teleop/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## Comparing `bunny_teleop-0.0.1.dist-info/LICENSE` & `bunny_teleop-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bunny_teleop-0.0.1.dist-info/RECORD` & `bunny_teleop-0.0.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-bunny_teleop/__init__.py,sha256=sXLh7g3KC4QCFxcZGBTpG2scR7hmmBsMjq6LqRptkRg,22
+bunny_teleop/__init__.py,sha256=QvlVh4JTl3JL7jQAja76yKtT-IvF4631ASjWY1wS6AQ,22
 bunny_teleop/bimanual_teleop_client.py,sha256=DFHvJHHsygpx0PSohmRa9gLFFWA_GZxcN5MuR00F564,4455
 bunny_teleop/bimanual_teleop_server.py,sha256=xKEvKOSqFb54kOmt1FEflVKJnZWlF10jIXFThVljmwU,3504
 bunny_teleop/init_config.py,sha256=txLUl9Eavm0v-5DCL86V5F8EWn_0QdzfcDmXW1AppBo,3491
-bunny_teleop-0.0.1.dist-info/LICENSE,sha256=0lv53JzxV6sTZTXgqbXC-5rdyt9GLtWNuRv8yurN5ik,1090
-bunny_teleop-0.0.1.dist-info/METADATA,sha256=AzcZMJHEsFL9VVM0MXkKjVNqWoTCrXxyNpx7UuAHOmY,1233
-bunny_teleop-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-bunny_teleop-0.0.1.dist-info/top_level.txt,sha256=nC-Fe0Wq-crhY2kryT8sGSVYXl0dm4p_u1eqmHmQQsE,13
-bunny_teleop-0.0.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-bunny_teleop-0.0.1.dist-info/RECORD,,
+bunny_teleop-0.0.2.dist-info/LICENSE,sha256=0lv53JzxV6sTZTXgqbXC-5rdyt9GLtWNuRv8yurN5ik,1090
+bunny_teleop-0.0.2.dist-info/METADATA,sha256=gP70oX8qgHHgx4z9iiulCv_u1PyJOWyDLSdk8OOZMIg,3811
+bunny_teleop-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+bunny_teleop-0.0.2.dist-info/top_level.txt,sha256=nC-Fe0Wq-crhY2kryT8sGSVYXl0dm4p_u1eqmHmQQsE,13
+bunny_teleop-0.0.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+bunny_teleop-0.0.2.dist-info/RECORD,,
```


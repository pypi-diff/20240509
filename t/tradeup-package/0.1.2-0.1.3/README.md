# Comparing `tmp/tradeup_package-0.1.2.tar.gz` & `tmp/tradeup_package-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradeup_package-0.1.2.tar", last modified: Thu May  2 19:21:33 2024, max compression
+gzip compressed data, was "tradeup_package-0.1.3.tar", last modified: Thu May  9 15:36:54 2024, max compression
```

## Comparing `tradeup_package-0.1.2.tar` & `tradeup_package-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-02 19:21:33.086153 tradeup_package-0.1.2/
--rw-rw-r--   0 script.master  (1001) script.master  (1001)     1068 2024-04-26 19:46:29.000000 tradeup_package-0.1.2/LICENSE
--rw-r--r--   0 script.master  (1001) script.master  (1001)      281 2024-05-02 19:21:33.086153 tradeup_package-0.1.2/PKG-INFO
--rw-rw-r--   0 script.master  (1001) script.master  (1001)     1041 2024-05-02 19:21:02.000000 tradeup_package-0.1.2/README.md
--rw-rw-r--   0 script.master  (1001) script.master  (1001)      323 2024-05-02 19:20:23.000000 tradeup_package-0.1.2/pyproject.toml
--rw-rw-r--   0 script.master  (1001) script.master  (1001)       38 2024-05-02 19:21:33.086153 tradeup_package-0.1.2/setup.cfg
-drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-02 19:21:33.086153 tradeup_package-0.1.2/tradeup/
--rw-rw-r--   0 script.master  (1001) script.master  (1001)     6195 2024-05-02 19:20:16.000000 tradeup_package-0.1.2/tradeup/Public.py
--rw-rw-r--   0 script.master  (1001) script.master  (1001)       21 2023-10-04 18:16:32.000000 tradeup_package-0.1.2/tradeup/__init__.py
-drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-02 19:21:33.086153 tradeup_package-0.1.2/tradeup_package.egg-info/
--rw-r--r--   0 script.master  (1001) script.master  (1001)      281 2024-05-02 19:21:33.000000 tradeup_package-0.1.2/tradeup_package.egg-info/PKG-INFO
--rw-rw-r--   0 script.master  (1001) script.master  (1001)      226 2024-05-02 19:21:33.000000 tradeup_package-0.1.2/tradeup_package.egg-info/SOURCES.txt
--rw-rw-r--   0 script.master  (1001) script.master  (1001)        1 2024-05-02 19:21:33.000000 tradeup_package-0.1.2/tradeup_package.egg-info/dependency_links.txt
--rw-rw-r--   0 script.master  (1001) script.master  (1001)        8 2024-05-02 19:21:33.000000 tradeup_package-0.1.2/tradeup_package.egg-info/top_level.txt
+drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)     1068 2024-04-26 19:46:29.000000 tradeup_package-0.1.3/LICENSE
+-rw-r--r--   0 script.master  (1001) script.master  (1001)      281 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/PKG-INFO
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)     1131 2024-05-09 15:33:22.000000 tradeup_package-0.1.3/README.md
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)      323 2024-05-09 15:31:52.000000 tradeup_package-0.1.3/pyproject.toml
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)       38 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/setup.cfg
+drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/tradeup/
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)     6193 2024-05-08 13:36:19.000000 tradeup_package-0.1.3/tradeup/Public.py
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)       21 2023-10-04 18:16:32.000000 tradeup_package-0.1.3/tradeup/__init__.py
+drwxrwxr-x   0 script.master  (1001) script.master  (1001)        0 2024-05-09 15:36:54.686897 tradeup_package-0.1.3/tradeup_package.egg-info/
+-rw-r--r--   0 script.master  (1001) script.master  (1001)      281 2024-05-09 15:36:54.000000 tradeup_package-0.1.3/tradeup_package.egg-info/PKG-INFO
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)      226 2024-05-09 15:36:54.000000 tradeup_package-0.1.3/tradeup_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)        1 2024-05-09 15:36:54.000000 tradeup_package-0.1.3/tradeup_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 script.master  (1001) script.master  (1001)        8 2024-05-09 15:36:54.000000 tradeup_package-0.1.3/tradeup_package.egg-info/top_level.txt
```

### Comparing `tradeup_package-0.1.2/LICENSE` & `tradeup_package-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tradeup_package-0.1.2/README.md` & `tradeup_package-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,8 +16,11 @@
 Release note 0.0.5   2023/11/29 16:43
 Created function create_partition(), automatically create partition of next month for each table, with hard coded user name and password
 
 Release note 0.1.1   2024/05/02 10:59
 Defined all functions under class Amazon as static method, no need to include argument 'self' when calling functions
 
 Release note 0.1.2   2024/05/02 15:20
-Excluded all 'self' under class amazon
+Excluded all 'self' under class amazon
+
+## Release note 0.1.3   2024/05/09 11:32
+Minor bug fix, correct typos in check_holiday()
```

### Comparing `tradeup_package-0.1.2/tradeup/Public.py` & `tradeup_package-0.1.3/tradeup/Public.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         return password    
     
     @staticmethod
     def check_holiday(date_obj, con, which='NYSE_Holiday'):
         date_str = date_obj.strftime("%Y-%m-%d")
         df = wr.redshift.read_sql_query(
             sql=f"""
-                SELECT "{which}" FROM Holiday.Holiday WHERE "Date" ='{date_str}'
+                SELECT "{which}" FROM holiday.holiday WHERE date ='{date_str}'
                 """,
             con=con
         )
         
         # not in holiday list
         if len(df) == 0:
             return False
```


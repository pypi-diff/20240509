# Comparing `tmp/plist_tracker-0.1.1.tar.gz` & `tmp/plist_tracker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plist_tracker-0.1.1.tar", max compression
+gzip compressed data, was "plist_tracker-0.1.2.tar", max compression
```

## Comparing `plist_tracker-0.1.1.tar` & `plist_tracker-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-09 13:13:18.078788 plist_tracker-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-09 13:13:18.078729 plist_tracker-0.1.1/plist_tracker/__init__.py
--rw-r--r--   0        0        0       41 2024-05-09 13:18:04.710333 plist_tracker-0.1.1/plist_tracker/__main__.py
--rw-r--r--   0        0        0     4234 2024-05-09 15:11:21.947008 plist_tracker-0.1.1/plist_tracker/cli.py
--rw-r--r--   0        0        0      453 2024-05-09 15:11:45.697889 plist_tracker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 plist_tracker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-09 13:13:18.078788 plist_tracker-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 13:13:18.078729 plist_tracker-0.1.2/plist_tracker/__init__.py
+-rw-r--r--   0        0        0       41 2024-05-09 13:18:04.710333 plist_tracker-0.1.2/plist_tracker/__main__.py
+-rw-r--r--   0        0        0     4189 2024-05-09 15:14:16.107352 plist_tracker-0.1.2/plist_tracker/cli.py
+-rw-r--r--   0        0        0      453 2024-05-09 15:14:21.431065 plist_tracker-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 plist_tracker-0.1.2/PKG-INFO
```

### Comparing `plist_tracker-0.1.1/plist_tracker/cli.py` & `plist_tracker-0.1.2/plist_tracker/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,17 +103,14 @@
 def main():
     temp_dir = Path(tempfile.mkdtemp())
     temp_system = temp_dir.joinpath("sys")
     temp_user = temp_dir.joinpath("usr")
     src_system = Path("/Library/Preferences")
     src_user = Path.home().joinpath("Library/Preferences")
 
-    print(temp_system)
-    print(temp_user)
-
     try:
         shutil.copytree(src_system, temp_system)
     except:
         pass
 
     try:
         shutil.copytree(src_user, temp_user)
```


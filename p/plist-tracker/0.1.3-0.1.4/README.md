# Comparing `tmp/plist_tracker-0.1.3.tar.gz` & `tmp/plist_tracker-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plist_tracker-0.1.3.tar", max compression
+gzip compressed data, was "plist_tracker-0.1.4.tar", max compression
```

## Comparing `plist_tracker-0.1.3.tar` & `plist_tracker-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-09 13:13:18.078788 plist_tracker-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-09 13:13:18.078729 plist_tracker-0.1.3/plist_tracker/__init__.py
--rw-r--r--   0        0        0       41 2024-05-09 13:18:04.710333 plist_tracker-0.1.3/plist_tracker/__main__.py
--rw-r--r--   0        0        0     4408 2024-05-09 15:21:45.699879 plist_tracker-0.1.3/plist_tracker/cli.py
--rw-r--r--   0        0        0      453 2024-05-09 15:22:28.316982 plist_tracker-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 plist_tracker-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-09 13:13:18.078788 plist_tracker-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 13:13:18.078729 plist_tracker-0.1.4/plist_tracker/__init__.py
+-rw-r--r--   0        0        0       41 2024-05-09 13:18:04.710333 plist_tracker-0.1.4/plist_tracker/__main__.py
+-rw-r--r--   0        0        0     4408 2024-05-09 18:46:41.770071 plist_tracker-0.1.4/plist_tracker/cli.py
+-rw-r--r--   0        0        0      453 2024-05-09 18:49:03.292377 plist_tracker-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 plist_tracker-0.1.4/PKG-INFO
```

### Comparing `plist_tracker-0.1.3/plist_tracker/cli.py` & `plist_tracker-0.1.4/plist_tracker/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     except:
         print(f"Error while removing temp dir. You can remove it manually: {temp_dir}")
 
 
 def _compare_files(src_path: Path, tmp_path: Path) -> List[DiffItem]:
     usr_cmp = filecmp.dircmp(src_path, tmp_path)
     result = [
-        DiffItem(src_path.joinpath(file), tmp_path.joinpath(file), file)
+        DiffItem(tmp_path.joinpath(file), src_path.joinpath(file), file)
         for file in usr_cmp.diff_files
     ]
     for item in result:
         item.compute_diff()
 
     return result
```


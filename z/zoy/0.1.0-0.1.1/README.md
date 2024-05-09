# Comparing `tmp/zoy-0.1.0.tar.gz` & `tmp/zoy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoy-0.1.0.tar", max compression
+gzip compressed data, was "zoy-0.1.1.tar", max compression
```

## Comparing `zoy-0.1.0.tar` & `zoy-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      389 2024-05-09 09:02:16.089476 zoy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       90 2024-05-09 08:50:52.974895 zoy-0.1.0/README.md
--rw-r--r--   0        0        0       21 2024-05-09 09:34:25.973841 zoy-0.1.0/zoy/__init__.py
--rw-r--r--   0        0        0      612 2024-05-09 09:03:59.661451 zoy-0.1.0/zoy/__main__.py
--rw-r--r--   0        0        0     1007 2024-05-09 09:04:10.596425 zoy-0.1.0/zoy/zoy.py
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 zoy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      436 2024-05-09 10:05:58.048076 zoy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      434 2024-05-09 10:02:40.346058 zoy-0.1.1/README.md
+-rw-r--r--   0        0        0       45 2024-05-09 10:06:03.983135 zoy-0.1.1/zoy/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-09 10:04:09.316799 zoy-0.1.1/zoy/__main__.py
+-rw-r--r--   0        0        0     1561 2024-05-09 10:03:53.543148 zoy-0.1.1/zoy/zoy.py
+-rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 zoy-0.1.1/PKG-INFO
```

### Comparing `zoy-0.1.0/zoy/zoy.py` & `zoy-0.1.1/zoy/zoy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 
 def count_lines_files_dirs(directory):
     total_lines = 0
     file_count = 0
     dir_count = 0
     tree = []
 
@@ -25,7 +26,25 @@
                 with open(entry_path, "r", encoding="utf-8") as f:
                     lines = f.readlines()
                     total_lines += len(lines)
                 tree.append("  " * level + "📄 " + entry)
 
     build_tree(directory)
     return total_lines, file_count, dir_count, tree
+
+def main():
+    if len(sys.argv) > 1:
+        directory_path = sys.argv[1]
+    else:
+        directory_path = input("Enter the directory path: ")
+    
+    total_lines, file_count, dir_count, tree = count_lines_files_dirs(directory_path)
+
+    print("Project Structure: ")
+    for line in tree:
+        print(line)
+
+    print("\n=========================================")
+
+    print(f"\nTotal Python files: {file_count}")
+    print(f"Total lines in Python files: {total_lines}")
+    print(f"Total directories: {dir_count}")
```


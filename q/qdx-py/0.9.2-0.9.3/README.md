# Comparing `tmp/qdx_py-0.9.2.tar.gz` & `tmp/qdx_py-0.9.3.tar.gz`

## Comparing `qdx_py-0.9.2.tar` & `qdx_py-0.9.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 qdx_py-0.9.2/Cargo.toml
--rw-r--r--   0     1000      100     2809 2023-11-16 02:44:04.000000 qdx_py-0.9.2/.github/workflows/CI.yml
--rw-r--r--   0     1000      100      685 2023-11-16 02:44:04.000000 qdx_py-0.9.2/.gitignore
--rw-r--r--   0     1000      100     2028 2024-04-04 02:54:02.000000 qdx_py-0.9.2/README.md
--rw-r--r--   0     1000      100      513 2024-04-15 06:01:05.000000 qdx_py-0.9.2/src/lib.rs
--rw-r--r--   0     1000      100     7083 2024-04-15 05:53:38.000000 qdx_py-0.9.2/src/qdx.rs
--rw-r--r--   0     1000      100    27482 2024-04-23 06:08:13.000000 qdx_py-0.9.2/Cargo.lock
--rw-r--r--   0     1000      100      366 2023-12-01 06:07:08.000000 qdx_py-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 qdx_py-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 qdx_py-0.9.3/Cargo.toml
+-rw-r--r--   0     1000      100     2809 2023-11-16 02:44:04.000000 qdx_py-0.9.3/.github/workflows/CI.yml
+-rw-r--r--   0     1000      100      685 2023-11-16 02:44:04.000000 qdx_py-0.9.3/.gitignore
+-rw-r--r--   0     1000      100     2028 2024-04-04 02:54:02.000000 qdx_py-0.9.3/README.md
+-rw-r--r--   0     1000      100      513 2024-04-15 06:01:05.000000 qdx_py-0.9.3/src/lib.rs
+-rw-r--r--   0     1000      100     7083 2024-04-15 05:53:38.000000 qdx_py-0.9.3/src/qdx.rs
+-rw-r--r--   0     1000      100    27482 2024-05-09 08:02:32.000000 qdx_py-0.9.3/Cargo.lock
+-rw-r--r--   0     1000      100      366 2023-12-01 06:07:08.000000 qdx_py-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 qdx_py-0.9.3/PKG-INFO
```

### Comparing `qdx_py-0.9.2/Cargo.toml` & `qdx_py-0.9.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qdx-py"
-version = "0.9.2"
+version = "0.9.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "qdx_py"
 crate-type = ["rlib", "cdylib"]
```

### Comparing `qdx_py-0.9.2/.github/workflows/CI.yml` & `qdx_py-0.9.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.2/.gitignore` & `qdx_py-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.2/README.md` & `qdx_py-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.2/src/lib.rs` & `qdx_py-0.9.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.2/src/qdx.rs` & `qdx_py-0.9.3/src/qdx.rs`

 * *Files identical despite different names*

### Comparing `qdx_py-0.9.2/Cargo.lock` & `qdx_py-0.9.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
  "tracing",
  "tracing-subscriber",
  "uuid",
 ]
 
 [[package]]
 name = "qdx-py"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "pyo3",
  "qdx-common",
  "serde",
  "serde_json",
 ]
```

### Comparing `qdx_py-0.9.2/PKG-INFO` & `qdx_py-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdx-py
-Version: 0.9.2
+Version: 0.9.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # QDX-py
```


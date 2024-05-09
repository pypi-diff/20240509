# Comparing `tmp/alphafold3-0.0.1.tar.gz` & `tmp/alphafold3-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphafold3-0.0.1.tar", max compression
+gzip compressed data, was "alphafold3-0.0.2.tar", max compression
```

## Comparing `alphafold3-0.0.1.tar` & `alphafold3-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-05-08 16:55:43.323225 alphafold3-0.0.1/LICENSE
--rw-r--r--   0        0        0      218 2024-05-08 16:57:40.637956 alphafold3-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-08 16:58:09.876923 alphafold3-0.0.1/alphafold3/__init__.py
--rw-r--r--   0        0        0     1349 2024-05-08 16:59:13.986504 alphafold3-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 alphafold3-0.0.1/setup.py
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 alphafold3-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-08 16:55:43.323225 alphafold3-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3885 2024-05-09 20:34:50.011249 alphafold3-0.0.2/README.md
+-rw-r--r--   0        0        0      169 2024-05-09 20:33:55.539381 alphafold3-0.0.2/alphafold3/__init__.py
+-rw-r--r--   0        0        0     4196 2024-05-08 17:23:47.690079 alphafold3-0.0.2/alphafold3/constants.py
+-rw-r--r--   0        0        0     5314 2024-05-09 19:20:59.867782 alphafold3-0.0.2/alphafold3/diffusion.py
+-rw-r--r--   0        0        0    17740 2024-05-09 20:33:09.520911 alphafold3-0.0.2/alphafold3/model.py
+-rw-r--r--   0        0        0     6604 2024-05-09 20:33:40.387129 alphafold3-0.0.2/alphafold3/pairformer.py
+-rw-r--r--   0        0        0     1364 2024-05-09 20:34:56.405112 alphafold3-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4674 1970-01-01 00:00:00.000000 alphafold3-0.0.2/setup.py
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 alphafold3-0.0.2/PKG-INFO
```

### Comparing `alphafold3-0.0.1/LICENSE` & `alphafold3-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alphafold3-0.0.1/pyproject.toml` & `alphafold3-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "alphafold3"
-version = "0.0.1"
+version = "0.0.2"
 description = "Paper - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/AlphaFold3"
 documentation = "https://github.com/kyegomez/AlphaFold3"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/AlphaFold3"
@@ -22,14 +22,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 zetascale = "*"
 torch = "*"
 einops = "*"
+openfold = "*"
 
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.6"
 types-toml = "^0.10.8.1"
 types-redis = "^4.3.21.6"
 types-pytz = "^2023.3.0.0"
```


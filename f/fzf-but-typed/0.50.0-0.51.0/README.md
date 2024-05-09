# Comparing `tmp/fzf_but_typed-0.50.0.tar.gz` & `tmp/fzf_but_typed-0.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fzf_but_typed-0.50.0.tar", max compression
+gzip compressed data, was "fzf_but_typed-0.51.0.tar", max compression
```

## Comparing `fzf_but_typed-0.50.0.tar` & `fzf_but_typed-0.51.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-11-13 22:24:10.574829 fzf_but_typed-0.50.0/LICENSE
--rw-r--r--   0        0        0     9088 2024-02-12 23:47:47.859282 fzf_but_typed-0.50.0/README.md
--rw-r--r--   0        0        0     1716 2024-05-09 18:10:42.005232 fzf_but_typed-0.50.0/pyproject.toml
--rw-r--r--   0        0        0     1199 2024-02-12 23:22:27.296580 fzf_but_typed-0.50.0/src/fzf_but_typed/__init__.py
--rw-r--r--   0        0        0     3744 2024-02-12 23:53:00.103088 fzf_but_typed-0.50.0/src/fzf_but_typed/__main__.py
--rw-r--r--   0        0        0    33816 2024-05-09 18:10:42.008565 fzf_but_typed-0.50.0/src/fzf_but_typed/lib.py
--rw-r--r--   0        0        0        0 2023-11-13 02:31:07.523497 fzf_but_typed-0.50.0/src/fzf_but_typed/py.typed
--rw-r--r--   0        0        0     9946 1970-01-01 00:00:00.000000 fzf_but_typed-0.50.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-11-13 22:24:10.574829 fzf_but_typed-0.51.0/LICENSE
+-rw-r--r--   0        0        0     9088 2024-02-12 23:47:47.859282 fzf_but_typed-0.51.0/README.md
+-rw-r--r--   0        0        0     1716 2024-05-09 18:10:49.155065 fzf_but_typed-0.51.0/pyproject.toml
+-rw-r--r--   0        0        0     1199 2024-02-12 23:22:27.296580 fzf_but_typed-0.51.0/src/fzf_but_typed/__init__.py
+-rw-r--r--   0        0        0     3744 2024-02-12 23:53:00.103088 fzf_but_typed-0.51.0/src/fzf_but_typed/__main__.py
+-rw-r--r--   0        0        0    34017 2024-05-09 18:10:49.158398 fzf_but_typed-0.51.0/src/fzf_but_typed/lib.py
+-rw-r--r--   0        0        0        0 2023-11-13 02:31:07.523497 fzf_but_typed-0.51.0/src/fzf_but_typed/py.typed
+-rw-r--r--   0        0        0     9946 1970-01-01 00:00:00.000000 fzf_but_typed-0.51.0/PKG-INFO
```

### Comparing `fzf_but_typed-0.50.0/LICENSE` & `fzf_but_typed-0.51.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fzf_but_typed-0.50.0/README.md` & `fzf_but_typed-0.51.0/README.md`

 * *Files identical despite different names*

### Comparing `fzf_but_typed-0.50.0/pyproject.toml` & `fzf_but_typed-0.51.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fzf_but_typed"
-version = "0.50.0"
+version = "0.51.0"
 description = "Statically typed API to fzf"
 authors = ["Bruno Fauth <149593@upf.br>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `fzf_but_typed-0.50.0/src/fzf_but_typed/__init__.py` & `fzf_but_typed-0.51.0/src/fzf_but_typed/__init__.py`

 * *Files identical despite different names*

### Comparing `fzf_but_typed-0.50.0/src/fzf_but_typed/__main__.py` & `fzf_but_typed-0.51.0/src/fzf_but_typed/__main__.py`

 * *Files identical despite different names*

### Comparing `fzf_but_typed-0.50.0/src/fzf_but_typed/lib.py` & `fzf_but_typed-0.51.0/src/fzf_but_typed/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,14 +302,15 @@
     BACKWARD_CHAR = "backward-char"
     BACKWARD_DELETE_CHAR = "backward-delete-char"
     BACKWARD_DELETE_CHAR_EOF = "backward-delete-char/eof"
     BACKWARD_KILL_WORD = "backward-kill-word"
     BACKWARD_WORD = "backward-word"
     BEGINNING_OF_LINE = "beginning-of-line"
     CANCEL = "cancel"
+    CHANGE_MULTI = "change-multi"
     CLEAR_QUERY = "clear-query"
     CLEAR_SCREEN = "clear-screen"
     CLEAR_SELECTION = "clear-selection"
     CLOSE = "close"
     DELETE_CHAR = "delete-char"
     DELETE_CHAR_EOF = "delete-char/eof"
     DESELECT = "deselect"
@@ -375,14 +376,15 @@
 
 
 @unique
 class ActionWithArgType(StrEnum):
     BECOME = "become"
     CHANGE_BORDER_LABEL = "change-border-label"
     CHANGE_HEADER = "change-header"
+    CHANGE_MULTI = "change-multi"
     CHANGE_PREVIEW = "change-preview"
     CHANGE_PREVIEW_LABEL = "change-preview-label"
     CHANGE_PREVIEW_WINDOW = "change-preview-window"
     CHANGE_PROMPT = "change-prompt"
     CHANGE_QUERY = "change-query"
     EXECUTE = "execute"
     EXECUTE_SILENT = "execute-silent"
@@ -912,14 +914,15 @@
     filter: str | None = None
     print_query: bool = False
     expect: list[Key] | None = None
     read0: bool = False
     print0: bool = False
     no_clear: bool = False
     sync: bool = False
+    with_shell: str | None = None
     listen: RemoteHost | None = None
     listen_unsafe: RemoteHost | None = None
 
     def as_args(self) -> list[str]:
         args = [
             '--select-1' if self.select_1 else '--no-select-1',
             '--exit-0' if self.exit_0 else '--no-exit-0',
@@ -935,14 +938,16 @@
             args.append(f'--filter={self.filter}')
         if self.listen is not None:
             args.append(f'--listen={self.listen}')
         if self.listen_unsafe is not None:
             args.append(f'--listen-unsafe={self.listen_unsafe}')
         if self.expect is not None:
             args.append(f'--expect={",".join(self.expect)}')
+        if self.with_shell is not None:
+            args.append(f'--with-shell={self.with_shell}')
         return args
 
 
 @unique
 class TraversalBehavior(StrEnum):
     FILE = "file"
     DIR = "dir"
```

### Comparing `fzf_but_typed-0.50.0/PKG-INFO` & `fzf_but_typed-0.51.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fzf_but_typed
-Version: 0.50.0
+Version: 0.51.0
 Summary: Statically typed API to fzf
 Home-page: https://github.com/brunofauth/fzf-but-typed
 License: MIT
 Keywords: cli,command-line,type,hint,fzf,fuzzy,finder
 Author: Bruno Fauth
 Author-email: 149593@upf.br
 Requires-Python: >=3.11,<4.0
```


# Comparing `tmp/golink-0.5.1.tar.gz` & `tmp/golink-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golink-0.5.1.tar", max compression
+gzip compressed data, was "golink-0.5.2.tar", max compression
```

## Comparing `golink-0.5.1.tar` & `golink-0.5.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-29 04:04:28.448306 golink-0.5.1/LICENSE
--rw-r--r--   0        0        0       22 2024-04-29 04:04:28.448306 golink-0.5.1/golink/__init__.py
--rw-r--r--   0        0        0     7890 2024-04-29 04:43:04.318263 golink-0.5.1/golink/cli.py
--rw-r--r--   0        0        0     1988 2024-04-29 04:04:28.448306 golink-0.5.1/golink/script.js
--rw-r--r--   0        0        0     3361 2024-04-29 04:04:28.448306 golink-0.5.1/golink/style.css
--rw-r--r--   0        0        0     7729 2024-04-29 04:04:28.448306 golink-0.5.1/golink/utils.py
--rw-r--r--   0        0        0      269 2024-05-03 17:34:36.550822 golink-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 golink-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-29 04:04:28.448306 golink-0.5.2/LICENSE
+-rw-r--r--   0        0        0     2858 2024-05-09 20:17:16.306197 golink-0.5.2/README.md
+-rw-r--r--   0        0        0      100 2024-05-09 20:26:37.020179 golink-0.5.2/golink/__init__.py
+-rw-r--r--   0        0        0     7928 2024-05-06 18:41:37.701305 golink-0.5.2/golink/cli.py
+-rw-r--r--   0        0        0     1988 2024-04-29 04:04:28.448306 golink-0.5.2/golink/script.js
+-rw-r--r--   0        0        0     3361 2024-04-29 04:04:28.448306 golink-0.5.2/golink/style.css
+-rw-r--r--   0        0        0     7729 2024-04-29 04:04:28.448306 golink-0.5.2/golink/utils.py
+-rw-r--r--   0        0        0      650 2024-05-09 20:26:12.929800 golink-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 golink-0.5.2/PKG-INFO
```

### Comparing `golink-0.5.1/LICENSE` & `golink-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `golink-0.5.1/golink/cli.py` & `golink-0.5.2/golink/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     if args["set"]:
         key = args["<key>"][0]
         assert key[-1] != "/", f'Key "{key}" should not end with a "/"!'
         url = args["<url>"]
         df = set_link(key, url, df)
         print_msg = f'Set key "{bolded(key)}" {bolded(ARROW)} "{bolded(url)}"'
         commit_msg = f'Set key "{key}" {ARROW} "{url}"'
-    elif args["rm"]:
+    elif args["rm"] or args["delete"]: # delete for legacy
         keys = args["<key>"]
         poss = set(df.key)
         deletable = [k for k in keys if k in poss]
         df = delete_links(deletable, df)
 
         not_deletable = set(keys) - set(deletable)
         if not_deletable:
```

### Comparing `golink-0.5.1/golink/script.js` & `golink-0.5.2/golink/script.js`

 * *Files identical despite different names*

### Comparing `golink-0.5.1/golink/style.css` & `golink-0.5.2/golink/style.css`

 * *Files identical despite different names*

### Comparing `golink-0.5.1/golink/utils.py` & `golink-0.5.2/golink/utils.py`

 * *Files identical despite different names*


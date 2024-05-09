# Comparing `tmp/hfive-0.1.1.tar.gz` & `tmp/hfive-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfive-0.1.1.tar", last modified: Tue May  7 22:58:42 2024, max compression
+gzip compressed data, was "hfive-0.1.2.tar", last modified: Thu May  9 13:18:41 2024, max compression
```

## Comparing `hfive-0.1.1.tar` & `hfive-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 22:58:42.776718 hfive-0.1.1/
--rw-r--r--   0 florez    (1000) florez    (1000)     1056 2024-04-26 13:36:33.000000 hfive-0.1.1/LICENSE
--rw-r--r--   0 florez    (1000) florez    (1000)     1985 2024-05-07 22:58:42.773385 hfive-0.1.1/PKG-INFO
--rw-r--r--   0 florez    (1000) florez    (1000)      156 2024-04-26 14:47:26.000000 hfive-0.1.1/README.md
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 22:58:42.773385 hfive-0.1.1/hfive/
--rw-r--r--   0 florez    (1000) florez    (1000)      119 2024-05-07 22:57:19.000000 hfive-0.1.1/hfive/__init__.py
--rw-r--r--   0 florez    (1000) florez    (1000)     3656 2024-05-07 22:56:41.000000 hfive-0.1.1/hfive/common.py
--rw-r--r--   0 florez    (1000) florez    (1000)    18315 2024-04-26 16:16:03.000000 hfive-0.1.1/hfive/main.py
--rw-r--r--   0 florez    (1000) florez    (1000)    14665 2024-04-26 14:48:06.000000 hfive-0.1.1/hfive/widgets.py
-drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-07 22:58:42.773385 hfive-0.1.1/hfive.egg-info/
--rw-r--r--   0 florez    (1000) florez    (1000)     1985 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/PKG-INFO
--rw-r--r--   0 florez    (1000) florez    (1000)      282 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/SOURCES.txt
--rw-r--r--   0 florez    (1000) florez    (1000)        1 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/dependency_links.txt
--rw-r--r--   0 florez    (1000) florez    (1000)       42 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/entry_points.txt
--rw-r--r--   0 florez    (1000) florez    (1000)       17 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/requires.txt
--rw-r--r--   0 florez    (1000) florez    (1000)        6 2024-05-07 22:58:42.000000 hfive-0.1.1/hfive.egg-info/top_level.txt
--rw-r--r--   0 florez    (1000) florez    (1000)      919 2024-05-07 22:57:09.000000 hfive-0.1.1/pyproject.toml
--rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-05-07 22:58:42.776718 hfive-0.1.1/setup.cfg
--rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-04-26 14:08:50.000000 hfive-0.1.1/setup.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-09 13:18:41.106258 hfive-0.1.2/
+-rw-r--r--   0 florez    (1000) florez    (1000)     1056 2024-04-26 13:36:33.000000 hfive-0.1.2/LICENSE
+-rw-r--r--   0 florez    (1000) florez    (1000)     1985 2024-05-09 13:18:41.102924 hfive-0.1.2/PKG-INFO
+-rw-r--r--   0 florez    (1000) florez    (1000)      156 2024-04-26 14:47:26.000000 hfive-0.1.2/README.md
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-09 13:18:41.102924 hfive-0.1.2/hfive/
+-rw-r--r--   0 florez    (1000) florez    (1000)      119 2024-05-09 13:17:53.000000 hfive-0.1.2/hfive/__init__.py
+-rw-r--r--   0 florez    (1000) florez    (1000)     3656 2024-05-07 22:56:41.000000 hfive-0.1.2/hfive/common.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    18315 2024-04-26 16:16:03.000000 hfive-0.1.2/hfive/main.py
+-rw-r--r--   0 florez    (1000) florez    (1000)    14517 2024-05-09 13:15:34.000000 hfive-0.1.2/hfive/widgets.py
+drwxr-xr-x   0 florez    (1000) florez    (1000)        0 2024-05-09 13:18:41.102924 hfive-0.1.2/hfive.egg-info/
+-rw-r--r--   0 florez    (1000) florez    (1000)     1985 2024-05-09 13:18:41.000000 hfive-0.1.2/hfive.egg-info/PKG-INFO
+-rw-r--r--   0 florez    (1000) florez    (1000)      282 2024-05-09 13:18:41.000000 hfive-0.1.2/hfive.egg-info/SOURCES.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)        1 2024-05-09 13:18:41.000000 hfive-0.1.2/hfive.egg-info/dependency_links.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)       42 2024-05-09 13:18:41.000000 hfive-0.1.2/hfive.egg-info/entry_points.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)       17 2024-05-09 13:18:41.000000 hfive-0.1.2/hfive.egg-info/requires.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)        6 2024-05-09 13:18:41.000000 hfive-0.1.2/hfive.egg-info/top_level.txt
+-rw-r--r--   0 florez    (1000) florez    (1000)      919 2024-05-09 13:17:53.000000 hfive-0.1.2/pyproject.toml
+-rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-05-09 13:18:41.106258 hfive-0.1.2/setup.cfg
+-rw-r--r--   0 florez    (1000) florez    (1000)       38 2024-04-26 14:08:50.000000 hfive-0.1.2/setup.py
```

### Comparing `hfive-0.1.1/LICENSE` & `hfive-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hfive-0.1.1/PKG-INFO` & `hfive-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfive
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple TUI for viewing HDF5 files.
 Author-email: Flavio Lorez <florez@ethz.ch>
 License: Copyright (c) 2024 Flavio Lorez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `hfive-0.1.1/hfive/common.py` & `hfive-0.1.2/hfive/common.py`

 * *Files identical despite different names*

### Comparing `hfive-0.1.1/hfive/main.py` & `hfive-0.1.2/hfive/main.py`

 * *Files identical despite different names*

### Comparing `hfive-0.1.1/hfive/widgets.py` & `hfive-0.1.2/hfive/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         if focus_map is None:
             focus_map = "green_box"
         super().__init__(self.widget, attr_map, focus_map)
 
     def __getattr__(self, name: str):
         return self.widget.base_widget.__getattribute__(name)
 
-    def keypress(self, size: tuple[()] | tuple[int] | tuple[int, int], key: str) -> str | None:
+    def keypress(self, size: tuple, key: str) -> str:
         return super().keypress(size, key)
 
 
 class cEdit(urwid.Edit):
     def __init__(self, *args, callback: callable = None, **kwargs):
         self.callback = callback
         super().__init__(*args, **kwargs)
@@ -177,15 +177,15 @@
         if self.is_visible:
             self.main_loop.widget = self.bottom_w
             self.is_visible = False
         else:
             self.main_loop.widget = self
             self.is_visible = True
 
-    def keypress(self, size: tuple[()] | tuple[int] | tuple[int, int], key: str) -> str | None:
+    def keypress(self, size: tuple, key: str) -> str:
         if key in ("esc", "q"):
             # Set the widget of loop back to the original widget
             return self.toggle()
 
         return self.bottom_w.keypress(size, key)
 
 
@@ -227,15 +227,15 @@
         self.callback()
         return
 
     def no(self, button: urwid.Button) -> None:
         Caller.exit_widget()
         return
 
-    def keypress(self, size: tuple[()] | tuple[int] | tuple[int, int], key: str) -> str | None:
+    def keypress(self, size: tuple, key: str) -> str:
         if key in ("esc", "q"):
             # Set the widget of loop back to the original widget
             Caller.exit_widget()
             return
         if key == "l":
             return super().keypress(size, "right")
         if key == "h":
@@ -355,15 +355,15 @@
                 item.column_focus_map = focus_map
             item._invalidate()
 
         self.items = items
         self._listwalker = urwid.SimpleFocusListWalker(self.items)
         super().__init__(self._listwalker, *args, **kwargs, keymap_jk=True)
 
-    def keypress(self, size: tuple[int], key: str) -> Union[str, None]:
+    def keypress(self, size: tuple, key: str) -> Union[str, None]:
         return super().keypress(size, key)
 
 
 class cPopup(urwid.Overlay):
 
     def __init__(self, widget: urwid.Widget, *args, **kwargs):
         """A custom Popup widget with a title, frame and footer.
@@ -417,15 +417,15 @@
             focus_map=kwargs.pop("focus_map"),
         )
 
         base_widget = Caller.main_loop.widget if Caller.main_loop else urwid.SolidFill(" ")
 
         super().__init__(box, base_widget, *args, **kwargs)
 
-    def keypress(self, size: tuple[int, int], key: str) -> str | None:
+    def keypress(self, size: tuple, key: str) -> str:
         return super().keypress((1,), key)
 
 
 class FocusedList(urwid.ListBox):
     """List box with a focused item even if the list is not in focus."""
 
     def render(self, size, focus=False):
```

### Comparing `hfive-0.1.1/hfive.egg-info/PKG-INFO` & `hfive-0.1.2/hfive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfive
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple TUI for viewing HDF5 files.
 Author-email: Flavio Lorez <florez@ethz.ch>
 License: Copyright (c) 2024 Flavio Lorez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `hfive-0.1.1/pyproject.toml` & `hfive-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hfive"
-version = "0.1.1"
+version = "0.1.2"
 description = "A simple TUI for viewing HDF5 files."
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [{ name = "Flavio Lorez", email = "florez@ethz.ch" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```


# Comparing `tmp/roff-0.4.3.tar.gz` & `tmp/roff-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roff-0.4.3.tar", last modified: Wed May  8 08:54:23 2024, max compression
+gzip compressed data, was "roff-0.5.0.tar", last modified: Thu May  9 13:23:44 2024, max compression
```

## Comparing `roff-0.4.3.tar` & `roff-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-21 09:37:21.000000 roff-0.4.3/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-05-08 08:54:23.162333 roff-0.4.3/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1673 2024-04-28 12:23:56.000000 roff-0.4.3/README.md
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/docs/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1645 2024-04-29 10:43:42.000000 roff-0.4.3/docs/roff.1
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2872 2024-04-30 19:29:45.000000 roff-0.4.3/docs/roff.5
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-21 09:38:29.000000 roff-0.4.3/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-05-08 08:54:23.162333 roff-0.4.3/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2155 2024-04-25 15:15:31.000000 roff-0.4.3/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.158332 roff-0.4.3/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/src/roff/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/src/roff/__cli__/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      114 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/__cli__/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      446 2024-04-25 15:15:31.000000 roff-0.4.3/src/roff/__cli__/convert.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1036 2024-04-27 11:45:13.000000 roff-0.4.3/src/roff/__cli__/template.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      403 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/__cli__/tree.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      747 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/__cli__/util.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1508 2024-05-08 08:54:12.000000 roff-0.4.3/src/roff/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2112 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/__main__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2645 2024-04-30 19:28:52.000000 roff-0.4.3/src/roff/_images.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2303 2024-04-27 11:04:01.000000 roff-0.4.3/src/roff/_markdown.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      909 2024-05-08 08:47:35.000000 roff-0.4.3/src/roff/_util.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)    11980 2024-05-08 08:51:57.000000 roff-0.4.3/src/roff/convert.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-08 08:54:23.162333 roff-0.4.3/src/roff.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      517 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/entry_points.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       94 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/requires.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-05-08 08:54:23.000000 roff-0.4.3/src/roff.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-09 13:23:44.730170 roff-0.5.0/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1072 2024-04-21 09:37:21.000000 roff-0.5.0/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-05-09 13:23:44.730170 roff-0.5.0/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1673 2024-04-28 12:23:56.000000 roff-0.5.0/README.md
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-09 13:23:44.726170 roff-0.5.0/docs/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1715 2024-05-09 13:23:37.000000 roff-0.5.0/docs/roff.1
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2934 2024-05-09 13:23:38.000000 roff-0.5.0/docs/roff.5
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-21 09:38:29.000000 roff-0.5.0/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-05-09 13:23:44.730170 roff-0.5.0/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2155 2024-04-25 15:15:31.000000 roff-0.5.0/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-09 13:23:44.726170 roff-0.5.0/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-09 13:23:44.726170 roff-0.5.0/src/roff/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-09 13:23:44.730170 roff-0.5.0/src/roff/__cli__/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      125 2024-05-09 10:00:12.000000 roff-0.5.0/src/roff/__cli__/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      548 2024-05-09 09:55:56.000000 roff-0.5.0/src/roff/__cli__/convert.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1036 2024-04-27 11:45:13.000000 roff-0.5.0/src/roff/__cli__/template.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      403 2024-04-30 19:28:52.000000 roff-0.5.0/src/roff/__cli__/tree.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      747 2024-04-30 19:28:52.000000 roff-0.5.0/src/roff/__cli__/util.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1325 2024-05-09 13:11:03.000000 roff-0.5.0/src/roff/__cli__/watch.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1510 2024-05-09 13:12:37.000000 roff-0.5.0/src/roff/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2434 2024-05-09 10:30:05.000000 roff-0.5.0/src/roff/__main__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2645 2024-04-30 19:28:52.000000 roff-0.5.0/src/roff/_images.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2303 2024-04-27 11:04:01.000000 roff-0.5.0/src/roff/_markdown.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      909 2024-05-08 08:47:35.000000 roff-0.5.0/src/roff/_util.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)    11971 2024-05-09 13:18:10.000000 roff-0.5.0/src/roff/convert.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-05-09 13:23:44.730170 roff-0.5.0/src/roff.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3370 2024-05-09 13:23:44.000000 roff-0.5.0/src/roff.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      543 2024-05-09 13:23:44.000000 roff-0.5.0/src/roff.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-05-09 13:23:44.000000 roff-0.5.0/src/roff.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       44 2024-05-09 13:23:44.000000 roff-0.5.0/src/roff.egg-info/entry_points.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       94 2024-05-09 13:23:44.000000 roff-0.5.0/src/roff.egg-info/requires.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        5 2024-05-09 13:23:44.000000 roff-0.5.0/src/roff.egg-info/top_level.txt
```

### Comparing `roff-0.4.3/LICENSE` & `roff-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roff-0.4.3/PKG-INFO` & `roff-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roff
-Version: 0.4.3
+Version: 0.5.0
 Summary: python-based cli to convert markdown to the roff (man-pages) format
 Home-page: https://github.com/utility-toolbox/roff
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-toolbox
 Project-URL: Homepage, https://github.com/utility-toolbox/roff/
 Project-URL: Bug Tracker, https://github.com/utility-toolbox/roff/issues
```

### Comparing `roff-0.4.3/README.md` & `roff-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `roff-0.4.3/docs/roff.1` & `roff-0.5.0/docs/roff.1`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,46 @@
-.\" generated with roff/v0.3.1
-.\" https://pypi.org/project/roff/0.3.1
+.\" generated with roff/v0.5.0
+.\" https://pypi.org/project/roff/0.5.0
 .\" https://github.com/utility-toolbox/roff/
 .\"
-.TH "ROFF" "1" "29 April 2024" "github.com/utility-toolbox/roff"
+.TH "ROFF" "1" "09 May 2024" "github.com/utility-toolbox/roff"
 .SH "NAME"
-\fBroff\fP • python-based cli to convert markdown to the roff (man-pages) format
+\fBroff\fP • python\[em]based cli to convert markdown to the roff (man\[em]pages) format
 .SH "SYNOPSIS"
 .sp
-• \fBroff\fP [\fB-h\fP] [\fB-v\fP] {\fIconvert\fP,\fItemplate\fP} ...
+• \fBroff\fP [\fB\-h\fP] [\fB\-v\fP] {\fIconvert\fP,\fItemplate\fP} ...
 .br
-• \fBroff\fP \fIconvert\fP [\fB-h\fP] \fIsource\fP [\fIdest\fP]
+• \fBroff\fP \fIconvert\fP [\fB\-h\fP] \fIsource\fP [\fIdest\fP]
 .br
-• \fBroff\fP \fItemplate\fP [\fB-h\fP] \fIdest\fP
+• \fBroff\fP \fItemplate\fP [\fB\-h\fP] \fIdest\fP
 .br
 .sp
 .SH "DESCRIPTION"
-python-based cli to convert markdown to the roff (man-pages) format\.
+.P
+python\[em]based cli to convert markdown to the roff (man\[em]pages) format.
 .sp
 .RS 2
 see roff(5) for more information about the file specification
 .RE
 .sp
+.P
 Support for all* Markdown features:
 .sp
 .RS 2
-*h1 is reserved for the head\.
+*h1 is reserved for the head.
 .RE
 .sp
 .sp
-• heading (h2-h6)
+• heading (h2\[em]h6)
 .br
 • Ordered Lists
 .br
 • Unordered Lists
 .br
-• Code-Blocks
+• Code\[em]Blocks
 .br
 • Inline
 .br
 .RS 2
 .br
 • Code
 .br
@@ -46,50 +48,58 @@
 .br
 • Emphasis
 .br
 • Links
 .br
 .br
 .RE
-• Images (rendered as braille-art)
+• Images (rendered as braille\[em]art)
 .br
-• Horizontal-Rule
+• Horizontal\[em]Rule
 .br
 .sp
 .SH "OPTIONS"
 .SS "\fBroff\fP \fIconvert\fP"
 .sp
 .RS 2
 Converts markdown files to roff files
 .RE
 .sp
 .sp
 \fIsource\fP:
 .sp
+.P
 Markdown file that should be parsed
 .sp
 \fI[dest]\fP:
 .sp
+.P
 Manpage file
 .SS "\fBroff\fP \fItemplate\fP"
 .sp
 .RS 2
 Generates a Markdown file that you can fill
 .RE
 .sp
 .sp
 \fI-y\fP, \fI--yes\fP:
 .sp
+.P
 Overwrite file if it exists
 .sp
 \fIdest\fP:
 .sp
+.P
 Target file that should be generated
 .SH "BUGS"
-https://github\.com/utility-toolbox/roff/issues
+.P
+https://github.com/utility\[em]toolbox/roff/issues
 .SH "AUTHOR"
-https://github\.com/PlayerG9
+.P
+https://github.com/PlayerG9
 .SH "SEE ALSO"
 .SS "Organisation:"
-https://github\.com/utility-toolbox
+.P
+https://github.com/utility\[em]toolbox
 .SS "Repository:"
-https://github\.com/utility-toolbox/roff
+.P
+https://github.com/utility\[em]toolbox/roff
```

### Comparing `roff-0.4.3/setup.py` & `roff-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.3/src/roff/__cli__/template.py` & `roff-0.5.0/src/roff/__cli__/template.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.3/src/roff/__cli__/util.py` & `roff-0.5.0/src/roff/__cli__/util.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.3/src/roff/__init__.py` & `roff-0.5.0/src/roff/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 
 __author__ = "PlayerG9"
 __copyright__ = "Copyright 2024, utility-toolbox"
 __credits__ = ["PlayerG9"]
 __license__ = "MIT"
 __maintainer__ = "PlayerG9"
 __email__ = None
-__status__ = "Prototype"  # Prototype, Development, Production
+__status__ = "Development"  # Prototype, Development, Production
 __description__ = "python-based cli to convert markdown to the roff (man-pages) format"
-__version_info__ = (0, 4, 3)
+__version_info__ = (0, 5, 0)
 __version__ = '.'.join(str(_) for _ in __version_info__)
```

### Comparing `roff-0.4.3/src/roff/__main__.py` & `roff-0.5.0/src/roff/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,21 @@
 tree_parser.set_defaults(__cmd__=__cli__.tree.__cmd__)
 tree_parser.add_argument('--show-text', action=ap.BooleanOptionalAction,
                          help="Show text in the tree")
 tree_parser.add_argument('source',
                          help="Markdown file that should be parsed")
 
 
+watch_parser = subparsers.add_parser('watch',
+                                     help="Start the manpage while automatically updating it. (experimental)")
+watch_parser.set_defaults(__cmd__=__cli__.watch.__cmd__)
+watch_parser.add_argument('source',
+                          help="Markdown file that should be parsed")
+
+
 def main():
     args = vars(parser.parse_args())
     cmd = args.pop('__cmd__')
     cmd(**args)
 
 
 if __name__ == '__main__':
```

### Comparing `roff-0.4.3/src/roff/_images.py` & `roff-0.5.0/src/roff/_images.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.3/src/roff/_markdown.py` & `roff-0.5.0/src/roff/_markdown.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.3/src/roff/_util.py` & `roff-0.5.0/src/roff/_util.py`

 * *Files identical despite different names*

### Comparing `roff-0.4.3/src/roff/convert.py` & `roff-0.5.0/src/roff/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     def _parse_children(self, children: t.List[markdown_it.tree.SyntaxTreeNode]) -> None:
         for child in children:
             self._parse_node(node=child)
 
     def _parse_node(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         if not self._had_head and node.tag != 'h1':
-            raise SyntaxError("First element in the document should be the header")
+            raise SyntaxError(f"First element in the document should be the header. (got {node.type})")
         parser = getattr(self, f"_parse_{node.tag}", None)
         if parser is None:
             warnings.warn(f"Unsupported node tag '{node.tag}' of type '{node.type}'", RuntimeWarning)
             return
         parser(node)
 
     def _render_inline(self, node: markdown_it.tree.SyntaxTreeNode) -> str:
@@ -184,16 +184,16 @@
     # maybe not the best solution
     _parse_h5 = _parse_h4
     _parse_h6 = _parse_h4
 
     def _parse_p(self, node: markdown_it.tree.SyntaxTreeNode) -> None:
         content = self._render_inline(node=node.children[0])
         content = re.sub(r'\n{2,}', '\n.sp\n', content)
-        # if node.level > 0:  # destroys the structure
-        #     self._stream.write('.P\n')
+        if node.level == 0:
+            self._stream.write('.P\n')
         self._stream.write(f'{content}\n')
 
     @staticmethod
     def _check_newline(text: str) -> bool:
         r""" checks the output of _render_inline if it won't fit into one line """
         return (
             # len(text) >= self.width  # won't fit in one line (good in theory. bad in praxis)
```

### Comparing `roff-0.4.3/src/roff.egg-info/PKG-INFO` & `roff-0.5.0/src/roff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roff
-Version: 0.4.3
+Version: 0.5.0
 Summary: python-based cli to convert markdown to the roff (man-pages) format
 Home-page: https://github.com/utility-toolbox/roff
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-toolbox
 Project-URL: Homepage, https://github.com/utility-toolbox/roff/
 Project-URL: Bug Tracker, https://github.com/utility-toolbox/roff/issues
```

### Comparing `roff-0.4.3/src/roff.egg-info/SOURCES.txt` & `roff-0.5.0/src/roff.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 src/roff.egg-info/entry_points.txt
 src/roff.egg-info/requires.txt
 src/roff.egg-info/top_level.txt
 src/roff/__cli__/__init__.py
 src/roff/__cli__/convert.py
 src/roff/__cli__/template.py
 src/roff/__cli__/tree.py
-src/roff/__cli__/util.py
+src/roff/__cli__/util.py
+src/roff/__cli__/watch.py
```


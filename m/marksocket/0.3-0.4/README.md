# Comparing `tmp/marksocket-0.3.tar.gz` & `tmp/marksocket-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marksocket-0.3.tar", last modified: Wed May  8 14:12:58 2024, max compression
+gzip compressed data, was "marksocket-0.4.tar", last modified: Thu May  9 17:09:11 2024, max compression
```

## Comparing `marksocket-0.3.tar` & `marksocket-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aapo      (1001) aapo      (1001)        0 2024-05-08 14:12:58.779684 marksocket-0.3/
--rw-r--r--   0 aapo      (1001) aapo      (1001)     7652 2024-05-08 11:42:29.000000 marksocket-0.3/LICENSE
--rw-r--r--   0 aapo      (1001) aapo      (1001)      452 2024-05-08 14:12:58.779684 marksocket-0.3/PKG-INFO
-drwxr-xr-x   0 aapo      (1001) aapo      (1001)        0 2024-05-08 14:12:58.775684 marksocket-0.3/marksocket.egg-info/
--rw-r--r--   0 aapo      (1001) aapo      (1001)      452 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/PKG-INFO
--rw-r--r--   0 aapo      (1001) aapo      (1001)      252 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/SOURCES.txt
--rw-r--r--   0 aapo      (1001) aapo      (1001)        1 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/dependency_links.txt
--rw-r--r--   0 aapo      (1001) aapo      (1001)       47 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/entry_points.txt
--rw-r--r--   0 aapo      (1001) aapo      (1001)       80 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/requires.txt
--rw-r--r--   0 aapo      (1001) aapo      (1001)       11 2024-05-08 14:12:58.000000 marksocket-0.3/marksocket.egg-info/top_level.txt
--rw-r-xr-x   0 aapo      (1001) aapo      (1001)     5957 2024-05-08 10:40:00.000000 marksocket-0.3/marksocket.py
--rw-r--r--   0 aapo      (1001) aapo      (1001)      566 2024-05-08 13:41:52.000000 marksocket-0.3/pyproject.toml
--rw-r--r--   0 aapo      (1001) aapo      (1001)     6838 2024-05-08 14:04:04.000000 marksocket-0.3/readme.md
--rw-r--r--   0 aapo      (1001) aapo      (1001)       38 2024-05-08 14:12:58.779684 marksocket-0.3/setup.cfg
+drwxr-xr-x   0 aapo      (1001) aapo      (1001)        0 2024-05-09 17:09:11.707873 marksocket-0.4/
+-rw-r--r--   0 aapo      (1001) aapo      (1001)     7652 2024-05-08 11:42:29.000000 marksocket-0.4/LICENSE
+-rw-r--r--   0 aapo      (1001) aapo      (1001)      537 2024-05-09 17:09:11.707873 marksocket-0.4/PKG-INFO
+drwxr-xr-x   0 aapo      (1001) aapo      (1001)        0 2024-05-09 17:09:11.703873 marksocket-0.4/marksocket.egg-info/
+-rw-r--r--   0 aapo      (1001) aapo      (1001)      537 2024-05-09 17:09:11.000000 marksocket-0.4/marksocket.egg-info/PKG-INFO
+-rw-r--r--   0 aapo      (1001) aapo      (1001)      252 2024-05-09 17:09:11.000000 marksocket-0.4/marksocket.egg-info/SOURCES.txt
+-rw-r--r--   0 aapo      (1001) aapo      (1001)        1 2024-05-09 17:09:11.000000 marksocket-0.4/marksocket.egg-info/dependency_links.txt
+-rw-r--r--   0 aapo      (1001) aapo      (1001)       47 2024-05-09 17:09:11.000000 marksocket-0.4/marksocket.egg-info/entry_points.txt
+-rw-r--r--   0 aapo      (1001) aapo      (1001)      118 2024-05-09 17:09:11.000000 marksocket-0.4/marksocket.egg-info/requires.txt
+-rw-r--r--   0 aapo      (1001) aapo      (1001)       11 2024-05-09 17:09:11.000000 marksocket-0.4/marksocket.egg-info/top_level.txt
+-rw-r-xr-x   0 aapo      (1001) aapo      (1001)     5957 2024-05-08 10:40:00.000000 marksocket-0.4/marksocket.py
+-rw-r--r--   0 aapo      (1001) aapo      (1001)      610 2024-05-09 17:08:11.000000 marksocket-0.4/pyproject.toml
+-rw-r--r--   0 aapo      (1001) aapo      (1001)     7156 2024-05-09 16:51:51.000000 marksocket-0.4/readme.md
+-rw-r--r--   0 aapo      (1001) aapo      (1001)       38 2024-05-09 17:09:11.707873 marksocket-0.4/setup.cfg
```

### Comparing `marksocket-0.3/LICENSE` & `marksocket-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `marksocket-0.3/marksocket.py` & `marksocket-0.4/marksocket.py`

 * *Files identical despite different names*

### Comparing `marksocket-0.3/readme.md` & `marksocket-0.4/readme.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Marksocket
 
-![](logo.svg)
+![](logo-light.svg#gh-light-mode-only)![](logo-dark.svg#gh-dark-mode-only)
 
 ## What
 
 A python script to parse and serve markdown documents to a browser with live reload.
 
 - Only one required external Python dependency: The markdown parser. The rest are optional Python-Markdown extensions.<br>
 - Only ~200 lines of python powered by the standard library.
@@ -23,29 +23,29 @@
 ```bash
 pip install marksocket
 ```
 
 With Markdown-Extensions:
 
 ```bash
-pip install marksocket[mermaid, highlights]
+pip install marksocket[mermaid,highlights]
 ```
 
 You can choose any or none of the extensions, mix them as you wish.
 
 ## Usage
 
 ```
-marksocket [-h] [-c CONFIG_FILE] [-p PORT] -x [EXTENSION]... [-s STYLESHEET]... [-j JAVASCRIPT]... markdown_file`
+marksocket [-h] [-c CONFIG_FILE] [-p PORT] -x [EXTENSION]... [-s STYLESHEET]... [-j JAVASCRIPT]... markdown_file
 ```
 
 ### Example
 
 ```bash
-marksocket -p 8001 -s style.css readme.md`
+marksocket -p 8001 -s style.css readme.md
 ```
 
 ### Options
 
 - -h: Help.
 - -c: Configuration file.
 - -p: The port to serve at. Command line argument takes precedence over the port specified in the configuration file. Defaults to 44444 if not specified on the command line or in the configuration file.
@@ -65,15 +65,15 @@
 
 ```
 marksocket -j script1.js -j script2.js readme.md
 ```
 
 ## Configuration file
 
-Allows specifying the port, stylesheet and javascript options. If the path to a configuration file is not given as a command line argument with the `-c` option, `~/.config/marksocket/config.toml` is looked for one. However both are optional and no configuration file is required to use the program. The command line option takes precedence over the default location, so the default configuration file in `~/.config/marksocket/config.toml` will not be loaded if the configuration file option `-c` is specified.
+Allows specifying the port, extension, stylesheet and javascript options. If the path to a configuration file is not given as a command line argument with the `-c` option, `~/.config/marksocket/config.toml` is looked for one. However both are optional and no configuration file is required to use the program. The command line option takes precedence over the default location, so the default configuration file in `~/.config/marksocket/config.toml` will not be loaded if the configuration file option `-c` is specified.
 
 The configuration file is written in TOML. All values in it are optional. You can specify any or none of them. It has the following schema:
 
 ```
 port = int
 extension = [ str ]
 javascript = [ str ]
@@ -85,42 +85,37 @@
 ```toml
 port = 8000
 extension = [ 'markdown_mermaid', 'fenced_code' ]
 javascript = [ 'mermaid.min.js', 'reload-mermaid.js' ]
 stylesheet = [ 'style.css' ]
 ```
 
-### Order of the javascript and stylesheet files
+### Mixing configuration file and command line options
 
-Command line options for loading javascript files (`-j`) and stylesheet files (`-s`) can both be used simultaneously with `javascript` and `stylesheet` options in the configuration file. The order the files are loaded in is as follows:
+Command line options for loading extensions (`-x`), javascript files (`-j`) and stylesheet files (`-s`) can all be used simultaneously with the `extension`, `javascript` and `stylesheet` options in the configuration file. The order the files are loaded in is as follows:
 
 1. JavaScript files specified in the configuration file, in the order they are specified.
 2. JavaScript files specified on the command line, in the order they are specified.
 3. Stylesheet files specified in the configuration file, in the order they are specified.
 4. Stylesheet files specified on the command line, in the order they are specified.
 
 ## Extensions
 
 ### Mermaid
 
 ```mermaid
-graph TB
+graph LR
     a(A)
     x{X}
     b(B)
     c(C)
 
     a --> x
     x -->|True| b
     x -->|False| c
-
-    style x fill:#fcf;
-    style a fill:#ccf;
-    style b fill:#cfc;
-    style c fill:#fcc;
 ```
 *Example of a Mermaid graph*
 
 If the optional dependency `mermaid` is specified during installation:
 
 ```bash
 pip install marksocket[mermaid]
@@ -143,23 +138,25 @@
     if (!e.isTrusted) {
         return;
     }
 
     scrollPos = window.scrollY;
 });
 
-window.addEventListener('load', () => {
+mermaid.initialize({theme: 'dark', startOnLoad: true});
+window.addEventListener('load', async () => {
     const observer = new MutationObserver(async () => {
         await mermaid.run();
         window.scrollTo(0, scrollPos);
     });
 
     observer.observe(document.body, {childList: true});
 });
 ```
+> *A list of available Mermaid themes can be found [here](https://mermaid.js.org/config/theming.html#available-themes).*
 
 Now marksocket could be called with said files to enable Mermaid graph rendering:
 
 ```bash
 marksocket -x markdown_mermaid -j mermaid.min.js -j reload-mermaid.js readme.md`
 ```
 
@@ -181,27 +178,27 @@
 An additional dependency [Pygments](https://pygments.org/) is installed. The Markdown-Python extension `codehilite` uses it for code highlighting (this extensions is included with Python-Markdown).
 
 #### Configuration
 
 Use Pygments to generate a stylesheet:
 
 ```bash
-pygmentize -S default -f html -a .codehilite > highlights.css
+pygmentize -S github-dark -f html -a .codehilite > highlights.css
 ```
 
-> *More options can be found in the [Pygments documentation](https://pygments.org/docs/)*
+> *More options can be found in the [Pygments documentation](https://pygments.org/docs/) and instructions on how to get a list of available styles can be found [here](https://pygments.org/docs/styles/).*
 
 And then include the codehilite extension with the `-x` flag and the stylesheet that was generated with the `-s` flag:
 
 ```bash
 marksocket -x codehilite -x fenced_code -s highlights.css readme.md
 ```
 
 Or include them in your configuration:
 
 ```TOML
 extension = [ 'codehilite', 'fenced_code' ]
 stylesheet = [ 'highlights.css' ]
 ```
 
-> ![NOTE]
+> [!NOTE]
 > You most likely want the [Fenced Code Blocks extension](https://python-markdown.github.io/extensions/fenced_code_blocks/) too when including code in your documents, which is why it was included in the examples. This extension ships with Python-Markdown so no additional configuration or installations are required.
```


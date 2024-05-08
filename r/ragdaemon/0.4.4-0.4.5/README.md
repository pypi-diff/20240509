# Comparing `tmp/ragdaemon-0.4.4.tar.gz` & `tmp/ragdaemon-0.4.5.tar.gz`

## Comparing `ragdaemon-0.4.4.tar` & `ragdaemon-0.4.5.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/app.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/context.py
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/graph.py
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/conftest.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0   669446 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/app.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/context.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/graph.py
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/utils.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/clusterer_binary.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/conftest.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/PKG-INFO
```

### Comparing `ragdaemon-0.4.4/tutorial.ipynb` & `ragdaemon-0.4.5/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/.github/workflows/run-tests.yml` & `ragdaemon-0.4.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/app.py` & `ragdaemon-0.4.5/ragdaemon/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,17 @@
 refresh = args.refresh
 verbose = True  # Always verbose in server mode
 code_extensions = None if args.code_extensions is None else set(args.code_extensions)
 diff = args.diff
 annotators = {
     "hierarchy": {},
     "chunker_llm": {"chunk_extensions": code_extensions},
-    "call_graph": {"call_extensions": code_extensions},
+    # "summarizer": {},
+    # "clusterer_binary": {},
+    # "call_graph": {"call_extensions": code_extensions},
     "diff": {"diff": diff},
     "layout_hierarchy": {},
 }
 daemon = Daemon(Path.cwd(), annotators=annotators, verbose=verbose)
 
 
 # Start/run daemon in the background
```

### Comparing `ragdaemon-0.4.4/ragdaemon/context.py` & `ragdaemon-0.4.5/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/daemon.py` & `ragdaemon-0.4.5/ragdaemon/daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import json
 import time
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Iterable, Optional
 
 from networkx.readwrite import json_graph
 from spice import Spice
 from spice.spice import Model
 
 from ragdaemon.annotators import Annotator, annotators_map
 from ragdaemon.context import ContextBuilder
@@ -65,35 +65,24 @@
         # Initialize an empty graph
         self.graph = KnowledgeGraph()
         self.graph.graph["cwd"] = self.cwd.as_posix()
         if self.verbose:
             print("Initialized empty graph.")
 
         annotators = annotators if annotators is not None else default_annotators()
-
-        # TODO: Maybe this should be a base annotator method? validate against all
-        if "call_graph" in annotators:
-            try:
-                chunker_type = next(a for a in annotators if "chunker" in a)
-                chunker_cls = annotators_map[chunker_type]
-                chunk_field_id = chunker_cls.chunk_field_id
-                annotators["call_graph"]["chunk_field_id"] = chunk_field_id
-            except StopIteration:
-                raise ValueError(
-                    "Call graph annotator requires a chunker annotator to be specified."
-                )
-
         if self.verbose:
             print(f"Initializing annotators: {list(annotators.keys())}...")
-        self.pipeline: dict[str, Annotator] = {
-            ann: annotators_map[ann](
-                **kwargs, verbose=self.verbose, spice_client=spice_client
+        self.pipeline = {}
+        for ann, kwargs in annotators.items():
+            self.pipeline[ann] = annotators_map[ann](
+                **kwargs,
+                verbose=self.verbose,
+                spice_client=spice_client,
+                pipeline=self.pipeline,
             )
-            for ann, kwargs in annotators.items()
-        }
 
     @property
     def db(self) -> Database:
         if not hasattr(self, "_db"):
             self._db = get_db(
                 self.cwd,
                 spice_client=self.spice_client,
@@ -138,17 +127,22 @@
                         _update_task.cancel()
                         await _update_task
                     except asyncio.CancelledError:
                         pass
                 last_updated = _last_updated
                 _update_task = asyncio.create_task(self.update())
 
-    def search(self, query: str, n: Optional[int] = None) -> list[dict[str, Any]]:
+    def search(
+        self,
+        query: str,
+        n: Optional[int] = None,
+        node_types: Iterable[str] = ("file", "chunk", "diff"),
+    ) -> list[dict[str, Any]]:
         """Return a sorted list of nodes that match the query."""
-        return self.db.query_graph(query, self.graph, n=n)
+        return self.db.query_graph(query, self.graph, n=n, node_types=node_types)
 
     def get_document(self, filename: str) -> str:
         checksum = self.graph.nodes[filename]["checksum"]
         document = self.db.get(checksum)["documents"][0]
         return document
 
     def get_context(
```

### Comparing `ragdaemon-0.4.4/ragdaemon/get_paths.py` & `ragdaemon-0.4.5/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/graph.py` & `ragdaemon-0.4.5/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/utils.py` & `ragdaemon-0.4.5/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/__init__.py` & `ragdaemon-0.4.5/ragdaemon/annotators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from ragdaemon.annotators.chunker import Chunker
 from ragdaemon.annotators.chunker_line import ChunkerLine
 from ragdaemon.annotators.chunker_llm import ChunkerLLM
 from ragdaemon.annotators.diff import Diff
 from ragdaemon.annotators.hierarchy import Hierarchy
 from ragdaemon.annotators.layout_hierarchy import LayoutHierarchy
 from ragdaemon.annotators.summarizer import Summarizer
+from ragdaemon.annotators.clusterer_binary import ClustererBinary
 
 annotators_map = {
-    "hierarchy": Hierarchy,
     "call_graph": CallGraph,
     "chunker": Chunker,
-    "chunker_llm": ChunkerLLM,
     "chunker_line": ChunkerLine,
+    "chunker_llm": ChunkerLLM,
+    "clusterer_binary": ClustererBinary,
     "diff": Diff,
+    "hierarchy": Hierarchy,
     "layout_hierarchy": LayoutHierarchy,
     "summarizer": Summarizer,
 }
```

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.4.5/ragdaemon/annotators/base_annotator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+from __future__ import annotations
+
 from typing import Optional
 
 from spice import Spice
 
 from ragdaemon.database import Database
 from ragdaemon.graph import KnowledgeGraph
 
 
 class Annotator:
     name: str = "base_annotator"
 
-    def __init__(self, verbose: bool = False, spice_client: Optional[Spice] = None):
+    def __init__(
+        self,
+        verbose: bool = False,
+        spice_client: Optional[Spice] = None,
+        pipeline: Optional[list[Annotator]] = None,
+    ):
         self.verbose = verbose
         self.spice_client = spice_client
         pass
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         raise NotImplementedError()
```

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.4.5/ragdaemon/annotators/call_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,24 +35,30 @@
     name = "call_graph"
     call_field_id = "calls"
 
     def __init__(
         self,
         *args,
         call_extensions: Optional[list[str]] = None,
-        chunk_field_id: Optional[str] = None,
         model: Optional[TextModel | str] = DEFAULT_COMPLETION_MODEL,
+        pipeline: list[Annotator] = [],
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         if call_extensions is None:
             call_extensions = DEFAULT_CODE_EXTENSIONS
         self.call_extensions = call_extensions
-        if chunk_field_id is None:
-            raise RagdaemonError("Chunk field ID is required for call graph annotator.")
+        try:
+            chunk_field_id = next(
+                getattr(a, "chunk_field_id") for a in pipeline if "chunker" in a.name
+            )
+        except (StopIteration, AttributeError):
+            raise RagdaemonError(
+                "CallGraph annotator requires a 'chunker' annotator with chunk_field_id."
+            )
         self.chunk_field_id = chunk_field_id
         self.model = model
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         for node, data in graph.nodes(data=True):
             if data is None:
                 raise RagdaemonError(f"Node {node} has no data.")
```

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/chunker.py` & `ragdaemon-0.4.5/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.4.5/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.4.5/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/diff.py` & `ragdaemon-0.4.5/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.4.5/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.4.5/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.4.5/ragdaemon/annotators/summarizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,27 +24,28 @@
 Python functions) which are integral to the functioning of the target code. Include a
 maximum of two (2) such named functions, but err on the side of brevity.
 """
 
 
 class Summarizer(Annotator):
     name = "summarizer"
+    summary_field_id = "summary"
 
     def __init__(
         self,
         *args,
         model: Optional[TextModel | str] = DEFAULT_COMPLETION_MODEL,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.model = model
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         return all(
-            data.get("summary") is not None
+            data.get(self.summary_field_id) is not None
             for _, data in graph.nodes(data=True)
             if data is not None and data.get("checksum") is not None
         )
 
     async def get_llm_response(self, document: str) -> str:
         if self.spice_client is None:
             raise RagdaemonError("Spice client is not initialized.")
@@ -61,27 +62,27 @@
 
     async def get_summary(self, data: dict[str, Any], db: Database):
         """Asynchronously generate summary and update graph and db"""
         record = db.get(data["checksum"])
         document = record["documents"][0]
         metadatas = record["metadatas"][0]
         summary = await self.get_llm_response(document)
-        metadatas["summary"] = summary
+        metadatas[self.summary_field_id] = summary
         db.update(data["checksum"], metadatas=metadatas)
-        data["summary"] = summary
+        data[self.summary_field_id] = summary
 
     async def annotate(
         self, graph: KnowledgeGraph, db: Database, refresh: bool = False
     ) -> KnowledgeGraph:
         # Generate/add summaries to nodes with checksums (file, chunk, diff)
         tasks = []
         for _, data in graph.nodes(data=True):
             if data is None or data.get("checksum") is None:
                 continue
-            if data.get("summary") is not None and not refresh:
+            if data.get(self.summary_field_id) is not None and not refresh:
                 continue
             tasks.append(self.get_summary(data, db))
         if len(tasks) > 0:
             if self.verbose:
                 await tqdm.gather(*tasks, desc="Summarizing code...")
             else:
                 await asyncio.gather(*tasks)
```

### Comparing `ragdaemon-0.4.4/ragdaemon/database/__init__.py` & `ragdaemon-0.4.5/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/database/chroma_database.py` & `ragdaemon-0.4.5/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/database/database.py` & `ragdaemon-0.4.5/ragdaemon/database/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Optional
+from typing import Iterable, Optional
 
 from ragdaemon.graph import KnowledgeGraph
 
 
 class Database:
     embedding_model: str | None = None
     _collection = None  # Collection | LiteDB
@@ -15,26 +15,30 @@
         """Delegate attribute access to the collection."""
         return getattr(self._collection, name)
 
     def query(self, query: str, active_checksums: list[str]) -> list[dict]:
         raise NotImplementedError
 
     def query_graph(
-        self, query: str, graph: KnowledgeGraph, n: Optional[int] = None
+        self,
+        query: str,
+        graph: KnowledgeGraph,
+        n: Optional[int] = None,
+        node_types: Iterable[str] = ("file", "chunk", "diff"),
     ) -> list[dict]:
         """Return documents, metadatas and distances, sorted, for nodes in the graph.
 
         Chroma's default search covers all records, including inactive ones, so we
         manually flag the active records, query them, and then unflag them.
         """
         active_checksums = list(
             {
                 data["checksum"]
                 for _, data in graph.nodes(data=True)
-                if data and "checksum" in data
+                if data and "checksum" in data and data["type"] in node_types
             }
         )
         results = self.query(query, active_checksums)
 
         # Add exact-match multiplier
         for result in results:
             distance = result["distance"]
```

### Comparing `ragdaemon-0.4.4/ragdaemon/database/lite_database.py` & `ragdaemon-0.4.5/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.4.5/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.4.5/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/static/favicon.ico` & `ragdaemon-0.4.5/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.4.5/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/static/js/main.js` & `ragdaemon-0.4.5/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.4.5/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/static/js/three/node.js` & `ragdaemon-0.4.5/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.4.5/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/ragdaemon/templates/index.html` & `ragdaemon-0.4.5/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/conftest.py` & `ragdaemon-0.4.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/test_comments.py` & `ragdaemon-0.4.5/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/test_context.py` & `ragdaemon-0.4.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/test_daemon.py` & `ragdaemon-0.4.5/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/test_get_paths.py` & `ragdaemon-0.4.5/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/test_sample.py` & `ragdaemon-0.4.5/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/annotators/test_chunker.py` & `ragdaemon-0.4.5/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.4.5/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/annotators/test_diff.py` & `ragdaemon-0.4.5/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/annotators/test_hierarchy.py` & `ragdaemon-0.4.5/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.4.5/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/annotators/test_summarizer.py` & `ragdaemon-0.4.5/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/data/chunker_graph.json` & `ragdaemon-0.4.5/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/data/context_message.txt` & `ragdaemon-0.4.5/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/data/diff_graph.json` & `ragdaemon-0.4.5/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/data/hard_to_chunk.txt` & `ragdaemon-0.4.5/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/data/hierarchy_graph.json` & `ragdaemon-0.4.5/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.4.5/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/tests/sample/src/interface.py` & `ragdaemon-0.4.5/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/LICENSE` & `ragdaemon-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/README.md` & `ragdaemon-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.4/pyproject.toml` & `ragdaemon-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.4.4"
+version = "0.4.5"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.4.4/PKG-INFO` & `ragdaemon-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.4.4
+Version: 0.4.5
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```


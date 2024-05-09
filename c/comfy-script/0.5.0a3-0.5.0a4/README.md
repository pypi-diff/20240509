# Comparing `tmp/comfy_script-0.5.0a3.tar.gz` & `tmp/comfy_script-0.5.0a4.tar.gz`

## Comparing `comfy_script-0.5.0a3.tar` & `comfy_script-0.5.0a4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/requirements.txt
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/settings.example.toml
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/.vscode/launch.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/README.md
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Runtime.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Transpiler.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Image/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Latent/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Models/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/Nodes/README.md
--rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/auto-queue.png
--rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/diff.png
--rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/plot.png
--rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/select.png
--rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/type-stubs.png
--rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/type-stubs2.png
--rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/workflow.png
--rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/README/workflow2.png
--rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/docs/images/Runtime/load-api-format.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/astutil.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/config.py
--rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/client/__init__.py
--rw-r--r--   0        0        0     8525 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/nodes/__init__.py
--rw-r--r--   0        0        0    45421 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/__init__.py
--rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/factory.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/nodes.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/data/Images.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/data/__init__.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/real/__init__.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/runtime/real/nodes.py
--rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/transpile/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/transpile/__main__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/transpile/prompt.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/transpile/passes/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/ui/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/ui/solara/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/src/comfy_script/ui/solara/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/test_astutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/transpile/__init__.py
--rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/transpile/bypass.json
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/transpile/default.json
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/tests/transpile/test_transpiler.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/LICENSE.txt
--rw-r--r--   0        0        0    14584 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/README.md
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/pyproject.toml
--rw-r--r--   0        0        0    16315 2020-02-02 00:00:00.000000 comfy_script-0.5.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/requirements.txt
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/settings.example.toml
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/.vscode/launch.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/README.md
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Runtime.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Transpiler.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Image/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Latent/README.md
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Models/README.md
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/Nodes/README.md
+-rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/auto-queue.png
+-rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/diff.png
+-rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/plot.png
+-rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/select.png
+-rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/type-stubs.png
+-rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/type-stubs2.png
+-rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/workflow.png
+-rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/README/workflow2.png
+-rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/docs/images/Runtime/load-api-format.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/astutil.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/config.py
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/client/__init__.py
+-rw-r--r--   0        0        0     8525 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/nodes/__init__.py
+-rw-r--r--   0        0        0    44839 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/__init__.py
+-rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/factory.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/nodes.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/data/Images.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/data/__init__.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/real/__init__.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/runtime/real/nodes.py
+-rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/transpile/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/transpile/__main__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/transpile/prompt.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/transpile/passes/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/ui/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/ui/solara/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/src/comfy_script/ui/solara/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/test_astutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/transpile/__init__.py
+-rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/transpile/bypass.json
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/transpile/default.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/tests/transpile/test_transpiler.py
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/LICENSE.txt
+-rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/README.md
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/pyproject.toml
+-rw-r--r--   0        0        0    16502 2020-02-02 00:00:00.000000 comfy_script-0.5.0a4/PKG-INFO
```

### Comparing `comfy_script-0.5.0a3/__init__.py` & `comfy_script-0.5.0a4/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/settings.example.toml` & `comfy_script-0.5.0a4/settings.example.toml`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/README.md` & `comfy_script-0.5.0a4/docs/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/Runtime.md` & `comfy_script-0.5.0a4/docs/Runtime.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/Image/README.md` & `comfy_script-0.5.0a4/docs/Image/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/Latent/README.md` & `comfy_script-0.5.0a4/docs/Latent/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/images/README/auto-queue.png` & `comfy_script-0.5.0a4/docs/images/README/auto-queue.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/images/README/diff.png` & `comfy_script-0.5.0a4/docs/images/README/diff.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/images/README/plot.png` & `comfy_script-0.5.0a4/docs/images/README/plot.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/images/README/select.png` & `comfy_script-0.5.0a4/docs/images/README/select.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/images/README/type-stubs.png` & `comfy_script-0.5.0a4/docs/images/README/type-stubs.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/images/README/type-stubs2.png` & `comfy_script-0.5.0a4/docs/images/README/type-stubs2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/images/README/workflow.png` & `comfy_script-0.5.0a4/docs/images/README/workflow.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/images/README/workflow2.png` & `comfy_script-0.5.0a4/docs/images/README/workflow2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/docs/images/Runtime/load-api-format.png` & `comfy_script-0.5.0a4/docs/images/Runtime/load-api-format.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/astutil.py` & `comfy_script-0.5.0a4/src/comfy_script/astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/client/__init__.py` & `comfy_script-0.5.0a4/src/comfy_script/client/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/nodes/__init__.py` & `comfy_script-0.5.0a4/src/comfy_script/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/runtime/__init__.py` & `comfy_script-0.5.0a4/src/comfy_script/runtime/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -412,37 +412,14 @@
     if prompt_queue is None:
         return
 
     import time
     while prompt_queue.get_tasks_remaining() != 0:
         time.sleep(0.1)
 
-def _print_progress(iteration, total, prefix = '', suffix = '', decimals = 0, length = 50, fill = '█', printEnd = '\r'):
-    """
-    Call in a loop to create terminal progress bar
-    @params:
-        iteration   - Required  : current iteration (Int)
-        total       - Required  : total iterations (Int)
-        prefix      - Optional  : prefix string (Str)
-        suffix      - Optional  : suffix string (Str)
-        decimals    - Optional  : positive number of decimals in percent complete (Int)
-        length      - Optional  : character length of bar (Int)
-        fill        - Optional  : bar fill character (Str)
-        printEnd    - Optional  : end character (e.g. "\r", "\r\n") (Str)
-    
-    From https://stackoverflow.com/questions/3173320/text-progress-bar-in-terminal-with-block-characters
-    """
-    percent = ("{0:3." + str(decimals) + "f}").format(100 * (iteration / float(total)))
-    filledLength = int(length * iteration // total)
-    bar = fill * filledLength + '-' * (length - filledLength)
-    print(f'\r{prefix}{percent}%|{bar}| {iteration}/{total}{suffix}', end = printEnd)
-    # Print New Line on Complete
-    if iteration == total: 
-        print()
-
 class TaskQueue:
     def __init__(self):
         self._tasks = {}
         self._watch_thread = None
         self._queue_empty_callback = None
         self._queue_remaining_callbacks = [self._when_empty_callback]
         self._watch_display_node = None
@@ -457,14 +434,17 @@
                     json = await response.json()
                     # print(json)
                     return json.get(prompt_id)
                 else:
                     print(f'ComfyScript: Failed to get history: {await client.response_to_str(response)}')
 
     async def _watch(self):
+        from tqdm.auto import tqdm
+        pbar = None
+
         while True:
             try:
                 async with client.client.session() as session:
                     async with session.ws_connect(f'{client.client.base_url}ws', params={'clientId': _client_id}) as ws:
                         self.queue_remaining = 0
                         executing = False
                         progress_data = None
@@ -518,15 +498,25 @@
                                         if self._watch_display_node:
                                             print(f'Queue remaining: {self.queue_remaining}')
                                 elif msg['type'] == 'progress':
                                     # See ComfyUI::main.hijack_progress
                                     # 'prompt_id', 'node': https://github.com/comfyanonymous/ComfyUI/issues/2425
                                     progress_data = msg['data']
                                     # TODO: Node
-                                    _print_progress(progress_data['value'], progress_data['max'])
+                                    value = progress_data['value']
+                                    max = progress_data['max']
+                                    if value == 1:
+                                        if pbar is not None:
+                                            pbar.close()
+                                        pbar = tqdm(initial=value, total=max)
+                                    else:
+                                        pbar.update(value - pbar.n)
+                                        if value == max:
+                                            pbar.close()
+                                            pbar = None
                             elif msg.type == aiohttp.WSMsgType.BINARY:
                                 event = client.BinaryEvent.from_bytes(msg.data)
                                 if event.type == client.BinaryEventTypes.PREVIEW_IMAGE:
                                     prompt_id = progress_data.get('prompt_id')
                                     if prompt_id is not None:
                                         task: Task = self._tasks.get(prompt_id)
                                         task._set_node_preview(progress_data['node'], event.to_object(), self._watch_display_node_preview)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `comfy_script-0.5.0a3/src/comfy_script/runtime/factory.py` & `comfy_script-0.5.0a4/src/comfy_script/runtime/factory.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/runtime/nodes.py` & `comfy_script-0.5.0a4/src/comfy_script/runtime/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/runtime/data/Images.py` & `comfy_script-0.5.0a4/src/comfy_script/runtime/data/Images.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/runtime/data/__init__.py` & `comfy_script-0.5.0a4/src/comfy_script/runtime/data/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/runtime/real/__init__.py` & `comfy_script-0.5.0a4/src/comfy_script/runtime/real/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/runtime/real/nodes.py` & `comfy_script-0.5.0a4/src/comfy_script/runtime/real/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/transpile/__init__.py` & `comfy_script-0.5.0a4/src/comfy_script/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/transpile/prompt.py` & `comfy_script-0.5.0a4/src/comfy_script/transpile/prompt.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/transpile/passes/__init__.py` & `comfy_script-0.5.0a4/src/comfy_script/transpile/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/src/comfy_script/ui/solara/metadata.py` & `comfy_script-0.5.0a4/src/comfy_script/ui/solara/metadata.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/tests/test_astutil.py` & `comfy_script-0.5.0a4/tests/test_astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/tests/transpile/bypass.json` & `comfy_script-0.5.0a4/tests/transpile/bypass.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/tests/transpile/default.json` & `comfy_script-0.5.0a4/tests/transpile/default.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/tests/transpile/test_transpiler.py` & `comfy_script-0.5.0a4/tests/transpile/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/.gitignore` & `comfy_script-0.5.0a4/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 private/
 *.private
 *.private.*
 
 /examples
 
 # Ignore dynaconf files
+/settings.toml
 .secrets.*
 *.local.*
 
 # Hatch will only respect the first .gitignore file
 /src/comfy_script/runtime/**/*.pyi
```

### Comparing `comfy_script-0.5.0a3/LICENSE.txt` & `comfy_script-0.5.0a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a3/README.md` & `comfy_script-0.5.0a4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -296,12 +296,13 @@
 Screenshot:
 
 ![](docs/images/README/select.png)
 
 ## [Documentation](docs/README.md)
 - [Runtime](docs/Runtime.md)
 - [Images](docs/Image/README.md)
+- [Models](docs/Models/README.md)
 - [Additional Nodes](docs/Nodes/README.md)
 - [Transpiler](docs/Transpiler.md)
 
 
 [^graph-gui]: [I hate nodes. (No offense comfyui) : StableDiffusion](https://www.reddit.com/r/StableDiffusion/comments/15cr5xx/i_hate_nodes_no_offense_comfyui/)
```

### Comparing `comfy_script-0.5.0a3/pyproject.toml` & `comfy_script-0.5.0a4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comfy-script"
-version = "0.5.0a3"
+version = "0.5.0a4"
 description = "A Python front end and library for ComfyUI"
 readme = "README.md"
 # ComfyUI: >=3.8
 # comfyui: >=3.9
 # >=3.6 is required to preserve insertion order of input types
 requires-python = ">=3.9"
 authors = [
@@ -46,27 +46,30 @@
   "dynaconf ~= 3.0",
 ]
 
 # Runtime
 runtime = [
   # Already required by ComfyUI
   "Pillow",
+  "tqdm ~= 4.0",
 
   "wrapt ~= 1.0",
 
   "comfy-script[client]",
 
   # Used to save script to images
   "comfy-script[transpile]",
 ]
 
 # Addtional nodes
+# See docs/Nodes/README.md for details 
 nodes = [
   "ComfyUI_Ib_CustomNodes >= 0.2.2",
   "comfyui-tooling-nodes",
+  "civitai_comfy_nodes",
 ]
 
 # Everything except UI (Jupyter and CLI)
 no-ui = [
   "comfy-script[client]",
   "comfy-script[transpile]",
   "comfy-script[runtime]",
@@ -75,14 +78,16 @@
 
 # Jupyter Notebook UI
 jupyter = [
   "ipywidgets ~= 8.1",
 
   # Already required by ComfyUI
   "Pillow",
+
+  "tqdm[notebook] ~= 4.0",
 ]
 
 default = [
   "comfy-script[no-ui]",
   "comfy-script[jupyter]",
 ]
```

### Comparing `comfy_script-0.5.0a3/PKG-INFO` & `comfy_script-0.5.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-script
-Version: 0.5.0a3
+Version: 0.5.0a4
 Summary: A Python front end and library for ComfyUI
 Project-URL: Homepage, https://github.com/Chaoses-Ib/ComfyScript
 Project-URL: Issues, https://github.com/Chaoses-Ib/ComfyScript/issues
 Author-email: Chaoses-Ib <Chaos-es@outlook.com>
 License-File: LICENSE.txt
 Keywords: comfyui
 Classifier: License :: OSI Approved :: MIT License
@@ -24,26 +24,29 @@
 Requires-Dist: yarl; extra == 'client'
 Provides-Extra: default
 Requires-Dist: comfy-script[jupyter]; extra == 'default'
 Requires-Dist: comfy-script[no-ui]; extra == 'default'
 Provides-Extra: jupyter
 Requires-Dist: ipywidgets~=8.1; extra == 'jupyter'
 Requires-Dist: pillow; extra == 'jupyter'
+Requires-Dist: tqdm[notebook]~=4.0; extra == 'jupyter'
 Provides-Extra: no-ui
 Requires-Dist: comfy-script[client]; extra == 'no-ui'
 Requires-Dist: comfy-script[nodes]; extra == 'no-ui'
 Requires-Dist: comfy-script[runtime]; extra == 'no-ui'
 Requires-Dist: comfy-script[transpile]; extra == 'no-ui'
 Provides-Extra: nodes
+Requires-Dist: civitai-comfy-nodes; extra == 'nodes'
 Requires-Dist: comfyui-ib-customnodes>=0.2.2; extra == 'nodes'
 Requires-Dist: comfyui-tooling-nodes; extra == 'nodes'
 Provides-Extra: runtime
 Requires-Dist: comfy-script[client]; extra == 'runtime'
 Requires-Dist: comfy-script[transpile]; extra == 'runtime'
 Requires-Dist: pillow; extra == 'runtime'
+Requires-Dist: tqdm~=4.0; extra == 'runtime'
 Requires-Dist: wrapt~=1.0; extra == 'runtime'
 Provides-Extra: transpile
 Requires-Dist: comfy-script[client]; extra == 'transpile'
 Requires-Dist: dynaconf~=3.0; extra == 'transpile'
 Requires-Dist: networkx[default]~=3.0; extra == 'transpile'
 Description-Content-Type: text/markdown
 
@@ -345,12 +348,13 @@
 Screenshot:
 
 ![](docs/images/README/select.png)
 
 ## [Documentation](docs/README.md)
 - [Runtime](docs/Runtime.md)
 - [Images](docs/Image/README.md)
+- [Models](docs/Models/README.md)
 - [Additional Nodes](docs/Nodes/README.md)
 - [Transpiler](docs/Transpiler.md)
 
 
 [^graph-gui]: [I hate nodes. (No offense comfyui) : StableDiffusion](https://www.reddit.com/r/StableDiffusion/comments/15cr5xx/i_hate_nodes_no_offense_comfyui/)
```


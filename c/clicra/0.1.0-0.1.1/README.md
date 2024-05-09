# Comparing `tmp/clicra-0.1.0.tar.gz` & `tmp/clicra-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clicra-0.1.0.tar", last modified: Thu May  9 04:23:13 2024, max compression
+gzip compressed data, was "clicra-0.1.1.tar", last modified: Thu May  9 13:18:55 2024, max compression
```

## Comparing `clicra-0.1.0.tar` & `clicra-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-09 04:23:13.845153 clicra-0.1.0/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     3167 2024-05-09 02:31:12.000000 clicra-0.1.0/.gitignore
--rw-r--r--   0 toshihiro  (1000) toshihiro  (1000)     2361 2024-05-09 04:23:13.845153 clicra-0.1.0/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1696 2024-05-09 04:19:50.000000 clicra-0.1.0/README.md
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-09 04:23:13.841153 clicra-0.1.0/clicra/
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       25 2024-05-09 01:28:09.000000 clicra-0.1.0/clicra/__init__.py
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     6224 2024-05-09 02:32:30.000000 clicra-0.1.0/clicra/clicra.py
-drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-09 04:23:13.841153 clicra-0.1.0/clicra.egg-info/
--rw-r--r--   0 toshihiro  (1000) toshihiro  (1000)     2361 2024-05-09 04:23:13.000000 clicra-0.1.0/clicra.egg-info/PKG-INFO
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2024-05-09 04:23:13.000000 clicra-0.1.0/clicra.egg-info/SOURCES.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2024-05-09 04:23:13.000000 clicra-0.1.0/clicra.egg-info/dependency_links.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       39 2024-05-09 04:23:13.000000 clicra-0.1.0/clicra.egg-info/entry_points.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       63 2024-05-09 04:23:13.000000 clicra-0.1.0/clicra.egg-info/requires.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        7 2024-05-09 04:23:13.000000 clicra-0.1.0/clicra.egg-info/top_level.txt
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      863 2024-05-09 02:53:24.000000 clicra-0.1.0/pyproject.toml
--rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2024-05-09 04:23:13.845153 clicra-0.1.0/setup.cfg
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-09 13:18:55.202475 clicra-0.1.1/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     3167 2024-05-09 02:31:12.000000 clicra-0.1.1/.gitignore
+-rw-r--r--   0 toshihiro  (1000) toshihiro  (1000)     2106 2024-05-09 13:18:55.202475 clicra-0.1.1/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     1441 2024-05-09 08:49:04.000000 clicra-0.1.1/README.md
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-09 13:18:55.198475 clicra-0.1.1/clicra/
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       25 2024-05-09 01:28:09.000000 clicra-0.1.1/clicra/__init__.py
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)     7596 2024-05-09 08:39:51.000000 clicra-0.1.1/clicra/clicra.py
+drwxrwxr-x   0 toshihiro  (1000) toshihiro  (1000)        0 2024-05-09 13:18:55.202475 clicra-0.1.1/clicra.egg-info/
+-rw-r--r--   0 toshihiro  (1000) toshihiro  (1000)     2106 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/PKG-INFO
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      253 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/SOURCES.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        1 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/dependency_links.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       39 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/entry_points.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       63 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/requires.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)        7 2024-05-09 13:18:55.000000 clicra-0.1.1/clicra.egg-info/top_level.txt
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)      863 2024-05-09 08:03:46.000000 clicra-0.1.1/pyproject.toml
+-rw-rw-r--   0 toshihiro  (1000) toshihiro  (1000)       38 2024-05-09 13:18:55.202475 clicra-0.1.1/setup.cfg
```

### Comparing `clicra-0.1.0/.gitignore` & `clicra-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `clicra-0.1.0/PKG-INFO` & `clicra-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clicra
-Version: 0.1.0
+Version: 0.1.1
 Summary: A LLM command-line crafter
 Author-email: Toshihiro Kamiya <kamiya@mbj.nifty.com>
 License: MIT LICENSE
 Project-URL: Souce, https://github.com/tos-kamiya/clicra
 Keywords: cli-tool,LLM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -50,30 +50,22 @@
 clicra [options] <task>
 ```
 
 - `<task>`: Description of the task you want to execute.
 
 ### Options
 
+- `-m, --model`: Specifies the LLM to use (default is `llama3`).
 - `-r, --run`: Generates and executes the command without confirmation and analyzes the outcome if there are errors.
 - `-f, --refer`: Executes a specified command and uses its output as additional context to improve the accuracy and relevance of task command generation.
-- `-m, --model`: Specifies the LLM to use (default is `llama3`).
 
 ### Examples
 
 To find source files containing TODO comments, you can provide the output of `ls` as context. This allows `clicra` to recognize the directory structure and file types:
 
 ```sh
 clicra "Find TODOs in source files" -f "ls"
 ```
 
-To get the volume size of an HDD, using the output of `lsb_release -a` provides additional system information, helping to generate the correct command:
-
-```sh
-clicra "Get HDD volume size" -f "lsb_release -a"
-```
-
 ## Screenshots
 
-Here is a screenshot of `clicra` in use:
-
-![](imgs/screenshot1.png)
+![](imgs/screenshot2.png)
```

### Comparing `clicra-0.1.0/README.md` & `clicra-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -30,30 +30,22 @@
 clicra [options] <task>
 ```
 
 - `<task>`: Description of the task you want to execute.
 
 ### Options
 
+- `-m, --model`: Specifies the LLM to use (default is `llama3`).
 - `-r, --run`: Generates and executes the command without confirmation and analyzes the outcome if there are errors.
 - `-f, --refer`: Executes a specified command and uses its output as additional context to improve the accuracy and relevance of task command generation.
-- `-m, --model`: Specifies the LLM to use (default is `llama3`).
 
 ### Examples
 
 To find source files containing TODO comments, you can provide the output of `ls` as context. This allows `clicra` to recognize the directory structure and file types:
 
 ```sh
 clicra "Find TODOs in source files" -f "ls"
 ```
 
-To get the volume size of an HDD, using the output of `lsb_release -a` provides additional system information, helping to generate the correct command:
-
-```sh
-clicra "Get HDD volume size" -f "lsb_release -a"
-```
-
 ## Screenshots
 
-Here is a screenshot of `clicra` in use:
-
-![](imgs/screenshot1.png)
+![](imgs/screenshot2.png)
```

### Comparing `clicra-0.1.0/clicra/clicra.py` & `clicra-0.1.1/clicra/clicra.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,32 @@
     exit("Install `ollama-python` by following the instruction on: https://github.com/ollama/ollama-python")
 
 
 import pkg_resources
 _version = pkg_resources.get_distribution('clicra').version
 
 DEFAULT_LLM = "llama3"
+DEFAULT_OUTPUT_MAX_CHARS = 2000
+
+
+def clip_text(text: str, max_chars: int) -> str:
+    if len(text) == 0:
+        return ""
+
+    snip_str = " ...(snip)... "
+
+    newline_pos = text.find("\n")
+    if newline_pos < 0 or newline_pos > max_chars:
+        return text[:max_chars] + snip_str + "\n"
+
+    while newline_pos >= 0:
+        next_newline_pos = text.find("\n", newline_pos + 1)
+        if next_newline_pos < 0 or next_newline_pos > max_chars:
+            return text[:newline_pos + 1] + snip_str + "\n"
+        newline_pos = next_newline_pos
 
 
 def stream_reader(
     stream: IO, output: TextIO, output_list: List[str]
 ) -> None:
     for line in iter(stream.readline, b""):
         line = line.decode("utf-8")
@@ -95,16 +113,19 @@
         else:
             highlighted_lines.append(line)
             if not code_block and line.startswith("```"):
                 in_code_block = True
     return "\n".join(highlighted_lines), "\n".join(code_block)
 
 
-def format_command_generation_prompt(task: str, context: Optional[str]) -> str:
-    p = f"Please provide the command line to accomplish the following task."
+def format_command_generation_prompt(task: str, context: Optional[str], generate_script: bool = False) -> str:
+    if generate_script:
+        p = f"Please provide a script to accomplish the following task."
+    else:
+        p = f"Please provide a command line to accomplish the following task."
     if task:
         p += f"\n## TASK\n{task}\n"
     if context:
         p += f"\n## CONTEXT\n{context}\n"
     return p
 
 
@@ -119,22 +140,22 @@
         p += f"\n## STDOUT\n{stdout}\n"
     if stderr:
         p += f"\n## STDERR\n{stderr}\n"
 
     return p
 
 
-def build_reference_context(command: str) -> str:
+def build_reference_context(command: str, max_chars: int) -> str:
     context = None
     exit_code, stdout, stderr = do_run_and_capture(command, thru_output=False)
     r = ["```", f"$ {command}"]
     if stdout:
-        r.append(stdout)
+        r.append(clip_text(stdout, max_chars))
     if stderr:
-        r.append(stderr)
+        r.append(clip_text(stderr, max_chars))
     if exit_code != 0:
         r.append(f"EXIT CODE: {exit_code}")
     r.append("```")
     context = "\n".join(r)
     return context
 
 
@@ -154,34 +175,49 @@
     parser.add_argument(
         "-m",
         "--model",
         default=DEFAULT_LLM,
         help="LLM name to use.",
     )
     parser.add_argument(
+        "-s",
+        "--script",
+        action="store_true",
+        help="ask to generate a script (instead of a command line).",
+    )
+    parser.add_argument(
+        "-M",
+        "--max-chars",
+        type=int,
+        default=DEFAULT_OUTPUT_MAX_CHARS,
+        help="max characters of command execution results.",
+    )
+    parser.add_argument(
         "-v", "--verbose", action="store_true"
     )
     parser.add_argument("--version", action="version",
                         version=f"%(prog)s {_version}")
     args = parser.parse_args()
 
     if not args.task:
         exit("Error: no task is given. Option `-h` for help.")
+    if args.run and args.script:
+        exit("Error: options --generate-script and --run are mutually exclusive.")
     task = " ".join(args.task)
 
     def chat(prompt: str) -> str:
         response = ollama.chat(
             model=args.model,
             messages=[{"role": "user", "content": prompt}],
         )
         return response["message"]["content"]
 
-    context = build_reference_context(args.refer) if args.refer else None
+    context = build_reference_context(args.refer, args.max_chars) if args.refer else None
 
-    p = format_command_generation_prompt(task, context)
+    p = format_command_generation_prompt(task, context, generate_script=args.script)
     if args.verbose:
         for L in p.split("\n"):
             print(colored(L, attrs=["dark"]), file=sys.stderr)
     command = chat(p)
 
     highlighted_text, code = highlight_and_extract_code(command)
     print(highlighted_text)
@@ -189,15 +225,18 @@
     if code:
         if args.run:
             ht_run = colored(f"-- RUN", "yellow", attrs=["bold"])
             print(f"\n{ht_run}: {code}\n")
             exit_code, stdout, stderr = do_run_and_capture(code)
             if exit_code != 0:
                 print("\n" + colored("-- DEBUG", "yellow", attrs=["bold"]) + "\n")
-                p = format_analysis_prompt(code, task, context, stdout, stderr)
+                p = format_analysis_prompt(
+                    code, task, context,
+                    clip_text(stdout, args.max_chars), clip_text(stderr, args.max_chars)
+                )
                 if args.verbose:
                     for L in p.split("\n"):
                         print(colored(L, attrs=["dark"]), file=sys.stderr)
                 analysis = chat(p)
                 print(analysis)
             exit(exit_code)
         else:
```

### Comparing `clicra-0.1.0/clicra.egg-info/PKG-INFO` & `clicra-0.1.1/clicra.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clicra
-Version: 0.1.0
+Version: 0.1.1
 Summary: A LLM command-line crafter
 Author-email: Toshihiro Kamiya <kamiya@mbj.nifty.com>
 License: MIT LICENSE
 Project-URL: Souce, https://github.com/tos-kamiya/clicra
 Keywords: cli-tool,LLM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -50,30 +50,22 @@
 clicra [options] <task>
 ```
 
 - `<task>`: Description of the task you want to execute.
 
 ### Options
 
+- `-m, --model`: Specifies the LLM to use (default is `llama3`).
 - `-r, --run`: Generates and executes the command without confirmation and analyzes the outcome if there are errors.
 - `-f, --refer`: Executes a specified command and uses its output as additional context to improve the accuracy and relevance of task command generation.
-- `-m, --model`: Specifies the LLM to use (default is `llama3`).
 
 ### Examples
 
 To find source files containing TODO comments, you can provide the output of `ls` as context. This allows `clicra` to recognize the directory structure and file types:
 
 ```sh
 clicra "Find TODOs in source files" -f "ls"
 ```
 
-To get the volume size of an HDD, using the output of `lsb_release -a` provides additional system information, helping to generate the correct command:
-
-```sh
-clicra "Get HDD volume size" -f "lsb_release -a"
-```
-
 ## Screenshots
 
-Here is a screenshot of `clicra` in use:
-
-![](imgs/screenshot1.png)
+![](imgs/screenshot2.png)
```

### Comparing `clicra-0.1.0/pyproject.toml` & `clicra-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
     "Operating System :: POSIX :: Linux",
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 [project.scripts]
 clicra = "clicra:main"
 
 [project.urls]
 Souce = "https://github.com/tos-kamiya/clicra"
```


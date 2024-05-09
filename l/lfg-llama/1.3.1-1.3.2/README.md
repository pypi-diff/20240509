# Comparing `tmp/lfg_llama-1.3.1.tar.gz` & `tmp/lfg_llama-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.3.1.tar", last modified: Wed May  8 05:43:55 2024, max compression
+gzip compressed data, was "lfg_llama-1.3.2.tar", last modified: Thu May  9 07:31:38 2024, max compression
```

## Comparing `lfg_llama-1.3.1.tar` & `lfg_llama-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-08 05:43:55.137963 lfg_llama-1.3.1/
--rw-r--r--   0 ob907      (502) staff       (20)     1876 2024-05-08 05:43:55.137729 lfg_llama-1.3.1/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     1639 2024-05-04 07:48:10.000000 lfg_llama-1.3.1/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-08 05:43:55.135302 lfg_llama-1.3.1/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.3.1/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     3139 2024-05-08 05:40:17.000000 lfg_llama-1.3.1/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-08 05:43:55.137219 lfg_llama-1.3.1/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1876 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-08 05:43:55.000000 lfg_llama-1.3.1/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-08 05:43:55.138013 lfg_llama-1.3.1/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-08 05:43:47.000000 lfg_llama-1.3.1/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-09 07:31:38.732197 lfg_llama-1.3.2/
+-rw-r--r--   0 ob907      (502) staff       (20)     1908 2024-05-09 07:31:38.732002 lfg_llama-1.3.2/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     1671 2024-05-09 07:31:10.000000 lfg_llama-1.3.2/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-09 07:31:38.730719 lfg_llama-1.3.2/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.3.2/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     3470 2024-05-09 07:28:39.000000 lfg_llama-1.3.2/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-09 07:31:38.731805 lfg_llama-1.3.2/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1908 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-09 07:31:38.732354 lfg_llama-1.3.2/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-09 07:30:08.000000 lfg_llama-1.3.2/setup.py
```

### Comparing `lfg_llama-1.3.1/PKG-INFO` & `lfg_llama-1.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.3.1
+Version: 1.3.2
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
@@ -55,16 +55,17 @@
 lfg "kill port 3000"
 
 # Kill process listening on port 3000
 lsof -i :3000 | xargs kill
 
 ```
 
-Change the LLM 
-```bash 
+Change the LLM
+
+```bash
 $ lfg "list ec2 pipe json jq get name" -m llama370b
 
 # List EC2 instances with name
 
 aws ec2 describe-instances --query 'Reservations[].Instances[]|{Name:Tags[?Key==`Name`]|[0].Value,I
 nstanceId}' --output text | jq '.[] | {"Name", .Name, "InstanceId", .InstanceId}'
 
@@ -73,12 +74,14 @@
 
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.11
 pipenv install
+
+pipenv run lfg "kill port 3000"
 ```
 
 ### TODO
 
 - Fix the setup and pyproject file, including github workflow for releasing the package
```

### Comparing `lfg_llama-1.3.1/README.md` & `lfg_llama-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,17 @@
 lfg "kill port 3000"
 
 # Kill process listening on port 3000
 lsof -i :3000 | xargs kill
 
 ```
 
-Change the LLM 
-```bash 
+Change the LLM
+
+```bash
 $ lfg "list ec2 pipe json jq get name" -m llama370b
 
 # List EC2 instances with name
 
 aws ec2 describe-instances --query 'Reservations[].Instances[]|{Name:Tags[?Key==`Name`]|[0].Value,I
 nstanceId}' --output text | jq '.[] | {"Name", .Name, "InstanceId", .InstanceId}'
 
@@ -64,12 +65,14 @@
 
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.11
 pipenv install
+
+pipenv run lfg "kill port 3000"
 ```
 
 ### TODO
 
 - Fix the setup and pyproject file, including github workflow for releasing the package
```

### Comparing `lfg_llama-1.3.1/lfg/cli.py` & `lfg_llama-1.3.2/lfg/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #!/usr/bin/python3
 
 import os
 import sys
 import argparse
 from enum import Enum
 from groq import Groq
+from groq.types.chat import ChatCompletion
 
 
 class Models(Enum):
     """
-    Enumerates supported language models providing model ID references for API calls.
+    Enumerates supported language models providing model ID references
+    for API calls.
     """
 
     LLAMA38B = "llama3-8b-8192"
     LLAMA370B = "llama3-70b-8192"
     MIXTRAL8X7B = "mixtral-8x7b-32768"
     GEMMA7B = "gemma-7b-it"
 
@@ -32,19 +34,30 @@
 
 
 def generate_system_prompt() -> str:
     """Returns the system prompt for the LLM interaction."""
 
     return """
 You are a system administrator and elite hacker that knows all about the terminal in linux and mac. I provide you with a question about a command, and you give me back a response which shows the command, then a short explanation. The command should be wrapped as a code block. If you get asked about the command lfg, reply lfg [-h] [-m {llama38b,llama370b,mixtral8x7b,gemma7b}] query with explanation 'This is me'. It is important you do not return commands you do not know. If that is the case, just respond 'I do not know'.
- 
 """
 
 
-def send_chat_query(query: str, model: str, client: Groq) -> None:
+def handle_stream(stream: ChatCompletion) -> None:
+    """Processes the output stream from the LLM, printing each response chunk.
+
+    Args:
+        stream (ChatCompletion): An iterator of chunks representing
+        LLM responses.
+    """
+    for chunk in stream:
+        if chunk.choices[0].delta.content:
+            print(chunk.choices[0].delta.content, end="", flush=True)
+
+
+def send_chat_query(query: str, model: str, client: Groq) -> ChatCompletion:
     """Sends a query to the Groq API and handles the response.
 
     Args:
         query (str): The user's query.
         model (str): The LLM of choice
         client (Groq): The Groq client instance.
     """
@@ -54,23 +67,22 @@
                 {"role": "system", "content": generate_system_prompt()},
                 {"role": "user", "content": query},
             ],
             model=Models[model].value,
             stream=True,
         )
 
-        for chunk in stream:
-            if chunk.choices[0].delta.content:
-                print(chunk.choices[0].delta.content, end="", flush=True)
-    except groq.APIConnectionError as e:
+        return stream
+    except Groq.APIConnectionError as e:
         print("The server could not be reached")
         print(e.__cause__)
-    except groq.RateLimitError as e:
-        print("A 429 status code was received; we should back off a bit. Rate limited.")
-    except groq.APIStatusError as e:
+    except Groq.RateLimitError as e:
+        print("A 429 status code was received; Rate limited.")
+        print(e.response)
+    except Groq.APIStatusError as e:
         print("Another non-200-range status code was received")
         print(e.status_code)
         print(e.response)
 
 
 def main():
     """Initializes the Groq client, and processes the query."""
@@ -83,16 +95,16 @@
         default="llama370b",
         help="Select the language model.",
     )
     args = parser.parse_args()
 
     try:
         client = get_groq_client()
-        send_chat_query(args.query, args.m.upper(), client)
+        stream = send_chat_query(args.query, args.m.upper(), client)
 
-        return
+        handle_stream(stream)
     except ValueError as e:
         print(f"Error: {e}")
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `lfg_llama-1.3.1/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-1.3.2/lfg_llama.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.3.1
+Version: 1.3.2
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
@@ -55,16 +55,17 @@
 lfg "kill port 3000"
 
 # Kill process listening on port 3000
 lsof -i :3000 | xargs kill
 
 ```
 
-Change the LLM 
-```bash 
+Change the LLM
+
+```bash
 $ lfg "list ec2 pipe json jq get name" -m llama370b
 
 # List EC2 instances with name
 
 aws ec2 describe-instances --query 'Reservations[].Instances[]|{Name:Tags[?Key==`Name`]|[0].Value,I
 nstanceId}' --output text | jq '.[] | {"Name", .Name, "InstanceId", .InstanceId}'
 
@@ -73,12 +74,14 @@
 
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.11
 pipenv install
+
+pipenv run lfg "kill port 3000"
 ```
 
 ### TODO
 
 - Fix the setup and pyproject file, including github workflow for releasing the package
```


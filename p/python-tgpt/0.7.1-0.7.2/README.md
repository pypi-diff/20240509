# Comparing `tmp/python_tgpt-0.7.1.tar.gz` & `tmp/python_tgpt-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_tgpt-0.7.1.tar", last modified: Sat May  4 10:22:59 2024, max compression
+gzip compressed data, was "python_tgpt-0.7.2.tar", last modified: Thu May  9 11:09:40 2024, max compression
```

## Comparing `python_tgpt-0.7.1.tar` & `python_tgpt-0.7.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.882453 python_tgpt-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-05-04 10:22:59.882453 python_tgpt-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 10:22:59.882453 python_tgpt-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/pytgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/pytgpt/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17361 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/api/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/async_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/pytgpt/auto/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/auto/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    16877 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/auto/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.866453 python_tgpt-0.7.1/src/pytgpt/blackboxai/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/blackboxai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/blackboxai/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    85577 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gemini/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/gpt4all/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4all/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/gpt4free/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4free/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4free/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/gpt4free/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/groq/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/groq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/groq/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/imager/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/imager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/imager/imager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/koboldai/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/koboldai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/koboldai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/leo/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/leo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/leo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/llama2/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/llama2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/llama2/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19455 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/openai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.870453 python_tgpt-0.7.1/src/pytgpt/opengpt/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/opengpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/opengpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/perplexity/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/perplexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/perplexity/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/phind/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/phind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/phind/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/poe/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/poe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/poe/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    36065 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/webchatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/webchatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/webchatgpt/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.874453 python_tgpt-0.7.1/src/pytgpt/yepchat/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/yepchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/src/pytgpt/yepchat/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.878453 python_tgpt-0.7.1/src/python_tgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 10:22:59.000000 python_tgpt-0.7.1/src/python_tgpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 10:22:59.878453 python_tgpt-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_auto_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_blackboxai_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_gpt4free_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_groq.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_imager.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_koboldai_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_leo_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_llama2_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_opengpt_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_phind_tgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_poe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_webchatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-04 10:22:23.000000 python_tgpt-0.7.1/tests/test_yepchat_tgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.193881 python_tgpt-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23347 2024-05-09 11:09:40.193881 python_tgpt-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20308 2024-05-09 11:09:39.000000 python_tgpt-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 11:09:40.193881 python_tgpt-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.177881 python_tgpt-0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.181881 python_tgpt-0.7.2/src/pytgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.181881 python_tgpt-0.7.2/src/pytgpt/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17361 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/async_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.181881 python_tgpt-0.7.2/src/pytgpt/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/auto/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16877 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/auto/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.181881 python_tgpt-0.7.2/src/pytgpt/blackboxai/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/blackboxai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16048 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/blackboxai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85580 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.181881 python_tgpt-0.7.2/src/pytgpt/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/gemini/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.181881 python_tgpt-0.7.2/src/pytgpt/gpt4all/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/gpt4all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/gpt4all/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/gpt4free/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/gpt4free/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/gpt4free/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/gpt4free/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/groq/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/groq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/groq/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/imager/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/imager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/imager/imager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/koboldai/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/koboldai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/koboldai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/leo/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/leo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18641 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/leo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/llama2/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/llama2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/llama2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19455 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/openai/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/opengpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/opengpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/opengpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/perplexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/perplexity/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/phind/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/phind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19038 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/phind/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.185881 python_tgpt-0.7.2/src/pytgpt/poe/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/poe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/poe/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36006 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.189881 python_tgpt-0.7.2/src/pytgpt/webchatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/webchatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/webchatgpt/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.189881 python_tgpt-0.7.2/src/pytgpt/yepchat/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/yepchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19001 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/src/pytgpt/yepchat/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.193881 python_tgpt-0.7.2/src/python_tgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23347 2024-05-09 11:09:40.000000 python_tgpt-0.7.2/src/python_tgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-09 11:09:40.000000 python_tgpt-0.7.2/src/python_tgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 11:09:40.000000 python_tgpt-0.7.2/src/python_tgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 11:09:40.000000 python_tgpt-0.7.2/src/python_tgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 11:09:40.000000 python_tgpt-0.7.2/src/python_tgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 11:09:40.000000 python_tgpt-0.7.2/src/python_tgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 11:09:40.193881 python_tgpt-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_auto_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_blackboxai_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_gpt4free_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_imager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_koboldai_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_leo_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_llama2_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_opengpt_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_phind_tgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_poe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_webchatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 11:09:10.000000 python_tgpt-0.7.2/tests/test_yepchat_tgpt.py
```

### Comparing `python_tgpt-0.7.1/LICENSE` & `python_tgpt-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/PKG-INFO` & `python_tgpt-0.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.7.1
+Version: 0.7.2
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -34,38 +34,40 @@
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: webchatgpt==0.3.0
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
-Requires-Dist: g4f>=0.3.0.8
+Requires-Dist: g4f>=0.2.6.1
 Requires-Dist: Helpingai_T2-fork==0.3.2
 Requires-Dist: python-vlc>=3.0.20
 Requires-Dist: httpx==0.27.0
+Provides-Extra: termux
+Requires-Dist: g4f==0.2.6.1; extra == "termux"
 Provides-Extra: cli
 Requires-Dist: click==8.1.3; extra == "cli"
 Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: g4f>=0.3.0.8; extra == "cli"
+Requires-Dist: g4f>=0.2.6.1; extra == "cli"
 Requires-Dist: python-dotenv==1.0.0; extra == "cli"
 Provides-Extra: api
 Requires-Dist: fastapi[all]==0.110.1; extra == "api"
 Provides-Extra: all
 Requires-Dist: g4f[all]>=0.2.6.1; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: gpt4all==2.2.0; extra == "all"
 Requires-Dist: click==8.1.3; extra == "all"
 Requires-Dist: rich==13.3.4; extra == "all"
 Requires-Dist: clipman==3.1.0; extra == "all"
 Requires-Dist: pyperclip==1.8.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: g4f>=0.3.0.8; extra == "all"
+Requires-Dist: g4f>=0.2.6.1; extra == "all"
 Requires-Dist: python-dotenv==1.0.0; extra == "all"
 Requires-Dist: fastapi[all]==0.110.1; extra == "all"
 
 <p align="center">
 <img src="https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true" width='40%'>
 </p>
 
@@ -76,16 +78,14 @@
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href=""><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="https://python-tgpt.onrender.com"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
-<a href=""><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
-<a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/release-date/Simatwa/python-tgpt?label=Release date&logo=github" alt="release date"></img></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/python-tgpt"/></a>      
 <a href="https://wakatime.com/badge/github/Simatwa/tgpt2"><img src="https://wakatime.com/badge/github/Simatwa/tgpt2.svg" alt="wakatime"></a>
 </p>
@@ -545,15 +545,15 @@
 | ------------ | ----------- |
 | `{{stream}}` | The piped input |
 | `{{copied}}` | The last copied text |
 
 This feature is particularly beneficial for intricate operations. For example:
 
 ```bash
-$ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a concise commit message from it, aligning with my commit message history: {{copied}}" --shell --new
+$ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a concise commit message from it, aligning with my commit message history: {{copied}}" --new
 ```
 > In this illustration, `{{stream}}` denotes the result of the `$ git diff` operation, while `{{copied}}` signifies the content copied from the output of the `$ git log` command.
 
 ### Awesome Prompts
 
 [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/all-acts.pdf?raw=True) are designed to guide the AI's behavior or responses in a particular direction, encouraging it to exhibit certain characteristics or behaviors. The  term "awesome-prompt" is not a formal term in AI or machine learning literature, but it encapsulates the idea of crafting prompts that are effective in achieving desired outcomes. Let's say you want it to behave like a *Linux Terminal*, *PHP Interpreter*, or just to [**JAIL BREAK.**](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
 
@@ -624,16 +624,16 @@
 ```bash
 $ pytgpt api run
 ```
 
 This command starts the RESTful API server, enabling you to interact with the service programmatically.
 
 For accessing the documentation and redoc, navigate to the following paths in your web browser:
-- Documentation: `*/docs`
-- ReDoc: `*/redoc`
+- Documentation: `/docs`
+- ReDoc: `/redoc`
 
 ## Speech Synthesis
 
 To enable speech synthesis of responses, ensure you have either the [VLC player](https://www.videolan.org/vlc/index.html) installed on your system or, if you are a [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/wiki/Termux:API) package.
 
 To activate speech synthesis, use the `--talk-to-me` flag or its shorthand `-ttm` when running your commands. For example:
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.1 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.2 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -19,34 +19,35 @@
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1 Requires-Dist: webchatgpt==0.3.0 Requires-Dist:
 GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
-brotli==1.1.0 Requires-Dist: g4f>=0.3.0.8 Requires-Dist: Helpingai_T2-
+brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai_T2-
 fork==0.3.2 Requires-Dist: python-vlc>=3.0.20 Requires-Dist: httpx==0.27.0
-Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
+Provides-Extra: termux Requires-Dist: g4f==0.2.6.1; extra == "termux" Provides-
+Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
 rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
-extra == "cli" Requires-Dist: g4f>=0.3.0.8; extra == "cli" Requires-Dist:
+extra == "cli" Requires-Dist: g4f>=0.2.6.1; extra == "cli" Requires-Dist:
 python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
 [all]==0.110.1; extra == "api" Provides-Extra: all Requires-Dist: g4f
 [all]>=0.2.6.1; extra == "all" Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
 extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
 clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.3.0.8;
+Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.2.6.1;
 extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
 Dist: fastapi[all]==0.110.1; extra == "all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
   _[_L_i_c_e_n_s_e_][Python version]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
-   [coverage]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
-                 _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
-     _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
+         _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
+  _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
+                        _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
 ```python >>> import pytgpt.phind as phind >>> bot = phind.PHIND() >>> bot.chat
 ('hello there') 'Hello! How can I assist you today?' ``` ```python from
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
@@ -169,35 +170,35 @@
 comprehensive utilization of the `--with-copied` option and support for
 accepting piped inputs. This improvement introduces placeholders, offering
 dynamic values for more versatile interactions. | Placeholder | Represents | |
 ------------ | ----------- | | `{{stream}}` | The piped input | | `{{copied}}`
 | The last copied text | This feature is particularly beneficial for intricate
 operations. For example: ```bash $ git diff | pytgpt generate "Here is a diff
 file: {{stream}} Make a concise commit message from it, aligning with my commit
-message history: {{copied}}" --shell --new ``` > In this illustration, `{
-{stream}}` denotes the result of the `$ git diff` operation, while `{{copied}}`
-signifies the content copied from the output of the `$ git log` command. ###
-Awesome Prompts [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/
-assets/all-acts.pdf?raw=True) are designed to guide the AI's behavior or
-responses in a particular direction, encouraging it to exhibit certain
-characteristics or behaviors. The term "awesome-prompt" is not a formal term in
-AI or machine learning literature, but it encapsulates the idea of crafting
-prompts that are effective in achieving desired outcomes. Let's say you want it
-to behave like a *Linux Terminal*, *PHP Interpreter*, or just to [**JAIL
-BREAK.**](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
-Instances : ```sh $ pytgpt interactve --awesome-prompt "Linux Terminal" # Act
-like a Linux Terminal $ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] >
-Awesome prompts are alternative to `--intro`. > Run `$ pytgpt awesome whole` to
-list available prompts (*200+*). > Run `$ pytgpt awesome --help` for more info.
-### Introducing RawDog RawDog is a masterpiece feature that exploits the
-versatile capabilities of Python to command and control your system as per your
-needs. You can literally do anything with it, since it generates and executes
-python codes, driven by **your prompts**! To have a bite of *rawdog* simply
-append the flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode.
-This introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
+message history: {{copied}}" --new ``` > In this illustration, `{{stream}}`
+denotes the result of the `$ git diff` operation, while `{{copied}}` signifies
+the content copied from the output of the `$ git log` command. ### Awesome
+Prompts [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/
+all-acts.pdf?raw=True) are designed to guide the AI's behavior or responses in
+a particular direction, encouraging it to exhibit certain characteristics or
+behaviors. The term "awesome-prompt" is not a formal term in AI or machine
+learning literature, but it encapsulates the idea of crafting prompts that are
+effective in achieving desired outcomes. Let's say you want it to behave like a
+*Linux Terminal*, *PHP Interpreter*, or just to [**JAIL BREAK.**](https://
+gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516) Instances : ```sh $
+pytgpt interactve --awesome-prompt "Linux Terminal" # Act like a Linux Terminal
+$ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] > Awesome prompts are
+alternative to `--intro`. > Run `$ pytgpt awesome whole` to list available
+prompts (*200+*). > Run `$ pytgpt awesome --help` for more info. ###
+Introducing RawDog RawDog is a masterpiece feature that exploits the versatile
+capabilities of Python to command and control your system as per your needs.
+You can literally do anything with it, since it generates and executes python
+codes, driven by **your prompts**! To have a bite of *rawdog* simply append the
+flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode. This
+introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
 [AbanteAI/rawdog](https://github.com/AbanteAI/rawdog) for the idea. This can be
 useful in some ways. For instance : ```sh $ pytgpt generate -n -q "Visualize
 the disk usage using pie chart" --rawdog ``` This will pop up a window showing
 system disk usage as shown below.
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/Figure_1.png?raw=true]
 ## Passing Environment Variables Pytgpt **v0.4.6** introduces a convention way
 of taking variables from the environment. To achieve that, set the environment
@@ -221,15 +222,15 @@
 API. Access docs and redoc at */docs* and */redoc* respectively. To launch the
 web interface for g4f-based providers, execute the following command in your
 terminal: ```bash $ pytgpt gpt4free gui ``` This command initializes the Web-
 user interface for interacting with g4f-based providers. To start the REST-API:
 ```bash $ pytgpt api run ``` This command starts the RESTful API server,
 enabling you to interact with the service programmatically. For accessing the
 documentation and redoc, navigate to the following paths in your web browser: -
-Documentation: `*/docs` - ReDoc: `*/redoc` ## Speech Synthesis To enable speech
+Documentation: `/docs` - ReDoc: `/redoc` ## Speech Synthesis To enable speech
 synthesis of responses, ensure you have either the [VLC player](https://
 www.videolan.org/vlc/index.html) installed on your system or, if you are a
 [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/
 wiki/Termux:API) package. To activate speech synthesis, use the `--talk-to-me`
 flag or its shorthand `-ttm` when running your commands. For example: ```bash $
 pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
 interactive -ttm ``` This flag instructs the system to audiolize the ai
```

### Comparing `python_tgpt-0.7.1/README.md` & `python_tgpt-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href=""><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="https://python-tgpt.onrender.com"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
-<a href=""><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
-<a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/release-date/Simatwa/python-tgpt?label=Release date&logo=github" alt="release date"></img></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/python-tgpt"/></a>      
 <a href="https://wakatime.com/badge/github/Simatwa/tgpt2"><img src="https://wakatime.com/badge/github/Simatwa/tgpt2.svg" alt="wakatime"></a>
 </p>
@@ -478,15 +476,15 @@
 | ------------ | ----------- |
 | `{{stream}}` | The piped input |
 | `{{copied}}` | The last copied text |
 
 This feature is particularly beneficial for intricate operations. For example:
 
 ```bash
-$ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a concise commit message from it, aligning with my commit message history: {{copied}}" --shell --new
+$ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a concise commit message from it, aligning with my commit message history: {{copied}}" --new
 ```
 > In this illustration, `{{stream}}` denotes the result of the `$ git diff` operation, while `{{copied}}` signifies the content copied from the output of the `$ git log` command.
 
 ### Awesome Prompts
 
 [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/all-acts.pdf?raw=True) are designed to guide the AI's behavior or responses in a particular direction, encouraging it to exhibit certain characteristics or behaviors. The  term "awesome-prompt" is not a formal term in AI or machine learning literature, but it encapsulates the idea of crafting prompts that are effective in achieving desired outcomes. Let's say you want it to behave like a *Linux Terminal*, *PHP Interpreter*, or just to [**JAIL BREAK.**](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
 
@@ -557,16 +555,16 @@
 ```bash
 $ pytgpt api run
 ```
 
 This command starts the RESTful API server, enabling you to interact with the service programmatically.
 
 For accessing the documentation and redoc, navigate to the following paths in your web browser:
-- Documentation: `*/docs`
-- ReDoc: `*/redoc`
+- Documentation: `/docs`
+- ReDoc: `/redoc`
 
 ## Speech Synthesis
 
 To enable speech synthesis of responses, ensure you have either the [VLC player](https://www.videolan.org/vlc/index.html) installed on your system or, if you are a [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/wiki/Termux:API) package.
 
 To activate speech synthesis, use the `--talk-to-me` flag or its shorthand `-ttm` when running your commands. For example:
 ```bash
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
   _[_L_i_c_e_n_s_e_][Python version]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
-   [coverage]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
-                 _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
-     _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
+         _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
+  _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
+                        _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
 ```python >>> import pytgpt.phind as phind >>> bot = phind.PHIND() >>> bot.chat
 ('hello there') 'Hello! How can I assist you today?' ``` ```python from
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
@@ -129,35 +129,35 @@
 comprehensive utilization of the `--with-copied` option and support for
 accepting piped inputs. This improvement introduces placeholders, offering
 dynamic values for more versatile interactions. | Placeholder | Represents | |
 ------------ | ----------- | | `{{stream}}` | The piped input | | `{{copied}}`
 | The last copied text | This feature is particularly beneficial for intricate
 operations. For example: ```bash $ git diff | pytgpt generate "Here is a diff
 file: {{stream}} Make a concise commit message from it, aligning with my commit
-message history: {{copied}}" --shell --new ``` > In this illustration, `{
-{stream}}` denotes the result of the `$ git diff` operation, while `{{copied}}`
-signifies the content copied from the output of the `$ git log` command. ###
-Awesome Prompts [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/
-assets/all-acts.pdf?raw=True) are designed to guide the AI's behavior or
-responses in a particular direction, encouraging it to exhibit certain
-characteristics or behaviors. The term "awesome-prompt" is not a formal term in
-AI or machine learning literature, but it encapsulates the idea of crafting
-prompts that are effective in achieving desired outcomes. Let's say you want it
-to behave like a *Linux Terminal*, *PHP Interpreter*, or just to [**JAIL
-BREAK.**](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
-Instances : ```sh $ pytgpt interactve --awesome-prompt "Linux Terminal" # Act
-like a Linux Terminal $ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] >
-Awesome prompts are alternative to `--intro`. > Run `$ pytgpt awesome whole` to
-list available prompts (*200+*). > Run `$ pytgpt awesome --help` for more info.
-### Introducing RawDog RawDog is a masterpiece feature that exploits the
-versatile capabilities of Python to command and control your system as per your
-needs. You can literally do anything with it, since it generates and executes
-python codes, driven by **your prompts**! To have a bite of *rawdog* simply
-append the flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode.
-This introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
+message history: {{copied}}" --new ``` > In this illustration, `{{stream}}`
+denotes the result of the `$ git diff` operation, while `{{copied}}` signifies
+the content copied from the output of the `$ git log` command. ### Awesome
+Prompts [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/
+all-acts.pdf?raw=True) are designed to guide the AI's behavior or responses in
+a particular direction, encouraging it to exhibit certain characteristics or
+behaviors. The term "awesome-prompt" is not a formal term in AI or machine
+learning literature, but it encapsulates the idea of crafting prompts that are
+effective in achieving desired outcomes. Let's say you want it to behave like a
+*Linux Terminal*, *PHP Interpreter*, or just to [**JAIL BREAK.**](https://
+gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516) Instances : ```sh $
+pytgpt interactve --awesome-prompt "Linux Terminal" # Act like a Linux Terminal
+$ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] > Awesome prompts are
+alternative to `--intro`. > Run `$ pytgpt awesome whole` to list available
+prompts (*200+*). > Run `$ pytgpt awesome --help` for more info. ###
+Introducing RawDog RawDog is a masterpiece feature that exploits the versatile
+capabilities of Python to command and control your system as per your needs.
+You can literally do anything with it, since it generates and executes python
+codes, driven by **your prompts**! To have a bite of *rawdog* simply append the
+flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode. This
+introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
 [AbanteAI/rawdog](https://github.com/AbanteAI/rawdog) for the idea. This can be
 useful in some ways. For instance : ```sh $ pytgpt generate -n -q "Visualize
 the disk usage using pie chart" --rawdog ``` This will pop up a window showing
 system disk usage as shown below.
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/Figure_1.png?raw=true]
 ## Passing Environment Variables Pytgpt **v0.4.6** introduces a convention way
 of taking variables from the environment. To achieve that, set the environment
@@ -181,15 +181,15 @@
 API. Access docs and redoc at */docs* and */redoc* respectively. To launch the
 web interface for g4f-based providers, execute the following command in your
 terminal: ```bash $ pytgpt gpt4free gui ``` This command initializes the Web-
 user interface for interacting with g4f-based providers. To start the REST-API:
 ```bash $ pytgpt api run ``` This command starts the RESTful API server,
 enabling you to interact with the service programmatically. For accessing the
 documentation and redoc, navigate to the following paths in your web browser: -
-Documentation: `*/docs` - ReDoc: `*/redoc` ## Speech Synthesis To enable speech
+Documentation: `/docs` - ReDoc: `/redoc` ## Speech Synthesis To enable speech
 synthesis of responses, ensure you have either the [VLC player](https://
 www.videolan.org/vlc/index.html) installed on your system or, if you are a
 [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/
 wiki/Termux:API) package. To activate speech synthesis, use the `--talk-to-me`
 flag or its shorthand `-ttm` when running your commands. For example: ```bash $
 pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
 interactive -ttm ``` This flag instructs the system to audiolize the ai
```

### Comparing `python_tgpt-0.7.1/setup.py` & `python_tgpt-0.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,50 +9,55 @@
     "requests[socks]==2.31.0",
     "appdirs==1.4.4",
     "pyyaml==6.0.1",
     "webchatgpt==0.3.0",
     "GoogleBard1>=2.1.4",
     "poe-api-wrapper==1.3.6",
     "brotli==1.1.0",
-    "g4f>=0.3.0.8",
+    "g4f>=0.2.6.1",
     "Helpingai_T2-fork==0.3.2",
     "python-vlc>=3.0.20",
     "httpx==0.27.0",
 ]
 
 cli_reqs = [
     "click==8.1.3",
     "rich==13.3.4",
     "clipman==3.1.0",
     "pyperclip==1.8.2",
     "colorama==0.4.6",
-    "g4f>=0.3.0.8",
+    "g4f>=0.2.6.1",
     "python-dotenv==1.0.0",
 ]
 
 api = [
     "fastapi[all]==0.110.1",
 ]
 
+termux = [
+    "g4f==0.2.6.1",
+]
+
 EXTRA_REQUIRE = {
+    "termux": termux,
     "cli": cli_reqs,
     "api": api,
     "all": ["g4f[all]>=0.2.6.1", "matplotlib", "gpt4all==2.2.0"] + cli_reqs + api,
 }
 
 DOCS_PATH = Path(__file__).parents[0] / "docs/README.md"
 PATH = Path("README.md")
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="python-tgpt",
-    version="0.7.1",
+    version="0.7.2",
     license="MIT",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Interact with AI without API key",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `python_tgpt-0.7.1/src/pytgpt/__init__.py` & `python_tgpt-0.7.2/src/pytgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/api/__init__.py` & `python_tgpt-0.7.2/src/pytgpt/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     title="python-tgpt",
     summary="Interact with AI without API key",
     description=(
         "For **text** generation, **text-to-image** and **text-to-audio** conversions."
         "\n\n"
         "Access redoc at [/redoc](/redoc) endpoint."
         "\n\n"
-        "Full documentation is available at official repo : [Simatwa/python-tgpt](https://github.com/Simatwa/python-tgpt)."
+        "Other documentation is available at official repo : [Simatwa/python-tgpt](https://github.com/Simatwa/python-tgpt)."
     ),
     version=__version__,
     contact={
         "name": "Smartwa",
         "email": "simatwacaleb@proton.me",
         "url": "https://simatwa.vercel.app",
     },
```

### Comparing `python_tgpt-0.7.1/src/pytgpt/api/utils.py` & `python_tgpt-0.7.2/src/pytgpt/api/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/api/v1.py` & `python_tgpt-0.7.2/src/pytgpt/api/v1.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/async_providers.py` & `python_tgpt-0.7.2/src/pytgpt/async_providers.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/auto/main.py` & `python_tgpt-0.7.2/src/pytgpt/auto/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/base.py` & `python_tgpt-0.7.2/src/pytgpt/base.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/blackboxai/main.py` & `python_tgpt-0.7.2/src/pytgpt/blackboxai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/console.py` & `python_tgpt-0.7.2/src/pytgpt/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -1024,15 +1024,15 @@
             "\nLLM :",
             "\n\n**LLM** :",
             re.sub("\nUser :", "\n\n**User** :", history),
         )
         self.output_bond("Chat History", formatted_history, self.color)
         if click.confirm("Do you wish to save this chat"):
             save_to = click.prompt(
-                "Enter path/file-name", default="llama-conversation.txt"
+                "Enter path/file-name", default=f"{self.provider}-chat.txt"
             )
             with open(save_to, "a") as fh:
                 fh.write(history)
             click.secho(f"Conversation saved successfully to '{save_to}'", fg="cyan")
 
     @busy_bar.run("while resetting conversation")
     def do_reset(self, line):
```

### Comparing `python_tgpt-0.7.1/src/pytgpt/gemini/main.py` & `python_tgpt-0.7.2/src/pytgpt/gemini/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/gpt4all/main.py` & `python_tgpt-0.7.2/src/pytgpt/gpt4all/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/gpt4free/main.py` & `python_tgpt-0.7.2/src/pytgpt/gpt4free/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/gpt4free/utils.py` & `python_tgpt-0.7.2/src/pytgpt/gpt4free/utils.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/groq/main.py` & `python_tgpt-0.7.2/src/pytgpt/groq/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/imager/imager.py` & `python_tgpt-0.7.2/src/pytgpt/imager/imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/koboldai/main.py` & `python_tgpt-0.7.2/src/pytgpt/koboldai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/leo/main.py` & `python_tgpt-0.7.2/src/pytgpt/leo/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/llama2/main.py` & `python_tgpt-0.7.2/src/pytgpt/llama2/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/openai/main.py` & `python_tgpt-0.7.2/src/pytgpt/openai/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/opengpt/main.py` & `python_tgpt-0.7.2/src/pytgpt/opengpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/perplexity/main.py` & `python_tgpt-0.7.2/src/pytgpt/perplexity/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/phind/main.py` & `python_tgpt-0.7.2/src/pytgpt/phind/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/poe/main.py` & `python_tgpt-0.7.2/src/pytgpt/poe/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/utils.py` & `python_tgpt-0.7.2/src/pytgpt/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pathlib import Path
 from typing import Union
 from typing import NoReturn
 import requests
 import vlc
 import httpx
 import asyncio
+import urllib.parse
 from time import sleep as wait
 
 appdir = appdirs.AppDirs("pytgpt", "Smartwa")
 
 default_path = appdir.user_cache_dir
 
 api_static_dir = Path(default_path) / "api"
@@ -302,15 +303,14 @@
     def update_prompts_from_online(self, override: bool = False):
         """Download awesome-prompts and update existing ones if available
         args:
            override (bool, optional): Overwrite existing contents in path
         """
         resp = {}
         if not self.__is_prompt_updated:
-            import requests
 
             logging.info("Downloading & updating awesome prompts")
             response = requests.get(self.awesome_prompt_url)
             response.raise_for_status
             resp.update(response.json())
             if os.path.isfile(self.awesome_prompt_path) and not override:
                 resp.update(self.get_acts())
@@ -434,16 +434,14 @@
         Args:
             whole (bool, optional): Return whole json response. Defaults to False.
             version (bool, optional): return version only. Defaults to False.
 
         Returns:
             bool|dict: version str or whole dict info
         """
-        import requests
-
         data = requests.get(self.url).json()
         if whole:
             return data
 
         elif version:
             return data.get("tag_name")
 
@@ -943,15 +941,15 @@
             voice in cls.all_voices
         ), f"Voice '{voice}' not one of [{', '.join(cls.all_voices)}]"
         # Base URL for provider API
         session = httpx.AsyncClient(
             headers=cls.headers, proxies=proxies, timeout=timeout
         )
         url: str = (
-            f"https://api.streamelements.com/kappa/v2/speech?voice={voice}&text={{{message}}}"
+            f"https://api.streamelements.com/kappa/v2/speech?voice={voice}&text={{{urllib.parse.quote(message)}}}"
         )
         resp = await session.get(url)
         if not resp.is_success:
             raise Exception(
                 f"Failed to perform the operation - ({resp.status_code}, {resp.reason_phrase}) - {resp.text}"
             )
 
@@ -1047,25 +1045,26 @@
             player.play()
             # Keep the script running until the audio finishes playing
             while player.get_state() != vlc.State.Ended:
                 pass
 
         def play_using_termux_media_player():
             # check if media-player is installed
+            help_message: str = (
+                "Install termux-api package in order to play audio files.\n apt update && apt install termux-api"
+            )
             check = run_system_command(
                 "termux-media-player --help",
                 exit_on_error=False,
                 stdout_error=False,
-                help="Install termux-api package in order to play audio files.\n apt update && apt install termux-api",
+                help=help_message,
             )[1]
 
             if check.returncode == 127:
-                raise Exception(
-                    "Install termux-api package in order to play audio files.\n apt update && apt install termux-api"
-                )
+                raise Exception(help_message)
             try:
                 run_system_command(f'termux-media-player play "{path_to_audio_file}"')
                 while (
                     run_system_command("termux-media-player info")[1].stdout.strip()
                     != "No track currently!"
                 ):
                     wait(1)
```

### Comparing `python_tgpt-0.7.1/src/pytgpt/webchatgpt/main.py` & `python_tgpt-0.7.2/src/pytgpt/webchatgpt/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/pytgpt/yepchat/main.py` & `python_tgpt-0.7.2/src/pytgpt/yepchat/main.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/python_tgpt.egg-info/PKG-INFO` & `python_tgpt-0.7.2/src/python_tgpt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-tgpt
-Version: 0.7.1
+Version: 0.7.2
 Summary: Interact with AI without API key
 Home-page: https://github.com/Simatwa/python-tgpt
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
@@ -34,38 +34,40 @@
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: webchatgpt==0.3.0
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: poe-api-wrapper==1.3.6
 Requires-Dist: brotli==1.1.0
-Requires-Dist: g4f>=0.3.0.8
+Requires-Dist: g4f>=0.2.6.1
 Requires-Dist: Helpingai_T2-fork==0.3.2
 Requires-Dist: python-vlc>=3.0.20
 Requires-Dist: httpx==0.27.0
+Provides-Extra: termux
+Requires-Dist: g4f==0.2.6.1; extra == "termux"
 Provides-Extra: cli
 Requires-Dist: click==8.1.3; extra == "cli"
 Requires-Dist: rich==13.3.4; extra == "cli"
 Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: g4f>=0.3.0.8; extra == "cli"
+Requires-Dist: g4f>=0.2.6.1; extra == "cli"
 Requires-Dist: python-dotenv==1.0.0; extra == "cli"
 Provides-Extra: api
 Requires-Dist: fastapi[all]==0.110.1; extra == "api"
 Provides-Extra: all
 Requires-Dist: g4f[all]>=0.2.6.1; extra == "all"
 Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: gpt4all==2.2.0; extra == "all"
 Requires-Dist: click==8.1.3; extra == "all"
 Requires-Dist: rich==13.3.4; extra == "all"
 Requires-Dist: clipman==3.1.0; extra == "all"
 Requires-Dist: pyperclip==1.8.2; extra == "all"
 Requires-Dist: colorama==0.4.6; extra == "all"
-Requires-Dist: g4f>=0.3.0.8; extra == "all"
+Requires-Dist: g4f>=0.2.6.1; extra == "all"
 Requires-Dist: python-dotenv==1.0.0; extra == "all"
 Requires-Dist: fastapi[all]==0.110.1; extra == "all"
 
 <p align="center">
 <img src="https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true" width='40%'>
 </p>
 
@@ -76,16 +78,14 @@
 -->
 <a href="https://github.com/Simatwa/python-tgpt/blob/main/LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
 <a href=""><img alt="Python version" src="https://img.shields.io/pypi/pyversions/python-tgpt"/></a>
 <a href="https://pypi.org/project/python-tgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/python-tgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"/></a>
 <a href="https://python-tgpt.onrender.com"><img alt="Website status" src="https://img.shields.io/website?url=https://python-tgpt.onrender.com"/></a>
 <a href="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml"><img alt="Python Package flow" src="https://github.com/Simatwa/python-tgpt/actions/workflows/python-package.yml/badge.svg?branch=master"/></a>
-<a href=""><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
-<a href="https://pepy.tech/project/tgpt2"><img src="https://static.pepy.tech/personalized-badge/tgpt2?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <a href="https://pepy.tech/project/python-tgpt"><img src="https://static.pepy.tech/personalized-badge/python-tgpt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads" alt="Downloads"></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases/latest"><img src="https://img.shields.io/github/downloads/Simatwa/python-tgpt/total?label=Asset%20Downloads&color=success" alt="Downloads"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/v/release/Simatwa/python-tgpt?color=success&label=Release&logo=github" alt="Latest release"></img></a>
 <a href="https://github.com/Simatwa/python-tgpt/releases"><img src="https://img.shields.io/github/release-date/Simatwa/python-tgpt?label=Release date&logo=github" alt="release date"></img></a>
 <a href="https://hits.seeyoufarm.com"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com/Simatwa/python-tgpt"/></a>      
 <a href="https://wakatime.com/badge/github/Simatwa/tgpt2"><img src="https://wakatime.com/badge/github/Simatwa/tgpt2.svg" alt="wakatime"></a>
 </p>
@@ -545,15 +545,15 @@
 | ------------ | ----------- |
 | `{{stream}}` | The piped input |
 | `{{copied}}` | The last copied text |
 
 This feature is particularly beneficial for intricate operations. For example:
 
 ```bash
-$ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a concise commit message from it, aligning with my commit message history: {{copied}}" --shell --new
+$ git diff | pytgpt generate "Here is a diff file: {{stream}} Make a concise commit message from it, aligning with my commit message history: {{copied}}" --new
 ```
 > In this illustration, `{{stream}}` denotes the result of the `$ git diff` operation, while `{{copied}}` signifies the content copied from the output of the `$ git log` command.
 
 ### Awesome Prompts
 
 [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/all-acts.pdf?raw=True) are designed to guide the AI's behavior or responses in a particular direction, encouraging it to exhibit certain characteristics or behaviors. The  term "awesome-prompt" is not a formal term in AI or machine learning literature, but it encapsulates the idea of crafting prompts that are effective in achieving desired outcomes. Let's say you want it to behave like a *Linux Terminal*, *PHP Interpreter*, or just to [**JAIL BREAK.**](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
 
@@ -624,16 +624,16 @@
 ```bash
 $ pytgpt api run
 ```
 
 This command starts the RESTful API server, enabling you to interact with the service programmatically.
 
 For accessing the documentation and redoc, navigate to the following paths in your web browser:
-- Documentation: `*/docs`
-- ReDoc: `*/redoc`
+- Documentation: `/docs`
+- ReDoc: `/redoc`
 
 ## Speech Synthesis
 
 To enable speech synthesis of responses, ensure you have either the [VLC player](https://www.videolan.org/vlc/index.html) installed on your system or, if you are a [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/wiki/Termux:API) package.
 
 To activate speech synthesis, use the `--talk-to-me` flag or its shorthand `-ttm` when running your commands. For example:
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.1 Summary: Interact with
+Metadata-Version: 2.1 Name: python-tgpt Version: 0.7.2 Summary: Interact with
 AI without API key Home-page: https://github.com/Simatwa/python-tgpt Author:
 Smartwa Author-email: simatwacaleb@proton.me Maintainer: Smartwa License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/python-tgpt/issues/new
 Project-URL: Homepage, https://github.com/Simatwa/python-tgpt Project-URL:
 Source Code, https://github.com/Simatwa/python-tgpt Project-URL: Issue Tracker,
 https://github.com/Simatwa/python-tgpt/issues Project-URL: Download, https://
 github.com/Simatwa/python-tgpt/releases Project-URL: Documentation, https://
@@ -19,34 +19,35 @@
 Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests[socks]==2.31.0 Requires-Dist: appdirs==1.4.4
 Requires-Dist: pyyaml==6.0.1 Requires-Dist: webchatgpt==0.3.0 Requires-Dist:
 GoogleBard1>=2.1.4 Requires-Dist: poe-api-wrapper==1.3.6 Requires-Dist:
-brotli==1.1.0 Requires-Dist: g4f>=0.3.0.8 Requires-Dist: Helpingai_T2-
+brotli==1.1.0 Requires-Dist: g4f>=0.2.6.1 Requires-Dist: Helpingai_T2-
 fork==0.3.2 Requires-Dist: python-vlc>=3.0.20 Requires-Dist: httpx==0.27.0
-Provides-Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
+Provides-Extra: termux Requires-Dist: g4f==0.2.6.1; extra == "termux" Provides-
+Extra: cli Requires-Dist: click==8.1.3; extra == "cli" Requires-Dist:
 rich==13.3.4; extra == "cli" Requires-Dist: clipman==3.1.0; extra == "cli"
 Requires-Dist: pyperclip==1.8.2; extra == "cli" Requires-Dist: colorama==0.4.6;
-extra == "cli" Requires-Dist: g4f>=0.3.0.8; extra == "cli" Requires-Dist:
+extra == "cli" Requires-Dist: g4f>=0.2.6.1; extra == "cli" Requires-Dist:
 python-dotenv==1.0.0; extra == "cli" Provides-Extra: api Requires-Dist: fastapi
 [all]==0.110.1; extra == "api" Provides-Extra: all Requires-Dist: g4f
 [all]>=0.2.6.1; extra == "all" Requires-Dist: matplotlib; extra == "all"
 Requires-Dist: gpt4all==2.2.0; extra == "all" Requires-Dist: click==8.1.3;
 extra == "all" Requires-Dist: rich==13.3.4; extra == "all" Requires-Dist:
 clipman==3.1.0; extra == "all" Requires-Dist: pyperclip==1.8.2; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.3.0.8;
+Requires-Dist: colorama==0.4.6; extra == "all" Requires-Dist: g4f>=0.2.6.1;
 extra == "all" Requires-Dist: python-dotenv==1.0.0; extra == "all" Requires-
 Dist: fastapi[all]==0.110.1; extra == "all"
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/py-tgpt.png?raw=true]
   _[_L_i_c_e_n_s_e_][Python version]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_W_e_b_s_i_t_e_ _s_t_a_t_u_s_]_[_P_y_t_h_o_n_ _P_a_c_k_a_g_e_ _f_l_o_w_]
-   [coverage]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]
-                 _[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
-     _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
+         _[_D_o_w_n_l_o_a_d_s_]_[_D_o_w_n_l_o_a_d_s_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/
+  _h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/_b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/
+                        _S_i_m_a_t_w_a_/_p_y_t_h_o_n_-_t_g_p_t_]_[_w_a_k_a_t_i_m_e_]
                              ******** ppyytthhoonn--ttggpptt ********
  [https://github.com/Simatwa/python-tgpt/blob/main/assets/demo-1.gif?raw=True]
 ```python >>> import pytgpt.phind as phind >>> bot = phind.PHIND() >>> bot.chat
 ('hello there') 'Hello! How can I assist you today?' ``` ```python from
 pytgpt.imager import Imager img = Imager() generated_images = img.generate
 (prompt="Cyberpunk", amount=3, stream=True) img.save(generated_images) ``` This
 project enables seamless interaction with over **45 free LLM providers**
@@ -169,35 +170,35 @@
 comprehensive utilization of the `--with-copied` option and support for
 accepting piped inputs. This improvement introduces placeholders, offering
 dynamic values for more versatile interactions. | Placeholder | Represents | |
 ------------ | ----------- | | `{{stream}}` | The piped input | | `{{copied}}`
 | The last copied text | This feature is particularly beneficial for intricate
 operations. For example: ```bash $ git diff | pytgpt generate "Here is a diff
 file: {{stream}} Make a concise commit message from it, aligning with my commit
-message history: {{copied}}" --shell --new ``` > In this illustration, `{
-{stream}}` denotes the result of the `$ git diff` operation, while `{{copied}}`
-signifies the content copied from the output of the `$ git log` command. ###
-Awesome Prompts [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/
-assets/all-acts.pdf?raw=True) are designed to guide the AI's behavior or
-responses in a particular direction, encouraging it to exhibit certain
-characteristics or behaviors. The term "awesome-prompt" is not a formal term in
-AI or machine learning literature, but it encapsulates the idea of crafting
-prompts that are effective in achieving desired outcomes. Let's say you want it
-to behave like a *Linux Terminal*, *PHP Interpreter*, or just to [**JAIL
-BREAK.**](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
-Instances : ```sh $ pytgpt interactve --awesome-prompt "Linux Terminal" # Act
-like a Linux Terminal $ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] >
-Awesome prompts are alternative to `--intro`. > Run `$ pytgpt awesome whole` to
-list available prompts (*200+*). > Run `$ pytgpt awesome --help` for more info.
-### Introducing RawDog RawDog is a masterpiece feature that exploits the
-versatile capabilities of Python to command and control your system as per your
-needs. You can literally do anything with it, since it generates and executes
-python codes, driven by **your prompts**! To have a bite of *rawdog* simply
-append the flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode.
-This introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
+message history: {{copied}}" --new ``` > In this illustration, `{{stream}}`
+denotes the result of the `$ git diff` operation, while `{{copied}}` signifies
+the content copied from the output of the `$ git log` command. ### Awesome
+Prompts [These prompts](https://github.com/Simatwa/gpt-cli/blob/main/assets/
+all-acts.pdf?raw=True) are designed to guide the AI's behavior or responses in
+a particular direction, encouraging it to exhibit certain characteristics or
+behaviors. The term "awesome-prompt" is not a formal term in AI or machine
+learning literature, but it encapsulates the idea of crafting prompts that are
+effective in achieving desired outcomes. Let's say you want it to behave like a
+*Linux Terminal*, *PHP Interpreter*, or just to [**JAIL BREAK.**](https://
+gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516) Instances : ```sh $
+pytgpt interactve --awesome-prompt "Linux Terminal" # Act like a Linux Terminal
+$ pytgpt interactive -ap DAN # Jailbreak ``` > [!NOTE] > Awesome prompts are
+alternative to `--intro`. > Run `$ pytgpt awesome whole` to list available
+prompts (*200+*). > Run `$ pytgpt awesome --help` for more info. ###
+Introducing RawDog RawDog is a masterpiece feature that exploits the versatile
+capabilities of Python to command and control your system as per your needs.
+You can literally do anything with it, since it generates and executes python
+codes, driven by **your prompts**! To have a bite of *rawdog* simply append the
+flag `--rawdog` *shortform* `-rd` in *generate/interactive* mode. This
+introduces a never seen-before feature in the *tgpt ecosystem*. Thanks to
 [AbanteAI/rawdog](https://github.com/AbanteAI/rawdog) for the idea. This can be
 useful in some ways. For instance : ```sh $ pytgpt generate -n -q "Visualize
 the disk usage using pie chart" --rawdog ``` This will pop up a window showing
 system disk usage as shown below.
 [https://github.com/Simatwa/python-tgpt/blob/main/assets/Figure_1.png?raw=true]
 ## Passing Environment Variables Pytgpt **v0.4.6** introduces a convention way
 of taking variables from the environment. To achieve that, set the environment
@@ -221,15 +222,15 @@
 API. Access docs and redoc at */docs* and */redoc* respectively. To launch the
 web interface for g4f-based providers, execute the following command in your
 terminal: ```bash $ pytgpt gpt4free gui ``` This command initializes the Web-
 user interface for interacting with g4f-based providers. To start the REST-API:
 ```bash $ pytgpt api run ``` This command starts the RESTful API server,
 enabling you to interact with the service programmatically. For accessing the
 documentation and redoc, navigate to the following paths in your web browser: -
-Documentation: `*/docs` - ReDoc: `*/redoc` ## Speech Synthesis To enable speech
+Documentation: `/docs` - ReDoc: `/redoc` ## Speech Synthesis To enable speech
 synthesis of responses, ensure you have either the [VLC player](https://
 www.videolan.org/vlc/index.html) installed on your system or, if you are a
 [Termux](https://termux.org) user, the [Termux:API](https://wiki.termux.com/
 wiki/Termux:API) package. To activate speech synthesis, use the `--talk-to-me`
 flag or its shorthand `-ttm` when running your commands. For example: ```bash $
 pytgpt generate "Generate an ogre story" --talk-to-me ``` or ```bash $ pytgpt
 interactive -ttm ``` This flag instructs the system to audiolize the ai
```

### Comparing `python_tgpt-0.7.1/src/python_tgpt.egg-info/SOURCES.txt` & `python_tgpt-0.7.2/src/python_tgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/src/python_tgpt.egg-info/requires.txt` & `python_tgpt-0.7.2/src/python_tgpt.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 requests[socks]==2.31.0
 appdirs==1.4.4
 pyyaml==6.0.1
 webchatgpt==0.3.0
 GoogleBard1>=2.1.4
 poe-api-wrapper==1.3.6
 brotli==1.1.0
-g4f>=0.3.0.8
+g4f>=0.2.6.1
 Helpingai_T2-fork==0.3.2
 python-vlc>=3.0.20
 httpx==0.27.0
 
 [all]
 g4f[all]>=0.2.6.1
 matplotlib
 gpt4all==2.2.0
 click==8.1.3
 rich==13.3.4
 clipman==3.1.0
 pyperclip==1.8.2
 colorama==0.4.6
-g4f>=0.3.0.8
+g4f>=0.2.6.1
 python-dotenv==1.0.0
 fastapi[all]==0.110.1
 
 [api]
 fastapi[all]==0.110.1
 
 [cli]
 click==8.1.3
 rich==13.3.4
 clipman==3.1.0
 pyperclip==1.8.2
 colorama==0.4.6
-g4f>=0.3.0.8
+g4f>=0.2.6.1
 python-dotenv==1.0.0
+
+[termux]
+g4f==0.2.6.1
```

### Comparing `python_tgpt-0.7.1/tests/test_api.py` & `python_tgpt-0.7.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/tests/test_imager.py` & `python_tgpt-0.7.2/tests/test_imager.py`

 * *Files identical despite different names*

### Comparing `python_tgpt-0.7.1/tests/test_utils.py` & `python_tgpt-0.7.2/tests/test_utils.py`

 * *Files identical despite different names*


# Comparing `tmp/ai4free-0.1.tar.gz` & `tmp/ai4free-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai4free-0.1.tar", last modified: Thu May  9 11:01:56 2024, max compression
+gzip compressed data, was "ai4free-0.2.tar", last modified: Thu May  9 14:51:51 2024, max compression
```

## Comparing `ai4free-0.1.tar` & `ai4free-0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:56.933261 ai4free-0.1/
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 ai4free-0.1/LICENSE.md
--rw-rw-rw-   0        0        0    10610 2024-05-09 11:01:56.919260 ai4free-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     9321 2024-05-09 10:57:47.000000 ai4free-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:56.603974 ai4free-0.1/ai4free/
--rw-rw-rw-   0        0        0    16349 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/Blackbox.py
--rw-rw-rw-   0        0        0     8277 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/Cohere.py
--rw-rw-rw-   0        0        0    15388 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/KOBOLDAI.py
--rw-rw-rw-   0        0        0    18500 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/OpenGPT.py
--rw-rw-rw-   0        0        0    20211 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/Openai.py
--rw-rw-rw-   0        0        0    19512 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/Phind.py
--rw-rw-rw-   0        0        0      319 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/__init__.py
--rw-rw-rw-   0        0        0    20824 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/groq.py
--rw-rw-rw-   0        0        0    20051 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/leo.py
--rw-rw-rw-   0        0        0     8482 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/reka.py
--rw-rw-rw-   0        0        0    19935 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/yep.py
--rw-rw-rw-   0        0        0     7580 2024-05-09 10:57:47.000000 ai4free-0.1/ai4free/you.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:01:56.904260 ai4free-0.1/ai4free.egg-info/
--rw-rw-rw-   0        0        0    10610 2024-05-09 11:01:54.000000 ai4free-0.1/ai4free.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-05-09 11:01:55.000000 ai4free-0.1/ai4free.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:01:54.000000 ai4free-0.1/ai4free.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-09 11:01:54.000000 ai4free-0.1/ai4free.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-09 11:01:54.000000 ai4free-0.1/ai4free.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 11:01:56.935270 ai4free-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1507 2024-05-09 11:00:27.000000 ai4free-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:51:51.314757 ai4free-0.2/
+-rw-rw-rw-   0        0        0     3186 2024-05-09 14:51:32.000000 ai4free-0.2/LICENSE.md
+-rw-rw-rw-   0        0        0    10616 2024-05-09 14:51:51.299626 ai4free-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9321 2024-05-09 10:57:47.000000 ai4free-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 14:51:51.199133 ai4free-0.2/ai4free/
+-rw-rw-rw-   0        0        0    16349 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/Blackbox.py
+-rw-rw-rw-   0        0        0     8277 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/Cohere.py
+-rw-rw-rw-   0        0        0    15388 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/KOBOLDAI.py
+-rw-rw-rw-   0        0        0    18500 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/OpenGPT.py
+-rw-rw-rw-   0        0        0    20211 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/Openai.py
+-rw-rw-rw-   0        0        0    19512 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/Phind.py
+-rw-rw-rw-   0        0        0      319 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/__init__.py
+-rw-rw-rw-   0        0        0    20824 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/groq.py
+-rw-rw-rw-   0        0        0    20051 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/leo.py
+-rw-rw-rw-   0        0        0     8482 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/reka.py
+-rw-rw-rw-   0        0        0    19935 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/yep.py
+-rw-rw-rw-   0        0        0     7580 2024-05-09 10:57:47.000000 ai4free-0.2/ai4free/you.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:51:51.286064 ai4free-0.2/ai4free.egg-info/
+-rw-rw-rw-   0        0        0    10616 2024-05-09 14:51:49.000000 ai4free-0.2/ai4free.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2024-05-09 14:51:50.000000 ai4free-0.2/ai4free.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 14:51:49.000000 ai4free-0.2/ai4free.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-09 14:51:49.000000 ai4free-0.2/ai4free.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-09 14:51:49.000000 ai4free-0.2/ai4free.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 14:51:51.314757 ai4free-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1557 2024-05-09 14:50:35.000000 ai4free-0.2/setup.py
```

### Comparing `ai4free-0.1/LICENSE.md` & `ai4free-0.2/LICENSE.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 ****************************************
-**** HelpingAI Simplified Universal License ****
+# Ai4Free Simplified Universal License 
 ****************************************
 
 Version 1.0
 
 ### Introduction
 
-This HelpingAI Simplified Universal License (HSUL) governs HelpingAI's content, including computer programs, scripts, datasets, documents, images, audio recordings, videos, and other digital assets. The HSUL provides simple, universal terms for accessing, modifying, and sharing resources while embracing ethical development practices.
+This Ai4Free Simplified Universal License (HSUL) governs Ai4Free's content, including computer programs, scripts, datasets, documents, images, audio recordings, videos, and other digital assets. The HSUL provides simple, universal terms for accessing, modifying, and sharing resources while embracing ethical development practices.
 
 ### Grant of Rights
 
-Under the HSUL, HelpingAI authorizes you to copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Content, subject to the terms and conditions detailed in this document.
+Under the HSUL, Ai4Free authorizes you to copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Content, subject to the terms and conditions detailed in this document.
 
 ### Conditions
 
 To qualify for the rights granted in section 1, you must strictly adhere to the following conditions:
 
 2.1. **Redistributions of Source Code.**
    If you redistribute the Source Code, you must include the entire HSUL with your distribution. Furthermore, you must add prominent notifications in all affected files stating:
 
-   > "This Work is released under the HelpingAI Simplified Universal License v1.0."
+   > "This Work is released under the Ai4Free Simplified Universal License v1.0."
 
 2.2. **Binary Form Redistributions.**
    If you distribute Binaries generated from the Source Code, you must ensure the inclusion of the following statement in your distribution:
 
-   > "This Work is based upon the HelpingAI Simplified Universally Licensed Work, under the HelpingAI Simplified Universal License v1.0."
+   > "This Work is based upon the Ai4Free Simplified Universally Licensed Work, under the Ai4Free Simplified Universal License v1.0."
 
 2.3. **Notification of Changes.**
    Clearly indicate any alterations you introduce to the Source Code or Documentation via prominent comments detailing the nature and scope of the change(s). Reference the date and originator of the modifications.
 
 2.4. **Branding Attribution.**
-   Do not remove or alter any HelpingAI branding, logos, or notices included in the Content without explicit prior consent from HelpingAI.
+   Do not remove or alter any Ai4Free branding, logos, or notices included in the Content without explicit prior consent from Ai4Free.
 
 2.5. **Exclusion of Warranty.**
    The Content is delivered "AS IS," bereft of any implicit guarantee, including — though not constrained to — warranties pertaining to marketability, applicability for a particular purpose, and non-infringement.
 
 2.6. **Limitation of Liability.**
-   To the maximum extent allowed by law, neither HelpingAI nor any contributor shall bear responsibility for any loss, personal injury, property damage, indirect, special, incidental, or consequential damages stemming from or relating to the Content or its employment.
+   To the maximum extent allowed by law, neither Ai4Free nor any contributor shall bear responsibility for any loss, personal injury, property damage, indirect, special, incidental, or consequential damages stemming from or relating to the Content or its employment.
 
 2.7. **Governing Law.**
-   This HSUL shall be managed and construed according to the laws of the jurisdiction where HelpingAI primarily operates.
+   This HSUL shall be managed and construed according to the laws of the jurisdiction where Ai4Free primarily operates.
 
 ### Definitions
 
 3.1. **"Source Code"** signifies the preferred form for editing the Content, typically represented by human-readable programming languages, scripts, or documentation formats.
 
 3.2. **"Binaries"** denote compiled forms of the Source Code, executables, libraries, or similar artifacts built from the Source Code.
 
-By leveraging this Content, you confirm your approval of the HSUL and pledge to honor its terms and conditions. If you disagree with the HSUL's rules, refrain from engaging with the Content.
+By leveraging this Content, you confirm your approval of the HSUL and pledge to honor its terms and conditions. If you disagree with the HSUL's rules, refrain from engaging with the Content.
+
+Copyright (c) 2023 Devs Do Code (Sree). All rights reserved
```

### Comparing `ai4free-0.1/PKG-INFO` & `ai4free-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ai4free
-Version: 0.1
+Version: 0.2
 Summary: collection of free AI provides
 Author: OEvortex
 Author-email: helpingai5@gmail.com
+Maintainer: Sree
 License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
-Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: Source, https://github.com/Devs-Do-Code/ai4free
+Project-URL: Tracker, https://github.com/Devs-Do-Code/ai4free/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
+Project-URL: Youtube, https://www.youtube.com/@DevsDoCode
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: ai4free Version: 0.1 Summary: collection of free AI
-provides Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
-Simplified Universal License Project-URL: Documentation, https://github.com/OE-
-LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
-Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-tls_client Requires-Dist: webscout
+Metadata-Version: 2.1 Name: ai4free Version: 0.2 Summary: collection of free AI
+provides Author: OEvortex Author-email: helpingai5@gmail.com Maintainer: Sree
+License: HelpingAI Simplified Universal License Project-URL: Source, https://
+github.com/Devs-Do-Code/ai4free Project-URL: Tracker, https://github.com/Devs-
+Do-Code/ai4free/issues Project-URL: YouTube, https://youtube.com/@OEvortex
+Project-URL: Youtube, https://www.youtube.com/@DevsDoCode Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: License :: Other/Proprietary License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Topic :: Internet :: WWW/HTTP ::
+Indexing/Search Classifier: Topic :: Software Development :: Libraries ::
+Python Modules Description-Content-Type: text/markdown License-File: LICENSE.md
+Requires-Dist: tls_client Requires-Dist: webscout
                             [HuggingChat API Badge]
           ************ FFrreeee -- UUnnooffffiicciiaall RReevveerrssee EEnnggiinneeeerreedd AAPPII ?ð??? ************
                   _[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _f_o_r_k_s_]_[_G_i_t_H_u_b_ _i_s_s_u_e_s_]
            _[_Y_o_u_T_u_b_e_]_[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 # AI4Free: A Python Library for Free Access to All Available Large Language
 Models AI4Free is a Python library that provides convenient access to a variety
 of large language models (LLMs) from different providers, all without requiring
```

### Comparing `ai4free-0.1/README.md` & `ai4free-0.2/README.md`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/Blackbox.py` & `ai4free-0.2/ai4free/Blackbox.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/Cohere.py` & `ai4free-0.2/ai4free/Cohere.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/KOBOLDAI.py` & `ai4free-0.2/ai4free/KOBOLDAI.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/OpenGPT.py` & `ai4free-0.2/ai4free/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/Openai.py` & `ai4free-0.2/ai4free/Openai.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/Phind.py` & `ai4free-0.2/ai4free/Phind.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/groq.py` & `ai4free-0.2/ai4free/groq.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/leo.py` & `ai4free-0.2/ai4free/leo.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/reka.py` & `ai4free-0.2/ai4free/reka.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/yep.py` & `ai4free-0.2/ai4free/yep.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free/you.py` & `ai4free-0.2/ai4free/you.py`

 * *Files identical despite different names*

### Comparing `ai4free-0.1/ai4free.egg-info/PKG-INFO` & `ai4free-0.2/ai4free.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ai4free
-Version: 0.1
+Version: 0.2
 Summary: collection of free AI provides
 Author: OEvortex
 Author-email: helpingai5@gmail.com
+Maintainer: Sree
 License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
-Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: Source, https://github.com/Devs-Do-Code/ai4free
+Project-URL: Tracker, https://github.com/Devs-Do-Code/ai4free/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
+Project-URL: Youtube, https://www.youtube.com/@DevsDoCode
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: ai4free Version: 0.1 Summary: collection of free AI
-provides Author: OEvortex Author-email: helpingai5@gmail.com License: HelpingAI
-Simplified Universal License Project-URL: Documentation, https://github.com/OE-
-LUCIFER/Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/
-Webscout Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
-Project-URL: YouTube, https://youtube.com/@OEvortex Classifier: Development
-Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
-CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
-tls_client Requires-Dist: webscout
+Metadata-Version: 2.1 Name: ai4free Version: 0.2 Summary: collection of free AI
+provides Author: OEvortex Author-email: helpingai5@gmail.com Maintainer: Sree
+License: HelpingAI Simplified Universal License Project-URL: Source, https://
+github.com/Devs-Do-Code/ai4free Project-URL: Tracker, https://github.com/Devs-
+Do-Code/ai4free/issues Project-URL: YouTube, https://youtube.com/@OEvortex
+Project-URL: Youtube, https://www.youtube.com/@DevsDoCode Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: License :: Other/Proprietary License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Topic :: Internet :: WWW/HTTP ::
+Indexing/Search Classifier: Topic :: Software Development :: Libraries ::
+Python Modules Description-Content-Type: text/markdown License-File: LICENSE.md
+Requires-Dist: tls_client Requires-Dist: webscout
                             [HuggingChat API Badge]
           ************ FFrreeee -- UUnnooffffiicciiaall RReevveerrssee EEnnggiinneeeerreedd AAPPII ?ð??? ************
                   _[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _f_o_r_k_s_]_[_G_i_t_H_u_b_ _i_s_s_u_e_s_]
            _[_Y_o_u_T_u_b_e_]_[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 # AI4Free: A Python Library for Free Access to All Available Large Language
 Models AI4Free is a Python library that provides convenient access to a variety
 of large language models (LLMs) from different providers, all without requiring
```


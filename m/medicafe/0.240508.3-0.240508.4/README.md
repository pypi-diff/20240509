# Comparing `tmp/medicafe-0.240508.3.tar.gz` & `tmp/medicafe-0.240508.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240508.3.tar", last modified: Thu May  9 04:42:15 2024, max compression
+gzip compressed data, was "medicafe-0.240508.4.tar", last modified: Thu May  9 04:56:40 2024, max compression
```

## Comparing `medicafe-0.240508.3.tar` & `medicafe-0.240508.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 04:42:15.241000 medicafe-0.240508.3/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240508.3/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240508.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-09 04:42:14.694000 medicafe-0.240508.3/MediBot/
--rwxrwxrwx   0        0        0     3614 2024-05-09 04:40:39.000000 medicafe-0.240508.3/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    16642 2024-05-09 04:18:06.000000 medicafe-0.240508.3/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240508.3/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    32227 2024-05-09 04:18:08.000000 medicafe-0.240508.3/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240508.3/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0    10260 2024-05-09 04:16:32.000000 medicafe-0.240508.3/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6366 2024-05-09 04:18:11.000000 medicafe-0.240508.3/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240508.3/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240508.3/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240508.3/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240508.3/MediBot/update_json.py
--rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240508.3/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-09 04:42:15.082000 medicafe-0.240508.3/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240508.3/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240508.3/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240508.3/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240508.3/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240508.3/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240508.3/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240508.3/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240508.3/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240508.3/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240508.3/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240508.3/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240508.3/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240508.3/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240508.3/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240508.3/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240508.3/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-09 04:42:15.227000 medicafe-0.240508.3/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240508.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 04:42:15.213000 medicafe-0.240508.3/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240508.3/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 04:42:15.237000 medicafe-0.240508.3/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-09 04:42:13.000000 medicafe-0.240508.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 04:56:40.453000 medicafe-0.240508.4/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240508.4/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240508.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-09 04:56:39.900000 medicafe-0.240508.4/MediBot/
+-rwxrwxrwx   0        0        0     3614 2024-05-09 04:40:39.000000 medicafe-0.240508.4/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    16642 2024-05-09 04:47:15.000000 medicafe-0.240508.4/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240508.4/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    32227 2024-05-09 04:18:08.000000 medicafe-0.240508.4/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240508.4/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10660 2024-05-09 04:53:27.000000 medicafe-0.240508.4/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6801 2024-05-09 04:53:21.000000 medicafe-0.240508.4/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240508.4/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240508.4/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240508.4/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240508.4/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240508.4/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-09 04:56:40.287000 medicafe-0.240508.4/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240508.4/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240508.4/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240508.4/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240508.4/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240508.4/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240508.4/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240508.4/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240508.4/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240508.4/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240508.4/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240508.4/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240508.4/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240508.4/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240508.4/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240508.4/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240508.4/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-09 04:56:40.437000 medicafe-0.240508.4/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240508.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 04:56:40.422000 medicafe-0.240508.4/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240508.4/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-09 04:56:39.000000 medicafe-0.240508.4/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 04:56:40.449000 medicafe-0.240508.4/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-09 04:56:38.000000 medicafe-0.240508.4/setup.py
```

### Comparing `medicafe-0.240508.3/LICENSE` & `medicafe-0.240508.4/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediBot/MediBot.bat` & `medicafe-0.240508.4/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediBot/MediBot.py` & `medicafe-0.240508.4/MediBot/MediBot.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import subprocess
 import os
 import tempfile
 import traceback
 import re  #for addresses
 from collections import OrderedDict
-from MediBot_UI import app_control, manage_script_pause, user_interaction
 import MediBot_dataformat_library
 import MediBot_Preprocessor
 from MediBot_Preprocessor import initialize, AHK_EXECUTABLE, CSV_FILE_PATH, field_mapping
 import MediBot_Preprocessor_lib
+from MediBot_UI import app_control, manage_script_pause, user_interaction
 
 # Add parent directory of the project to the Python path
 import sys
 project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
 sys.path.append(project_dir)
 
 from MediLink import MediLink_ConfigLoader
```

### Comparing `medicafe-0.240508.3/MediBot/MediBot_Charges.py` & `medicafe-0.240508.4/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240508.4/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240508.4/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediBot/MediBot_UI.py` & `medicafe-0.240508.4/MediBot/MediBot_UI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 from sys import exit
 import ctypes
 from ctypes import wintypes
 import time
 import re
-from MediBot_Preprocessor import config
+
+# Add parent directory of the project to the Python path
+import os
+import sys
+project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
+sys.path.append(project_dir)
+
+try: 
+    from MediLink import MediLink_ConfigLoader
+    config, crosswalk = MediLink_ConfigLoader.load_configuration()
+except ImportError:
+    from MediLink_ConfigLoader import load_configuration
+    config, crosswalk = load_configuration()
 
 """
 User Interaction Refinements
 - [ ] Refine the menu options for clearer user guidance during script pauses and errors.
 - [ ] Add functionality for user to easily repeat or skip specific entries without script restart.
     Develop more intuitive skip and retry mechanisms that are responsive to user input during data entry sessions.
 """
```

### Comparing `medicafe-0.240508.3/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240508.4/MediBot/MediBot_dataformat_library.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 import re
 from datetime import datetime
 import re  #for addresses
-from MediBot_Preprocessor import config, initialize
+
+# Add parent directory of the project to the Python path
+import os
+import sys
+project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
+sys.path.append(project_dir)
+
+try: 
+    from MediLink import MediLink_ConfigLoader
+    config, crosswalk = MediLink_ConfigLoader.load_configuration()
+except ImportError:
+    from MediLink_ConfigLoader import load_configuration
+    config, crosswalk = load_configuration()
+
+from MediBot_Preprocessor import initialize
 from MediBot_Preprocessor_lib import open_csv_for_editing
 from MediBot_UI import manage_script_pause, app_control
 
 # Bring in all the constants
 initialize(config)
 
 # Format Data
```

### Comparing `medicafe-0.240508.3/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240508.4/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediBot/update_json.py` & `medicafe-0.240508.4/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediBot/update_medicafe.py` & `medicafe-0.240508.4/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink.py` & `medicafe-0.240508.4/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_277_decoder.py` & `medicafe-0.240508.4/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240508.4/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240508.4/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240508.4/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240508.4/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_Down.py` & `medicafe-0.240508.4/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240508.4/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_Gmail.py` & `medicafe-0.240508.4/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_Scheduler.py` & `medicafe-0.240508.4/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_UI.py` & `medicafe-0.240508.4/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/MediLink/MediLink_Up.py` & `medicafe-0.240508.4/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/PKG-INFO` & `medicafe-0.240508.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240508.3
+Version: 0.240508.4
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240508.3/README.md` & `medicafe-0.240508.4/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/medicafe.egg-info/PKG-INFO` & `medicafe-0.240508.4/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240508.3
+Version: 0.240508.4
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240508.3/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240508.4/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.3/setup.py` & `medicafe-0.240508.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240508.3",
+    version="0.240508.4",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```


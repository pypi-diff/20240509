# Comparing `tmp/medicafe-0.240508.1.tar.gz` & `tmp/medicafe-0.240508.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240508.1.tar", last modified: Thu May  9 02:22:27 2024, max compression
+gzip compressed data, was "medicafe-0.240508.2.tar", last modified: Thu May  9 03:14:34 2024, max compression
```

## Comparing `medicafe-0.240508.1.tar` & `medicafe-0.240508.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 02:22:27.953000 medicafe-0.240508.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240508.1/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240508.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-09 02:22:27.232000 medicafe-0.240508.1/MediBot/
--rwxrwxrwx   0        0        0     2737 2024-05-09 01:25:47.000000 medicafe-0.240508.1/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    25828 2024-05-09 02:18:51.000000 medicafe-0.240508.1/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240508.1/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    32072 2024-05-09 01:21:49.000000 medicafe-0.240508.1/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240508.1/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0        0 2024-05-09 02:18:54.000000 medicafe-0.240508.1/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6393 2024-05-09 02:20:18.000000 medicafe-0.240508.1/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240508.1/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240508.1/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240508.1/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240508.1/MediBot/update_json.py
--rw-rw-rw-   0        0        0     1055 2024-05-07 01:05:17.000000 medicafe-0.240508.1/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-09 02:22:27.745000 medicafe-0.240508.1/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240508.1/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240508.1/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240508.1/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240508.1/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240508.1/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240508.1/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240508.1/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240508.1/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240508.1/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240508.1/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240508.1/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240508.1/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240508.1/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240508.1/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240508.1/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240508.1/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-09 02:22:27.937000 medicafe-0.240508.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240508.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 02:22:27.901000 medicafe-0.240508.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240508.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 02:22:27.949000 medicafe-0.240508.1/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-09 02:22:22.000000 medicafe-0.240508.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 03:14:34.696000 medicafe-0.240508.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240508.2/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240508.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-09 03:14:34.142000 medicafe-0.240508.2/MediBot/
+-rwxrwxrwx   0        0        0     2737 2024-05-09 01:25:47.000000 medicafe-0.240508.2/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    16303 2024-05-09 03:10:37.000000 medicafe-0.240508.2/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240508.2/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    32072 2024-05-09 01:21:49.000000 medicafe-0.240508.2/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240508.2/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0     9823 2024-05-09 03:11:09.000000 medicafe-0.240508.2/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6372 2024-05-09 03:12:27.000000 medicafe-0.240508.2/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240508.2/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240508.2/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240508.2/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240508.2/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240508.2/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-09 03:14:34.533000 medicafe-0.240508.2/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240508.2/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240508.2/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240508.2/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240508.2/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240508.2/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240508.2/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240508.2/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240508.2/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240508.2/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240508.2/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240508.2/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240508.2/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240508.2/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240508.2/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240508.2/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240508.2/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-09 03:14:34.682000 medicafe-0.240508.2/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240508.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 03:14:34.667000 medicafe-0.240508.2/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240508.2/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 03:14:34.692000 medicafe-0.240508.2/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-09 03:14:32.000000 medicafe-0.240508.2/setup.py
```

### Comparing `medicafe-0.240508.1/LICENSE` & `medicafe-0.240508.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediBot/MediBot.bat` & `medicafe-0.240508.2/MediBot/MediBot.bat`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediBot/MediBot_Charges.py` & `medicafe-0.240508.2/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240508.2/MediBot/MediBot_Preprocessor.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240508.2/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240508.2/MediBot/MediBot_dataformat_library.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 from datetime import datetime
 import re  #for addresses
 from MediBot_Preprocessor import config, initialize
 from MediBot_Preprocessor_lib import open_csv_for_editing
-#from MediBot_UI import manage_script_pause
-from MediBot import manage_script_pause
+from MediBot_UI import manage_script_pause, pause_control
 
 # Bring in all the constants
 initialize(config)
 
 # Format Data
 def format_name(value):  
     if ',' in value:
@@ -42,16 +41,15 @@
     alphanumeric = ''.join(filter(str.isalnum, value))
     return alphanumeric
 
 def format_gender(value):
     return value[0].upper()
 
 def format_street(value, csv_data, reverse_mapping, parsed_address_components):
-    global script_paused
-    script_paused = False
+    pause_control.set_pause_status(False)
     
     # Remove periods from the input (seems to be an XP-only issue?)
     value = value.replace('.', '')
     
     # Only proceed with parsing if a comma is present in the value
     if ',' in value:
         try:
@@ -95,15 +93,15 @@
                     parsed_address_components['Zip Code'] = match.group('Zip')
 
                     return match.group('Street').strip()  # Return formatted street address
                     
         except Exception as e:
             print("Address format error: Unable to parse address '{}'. Error: {}".format(value, e))
             print("Please update the CSV file for this record.")
-            script_paused = True
+            pause_control.set_pause_status(True)
             open_csv_for_editing(CSV_FILE_PATH)  # Offer to open the CSV for manual correction
             manage_script_pause(csv_data, e, reverse_mapping) 
             return value.replace(' ', '{Space}')  # Fallback to return original value with spaces escaped
     else:
         # If no comma is present, return the value as is, assuming it's just a street name
         return value.replace(' ', '{Space}')
```

### Comparing `medicafe-0.240508.1/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240508.2/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediBot/update_json.py` & `medicafe-0.240508.2/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink.py` & `medicafe-0.240508.2/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_277_decoder.py` & `medicafe-0.240508.2/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240508.2/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240508.2/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240508.2/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240508.2/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_Down.py` & `medicafe-0.240508.2/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240508.2/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_Gmail.py` & `medicafe-0.240508.2/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_Scheduler.py` & `medicafe-0.240508.2/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_UI.py` & `medicafe-0.240508.2/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/MediLink/MediLink_Up.py` & `medicafe-0.240508.2/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/PKG-INFO` & `medicafe-0.240508.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240508.1
+Version: 0.240508.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240508.1/README.md` & `medicafe-0.240508.2/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240508.2/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240508.1
+Version: 0.240508.2
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240508.1/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240508.2/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.1/setup.py` & `medicafe-0.240508.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240508.1",
+    version="0.240508.2",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```


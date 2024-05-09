# Comparing `tmp/medicafe-0.240508.2.tar.gz` & `tmp/medicafe-0.240508.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240508.2.tar", last modified: Thu May  9 03:14:34 2024, max compression
+gzip compressed data, was "medicafe-0.240508.3.tar", last modified: Thu May  9 04:42:15 2024, max compression
```

## Comparing `medicafe-0.240508.2.tar` & `medicafe-0.240508.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 03:14:34.696000 medicafe-0.240508.2/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240508.2/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240508.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-09 03:14:34.142000 medicafe-0.240508.2/MediBot/
--rwxrwxrwx   0        0        0     2737 2024-05-09 01:25:47.000000 medicafe-0.240508.2/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    16303 2024-05-09 03:10:37.000000 medicafe-0.240508.2/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240508.2/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    32072 2024-05-09 01:21:49.000000 medicafe-0.240508.2/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240508.2/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0     9823 2024-05-09 03:11:09.000000 medicafe-0.240508.2/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6372 2024-05-09 03:12:27.000000 medicafe-0.240508.2/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240508.2/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240508.2/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240508.2/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240508.2/MediBot/update_json.py
--rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240508.2/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-09 03:14:34.533000 medicafe-0.240508.2/MediLink/
--rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240508.2/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240508.2/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240508.2/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240508.2/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240508.2/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240508.2/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240508.2/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240508.2/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240508.2/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240508.2/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240508.2/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240508.2/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240508.2/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240508.2/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240508.2/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240508.2/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-09 03:14:34.682000 medicafe-0.240508.2/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240508.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 03:14:34.667000 medicafe-0.240508.2/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240508.2/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-09 03:14:33.000000 medicafe-0.240508.2/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 03:14:34.692000 medicafe-0.240508.2/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-09 03:14:32.000000 medicafe-0.240508.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 04:42:15.241000 medicafe-0.240508.3/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240508.3/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240508.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-09 04:42:14.694000 medicafe-0.240508.3/MediBot/
+-rwxrwxrwx   0        0        0     3614 2024-05-09 04:40:39.000000 medicafe-0.240508.3/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    16642 2024-05-09 04:18:06.000000 medicafe-0.240508.3/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240508.3/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    32227 2024-05-09 04:18:08.000000 medicafe-0.240508.3/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240508.3/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0    10260 2024-05-09 04:16:32.000000 medicafe-0.240508.3/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6366 2024-05-09 04:18:11.000000 medicafe-0.240508.3/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240508.3/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240508.3/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240508.3/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240508.3/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     1118 2024-05-09 02:39:09.000000 medicafe-0.240508.3/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-09 04:42:15.082000 medicafe-0.240508.3/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240508.3/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240508.3/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240508.3/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240508.3/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240508.3/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240508.3/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240508.3/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240508.3/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240508.3/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240508.3/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240508.3/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240508.3/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240508.3/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240508.3/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240508.3/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240508.3/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-09 04:42:15.227000 medicafe-0.240508.3/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240508.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 04:42:15.213000 medicafe-0.240508.3/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240508.3/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-09 04:42:14.000000 medicafe-0.240508.3/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 04:42:15.237000 medicafe-0.240508.3/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-09 04:42:13.000000 medicafe-0.240508.3/setup.py
```

### Comparing `medicafe-0.240508.2/LICENSE` & `medicafe-0.240508.3/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediBot/MediBot.bat` & `medicafe-0.240508.3/MediBot/MediBot.bat`

 * *Files 16% similar despite different names*

```diff
@@ -8,40 +8,62 @@
 set "source_folder=C:\MEDIANSI\MediCare"
 set "target_folder=C:\MEDIANSI\MediCare\CSV"
 set "config_file=F:\Medibot\json\config.json"
 set "python_script=C:\Python34\Lib\site-packages\MediBot\update_json.py"
 set "python_script2=C:\Python34\Lib\site-packages\MediBot\Medibot.py"
 set "medicafe_package=medicafe"
 set "upgrade_medicafe=F:\Medibot\update_medicafe.py"
+set "temp_file=F:\Medibot\last_update_timestamp.txt"
+
+:: Check if temp file exists and read last update timestamp
+if exist "%temp_file%" (
+    set /p last_update=<"%temp_file%"
+    echo Last update timestamp: !last_update!
+) else (
+    echo No previous update timestamp found.
+)
+
+:: Calculate current date in MMDDYY format
+for /f "tokens=1-3 delims=/" %%a in ("%date%") do (
+    set "month=%%a"
+    set "day=%%b"
+    set "year=%%c"
+)
+set "datestamp=!month!!day!!year:~2,2!"
+
+:: Check if last update was performed today
+if "%last_update%"=="!datestamp!" (
+    echo The Medicafe package was already updated today.
+    timeout /t 1 /nobreak >nul
+    goto :SKIP_UPDATE
+)
 
 :: Prompt user to check for update
 set /p check_update="Do you want to check for an update? (yes/no): "
 if /i "%check_update%"=="no" goto :SKIP_UPDATE
 
 :: Set PYTHONWARNINGS environment variable to ignore deprecation warnings
 set PYTHONWARNINGS=ignore
 
-:: Upgrade Medicafe package in a separate process
-start "Upgrade Medicafe" py "%upgrade_medicafe%"
+:: Upgrade Medicafe package in a separate process and keep the window open after completion
+start "Upgrade Medicafe" cmd /k py "%upgrade_medicafe%" > upgrade_log.txt 2>&1
+exit /b
 
-:: Wait for the upgrade process to complete
-:WAIT_FOR_UPGRADE
-timeout /t 1 /nobreak >nul
-
-:: Check if the upgrade process is still running
-tasklist /fi "WINDOWTITLE eq Upgrade Medicafe" | findstr "py.exe" >nul
-if errorlevel 1 (
-    :: Upgrade process has finished
-    echo Upgrade process completed.
-) else (
-    :: Upgrade process is still running, continue waiting
-    goto WAIT_FOR_UPGRADE
+:SKIP_UPDATE
+
+:: Check if user wants to force an update during the waiting period
+echo Press any key within 3 seconds to force an update anyway...
+timeout /t 3 /nobreak >nul
+if not errorlevel 1 (
+    echo Forcing update...
+    goto :FORCE_UPDATE
 )
 
-:SKIP_UPDATE
+:: Continue script if no key pressed within 3 seconds
+echo Continuing script...
 
 :: Check for the latest CSV file in source folder
 set "latest_csv="
 for /f "delims=" %%a in ('dir /b /a-d /o-d "%source_folder%\*.csv" 2^>nul') do (
     set "latest_csv=%%a"
     goto :found_latest_csv
 )
@@ -61,22 +83,14 @@
     echo No CSV file found.
     goto :end_script
 )
 
 :: Display the name of the found CSV file to the user
 ::echo CSV: !latest_csv!
 
-:: Get the current date in MMDDYY format
-for /f "tokens=1-3 delims=/" %%a in ("%date%") do (
-    set "month=%%a"
-    set "day=%%b"
-    set "year=%%c"
-)
-set "datestamp=!month!!day!!year:~2,2!"
-
 :: Move and rename the CSV file only if found in source folder
 if exist "%source_folder%\!latest_csv!" (
     move "%source_folder%\!latest_csv!" "%target_folder%\SX_CSV_!datestamp!.csv"
     set "new_csv_path=%target_folder%\SX_CSV_!datestamp!.csv"
 ) else (
     set "new_csv_path=%target_folder%\!latest_csv!"
 )
@@ -85,7 +99,18 @@
 py "%python_script%" "%config_file%" "!new_csv_path!"
 
 :: Execute the second Python script
 py "%python_script2%" "%config_file%"
 
 :end_script
 pause
+exit /b
+
+:FORCE_UPDATE
+:: Run the upgrade process
+start "Upgrade Medicafe" cmd /k py "%upgrade_medicafe%" > upgrade_log.txt 2>&1
+
+:: Optionally, you can perform additional actions here
+:: For example, you can display a message to the user indicating that the upgrade is being forced, 
+:: or you can perform cleanup tasks before starting the upgrade process again.
+pause
+exit /b
```

### Comparing `medicafe-0.240508.2/MediBot/MediBot.py` & `medicafe-0.240508.3/MediBot/MediBot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import subprocess
 import os
 import tempfile
 import traceback
 import re  #for addresses
 from collections import OrderedDict
-from MediBot_UI import pause_control, manage_script_pause, user_interaction, MAPAT_MED_PATH, MEDISOFT_SHORTCUT
+from MediBot_UI import app_control, manage_script_pause, user_interaction
 import MediBot_dataformat_library
 import MediBot_Preprocessor
 from MediBot_Preprocessor import initialize, AHK_EXECUTABLE, CSV_FILE_PATH, field_mapping
 import MediBot_Preprocessor_lib
 
 # Add parent directory of the project to the Python path
 import sys
@@ -144,15 +144,15 @@
     while current_row_index < len(csv_data):
         row = csv_data[current_row_index]
         
         # Handle script pause at the start of each row (patient record). 
         manage_script_pause(csv_data, error_message, reverse_mapping)
         error_message = ''  # Clear error message for the next iteration
         
-        if pause_control.get_pause_status():
+        if app_control.get_pause_status():
             continue  # Skip processing this row if the script is paused
 
         # I feel like this is overwriting what would have already been idenfitied in the mapping. 
         # This probably needs to be initialized differently.
         # parsed_address_components = {'City': '', 'State': '', 'Zip Code': ''}
         parsed_address_components = {}
 
@@ -171,15 +171,15 @@
             continue
         elif action == -2:  # Go back two patients and redo
             current_row_index = max(0, current_row_index - 2)  # Go back two rows, but not below 0
             continue
 
         # Code to handle the end of a patient record
         # TODO One day this can just not pause...
-        pause_control.set_pause_status(True)  # Pause at the end of processing each patient record
+        app_control.set_pause_status(True)  # Pause at the end of processing each patient record
         current_row_index += 1  # Move to the next row by default
 
 def open_medisoft(shortcut_path):
     try:
         os.startfile(shortcut_path)
         print("Medisoft is being opened...\n")
     except subprocess.CalledProcessError as e:
@@ -261,15 +261,21 @@
         #print("Debug - Identified fields mapping (main): {}".format(identified_fields)) # Debug Line
         
         proceed, selected_patient_ids, selected_indices, fixed_values = user_interaction(csv_data, interaction_mode, error_message, reverse_mapping)
 
         if proceed:
             # Filter csv_data for selected patients from Triage mode.
             csv_data = [row for index, row in enumerate(csv_data) if index in selected_indices]
-            existing_patients, patients_to_process = MediBot_Preprocessor.check_existing_patients(selected_patient_ids, MAPAT_MED_PATH)
+            
+            # Check if MAPAT_MED_PATH is missing or blank
+            if not app_control.get_mapat_med_path() or not os.path.exists(app_control.get_mapat_med_path()):
+                print("Warning: MAPAT.MED PATH is missing or invalid. Please check the path configuration.")
+
+            # Perform the existing patients check
+            existing_patients, patients_to_process = MediBot_Preprocessor.check_existing_patients(selected_patient_ids, app_control.get_mapat_med_path())
             
             if existing_patients:
                 print("\nNOTE: The following patient(s) already EXIST in the system and \n      will be excluded from processing:")
                 for patient_id, patient_name in existing_patients:
                     print("(ID: {0}) {1}".format(patient_id, patient_name))
                 # Update csv_data to exclude existing patients
                 csv_data = [row for row in csv_data if row[reverse_mapping['Patient ID #2']] in patients_to_process]
@@ -296,16 +302,16 @@
             #        exit(1)
 
                 print("\nRemember, when in Medisoft:")
                 print("  Press 'F8'  to create a New Patient.")
                 print("  Press 'F12' to begin data entry.")
                 print("  Press 'F11' at any time to Pause.")
                 input("\n*** Press [Enter] when ready to begin! ***\n")
-                open_medisoft(MEDISOFT_SHORTCUT)
-                pause_control.set_pause_status(True)
+                open_medisoft(app_control.get_medisoft_shortcut())
+                app_control.set_pause_status(True)
                 _ = manage_script_pause(csv_data, error_message, reverse_mapping)
                 data_entry_loop(csv_data, field_mapping, reverse_mapping, fixed_values)
                 cleanup()                
             else:
                 print("Data entry canceled by user. Exiting MediBot.")
     except Exception as e:
         if e_state:
```

### Comparing `medicafe-0.240508.2/MediBot/MediBot_Charges.py` & `medicafe-0.240508.3/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240508.3/MediBot/MediBot_Preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,20 @@
     import MediLink_DataMgmt
 
 try:
     import MediBot_Preprocessor_lib
 except ImportError:
     from MediBot import MediBot_Preprocessor_lib
 
+try:
+    from MediBot_UI import app_control
+except ImportError:
+    from MediBot import MediBot_UI
+    app_control = MediBot_UI.app_control
+
 """
 Preprocessing Enhancements
 - [X] Preprocess Insurance Policy Numbers and Group Numbers to replace '-' with ''.
 - [X] De-duplicate entries in the CSV and only entering the px once even if they show up twice in the file.
 - [ ] Implement dynamic field combination in CSV pre-processing for flexibility with various CSV formats.
 - [ ] Enhance SSN cleaning logic to handle more variations of sensitive data masking.
 - [ ] Optimize script startup and CSV loading to reduce initial latency.
@@ -144,15 +150,15 @@
         config (dict): Configuration object containing necessary paths and parameters.
         crosswalk ... ADD HERE.
 
     Returns:
         dict: A dictionary mapping patient IDs to insurance IDs.
     """
     # Retrieve MAPAT path and slicing information from the configuration
-    mapat_path = config['MAPAT_MED_PATH']
+    mapat_path = app_control.get_mapat_med_path()
     mapat_slices = crosswalk['mapat_mapping']['slices']
     
     # Initialize the dictionary to hold the patient ID to insurance ID mappings
     patient_id_to_insurance_id = {}
     
     # Read data from MAPAT using a provided function to handle fixed-width data
     for record, _ in MediLink_DataMgmt.read_general_fixed_width_data(mapat_path, mapat_slices):
```

### Comparing `medicafe-0.240508.2/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240508.3/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediBot/MediBot_UI.py` & `medicafe-0.240508.3/MediBot/MediBot_UI.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,53 +6,74 @@
 from MediBot_Preprocessor import config
 
 """
 User Interaction Refinements
 - [ ] Refine the menu options for clearer user guidance during script pauses and errors.
 - [ ] Add functionality for user to easily repeat or skip specific entries without script restart.
     Develop more intuitive skip and retry mechanisms that are responsive to user input during data entry sessions.
-
 """
 # Function to check if a specific key is pressed
 VK_END = int(config.get('VK_END', ""), 16) # Try F12 (7B). Virtual key code for 'End' (23)
 VK_PAUSE = int(config.get('VK_PAUSE', ""), 16) # Try F11 (7A). Virtual-key code for 'Home' (24)
 
-MAPAT_MED_PATH = '' # Initialize global constant for MAPAT path
-MEDISOFT_SHORTCUT = '' # Initialize global constant for LNK path
-
-class PauseControl:
+class AppControl:
     def __init__(self):
         self.script_paused = False
+        self.mapat_med_path = ''
+        self.medisoft_shortcut = ''
+        # Load initial paths from config when instance is created
+        self.load_paths_from_config()
 
     def get_pause_status(self):
         return self.script_paused
 
     def set_pause_status(self, status):
         self.script_paused = status
-        
-pause_control = PauseControl()
+
+    def get_mapat_med_path(self):
+        return self.mapat_med_path
+
+    def set_mapat_med_path(self, path):
+        self.mapat_med_path = path
+
+    def get_medisoft_shortcut(self):
+        return self.medisoft_shortcut
+
+    def set_medisoft_shortcut(self, path):
+        self.medisoft_shortcut = path
+
+    def load_paths_from_config(self, medicare=False):
+        # Assuming `config` is a module or a globally accessible configuration dictionary
+        if medicare:
+            self.mapat_med_path = config.get('MEDICARE_MAPAT_MED_PATH', "")
+            self.medisoft_shortcut = config.get('MEDICARE_SHORTCUT', "")
+        else:
+            self.mapat_med_path = config.get('MAPAT_MED_PATH', "")
+            self.medisoft_shortcut = config.get('PRIVATE_SHORTCUT', "")
+
+app_control = AppControl()
 
 def is_key_pressed(key_code):
     user32 = ctypes.WinDLL('user32', use_last_error=True)
     user32.GetAsyncKeyState.restype = wintypes.SHORT
     user32.GetAsyncKeyState.argtypes = [wintypes.INT]
     return user32.GetAsyncKeyState(key_code) & 0x8000 != 0
 
 def manage_script_pause(csv_data, error_message, reverse_mapping):
     user_action = 0 # initialize as 'continue'
     
-    if not pause_control.get_pause_status() and is_key_pressed(VK_PAUSE):
-        pause_control.set_pause_status(True)
+    if not app_control.get_pause_status() and is_key_pressed(VK_PAUSE):
+        app_control.set_pause_status(True)
         print("Script paused. Opening menu...")
         interaction_mode = 'normal'  # Assuming normal interaction mode for script pause
         user_action = user_interaction(csv_data, interaction_mode, error_message, reverse_mapping)
     
-    while pause_control.get_pause_status():
+    while app_control.get_pause_status():
         if is_key_pressed(VK_END):
-            pause_control.set_pause_status(False)
+            app_control.set_pause_status(False)
             print("Continuing...")
         elif is_key_pressed(VK_PAUSE):
             user_action = user_interaction(csv_data, 'normal', error_message, reverse_mapping)
         time.sleep(0.1)
     
     return user_action
 
@@ -171,44 +192,37 @@
         elif choice == '4':
             print("Exiting the script.")
             exit()
         else:
             print("Invalid choice. Please enter a valid number.")
 
 def user_interaction(csv_data, interaction_mode, error_message, reverse_mapping):
-    # Consider logging the actions taken during user interaction for audit purposes.
-    global MAPAT_MED_PATH, MEDISOFT_SHORTCUT # Initialize global constants
+    global app_control  # Use the instance of AppControl
     selected_patient_ids = []
     selected_indices = []
 
     if interaction_mode == 'triage':
-    
         display_menu_header("            =(^.^)= Welcome to MediBot! =(^.^)=")
-        
+
         while True:
             response = input("\nAm I processing Medicare patients? (yes/no): ").lower().strip()
-            if response:  # Check if the response is not empty
+            if response:
                 if response in ['yes', 'y']:
-                    proceed_as_medicare = True
+                    app_control.load_paths_from_config(medicare=True)
                     break
                 elif response in ['no', 'n']:
-                    proceed_as_medicare = False
+                    app_control.load_paths_from_config(medicare=False)
                     break
                 else:
                     print("Invalid entry. Please enter 'yes' or 'no'.")
             else:
                 print("A response is required. Please try again.")
 
-        MAPAT_MED_PATH = config.get('MEDICARE_MAPAT_MED_PATH', "") if proceed_as_medicare else config.get('MAPAT_MED_PATH', "")
-        MEDISOFT_SHORTCUT = config.get('MEDICARE_SHORTCUT', "") if proceed_as_medicare else config.get('PRIVATE_SHORTCUT', "")
-        
         fixed_values = config.get('fixed_values', {})  # Get fixed values from config json 
-        if proceed_as_medicare:
+        if response in ['yes', 'y']:
             medicare_added_fixed_values = config.get('medicare_added_fixed_values', {})
-            fixed_values.update(medicare_added_fixed_values) # Add any medicare-specific fixed values from config
+            fixed_values.update(medicare_added_fixed_values)  # Add any medicare-specific fixed values from config
         
-        proceed, selected_patient_ids, selected_indices = display_patient_selection_menu(csv_data, reverse_mapping, proceed_as_medicare)
+        proceed, selected_patient_ids, selected_indices = display_patient_selection_menu(csv_data, reverse_mapping, response in ['yes', 'y'])
         return proceed, selected_patient_ids, selected_indices, fixed_values
-    
-    return handle_user_interaction(interaction_mode, error_message)
-
 
+    return handle_user_interaction(interaction_mode, error_message)
```

### Comparing `medicafe-0.240508.2/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240508.3/MediBot/MediBot_dataformat_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from datetime import datetime
 import re  #for addresses
 from MediBot_Preprocessor import config, initialize
 from MediBot_Preprocessor_lib import open_csv_for_editing
-from MediBot_UI import manage_script_pause, pause_control
+from MediBot_UI import manage_script_pause, app_control
 
 # Bring in all the constants
 initialize(config)
 
 # Format Data
 def format_name(value):  
     if ',' in value:
@@ -41,15 +41,15 @@
     alphanumeric = ''.join(filter(str.isalnum, value))
     return alphanumeric
 
 def format_gender(value):
     return value[0].upper()
 
 def format_street(value, csv_data, reverse_mapping, parsed_address_components):
-    pause_control.set_pause_status(False)
+    app_control.set_pause_status(False)
     
     # Remove periods from the input (seems to be an XP-only issue?)
     value = value.replace('.', '')
     
     # Only proceed with parsing if a comma is present in the value
     if ',' in value:
         try:
@@ -93,15 +93,15 @@
                     parsed_address_components['Zip Code'] = match.group('Zip')
 
                     return match.group('Street').strip()  # Return formatted street address
                     
         except Exception as e:
             print("Address format error: Unable to parse address '{}'. Error: {}".format(value, e))
             print("Please update the CSV file for this record.")
-            pause_control.set_pause_status(True)
+            app_control.set_pause_status(True)
             open_csv_for_editing(CSV_FILE_PATH)  # Offer to open the CSV for manual correction
             manage_script_pause(csv_data, e, reverse_mapping) 
             return value.replace(' ', '{Space}')  # Fallback to return original value with spaces escaped
     else:
         # If no comma is present, return the value as is, assuming it's just a street name
         return value.replace(' ', '{Space}')
```

### Comparing `medicafe-0.240508.2/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240508.3/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediBot/update_json.py` & `medicafe-0.240508.3/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediBot/update_medicafe.py` & `medicafe-0.240508.3/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink.py` & `medicafe-0.240508.3/MediLink/MediLink.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_277_decoder.py` & `medicafe-0.240508.3/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240508.3/MediLink/MediLink_837p_encoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240508.3/MediLink/MediLink_837p_encoder_library.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240508.3/MediLink/MediLink_ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240508.3/MediLink/MediLink_DataMgmt.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_Down.py` & `medicafe-0.240508.3/MediLink/MediLink_Down.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240508.3/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_Gmail.py` & `medicafe-0.240508.3/MediLink/MediLink_Gmail.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_Scheduler.py` & `medicafe-0.240508.3/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_UI.py` & `medicafe-0.240508.3/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/MediLink/MediLink_Up.py` & `medicafe-0.240508.3/MediLink/MediLink_Up.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/PKG-INFO` & `medicafe-0.240508.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240508.2
+Version: 0.240508.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240508.2/README.md` & `medicafe-0.240508.3/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/medicafe.egg-info/PKG-INFO` & `medicafe-0.240508.3/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240508.2
+Version: 0.240508.3
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240508.2/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240508.3/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240508.2/setup.py` & `medicafe-0.240508.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240508.2",
+    version="0.240508.3",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```


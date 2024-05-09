# Comparing `tmp/medicafe-0.240507.1.tar.gz` & `tmp/medicafe-0.240508.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medicafe-0.240507.1.tar", last modified: Tue May  7 17:30:27 2024, max compression
+gzip compressed data, was "medicafe-0.240508.1.tar", last modified: Thu May  9 02:22:27 2024, max compression
```

## Comparing `medicafe-0.240507.1.tar` & `medicafe-0.240508.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 17:30:27.414000 medicafe-0.240507.1/
--rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240507.1/LICENSE
--rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240507.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-07 17:30:26.739000 medicafe-0.240507.1/MediBot/
--rwxrwxrwx   0        0        0     2712 2024-05-02 00:07:18.000000 medicafe-0.240507.1/MediBot/MediBot.bat
--rw-rw-rw-   0        0        0    16281 2024-05-02 09:57:36.000000 medicafe-0.240507.1/MediBot/MediBot.py
--rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240507.1/MediBot/MediBot_Charges.py
--rw-rw-rw-   0        0        0    31819 2024-05-07 16:03:03.000000 medicafe-0.240507.1/MediBot/MediBot_Preprocessor.py
--rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240507.1/MediBot/MediBot_Preprocessor_lib.py
--rw-rw-rw-   0        0        0     9619 2024-05-01 03:56:22.000000 medicafe-0.240507.1/MediBot/MediBot_UI.py
--rw-rw-rw-   0        0        0     6314 2024-04-20 04:29:42.000000 medicafe-0.240507.1/MediBot/MediBot_dataformat_library.py
--rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240507.1/MediBot/MediPost.py
--rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240507.1/MediBot/PDF_to_CSV_Cleaner.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240507.1/MediBot/__init__.py
--rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240507.1/MediBot/update_json.py
--rw-rw-rw-   0        0        0     1055 2024-05-07 01:05:17.000000 medicafe-0.240507.1/MediBot/update_medicafe.py
-drwxrwxrwx   0        0        0        0 2024-05-07 17:30:27.204000 medicafe-0.240507.1/MediLink/
--rw-rw-rw-   0        0        0    18006 2024-05-07 17:25:38.000000 medicafe-0.240507.1/MediLink/MediLink.py
--rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240507.1/MediLink/MediLink_277_decoder.py
--rw-rw-rw-   0        0        0    19881 2024-04-30 22:21:02.000000 medicafe-0.240507.1/MediLink/MediLink_837p_encoder.py
--rw-rw-rw-   0        0        0    35159 2024-05-07 16:30:33.000000 medicafe-0.240507.1/MediLink/MediLink_837p_encoder_library.py
--rw-rw-rw-   0        0        0     3893 2024-05-07 16:04:14.000000 medicafe-0.240507.1/MediLink/MediLink_ConfigLoader.py
--rw-rw-rw-   0        0        0    11158 2024-05-07 17:18:02.000000 medicafe-0.240507.1/MediLink/MediLink_DataMgmt.py
--rw-rw-rw-   0        0        0     7131 2024-05-02 10:20:35.000000 medicafe-0.240507.1/MediLink/MediLink_Down.py
--rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240507.1/MediLink/MediLink_ERA_decoder.py
--rw-rw-rw-   0        0        0     6297 2024-05-06 22:21:25.000000 medicafe-0.240507.1/MediLink/MediLink_Gmail.py
--rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240507.1/MediLink/MediLink_Scheduler.py
--rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240507.1/MediLink/MediLink_StatusCheck.py
--rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240507.1/MediLink/MediLink_UI.py
--rw-rw-rw-   0        0        0     5909 2024-05-02 10:20:36.000000 medicafe-0.240507.1/MediLink/MediLink_Up.py
--rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240507.1/MediLink/MediLink_batch.bat
--rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240507.1/MediLink/Soumit_api.py
--rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240507.1/MediLink/__init__.py
--rw-rw-rw-   0        0        0      730 2024-05-07 17:30:27.401000 medicafe-0.240507.1/PKG-INFO
--rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240507.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 17:30:27.377000 medicafe-0.240507.1/medicafe.egg-info/
--rw-rw-rw-   0        0        0      730 2024-05-07 17:30:26.000000 medicafe-0.240507.1/medicafe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-05-07 17:30:26.000000 medicafe-0.240507.1/medicafe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 17:30:26.000000 medicafe-0.240507.1/medicafe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240507.1/medicafe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       60 2024-05-07 17:30:26.000000 medicafe-0.240507.1/medicafe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-07 17:30:26.000000 medicafe-0.240507.1/medicafe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 17:30:27.411000 medicafe-0.240507.1/setup.cfg
--rw-rw-rw-   0        0        0     1164 2024-05-07 17:30:23.000000 medicafe-0.240507.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:22:27.953000 medicafe-0.240508.1/
+-rw-rw-rw-   0        0        0     1096 2024-04-16 02:27:27.000000 medicafe-0.240508.1/LICENSE
+-rw-rw-rw-   0        0        0       64 2024-04-19 20:12:06.000000 medicafe-0.240508.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-09 02:22:27.232000 medicafe-0.240508.1/MediBot/
+-rwxrwxrwx   0        0        0     2737 2024-05-09 01:25:47.000000 medicafe-0.240508.1/MediBot/MediBot.bat
+-rw-rw-rw-   0        0        0    25828 2024-05-09 02:18:51.000000 medicafe-0.240508.1/MediBot/MediBot.py
+-rw-rw-rw-   0        0        0     1963 2024-04-17 03:06:31.000000 medicafe-0.240508.1/MediBot/MediBot_Charges.py
+-rw-rw-rw-   0        0        0    32072 2024-05-09 01:21:49.000000 medicafe-0.240508.1/MediBot/MediBot_Preprocessor.py
+-rw-rw-rw-   0        0        0     4652 2024-05-02 02:13:23.000000 medicafe-0.240508.1/MediBot/MediBot_Preprocessor_lib.py
+-rw-rw-rw-   0        0        0        0 2024-05-09 02:18:54.000000 medicafe-0.240508.1/MediBot/MediBot_UI.py
+-rw-rw-rw-   0        0        0     6393 2024-05-09 02:20:18.000000 medicafe-0.240508.1/MediBot/MediBot_dataformat_library.py
+-rw-rw-rw-   0        0        0      336 2024-04-18 22:50:25.000000 medicafe-0.240508.1/MediBot/MediPost.py
+-rw-rw-rw-   0        0        0     8799 2024-01-30 04:51:58.000000 medicafe-0.240508.1/MediBot/PDF_to_CSV_Cleaner.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:16.000000 medicafe-0.240508.1/MediBot/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-12 16:06:52.000000 medicafe-0.240508.1/MediBot/update_json.py
+-rw-rw-rw-   0        0        0     1055 2024-05-07 01:05:17.000000 medicafe-0.240508.1/MediBot/update_medicafe.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:22:27.745000 medicafe-0.240508.1/MediLink/
+-rw-rw-rw-   0        0        0    18174 2024-05-08 01:57:26.000000 medicafe-0.240508.1/MediLink/MediLink.py
+-rw-rw-rw-   0        0        0     4358 2024-04-13 18:24:36.000000 medicafe-0.240508.1/MediLink/MediLink_277_decoder.py
+-rw-rw-rw-   0        0        0    19946 2024-05-08 01:52:49.000000 medicafe-0.240508.1/MediLink/MediLink_837p_encoder.py
+-rw-rw-rw-   0        0        0    35258 2024-05-09 01:32:35.000000 medicafe-0.240508.1/MediLink/MediLink_837p_encoder_library.py
+-rw-rw-rw-   0        0        0     3914 2024-05-09 02:18:58.000000 medicafe-0.240508.1/MediLink/MediLink_ConfigLoader.py
+-rw-rw-rw-   0        0        0    11166 2024-05-08 01:54:15.000000 medicafe-0.240508.1/MediLink/MediLink_DataMgmt.py
+-rw-rw-rw-   0        0        0     7264 2024-05-08 01:45:53.000000 medicafe-0.240508.1/MediLink/MediLink_Down.py
+-rw-rw-rw-   0        0        0     8724 2024-05-01 03:44:46.000000 medicafe-0.240508.1/MediLink/MediLink_ERA_decoder.py
+-rw-rw-rw-   0        0        0     7063 2024-05-08 21:34:31.000000 medicafe-0.240508.1/MediLink/MediLink_Gmail.py
+-rw-rw-rw-   0        0        0     6040 2024-04-18 22:53:51.000000 medicafe-0.240508.1/MediLink/MediLink_Scheduler.py
+-rw-rw-rw-   0        0        0      222 2024-04-13 17:51:42.000000 medicafe-0.240508.1/MediLink/MediLink_StatusCheck.py
+-rw-rw-rw-   0        0        0     4942 2024-05-07 17:08:35.000000 medicafe-0.240508.1/MediLink/MediLink_UI.py
+-rw-rw-rw-   0        0        0     5904 2024-05-08 01:58:53.000000 medicafe-0.240508.1/MediLink/MediLink_Up.py
+-rwxrwxrwx   0        0        0      118 2024-04-19 22:20:37.000000 medicafe-0.240508.1/MediLink/MediLink_batch.bat
+-rw-rw-rw-   0        0        0      497 2024-03-15 19:39:51.000000 medicafe-0.240508.1/MediLink/Soumit_api.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 02:51:01.000000 medicafe-0.240508.1/MediLink/__init__.py
+-rw-rw-rw-   0        0        0      730 2024-05-09 02:22:27.937000 medicafe-0.240508.1/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2024-04-16 02:33:22.000000 medicafe-0.240508.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 02:22:27.901000 medicafe-0.240508.1/medicafe.egg-info/
+-rw-rw-rw-   0        0        0      730 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1006 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 03:47:58.000000 medicafe-0.240508.1/medicafe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       60 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-09 02:22:26.000000 medicafe-0.240508.1/medicafe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 02:22:27.949000 medicafe-0.240508.1/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2024-05-09 02:22:22.000000 medicafe-0.240508.1/setup.py
```

### Comparing `medicafe-0.240507.1/LICENSE` & `medicafe-0.240508.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediBot/MediBot.bat` & `medicafe-0.240508.1/MediBot/MediBot.bat`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 @echo off
+
+echo Please wait...
+
 setlocal enabledelayedexpansion
 
 :: Define paths
 set "source_folder=C:\MEDIANSI\MediCare"
 set "target_folder=C:\MEDIANSI\MediCare\CSV"
 set "config_file=F:\Medibot\json\config.json"
 set "python_script=C:\Python34\Lib\site-packages\MediBot\update_json.py"
```

### Comparing `medicafe-0.240507.1/MediBot/MediBot_Charges.py` & `medicafe-0.240508.1/MediBot/MediBot_Charges.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediBot/MediBot_Preprocessor.py` & `medicafe-0.240508.1/MediBot/MediBot_Preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,16 @@
     Returns:
         dict: A dictionary mapping insurance names to insurance IDs.
     """
     # Reset config pull to make sure its not using the MediLink config key subset
     config, crosswalk = MediLink_ConfigLoader.load_configuration()
     
     # Retrieve MAINS path and slicing information from the configuration   
-    # TODO For secondary insurance, this needs to be pulling from the correct MAINS (there are 2)
-    # TODO Performance: There probably needs to be a dictionary proxy for MAINS that gets updated.
+    # TODO (Low) For secondary insurance, this needs to be pulling from the correct MAINS (there are 2)
+    # TODO (Low) Performance: There probably needs to be a dictionary proxy for MAINS that gets updated.
     mains_path = config['MAINS_MED_PATH']
     mains_slices = crosswalk['mains_mapping']['slices']
     
     # Initialize the dictionary to hold the insurance to insurance ID mappings
     insurance_to_id = {}
     
     # Read data from MAINS using a provided function to handle fixed-width data
@@ -220,30 +220,29 @@
 
         # Loop through each file in the directory containing Carol's historical CSVs
         for filename in os.listdir(directory_path):
             file_path = os.path.join(directory_path, filename)
             if filename.endswith('.csv'):
                 try:
                     with open(file_path, 'r', encoding='utf-8') as csvfile:
-                                reader = csv.DictReader(csvfile)
-                                found_data = False  # Flag to track if any valid data is found in the CSV
-                                for row in reader:
-                                    if 'Patient ID' not in row or 'Ins1 Payer ID' not in row:
-                                        continue  # Skip this row if either key is missing
-                                    if not row.get('Patient ID').strip() or not row.get('Ins1 Payer ID').strip():
-                                        continue  # Skip this row if either value is missing or empty
-                                    
-                                    found_data = True
-                                    payer_id = row['Ins1 Payer ID'].strip()
-                                    patient_id = row['Patient ID'].strip()
-                                    payer_to_patient_ids[payer_id].add(patient_id)
-                                    MediLink_ConfigLoader.log("Found Patient ID {} with Payer ID {}".format(patient_id, payer_id))
-                                
-                                if not found_data:
-                                    raise ValueError("CSV file '{}' is empty or does not have either Patient ID or Payer ID.".format(filename))
+                        reader = csv.DictReader(csvfile)
+                        found_data = False  # Flag to track if any valid data is found in the CSV
+                        for row in reader:
+                            if 'Patient ID' not in row or 'Ins1 Payer ID' not in row:
+                                continue  # Skip this row if either key is missing
+                            if not row.get('Patient ID').strip() or not row.get('Ins1 Payer ID').strip():
+                                continue  # Skip this row if either value is missing or empty
+                            
+                            found_data = True
+                            payer_id = row['Ins1 Payer ID'].strip()
+                            patient_id = row['Patient ID'].strip()
+                            payer_to_patient_ids[payer_id].add(patient_id)
+                            MediLink_ConfigLoader.log("Found Patient ID {} with Payer ID {}".format(patient_id, payer_id))
+                        if not found_data:
+                            MediLink_ConfigLoader.log("CSV file '{}' is empty or does not have either Patient ID or Payer ID.".format(filename))
                 except Exception as e:
                     print("Error processing file {}: {}".format(filename, e))
     except FileNotFoundError as e:
         print("Error: {}".format(e))
 
     if not payer_to_patient_ids:
         print("No historical mappings were generated.")
@@ -288,15 +287,17 @@
                 medisoft_id = patient_id_to_insurance_id[patient_id]
                 medisoft_ids.add(medisoft_id)
                 MediLink_ConfigLoader.log("Added Medisoft ID {} for Patient ID {} and Payer ID {}".format(medisoft_id, patient_id, payer_id))
             else:
                 MediLink_ConfigLoader.log("No matching Insurance ID found for Patient ID {}".format(patient_id))
         if medisoft_ids:
             payer_id_to_details[payer_id] = {
-                "endpoint": "OPTUMEDI",  # TODO This should be determined via API or configured
+                "endpoint": "OPTUMEDI",  
+                # TODO (Crosswalk Low) This is the initialization default
+                # should be determined via API or configured.
                 "medisoft_id": list(medisoft_ids)
             }
     
     # Update the crosswalk for payer IDs only, retaining other mappings
     crosswalk['payer_id'] = payer_id_to_details
     
     # Save the initial crosswalk
@@ -359,36 +360,37 @@
     }
 
     """    
     # Load insurance mappings from MAINS (Insurance Name to Insurance ID)
     insurance_name_to_id = load_insurance_data_from_mains(config)
     MediLink_ConfigLoader.log("Loaded insurance data from MAINS...")
     
-    # Load new Patient ID to Payer ID mappings from Carol's CSV (This is really just a performance increment)
+    # Load new Patient ID to Payer ID mappings from Carol's CSV (Not Necessary, Right?)
     # patient_id_to_payer_id = load_patient_to_payer_mappings(config)
     
-    # TODO this should work for now but can get bogged down in the futrue since we won't need very old CSVs for incremental changes.
+    # TODO (Performance Low) this should work for now but can get bogged down in the futrue since we 
+    # won't need very old CSVs for incremental changes.
     patient_id_to_payer_id = load_historical_payer_to_patient_mappings(config)
     MediLink_ConfigLoader.log("Loaded historical mappings...")
   
     # Load incremental mapping data from Z.dat (Patient ID to Insurance Name)
-    # BUG Wouldn't the incremental information also be available in the latest MAPAT? Why do I need to wait until Z.dat to get the 
+    # TODO (Crosswalk Med Update Logic) Wouldn't the incremental information also be available in the latest MAPAT? Why do I need to wait until Z.dat to get the 
     # latest update? Seems slower since the initial saving of the patient goes into MAPAT anyway.
     patient_id_to_insurance_name = parse_z_dat(config['MediLink_Config']['Z_DAT_PATH'], config['MediLink_Config'])
     MediLink_ConfigLoader.log("Parsed Z data...")
 
     # Update the crosswalk with new or revised mappings
     for patient_id, payer_id in patient_id_to_payer_id.items():
         insurance_name = patient_id_to_insurance_name.get(patient_id)
         if insurance_name and insurance_name in insurance_name_to_id:
             insurance_id = insurance_name_to_id[insurance_name]
 
             # Ensure payer ID is in the crosswalk and initialize if not
             MediLink_ConfigLoader.log("Initializing payer_id key...")
-            # BUG OPTUMEDI hardcode should be gathered via API
+            # TODO (Crosswalk Low Endpoint) OPTUMEDI hardcode should be gathered via API
             if 'payer_id' not in crosswalk:
                 crosswalk['payer_id'] = {}
             if payer_id not in crosswalk['payer_id']:
                 crosswalk['payer_id'][payer_id] = {'endpoint': 'OPTUMEDI', 'medisoft_id': set()}
 
             # Update the medisoft_id set, temporarily using a set to avoid duplicates
             crosswalk['payer_id'][payer_id]['medisoft_id'].add(insurance_id)
@@ -455,43 +457,45 @@
             # Combine address fields
             address1 = row.get('Patient Address1', '').strip()
             address2 = row.get('Patient Address2', '').strip()
             row['Patient Street'] = "{} {}".format(address1, address2).strip()
             
             # Probably make a data_format function for this?
             # Define the replacements as a dictionary.
-            # TODO this probably needs to sit in the config eventually and not hardcode
+            # TODO (Refactor data_format) this probably needs to sit in the config eventually and not hardcode
             replacements = {
                 '777777777': '',  # Replace '777777777' with an empty string
                 'RAILROAD MEDICARE': 'RAILROAD',  # Replace 'RAILROAD MEDICARE' with 'RAILROAD'
                 'AARP MEDICARE COMPLETE': 'AARP COMPLETE'  # Replace 'AARP MEDICARE COMPLETE' with 'AARP COMPLETE'
             }
 
             # Iterate over each key-value pair in the replacements dictionary
             for old_value, new_value in replacements.items():
                 # Replace the old value with the new value if it exists in the row
                 if row.get('Patient SSN', '') == old_value:
                     row['Patient SSN'] = new_value
                 elif row.get('Primary Insurance', '') == old_value:
                     row['Primary Insurance'] = new_value
 
-            # TODO This is probably the wrong place to implement this? 
-            # TODO Also check to see if it's not overwriting the Medicare '1' assginment within triage.
+            # TODO (Crosswalk Refactor) This is probably the wrong place to implement this? 
+            # TODO (Crosswalk Bot Med) Also check to see if it's not overwriting the Medicare '1' assginment within triage.
             # Add a column with header "Ins1 Insurance ID" based on crosswalk and "Ins1 Payer ID" column for each row
             ins1_payer_id = row.get('Ins1 Payer ID', '').strip()  # Get the Ins1 Payer ID from the row
             if ins1_payer_id:  # Check if Ins1 Payer ID is not empty
                 if ins1_payer_id in crosswalk.get('payer_id', {}):  # Check if Ins1 Payer ID exists in the crosswalk
                     # Get the corresponding medisoft_id(s) for the Ins1 Payer ID from the crosswalk
                     medisoft_ids = crosswalk['payer_id'][ins1_payer_id].get('medisoft_id', [])
                     if medisoft_ids:  # Check if medisoft_ids exist
-                        # TODO Default now is always Assign the first medisoft_id to the "Ins1 Insurance ID" column.
+                        # Convert medisoft_ids from strings to integers
+                        medisoft_ids = [int(id) for id in medisoft_ids]
+                        # TODO (Crosswalk Med) Default now is always Assign the first medisoft_id to the "Ins1 Insurance ID" column.
                         # This needs to be updated so try to match against Carol's naming convention to get a better match
                         row['Ins1 Insurance ID'] = medisoft_ids[0]
                 else:
-                    # TODO If Ins1 Payer ID is not found in the crosswalk then we should make a crosswalk_update entry for the new payer_id
+                    # TODO (Crosswalk Low) If Ins1 Payer ID is not found in the crosswalk then we should make a crosswalk_update entry for the new payer_id
                     # and then it should be passively looking for when the user updates one of these patients in Medisoft. This behavior
                     # should already be covered by the way crosswalk_update works or by the initializer or something, but the initialization
                     # is still pretty janky and I think it will miss older assignments if it doesn't basically do a full re-initialize each time. 
                     # Obviously diminishing returns on age of CSV.
                     MediLink_ConfigLoader.log("Ins1 Payer ID '{}' not found in the crosswalk.".format(ins1_payer_id))
 
     except Exception as e:
```

### Comparing `medicafe-0.240507.1/MediBot/MediBot_Preprocessor_lib.py` & `medicafe-0.240508.1/MediBot/MediBot_Preprocessor_lib.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediBot/MediBot_dataformat_library.py` & `medicafe-0.240508.1/MediBot/MediBot_dataformat_library.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
 from datetime import datetime
 import re  #for addresses
-from MediBot_Preprocessor import open_csv_for_editing, config, initialize
-from MediBot_UI import manage_script_pause
+from MediBot_Preprocessor import config, initialize
+from MediBot_Preprocessor_lib import open_csv_for_editing
+#from MediBot_UI import manage_script_pause
+from MediBot import manage_script_pause
 
 # Bring in all the constants
 initialize(config)
 
 # Format Data
 def format_name(value):  
     if ',' in value:
```

### Comparing `medicafe-0.240507.1/MediBot/PDF_to_CSV_Cleaner.py` & `medicafe-0.240508.1/MediBot/PDF_to_CSV_Cleaner.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediBot/update_json.py` & `medicafe-0.240508.1/MediBot/update_json.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediBot/update_medicafe.py` & `medicafe-0.240508.1/MediBot/update_medicafe.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediLink/MediLink.py` & `medicafe-0.240508.1/MediLink/MediLink.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,18 @@
 Automate response file handling from endpoints and integrate feedback into MediSoft with exception alerts.
 De-persisting Intermediate Files.
 When transmissions fail, there is some retaining of patient data in memory or something that seems to default
 any new endpoint changes to Optum. May need to "de-confirm" patients, but leave the suggested endpoints as the previously
 confirmed endpoints. This should be similar logic to if the user made a mistake and wants to go back and fix it.
 These tasks involve backend enhancements such as dynamic configurations, file detection improvements, file transmission verification, automation of response file handling, and management of intermediate files and transmission failures.
 
-TODO Crosswalk should be to PayerID key vs Medisoft:Endpoint.
-TODO Availity has a response file that says "File was received at TIME. File was sent for processing." as a confirmation 
+TODO (Low) Availity has a response file that says "File was received at TIME. File was sent for processing." as a confirmation 
 that sits in the SendFiles folder after a submittal. 
 
-TODO When an endpoint is updated in the UI, the crosswalk should also be updated and saved for that payer ID because that payer ID
+TODO (Crosswalk) When an endpoint is updated in the UI, the crosswalk should also be updated and saved for that payer ID because that payer ID
 would basically forever need to be going to that endpoint for any patient. the suggested_endpoint should eventually be always correct.
 
 BUG Suggested Endpoint when you say 'n' to proceed with transmission is not getting updated with the endpoint 
 that was selected previously by the user. However, when we go back to the confirmation list, we do have a persist of the assignment.
 This can be confusing for the user.
 
 MediLink
@@ -116,20 +115,20 @@
     detailed_patient_data = []
     
     for personal_info, insurance_info, service_info in MediLink_837p_encoder.read_fixed_width_data(file_path, config.get('MediLink_Config', {})):
         parsed_data = MediLink_837p_encoder.parse_fixed_width_data(personal_info, insurance_info, service_info, config.get('MediLink_Config', {}))
         
         primary_insurance = parsed_data.get('INAME')
         
-        # TODO This suggested endpoint should be a payerid_to_endpoint_mapping.
+        # TODO (High Crosswalk) This suggested endpoint should be a payerid_to_endpoint_mapping.
         # No, we've completely changed this structure so the whole thing is wrong.
         # We're going to have something like payer_id {endpoint:'AVAILITY', insurance_id: {105, 12}}
         # we'll need MAINS to map primary_insurance to insurance_id first and then look for the number in the values.
         try:
-            # TODO Fix this soon. new json format.
+            # Fix this soon. new json format.
             suggested_endpoint = crosswalk['insurance_to_endpoint_mapping'][primary_insurance]
         except KeyError:
             suggested_endpoint = 'AVAILITY'
 
         # Directly enrich detailed patient data with additional information and suggested endpoint
         detailed_data = parsed_data.copy()  # Copy parsed_data to avoid modifying the original dictionary
         detailed_data.update({
@@ -169,49 +168,50 @@
     print("\nChecking for new files across all endpoints...")
     endpoints = config['MediLink_Config']['endpoints']
     processed_endpoints = []
     
     if isinstance(endpoints, dict): # BUG This check can probably be removed later.
         for endpoint_key, endpoint_info in tqdm(endpoints.items(), desc="Processing endpoints"):
             if 'remote_directory_down' in endpoint_info:  # Check if the 'remote_directory_down' key exists
-                #print("Processing endpoint: ", endpoint_info['name']) # BUG this is really for debug only. Positive statements can be muted.
+                #print("Processing endpoint: ", endpoint_info['name']) 
+                # BUG (Debug and verbosity removal) this is really for debug only. Positive statements can be muted.
                 try:
                     ERA_path = MediLink_Down.main(desired_endpoint=endpoint_key)
                     processed_endpoints.append((endpoint_info['name'], ERA_path))
                     MediLink_ConfigLoader.log("Results for {} saved to: {}".format(endpoint_info['name'], ERA_path))
-                    # BUG This needs to check to see if this actually worked maybe winscplog before saying it completed successfully 
+                    # TODO (Low SFTP) This needs to check to see if this actually worked maybe winscplog before saying it completed successfully 
                 except Exception as e:
                     print("An error occurred while checking remittances for {}: {}".format(endpoint_info['name'], e))
             else:
                 MediLink_ConfigLoader.log("Skipping endpoint '{}' as it does not have 'remote_directory_down' configured.".format(endpoint_info['name']))
     else:
         print("Error: Endpoint config is not a 'dictionary' as expected.")
     # Check if all ERA paths are the same
     unique_era_paths = set(path for _, path in processed_endpoints)
     if len(unique_era_paths) == 1:
         common_era_path = unique_era_paths.pop()  # Get the common ERA path
         endpoints_list = ", ".join(endpoint for endpoint, _ in processed_endpoints)
         print("\nProcessed Endpoints: {}".format(endpoints_list))
         print("File located at: {}\n".format(common_era_path))
-        # TODO These prints will eventually be logs when MediPost is made.
+        # TODO (MediPost) These prints will eventually be logs when MediPost is made.
         
     else:
         if processed_endpoints:
             print("\nProcessed Endpoints:")
             for endpoint, path in processed_endpoints:
                 print("Endpoint: {}, ERA Path: {}".format(endpoint, path))
         else:
             print("No endpoints were processed.")
 
 def user_decision_on_suggestions(detailed_patient_data, config):
     """
     Presents the user with all patient summaries and suggested endpoints,
     then asks for confirmation to proceed with all or specify adjustments manually.
     
-    BUG The display summary suggested_endpoint key isn't updating per the user's decision 
+    BUG (Med suggested_endpoint) The display summary suggested_endpoint key isn't updating per the user's decision 
     although the user decision is persisting.
     """
     # Display summaries of patient details and endpoints.
     MediLink_UI.display_patient_summaries(detailed_patient_data)
 
     # Ask the user if they want to proceed with all suggested endpoints.
     proceed = MediLink_UI.ask_for_proceeding_with_endpoints()
@@ -232,15 +232,15 @@
             data['confirmed_endpoint'] = data['suggested_endpoint']
     return detailed_patient_data
 
 def select_and_adjust_files(detailed_patient_data, config):
     """
     Allows users to select patients and adjust their endpoints by interfacing with UI functions.
     
-    BUG After the user is done making their selection, suggested_endpoint should update to persist the 
+    BUG (Med suggested_endpoint) After the user is done making their selection, suggested_endpoint should update to persist the 
     user selection as priority over its original suggestion. Also, the crosswalk should persist the change 
     in the endpoint as well.
     """
     # Display options for patients
     MediLink_UI.display_patient_options(detailed_patient_data)
 
     # Get user-selected indices for adjustment
@@ -259,31 +259,32 @@
             MediLink_UI.display_endpoint_options(config['MediLink_Config']['endpoints'])
             endpoint_index = int(MediLink_UI.get_new_endpoint_choice()) - 1  # Adjusting for zero-based index
             
             if 0 <= endpoint_index < len(endpoint_keys):
                 selected_endpoint_key = endpoint_keys[endpoint_index]
                 data['confirmed_endpoint'] = selected_endpoint_key
                 print("Endpoint changed to {0} for patient {1}.".format(config['MediLink_Config']['endpoints'][selected_endpoint_key]['name'], data['patient_name']))
-                # BUG Probably update crosswalk and suggested endpoint here???
+                # BUG (Med, Crosswalk & suggested_endpoint) Probably update crosswalk and suggested endpoint here???
             else:
                 print("Invalid selection. Keeping the suggested endpoint.")
         else:
             data['confirmed_endpoint'] = data.get('suggested_endpoint', 'N/A')
 
     return detailed_patient_data
 
 def main_menu():
     """
     Initializes the main menu loop and handles the overall program flow,
     including loading configurations and managing user input for menu selections.
     """
     # Load configuration settings and display the initial welcome message.
-    config, crosswalk = MediLink_ConfigLoader.load_configuration() # BUG does this need an argument?
+    config, crosswalk = MediLink_ConfigLoader.load_configuration() 
+    # BUG (Low, Config) does this need an argument? Not sure.
     
-    # TODO Add here a check in config.json for key "MediLink_Config": { "TestMode": true, ...}. If it is true,
+    # TODO (Test Mode) Add here a check in config.json for key "MediLink_Config": { "TestMode": true, ...}. If it is true,
     # prompt the user to say that MediLink is in Test Mode and ask if the user wants to stay in test mode? 
     # Then put placeholder text for now because I don't know what the logic should be.
     
     # Display Welcome Message
     MediLink_UI.display_welcome()
 
     # Normalize the directory path for file operations.
```

### Comparing `medicafe-0.240507.1/MediLink/MediLink_277_decoder.py` & `medicafe-0.240508.1/MediLink/MediLink_277_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediLink/MediLink_837p_encoder.py` & `medicafe-0.240508.1/MediLink/MediLink_837p_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     # Placeholder for the SE segment to be updated with actual segment count later
     segments.append("SE**{transaction_set_control_number:04d}~")
 
     # Update SE segment with the actual segment count and generate the final formatted 837P string
     formatted_837p = MediLink_837p_encoder_library.generate_segment_counts('\n'.join(filter(None, segments)), transaction_set_control_number)
 
     # Optionally, print or log the formatted 837P for debugging or verification
-    # BUG Add chart number to this.
+    # TODO (Low UI/usability) Add chart number to this.
     MediLink_ConfigLoader.log("Formatted 837P for endpoint {}.".format(endpoint), config, level="INFO")
 
     return formatted_837p
 
 def write_output_file(document_segments, output_directory, endpoint_key, input_file_path, config):
     """
     Writes formatted 837P document segments to an output file with a dynamically generated name.
@@ -242,15 +242,15 @@
     if not endpoint_config:
         print("Endpoint configuration for {} not found.".format(endpoint))
         return None
 
     # Retrieve desired default output file path from config
     output_directory = config.get('outputFilePath', '')
     
-    # BUG This is a WinSCP validation because of the mishandling of spaces in paths. 
+    # BUG (Low SFTP) This is a WinSCP validation because of the mishandling of spaces in paths. 
     # This shouldn't need to exist.
     output_directory = winscp_validate_output_directory(output_directory)
     
     if not os.path.isdir(output_directory):
         print("Output directory does not exist. Please check the configuration.")
         return None
 
@@ -260,15 +260,16 @@
 
     # Initialize the transaction set control number
     transaction_set_control_number = 1
 
     # Process each patient's data in the list
     for patient_data in patient_data_list:
         # Assuming validate_claim_data is adapted to handle individual patient data dictionaries
-        if True: #validate_claim_data(patient_data, config): BUG DISABLED VALIDATION
+        if True: #validate_claim_data(patient_data, config):
+            # BUG (Low- Reliability) DISABLED VALIDATION
             # The format_single_claim function needs to be adapted to handle individual patient data dictionaries
             formatted_claim = format_single_claim(patient_data, config, endpoint, transaction_set_control_number)
             document_segments.append(formatted_claim)
             transaction_set_control_number += 1
 
     # Append interchange trailer
     ge_trailer, iea_trailer = MediLink_837p_encoder_library.create_interchange_trailer(config, endpoint, transaction_set_control_number - 1)
```

### Comparing `medicafe-0.240507.1/MediLink/MediLink_837p_encoder_library.py` & `medicafe-0.240508.1/MediLink/MediLink_837p_encoder_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,27 +210,27 @@
         
         # Get payer ID corresponding to the medisoft ID
         for payer, payer_info in crosswalk['payer_id'].items():
             if medisoft_id_str in payer_info['medisoft_id']:
                 return payer
         
         raise ValueError("No payer ID found for Medisoft ID: {}".format(medisoft_id))
-        # TODO OK so then what? This is when the crosswalk has insufficient information.
+        # TODO (Med Crosswalk) OK so then what? This is when the crosswalk has insufficient information.
         # This means there is a new insurance from the Z data that we haven't seen before?
         # update_crosswalk would have had to catch this earlier in the flow.
         
     except ValueError as e:
         if "JSON" in str(e) and "decode" in str(e):
             raise ValueError("Error decoding the crosswalk JSON file")
         else:
             raise e
 
 def fetch_payer_name_from_crosswalk(payer_id, config, endpoint):
     """
-    BUG TODO This is the backup function for when Availity cant resolve the payer name.
+    TODO (Low Crosswalk) This is the backup function for when Availity cant resolve the payer name.
     The best thing to do here would probably be to pull from Carol's CSV but maybe we 
     can start with trying to pull from MAINS and just use that as the default for now.
     For now, this is not make-work because Availity can resolve what we want right now.
     
     Retrieves the payer name corresponding to a given payer ID from a crosswalk mapping.
     
     Parameters:
@@ -246,17 +246,18 @@
     # Ensure the 'crosswalkPath' key exists in config and contains the path to the crosswalk JSON file
     if 'crosswalkPath' not in config:
         raise ValueError("Crosswalk path not defined in configuration.")
 
     crosswalk_path = config.get('crosswalkPath')
     try:
         with open(crosswalk_path, 'r') as file:
-            crosswalk_mappings = json.load(file) # BUG This should be using ConfigLoader.
+            crosswalk_mappings = json.load(file) 
+            # BUG (Low ConfigLoader) This should be using ConfigLoader.
         # Select the endpoint-specific section from the mappings
-        # BUG This whole thing needs to be re-worked.
+        # This whole thing needs to be re-worked. Why again? I forgot.
         endpoint_mappings = crosswalk_mappings['payer_id'].get(endpoint, {})
         payer_name = endpoint_mappings.get(payer_id)
 
         if not payer_name:
             raise ValueError("Payer name not found for payer ID: {} in {} mappings.".format(payer_id, endpoint))
 
         return payer_name
@@ -349,15 +350,15 @@
     n3_segment = "N3*{}~".format(payer_address_line_1)
     n4_segment = "N4*{}*{}*{}~".format(payer_city, payer_state, payer_zip)
 
     return [n3_segment, n4_segment]
 
 # Fetches the payer name from API based on the payer ID.
 # Initialize a global dictionary to store the access token and its expiry time
-# BUG This will need to get setup for each endpoint separately. 
+# TODO (Low API) This will need to get setup for each endpoint separately. 
 token_cache = {
     'access_token': None,
     'expires_at': 0  # Timestamp of when the token expires
 }
 
 def get_access_token(endpoint_config):
     current_time = time.time()
@@ -465,26 +466,25 @@
     # If the payer is secondary insurance after Medicare, use 'S' (Secondary)
     # Assume everything is Primary for now.
     responsibility_code = 'P'
 
     # Insurance Type Code
     insurance_type_code = insurance_type_selection()
 
-
     # Construct the SBR segment using the determined codes
     sbr_segment = "SBR*{responsibility_code}*18*******{insurance_type_code}~".format(
         responsibility_code=responsibility_code,
         insurance_type_code=insurance_type_code
     )
 
     return sbr_segment
 
 def insurance_type_selection():
     """
-    TODO Finish making this function. This should integrate into a menu for now and then figure 
+    TODO (Med SBR09) Finish making this function. This should integrate into a menu for now and then figure 
     out the automated/API method to getting this.
     
     11 - Other Non-Federal Programs
     12 - Preferred Provider Organization (PPO)
     13 - Point of Service (POS)
     14 - Exclusive Provider Organization (EPO)
     15 - Indemnity Insurance
```

### Comparing `medicafe-0.240507.1/MediLink/MediLink_ConfigLoader.py` & `medicafe-0.240508.1/MediLink/MediLink_ConfigLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 from collections import OrderedDict
 import sys
 import platform
 
 """
 This function should be generalizable to have a initialization script over all the Medi* functions
 """
-
 def load_configuration(config_path=os.path.join(os.path.dirname(__file__), '..', 'json', 'config.json'), crosswalk_path=os.path.join(os.path.dirname(__file__), '..', 'json', 'crosswalk.json')):
     """
     Loads endpoint configuration, credentials, and other settings from JSON files.
         
     Returns: A tuple containing dictionaries with configuration settings for the main config and crosswalk.
     """
-    # TODO The Medicare / Private differentiator flag probably needs to be pulled or passed to this.
-    # BUG HARDCODE FOR NOW:
+    # TODO (Low Config Upgrade) The Medicare / Private differentiator flag probably needs to be pulled or passed to this.
+    # BUG (HARDCODE) FOR NOW:
     # Detect the operating system
     if platform.system() == 'Windows' and platform.release() == 'XP':
         # Use F: paths for Windows XP
         config_path = "F:\\Medibot\\json\\config.json"
         crosswalk_path = "F:\\Medibot\\json\\crosswalk.json"
     else:
         # Use G: paths for other versions of Windows
```

### Comparing `medicafe-0.240507.1/MediLink/MediLink_DataMgmt.py` & `medicafe-0.240508.1/MediLink/MediLink_DataMgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import csv
 import os
 from datetime import datetime, timedelta
-import subprocess # BUG Currently disabled for testing.
+import subprocess 
 
 # Need this for running Medibot and MediLink
 try:
     import MediLink_ConfigLoader
 except ImportError:
     from . import MediLink_ConfigLoader
 
@@ -47,15 +47,15 @@
                     personal_info, insurance_info, service_info = lines_buffer
                     MediLink_ConfigLoader.log("Successfully read data from file: {}".format(file_path), config, level="INFO")
                     yield personal_info, insurance_info, service_info
                     lines_buffer.clear()  # Reset buffer for the next patient record
             # If the line is blank but we have already started collecting a patient record,
             # we continue without resetting the buffer, effectively skipping blank lines.
 
-# TODO Consider consolidating with the other read_fixed_with_data 
+# TODO (Refactor) Consider consolidating with the other read_fixed_with_data 
 def read_general_fixed_width_data(file_path, slices):
     # handle any fixed-width data based on provided slice definitions
     with open(file_path, 'r', encoding='utf-8') as file:
         next(file)  # Skip the header
         for line_number, line in enumerate(file, start=1):
             insurance_name = {key: line[start:end].strip() for key, (start, end) in slices.items()}
             yield insurance_name, line_number
@@ -131,15 +131,15 @@
         'remote_directory_down': '/remote/download/path'
     }
 
     operate_winscp('download', None, download_config, 'path/to/local/storage', config)
     """
     # Setup paths
     try:
-        # TODO Get this updated. ??
+        # TODO (Easy / Config) Get this updated. ??
         winscp_path = config['winscp_path']
     except KeyError:
         winscp_path = os.path.join(os.getcwd(), "Installers", "WinSCP-Portable", "WinSCP.com")
     except Exception as e:
         # Handle any other exceptions here
         print("An error occurred while running WinSCP:", e)
         winscp_path = None
@@ -164,15 +164,15 @@
         '/command',
         'open {}'.format(session_name),
         'cd /',
         'cd {}'.format(remote_directory)
     ]
 
     # Add commands to WinSCP script
-    # BUG We really need to fix this path situation.
+    # BUG (Low SFTP) We really need to fix this path situation.
     #  Unfortunately, this just needs to be a non-spaced path because WinSCP can't
     #  handle the spaces. Also, Windows won't let me use shutil to move the files out of G:\ into C:\ and it it wants an administrator security 
     #  check or verification thing for me to even move the file by hand so that doesn't work either. 
     #  command.append("put {}".format("C:\\Z_optumedi_04161742.txt"))
     if operation_type == "upload":
         for file_path in files:
             normalized_path = os.path.normpath(file_path)
@@ -192,16 +192,16 @@
         # TestMode is not enabled, execute the command
         process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False)
         stdout, stderr = process.communicate()
 
     
     if True: #process.returncode == 0:
         # Replace this with your condition to check if WinSCP operation was successful
-        # BUG This return code is a little trigger happy.
-        # BUG If the WinSCP command specifies the correct download path, this might not be necessary
+        # BUG (Low SFTP) This return code is a little trigger happy.
+        # If the WinSCP command specifies the correct download path, this might not be necessary
         # move_downloaded_files(local_storage_path)
         # print("WINSCP IS CURRENTLY DISABLED FOR TESTING.") # BUG
         MediLink_ConfigLoader.log("Files {}ed successfully.".format(operation_type))
         
         # Construct a list of downloaded files if operation_type is 'download'
         if operation_type == 'download':
             downloaded_files = []
```

### Comparing `medicafe-0.240507.1/MediLink/MediLink_Down.py` & `medicafe-0.240508.1/MediLink/MediLink_Down.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,16 @@
             consolidate_csv_path = MediLink_ERA_decoder.consolidate_csvs(output_directory)
             MediLink_ConfigLoader.log("Translation and consolidation completed.")
             return consolidate_csv_path
         else:
             MediLink_ConfigLoader.log("No ERA files found matching: {}".format(args.era_file_path))
             return
     
-    # TODO This probably needs to be built into a loop that cycles through all 3 endpoints. 
+    # TODO (Low Remit) This probably needs to be built into a loop that cycles through all 3 endpoints. 
+    # I think the uploader has something like this implemented already since it sends to all the endpoints.
     # The loop should use the tdqa or whatever the progress bar is called.
     # print("Please wait...\n")
     
     # Validate endpoint key
     endpoint_key = args.desired_endpoint
     if endpoint_key not in config['MediLink_Config']['endpoints']:
         MediLink_ConfigLoader.log("Endpoint '{}' not found in configuration. Using default 'AVAILITY'.".format(endpoint_key))
@@ -103,15 +104,15 @@
         
     # Download ERA files from the configured endpoint
     downloaded_files = operate_winscp("download", None, endpoint_config, local_storage_path, config)
 
     # Translate downloaded ERA files to CSV format
     translated_csv_paths = []
     for file in downloaded_files:
-        # TODO This needs to add functionality for differentiating between ERA, 277, IBT or 
+        # TODO (Low Remit) This needs to add functionality for differentiating between ERA, 277, IBT or 
         # whatever else might be included in the download folders.
         MediLink_ERA_decoder.translate_era_to_csv([file], output_directory)
         csv_file_path = os.path.join(output_directory, os.path.basename(file) + '.csv')
         translated_csv_paths.append(csv_file_path)
         MediLink_ConfigLoader.log("Translated ERA to CSV: {}".format(csv_file_path))
     
     # Consolidate new CSVs
```

### Comparing `medicafe-0.240507.1/MediLink/MediLink_ERA_decoder.py` & `medicafe-0.240508.1/MediLink/MediLink_ERA_decoder.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediLink/MediLink_Gmail.py` & `medicafe-0.240508.1/MediLink/MediLink_Gmail.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 **Google Apps Script (Server Side)**
 - **Functionality**:
     - Authenticate and access Gmail to extract the 'Read the message' link.
     - Provide support for initial email filtering and link extraction.
     - Not involved in the decryption or direct handling of PHI data to ensure compliance with HIPAA.
 
 This architecture ensures the system handles sensitive PHI data in compliance with HIPAA regulations while maintaining robust and reliable email processing and file handling mechanisms. All sensitive data transfers occur directly from Microsoft's secure environment, minimizing the risk of unauthorized access during transit.
+
+TODO (High GMail)
 """
 import requests
 import webbrowser
 import time
 from MediLink_ConfigLoader import log
 
 def initiate_process():
@@ -79,35 +81,57 @@
     """
     Retrieves the 'Read the message' link from the Google Apps Script.
     """
     try:
         url = "https://script.google.com/macros/s/AKfycbzlq8d32mDlLdtFxgL_zvLJernlGPB64ftyxyH8F1nNlr3P-VBH6Yd0NGa1pbBc5AozvQ/exec"
         params = {'action': 'get_link'}
         response = requests.get(url, params=params)
-        if response.status_code == 200 and response.text.startswith("http"):
-            return response.text
+        if response.status_code == 200:
+            # Use the new JSON response handling method
+            link_response = handle_response(response)
+            if link_response:
+                return link_response
+            else:
+                log("Failed to retrieve link: No link available in the response.")
         else:
             log("Failed to retrieve link: HTTP status {}, Response text: {}".format(response.status_code, response.text))
-            return None
     except Exception as e:
         log("Error retrieving link: {}".format(str(e)))
-        return None
+    return None
 
 def poll_for_otp():
     """
     Polls the Google Apps Script for the OTP, waiting until it is available.
     """
     url = "https://script.google.com/macros/s/AKfycbzlq8d32mDlLdtFxgL_zvLJernlGPB64ftyxyH8F1nNlr3P-VBH6Yd0NGa1pbBc5AozvQ/exec"
     params = {'action': 'get_otp'}
-    timeout = time.time() + 60*3  # Poll for 3 minutes max
+    timeout = time.time() + 60*1  # Poll for 1 minute max
     while time.time() < timeout:
         response = requests.get(url, params=params)
-        if response.status_code == 200 and response.text.isdigit():
-            return response.text
-        elif response.status_code != 200:
+        if response.status_code == 200:
+            # Use the new JSON response handling method
+            otp_response = handle_response(response)
+            if otp_response:
+                return otp_response
+        else:
             log("Failed to retrieve OTP, HTTP status: {}".format(response.status_code))
-        time.sleep(5)  # Poll every 5 seconds
+        time.sleep(15)  # Poll every 15 seconds
     log("OTP not retrieved within the timeout period.")
     return None
 
+def handle_response(response):
+    """
+    Parses the JSON response from the server and returns data if successful,
+    otherwise logs an error message.
+    """
+    try:
+        data = response.json()  # Parse the JSON string
+        if data['status'] == 'success':
+            return data['data']
+        else:
+            log("Error: " + data['message'])
+    except ValueError:
+        log("Error parsing response: Invalid JSON format.")
+    return None
+
 if __name__ == "__main__":
     initiate_process()
```

### Comparing `medicafe-0.240507.1/MediLink/MediLink_Scheduler.py` & `medicafe-0.240508.1/MediLink/MediLink_Scheduler.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediLink/MediLink_UI.py` & `medicafe-0.240508.1/MediLink/MediLink_UI.py`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/MediLink/MediLink_Up.py` & `medicafe-0.240508.1/MediLink/MediLink_Up.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import os
 import subprocess
-import logging
 import MediLink_837p_encoder
 from MediLink_ConfigLoader import log
 from tqdm import tqdm
 from MediLink_DataMgmt import operate_winscp
 
 """
 Handles the transmission of files to endpoints and related tasks for the MediLink script.
@@ -43,19 +41,19 @@
     """
     Handles the result of the file transmission process. Logs the outcome and provides user feedback.
 
     :param transmission_result: The result of the file transmission process.
     """
     #if transmission_result:
         #log("Transmission successful")
-        # TODO This needs to do an actual check in the WinSCP log to make sure this is actually true.
+        # TODO (Low SFTP) This needs to do an actual check in the WinSCP log to make sure this is actually true.
         #print("Files have been successfully transmitted.")
     #else:
         #log("Transmission failed")
-        # TODO This needs to do a pull from the WinSCP log to show the user what happened.
+        # TODO (Low SFTP) This needs to do a pull from the WinSCP log to show the user what happened.
         #print("There was an issue with the file transmission.")
 
 def submit_claims(detailed_patient_data_grouped_by_endpoint, config):
     if not detailed_patient_data_grouped_by_endpoint:
         print("No new files detected for submission.")
         return
```

### Comparing `medicafe-0.240507.1/PKG-INFO` & `medicafe-0.240508.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240507.1
+Version: 0.240508.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240507.1/README.md` & `medicafe-0.240508.1/README.md`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/medicafe.egg-info/PKG-INFO` & `medicafe-0.240508.1/medicafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medicafe
-Version: 0.240507.1
+Version: 0.240508.1
 Summary: MediCafe
 Home-page: https://github.com/katanada2
 Author: Daniel Vidaud
 Author-email: daniel@personalizedtransformation.com
 License: MIT
 Keywords: medicafe python34 medibot medilink
 Description-Content-Type: text/markdown
```

### Comparing `medicafe-0.240507.1/medicafe.egg-info/SOURCES.txt` & `medicafe-0.240508.1/medicafe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medicafe-0.240507.1/setup.py` & `medicafe-0.240508.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medicafe',
-    version="0.240507.1",
+    version="0.240508.1",
     description='MediCafe',
     long_description='This module ensures that MediCafe remains up-to-date by performing version checks for its dependencies on startup. It utilizes PyPI, the official repository for Python packages, to retrieve information about the latest available versions of the required packages. When an internet connection is available, MediUpdate automatically installs any available updates using pip, the package installer for Python.',
     long_description_content_type='text/markdown',
     keywords = 'medicafe python34 medibot medilink',
     url='https://github.com/katanada2',
     author='Daniel Vidaud',
     author_email='daniel@personalizedtransformation.com',
```


# Comparing `tmp/mesa2_preprocessing-0.1.0.tar.gz` & `tmp/mesa2_preprocessing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mesa2_preprocessing-0.1.0.tar", last modified: Wed May  8 20:42:55 2024, max compression
+gzip compressed data, was "mesa2_preprocessing-0.2.0.tar", last modified: Thu May  9 08:53:26 2024, max compression
```

## Comparing `mesa2_preprocessing-0.1.0.tar` & `mesa2_preprocessing-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 20:42:55.927894 mesa2_preprocessing-0.1.0/
--rw-rw-rw-   0        0        0     1091 2024-05-08 20:04:06.000000 mesa2_preprocessing-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1977 2024-05-08 20:42:55.924902 mesa2_preprocessing-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1111 2024-05-08 20:14:08.000000 mesa2_preprocessing-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 20:42:55.870267 mesa2_preprocessing-0.1.0/mesa2_preprocessing/
--rw-rw-rw-   0        0        0      122 2024-05-08 20:42:20.000000 mesa2_preprocessing-0.1.0/mesa2_preprocessing/__init__.py
--rw-rw-rw-   0        0        0    11863 2024-05-08 19:35:26.000000 mesa2_preprocessing-0.1.0/mesa2_preprocessing/operations.py
-drwxrwxrwx   0        0        0        0 2024-05-08 20:42:55.918869 mesa2_preprocessing-0.1.0/mesa2_preprocessing.egg-info/
--rw-rw-rw-   0        0        0     1977 2024-05-08 20:42:55.000000 mesa2_preprocessing-0.1.0/mesa2_preprocessing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-05-08 20:42:55.000000 mesa2_preprocessing-0.1.0/mesa2_preprocessing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 20:42:55.000000 mesa2_preprocessing-0.1.0/mesa2_preprocessing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-08 20:42:55.000000 mesa2_preprocessing-0.1.0/mesa2_preprocessing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-08 20:42:55.000000 mesa2_preprocessing-0.1.0/mesa2_preprocessing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 20:42:55.927894 mesa2_preprocessing-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1082 2024-05-08 20:14:08.000000 mesa2_preprocessing-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:26.799644 mesa2_preprocessing-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2024-05-08 20:04:06.000000 mesa2_preprocessing-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1972 2024-05-09 08:53:26.796638 mesa2_preprocessing-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1107 2024-05-09 08:39:03.000000 mesa2_preprocessing-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:26.753004 mesa2_preprocessing-0.2.0/mesa2_preprocessing/
+-rw-rw-rw-   0        0        0      165 2024-05-09 08:39:03.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    12019 2024-05-09 08:39:03.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing/operations.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:26.793626 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/
+-rw-rw-rw-   0        0        0     1972 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-09 08:53:26.000000 mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 08:53:26.800637 mesa2_preprocessing-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2024-05-09 08:53:15.000000 mesa2_preprocessing-0.2.0/setup.py
```

### Comparing `mesa2_preprocessing-0.1.0/LICENSE` & `mesa2_preprocessing-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mesa2_preprocessing-0.1.0/PKG-INFO` & `mesa2_preprocessing-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mesa2_preprocessing
-Version: 0.1.0
-Summary: A tool for post-processing MESA2.0 measurement data
+Version: 0.2.0
+Summary: A tool for pre-processing MESA2.0 measurement data
 Author: Nadir Nadirov
 Author-email: nadirnadirov1999@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.0
 Requires-Dist: numpy>=1.18
 Requires-Dist: nptdms>=0.25
 
-# MESA2.0 Postprocessing Tool
+# MESA2.0 Preprocessing Tool
 
 This package provides a set of tools designed for pre-processing MESA2.0 measurement data. It includes functionality to read, merge, and process measurement data efficiently.
 
 ## Features
 - Read data from `.dat` and associated binary files.
 - Merge data from different sources like TDMS and DAT files.
 - Export processed data to various formats such as CSV and Parquet.
@@ -54,8 +54,8 @@
 
 - Python >= 3.8
 - pandas
 - numpy
 - nptdms
 
 ## License
-This project is licensed under the MIT License - see the LICENSE.md file for details.
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `mesa2_preprocessing-0.1.0/README.md` & `mesa2_preprocessing-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# MESA2.0 Postprocessing Tool
+# MESA2.0 Preprocessing Tool
 
 This package provides a set of tools designed for pre-processing MESA2.0 measurement data. It includes functionality to read, merge, and process measurement data efficiently.
 
 ## Features
 - Read data from `.dat` and associated binary files.
 - Merge data from different sources like TDMS and DAT files.
 - Export processed data to various formats such as CSV and Parquet.
@@ -31,8 +31,8 @@
 
 - Python >= 3.8
 - pandas
 - numpy
 - nptdms
 
 ## License
-This project is licensed under the MIT License - see the LICENSE.md file for details.
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `mesa2_preprocessing-0.1.0/mesa2_preprocessing/operations.py` & `mesa2_preprocessing-0.2.0/mesa2_preprocessing/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,57 +153,61 @@
             dataframe.to_csv(csv_file_name, sep=';', index=False)
             print(f"Data saved to {csv_file_name}")
         else:
             print("No data available to save to CSV.")
     except Exception as e:
         print(f"Failed to save data to CSV: {e}")
 
-def merge_dat_with_tdms(tdms_path, dat_path, fill_missing='nan'):
+
+def merge_dat_with_tdms(tdms_path, dat_path, base_channel='UnixTime', fill_missing='nan'):
     """
     Merges data from TDMS and DAT files into a single DataFrame.
 
     Parameters:
         tdms_path (str): The file path to the TDMS file.
         dat_path (str): The file path to the DAT file.
+        base_channel (str): The channel for merging data from DAT to TDMS
         fill_missing (str): Specifies how to handle missing values: 'drop' or 'nan'.
 
     Returns:
         tuple: Contains merged DataFrame, TDMS channel units, DAT channel units, and the root name.
     """
     try:
         tdms_file = TdmsFile.read(tdms_path)
         tdms_df = tdms_file.as_dataframe()
 
         # Adjust column names by removing quotes and paths
         tdms_df.columns = [col.split('/')[-1].replace("'", "").strip() for col in tdms_df.columns]
-        tdms_channel_units = {channel.path.split('/')[-1].replace("'", "").strip(): channel.properties.get('unit_string', 'unknown')
-                              for group in tdms_file.groups() for channel in group.channels()}
+        tdms_channel_units = {
+            channel.path.split('/')[-1].replace("'", "").strip(): channel.properties.get('unit_string', 'unknown')
+            for group in tdms_file.groups() for channel in group.channels()}
 
         channels, _ = read_dat_file(dat_path)
         dat_df = dat_to_df(dat_path)
 
         root_name = 'Measurement'
         for group in tdms_file.groups():
             root_name = group.name
 
         # Store units and names for .dat channels
         dat_channel_units = {channel['name']: channel.get('unit', 'unknown') for channel in channels.values()}
 
-        merged_df = pd.merge(tdms_df, dat_df, on='UnixTime', how='left')
+        merged_df = pd.merge(tdms_df, dat_df, on=base_channel, how='left')
 
         if fill_missing == 'drop':
             merged_df.dropna(inplace=True)
         elif fill_missing == 'nan':
             merged_df.fillna(value=np.nan, inplace=True)
 
         return merged_df, tdms_channel_units, dat_channel_units, root_name
     except Exception as e:
         print(f"Error merging TDMS and DAT files: {e}")
         return pd.DataFrame(), {}, {}, 'Measurement'
 
+
 def save_to_tdms(df, tdms_channel_units, dat_channel_units, tdms_path_read, root_name, output_directory):
     """
     Saves the merged DataFrame to a new TDMS file with metadata.
 
     Parameters:
         df (pd.DataFrame): The DataFrame to save.
         tdms_channel_units (dict): Dictionary of units from TDMS channels.
@@ -229,26 +233,26 @@
                 channel = ChannelObject(root_name, column, df[column].values, properties=properties)
                 tdms_writer.write_segment([root_object, channel])
             print(f"Data successfully saved to TDMS file: {tdms_path_write}")
     except Exception as e:
         print(f"Error saving data to TDMS file: {e}")
 
 
-def create_merged_tdms(tdms_path, dat_path, output_directory, fill_missing='drop'):
+def create_merged_tdms(tdms_path, dat_path, output_directory, base_channel='UnixTime', fill_missing='drop'):
     """
     Creates a merged TDMS file from TDMS and DAT sources.
 
     Parameters:
         tdms_path (str): The file path to the TDMS file.
         dat_path (str): The file path to the DAT file.
         output_directory (str): The directory to save the merged TDMS file.
         fill_missing (str): Specifies how to handle missing values in the merge.
     """
     result_df, tdms_channel_units, dat_channel_units, root_name = merge_dat_with_tdms(
-        tdms_path, dat_path, fill_missing=fill_missing)
+        tdms_path, dat_path, base_channel=base_channel, fill_missing=fill_missing)
     save_to_tdms(result_df, tdms_channel_units, dat_channel_units, tdms_path, root_name, output_directory)
 
 
 def tdms_to_parquet(tdms_path, parquet_file_name):
     try:
         tdms_file = TdmsFile.read(tdms_path)
         dataframe = tdms_file.as_dataframe()
@@ -292,8 +296,8 @@
         # Determine the output file path
         output_file_path = os.path.splitext(tdms_path)[0] + "_metadata.csv"
 
         # Save the DataFrame to CSV
         metadata_df.to_csv(output_file_path, sep=';', index=False)
         print(f"Metadata saved successfully to: {output_file_path}")
     except Exception as e:
-        print(f"An error occurred while extracting metadata from the TDMS file: {e}")
+        print(f"An error occurred while extracting metadata from the TDMS file: {e}")
```

### Comparing `mesa2_preprocessing-0.1.0/mesa2_preprocessing.egg-info/PKG-INFO` & `mesa2_preprocessing-0.2.0/mesa2_preprocessing.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mesa2-preprocessing
-Version: 0.1.0
-Summary: A tool for post-processing MESA2.0 measurement data
+Version: 0.2.0
+Summary: A tool for pre-processing MESA2.0 measurement data
 Author: Nadir Nadirov
 Author-email: nadirnadirov1999@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.0
 Requires-Dist: numpy>=1.18
 Requires-Dist: nptdms>=0.25
 
-# MESA2.0 Postprocessing Tool
+# MESA2.0 Preprocessing Tool
 
 This package provides a set of tools designed for pre-processing MESA2.0 measurement data. It includes functionality to read, merge, and process measurement data efficiently.
 
 ## Features
 - Read data from `.dat` and associated binary files.
 - Merge data from different sources like TDMS and DAT files.
 - Export processed data to various formats such as CSV and Parquet.
@@ -54,8 +54,8 @@
 
 - Python >= 3.8
 - pandas
 - numpy
 - nptdms
 
 ## License
-This project is licensed under the MIT License - see the LICENSE.md file for details.
+This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `mesa2_preprocessing-0.1.0/setup.py` & `mesa2_preprocessing-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mesa2_preprocessing',
-    version='0.1.0',
+    version='0.2.0',
     author='Nadir Nadirov',
     author_email='nadirnadirov1999@gmail.com',
-    description='A tool for post-processing MESA2.0 measurement data',
+    description='A tool for pre-processing MESA2.0 measurement data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'pandas>=1.0',
         'numpy>=1.18',
         'nptdms>=0.25'
```


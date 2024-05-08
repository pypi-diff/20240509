# Comparing `tmp/opex_manifest_generator-1.1.7.tar.gz` & `tmp/opex_manifest_generator-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opex_manifest_generator-1.1.7.tar", last modified: Mon May  6 06:55:04 2024, max compression
+gzip compressed data, was "opex_manifest_generator-1.1.8.tar", last modified: Wed May  8 22:42:41 2024, max compression
```

## Comparing `opex_manifest_generator-1.1.7.tar` & `opex_manifest_generator-1.1.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.617000 opex_manifest_generator-1.1.7/
--rw-rw-rw-   0        0        0      124 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/.gitignore
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.7/LICENSE.md
--rw-rw-rw-   0        0        0      701 2024-05-06 06:55:04.583000 opex_manifest_generator-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    21573 2024-05-04 20:51:45.000000 opex_manifest_generator-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 06:55:03.402000 opex_manifest_generator-1.1.7/assets/
--rw-rw-rw-   0        0        0     8271 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/Column Headers.png
--rw-rw-rw-   0        0        0    27359 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/FullName Column.png
--rw-rw-rw-   0        0        0    16064 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/Hash Headers.png
--rw-rw-rw-   0        0        0     4920 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/Identifiers Headers.png
--rw-rw-rw-   0        0        0     2602 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/assets/XML Headers.png
-drwxrwxrwx   0        0        0        0 2024-05-06 06:55:03.688000 opex_manifest_generator-1.1.7/opex_manifest_generator/
--rw-rw-rw-   0        0        0      476 2024-05-04 20:51:45.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/__init__.py
--rw-rw-rw-   0        0        0     6485 2024-05-06 06:50:52.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/cli.py
--rw-rw-rw-   0        0        0      676 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/common.py
--rw-rw-rw-   0        0        0     1025 2024-05-06 06:38:56.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/hash.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.095000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/
--rw-rw-rw-   0        0        0      775 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/DublinCore Template.xml
--rw-rw-rw-   0        0        0     2268 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/EAD Template.xml
--rw-rw-rw-   0        0        0      483 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/GDPR Template.xml
--rw-rw-rw-   0        0        0     2701 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/MODS Template.xml
--rw-rw-rw-   0        0        0    30563 2024-05-06 06:50:43.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/opex_manifest.py
--rw-rw-rw-   0        0        0      313 2024-04-07 11:10:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/pstats_test.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.201000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/
--rw-rw-rw-   0        0        0      389 2023-02-23 12:37:11.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/Opex.xml
--rw-rw-rw-   0        0        0    24938 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx
-drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.505000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/
--rw-rw-rw-   0        0        0    22794 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/dctemplate.xlsx
--rw-rw-rw-   0        0        0    19299 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/eadtemplate.xlsx
--rw-rw-rw-   0        0        0    18662 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx
--rw-rw-rw-   0        0        0    19509 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/modstemplate.xlsx
--rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.7/opex_manifest_generator/test_cli.py
-drwxrwxrwx   0        0        0        0 2024-05-06 06:55:04.557000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/
--rw-rw-rw-   0        0        0      701 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1260 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-06 06:55:02.000000 opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      940 2024-05-06 06:54:04.000000 opex_manifest_generator-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 06:55:04.611000 opex_manifest_generator-1.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 22:42:41.796000 opex_manifest_generator-1.1.8/
+-rw-rw-rw-   0        0        0      124 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.8/.gitignore
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.8/LICENSE.md
+-rw-rw-rw-   0        0        0      701 2024-05-08 22:42:41.626000 opex_manifest_generator-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    21573 2024-05-04 20:51:45.000000 opex_manifest_generator-1.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 22:42:36.549000 opex_manifest_generator-1.1.8/assets/
+-rw-rw-rw-   0        0        0     8271 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.8/assets/Column Headers.png
+-rw-rw-rw-   0        0        0    27359 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.8/assets/FullName Column.png
+-rw-rw-rw-   0        0        0    16064 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.8/assets/Hash Headers.png
+-rw-rw-rw-   0        0        0     4920 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.8/assets/Identifiers Headers.png
+-rw-rw-rw-   0        0        0     2602 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.8/assets/XML Headers.png
+drwxrwxrwx   0        0        0        0 2024-05-08 22:42:37.273000 opex_manifest_generator-1.1.8/opex_manifest_generator/
+-rw-rw-rw-   0        0        0      476 2024-05-04 20:51:45.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/__init__.py
+-rw-rw-rw-   0        0        0     6537 2024-05-06 07:28:39.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/cli.py
+-rw-rw-rw-   0        0        0      676 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/common.py
+-rw-rw-rw-   0        0        0     1025 2024-05-06 06:38:56.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/hash.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:42:39.211000 opex_manifest_generator-1.1.8/opex_manifest_generator/metadata/
+-rw-rw-rw-   0        0        0      775 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/metadata/DublinCore Template.xml
+-rw-rw-rw-   0        0        0     2268 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/metadata/EAD Template.xml
+-rw-rw-rw-   0        0        0      483 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/metadata/GDPR Template.xml
+-rw-rw-rw-   0        0        0     2701 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/metadata/MODS Template.xml
+-rw-rw-rw-   0        0        0    30561 2024-05-06 20:53:58.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/opex_manifest.py
+-rw-rw-rw-   0        0        0      313 2024-04-07 11:10:20.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/pstats_test.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:42:39.892000 opex_manifest_generator-1.1.8/opex_manifest_generator/samples/
+-rw-rw-rw-   0        0        0      389 2023-02-23 12:37:11.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/samples/Opex.xml
+-rw-rw-rw-   0        0        0    24938 2024-04-13 10:14:02.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx
+drwxrwxrwx   0        0        0        0 2024-05-08 22:42:41.176000 opex_manifest_generator-1.1.8/opex_manifest_generator/samples/spreads/
+-rw-rw-rw-   0        0        0    22794 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/samples/spreads/dctemplate.xlsx
+-rw-rw-rw-   0        0        0    19299 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/samples/spreads/eadtemplate.xlsx
+-rw-rw-rw-   0        0        0    18662 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx
+-rw-rw-rw-   0        0        0    19509 2024-04-05 23:28:20.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/samples/spreads/modstemplate.xlsx
+-rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.8/opex_manifest_generator/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-08 22:42:41.452000 opex_manifest_generator-1.1.8/opex_manifest_generator.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-05-08 22:42:30.000000 opex_manifest_generator-1.1.8/opex_manifest_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1260 2024-05-08 22:42:34.000000 opex_manifest_generator-1.1.8/opex_manifest_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 22:42:30.000000 opex_manifest_generator-1.1.8/opex_manifest_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-08 22:42:30.000000 opex_manifest_generator-1.1.8/opex_manifest_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-05-08 22:42:30.000000 opex_manifest_generator-1.1.8/opex_manifest_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-08 22:42:31.000000 opex_manifest_generator-1.1.8/opex_manifest_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      940 2024-05-06 07:30:43.000000 opex_manifest_generator-1.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 22:42:41.780000 opex_manifest_generator-1.1.8/setup.cfg
```

### Comparing `opex_manifest_generator-1.1.7/LICENSE.md` & `opex_manifest_generator-1.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/PKG-INFO` & `opex_manifest_generator-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.7
+Version: 1.1.8
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.7/README.md` & `opex_manifest_generator-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/assets/Column Headers.png` & `opex_manifest_generator-1.1.8/assets/Column Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/assets/FullName Column.png` & `opex_manifest_generator-1.1.8/assets/FullName Column.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/assets/Hash Headers.png` & `opex_manifest_generator-1.1.8/assets/Hash Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/assets/Identifiers Headers.png` & `opex_manifest_generator-1.1.8/assets/Identifiers Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/assets/XML Headers.png` & `opex_manifest_generator-1.1.8/assets/XML Headers.png`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/cli.py` & `opex_manifest_generator-1.1.8/opex_manifest_generator/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,11 +108,12 @@
                           empty_flag = args.remove_empty, 
                           remove_flag = args.remove, 
                           clear_opex_flag = args.clear_opex, 
                           algorithm = args.fixity, 
                           startref = args.start_ref, 
                           export_flag = args.export, 
                           meta_dir_flag = args.disable_meta_dir, 
-                          metadata_flag = args.metadata, 
+                          metadata_flag = args.metadata,
+                          hidden_flag= args.hidden,
                           zip_flag = args.zip, 
                           input = args.input, 
                           output_format = args.output_format).main()
```

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/common.py` & `opex_manifest_generator-1.1.8/opex_manifest_generator/common.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/hash.py` & `opex_manifest_generator-1.1.8/opex_manifest_generator/hash.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/DublinCore Template.xml` & `opex_manifest_generator-1.1.8/opex_manifest_generator/metadata/DublinCore Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/EAD Template.xml` & `opex_manifest_generator-1.1.8/opex_manifest_generator/metadata/EAD Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/metadata/MODS Template.xml` & `opex_manifest_generator-1.1.8/opex_manifest_generator/metadata/MODS Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/opex_manifest.py` & `opex_manifest_generator-1.1.8/opex_manifest_generator/opex_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,15 @@
                         self.identifier.set("type", key_name)
                         self.identifier.text = str(ident)
         except Exception as e:
             print('Error looking up Identifiers')
             print(e)            
     
     def check_opex(self, opex_path: str):
+        opex_path = opex_path + ".opex" 
         if os.path.exists(win_256_check(opex_path)):
             return False
         else:
             return True
 
     def write_opex(self, path: str, opexxml: ET.Element):
         opex_path = str(win_256_check(path)) + ".opex"
@@ -347,15 +348,15 @@
                             if self.metadata_flag in {'e', 'exact'}:
                                 val = self.df.loc[idx, path].values[0]
                             elif self.metadata_flag in {'f', 'flat'}:
                                 val = self.df.loc[idx, name].values[0]
                             if pd.isnull(val):
                                 continue
                             else:
-                                if is_datetime64_any_dtype(val):
+                                if is_datetime64_any_dtype(str(val)):
                                     val = pd.to_datetime(val)
                                     val = datetime.strftime(val, "%Y-%m-%dT%H-%M-%S.00Z")
                         except KeyError as e:
                             print('Key Error: please ensure column header\'s are an exact match...')
                             print(f'Missing Column: {e}')
                             print('Alternatively use flat mode...')
                             time.sleep(3)
@@ -488,44 +489,44 @@
         if self.OMG.autoclass_flag or self.OMG.input:
             self.OMG.generate_opex_properties(self.xmlroot, self.index, 
                                               title = self.title,
                                               description = self.description,
                                               security = self.security)
             if not self.OMG.metadata_flag in {'none', 'n'}:
                 self.xml_descmeta = ET.SubElement(self.xmlroot,f"{{{self.opexns}}}DescriptiveMetadata")
-                self.OMG.generate_descriptive_metadata(self.xmlroot, self.folder_path, idx = self.index)
+                self.OMG.generate_descriptive_metadata(self.xmlroot, idx = self.index)
 
     def filter_directories(self, directory: str):
-        if not self.OMG.hidden_flag:
+        if self.OMG.hidden_flag is False:
             list_directories = sorted([os.path.join(directory, f.name) for f in os.scandir(directory)
                                        if not f.name.startswith('.')
                                        and not bool(os.stat(os.path.join(directory, f.name)).st_file_attributes & stat.FILE_ATTRIBUTE_HIDDEN)
                                        and f.name != 'meta'
                                        and f.name != os.path.basename(__file__)]
                                        , key=str.casefold)
-        else:
+        elif self.OMG.hidden_flag is True:
             list_directories = sorted([os.path.join(directory, f.name) for f in os.scandir(directory) \
                                        if f.name != 'meta' \
                                        and f.name != os.path.basename(__file__)], key=str.casefold)
         return list_directories
         
     def generate_opex_dirs(self, path: str):
         self = OpexDir(self.OMG, path)
         opex_path = os.path.join(os.path.abspath(self.folder_path), os.path.basename(self.folder_path))
+        for f_path in self.filter_directories(path):
+            if f_path.endswith('.opex'):
+                pass
+            elif os.path.isdir(f_path):
+                if not self.ignore:
+                    self.folder = ET.SubElement(self.folders, f"{{{self.opexns}}}Folder")
+                    self.folder.text = str(os.path.basename(f_path))
+                self.generate_opex_dirs(f_path)
+            else:
+                OpexFile(self.OMG, f_path, self.OMG.algorithm)
         if self.OMG.check_opex(opex_path):
-            for f_path in self.filter_directories(path):
-                if f_path.endswith('.opex'):
-                    pass
-                elif os.path.isdir(f_path):
-                    if not self.ignore:
-                        self.folder = ET.SubElement(self.folders, f"{{{self.opexns}}}Folder")
-                        self.folder.text = str(os.path.basename(f_path))
-                    self.generate_opex_dirs(f_path)
-                else:
-                    OpexFile(self.OMG, f_path, self.OMG.algorithm)
             if not self.ignore:
                 for f_path in self.filter_directories(path):
                     if os.path.isfile(f_path):
                         file = ET.SubElement(self.files, f"{{{self.opexns}}}File")
                         if f_path.endswith('.opex'):
                             file.set("type", "metadata")
                         else:
@@ -540,15 +541,15 @@
     def __init__(self, OMG: OpexManifestGenerator, file_path: str, algorithm: str = None, title: str = None, description: str = None, security: str = None):
         self.OMG = OMG
         self.opexns = self.OMG.opexns  
         if file_path.startswith(u'\\\\?\\'):
             self.file_path = file_path.replace(u'\\\\?\\', "")
         else:
             self.file_path = file_path
-        if self.OMG.check_opex(self.file_path + ".opex"):
+        if self.OMG.check_opex(self.file_path):
             if self.OMG.input or self.OMG.autoclass_flag in {"c","catalog","a","accession","b","both","cg","catalog-generic","ag","accession-generic","bg","both-generic"} \
                 or self.OMG.ignore_flag or self.OMG.remove_flag or self.OMG.sourceid_flag \
                 or self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
                     self.index = self.OMG.index_df_lookup(self.file_path)
             elif self.OMG.autoclass_flag is None or self.OMG.autoclass_flag in {"g","generic"}:
                 self.index = None
             if self.OMG.ignore_flag:
@@ -588,13 +589,13 @@
                 if self.OMG.autoclass_flag or self.OMG.input:
                     self.OMG.generate_opex_properties(self.xmlroot, self.index,
                                                       title = self.title,
                                                       description = self.description,
                                                       security = self.security)
                     if not self.OMG.metadata_flag in {'none','n'}:
                         self.xml_descmeta = ET.SubElement(self.xmlroot, f"{{{self.opexns}}}DescriptiveMetadata")
-                        self.OMG.generate_descriptive_metadata(self.xml_descmeta, self.file_path, self.index)
+                        self.OMG.generate_descriptive_metadata(self.xml_descmeta, self.index)
                 opex_path = self.OMG.write_opex(self.file_path, self.xmlroot)
                 if self.OMG.zip_flag:
                     zip_opex(self.file_path, opex_path)
         else:
-            print(f"Opex exists for: {self.file_path}: Avoiding override")
+            print(f"Avoiding override, Opex exists at: {self.file_path}: ")
```

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx` & `opex_manifest_generator-1.1.8/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/dctemplate.xlsx` & `opex_manifest_generator-1.1.8/opex_manifest_generator/samples/spreads/dctemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/eadtemplate.xlsx` & `opex_manifest_generator-1.1.8/opex_manifest_generator/samples/spreads/eadtemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx` & `opex_manifest_generator-1.1.8/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator/samples/spreads/modstemplate.xlsx` & `opex_manifest_generator-1.1.8/opex_manifest_generator/samples/spreads/modstemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/PKG-INFO` & `opex_manifest_generator-1.1.8/opex_manifest_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.7
+Version: 1.1.8
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.7/opex_manifest_generator.egg-info/SOURCES.txt` & `opex_manifest_generator-1.1.8/opex_manifest_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.7/pyproject.toml` & `opex_manifest_generator-1.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 00000030: 746f 6f6c 732d 7363 6d22 5d0d 0a62 7569  tools-scm"]..bui
 00000040: 6c64 2d62 6163 6b65 6e64 203d 2022 7365  ld-backend = "se
 00000050: 7475 7074 6f6f 6c73 2e62 7569 6c64 5f6d  tuptools.build_m
 00000060: 6574 6122 0d0a 0d0a 5b70 726f 6a65 6374  eta"....[project
 00000070: 5d0d 0a6e 616d 6520 3d20 226f 7065 785f  ]..name = "opex_
 00000080: 6d61 6e69 6665 7374 5f67 656e 6572 6174  manifest_generat
 00000090: 6f72 220d 0a76 6572 7369 6f6e 203d 2022  or"..version = "
-000000a0: 312e 312e 3722 0d0a 6175 7468 6f72 7320  1.1.7"..authors 
+000000a0: 312e 312e 3822 0d0a 6175 7468 6f72 7320  1.1.8"..authors 
 000000b0: 3d20 5b0d 0a20 2020 207b 6e61 6d65 3d22  = [..    {name="
 000000c0: 4368 7269 7374 6f70 6865 7220 5072 696e  Christopher Prin
 000000d0: 6365 222c 2065 6d61 696c 3d22 632e 706a  ce", email="c.pj
 000000e0: 2e70 7269 6e63 6540 676d 6169 6c2e 636f  .prince@gmail.co
 000000f0: 6d22 7d0d 0a20 2020 205d 0d0a 6465 7363  m"}..    ]..desc
 00000100: 7269 7074 696f 6e20 3d20 224f 7065 7820  ription = "Opex 
 00000110: 4d61 6e69 6665 7374 2047 656e 6572 6174  Manifest Generat
```


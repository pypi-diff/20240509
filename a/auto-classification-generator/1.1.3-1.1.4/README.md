# Comparing `tmp/auto_classification_generator-1.1.3.tar.gz` & `tmp/auto_classification_generator-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_classification_generator-1.1.3.tar", last modified: Sun Apr 21 19:15:36 2024, max compression
+gzip compressed data, was "auto_classification_generator-1.1.4.tar", last modified: Wed May  8 23:10:32 2024, max compression
```

## Comparing `auto_classification_generator-1.1.3.tar` & `auto_classification_generator-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 19:15:36.621886 auto_classification_generator-1.1.3/
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 auto_classification_generator-1.1.3/LICENSE.md
--rw-rw-rw-   0        0        0      642 2024-04-21 19:15:36.621886 auto_classification_generator-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     8408 2024-04-21 18:05:12.000000 auto_classification_generator-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 19:15:36.567937 auto_classification_generator-1.1.3/auto_classification_generator/
--rw-rw-rw-   0        0        0      451 2024-04-21 18:40:21.000000 auto_classification_generator-1.1.3/auto_classification_generator/__init__.py
--rw-rw-rw-   0        0        0    15384 2024-04-21 18:04:22.000000 auto_classification_generator-1.1.3/auto_classification_generator/classification_generator.py
--rw-rw-rw-   0        0        0     2618 2024-04-21 18:40:30.000000 auto_classification_generator-1.1.3/auto_classification_generator/cli.py
--rw-rw-rw-   0        0        0     2224 2024-03-20 15:06:23.000000 auto_classification_generator-1.1.3/auto_classification_generator/common.py
--rw-rw-rw-   0        0        0      978 2024-04-12 13:13:37.000000 auto_classification_generator-1.1.3/auto_classification_generator/hash.py
--rw-rw-rw-   0        0        0       64 2024-03-23 11:12:41.000000 auto_classification_generator-1.1.3/auto_classification_generator/test_cli.py
-drwxrwxrwx   0        0        0        0 2024-04-21 19:15:36.621886 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/
--rw-rw-rw-   0        0        0      642 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-04-21 19:15:36.000000 auto_classification_generator-1.1.3/auto_classification_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      900 2024-04-21 18:52:54.000000 auto_classification_generator-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 19:15:36.629979 auto_classification_generator-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 23:10:32.288000 auto_classification_generator-1.1.4/
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 auto_classification_generator-1.1.4/LICENSE.md
+-rw-rw-rw-   0        0        0      642 2024-05-08 23:10:32.092000 auto_classification_generator-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8408 2024-04-14 07:44:23.000000 auto_classification_generator-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 23:10:30.678000 auto_classification_generator-1.1.4/auto_classification_generator/
+-rw-rw-rw-   0        0        0      451 2024-05-06 06:53:31.000000 auto_classification_generator-1.1.4/auto_classification_generator/__init__.py
+-rw-rw-rw-   0        0        0    16019 2024-05-08 22:58:25.000000 auto_classification_generator-1.1.4/auto_classification_generator/classification_generator.py
+-rw-rw-rw-   0        0        0     2800 2024-05-08 23:06:56.000000 auto_classification_generator-1.1.4/auto_classification_generator/cli.py
+-rw-rw-rw-   0        0        0     2368 2024-05-06 08:54:16.000000 auto_classification_generator-1.1.4/auto_classification_generator/common.py
+-rw-rw-rw-   0        0        0      978 2024-04-11 18:51:32.000000 auto_classification_generator-1.1.4/auto_classification_generator/hash.py
+-rw-rw-rw-   0        0        0       64 2024-04-13 10:15:57.000000 auto_classification_generator-1.1.4/auto_classification_generator/test_cli.py
+-rw-rw-rw-   0        0        0      474 2024-04-13 10:15:48.000000 auto_classification_generator-1.1.4/auto_classification_generator/test_pstats.py
+drwxrwxrwx   0        0        0        0 2024-05-08 23:10:31.987000 auto_classification_generator-1.1.4/auto_classification_generator.egg-info/
+-rw-rw-rw-   0        0        0      642 2024-05-08 23:10:27.000000 auto_classification_generator-1.1.4/auto_classification_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      657 2024-05-08 23:10:28.000000 auto_classification_generator-1.1.4/auto_classification_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 23:10:27.000000 auto_classification_generator-1.1.4/auto_classification_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-08 23:10:28.000000 auto_classification_generator-1.1.4/auto_classification_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 23:10:28.000000 auto_classification_generator-1.1.4/auto_classification_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-05-08 23:10:28.000000 auto_classification_generator-1.1.4/auto_classification_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      900 2024-05-08 23:03:40.000000 auto_classification_generator-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-08 23:10:32.262000 auto_classification_generator-1.1.4/setup.cfg
```

### Comparing `auto_classification_generator-1.1.3/LICENSE.md` & `auto_classification_generator-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.3/PKG-INFO` & `auto_classification_generator-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_classification_generator
-Version: 1.1.3
+Version: 1.1.4
 Summary: Auto Classification Generator Tool for Archivists
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/auto_classification_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/auto_classification_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `auto_classification_generator-1.1.3/README.md` & `auto_classification_generator-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.3/auto_classification_generator/classification_generator.py` & `auto_classification_generator-1.1.4/auto_classification_generator/classification_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 import os
 import stat
 import pandas as pd
 from datetime import datetime
 import time
 
 class ClassificationGenerator():
-    def __init__(self,
-                 root: str,
-                 output_path: str = os.getcwd(),
-                 prefix: str = None,
-                 accprefix: str = None,
-                 start_ref: int = 1,
-                 fixity: str = None,
-                 empty_flag: bool = False,
-                 skip_flag: bool = False,
-                 accession_flag: bool = False,
-                 meta_dir_flag: bool = True,
-                 hidden_flag: bool = False,
+    def __init__(self, 
+                 root: str, 
+                 output_path: str = os.getcwd(), 
+                 prefix: str = None, 
+                 accprefix: str = None, 
+                 start_ref: int = 1, 
+                 fixity: str = None, 
+                 empty_flag: bool = False, 
+                 skip_flag: bool = False, 
+                 accession_flag: bool = False, 
+                 meta_dir_flag: bool = True, 
+                 hidden_flag: bool = False, 
                  output_format: str = "xlsx"):
 
         self.root = os.path.abspath(root)
         self.root_level = self.root.count(os.sep)
         self.root_path = os.path.dirname(self.root)
         self.output_path = output_path
         self.output_format = output_format
@@ -70,47 +70,46 @@
                                \nTyping any other character will abort the program... \
                                \n\nPlease confirm your choice: ')
         if confirm_delete.lower() != "y":
             print('Aborting...')
             time.sleep(1)
             raise SystemExit()
         empty_dirs = []
-        for dirpath, dirnames, filenames in os.walk(self.root, topdown=False):
+        for dirpath, dirnames, filenames in os.walk(self.root, topdown = False):
             if not any((dirnames, filenames)):
                 empty_dirs.append(dirpath)
                 try:
                     os.rmdir(dirpath)
                     print(f'Removed Directory: {dirpath}')
                 except OSError as e:
                     print(f"Error removing directory '{dirpath}': {e}")
         if empty_dirs:
-            output_txt = define_output_file(self.output_path, self.root, self.meta_dir_flag,
-                                            output_suffix="_EmptyDirectoriesRemoved",output_format="txt")
+            output_txt = define_output_file(self.output_path, self.root, self.meta_dir_flag, 
+                                            output_suffix = "_EmptyDirectoriesRemoved", output_format = "txt")
             export_list_txt(empty_dirs, output_txt)
         else:
             print('No directories removed!')
 
     def filter_directories(self, directory):
         """
         Sorts the list alphabetically and filters out certain files.
         """
         try:
             if not self.hidden_flag:
                 list_directories = sorted([f.name for f in os.scandir(directory)
                                             if not f.name.startswith('.')
-                                            and not bool(os.stat(win_256_check(os.path.join(directory, f.name))).st_file_attributes &
-                                                        stat.FILE_ATTRIBUTE_HIDDEN)
+                                            and not bool(os.stat(win_256_check(os.path.join(directory, f.name))).st_file_attributes & stat.FILE_ATTRIBUTE_HIDDEN)
                                             and not f.name.endswith('.opex')
                                             and f.name != 'meta'
-                                            and f.name != os.path.basename(__file__)], key=str.casefold)
+                                            and f.name != os.path.basename(__file__)], key = str.casefold)
             else:
                 list_directories = sorted([f.name for f in os.scandir(directory)
                                             if not f.name.endswith('.opex')
                                             and f.name != 'meta'
-                                            and f.name != os.path.basename(__file__)], key=str.casefold)
+                                            and f.name != os.path.basename(__file__)], key = str.casefold)
             return list_directories
         except Exception as e:
             print('Failed to Filter')
             print(e)
             raise SystemError()
 
     def parse_directory_dict(self, file_path: str, level: str, ref: int):
@@ -126,25 +125,25 @@
             if self.accession_flag:
                 acc_ref = self.accession_running_number(parse_path)
                 self.accession_list.append(acc_ref)
             if os.path.isdir(file_path):
                 file_type = "Dir"
             else:
                 file_type = "File"
-            class_dict = {'RelativeName': str(parse_path).replace(self.root_path, ""),
-                        'FullName': str(os.path.abspath(parse_path)),
-                        'Basename': os.path.splitext(os.path.basename(file_path))[0],
-                        'Extension': os.path.splitext(file_path)[1],
-                        'Parent': os.path.abspath(os.path.join(os.path.abspath(parse_path), os.pardir)),
-                        'Attribute': file_type,
-                        'Size': file_stats.st_size,
-                        'CreateDate': datetime.fromtimestamp(file_stats.st_ctime),
-                        'ModifiedDate': datetime.fromtimestamp(file_stats.st_mtime),
-                        'AccessDate': datetime.fromtimestamp(file_stats.st_atime),
-                        'Level': level,
+            class_dict = {'RelativeName': str(parse_path).replace(self.root_path, ""), 
+                        'FullName': str(os.path.abspath(parse_path)), 
+                        'Basename': os.path.splitext(os.path.basename(file_path))[0], 
+                        'Extension': os.path.splitext(file_path)[1], 
+                        'Parent': os.path.abspath(os.path.join(os.path.abspath(parse_path), os.pardir)), 
+                        'Attribute': file_type, 
+                        'Size': file_stats.st_size, 
+                        'CreateDate': datetime.fromtimestamp(file_stats.st_ctime), 
+                        'ModifiedDate': datetime.fromtimestamp(file_stats.st_mtime), 
+                        'AccessDate': datetime.fromtimestamp(file_stats.st_atime), 
+                        'Level': level, 
                         'Ref_Section': ref}
             if self.fixity and not os.path.isdir(file_path):
                 hash = HashGenerator(self.fixity).hash_generator(file_path)
                 class_dict.update({"Algorithm": self.fixity, "Hash": hash})
             self.record_list.append(class_dict)
             return class_dict
         except:
@@ -164,36 +163,36 @@
             else:
                 level = directory.count(os.sep) - self.root_level + 1
             for file in list_directory:
                 file_path = win_256_check(os.path.join(directory, file))
                 self.parse_directory_dict(file_path, level, ref)
                 ref = int(ref) + int(1)
                 if os.path.isdir(file_path):
-                    self.list_directories(file_path, ref=1)
+                    self.list_directories(file_path, ref = 1)
         except Exception as e:
             print(e)
             print("Error occurred for directory/file: {}".format(list_directory))
             raise SystemError()
             pass
 
     def init_dataframe(self):
         """
         Lists the directories and forms dicts from the above two functions.
         Looks up and pulls through the Parent row's data to the Child Row.
         Merges the dataframe on itself, Parent is merged 'left' on FullName to pull through the Parent's data
         (lookup is based on File Path's), and unnecessary data is dropped.
         Any errors are turned to 0 and the result are based on the reference loop initialisation.
         """
-        self.parse_directory_dict(file_path=self.root, level=0, ref=0)
+        self.parse_directory_dict(file_path = self.root, level = 0, ref = 0)
         self.list_directories(self.root, self.start_ref)
         self.df = pd.DataFrame(self.record_list)
-        self.df = self.df.merge(self.df[['FullName', 'Ref_Section']], how='left', left_on='Parent',
-                                right_on='FullName')
-        self.df = self.df.drop(['FullName_y'], axis=1)
-        self.df = self.df.rename(columns={'Ref_Section_x': 'Ref_Section', 'Ref_Section_y': 'Parent_Ref',
+        self.df = self.df.merge(self.df[['FullName', 'Ref_Section']], how = 'left', left_on = 'Parent', 
+                                right_on = 'FullName')
+        self.df = self.df.drop(['FullName_y'], axis = 1)
+        self.df = self.df.rename(columns = {'Ref_Section_x': 'Ref_Section', 'Ref_Section_y': 'Parent_Ref', 
                                           'FullName_x': 'FullName'})
         self.df['Parent_Ref'] = self.df['Parent_Ref'].fillna(0)
         self.df = self.df.astype({'Parent_Ref': int})
         self.df.index.name = "Index"
         self.list_loop = self.df[['Ref_Section', 'Parent', 'Level']].values.tolist()
         if self.skip_flag:
             pass
@@ -205,24 +204,24 @@
         """
         Initialises the Reference loop. Sets some of the pre-variables necessary for the loop.
         """
         c = 0
         tot = len(self.list_loop)
         for REF, PARENT, LEVEL in self.list_loop:
             c += 1
-            print(f"Generating Auto Classification for: {c} / {tot}",end="\r")
+            print(f"Generating Auto Classification for: {c} / {tot}", end = "\r")
             TRACK = 1  
-            self.reference_loop(REF,PARENT,TRACK,LEVEL)
+            self.reference_loop(REF, PARENT, TRACK, LEVEL)
 
         self.df['Archive_Reference'] = self.reference_list
         if self.accession_flag:
             self.df['Accession_Reference'] = self.accession_list
         return self.df
 
-    def reference_loop(self, REF, PARENT, TRACK, LEVEL, NEWREF=None):
+    def reference_loop(self, REF, PARENT, TRACK, LEVEL, NEWREF = None):
         """
         The Reference loop works upwards, running an "index lookup" against the parent folder until it reaches the top.
 
         REF is the reference section derived from the list in the list_directories function. [Stays Constant]
         PARENT is the parent folder of the child. [Varies]
         TRACK is an iteration tracker to distinguish between first and later iterations. [Varies]
         LEVEL is the level of the folder, 0 being the root. [Stays Constant]
@@ -278,42 +277,57 @@
                 self.reference_loop(REF, PARENT, TRACK, LEVEL, NEWREF)
 
         except Exception as e:
             print('Passed?')
             print(e)
             pass
 
-    def accession_running_number(self,file_path):
+    def accession_running_number(self, file_path):
         """
         Generates a Running Number / Accession Code, can be set to 3 different "modes", counting Files, Directories or Both
         """
 
-        if self.accession_flag == "File":
+        if self.accession_flag.lower() == "file":
             if os.path.isdir(file_path):
-                accession_ref = self.accession_prefix + "-Dir"
+                if self.accession_prefix:
+                    accession_ref = self.accession_prefix + "-Dir"
+                else: accession_ref = "Dir"
             else:
-                accession_ref = self.accession_prefix + "-" + str(self.accession_count)
+                if self.accession_prefix:
+                    accession_ref = self.accession_prefix + "-" + str(self.accession_count)
+                else:
+                    accession_ref = self.accession_count
                 self.accession_count += 1
-        elif self.accession_flag == "Dir":
+        elif self.accession_flag.lower() == "dir":
             if os.path.isdir(file_path):
-                accession_ref = self.accession_prefix + "-" + str(self.accession_count)
+                if self.accession_prefix:
+                    accession_ref = self.accession_prefix + "-" + str(self.accession_count)
+                else:
+                    accession_ref = self.accession_count
                 self.accession_count += 1
             else:
-                accession_ref = self.accession_prefix + "-File"
-        elif self.accession_flag == "All":
-            accession_ref = self.accession_prefix + "-" + str(self.accession_count)
+                if self.accession_prefix:
+                    accession_ref = self.accession_prefix + "-File"
+                else:
+                    accession_ref = "File"
+        elif self.accession_flag.lower() == "all":
+            if self.accession_prefix:
+                accession_ref = self.accession_prefix + "-" + str(self.accession_count)
+            else:
+                accession_ref = self.accession_count
             self.accession_count += 1
         return accession_ref
 
     def main(self):
         """
         Runs Program :)
         """
-        if self.empty_flag: self.remove_empty_directories()
+        if self.empty_flag:
+            self.remove_empty_directories()
         self.init_dataframe()
-        output_file = define_output_file(self.output_path, self.root, meta_dir_flag=self.meta_dir_flag,
-                                         output_format=self.output_format)
+        output_file = define_output_file(self.output_path, self.root, meta_dir_flag = self.meta_dir_flag, 
+                                         output_format = self.output_format)
         if self.output_format == "xlsx":
-            export_xl(df=self.df, output_filename=output_file)
+            export_xl(df = self.df, output_filename = output_file)
         elif self.output_format == "csv":
-            export_csv(df=self.df, output_filename=output_file)
+            export_csv(df = self.df, output_filename = output_file)
         self.print_running_time()
```

### Comparing `auto_classification_generator-1.1.3/auto_classification_generator/common.py` & `auto_classification_generator-1.1.4/auto_classification_generator/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,62 +6,66 @@
 """
 
 import os
 import time
 import pandas as pd
 import sys
 
-def path_check(path):
+def path_check(path: str):
     if os.path.exists(path):
         pass
-    else: os.makedirs(path)
+    else:
+        os.makedirs(path)
 
-def define_output_file(output_path,output_name,meta_dir_flag=True,output_suffix="_AutoClass",output_format="xlsx"):
+def define_output_file(output_path: str, output_name: str, meta_dir_flag: bool = True, output_suffix: str = "_AutoClass", output_format: str = "xlsx"):
     path_check(output_path)
     if meta_dir_flag:
         path_check(os.path.join(output_path,"meta"))
         output_dir = os.path.join(output_path,"meta",str(os.path.basename(output_name)) + output_suffix + "." + output_format)
-    else: output_dir = os.path.join(output_path,str(os.path.basename(output_name)) + output_suffix + "." + output_format)
+    else:
+        output_dir = os.path.join(output_path,str(os.path.basename(output_name)) + output_suffix + "." + output_format)
     return output_dir
 
-def export_list_txt(txt_list,output_filename):
+def export_list_txt(txt_list: list, output_filename: str):
     try: 
         with open(output_filename,'w') as writer:
             for line in txt_list:
                 writer.write(f"{line}\n")
     except Exception as e:
         print(e)
         print('Waiting 10 Seconds to try again...')
         time.sleep(10)
-        export_list_txt(txt_list,output_filename)
+        export_list_txt(txt_list, output_filename)
     finally:
         print(f"Saved to: {output_filename}")
 
-def export_csv(df,output_filename):
+def export_csv(df: pd.DataFrame, output_filename: str):
     try:
         df['Archive_Reference'] = df['Archive_Reference'].astype('string')
-        df.to_csv(output_filename,sep=",",encoding="utf-8")
+        df.to_csv(output_filename,sep = ",",encoding = "utf-8")
     except Exception as e:
         print(e)
         print('Waiting 10 Seconds to try again...')
         time.sleep(10)
         export_csv(df,output_filename)
     finally:
         print(f"Saved to: {output_filename}")
 
-def export_xl(df,output_filename):
+def export_xl(df: pd.DataFrame, output_filename: str):
     try:
-        with pd.ExcelWriter(output_filename,mode='w') as writer:
+        with pd.ExcelWriter(output_filename,mode = 'w') as writer:
             df.to_excel(writer)
     except Exception as e:
         print(e)
         print('Waiting 10 Seconds to try again...')
         time.sleep(10)
         export_xl(df,output_filename)
     finally:
         print(f"Saved to: {output_filename}")
 
 def win_256_check(path: str):
     if len(path) > 255 and sys.platform == "win32":
-        if path.startswith(u'\\\\?\\'): path = path
-        else: path = u"\\\\?\\" + path
+        if path.startswith(u'\\\\?\\'):
+            path = path
+        else:
+            path = u"\\\\?\\" + path
     return path
```

### Comparing `auto_classification_generator-1.1.3/auto_classification_generator/hash.py` & `auto_classification_generator-1.1.4/auto_classification_generator/hash.py`

 * *Files identical despite different names*

### Comparing `auto_classification_generator-1.1.3/auto_classification_generator.egg-info/PKG-INFO` & `auto_classification_generator-1.1.4/auto_classification_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_classification_generator
-Version: 1.1.3
+Version: 1.1.4
 Summary: Auto Classification Generator Tool for Archivists
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/auto_classification_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/auto_classification_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `auto_classification_generator-1.1.3/auto_classification_generator.egg-info/SOURCES.txt` & `auto_classification_generator-1.1.4/auto_classification_generator.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -3,13 +3,14 @@
 pyproject.toml
 auto_classification_generator/__init__.py
 auto_classification_generator/classification_generator.py
 auto_classification_generator/cli.py
 auto_classification_generator/common.py
 auto_classification_generator/hash.py
 auto_classification_generator/test_cli.py
+auto_classification_generator/test_pstats.py
 auto_classification_generator.egg-info/PKG-INFO
 auto_classification_generator.egg-info/SOURCES.txt
 auto_classification_generator.egg-info/dependency_links.txt
 auto_classification_generator.egg-info/entry_points.txt
 auto_classification_generator.egg-info/requires.txt
 auto_classification_generator.egg-info/top_level.txt
```

### Comparing `auto_classification_generator-1.1.3/pyproject.toml` & `auto_classification_generator-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2261 7574 6f5f 636c  .name = "auto_cl
 00000070: 6173 7369 6669 6361 7469 6f6e 5f67 656e  assification_gen
 00000080: 6572 6174 6f72 220d 0a76 6572 7369 6f6e  erator"..version
-00000090: 203d 2022 312e 312e 3322 0d0a 6175 7468   = "1.1.3"..auth
+00000090: 203d 2022 312e 312e 3422 0d0a 6175 7468   = "1.1.4"..auth
 000000a0: 6f72 7320 3d20 5b0d 0a20 2020 207b 6e61  ors = [..    {na
 000000b0: 6d65 3d22 4368 7269 7374 6f70 6865 7220  me="Christopher 
 000000c0: 5072 696e 6365 222c 2065 6d61 696c 3d22  Prince", email="
 000000d0: 632e 706a 2e70 7269 6e63 6540 676d 6169  c.pj.prince@gmai
 000000e0: 6c2e 636f 6d22 7d0d 0a20 2020 205d 0d0a  l.com"}..    ]..
 000000f0: 6465 7363 7269 7074 696f 6e20 3d20 2241  description = "A
 00000100: 7574 6f20 436c 6173 7369 6669 6361 7469  uto Classificati
```


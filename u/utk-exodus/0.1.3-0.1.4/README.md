# Comparing `tmp/utk_exodus-0.1.3.tar.gz` & `tmp/utk_exodus-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utk_exodus-0.1.3.tar", max compression
+gzip compressed data, was "utk_exodus-0.1.4.tar", max compression
```

## Comparing `utk_exodus-0.1.3.tar` & `utk_exodus-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     2575 2024-05-08 21:11:48.505135 utk_exodus-0.1.3/README.md
--rw-r--r--   0        0        0      576 2024-05-08 18:41:24.522141 utk_exodus-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      440 2024-05-08 14:55:57.119783 utk_exodus-0.1.3/utk_exodus/__init__.py
--rw-r--r--   0        0        0       43 2024-05-08 14:32:31.650721 utk_exodus-0.1.3/utk_exodus/controller/__init__.py
--rw-r--r--   0        0        0     4596 2024-05-08 21:37:32.451209 utk_exodus-0.1.3/utk_exodus/controller/controller.py
--rw-r--r--   0        0        0       31 2024-05-07 18:16:58.412662 utk_exodus-0.1.3/utk_exodus/curate/__init__.py
--rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.3/utk_exodus/curate/curate.py
--rw-r--r--   0        0        0     3943 2024-05-08 21:19:12.996464 utk_exodus-0.1.3/utk_exodus/exodus.py
--rw-r--r--   0        0        0       32 2024-05-08 12:26:21.007671 utk_exodus-0.1.3/utk_exodus/fedora/__init__.py
--rw-r--r--   0        0        0     1256 2024-05-08 21:08:02.300387 utk_exodus-0.1.3/utk_exodus/fedora/fedora.py
--rw-r--r--   0        0        0       33 2024-04-30 19:26:23.807597 utk_exodus-0.1.3/utk_exodus/finder/__init__.py
--rw-r--r--   0        0        0    18718 2024-05-05 21:13:01.677173 utk_exodus-0.1.3/utk_exodus/finder/finder.py
--rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.3/utk_exodus/metadata/__init__.py
--rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.3/utk_exodus/metadata/base/__init__.py
--rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.3/utk_exodus/metadata/base/base.py
--rw-r--r--   0        0        0    39221 2024-05-06 19:12:21.699513 utk_exodus-0.1.3/utk_exodus/metadata/metadata.py
--rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.3/utk_exodus/risearch/__init__.py
--rw-r--r--   0        0        0     8833 2024-05-08 15:14:24.860576 utk_exodus-0.1.3/utk_exodus/risearch/risearch.py
--rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.3/utk_exodus/validate/__init__.py
--rw-r--r--   0        0        0     6236 2024-05-08 21:38:20.027155 utk_exodus-0.1.3/utk_exodus/validate/validate.py
--rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 utk_exodus-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2575 2024-05-08 21:11:48.505135 utk_exodus-0.1.4/README.md
+-rw-r--r--   0        0        0      654 2024-05-09 12:54:40.198668 utk_exodus-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      440 2024-05-08 14:55:57.119783 utk_exodus-0.1.4/utk_exodus/__init__.py
+-rw-r--r--   0        0        0     2387 2022-10-30 16:46:31.391736 utk_exodus-0.1.4/utk_exodus/config/samvera_default.yml
+-rw-r--r--   0        0        0    12260 2024-05-06 16:36:47.872904 utk_exodus-0.1.4/utk_exodus/config/utk_dc.yml
+-rw-r--r--   0        0        0    11044 2024-05-06 16:37:06.967592 utk_exodus-0.1.4/utk_exodus/config/utk_dc_no_uris.yml
+-rw-r--r--   0        0        0     7824 2024-05-06 16:36:57.261544 utk_exodus-0.1.4/utk_exodus/config/utk_no_uris_no_names.yml
+-rw-r--r--   0        0        0       43 2024-05-08 14:32:31.650721 utk_exodus-0.1.4/utk_exodus/controller/__init__.py
+-rw-r--r--   0        0        0     4493 2024-05-09 12:53:43.841673 utk_exodus-0.1.4/utk_exodus/controller/controller.py
+-rw-r--r--   0        0        0       31 2024-05-07 18:16:58.412662 utk_exodus-0.1.4/utk_exodus/curate/__init__.py
+-rw-r--r--   0        0        0     3927 2024-05-07 19:23:07.831658 utk_exodus-0.1.4/utk_exodus/curate/curate.py
+-rw-r--r--   0        0        0     4049 2024-05-09 12:53:35.105919 utk_exodus-0.1.4/utk_exodus/exodus.py
+-rw-r--r--   0        0        0       32 2024-05-08 12:26:21.007671 utk_exodus-0.1.4/utk_exodus/fedora/__init__.py
+-rw-r--r--   0        0        0     1256 2024-05-08 21:08:02.300387 utk_exodus-0.1.4/utk_exodus/fedora/fedora.py
+-rw-r--r--   0        0        0       33 2024-04-30 19:26:23.807597 utk_exodus-0.1.4/utk_exodus/finder/__init__.py
+-rw-r--r--   0        0        0    18718 2024-05-05 21:13:01.677173 utk_exodus-0.1.4/utk_exodus/finder/finder.py
+-rw-r--r--   0        0        0      640 2024-05-06 19:12:23.968154 utk_exodus-0.1.4/utk_exodus/metadata/__init__.py
+-rw-r--r--   0        0        0      135 2024-04-30 21:46:50.224208 utk_exodus-0.1.4/utk_exodus/metadata/base/__init__.py
+-rw-r--r--   0        0        0     1280 2024-04-30 21:46:50.195943 utk_exodus-0.1.4/utk_exodus/metadata/base/base.py
+-rw-r--r--   0        0        0    39221 2024-05-08 23:29:50.024088 utk_exodus-0.1.4/utk_exodus/metadata/metadata.py
+-rw-r--r--   0        0        0       75 2024-05-01 12:54:48.901975 utk_exodus-0.1.4/utk_exodus/risearch/__init__.py
+-rw-r--r--   0        0        0     8833 2024-05-08 15:14:24.860576 utk_exodus-0.1.4/utk_exodus/risearch/risearch.py
+-rw-r--r--   0        0        0       71 2024-05-06 19:50:10.979729 utk_exodus-0.1.4/utk_exodus/validate/__init__.py
+-rw-r--r--   0        0        0     6236 2024-05-08 21:38:20.027155 utk_exodus-0.1.4/utk_exodus/validate/validate.py
+-rw-r--r--   0        0        0     3473 1970-01-01 00:00:00.000000 utk_exodus-0.1.4/PKG-INFO
```

### Comparing `utk_exodus-0.1.3/README.md` & `utk_exodus-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.3/utk_exodus/controller/controller.py` & `utk_exodus-0.1.4/utk_exodus/controller/controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,113 +4,93 @@
 import shutil
 from utk_exodus.finder import FileOrganizer
 from utk_exodus.fedora import FedoraObject
 from utk_exodus.curate import FileCurator
 from utk_exodus.metadata import MetadataMapping
 from utk_exodus.risearch import ResourceIndexSearch
 from utk_exodus.validate import ValidateMigration
+from pathlib import Path
 
 
 class InterfaceController:
     def __init__(self, config, output, remote, total_size):
-        self.config = config
+        self.config = self.__load_config(config)
         self.output = output
         self.remote = remote
         self.total_size = total_size
 
+    @staticmethod
+    def __load_config(config):
+        configs = {
+            "utk_dc": "utk_dc.yml",
+            "samvera": "samvera_default.yml",
+            "utk_dc_no_uris": "utk_dc_no_uris.yml",
+            "utk_dc_no_uris_or_names": "utk_no_uris_no_names.yml",
+        }
+        config_path = Path(__file__).parent / "../config"
+        return config_path / configs.get(config)
+
     def __curate_filesets_and_attachments(self):
         click.echo(
             click.style(
-                "Curating filesets and attachments ...",
-                fg='magenta',
-                bold=True
+                "Curating filesets and attachments ...", fg="magenta", bold=True
             )
         )
         curator = FileCurator(f"{self.output}/{self.output.split('/')[-1]}.csv")
         curator.write_files_and_attachments_only(
             f"{self.output}/{self.output.split('/')[-1]}.csv_filesheets_and_attachments_only.csv",
             attachments_per_sheet=int(self.total_size),
             multi_sheets="multi",
         )
         curator.write_works_and_collections_only(
             f"{self.output}/{self.output.split('/')[-1]}_works_and_collections_only.csv"
         )
         return
 
     def __generate_metadata_sheet(self, path):
-        click.echo(
-            click.style(
-                "Generating metadata sheet ...",
-                fg='green',
-                bold=True
-            )
-        )
+        click.echo(click.style("Generating metadata sheet ...", fg="green", bold=True))
         os.makedirs(self.output, exist_ok=True)
         metadata = MetadataMapping(self.config, path)
         os.makedirs("tmp", exist_ok=True)
         metadata.write_csv("tmp/works.csv")
         return
 
     def __get_mods(self, collection, work_type):
-        click.echo(
-            click.style(
-                "Finding MODS files ...",
-                fg='red',
-                bold=True
-            )
-        )
+        click.echo(click.style("Finding MODS files ...", fg="red", bold=True))
         risearch = ResourceIndexSearch().get_works_based_on_type_and_collection(
             work_type, collection
         )
         return risearch
 
     def __grab_file_info(self):
-        click.echo(
-            click.style(
-                "Grabbing file info ...",
-                fg='yellow',
-                bold=True
-            )
-        )
+        click.echo(click.style("Grabbing file info ...", fg="yellow", bold=True))
         x = FileOrganizer("tmp/works.csv", ["filesets", "attachments"], self.remote)
         x.write_csv(f"{self.output}/{self.output.split('/')[-1]}.csv")
         r = requests.get(
             "https://raw.githubusercontent.com/utkdigitalinitiatives/m3_profiles/main/maps/utk.yml"
         )
         with open("tmp/m3.yml", "wb") as f:
             f.write(r.content)
         return
 
     def __validate_import(self):
-        click.echo(
-            click.style(
-                "Validating import ...",
-                fg='blue',
-                bold=True
-            )
-        )
+        click.echo(click.style("Validating import ...", fg="blue", bold=True))
         validator = ValidateMigration(
             profile="tmp/m3.yml",
             migration_sheet=f"{self.output}/{self.output.split('/')[-1]}.csv",
         )
         validator.iterate()
         return
 
     def build_import_from_directory(self, path):
         self.__generate_metadata_sheet(path)
         self.__grab_file_info()
         self.__validate_import()
         self.__curate_filesets_and_attachments()
-        click.echo(
-            click.style(
-                "Done ...",
-                fg='cyan',
-                bold=True
-            )
-        )
+        click.echo(click.style("Done ...", fg="cyan", bold=True))
         return
 
     def download_mods(self, collection, work_type):
         mods = self.__get_mods(collection, work_type)
         os.makedirs("tmp", exist_ok=True)
         os.makedirs("tmp/mods_downloads", exist_ok=True)
         os.makedirs("tmp/mods_downloads/current_collection", exist_ok=True)
@@ -127,15 +107,9 @@
                 dsid="MODS", output="tmp/mods_downloads/current_collection"
             )
         self.__generate_metadata_sheet("tmp/mods_downloads/current_collection")
         shutil.rmtree("tmp/mods_downloads/current_collection")
         self.__grab_file_info()
         self.__validate_import()
         self.__curate_filesets_and_attachments()
-        click.echo(
-            click.style(
-                "Done ...",
-                fg='cyan',
-                bold=True
-            )
-        )
+        click.echo(click.style("Done ...", fg="cyan", bold=True))
         return
```

### Comparing `utk_exodus-0.1.3/utk_exodus/curate/curate.py` & `utk_exodus-0.1.4/utk_exodus/curate/curate.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.3/utk_exodus/exodus.py` & `utk_exodus-0.1.4/utk_exodus/exodus.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     pass
 
 
 @cli.command("works", help="Create import sheet for works with metadata.")
 @click.option(
     "--config",
     "-c",
-    default="data/utk_dc.yml",
+    default="config/utk_dc.yml",
     help="Path to the configuration file for metadata mapping.",
 )
 @click.option(
     "--path",
     "-p",
     required=True,
     help="Path to the directory containing the metadata files.",
@@ -76,30 +76,31 @@
     x.write_csv(files_sheet)
 
 
 @cli.command("works_and_files", help="Create import sheet with works and files.")
 @click.option(
     "--config",
     "-c",
-    default="data/utk_dc.yml",
-    help="Path to the configuration file for metadata mapping.",
+    default="utk_dc",
+    type=click.Choice(
+        ["utk_dc", "samvera", "utk_dc_no_uris", "utk_dc_no_uris_or_names"],
+        case_sensitive=False,
+    ),
+    help="The configuration you want to use. By default, utk_dc.",
 )
 @click.option(
     "--collection",
     "-l",
-    help="Specify the collection you want to download metadata for."
+    help="Specify the collection you want to download metadata for.",
 )
 @click.option(
     "--model",
     "-m",
-    type=click.Choice(
-        ['book', 'image', 'pdf', 'audio', 'video'],
-        case_sensitive=False
-    ),
-    help="The model you want to download metadata for."
+    type=click.Choice(["book", "image", "pdf", "audio", "video"], case_sensitive=False),
+    help="The model you want to download metadata for.",
 )
 @click.option(
     "--path",
     "-p",
     help="Path to the directory containing the metadata files.",
 )
 @click.option(
@@ -117,23 +118,25 @@
 @click.option(
     "--total_size",
     "-t",
     help="Specify maximum number of attachments and filesets per sheet.",
     default=800,
 )
 def works_and_files(
-        collection: str,
-        config: str,
-        model: str,
-        path: str,
-        output: str,
-        remote: str,
-        total_size: int
+    collection: str,
+    config: str,
+    model: str,
+    path: str,
+    output: str,
+    remote: str,
+    total_size: int,
 ) -> None:
     if model and collection:
         interface = InterfaceController(config, output, remote, total_size)
         interface.download_mods(collection, model)
     elif path:
         interface = InterfaceController(config, output, remote, total_size)
         interface.build_import_from_directory(path)
     else:
-        print("You must specify either a path to a directory or both a collection and model.")
+        print(
+            "You must specify either a path to a directory or both a collection and model."
+        )
```

### Comparing `utk_exodus-0.1.3/utk_exodus/fedora/fedora.py` & `utk_exodus-0.1.4/utk_exodus/fedora/fedora.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.3/utk_exodus/finder/finder.py` & `utk_exodus-0.1.4/utk_exodus/finder/finder.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.3/utk_exodus/metadata/__init__.py` & `utk_exodus-0.1.4/utk_exodus/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.3/utk_exodus/metadata/base/base.py` & `utk_exodus-0.1.4/utk_exodus/metadata/base/base.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.3/utk_exodus/metadata/metadata.py` & `utk_exodus-0.1.4/utk_exodus/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.3/utk_exodus/risearch/risearch.py` & `utk_exodus-0.1.4/utk_exodus/risearch/risearch.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.3/utk_exodus/validate/validate.py` & `utk_exodus-0.1.4/utk_exodus/validate/validate.py`

 * *Files identical despite different names*

### Comparing `utk_exodus-0.1.3/PKG-INFO` & `utk_exodus-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utk-exodus
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool for building import sheets from UTK legacy systems
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```


# Comparing `tmp/module_qc_database_tools-2.2.8rc1.tar.gz` & `tmp/module_qc_database_tools-2.2.8rc2.tar.gz`

## Comparing `module_qc_database_tools-2.2.8rc1.tar` & `module_qc_database_tools-2.2.8rc2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/.env.template
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/.gitlab-ci.yml
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/ci/pre-commit-update.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/docs/.gitkeep
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/__init__.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/_version.py
--rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/chip_config_api.py
--rw-r--r--   0        0        0    26057 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/core.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/utils.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/__main__.py
--rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/generate_yarr_config.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/main.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/register_component.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/data/componentConfigs.json
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/data/YARR/chip_template.json
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tests/test_cli.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tests/test_config_api.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tests/test_package.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/tests/test_utils.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/LICENSE
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/README.md
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/pyproject.toml
--rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc1/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/.env.template
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/docs/.gitkeep
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/__init__.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/_version.py
+-rw-r--r--   0        0        0    11697 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/chip_config_api.py
+-rw-r--r--   0        0        0    26057 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/core.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/utils.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/cli/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/cli/__main__.py
+-rw-r--r--   0        0        0     6796 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/cli/generate_yarr_config.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/cli/main.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/cli/register_component.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/data/componentConfigs.json
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/data/YARR/chip_template.json
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/tests/test_cli.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/tests/test_config_api.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/tests/test_package.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/tests/test_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/LICENSE
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/README.md
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/pyproject.toml
+-rw-r--r--   0        0        0     6347 2020-02-02 00:00:00.000000 module_qc_database_tools-2.2.8rc2/PKG-INFO
```

### Comparing `module_qc_database_tools-2.2.8rc1/.gitlab-ci.yml` & `module_qc_database_tools-2.2.8rc2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/.pre-commit-config.yaml` & `module_qc_database_tools-2.2.8rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/tbump.toml` & `module_qc_database_tools-2.2.8rc2/tbump.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2232 2e32 2e38 7263 3122 0a0a  t = "2.2.8rc1"..
+00000010: 7420 3d20 2232 2e32 2e38 7263 3222 0a0a  t = "2.2.8rc2"..
 00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
 00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
 00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
 00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
 00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
 00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
 00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
@@ -15,15 +15,15 @@
 000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
 000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
 00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
 00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
 00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
 00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
 00000140: 2242 756d 7020 7665 7273 696f 6e3a 2032  "Bump version: 2
-00000150: 2e32 2e38 7263 3120 e286 9220 7b6e 6577  .2.8rc1 ... {new
+00000150: 2e32 2e38 7263 3220 e286 9220 7b6e 6577  .2.8rc2 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
```

### Comparing `module_qc_database_tools-2.2.8rc1/ci/pre-commit-update.sh` & `module_qc_database_tools-2.2.8rc2/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/__init__.py` & `module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/chip_config_api.py` & `module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/chip_config_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import pickle
 from typing import Optional
 
 import gridfs
 from bson.objectid import ObjectId
 from jsondiff import diff
 
+from module_qc_database_tools.utils import get_chip_type_from_config
+
 log = logging.getLogger(__name__)
 
 
 class ChipConfigAPI:
     """
     A class representing a JSON configuration stored in MongoDB, with revision history.
     """
@@ -148,35 +150,39 @@
 
             filesystem = gridfs.GridFS(self.client.localdb)
 
             data = filesystem.get(pixcfg_id).read()
 
             pixcfg = pickle.load(io.BytesIO(data))
 
-            config_data.get("RD53B").update({"PixelConfig": pixcfg})
+            config_data.get(get_chip_type_from_config(config_data)).update(
+                {"PixelConfig": pixcfg}
+            )
 
         return config_data
 
     def commit(self, config_id, fe_cfg, message=""):
         """
         Commit the config for a given commit_id with some message.
         """
-        pixelcfg = fe_cfg.get("RD53B").get("PixelConfig")
+        pixelcfg = fe_cfg.get(get_chip_type_from_config(fe_cfg)).get("PixelConfig")
 
         keys_to_remove = []
 
         is_pixelcfg_revised = None
 
         if pixelcfg is not None:
             log.info("pickling pixelcfg...")
             binary = pickle.dumps(pixelcfg)
 
             keys_to_remove = [
                 var
-                for var, contents in fe_cfg.get("RD53B").items()
+                for var, contents in fe_cfg.get(
+                    get_chip_type_from_config(fe_cfg)
+                ).items()
                 if var not in ["GlobalConfig", "Parameter"]
             ]
 
             filesystem = gridfs.GridFS(self.client.localdb)
 
             md5 = hashlib.md5(binary).hexdigest()
 
@@ -196,15 +202,18 @@
                 is_pixelcfg_revised = True
 
         else:
             log.info("pixelcfg is None, skipping pickling")
             pixelcfg_doc = None
             is_pixelcfg_revised = True
 
-        _ = [fe_cfg.get("RD53B").pop(key) for key in keys_to_remove]
+        _ = [
+            fe_cfg.get(get_chip_type_from_config(fe_cfg)).pop(key)
+            for key in keys_to_remove
+        ]
 
         config = self.database.fe_configs.find_one({"_id": ObjectId(config_id)})
         previous_revision_id = config.get("current_revision_id")
 
         # Compute the diff between the previous and new configuration
         if previous_revision_id is None:
             the_diff = fe_cfg
```

### Comparing `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/core.py` & `module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/core.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/utils.py` & `module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -62,7 +62,24 @@
 
     if serial_number[7] in ["1", "2"]:
         return "RD53B"
     if serial_number[7] == "3":
         return "ITKPIXV2"
     log.exception("Invalid serial number: %s", serial_number)
     raise ValueError()
+
+
+def get_chip_type_from_config(config):
+    """
+    Get chip type from keyword in chip config
+    """
+    chiptype = ""
+    try:
+        chiptype = next(iter(config.keys()))
+    except IndexError:
+        log.error("One of your chip configuration files is empty")
+
+    if chiptype not in {"RD53B", "ITKPIXV2"}:
+        log.warning(
+            "Chip name in configuration not one of expected chip names (RD53B or ITKPIXV2)"
+        )
+    return chiptype
```

### Comparing `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/generate_yarr_config.py` & `module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/cli/generate_yarr_config.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/main.py` & `module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/cli/register_component.py` & `module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/cli/register_component.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/src/module_qc_database_tools/data/componentConfigs.json` & `module_qc_database_tools-2.2.8rc2/src/module_qc_database_tools/data/componentConfigs.json`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/tests/test_cli.py` & `module_qc_database_tools-2.2.8rc2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/tests/test_config_api.py` & `module_qc_database_tools-2.2.8rc2/tests/test_config_api.py`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/.gitignore` & `module_qc_database_tools-2.2.8rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/LICENSE` & `module_qc_database_tools-2.2.8rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/README.md` & `module_qc_database_tools-2.2.8rc2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Module QC Database Tools v2.2.8rc1
+# Module QC Database Tools v2.2.8rc2
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

### Comparing `module_qc_database_tools-2.2.8rc1/pyproject.toml` & `module_qc_database_tools-2.2.8rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-2.2.8rc1/PKG-INFO` & `module_qc_database_tools-2.2.8rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: module-qc-database-tools
-Version: 2.2.8rc1
+Version: 2.2.8rc2
 Summary: Python wrapper to interface with LocalDB and Production DB for common tasks for pixel modules.
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>, Elisabetta Pianori <elisabetta.pianori@cern.ch>, Lingxin Meng <lingxin.meng@cern.ch>
 License: Copyright (c) 2022 ATLAS ITk Pixel Modules
@@ -50,15 +50,15 @@
 Requires-Dist: pyarrow
 Requires-Dist: pymongo
 Requires-Dist: rich
 Requires-Dist: typer
 Requires-Dist: urllib3<2,>=1.26.11; 'el7.x86_64' in platform_release
 Description-Content-Type: text/markdown
 
-# Module QC Database Tools v2.2.8rc1
+# Module QC Database Tools v2.2.8rc2
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```


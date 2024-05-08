# Comparing `tmp/package_auto_assembler-0.1.1.tar.gz` & `tmp/package_auto_assembler-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "package_auto_assembler-0.1.1.tar", last modified: Sat Apr 27 22:44:55 2024, max compression
+gzip compressed data, was "package_auto_assembler-0.1.2.tar", last modified: Wed May  8 22:15:05 2024, max compression
```

## Comparing `package_auto_assembler-0.1.1.tar` & `package_auto_assembler-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:55.025755 package_auto_assembler-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-27 22:41:42.000000 package_auto_assembler-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-04-27 22:44:55.025755 package_auto_assembler-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-27 22:41:42.000000 package_auto_assembler-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:55.025755 package_auto_assembler-0.1.1/package_auto_assembler/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:44:50.000000 package_auto_assembler-0.1.1/package_auto_assembler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59120 2024-04-27 22:44:50.000000 package_auto_assembler-0.1.1/package_auto_assembler/package_auto_assembler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-27 22:44:54.000000 package_auto_assembler-0.1.1/package_auto_assembler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:44:55.025755 package_auto_assembler-0.1.1/package_auto_assembler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-04-27 22:44:54.000000 package_auto_assembler-0.1.1/package_auto_assembler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-27 22:44:54.000000 package_auto_assembler-0.1.1/package_auto_assembler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:44:54.000000 package_auto_assembler-0.1.1/package_auto_assembler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-27 22:44:54.000000 package_auto_assembler-0.1.1/package_auto_assembler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-27 22:44:54.000000 package_auto_assembler-0.1.1/package_auto_assembler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:44:55.025755 package_auto_assembler-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-08 22:10:48.000000 package_auto_assembler-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26182 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-08 22:10:48.000000 package_auto_assembler-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/package_auto_assembler/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:14:32.000000 package_auto_assembler-0.1.2/package_auto_assembler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61558 2024-05-08 22:14:32.000000 package_auto_assembler-0.1.2/package_auto_assembler/package_auto_assembler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 22:15:04.000000 package_auto_assembler-0.1.2/package_auto_assembler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26182 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 22:15:05.000000 package_auto_assembler-0.1.2/package_auto_assembler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:15:05.329915 package_auto_assembler-0.1.2/setup.cfg
```

### Comparing `package_auto_assembler-0.1.1/LICENSE` & `package_auto_assembler-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `package_auto_assembler-0.1.1/PKG-INFO` & `package_auto_assembler-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package_auto_assembler
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,17 @@
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
 
 
 
 ```python
-from package_auto_assembler import (VersionHandler, \
+import sys
+sys.path.append('../')
+from python_modules.package_auto_assembler import (VersionHandler, \
     ImportMappingHandler, RequirementsHandler, MetadataHandler, \
         LocalDependaciesHandler, LongDocHandler, SetupDirHandler, \
             ReleaseNotesHandler, PackageAutoAssembler)
 ```
 
 ## Usage examples
 
@@ -163,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-04-27 22:44:51</td>
+      <td>2024-05-08 22:14:33</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-04-27 22:44:51</td>
+      <td>2024-05-08 22:14:33</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-04-27 22:44:51</td>
+      <td>2024-05-08 22:14:33</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -344,14 +346,82 @@
 
 
 
     ['### example_module.py', 'attrs>=22.2.0']
 
 
 
+#### Audit dependencies
+
+
+```python
+rh.check_vulnerabilities(
+    # optional if ran extract_requirements() before
+    requirements_list = None,
+    raise_error = True
+)
+```
+
+    No known vulnerabilities found
+    
+
+
+    
+
+
+
+```python
+rh.vulnerabilities
+```
+
+
+
+
+    []
+
+
+
+
+```python
+try:
+    rh.check_vulnerabilities(
+        # optional if ran extract_requirements() before
+        requirements_list = ['attrs>=22.2.0', 'pandas', 'hnswlib==0.7.0'],
+        raise_error = True
+    )
+except Exception as e:
+    print(f"Error: {e}")
+```
+
+    Found 1 known vulnerability in 1 package
+    
+
+
+    Name    Version ID                  Fix Versions
+    ------- ------- ------------------- ------------
+    hnswlib 0.7.0   GHSA-xwc8-rf6m-xr86
+    
+    Error: Found vulnerabilities, resolve them or ignore check to move forwards!
+
+
+
+```python
+rh.vulnerabilities
+```
+
+
+
+
+    [{'name': 'hnswlib',
+      'version': '0.7.0',
+      'id': 'GHSA-xwc8-rf6m-xr86',
+      'fix_versions': None}]
+
+
+
 #### Save requirements to a file
 
 
 ```python
 rh.write_requirements_file(
     # optional/required later
     module_name = 'example_module',
@@ -686,15 +756,16 @@
                     'Programming Language :: Python :: 3.11',
                     'License :: OSI Approved :: MIT License',
                     'Topic :: Scientific/Engineering'],
     requirements_list = [],
     execute_readme_notebook = True,
     python_version = "3.8",
     version_increment_type = "patch",
-    default_version = "0.0.1"
+    default_version = "0.0.1",
+    check_vulnerabilities = True
 )
 ```
 
 #### Add metadata from module
 
 
 ```python
@@ -757,38 +828,45 @@
                         'flask': 'Flask',
                         'stdlib_list': 'stdlib-list',
                         'sklearn': 'scikit-learn',
                         'yaml': 'pyyaml'}
 )
 ```
 
-#### Make README out of example notebook
+    No known vulnerabilities found
+    
 
 
-```python
-paa.add_readme(
-    # optional
-    example_notebook_path = "../tests/package_auto_assembler/example_module.ipynb",
-    output_path = "./example_module/README.md",
-    execute_notebook=False,
-)
-```
+    
+
 
 
 ```python
 paa.requirements_list
 ```
 
 
 
 
     ['### example_module.py', 'attrs>=22.2.0']
 
 
 
+#### Make README out of example notebook
+
+
+```python
+paa.add_readme(
+    # optional
+    example_notebook_path = "../tests/package_auto_assembler/example_module.ipynb",
+    output_path = "./example_module/README.md",
+    execute_notebook=False,
+)
+```
+
 #### Prepare setup file
 
 
 ```python
 paa.prep_setup_file(
     # optional
     metadata = {'author': 'Kyrylo Mordan',
```

### Comparing `package_auto_assembler-0.1.1/README.md` & `package_auto_assembler-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 It provides a method to output various types of lines and headers, with customizable message and line lengths.
 The purpose is to be integrated into other classes that also use logger.
 
 [module](python_modules/gridlooper.py) | [usage](docs/gridlooper.md) | [drawio: -flow](docs/gridlooper-flow.png) | [![PyPiVersion](https://img.shields.io/pypi/v/gridlooper)](https://pypi.org/project/gridlooper/) - Grid Looper
 
 A tool to run experiments based on defined grid and function with single iteration.
 
-[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
+[module](python_modules/package_auto_assembler.py) | [usage](docs/package_auto_assembler.md) | [drawio: -flow](docs/package_auto_assembler-flow.png) | [drawio: -usage](docs/package_auto_assembler-usage.png) | [release notes](release_notes/package_auto_assembler.md) | [![PyPiVersion](https://img.shields.io/pypi/v/package-auto-assembler)](https://pypi.org/project/package-auto-assembler/) - Package Auto Assembler
 
 This tool is meant to streamline creation of single module packages.
 Its purpose is to automate as many aspects of python package creation as possible,
 to shorten a development cycle of reusable components, maintain certain standard of quality
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
@@ -44,15 +44,15 @@
 with a use of more expensive, slower or simply no-existant method.
 
 [module](python_modules/google_drive_support.py) - Google Drive API Utilities Module
 
 This module provides a set of functions for interacting with the Google Drive API.
 It allows you to authenticate with the API, upload, download, and manage files and folders in Google Drive.
 
-[module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameter frame
+[module](python_modules/parameterframe.py) | [usage](docs/parameterframe.md) | [drawio: -flow](docs/parameterframe-flow.png) | [drawio: -schema](docs/parameterframe-schema.png) | [drawio: -usage](docs/parameterframe-usage.png) | [release notes](release_notes/parameterframe.md) | [![PyPiVersion](https://img.shields.io/pypi/v/parameterframe)](https://pypi.org/project/parameterframe/) - Parameterframe
 
 The module provides an interface for managing solution parameters.
 It allows for the structured storage and retrieval of parameter sets from a database.
 
 [module](python_modules/comparisonframe.py) | [usage](docs/comparisonframe.md) | [plantuml](docs/comparisonframe_plantuml.png) - Comparison Frame
 
 Designed to automate and streamline the process of comparing textual data, particularly focusing on various metrics
```

### Comparing `package_auto_assembler-0.1.1/package_auto_assembler/package_auto_assembler.py` & `package_auto_assembler-0.1.2/package_auto_assembler/package_auto_assembler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import pandas as pd #==2.1.1
 import yaml
 import nbformat
 from nbconvert import MarkdownExporter
 from nbconvert.preprocessors import ExecutePreprocessor
 import attr #>=22.2.0
 from stdlib_list import stdlib_list
+import tempfile
+import pip_audit #==2.7.3
 
 
 # Metadata for package creation
 __package_metadata__ = {
     "author": "Kyrylo Mordan",
     "author_email": "parachute.repo@gmail.com",
     "description": "A tool to automate package creation within ci based on just .py and optionally .ipynb file.",
@@ -373,23 +375,26 @@
     requirements_output_path  = attr.ib(default='./')
     output_requirements_prefix = attr.ib(default="requirements_")
     custom_modules_filepath = attr.ib(default=None)
     python_version = attr.ib(default='3.8')
 
     # output
     module_name = attr.ib(init=False)
-    requirements_list = attr.ib(init=False)
+    requirements_list = attr.ib(default=[], type = list)
+    vulnerabilities = attr.ib(default=[], type = list)
 
     logger = attr.ib(default=None)
     logger_name = attr.ib(default='Package Requirements Handler')
     loggerLvl = attr.ib(default=logging.INFO)
     logger_format = attr.ib(default=None)
 
     def __attrs_post_init__(self):
         self._initialize_logger()
+        self.vulnerabilities = []
+        self.requirements_list = []
 
 
     def _initialize_logger(self):
 
         """
         Initialize a logger for the class instance based on the specified logging level and logger name.
         """
@@ -397,14 +402,72 @@
         if self.logger is None:
             logging.basicConfig(level=self.loggerLvl, format=self.logger_format)
             logger = logging.getLogger(self.logger_name)
             logger.setLevel(self.loggerLvl)
 
             self.logger = logger
 
+    def check_vulnerabilities(self,
+                              requirements_list : list = None,
+                              raise_error : bool = True):
+
+        """
+        Checks vulnerabilities with pip-audit
+        """
+
+        if requirements_list is None:
+            requirements_list = self.requirements_list
+
+        # Create a temporary requirements file
+        with tempfile.NamedTemporaryFile(delete=True, mode='w', suffix='.txt') as temp_req_file:
+            for dep in requirements_list:
+                temp_req_file.write(dep + '\n')
+            temp_req_file.flush()
+
+            # Run pip-audit on the temporary requirements file
+            result = subprocess.run(
+                ["pip-audit", "-r", temp_req_file.name, "--progress-spinner=off"],
+                capture_output=True, text=True
+            )
+
+            print(result.stdout)
+            self.logger.info(result.stderr)
+
+            if result.returncode == 0:
+                vulnerabilities = []
+            else:
+
+                if result.stdout:
+                    # Access stdout
+                    stdout = result.stdout.strip()
+
+                    # Split into lines and skip the header (assumed to be the first two lines here)
+                    lines = stdout.splitlines()
+                    header_line = ['name', 'version', 'id', 'fix_versions']
+                    data_lines = lines[2:]
+
+                    # Prepare a list of dictionaries
+                    vulnerabilities = []
+
+                    # Process each data line into a dictionary
+                    for line in data_lines:
+                        values = line.split()
+
+                        vd = {key:value for key,value in zip(header_line, values)}
+                        if len(values) <= 3:
+                            vd['fix_versions'] = None
+
+                        vulnerabilities.append(vd)
+                else:
+                    vulnerabilities = []
+
+        self.vulnerabilities += vulnerabilities
+
+        if vulnerabilities and raise_error:
+            raise ValueError("Found vulnerabilities, resolve them or ignore check to move forwards!")
 
     def list_custom_modules(self,
                             custom_modules_filepath : str = None):
         """
         List all custom module names in the specified directory.
         """
 
@@ -527,15 +590,15 @@
                     requirements.append(f"{module}{version_info}")
                 else:
                     requirements.append(module)
 
                 # deduplicate requirements
                 requirements = [requirements[0]] + list(set(requirements[1:]))
 
-        self.requirements_list = requirements
+        self.requirements_list += requirements
 
         return requirements
 
     def write_requirements_file(self,
                                 module_name : str = None,
                                 requirements : list = None,
                                 output_path : str = None,
@@ -1438,14 +1501,15 @@
                                     'Topic :: Scientific/Engineering'])
     requirements_list = attr.ib(default=[])
     execute_readme_notebook = attr.ib(default=True, type = bool)
     python_version = attr.ib(default="3.8")
     version_increment_type = attr.ib(default="patch", type = str)
     default_version = attr.ib(default="0.0.1", type = str)
     kernel_name = attr.ib(default = 'python', type = str)
+    check_vulnerabilities = attr.ib(default=True, type = bool)
 
     ## handler classes
     setup_dir_h_class = attr.ib(default=SetupDirHandler)
     version_h_class = attr.ib(default=VersionHandler)
     import_mapping_h_class = attr.ib(default=ImportMappingHandler)
     local_dependacies_h_class = attr.ib(default=LocalDependaciesHandler)
     requirements_h_class = attr.ib(default=RequirementsHandler)
@@ -1685,14 +1749,15 @@
 
         # extracting package requirements
         self.requirements_list = self.requirements_list + \
             self.requirements_h.extract_requirements(
                 package_mappings=import_mappings,
                 module_filepath=module_filepath,
                 custom_modules=custom_modules)
+        self.requirements_h.check_vulnerabilities()
 
     def add_readme(self,
                     example_notebook_path : str = None,
                     output_path : str = None,
                     execute_notebook : bool = None):
 
         """
```

### Comparing `package_auto_assembler-0.1.1/package_auto_assembler/setup.py` & `package_auto_assembler-0.1.2/package_auto_assembler/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,14 @@
       long_description = fh.read()
 else:
   long_description = ''
 
 setup(
     name="package_auto_assembler",
     packages=["package_auto_assembler"],
-    install_requires=['### package_auto_assembler.py', 'pandas', 'attrs>=22.2.0', 'pyyaml', 'nbformat', 'stdlib-list', 'nbconvert'],
+    install_requires=['### package_auto_assembler.py', 'pandas', 'pyyaml', 'pip_audit==2.7.3', 'nbconvert', 'attrs>=22.2.0', 'stdlib-list', 'nbformat'],
     classifiers=['Development Status :: 3 - Alpha', 'Intended Audience :: Developers', 'Intended Audience :: Science/Research', 'Programming Language :: Python :: 3', 'Programming Language :: Python :: 3.9', 'Programming Language :: Python :: 3.10', 'Programming Language :: Python :: 3.11', 'License :: OSI Approved :: MIT License', 'Topic :: Scientific/Engineering'],
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.1.1"
+    author="Kyrylo Mordan", author_email="parachute.repo@gmail.com", description="A tool to automate package creation within ci based on just .py and optionally .ipynb file.", keywords="['python', 'packaging']", version="0.1.2"
 )
```

### Comparing `package_auto_assembler-0.1.1/package_auto_assembler.egg-info/PKG-INFO` & `package_auto_assembler-0.1.2/package_auto_assembler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: package-auto-assembler
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to automate package creation within ci based on just .py and optionally .ipynb file.
 Author: Kyrylo Mordan
 Author-email: parachute.repo@gmail.com
 Keywords: ['python','packaging']
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,17 @@
 for reusable code. It provides tool to simplify the process of package creatrion
 to a point that it can be triggered automatically within ci/cd pipelines,
 with minimal preparations and requirements for new modules.
 
 
 
 ```python
-from package_auto_assembler import (VersionHandler, \
+import sys
+sys.path.append('../')
+from python_modules.package_auto_assembler import (VersionHandler, \
     ImportMappingHandler, RequirementsHandler, MetadataHandler, \
         LocalDependaciesHandler, LongDocHandler, SetupDirHandler, \
             ReleaseNotesHandler, PackageAutoAssembler)
 ```
 
 ## Usage examples
 
@@ -163,27 +165,27 @@
       <th>0</th>
       <td>2024-01-06 00:54:04</td>
       <td>example_module</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>1</th>
-      <td>2024-04-27 22:44:51</td>
+      <td>2024-05-08 22:14:33</td>
       <td>new_package</td>
       <td>0.0.1</td>
     </tr>
     <tr>
       <th>2</th>
-      <td>2024-04-27 22:44:51</td>
+      <td>2024-05-08 22:14:33</td>
       <td>new_package</td>
       <td>0.0.2</td>
     </tr>
     <tr>
       <th>3</th>
-      <td>2024-04-27 22:44:51</td>
+      <td>2024-05-08 22:14:33</td>
       <td>another_new_package</td>
       <td>0.0.1</td>
     </tr>
   </tbody>
 </table>
 </div>
 
@@ -344,14 +346,82 @@
 
 
 
     ['### example_module.py', 'attrs>=22.2.0']
 
 
 
+#### Audit dependencies
+
+
+```python
+rh.check_vulnerabilities(
+    # optional if ran extract_requirements() before
+    requirements_list = None,
+    raise_error = True
+)
+```
+
+    No known vulnerabilities found
+    
+
+
+    
+
+
+
+```python
+rh.vulnerabilities
+```
+
+
+
+
+    []
+
+
+
+
+```python
+try:
+    rh.check_vulnerabilities(
+        # optional if ran extract_requirements() before
+        requirements_list = ['attrs>=22.2.0', 'pandas', 'hnswlib==0.7.0'],
+        raise_error = True
+    )
+except Exception as e:
+    print(f"Error: {e}")
+```
+
+    Found 1 known vulnerability in 1 package
+    
+
+
+    Name    Version ID                  Fix Versions
+    ------- ------- ------------------- ------------
+    hnswlib 0.7.0   GHSA-xwc8-rf6m-xr86
+    
+    Error: Found vulnerabilities, resolve them or ignore check to move forwards!
+
+
+
+```python
+rh.vulnerabilities
+```
+
+
+
+
+    [{'name': 'hnswlib',
+      'version': '0.7.0',
+      'id': 'GHSA-xwc8-rf6m-xr86',
+      'fix_versions': None}]
+
+
+
 #### Save requirements to a file
 
 
 ```python
 rh.write_requirements_file(
     # optional/required later
     module_name = 'example_module',
@@ -686,15 +756,16 @@
                     'Programming Language :: Python :: 3.11',
                     'License :: OSI Approved :: MIT License',
                     'Topic :: Scientific/Engineering'],
     requirements_list = [],
     execute_readme_notebook = True,
     python_version = "3.8",
     version_increment_type = "patch",
-    default_version = "0.0.1"
+    default_version = "0.0.1",
+    check_vulnerabilities = True
 )
 ```
 
 #### Add metadata from module
 
 
 ```python
@@ -757,38 +828,45 @@
                         'flask': 'Flask',
                         'stdlib_list': 'stdlib-list',
                         'sklearn': 'scikit-learn',
                         'yaml': 'pyyaml'}
 )
 ```
 
-#### Make README out of example notebook
+    No known vulnerabilities found
+    
 
 
-```python
-paa.add_readme(
-    # optional
-    example_notebook_path = "../tests/package_auto_assembler/example_module.ipynb",
-    output_path = "./example_module/README.md",
-    execute_notebook=False,
-)
-```
+    
+
 
 
 ```python
 paa.requirements_list
 ```
 
 
 
 
     ['### example_module.py', 'attrs>=22.2.0']
 
 
 
+#### Make README out of example notebook
+
+
+```python
+paa.add_readme(
+    # optional
+    example_notebook_path = "../tests/package_auto_assembler/example_module.ipynb",
+    output_path = "./example_module/README.md",
+    execute_notebook=False,
+)
+```
+
 #### Prepare setup file
 
 
 ```python
 paa.prep_setup_file(
     # optional
     metadata = {'author': 'Kyrylo Mordan',
```


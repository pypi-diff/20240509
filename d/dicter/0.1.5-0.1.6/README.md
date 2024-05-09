# Comparing `tmp/dicter-0.1.5.tar.gz` & `tmp/dicter-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicter-0.1.5.tar", last modified: Sat Jan 14 11:51:49 2023, max compression
+gzip compressed data, was "dicter-0.1.6.tar", last modified: Thu May  9 19:11:21 2024, max compression
```

## Comparing `dicter-0.1.5.tar` & `dicter-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-14 11:51:49.074683 dicter-0.1.5/
--rw-rw-rw-   0        0        0     1094 2023-01-01 11:16:22.000000 dicter-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       52 2022-12-31 19:11:06.000000 dicter-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6993 2023-01-14 11:51:49.074683 dicter-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6411 2023-01-14 10:48:32.000000 dicter-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-14 11:51:49.012885 dicter-0.1.5/dicter/
--rw-rw-rw-   0        0        0     1603 2023-01-14 11:05:20.000000 dicter-0.1.5/dicter/__init__.py
--rw-rw-rw-   0        0        0    18843 2023-01-14 11:12:37.000000 dicter-0.1.5/dicter/dicter.py
--rw-rw-rw-   0        0        0      727 2023-01-14 11:10:53.000000 dicter-0.1.5/dicter/examples.py
-drwxrwxrwx   0        0        0        0 2023-01-14 11:51:49.071691 dicter-0.1.5/dicter.egg-info/
--rw-rw-rw-   0        0        0     6993 2023-01-14 11:51:47.000000 dicter-0.1.5/dicter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-01-14 11:51:48.000000 dicter-0.1.5/dicter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-14 11:51:47.000000 dicter-0.1.5/dicter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-01-14 11:51:48.000000 dicter-0.1.5/dicter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-14 11:51:48.000000 dicter-0.1.5/dicter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-14 11:51:49.075683 dicter-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1366 2023-01-03 23:30:37.000000 dicter-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:11:21.115530 dicter-0.1.6/
+-rw-rw-rw-   0        0        0     1094 2024-05-09 18:54:10.000000 dicter-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       52 2024-05-09 18:54:10.000000 dicter-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7018 2024-05-09 19:11:21.115530 dicter-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6411 2024-05-09 18:54:10.000000 dicter-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 19:11:21.111502 dicter-0.1.6/dicter/
+-rw-rw-rw-   0        0        0     1595 2024-05-09 19:07:42.000000 dicter-0.1.6/dicter/__init__.py
+-rw-rw-rw-   0        0        0    20622 2024-05-09 19:04:28.000000 dicter-0.1.6/dicter/dicter.py
+-rw-rw-rw-   0        0        0      727 2024-05-09 18:54:10.000000 dicter-0.1.6/dicter/examples.py
+drwxrwxrwx   0        0        0        0 2024-05-09 19:11:21.115530 dicter-0.1.6/dicter.egg-info/
+-rw-rw-rw-   0        0        0     7018 2024-05-09 19:11:20.000000 dicter-0.1.6/dicter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-09 19:11:20.000000 dicter-0.1.6/dicter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 19:11:20.000000 dicter-0.1.6/dicter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-09 19:11:20.000000 dicter-0.1.6/dicter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-09 19:11:20.000000 dicter-0.1.6/dicter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 19:11:21.115530 dicter-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1383 2024-05-09 19:07:09.000000 dicter-0.1.6/setup.py
```

### Comparing `dicter-0.1.5/LICENSE` & `dicter-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dicter-0.1.5/PKG-INFO` & `dicter-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dicter
-Version: 0.1.5
+Version: 0.1.6
 Summary: dicter is a Python package with advanced dictionary functions.
 Home-page: https://github.com/erdogant/dicter
-Download-URL: https://github.com/erdogant/dicter/archive/0.1.5.tar.gz
+Download-URL: https://github.com/erdogant/dicter/archive/0.1.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: tqdm
 
 
 <p align="center">
   <a href="https://erdogant.github.io/dicter/">
   <img src="https://github.com/erdogant/dicter/blob/main/docs/figs/logo.png" width="400" />
   </a>
 </p>
@@ -217,9 +218,7 @@
 
 ### Contribute
 * All kinds of contributions are welcome!
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
 
 ### Licence
 See [LICENSE](LICENSE) for details.
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: dicter Version: 0.1.5 Summary: dicter is a Python
+Metadata-Version: 2.1 Name: dicter Version: 0.1.6 Summary: dicter is a Python
 package with advanced dictionary functions. Home-page: https://github.com/
 erdogant/dicter Download-URL: https://github.com/erdogant/dicter/archive/
-0.1.5.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com License:
-UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE
+0.1.6.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: pandas Requires-Dist: numpy Requires-Dist: tqdm
        _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_d_i_c_t_e_r_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_f_i_g_s_/_l_o_g_o_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/dicter)](https://
 img.shields.io/pypi/pyversions/dicter) [![Pypi](https://img.shields.io/pypi/v/
 dicter)](https://pypi.org/project/dicter/) [![Docs](https://img.shields.io/
 badge/Sphinx-Docs-Green)](https://erdogant.github.io/dicter/) [![LOC](https://
 sloc.xyz/github/erdogant/dicter/?category=code)](https://github.com/erdogant/
 dicter/) [![Downloads](https://static.pepy.tech/personalized-badge/
```

### Comparing `dicter-0.1.5/README.md` & `dicter-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dicter-0.1.5/dicter/__init__.py` & `dicter-0.1.6/dicter/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from dicter.dicter import (
     set_nested,
     get_nested,
+    update,
     traverse,
     flatten,
     depth,
     compare,
     save,
     load,
     to_df,
     clean_filename,
     is_key,
-    set_logger)
+    set_logger,
+    )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 
 # module level doc-string
 __doc__ = """
 dicter
 =====================================================================
 
-Description
------------
 dicter is a Python package with advanced dictionary functions:
 	* Traverse through nested dicts to retrieve key-path.
 	* Set value in dictionary using path.
 	* Get value in dictionary using path.
 	* Flattens dicts.
 	* Compare two dicts.
 	* Store and load in json.
-    
-Example
--------
+
+Examples
+--------
 >>> # Import dicter
 >>> import dicter as dt
 >>>
 >>> # Example dict
 >>> d = {'level_a': 1, 'level_b': {'a': 'hello world'}, 'level_c': 3, 'level_d': {'a': 1, 'b': 2, 'c': {'e': 10}}, 'level_e': 2}
 >>>
 >>> # Get values using nested key
```

### Comparing `dicter-0.1.5/dicter/dicter.py` & `dicter-0.1.6/dicter/dicter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-"""dicter is a Python package with advanced dictionary functions.
-
-# Name        : dicter.py
-# Author      : E.Taskesen
-# Contact     : erdogant@gmail.com
-# github      : https://github.com/erdogant/dicter
-# Licence     : MIT
-"""
-
 import os
 import logging
 import json
 from functools import reduce
 from operator import getitem
 import re
 import pandas as pd
@@ -49,17 +40,14 @@
     Examples
     --------
     >>> # Import dicter
     >>> import dicter as dt
     >>> #
     >>> # Example dictionary
     >>> d = {'level_a': 1, 'level_b': {'a': 'hello world'}, 'level_c': 3, 'level_d': {'a': 1, 'b': 2, 'c': {'e': 10}}, 'level_e': 2}
-    >>> # Get the value for the nested path for:
-    >>> value = dt.is_key(d, "level_a")
-    >>> print(value)  # 1
     >>> #
     >>> # Get the value for the nested path for:
     >>> value = dt.is_key(d, ["level_b","a"])
     """
 
     if not isinstance(d, dict):
         raise AttributeError('is_key() expects dict as first argument.')
@@ -377,16 +365,14 @@
     return 0
 
 
 # %% Compare two dictionaries.
 def compare(d1: dict, d2: dict):
     """Compare two dictionaries.
 
-    Description
-    -----------
     The second dictionary is compared with the first one, and results are shown accordingly.
 
     Parameters
     ----------
     d1 : dict
         Dictionary.
     d2 : dict
@@ -540,14 +526,77 @@
         logger.info('File loaded.')
     else:
         logger.warning('File not found: %s' %(filepath))
     return d
 
 
 # %%
+def update(dictionary, key_to_update, new_value):
+    """Update a nested dictionary for a specific key with a new value.
+
+        Parameters
+        ----------
+        dictionary : dict
+            The nested dictionary to update.
+        key_to_update : str
+            The key to update.
+        new_value : any
+            The new value to assign to the specified key.
+
+        Examples
+        --------
+        >>> data_dict_template = {
+        ...     'DEPARTURE': {
+        ...         'SLOPE': 3,
+        ...         'INTERSECTION': 'V4',
+        ...         'TORA': '1234',
+        ...         'CIRCUIT_ALTITUDE': '1000',
+        ...         'TOWER': '122.108',
+        ...         'alignment': 'concrete'
+        ...     }
+        ... }
+        >>> update(data_dict_template['DEPARTURE'], 'SLOPE', 5)
+        >>> data_dict_template['DEPARTURE']['SLOPE']
+        5
+
+        >>> update(data_dict_template['DEPARTURE'], 'INTERSECTION', 'V5')
+        >>> data_dict_template['DEPARTURE']['INTERSECTION']
+        'V5'
+
+        >>> update(data_dict_template['DEPARTURE'], 'TORA', '2000')
+        >>> data_dict_template['DEPARTURE']['TORA']
+        '2000'
+
+        >>> update(data_dict_template['DEPARTURE'], 'CIRCUIT_ALTITUDE', '1500')
+        >>> data_dict_template['DEPARTURE']['CIRCUIT_ALTITUDE']
+        '1500'
+
+        >>> update(data_dict_template['DEPARTURE'], 'TOWER', '122.109')
+        >>> data_dict_template['DEPARTURE']['TOWER']
+        '122.109'
+
+        >>> update(data_dict_template['DEPARTURE'], 'alignment', 'asphalt')
+        >>> data_dict_template['DEPARTURE']['alignment']
+        'asphalt'
+
+    """
+    for key, value in dictionary.items():
+        if isinstance(value, dict):
+            update(value, key_to_update, new_value)
+        elif key == key_to_update:
+            dictionary[key] = new_value
+        elif isinstance(value, list):
+            for item in value:
+                if isinstance(item, dict):
+                    update(item, key_to_update, new_value)
+                    if key_to_update in item:
+                        item[key_to_update] = new_value
+
+
+# %%
 def set_logger(verbose: [str, int] = 'info'):
     """Set the logger for verbosity messages.
 
     Parameters
     ----------
     verbose : [str, int], default is 'info' or 20
         Set the verbose messages using string or integer values.
```

### Comparing `dicter-0.1.5/dicter/examples.py` & `dicter-0.1.6/dicter/examples.py`

 * *Files identical despite different names*

### Comparing `dicter-0.1.5/dicter.egg-info/PKG-INFO` & `dicter-0.1.6/dicter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dicter
-Version: 0.1.5
+Version: 0.1.6
 Summary: dicter is a Python package with advanced dictionary functions.
 Home-page: https://github.com/erdogant/dicter
-Download-URL: https://github.com/erdogant/dicter/archive/0.1.5.tar.gz
+Download-URL: https://github.com/erdogant/dicter/archive/0.1.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: tqdm
 
 
 <p align="center">
   <a href="https://erdogant.github.io/dicter/">
   <img src="https://github.com/erdogant/dicter/blob/main/docs/figs/logo.png" width="400" />
   </a>
 </p>
@@ -217,9 +218,7 @@
 
 ### Contribute
 * All kinds of contributions are welcome!
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
 
 ### Licence
 See [LICENSE](LICENSE) for details.
-
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: dicter Version: 0.1.5 Summary: dicter is a Python
+Metadata-Version: 2.1 Name: dicter Version: 0.1.6 Summary: dicter is a Python
 package with advanced dictionary functions. Home-page: https://github.com/
 erdogant/dicter Download-URL: https://github.com/erdogant/dicter/archive/
-0.1.5.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com License:
-UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3 Description-Content-Type: text/markdown
-License-File: LICENSE
+0.1.6.tar.gz Author: Erdogan Taskesen Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: pandas Requires-Dist: numpy Requires-Dist: tqdm
        _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_r_d_o_g_a_n_t_/_d_i_c_t_e_r_/_b_l_o_b_/_m_a_i_n_/_d_o_c_s_/_f_i_g_s_/_l_o_g_o_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/dicter)](https://
 img.shields.io/pypi/pyversions/dicter) [![Pypi](https://img.shields.io/pypi/v/
 dicter)](https://pypi.org/project/dicter/) [![Docs](https://img.shields.io/
 badge/Sphinx-Docs-Green)](https://erdogant.github.io/dicter/) [![LOC](https://
 sloc.xyz/github/erdogant/dicter/?category=code)](https://github.com/erdogant/
 dicter/) [![Downloads](https://static.pepy.tech/personalized-badge/
```

### Comparing `dicter-0.1.5/setup.py` & `dicter-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 getversion = re.search( r"^__version__ = ['\"]([^'\"]*)['\"]", open(VERSIONFILE, "rt").read(), re.M)
 if getversion:
     new_version = getversion.group(1)
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=['pandas', 'numpy', 'tqdm'],
      python_requires='>=3',
      name='dicter',
      version=new_version,
      author="Erdogan Taskesen",
```


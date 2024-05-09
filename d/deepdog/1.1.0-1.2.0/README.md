# Comparing `tmp/deepdog-1.1.0.tar.gz` & `tmp/deepdog-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-1.1.0.tar", max compression
+gzip compressed data, was "deepdog-1.2.0.tar", max compression
```

## Comparing `deepdog-1.1.0.tar` & `deepdog-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      366 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/__init__.py
--rw-r--r--   0        0        0       80 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/probs/__init__.py
--rw-r--r--   0        0        0     1389 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/probs/args.py
--rw-r--r--   0        0        0     6243 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/probs/dicts.py
--rw-r--r--   0        0        0     2945 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/cli/probs/main.py
--rw-r--r--   0        0        0      161 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/direct_monte_carlo/__init__.py
--rw-r--r--   0        0        0      329 2024-05-03 04:14:47.847241 deepdog-1.1.0/deepdog/direct_monte_carlo/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7897 2024-05-03 04:14:47.851241 deepdog-1.1.0/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc
--rw-r--r--   0        0        0     3902 2024-05-03 04:14:47.855242 deepdog-1.1.0/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc
--rw-r--r--   0        0        0      461 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/direct_monte_carlo/compose_filter.py
--rw-r--r--   0        0        0     9338 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/direct_monte_carlo/direct_mc.py
--rw-r--r--   0        0        0     3393 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/direct_monte_carlo/dmc_filters.py
--rw-r--r--   0        0        0     1700 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/indexify/__init__.py
--rw-r--r--   0        0        0     2432 2024-05-03 04:14:47.911244 deepdog-1.1.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       73 2024-05-03 04:14:05.565158 deepdog-1.1.0/deepdog/meta.py
--rw-r--r--   0        0        0    12392 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0     4858 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/results/__init__.py
--rw-r--r--   0        0        0     5927 2024-05-03 04:14:47.923245 deepdog-1.1.0/deepdog/results/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      110 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/subset_simulation/__init__.py
--rw-r--r--   0        0        0    11428 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/subset_simulation/subset_simulation_impl.py
--rw-r--r--   0        0        0     6794 2024-05-03 04:14:05.569158 deepdog-1.1.0/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0     1084 2024-05-03 04:14:05.569158 deepdog-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 deepdog-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      366 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/probs/__init__.py
+-rw-r--r--   0        0        0     1389 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/probs/args.py
+-rw-r--r--   0        0        0     6243 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/probs/dicts.py
+-rw-r--r--   0        0        0     2945 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/cli/probs/main.py
+-rw-r--r--   0        0        0      161 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/direct_monte_carlo/__init__.py
+-rw-r--r--   0        0        0      329 2024-05-09 03:25:59.053941 deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7897 2024-05-09 03:25:59.057942 deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc
+-rw-r--r--   0        0        0     3902 2024-05-09 03:25:59.061942 deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc
+-rw-r--r--   0        0        0      461 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/direct_monte_carlo/compose_filter.py
+-rw-r--r--   0        0        0     9338 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/direct_monte_carlo/direct_mc.py
+-rw-r--r--   0        0        0     3393 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/direct_monte_carlo/dmc_filters.py
+-rw-r--r--   0        0        0     1700 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/indexify/__init__.py
+-rw-r--r--   0        0        0     2432 2024-05-09 03:25:59.109944 deepdog-1.2.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       73 2024-05-09 03:25:18.347863 deepdog-1.2.0/deepdog/meta.py
+-rw-r--r--   0        0        0    12392 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0     5732 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/results/__init__.py
+-rw-r--r--   0        0        0     6896 2024-05-09 03:25:59.133946 deepdog-1.2.0/deepdog/results/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      110 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0    11428 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2024-05-09 03:25:18.351863 deepdog-1.2.0/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0     1084 2024-05-09 03:25:18.351863 deepdog-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 deepdog-1.2.0/PKG-INFO
```

### Comparing `deepdog-1.1.0/deepdog/cli/probs/args.py` & `deepdog-1.2.0/deepdog/cli/probs/args.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.1.0/deepdog/cli/probs/dicts.py` & `deepdog-1.2.0/deepdog/cli/probs/dicts.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.1.0/deepdog/cli/probs/main.py` & `deepdog-1.2.0/deepdog/cli/probs/main.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.1.0/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc` & `deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/direct_mc.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 04:14:05 2024 UTC, .py size: 9338 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8d64 3466 7a24 0000  a........d4fz$..
+00000000: 610d 0d0a 0000 0000 1e42 3c66 7a24 0000  a........B<fz$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a02 6400 6401 6c04 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c05 5a02 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0b 5a0b 6d0c 5a0c 0100 6400 6403 6c0d  m.Z.m.Z...d.d.l.
@@ -34,15 +34,15 @@
 00000210: 7175 616c 6e61 6d65 5f5f da03 696e 74da  qualname__..int.
 00000220: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
 00000230: da05 666c 6f61 74da 0373 7472 a900 7214  ..float..str..r.
 00000240: 0000 0072 1400 0000 fa61 2f68 6f6d 652f  ...r.....a/home/
 00000250: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
 00000260: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
 00000270: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
-00000280: 312e 302f 6465 6570 646f 672f 6469 7265  1.0/deepdog/dire
+00000280: 322e 302f 6465 6570 646f 672f 6469 7265  2.0/deepdog/dire
 00000290: 6374 5f6d 6f6e 7465 5f63 6172 6c6f 2f64  ct_monte_carlo/d
 000002a0: 6972 6563 745f 6d63 2e70 7972 0800 0000  irect_mc.pyr....
 000002b0: 1400 0000 7308 0000 000a 0208 0108 0108  ....s...........
 000002c0: 0172 0800 0000 6300 0000 0000 0000 0000  .r....c.........
 000002d0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
 000002e0: 8200 0000 6500 5a01 6400 5a02 5500 6401  ....e.Z.d.Z.U.d.
 000002f0: 5a03 6504 6505 6402 3c00 6403 5a06 6504  Z.e.e.d.<.d.Z.e.
```

### Comparing `deepdog-1.1.0/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc` & `deepdog-1.2.0/deepdog/direct_monte_carlo/__pycache__/dmc_filters.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 04:14:05 2024 UTC, .py size: 3393 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8d64 3466 410d 0000  a........d4fA...
+00000000: 610d 0d0a 0000 0000 1e42 3c66 410d 0000  a........B<fA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 5a07 6400 6404 6c08  ..d.d.l.Z.d.d.l.
 00000060: 5a07 6400 6404 6c09 5a07 6400 6404 6c0a  Z.d.d.l.Z.d.d.l.
 00000070: 5a07 6400 6404 6c00 5a00 4700 6405 6406  Z.d.d.l.Z.G.d.d.
@@ -31,15 +31,15 @@
 000001e0: 0000 0073 1800 0000 6700 7c00 5d10 7d01  ...s....g.|.].}.
 000001f0: 7c01 6a00 7c01 6a01 6602 9102 7104 5300  |.j.|.j.f...q.S.
 00000200: a900 a902 da01 72da 0166 a902 da02 2e30  ......r..f.....0
 00000210: da07 6d65 6173 7572 6572 0800 0000 7208  ..measurer....r.
 00000220: 0000 00fa 632f 686f 6d65 2f6a 656e 6b69  ....c/home/jenki
 00000230: 6e73 2f61 6765 6e74 2f77 6f72 6b73 7061  ns/agent/workspa
 00000240: 6365 2f67 6974 6561 2d70 6879 7369 6373  ce/gitea-physics
-00000250: 5f64 6565 7064 6f67 5f31 2e31 2e30 2f64  _deepdog_1.1.0/d
+00000250: 5f64 6565 7064 6f67 5f31 2e32 2e30 2f64  _deepdog_1.2.0/d
 00000260: 6565 7064 6f67 2f64 6972 6563 745f 6d6f  eepdog/direct_mo
 00000270: 6e74 655f 6361 726c 6f2f 646d 635f 6669  nte_carlo/dmc_fi
 00000280: 6c74 6572 732e 7079 da0a 3c6c 6973 7463  lters.py..<listc
 00000290: 6f6d 703e 0e00 0000 f300 0000 007a 3553  omp>.........z5S
 000002a0: 696e 676c 6544 6f74 506f 7465 6e74 6961  ingleDotPotentia
 000002b0: 6c46 696c 7465 722e 5f5f 696e 6974 5f5f  lFilter.__init__
 000002c0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
```

### Comparing `deepdog-1.1.0/deepdog/direct_monte_carlo/direct_mc.py` & `deepdog-1.2.0/deepdog/direct_monte_carlo/direct_mc.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.1.0/deepdog/direct_monte_carlo/dmc_filters.py` & `deepdog-1.2.0/deepdog/direct_monte_carlo/dmc_filters.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.1.0/deepdog/indexify/__init__.py` & `deepdog-1.2.0/deepdog/indexify/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.1.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc` & `deepdog-1.2.0/deepdog/indexify/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 04:14:05 2024 UTC, .py size: 1700 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 8d64 3466 a406 0000  a........d4f....
+00000000: 610d 0d0a 0000 0000 1e42 3c66 a406 0000  a........B<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4800 0000 6400  .....@...sH...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6503 a005 6506 a101 5a07 6403 6404  Z.e...e...Z.d.d.
 00000060: 8400 5a08 4700 6405 6406 8400 6406 8302  ..Z.G.d.d...d...
 00000070: 5a09 6402 5300 2907 7ac7 0a50 726f 6261  Z.d.S.).z..Proba
@@ -41,15 +41,15 @@
 00000280: 8302 8301 5600 0100 7102 6400 5300 a901  ....V...q.d.S...
 00000290: 4e29 03da 0464 6963 74da 037a 6970 da04  N)...dict..zip..
 000002a0: 6b65 7973 2902 da02 2e30 da01 78a9 01da  keys)....0..x...
 000002b0: 0564 6963 7473 a900 fa56 2f68 6f6d 652f  .dicts...V/home/
 000002c0: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
 000002d0: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
 000002e0: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
-000002f0: 312e 302f 6465 6570 646f 672f 696e 6465  1.0/deepdog/inde
+000002f0: 322e 302f 6465 6570 646f 672f 696e 6465  2.0/deepdog/inde
 00000300: 7869 6679 2f5f 5f69 6e69 745f 5f2e 7079  xify/__init__.py
 00000310: da09 3c67 656e 6578 7072 3e17 0000 00f3  ..<genexpr>.....
 00000320: 0000 0000 7a20 5f64 6963 745f 7072 6f64  ....z _dict_prod
 00000330: 7563 742e 3c6c 6f63 616c 733e 2e3c 6765  uct.<locals>.<ge
 00000340: 6e65 7870 723e 2904 da04 6c69 7374 da09  nexpr>)...list..
 00000350: 6974 6572 746f 6f6c 73da 0770 726f 6475  itertools..produ
 00000360: 6374 da06 7661 6c75 6573 7208 0000 0072  ct..valuesr....r
```

### Comparing `deepdog-1.1.0/deepdog/real_spectrum_run.py` & `deepdog-1.2.0/deepdog/real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.1.0/deepdog/results/__init__.py` & `deepdog-1.2.0/deepdog/results/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,45 +7,58 @@
 import csv
 
 _logger = logging.getLogger(__name__)
 
 FILENAME_REGEX = r"(?P<timestamp>\d{8}-\d{6})-(?P<filename_slug>.*)\.realdata\.fast_filter\.bayesrun\.csv"
 
 MODEL_REGEXES = [
-	r"geom_(?P<xmin>-?\d+)_(?P<xmax>-?\d+)_(?P<ymin>-?\d+)_(?P<ymax>-?\d+)_(?P<zmin>-?\d+)_(?P<zmax>-?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)"
+	r"geom_(?P<xmin>-?\d+)_(?P<xmax>-?\d+)_(?P<ymin>-?\d+)_(?P<ymax>-?\d+)_(?P<zmin>-?\d+)_(?P<zmax>-?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)",
+	r"geom_(?P<xmin>-?\d+)_(?P<xmax>-?\d+)_(?P<ymin>-?\d+)_(?P<ymax>-?\d+)_(?P<zmin>-?\d+)_(?P<zmax>-?\d+)-magnitude_(?P<log_magnitude>\d*\.?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)",
+	r"geom_(?P<xmin>-?\d*\.?\d+)_(?P<xmax>-?\d*\.?\d+)_(?P<ymin>-?\d*\.?\d+)_(?P<ymax>-?\d*\.?\d+)_(?P<zmin>-?\d*\.?\d+)_(?P<zmax>-?\d*\.?\d+)-magnitude_(?P<log_magnitude>\d*\.?\d+)-orientation_(?P<orientation>free|fixedxy|fixedz)-dipole_count_(?P<avg_filled>\d+)_(?P<field_name>\w*)"
 ]
 
 FILE_SLUG_REGEXES = [
 	r"mock_tarucha-(?P<job_index>\d+)",
 	r"(?:(?P<mock>mock)_)?tarucha(?:_(?P<tarucha_run_id>\d+))?-(?P<job_index>\d+)",
+	r"(?P<tag>\w+)-(?P<job_index>\d+)",
 ]
 
 
 @dataclasses.dataclass
 class BayesrunOutputFilename:
 	timestamp: str
 	filename_slug: str
 	path: pathlib.Path
 
 
-@dataclasses.dataclass
 class BayesrunColumnParsed:
 	"""
 	class for parsing a bayesrun while pulling certain special fields out
 	"""
 
 	def __init__(self, groupdict: typing.Dict[str, str]):
 		self.column_field = groupdict["field_name"]
 		self.model_field_dict = {
 			k: v for k, v in groupdict.items() if k != "field_name"
 		}
+		self._groupdict_str = repr(groupdict)
 
 	def __str__(self):
 		return f"BayesrunColumnParsed[{self.column_field}: {self.model_field_dict}]"
 
+	def __repr__(self):
+		return f"BayesrunColumnParsed({self._groupdict_str})"
+
+	def __eq__(self, other):
+		if isinstance(other, BayesrunColumnParsed):
+			return (self.column_field == other.column_field) and (
+				self.model_field_dict == other.model_field_dict
+			)
+		return NotImplemented
+
 
 @dataclasses.dataclass
 class BayesrunModelResult:
 	parsed_model_keys: typing.Dict[str, str]
 	success: int
 	count: int
```

### Comparing `deepdog-1.1.0/deepdog/results/__pycache__/__init__.cpython-39.pyc` & `deepdog-1.2.0/deepdog/results/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri May  3 04:14:05 2024 UTC, .py size: 4858 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,371 +1,431 @@
-00000000: 610d 0d0a 0000 0000 8d64 3466 fa12 0000  a........d4f....
+00000000: 610d 0d0a 0000 0000 1e42 3c66 6416 0000  a........B<fd...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
+00000020: 0005 0000 0040 0000 0073 3401 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a05 6400 6401 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6401 6c07 5a07 6503 a008 6509 a101 5a0a  d.l.Z.e...e...Z.
-00000070: 6402 5a0b 6403 6701 5a0c 6404 6405 6702  d.Z.d.g.Z.d.d.g.
-00000080: 5a0d 6500 6a0e 4700 6406 6407 8400 6407  Z.e.j.G.d.d...d.
-00000090: 8302 8301 5a0f 6500 6a0e 4700 6408 6409  ....Z.e.j.G.d.d.
-000000a0: 8400 6409 8302 8301 5a10 6500 6a0e 4700  ..d.....Z.e.j.G.
-000000b0: 640a 640b 8400 640b 8302 8301 5a11 6500  d.d...d.....Z.e.
-000000c0: 6a0e 4700 640c 640d 8400 640d 8302 8301  j.G.d.d...d.....
-000000d0: 5a12 6420 640f 6410 8401 5a13 6514 6502  Z.d d.d...Z.e.e.
-000000e0: 6a15 6510 1900 6411 9c02 6412 6413 8404  j.e...d...d.d...
-000000f0: 5a16 6502 6a17 6514 6514 6602 1900 6502  Z.e.j.e.e.f...e.
-00000100: 6a18 6511 1900 6414 9c02 6415 6416 8404  j.e...d...d.d...
-00000110: 5a19 6506 6a1a 650f 6417 9c02 6418 6419  Z.e.j.e.d...d.d.
-00000120: 8404 5a1b 6514 6502 6a15 6502 6a17 6514  ..Z.e.e.j.e.j.e.
-00000130: 6514 6602 1900 1900 641a 9c02 641b 641c  e.f.....d...d.d.
-00000140: 8404 5a1c 6506 6a1a 6502 6a15 6505 6a1d  ..Z.e.j.e.j.e.j.
-00000150: 6a1e 1900 6512 641d 9c03 641e 641f 8404  j...e.d...d.d...
-00000160: 5a1f 6401 5300 2921 e900 0000 004e 7a56  Z.d.S.)!.....NzV
-00000170: 283f 503c 7469 6d65 7374 616d 703e 5c64  (?P<timestamp>\d
-00000180: 7b38 7d2d 5c64 7b36 7d29 2d28 3f50 3c66  {8}-\d{6})-(?P<f
-00000190: 696c 656e 616d 655f 736c 7567 3e2e 2a29  ilename_slug>.*)
-000001a0: 5c2e 7265 616c 6461 7461 5c2e 6661 7374  \.realdata\.fast
-000001b0: 5f66 696c 7465 725c 2e62 6179 6573 7275  _filter\.bayesru
-000001c0: 6e5c 2e63 7376 7aca 6765 6f6d 5f28 3f50  n\.csvz.geom_(?P
-000001d0: 3c78 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50  <xmin>-?\d+)_(?P
-000001e0: 3c78 6d61 783e 2d3f 5c64 2b29 5f28 3f50  <xmax>-?\d+)_(?P
-000001f0: 3c79 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50  <ymin>-?\d+)_(?P
-00000200: 3c79 6d61 783e 2d3f 5c64 2b29 5f28 3f50  <ymax>-?\d+)_(?P
-00000210: 3c7a 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50  <zmin>-?\d+)_(?P
-00000220: 3c7a 6d61 783e 2d3f 5c64 2b29 2d6f 7269  <zmax>-?\d+)-ori
-00000230: 656e 7461 7469 6f6e 5f28 3f50 3c6f 7269  entation_(?P<ori
-00000240: 656e 7461 7469 6f6e 3e66 7265 657c 6669  entation>free|fi
-00000250: 7865 6478 797c 6669 7865 647a 292d 6469  xedxy|fixedz)-di
-00000260: 706f 6c65 5f63 6f75 6e74 5f28 3f50 3c61  pole_count_(?P<a
-00000270: 7667 5f66 696c 6c65 643e 5c64 2b29 5f28  vg_filled>\d+)_(
-00000280: 3f50 3c66 6965 6c64 5f6e 616d 653e 5c77  ?P<field_name>\w
-00000290: 2a29 7a1f 6d6f 636b 5f74 6172 7563 6861  *)z.mock_tarucha
-000002a0: 2d28 3f50 3c6a 6f62 5f69 6e64 6578 3e5c  -(?P<job_index>\
-000002b0: 642b 297a 4b28 3f3a 283f 503c 6d6f 636b  d+)zK(?:(?P<mock
-000002c0: 3e6d 6f63 6b29 5f29 3f74 6172 7563 6861  >mock)_)?tarucha
-000002d0: 283f 3a5f 283f 503c 7461 7275 6368 615f  (?:_(?P<tarucha_
-000002e0: 7275 6e5f 6964 3e5c 642b 2929 3f2d 283f  run_id>\d+))?-(?
-000002f0: 503c 6a6f 625f 696e 6465 783e 5c64 2b29  P<job_index>\d+)
-00000300: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000310: 0003 0000 0040 0000 0073 2800 0000 6500  .....@...s(...e.
-00000320: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
-00000330: 6503 6504 6402 3c00 6505 6a06 6504 6403  e.e.d.<.e.j.e.d.
-00000340: 3c00 6404 5300 2905 da16 4261 7965 7372  <.d.S.)...Bayesr
-00000350: 756e 4f75 7470 7574 4669 6c65 6e61 6d65  unOutputFilename
-00000360: da09 7469 6d65 7374 616d 70da 0d66 696c  ..timestamp..fil
-00000370: 656e 616d 655f 736c 7567 da04 7061 7468  ename_slug..path
-00000380: 4e29 07da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
-00000390: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
-000003a0: 6c6e 616d 655f 5fda 0373 7472 da0f 5f5f  lname__..str..__
-000003b0: 616e 6e6f 7461 7469 6f6e 735f 5fda 0770  annotations__..p
-000003c0: 6174 686c 6962 da04 5061 7468 a900 720d  athlib..Path..r.
-000003d0: 0000 0072 0d00 0000 fa55 2f68 6f6d 652f  ...r.....U/home/
-000003e0: 6a65 6e6b 696e 732f 6167 656e 742f 776f  jenkins/agent/wo
-000003f0: 726b 7370 6163 652f 6769 7465 612d 7068  rkspace/gitea-ph
-00000400: 7973 6963 735f 6465 6570 646f 675f 312e  ysics_deepdog_1.
-00000410: 312e 302f 6465 6570 646f 672f 7265 7375  1.0/deepdog/resu
-00000420: 6c74 732f 5f5f 696e 6974 5f5f 2e70 7972  lts/__init__.pyr
-00000430: 0200 0000 1700 0000 7306 0000 000a 0208  ........s.......
-00000440: 0108 0172 0200 0000 6300 0000 0000 0000  ...r....c.......
-00000450: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000460: 0073 3000 0000 6500 5a01 6400 5a02 6401  .s0...e.Z.d.Z.d.
-00000470: 5a03 6504 6a05 6506 6506 6602 1900 6402  Z.e.j.e.e.f...d.
-00000480: 9c01 6403 6404 8404 5a07 6405 6406 8400  ..d.d...Z.d.d...
-00000490: 5a08 6407 5300 2908 da14 4261 7965 7372  Z.d.S.)...Bayesr
-000004a0: 756e 436f 6c75 6d6e 5061 7273 6564 7a49  unColumnParsedzI
-000004b0: 0a09 636c 6173 7320 666f 7220 7061 7273  ..class for pars
-000004c0: 696e 6720 6120 6261 7965 7372 756e 2077  ing a bayesrun w
-000004d0: 6869 6c65 2070 756c 6c69 6e67 2063 6572  hile pulling cer
-000004e0: 7461 696e 2073 7065 6369 616c 2066 6965  tain special fie
-000004f0: 6c64 7320 6f75 740a 0929 01da 0967 726f  lds out..)...gro
-00000500: 7570 6469 6374 6302 0000 0000 0000 0000  updictc.........
-00000510: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00000520: 2200 0000 7c01 6401 1900 7c00 5f00 6402  "...|.d...|._.d.
-00000530: 6403 8400 7c01 a001 a100 4400 8301 7c00  d...|.....D...|.
-00000540: 5f02 6400 5300 2904 4eda 0a66 6965 6c64  _.d.S.).N..field
-00000550: 5f6e 616d 6563 0100 0000 0000 0000 0000  _namec..........
-00000560: 0000 0300 0000 0400 0000 5300 0000 731e  ..........S...s.
-00000570: 0000 0069 007c 005d 165c 027d 017d 027c  ...i.|.].\.}.}.|
-00000580: 0164 006b 0372 047c 017c 0293 0271 0453  .d.k.r.|.|...q.S
-00000590: 0029 0172 1100 0000 720d 0000 0029 03da  .).r....r....)..
-000005a0: 022e 30da 016b da01 7672 0d00 0000 720d  ..0..k..vr....r.
-000005b0: 0000 0072 0e00 0000 da0a 3c64 6963 7463  ...r......<dictc
-000005c0: 6f6d 703e 2600 0000 7302 0000 0006 017a  omp>&...s......z
-000005d0: 3142 6179 6573 7275 6e43 6f6c 756d 6e50  1BayesrunColumnP
-000005e0: 6172 7365 642e 5f5f 696e 6974 5f5f 2e3c  arsed.__init__.<
-000005f0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
-00000600: 703e 2903 da0c 636f 6c75 6d6e 5f66 6965  p>)...column_fie
-00000610: 6c64 da05 6974 656d 73da 106d 6f64 656c  ld..items..model
-00000620: 5f66 6965 6c64 5f64 6963 7429 02da 0473  _field_dict)...s
-00000630: 656c 6672 1000 0000 720d 0000 0072 0d00  elfr....r....r..
-00000640: 0000 720e 0000 00da 085f 5f69 6e69 745f  ..r......__init_
-00000650: 5f24 0000 0073 0800 0000 0001 0a01 0601  _$...s..........
-00000660: 06ff 7a1d 4261 7965 7372 756e 436f 6c75  ..z.BayesrunColu
-00000670: 6d6e 5061 7273 6564 2e5f 5f69 6e69 745f  mnParsed.__init_
-00000680: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00000690: 0000 0500 0000 4300 0000 7316 0000 0064  ......C...s....d
-000006a0: 017c 006a 009b 0064 027c 006a 019b 0064  .|.j...d.|.j...d
-000006b0: 039d 0553 0029 044e 7a15 4261 7965 7372  ...S.).Nz.Bayesr
-000006c0: 756e 436f 6c75 6d6e 5061 7273 6564 5b7a  unColumnParsed[z
-000006d0: 023a 20da 015d 2902 7216 0000 0072 1800  .: ..]).r....r..
-000006e0: 0000 2901 7219 0000 0072 0d00 0000 720d  ..).r....r....r.
-000006f0: 0000 0072 0e00 0000 da07 5f5f 7374 725f  ...r......__str_
-00000700: 5f2a 0000 0073 0200 0000 0001 7a1c 4261  _*...s......z.Ba
-00000710: 7965 7372 756e 436f 6c75 6d6e 5061 7273  yesrunColumnPars
-00000720: 6564 2e5f 5f73 7472 5f5f 4e29 0972 0600  ed.__str__N).r..
-00000730: 0000 7207 0000 0072 0800 0000 da07 5f5f  ..r....r......__
-00000740: 646f 635f 5fda 0674 7970 696e 67da 0444  doc__..typing..D
-00000750: 6963 7472 0900 0000 721a 0000 0072 1c00  ictr....r....r..
-00000760: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000770: 0072 0e00 0000 720f 0000 001e 0000 0073  .r....r........s
-00000780: 0600 0000 0802 0404 1806 720f 0000 0063  ..........r....c
-00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007a0: 0300 0000 4000 0000 7330 0000 0065 005a  ....@...s0...e.Z
-000007b0: 0164 005a 0255 0065 036a 0465 0565 0566  .d.Z.U.e.j.e.e.f
-000007c0: 0219 0065 0664 013c 0065 0765 0664 023c  ...e.d.<.e.e.d.<
-000007d0: 0065 0765 0664 033c 0064 0453 0029 05da  .e.e.d.<.d.S.)..
-000007e0: 1342 6179 6573 7275 6e4d 6f64 656c 5265  .BayesrunModelRe
-000007f0: 7375 6c74 da11 7061 7273 6564 5f6d 6f64  sult..parsed_mod
-00000800: 656c 5f6b 6579 73da 0773 7563 6365 7373  el_keys..success
-00000810: da05 636f 756e 744e 2908 7206 0000 0072  ..countN).r....r
-00000820: 0700 0000 7208 0000 0072 1e00 0000 721f  ....r....r....r.
-00000830: 0000 0072 0900 0000 720a 0000 00da 0369  ...r....r......i
-00000840: 6e74 720d 0000 0072 0d00 0000 720d 0000  ntr....r....r...
-00000850: 0072 0e00 0000 7220 0000 002e 0000 0073  .r....r .......s
-00000860: 0600 0000 0a02 1201 0801 7220 0000 0063  ..........r ...c
-00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000880: 0300 0000 4000 0000 7338 0000 0065 005a  ....@...s8...e.Z
-00000890: 0164 005a 0255 0065 0365 0464 013c 0065  .d.Z.U.e.e.d.<.e
-000008a0: 056a 0664 0265 056a 0766 0219 0065 0464  .j.d.e.j.f...e.d
-000008b0: 033c 0065 056a 0865 0919 0065 0464 043c  .<.e.j.e...e.d.<
-000008c0: 0064 0553 0029 06da 0e42 6179 6573 7275  .d.S.)...Bayesru
-000008d0: 6e4f 7574 7075 74da 0866 696c 656e 616d  nOutput..filenam
-000008e0: 6572 0900 0000 da04 6461 7461 da07 7265  er......data..re
-000008f0: 7375 6c74 734e 290a 7206 0000 0072 0700  sultsN).r....r..
-00000900: 0000 7208 0000 0072 0200 0000 720a 0000  ..r....r....r...
-00000910: 0072 1e00 0000 721f 0000 00da 0341 6e79  .r....r......Any
-00000920: da08 5365 7175 656e 6365 7220 0000 0072  ..Sequencer ...r
-00000930: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00000940: 0000 0072 2500 0000 3500 0000 7306 0000  ...r%...5...s...
-00000950: 000a 0208 0114 0172 2500 0000 e901 0000  .......r%.......
-00000960: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
-00000970: 0000 0700 0000 6300 0000 7336 0000 0074  ......c...s6...t
-00000980: 0064 0174 017c 0083 017c 0183 0344 005d  .d.t.|...|...D.]
-00000990: 207d 027c 007c 0274 027c 027c 0117 0074   }.|.|.t.|.|...t
-000009a0: 017c 0083 0183 0285 0219 0056 0001 0071  .|.........V...q
-000009b0: 1064 0253 0029 037a 460a 0975 7469 6c69  .d.S.).zF..utili
-000009c0: 7479 2066 6f72 2062 6174 6368 696e 6720  ty for batching 
-000009d0: 6261 7965 7372 756e 2066 696c 6573 2077  bayesrun files w
-000009e0: 6865 7265 2063 6f6c 756d 6e73 2061 7070  here columns app
-000009f0: 6561 7220 696e 2074 6872 6565 730a 0972  ear in threes..r
-00000a00: 0100 0000 4e29 03da 0572 616e 6765 da03  ....N)...range..
-00000a10: 6c65 6eda 036d 696e 2903 da08 6974 6572  len..min)...iter
-00000a20: 6162 6c65 da01 6e5a 036e 6478 720d 0000  able..nZ.ndxr...
-00000a30: 0072 0d00 0000 720e 0000 00da 1b5f 6261  .r....r......_ba
-00000a40: 7463 685f 6974 6572 6162 6c65 5f69 6e74  tch_iterable_int
-00000a50: 6f5f 6368 756e 6b73 3c00 0000 7304 0000  o_chunks<...s...
-00000a60: 0000 0414 0172 3100 0000 2902 da06 636f  .....r1...)...co
-00000a70: 6c75 6d6e da06 7265 7475 726e 6301 0000  lumn..returnc...
-00000a80: 0000 0000 0000 0000 0003 0000 0005 0000  ................
-00000a90: 0043 0000 0073 2e00 0000 7400 4400 5d24  .C...s....t.D.]$
-00000aa0: 7d01 7401 a002 7c01 7c00 a102 7d02 7c02  }.t...|.|...}.|.
-00000ab0: 7204 7403 7c02 a004 a100 8301 0200 0100  r.t.|...........
-00000ac0: 5300 7104 6401 5300 2902 7aa3 0a09 5472  S.q.d.S.).z...Tr
-00000ad0: 6965 7320 6f6e 6520 6279 206f 6e65 2061  ies one by one a
-00000ae0: 6c6c 206f 6620 6120 7072 6564 6566 696e  ll of a predefin
-00000af0: 6564 206c 6973 7420 6f66 2072 6567 6578  ed list of regex
-00000b00: 6573 2074 6861 7420 4920 6d69 6768 7420  es that I might 
-00000b10: 6861 7665 2075 7365 6420 696e 2074 6865  have used in the
-00000b20: 2070 6173 742e 0a09 5265 7475 726e 7320   past...Returns 
-00000b30: 7468 6520 6772 6f75 7064 6963 7420 666f  the groupdict fo
-00000b40: 7220 7468 6520 6669 7273 7420 6d61 7463  r the first matc
-00000b50: 682c 206f 7220 4e6f 6e65 2069 6620 6e6f  h, or None if no
-00000b60: 206d 6174 6368 2066 6f75 6e64 2e0a 094e   match found...N
-00000b70: 2905 da0d 4d4f 4445 4c5f 5245 4745 5845  )...MODEL_REGEXE
-00000b80: 53da 0272 65da 056d 6174 6368 720f 0000  S..re..matchr...
-00000b90: 0072 1000 0000 2903 7232 0000 00da 0770  .r....).r2.....p
-00000ba0: 6174 7465 726e 7236 0000 0072 0d00 0000  atternr6...r....
-00000bb0: 720d 0000 0072 0e00 0000 da16 5f70 6172  r....r......_par
-00000bc0: 7365 5f62 6179 6573 7275 6e5f 636f 6c75  se_bayesrun_colu
-00000bd0: 6d6e 4400 0000 730a 0000 0000 0708 010c  mnD...s.........
-00000be0: 0104 0112 0272 3800 0000 2902 da03 726f  .....r8...)...ro
-00000bf0: 7772 3300 0000 6301 0000 0000 0000 0000  wr3...c.........
-00000c00: 0000 0009 0000 0008 0000 0003 0000 0073  ...............s
-00000c10: f200 0000 6700 7d01 7400 7401 8800 a002  ....g.}.t.t.....
-00000c20: a100 8301 6401 8302 7d02 7c02 4400 5dd2  ....d...}.|.D.].
-00000c30: 7d03 6402 6403 8400 7c03 4400 8301 7d04  }.d.d...|.D...}.
-00000c40: 8700 6601 6404 6403 8408 7c03 4400 8301  ..f.d.d...|.D...
-00000c50: 7d05 7c04 6405 1900 6400 7500 7258 7403  }.|.d...d.u.rXt.
-00000c60: 6406 7c03 9b00 9d02 8301 8201 7c04 6407  d.|.........|.d.
-00000c70: 1900 6400 7500 7272 7403 6408 7c03 9b00  ..d.u.rrt.d.|...
-00000c80: 9d02 8301 8201 7c04 6405 1900 6a04 6409  ......|.d...j.d.
-00000c90: 6b03 7294 7403 640a 7c03 6405 1900 9b00  k.r.t.d.|.d.....
-00000ca0: 640b 9d03 8301 8201 7c04 6407 1900 6a04  d.......|.d...j.
-00000cb0: 640c 6b03 72b6 7403 640a 7c03 6407 1900  d.k.r.t.d.|.d...
-00000cc0: 9b00 640d 9d03 8301 8201 7c04 6405 1900  ..d.......|.d...
-00000cd0: 6a05 7d06 7406 7c05 6405 1900 8301 7d07  j.}.t.|.d.....}.
-00000ce0: 7406 7c05 6407 1900 8301 7d08 7c01 a007  t.|.d.....}.|...
-00000cf0: 7408 7c06 7c07 7c08 640e 8d03 a101 0100  t.|.|.|.d.......
-00000d00: 711a 7c01 5300 290f 4ee9 0300 0000 6301  q.|.S.).N.....c.
-00000d10: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000d20: 0000 0053 0000 0073 1400 0000 6700 7c00  ...S...s....g.|.
-00000d30: 5d0c 7d01 7400 7c01 8301 9102 7104 5300  ].}.t.|.....q.S.
-00000d40: 720d 0000 0029 0172 3800 0000 a902 7212  r....).r8.....r.
-00000d50: 0000 0072 3200 0000 720d 0000 0072 0d00  ...r2...r....r..
-00000d60: 0000 720e 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
-00000d70: 6d70 3e5a 0000 00f3 0000 0000 7a27 5f70  mp>Z........z'_p
-00000d80: 6172 7365 5f62 6179 6573 7275 6e5f 726f  arse_bayesrun_ro
-00000d90: 772e 3c6c 6f63 616c 733e 2e3c 6c69 7374  w.<locals>.<list
-00000da0: 636f 6d70 3e63 0100 0000 0000 0000 0000  comp>c..........
-00000db0: 0000 0200 0000 0400 0000 1300 0000 7314  ..............s.
-00000dc0: 0000 0067 007c 005d 0c7d 0188 007c 0119  ...g.|.].}...|..
-00000dd0: 0091 0271 0453 0072 0d00 0000 720d 0000  ...q.S.r....r...
-00000de0: 0072 3b00 0000 a901 7239 0000 0072 0d00  .r;.....r9...r..
-00000df0: 0000 720e 0000 0072 3c00 0000 5b00 0000  ..r....r<...[...
-00000e00: 723d 0000 0072 0100 0000 7a25 6e6f 2076  r=...r....z%no v
-00000e10: 6961 626c 6520 7375 6363 6573 7320 726f  iable success ro
-00000e20: 7720 666f 756e 6420 666f 7220 6b65 7973  w found for keys
-00000e30: 2072 2b00 0000 7a23 6e6f 2076 6961 626c   r+...z#no viabl
-00000e40: 6520 636f 756e 7420 726f 7720 666f 756e  e count row foun
-00000e50: 6420 666f 7220 6b65 7973 2072 2200 0000  d for keys r"...
-00000e60: 7a0b 5468 6520 636f 6c75 6d6e 207a 1720  z.The column z. 
-00000e70: 6973 206e 6f74 2061 2073 7563 6365 7373  is not a success
-00000e80: 2066 6965 6c64 7223 0000 007a 1520 6973   fieldr#...z. is
-00000e90: 206e 6f74 2061 2063 6f75 6e74 2066 6965   not a count fie
-00000ea0: 6c64 2903 7221 0000 0072 2200 0000 7223  ld).r!...r"...r#
-00000eb0: 0000 0029 0972 3100 0000 da04 6c69 7374  ...).r1.....list
-00000ec0: da04 6b65 7973 da0a 5661 6c75 6545 7272  ..keys..ValueErr
-00000ed0: 6f72 7216 0000 0072 1800 0000 7224 0000  orr....r....r$..
-00000ee0: 00da 0661 7070 656e 6472 2000 0000 2909  ...appendr ...).
-00000ef0: 7239 0000 0072 2800 0000 5a0c 6261 7463  r9...r(...Z.batc
-00000f00: 6865 645f 6b65 7973 5a0a 6d6f 6465 6c5f  hed_keysZ.model_
-00000f10: 6b65 7973 da06 7061 7273 6564 da06 7661  keys..parsed..va
-00000f20: 6c75 6573 5a0b 7061 7273 6564 5f6b 6579  luesZ.parsed_key
-00000f30: 7372 2200 0000 7223 0000 0072 0d00 0000  sr"...r#...r....
-00000f40: 723e 0000 0072 0e00 0000 da13 5f70 6172  r>...r......_par
-00000f50: 7365 5f62 6179 6573 7275 6e5f 726f 7753  se_bayesrun_rowS
-00000f60: 0000 0073 3000 0000 0004 0401 1201 0801  ...s0...........
-00000f70: 0e01 1201 0c01 0e01 0c01 0e01 0e01 1401  ................
-00000f80: 0e01 1401 0a01 0c01 0c01 0401 0201 0201  ................
-00000f90: 0201 02fd 04ff 0607 7245 0000 0029 02da  ........rE...)..
-00000fa0: 0466 696c 6572 3300 0000 6301 0000 0000  .filer3...c.....
-00000fb0: 0000 0000 0000 0004 0000 0005 0000 0043  ...............C
-00000fc0: 0000 0073 4200 0000 7c00 6a00 7d01 7401  ...sB...|.j.}.t.
-00000fd0: a002 7403 7c01 a102 7d02 7c02 7324 7404  ..t.|...}.|.s$t.
-00000fe0: 7c01 9b00 6401 9d02 8301 8201 7c02 a005  |...d.......|...
-00000ff0: a100 7d03 7406 7c03 6402 1900 7c03 6403  ..}.t.|.d...|.d.
-00001000: 1900 7c00 6404 8d03 5300 2905 4e7a 2020  ..|.d...S.).Nz  
-00001010: 7761 7320 6e6f 7420 6120 7661 6c69 6420  was not a valid 
-00001020: 6261 7965 7372 756e 206f 7574 7075 7472  bayesrun outputr
-00001030: 0300 0000 7204 0000 0029 0372 0300 0000  ....r....).r....
-00001040: 7204 0000 0072 0500 0000 2907 da04 6e61  r....r....)...na
-00001050: 6d65 7235 0000 0072 3600 0000 da0e 4649  mer5...r6.....FI
-00001060: 4c45 4e41 4d45 5f52 4547 4558 7241 0000  LENAME_REGEXrA..
-00001070: 0072 1000 0000 7202 0000 0029 0472 4600  .r....r....).rF.
-00001080: 0000 7226 0000 0072 3600 0000 da06 6772  ..r&...r6.....gr
-00001090: 6f75 7073 720d 0000 0072 0d00 0000 720e  oupsr....r....r.
-000010a0: 0000 00da 165f 7061 7273 655f 6f75 7470  ....._parse_outp
-000010b0: 7574 5f66 696c 656e 616d 6571 0000 0073  ut_filenameq...s
-000010c0: 1000 0000 0001 0601 0c01 0401 0e01 0801  ................
-000010d0: 0201 0eff 724a 0000 0029 02da 0473 6c75  ....rJ...)...slu
-000010e0: 6772 3300 0000 6301 0000 0000 0000 0000  gr3...c.........
-000010f0: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-00001100: 2a00 0000 7400 4400 5d20 7d01 7401 a002  *...t.D.] }.t...
-00001110: 7c01 7c00 a102 7d02 7c02 7204 7c02 a003  |.|...}.|.r.|...
-00001120: a100 0200 0100 5300 7104 6400 5300 2901  ......S.q.d.S.).
-00001130: 4e29 04da 1146 494c 455f 534c 5547 5f52  N)...FILE_SLUG_R
-00001140: 4547 4558 4553 7235 0000 0072 3600 0000  EGEXESr5...r6...
-00001150: 7210 0000 0029 0372 4b00 0000 7237 0000  r....).rK...r7..
-00001160: 0072 3600 0000 720d 0000 0072 0d00 0000  .r6...r....r....
-00001170: 720e 0000 00da 105f 7061 7273 655f 6669  r......_parse_fi
-00001180: 6c65 5f73 6c75 677c 0000 0073 0a00 0000  le_slug|...s....
-00001190: 0001 0801 0c01 0401 0e02 724d 0000 0029  ..........rM...)
-000011a0: 0372 4600 0000 da0a 696e 6465 7869 6669  .rF.....indexifi
-000011b0: 6572 7233 0000 0063 0200 0000 0000 0000  err3...c........
-000011c0: 0000 0000 0d00 0000 0800 0000 4300 0000  ............C...
-000011d0: 732c 0100 0074 007c 0083 0104 007d 027d  s,...t.|.....}.}
-000011e0: 0374 017c 0269 0067 0064 018d 037d 047c  .t.|.i.g.d...}.|
-000011f0: 046a 02a0 0374 04a0 057c 03a1 01a1 0101  .j...t...|......
-00001200: 0074 067c 026a 0783 017d 057c 0564 0075  .t.|.j...}.|.d.u
-00001210: 0072 5274 08a0 0964 027c 039b 0064 039d  .rRt...d.|...d..
-00001220: 03a1 0101 006e 607c 046a 02a0 037c 05a1  .....n`|.j...|..
-00001230: 0101 007c 0164 0075 0172 b27a 267c 0564  ...|.d.u.r.z&|.d
-00001240: 0419 007d 067c 01a0 0a74 0b7c 0683 01a1  ...}.|...t.|....
-00001250: 017d 077c 046a 02a0 037c 07a1 0101 0057  .}.|.j...|.....W
-00001260: 006e 2404 0074 0c79 b001 0001 0001 0074  .n$..t.y.......t
-00001270: 08a0 0964 057c 059b 0064 069d 03a1 0101  ...d.|...d......
-00001280: 0059 006e 0230 007c 00a0 0da1 008f 4e7d  .Y.n.0.|......N}
-00001290: 0874 0ea0 0f7c 08a1 017d 0964 0764 0884  .t...|...}.d.d..
-000012a0: 007c 0944 0083 017d 0a74 107c 0a83 0164  .|.D...}.t.|...d
-000012b0: 096b 0272 ea7c 0a64 0a19 007d 0b6e 1074  .k.r.|.d...}.n.t
-000012c0: 1164 0b7c 006a 129b 009d 0283 0182 0157  .d.|.j.........W
-000012d0: 0064 0004 0004 0083 0301 006e 1231 0090  .d.........n.1..
-000012e0: 0173 1030 0001 0001 0001 0059 0001 0074  .s.0.......Y...t
-000012f0: 137c 0b83 017d 0c7c 0c7c 045f 147c 0453  .|...}.|.|._.|.S
-00001300: 0029 0c4e 2903 7226 0000 0072 2700 0000  .).N).r&...r'...
-00001310: 7228 0000 007a 1043 6f75 6c64 206e 6f74  r(...z.Could not
-00001320: 2070 6172 7365 207a 3820 6167 6169 6e73   parse z8 agains
-00001330: 7420 616e 7920 6d61 7463 6869 6e67 2072  t any matching r
-00001340: 6567 6578 6573 2e20 476f 696e 6720 746f  egexes. Going to
-00001350: 2073 6b69 7020 7461 6720 7061 7273 696e   skip tag parsin
-00001360: 67da 096a 6f62 5f69 6e64 6578 7a0e 5061  g..job_indexz.Pa
-00001370: 7273 6564 2074 6167 2074 6f20 7a52 2c20  rsed tag to zR, 
-00001380: 616e 6420 6174 7465 6d70 7465 6420 746f  and attempted to
-00001390: 2069 6e64 6578 6966 7920 6275 7420 6e6f   indexify but no
-000013a0: 206a 6f62 5f69 6e64 6578 206b 6579 2077   job_index key w
-000013b0: 6173 2066 6f75 6e64 2e20 736b 6970 7069  as found. skippi
-000013c0: 6e67 2061 6e64 206d 6f76 696e 6720 6f6e  ng and moving on
-000013d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000013e0: 0003 0000 0053 0000 0073 1000 0000 6700  .....S...s....g.
-000013f0: 7c00 5d08 7d01 7c01 9102 7104 5300 720d  |.].}.|...q.S.r.
-00001400: 0000 0072 0d00 0000 2902 7212 0000 00da  ...r....).r.....
-00001410: 0172 720d 0000 0072 0d00 0000 720e 0000  .rr....r....r...
-00001420: 0072 3c00 0000 a100 0000 723d 0000 007a  .r<.......r=...z
-00001430: 2472 6561 645f 6f75 7470 7574 5f66 696c  $read_output_fil
-00001440: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
-00001450: 636f 6d70 3e72 2b00 0000 7201 0000 007a  comp>r+...r....z
-00001460: 2743 6f6e 6675 7365 6420 6162 6f75 7420  'Confused about 
-00001470: 6861 7669 6e67 206d 756c 7469 706c 6520  having multiple 
-00001480: 726f 7773 2069 6e20 2915 724a 0000 0072  rows in ).rJ...r
-00001490: 2500 0000 7227 0000 00da 0675 7064 6174  %...r'.....updat
-000014a0: 65da 0b64 6174 6163 6c61 7373 6573 da06  e..dataclasses..
-000014b0: 6173 6469 6374 724d 0000 0072 0400 0000  asdictrM...r....
-000014c0: da07 5f6c 6f67 6765 72da 0777 6172 6e69  .._logger..warni
-000014d0: 6e67 da08 696e 6465 7869 6679 7224 0000  ng..indexifyr$..
-000014e0: 00da 084b 6579 4572 726f 72da 046f 7065  ...KeyError..ope
-000014f0: 6eda 0363 7376 da0a 4469 6374 5265 6164  n..csv..DictRead
-00001500: 6572 722d 0000 0072 4100 0000 7247 0000  err-...rA...rG..
-00001510: 0072 4500 0000 7228 0000 0029 0d72 4600  .rE...r(...).rF.
-00001520: 0000 724e 0000 005a 0f70 6172 7365 645f  ..rN...Z.parsed_
-00001530: 6669 6c65 6e61 6d65 da03 7461 67da 036f  filename..tag..o
-00001540: 7574 5a0a 7061 7273 6564 5f74 6167 724f  utZ.parsed_tagrO
-00001550: 0000 005a 0a69 6e64 6578 6966 6965 645a  ...Z.indexifiedZ
-00001560: 0a69 6e70 7574 5f66 696c 65da 0672 6561  .input_file..rea
-00001570: 6465 72da 0472 6f77 7372 3900 0000 7228  der..rowsr9...r(
-00001580: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00001590: 0000 da10 7265 6164 5f6f 7574 7075 745f  ....read_output_
-000015a0: 6669 6c65 8500 0000 7336 0000 0000 040c  file....s6......
-000015b0: 010e 0212 010a 0108 0104 010a ff06 040c  ................
-000015c0: 0108 0102 0108 010e 0110 010c 0204 010a  ................
-000015d0: ff0a 040a 010a 010e 010c 010a 0230 0108  .............0..
-000015e0: 0206 0272 5f00 0000 2901 722b 0000 0029  ...r_...).r+...)
-000015f0: 2072 5200 0000 7235 0000 0072 1e00 0000   rR...r5...r....
-00001600: da07 6c6f 6767 696e 67da 1064 6565 7064  ..logging..deepd
-00001610: 6f67 2e69 6e64 6578 6966 79da 0764 6565  og.indexify..dee
-00001620: 7064 6f67 720b 0000 0072 5900 0000 da09  pdogr....rY.....
-00001630: 6765 744c 6f67 6765 7272 0600 0000 7254  getLoggerr....rT
-00001640: 0000 0072 4800 0000 7234 0000 0072 4c00  ...rH...r4...rL.
-00001650: 0000 da09 6461 7461 636c 6173 7372 0200  ....dataclassr..
-00001660: 0000 720f 0000 0072 2000 0000 7225 0000  ..r....r ...r%..
-00001670: 0072 3100 0000 7209 0000 00da 084f 7074  .r1...r......Opt
-00001680: 696f 6e61 6c72 3800 0000 721f 0000 0072  ionalr8...r....r
-00001690: 2a00 0000 7245 0000 0072 0c00 0000 724a  *...rE...r....rJ
-000016a0: 0000 0072 4d00 0000 7256 0000 00da 0a49  ...rM...rV.....I
-000016b0: 6e64 6578 6966 6965 7272 5f00 0000 720d  ndexifierr_...r.
-000016c0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-000016d0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000016e0: 7342 0000 0008 0108 0108 0108 0108 0108  sB..............
-000016f0: 0108 020a 0204 0302 ff04 0502 0102 fe04  ................
-00001700: 0604 0110 0604 0110 0f04 0110 0604 0110  ................
-00001710: 060a 0902 0108 fe0c 100c 0108 fe0c 1e12  ................
-00001720: 0b20 0a10 0102 fe                        . .....
+00000070: 6402 5a0b 6700 6403 a201 5a0c 6700 6404  d.Z.g.d...Z.g.d.
+00000080: a201 5a0d 6500 6a0e 4700 6405 6406 8400  ..Z.e.j.G.d.d...
+00000090: 6406 8302 8301 5a0f 4700 6407 6408 8400  d.....Z.G.d.d...
+000000a0: 6408 8302 5a10 6500 6a0e 4700 6409 640a  d...Z.e.j.G.d.d.
+000000b0: 8400 640a 8302 8301 5a11 6500 6a0e 4700  ..d.....Z.e.j.G.
+000000c0: 640b 640c 8400 640c 8302 8301 5a12 641f  d.d...d.....Z.d.
+000000d0: 640e 640f 8401 5a13 6514 6502 6a15 6510  d.d...Z.e.e.j.e.
+000000e0: 1900 6410 9c02 6411 6412 8404 5a16 6502  ..d...d.d...Z.e.
+000000f0: 6a17 6514 6514 6602 1900 6502 6a18 6511  j.e.e.f...e.j.e.
+00000100: 1900 6413 9c02 6414 6415 8404 5a19 6506  ..d...d.d...Z.e.
+00000110: 6a1a 650f 6416 9c02 6417 6418 8404 5a1b  j.e.d...d.d...Z.
+00000120: 6514 6502 6a15 6502 6a17 6514 6514 6602  e.e.j.e.j.e.e.f.
+00000130: 1900 1900 6419 9c02 641a 641b 8404 5a1c  ....d...d.d...Z.
+00000140: 6506 6a1a 6502 6a15 6505 6a1d 6a1e 1900  e.j.e.j.e.j.j...
+00000150: 6512 641c 9c03 641d 641e 8404 5a1f 6401  e.d...d.d...Z.d.
+00000160: 5300 2920 e900 0000 004e 7a56 283f 503c  S.) .....NzV(?P<
+00000170: 7469 6d65 7374 616d 703e 5c64 7b38 7d2d  timestamp>\d{8}-
+00000180: 5c64 7b36 7d29 2d28 3f50 3c66 696c 656e  \d{6})-(?P<filen
+00000190: 616d 655f 736c 7567 3e2e 2a29 5c2e 7265  ame_slug>.*)\.re
+000001a0: 616c 6461 7461 5c2e 6661 7374 5f66 696c  aldata\.fast_fil
+000001b0: 7465 725c 2e62 6179 6573 7275 6e5c 2e63  ter\.bayesrun\.c
+000001c0: 7376 2903 7aca 6765 6f6d 5f28 3f50 3c78  sv).z.geom_(?P<x
+000001d0: 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50 3c78  min>-?\d+)_(?P<x
+000001e0: 6d61 783e 2d3f 5c64 2b29 5f28 3f50 3c79  max>-?\d+)_(?P<y
+000001f0: 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50 3c79  min>-?\d+)_(?P<y
+00000200: 6d61 783e 2d3f 5c64 2b29 5f28 3f50 3c7a  max>-?\d+)_(?P<z
+00000210: 6d69 6e3e 2d3f 5c64 2b29 5f28 3f50 3c7a  min>-?\d+)_(?P<z
+00000220: 6d61 783e 2d3f 5c64 2b29 2d6f 7269 656e  max>-?\d+)-orien
+00000230: 7461 7469 6f6e 5f28 3f50 3c6f 7269 656e  tation_(?P<orien
+00000240: 7461 7469 6f6e 3e66 7265 657c 6669 7865  tation>free|fixe
+00000250: 6478 797c 6669 7865 647a 292d 6469 706f  dxy|fixedz)-dipo
+00000260: 6c65 5f63 6f75 6e74 5f28 3f50 3c61 7667  le_count_(?P<avg
+00000270: 5f66 696c 6c65 643e 5c64 2b29 5f28 3f50  _filled>\d+)_(?P
+00000280: 3c66 6965 6c64 5f6e 616d 653e 5c77 2a29  <field_name>\w*)
+00000290: 7af1 6765 6f6d 5f28 3f50 3c78 6d69 6e3e  z.geom_(?P<xmin>
+000002a0: 2d3f 5c64 2b29 5f28 3f50 3c78 6d61 783e  -?\d+)_(?P<xmax>
+000002b0: 2d3f 5c64 2b29 5f28 3f50 3c79 6d69 6e3e  -?\d+)_(?P<ymin>
+000002c0: 2d3f 5c64 2b29 5f28 3f50 3c79 6d61 783e  -?\d+)_(?P<ymax>
+000002d0: 2d3f 5c64 2b29 5f28 3f50 3c7a 6d69 6e3e  -?\d+)_(?P<zmin>
+000002e0: 2d3f 5c64 2b29 5f28 3f50 3c7a 6d61 783e  -?\d+)_(?P<zmax>
+000002f0: 2d3f 5c64 2b29 2d6d 6167 6e69 7475 6465  -?\d+)-magnitude
+00000300: 5f28 3f50 3c6c 6f67 5f6d 6167 6e69 7475  _(?P<log_magnitu
+00000310: 6465 3e5c 642a 5c2e 3f5c 642b 292d 6f72  de>\d*\.?\d+)-or
+00000320: 6965 6e74 6174 696f 6e5f 283f 503c 6f72  ientation_(?P<or
+00000330: 6965 6e74 6174 696f 6e3e 6672 6565 7c66  ientation>free|f
+00000340: 6978 6564 7879 7c66 6978 6564 7a29 2d64  ixedxy|fixedz)-d
+00000350: 6970 6f6c 655f 636f 756e 745f 283f 503c  ipole_count_(?P<
+00000360: 6176 675f 6669 6c6c 6564 3e5c 642b 295f  avg_filled>\d+)_
+00000370: 283f 503c 6669 656c 645f 6e61 6d65 3e5c  (?P<field_name>\
+00000380: 772a 2961 1501 0000 6765 6f6d 5f28 3f50  w*)a....geom_(?P
+00000390: 3c78 6d69 6e3e 2d3f 5c64 2a5c 2e3f 5c64  <xmin>-?\d*\.?\d
+000003a0: 2b29 5f28 3f50 3c78 6d61 783e 2d3f 5c64  +)_(?P<xmax>-?\d
+000003b0: 2a5c 2e3f 5c64 2b29 5f28 3f50 3c79 6d69  *\.?\d+)_(?P<ymi
+000003c0: 6e3e 2d3f 5c64 2a5c 2e3f 5c64 2b29 5f28  n>-?\d*\.?\d+)_(
+000003d0: 3f50 3c79 6d61 783e 2d3f 5c64 2a5c 2e3f  ?P<ymax>-?\d*\.?
+000003e0: 5c64 2b29 5f28 3f50 3c7a 6d69 6e3e 2d3f  \d+)_(?P<zmin>-?
+000003f0: 5c64 2a5c 2e3f 5c64 2b29 5f28 3f50 3c7a  \d*\.?\d+)_(?P<z
+00000400: 6d61 783e 2d3f 5c64 2a5c 2e3f 5c64 2b29  max>-?\d*\.?\d+)
+00000410: 2d6d 6167 6e69 7475 6465 5f28 3f50 3c6c  -magnitude_(?P<l
+00000420: 6f67 5f6d 6167 6e69 7475 6465 3e5c 642a  og_magnitude>\d*
+00000430: 5c2e 3f5c 642b 292d 6f72 6965 6e74 6174  \.?\d+)-orientat
+00000440: 696f 6e5f 283f 503c 6f72 6965 6e74 6174  ion_(?P<orientat
+00000450: 696f 6e3e 6672 6565 7c66 6978 6564 7879  ion>free|fixedxy
+00000460: 7c66 6978 6564 7a29 2d64 6970 6f6c 655f  |fixedz)-dipole_
+00000470: 636f 756e 745f 283f 503c 6176 675f 6669  count_(?P<avg_fi
+00000480: 6c6c 6564 3e5c 642b 295f 283f 503c 6669  lled>\d+)_(?P<fi
+00000490: 656c 645f 6e61 6d65 3e5c 772a 2929 037a  eld_name>\w*)).z
+000004a0: 1f6d 6f63 6b5f 7461 7275 6368 612d 283f  .mock_tarucha-(?
+000004b0: 503c 6a6f 625f 696e 6465 783e 5c64 2b29  P<job_index>\d+)
+000004c0: 7a4b 283f 3a28 3f50 3c6d 6f63 6b3e 6d6f  zK(?:(?P<mock>mo
+000004d0: 636b 295f 293f 7461 7275 6368 6128 3f3a  ck)_)?tarucha(?:
+000004e0: 5f28 3f50 3c74 6172 7563 6861 5f72 756e  _(?P<tarucha_run
+000004f0: 5f69 643e 5c64 2b29 293f 2d28 3f50 3c6a  _id>\d+))?-(?P<j
+00000500: 6f62 5f69 6e64 6578 3e5c 642b 297a 1f28  ob_index>\d+)z.(
+00000510: 3f50 3c74 6167 3e5c 772b 292d 283f 503c  ?P<tag>\w+)-(?P<
+00000520: 6a6f 625f 696e 6465 783e 5c64 2b29 6300  job_index>\d+)c.
+00000530: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000540: 0000 0040 0000 0073 2800 0000 6500 5a01  ...@...s(...e.Z.
+00000550: 6400 5a02 5500 6503 6504 6401 3c00 6503  d.Z.U.e.e.d.<.e.
+00000560: 6504 6402 3c00 6505 6a06 6504 6403 3c00  e.d.<.e.j.e.d.<.
+00000570: 6404 5300 2905 da16 4261 7965 7372 756e  d.S.)...Bayesrun
+00000580: 4f75 7470 7574 4669 6c65 6e61 6d65 da09  OutputFilename..
+00000590: 7469 6d65 7374 616d 70da 0d66 696c 656e  timestamp..filen
+000005a0: 616d 655f 736c 7567 da04 7061 7468 4e29  ame_slug..pathN)
+000005b0: 07da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+000005c0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+000005d0: 616d 655f 5fda 0373 7472 da0f 5f5f 616e  ame__..str..__an
+000005e0: 6e6f 7461 7469 6f6e 735f 5fda 0770 6174  notations__..pat
+000005f0: 686c 6962 da04 5061 7468 a900 720d 0000  hlib..Path..r...
+00000600: 0072 0d00 0000 fa55 2f68 6f6d 652f 6a65  .r.....U/home/je
+00000610: 6e6b 696e 732f 6167 656e 742f 776f 726b  nkins/agent/work
+00000620: 7370 6163 652f 6769 7465 612d 7068 7973  space/gitea-phys
+00000630: 6963 735f 6465 6570 646f 675f 312e 322e  ics_deepdog_1.2.
+00000640: 302f 6465 6570 646f 672f 7265 7375 6c74  0/deepdog/result
+00000650: 732f 5f5f 696e 6974 5f5f 2e70 7972 0200  s/__init__.pyr..
+00000660: 0000 1a00 0000 7306 0000 000a 0208 0108  ......s.........
+00000670: 0172 0200 0000 6300 0000 0000 0000 0000  .r....c.........
+00000680: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00000690: 4000 0000 6500 5a01 6400 5a02 6401 5a03  @...e.Z.d.Z.d.Z.
+000006a0: 6504 6a05 6506 6506 6602 1900 6402 9c01  e.j.e.e.f...d...
+000006b0: 6403 6404 8404 5a07 6405 6406 8400 5a08  d.d...Z.d.d...Z.
+000006c0: 6407 6408 8400 5a09 6409 640a 8400 5a0a  d.d...Z.d.d...Z.
+000006d0: 640b 5300 290c da14 4261 7965 7372 756e  d.S.)...Bayesrun
+000006e0: 436f 6c75 6d6e 5061 7273 6564 7a49 0a09  ColumnParsedzI..
+000006f0: 636c 6173 7320 666f 7220 7061 7273 696e  class for parsin
+00000700: 6720 6120 6261 7965 7372 756e 2077 6869  g a bayesrun whi
+00000710: 6c65 2070 756c 6c69 6e67 2063 6572 7461  le pulling certa
+00000720: 696e 2073 7065 6369 616c 2066 6965 6c64  in special field
+00000730: 7320 6f75 740a 0929 01da 0967 726f 7570  s out..)...group
+00000740: 6469 6374 6302 0000 0000 0000 0000 0000  dictc...........
+00000750: 0002 0000 0003 0000 0043 0000 0073 2c00  .........C...s,.
+00000760: 0000 7c01 6401 1900 7c00 5f00 6402 6403  ..|.d...|._.d.d.
+00000770: 8400 7c01 a001 a100 4400 8301 7c00 5f02  ..|.....D...|._.
+00000780: 7403 7c01 8301 7c00 5f04 6400 5300 2904  t.|...|._.d.S.).
+00000790: 4eda 0a66 6965 6c64 5f6e 616d 6563 0100  N..field_namec..
+000007a0: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+000007b0: 0000 5300 0000 731e 0000 0069 007c 005d  ..S...s....i.|.]
+000007c0: 165c 027d 017d 027c 0164 006b 0372 047c  .\.}.}.|.d.k.r.|
+000007d0: 017c 0293 0271 0453 0029 0172 1100 0000  .|...q.S.).r....
+000007e0: 720d 0000 0029 03da 022e 30da 016b da01  r....)....0..k..
+000007f0: 7672 0d00 0000 720d 0000 0072 0e00 0000  vr....r....r....
+00000800: da0a 3c64 6963 7463 6f6d 703e 2800 0000  ..<dictcomp>(...
+00000810: 7302 0000 0006 017a 3142 6179 6573 7275  s......z1Bayesru
+00000820: 6e43 6f6c 756d 6e50 6172 7365 642e 5f5f  nColumnParsed.__
+00000830: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00000840: 3c64 6963 7463 6f6d 703e 2905 da0c 636f  <dictcomp>)...co
+00000850: 6c75 6d6e 5f66 6965 6c64 da05 6974 656d  lumn_field..item
+00000860: 73da 106d 6f64 656c 5f66 6965 6c64 5f64  s..model_field_d
+00000870: 6963 74da 0472 6570 72da 0e5f 6772 6f75  ict..repr.._grou
+00000880: 7064 6963 745f 7374 7229 02da 0473 656c  pdict_str)...sel
+00000890: 6672 1000 0000 720d 0000 0072 0d00 0000  fr....r....r....
+000008a0: 720e 0000 00da 085f 5f69 6e69 745f 5f26  r......__init__&
+000008b0: 0000 0073 0a00 0000 0001 0a01 0601 06ff  ...s............
+000008c0: 0803 7a1d 4261 7965 7372 756e 436f 6c75  ..z.BayesrunColu
+000008d0: 6d6e 5061 7273 6564 2e5f 5f69 6e69 745f  mnParsed.__init_
+000008e0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+000008f0: 0000 0500 0000 4300 0000 7316 0000 0064  ......C...s....d
+00000900: 017c 006a 009b 0064 027c 006a 019b 0064  .|.j...d.|.j...d
+00000910: 039d 0553 0029 044e 7a15 4261 7965 7372  ...S.).Nz.Bayesr
+00000920: 756e 436f 6c75 6d6e 5061 7273 6564 5b7a  unColumnParsed[z
+00000930: 023a 20da 015d 2902 7216 0000 0072 1800  .: ..]).r....r..
+00000940: 0000 a901 721b 0000 0072 0d00 0000 720d  ....r....r....r.
+00000950: 0000 0072 0e00 0000 da07 5f5f 7374 725f  ...r......__str_
+00000960: 5f2d 0000 0073 0200 0000 0001 7a1c 4261  _-...s......z.Ba
+00000970: 7965 7372 756e 436f 6c75 6d6e 5061 7273  yesrunColumnPars
+00000980: 6564 2e5f 5f73 7472 5f5f 6301 0000 0000  ed.__str__c.....
+00000990: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+000009a0: 0000 0073 0e00 0000 6401 7c00 6a00 9b00  ...s....d.|.j...
+000009b0: 6402 9d03 5300 2903 4e7a 1542 6179 6573  d...S.).Nz.Bayes
+000009c0: 7275 6e43 6f6c 756d 6e50 6172 7365 6428  runColumnParsed(
+000009d0: da01 2929 0172 1a00 0000 721e 0000 0072  ..)).r....r....r
+000009e0: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
+000009f0: 5f5f 7265 7072 5f5f 3000 0000 7302 0000  __repr__0...s...
+00000a00: 0000 017a 1d42 6179 6573 7275 6e43 6f6c  ...z.BayesrunCol
+00000a10: 756d 6e50 6172 7365 642e 5f5f 7265 7072  umnParsed.__repr
+00000a20: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
+00000a30: 0000 0003 0000 0043 0000 0073 2600 0000  .......C...s&...
+00000a40: 7400 7c01 7401 8302 7222 7c00 6a02 7c01  t.|.t...r"|.j.|.
+00000a50: 6a02 6b02 6f20 7c00 6a03 7c01 6a03 6b02  j.k.o |.j.|.j.k.
+00000a60: 5300 7404 5300 a901 4e29 05da 0a69 7369  S.t.S...N)...isi
+00000a70: 6e73 7461 6e63 6572 0f00 0000 7216 0000  nstancer....r...
+00000a80: 0072 1800 0000 da0e 4e6f 7449 6d70 6c65  .r......NotImple
+00000a90: 6d65 6e74 6564 2902 721b 0000 00da 056f  mented).r......o
+00000aa0: 7468 6572 720d 0000 0072 0d00 0000 720e  therr....r....r.
+00000ab0: 0000 00da 065f 5f65 715f 5f33 0000 0073  .....__eq__3...s
+00000ac0: 0a00 0000 0001 0a01 0c01 0aff 0203 7a1b  ..............z.
+00000ad0: 4261 7965 7372 756e 436f 6c75 6d6e 5061  BayesrunColumnPa
+00000ae0: 7273 6564 2e5f 5f65 715f 5f4e 290b 7206  rsed.__eq__N).r.
+00000af0: 0000 0072 0700 0000 7208 0000 00da 075f  ...r....r......_
+00000b00: 5f64 6f63 5f5f da06 7479 7069 6e67 da04  _doc__..typing..
+00000b10: 4469 6374 7209 0000 0072 1c00 0000 721f  Dictr....r....r.
+00000b20: 0000 0072 2100 0000 7226 0000 0072 0d00  ...r!...r&...r..
+00000b30: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00000b40: 0072 0f00 0000 2100 0000 730a 0000 0008  .r....!...s.....
+00000b50: 0104 0418 0708 0308 0372 0f00 0000 6300  .........r....c.
+00000b60: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000b70: 0000 0040 0000 0073 3000 0000 6500 5a01  ...@...s0...e.Z.
+00000b80: 6400 5a02 5500 6503 6a04 6505 6505 6602  d.Z.U.e.j.e.e.f.
+00000b90: 1900 6506 6401 3c00 6507 6506 6402 3c00  ..e.d.<.e.e.d.<.
+00000ba0: 6507 6506 6403 3c00 6404 5300 2905 da13  e.e.d.<.d.S.)...
+00000bb0: 4261 7965 7372 756e 4d6f 6465 6c52 6573  BayesrunModelRes
+00000bc0: 756c 74da 1170 6172 7365 645f 6d6f 6465  ult..parsed_mode
+00000bd0: 6c5f 6b65 7973 da07 7375 6363 6573 73da  l_keys..success.
+00000be0: 0563 6f75 6e74 4e29 0872 0600 0000 7207  .countN).r....r.
+00000bf0: 0000 0072 0800 0000 7228 0000 0072 2900  ...r....r(...r).
+00000c00: 0000 7209 0000 0072 0a00 0000 da03 696e  ..r....r......in
+00000c10: 7472 0d00 0000 720d 0000 0072 0d00 0000  tr....r....r....
+00000c20: 720e 0000 0072 2a00 0000 3b00 0000 7306  r....r*...;...s.
+00000c30: 0000 000a 0212 0108 0172 2a00 0000 6300  .........r*...c.
+00000c40: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000c50: 0000 0040 0000 0073 3800 0000 6500 5a01  ...@...s8...e.Z.
+00000c60: 6400 5a02 5500 6503 6504 6401 3c00 6505  d.Z.U.e.e.d.<.e.
+00000c70: 6a06 6402 6505 6a07 6602 1900 6504 6403  j.d.e.j.f...e.d.
+00000c80: 3c00 6505 6a08 6509 1900 6504 6404 3c00  <.e.j.e...e.d.<.
+00000c90: 6405 5300 2906 da0e 4261 7965 7372 756e  d.S.)...Bayesrun
+00000ca0: 4f75 7470 7574 da08 6669 6c65 6e61 6d65  Output..filename
+00000cb0: 7209 0000 00da 0464 6174 61da 0772 6573  r......data..res
+00000cc0: 756c 7473 4e29 0a72 0600 0000 7207 0000  ultsN).r....r...
+00000cd0: 0072 0800 0000 7202 0000 0072 0a00 0000  .r....r....r....
+00000ce0: 7228 0000 0072 2900 0000 da03 416e 79da  r(...r).....Any.
+00000cf0: 0853 6571 7565 6e63 6572 2a00 0000 720d  .Sequencer*...r.
+00000d00: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000d10: 0000 722f 0000 0042 0000 0073 0600 0000  ..r/...B...s....
+00000d20: 0a02 0801 1401 722f 0000 00e9 0100 0000  ......r/........
+00000d30: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000d40: 0007 0000 0063 0000 0073 3600 0000 7400  .....c...s6...t.
+00000d50: 6401 7401 7c00 8301 7c01 8303 4400 5d20  d.t.|...|...D.] 
+00000d60: 7d02 7c00 7c02 7402 7c02 7c01 1700 7401  }.|.|.t.|.|...t.
+00000d70: 7c00 8301 8302 8502 1900 5600 0100 7110  |.........V...q.
+00000d80: 6402 5300 2903 7a46 0a09 7574 696c 6974  d.S.).zF..utilit
+00000d90: 7920 666f 7220 6261 7463 6869 6e67 2062  y for batching b
+00000da0: 6179 6573 7275 6e20 6669 6c65 7320 7768  ayesrun files wh
+00000db0: 6572 6520 636f 6c75 6d6e 7320 6170 7065  ere columns appe
+00000dc0: 6172 2069 6e20 7468 7265 6573 0a09 7201  ar in threes..r.
+00000dd0: 0000 004e 2903 da05 7261 6e67 65da 036c  ...N)...range..l
+00000de0: 656e da03 6d69 6e29 03da 0869 7465 7261  en..min)...itera
+00000df0: 626c 65da 016e 5a03 6e64 7872 0d00 0000  ble..nZ.ndxr....
+00000e00: 720d 0000 0072 0e00 0000 da1b 5f62 6174  r....r......_bat
+00000e10: 6368 5f69 7465 7261 626c 655f 696e 746f  ch_iterable_into
+00000e20: 5f63 6875 6e6b 7349 0000 0073 0400 0000  _chunksI...s....
+00000e30: 0004 1401 723b 0000 0029 02da 0663 6f6c  ....r;...)...col
+00000e40: 756d 6eda 0672 6574 7572 6e63 0100 0000  umn..returnc....
+00000e50: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+00000e60: 4300 0000 732e 0000 0074 0044 005d 247d  C...s....t.D.]$}
+00000e70: 0174 01a0 027c 017c 00a1 027d 027c 0272  .t...|.|...}.|.r
+00000e80: 0474 037c 02a0 04a1 0083 0102 0001 0053  .t.|...........S
+00000e90: 0071 0464 0153 0029 027a a30a 0954 7269  .q.d.S.).z...Tri
+00000ea0: 6573 206f 6e65 2062 7920 6f6e 6520 616c  es one by one al
+00000eb0: 6c20 6f66 2061 2070 7265 6465 6669 6e65  l of a predefine
+00000ec0: 6420 6c69 7374 206f 6620 7265 6765 7865  d list of regexe
+00000ed0: 7320 7468 6174 2049 206d 6967 6874 2068  s that I might h
+00000ee0: 6176 6520 7573 6564 2069 6e20 7468 6520  ave used in the 
+00000ef0: 7061 7374 2e0a 0952 6574 7572 6e73 2074  past...Returns t
+00000f00: 6865 2067 726f 7570 6469 6374 2066 6f72  he groupdict for
+00000f10: 2074 6865 2066 6972 7374 206d 6174 6368   the first match
+00000f20: 2c20 6f72 204e 6f6e 6520 6966 206e 6f20  , or None if no 
+00000f30: 6d61 7463 6820 666f 756e 642e 0a09 4e29  match found...N)
+00000f40: 05da 0d4d 4f44 454c 5f52 4547 4558 4553  ...MODEL_REGEXES
+00000f50: da02 7265 da05 6d61 7463 6872 0f00 0000  ..re..matchr....
+00000f60: 7210 0000 0029 0372 3c00 0000 da07 7061  r....).r<.....pa
+00000f70: 7474 6572 6e72 4000 0000 720d 0000 0072  tternr@...r....r
+00000f80: 0d00 0000 720e 0000 00da 165f 7061 7273  ....r......_pars
+00000f90: 655f 6261 7965 7372 756e 5f63 6f6c 756d  e_bayesrun_colum
+00000fa0: 6e51 0000 0073 0a00 0000 0007 0801 0c01  nQ...s..........
+00000fb0: 0401 1202 7242 0000 0029 02da 0372 6f77  ....rB...)...row
+00000fc0: 723d 0000 0063 0100 0000 0000 0000 0000  r=...c..........
+00000fd0: 0000 0900 0000 0800 0000 0300 0000 73f2  ..............s.
+00000fe0: 0000 0067 007d 0174 0074 0188 00a0 02a1  ...g.}.t.t......
+00000ff0: 0083 0164 0183 027d 027c 0244 005d d27d  ...d...}.|.D.].}
+00001000: 0364 0264 0384 007c 0344 0083 017d 0487  .d.d...|.D...}..
+00001010: 0066 0164 0464 0384 087c 0344 0083 017d  .f.d.d...|.D...}
+00001020: 057c 0464 0519 0064 0075 0072 5874 0364  .|.d...d.u.rXt.d
+00001030: 067c 039b 009d 0283 0182 017c 0464 0719  .|.........|.d..
+00001040: 0064 0075 0072 7274 0364 087c 039b 009d  .d.u.rrt.d.|....
+00001050: 0283 0182 017c 0464 0519 006a 0464 096b  .....|.d...j.d.k
+00001060: 0372 9474 0364 0a7c 0364 0519 009b 0064  .r.t.d.|.d.....d
+00001070: 0b9d 0383 0182 017c 0464 0719 006a 0464  .......|.d...j.d
+00001080: 0c6b 0372 b674 0364 0a7c 0364 0719 009b  .k.r.t.d.|.d....
+00001090: 0064 0d9d 0383 0182 017c 0464 0519 006a  .d.......|.d...j
+000010a0: 057d 0674 067c 0564 0519 0083 017d 0774  .}.t.|.d.....}.t
+000010b0: 067c 0564 0719 0083 017d 087c 01a0 0774  .|.d.....}.|...t
+000010c0: 087c 067c 077c 0864 0e8d 03a1 0101 0071  .|.|.|.d.......q
+000010d0: 1a7c 0153 0029 0f4e e903 0000 0063 0100  .|.S.).N.....c..
+000010e0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000010f0: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
+00001100: 0c7d 0174 007c 0183 0191 0271 0453 0072  .}.t.|.....q.S.r
+00001110: 0d00 0000 2901 7242 0000 00a9 0272 1200  ....).rB.....r..
+00001120: 0000 723c 0000 0072 0d00 0000 720d 0000  ..r<...r....r...
+00001130: 0072 0e00 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00001140: 703e 6700 0000 f300 0000 007a 275f 7061  p>g........z'_pa
+00001150: 7273 655f 6261 7965 7372 756e 5f72 6f77  rse_bayesrun_row
+00001160: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00001170: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+00001180: 0002 0000 0004 0000 0013 0000 0073 1400  .............s..
+00001190: 0000 6700 7c00 5d0c 7d01 8800 7c01 1900  ..g.|.].}...|...
+000011a0: 9102 7104 5300 720d 0000 0072 0d00 0000  ..q.S.r....r....
+000011b0: 7245 0000 00a9 0172 4300 0000 720d 0000  rE.....rC...r...
+000011c0: 0072 0e00 0000 7246 0000 0068 0000 0072  .r....rF...h...r
+000011d0: 4700 0000 7201 0000 007a 256e 6f20 7669  G...r....z%no vi
+000011e0: 6162 6c65 2073 7563 6365 7373 2072 6f77  able success row
+000011f0: 2066 6f75 6e64 2066 6f72 206b 6579 7320   found for keys 
+00001200: 7235 0000 007a 236e 6f20 7669 6162 6c65  r5...z#no viable
+00001210: 2063 6f75 6e74 2072 6f77 2066 6f75 6e64   count row found
+00001220: 2066 6f72 206b 6579 7320 722c 0000 007a   for keys r,...z
+00001230: 0b54 6865 2063 6f6c 756d 6e20 7a17 2069  .The column z. i
+00001240: 7320 6e6f 7420 6120 7375 6363 6573 7320  s not a success 
+00001250: 6669 656c 6472 2d00 0000 7a15 2069 7320  fieldr-...z. is 
+00001260: 6e6f 7420 6120 636f 756e 7420 6669 656c  not a count fiel
+00001270: 6429 0372 2b00 0000 722c 0000 0072 2d00  d).r+...r,...r-.
+00001280: 0000 2909 723b 0000 00da 046c 6973 74da  ..).r;.....list.
+00001290: 046b 6579 73da 0a56 616c 7565 4572 726f  .keys..ValueErro
+000012a0: 7272 1600 0000 7218 0000 0072 2e00 0000  rr....r....r....
+000012b0: da06 6170 7065 6e64 722a 0000 0029 0972  ..appendr*...).r
+000012c0: 4300 0000 7232 0000 005a 0c62 6174 6368  C...r2...Z.batch
+000012d0: 6564 5f6b 6579 735a 0a6d 6f64 656c 5f6b  ed_keysZ.model_k
+000012e0: 6579 73da 0670 6172 7365 64da 0676 616c  eys..parsed..val
+000012f0: 7565 735a 0b70 6172 7365 645f 6b65 7973  uesZ.parsed_keys
+00001300: 722c 0000 0072 2d00 0000 720d 0000 0072  r,...r-...r....r
+00001310: 4800 0000 720e 0000 00da 135f 7061 7273  H...r......_pars
+00001320: 655f 6261 7965 7372 756e 5f72 6f77 6000  e_bayesrun_row`.
+00001330: 0000 7330 0000 0000 0404 0112 0108 010e  ..s0............
+00001340: 0112 010c 010e 010c 010e 010e 0114 010e  ................
+00001350: 0114 010a 010c 010c 0104 0102 0102 0102  ................
+00001360: 0102 fd04 ff06 0772 4f00 0000 2902 da04  .......rO...)...
+00001370: 6669 6c65 723d 0000 0063 0100 0000 0000  filer=...c......
+00001380: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+00001390: 0000 7342 0000 007c 006a 007d 0174 01a0  ..sB...|.j.}.t..
+000013a0: 0274 037c 01a1 027d 027c 0273 2474 047c  .t.|...}.|.s$t.|
+000013b0: 019b 0064 019d 0283 0182 017c 02a0 05a1  ...d.......|....
+000013c0: 007d 0374 067c 0364 0219 007c 0364 0319  .}.t.|.d...|.d..
+000013d0: 007c 0064 048d 0353 0029 054e 7a20 2077  .|.d...S.).Nz  w
+000013e0: 6173 206e 6f74 2061 2076 616c 6964 2062  as not a valid b
+000013f0: 6179 6573 7275 6e20 6f75 7470 7574 7203  ayesrun outputr.
+00001400: 0000 0072 0400 0000 2903 7203 0000 0072  ...r....).r....r
+00001410: 0400 0000 7205 0000 0029 07da 046e 616d  ....r....)...nam
+00001420: 6572 3f00 0000 7240 0000 00da 0e46 494c  er?...r@.....FIL
+00001430: 454e 414d 455f 5245 4745 5872 4b00 0000  ENAME_REGEXrK...
+00001440: 7210 0000 0072 0200 0000 2904 7250 0000  r....r....).rP..
+00001450: 0072 3000 0000 7240 0000 00da 0667 726f  .r0...r@.....gro
+00001460: 7570 7372 0d00 0000 720d 0000 0072 0e00  upsr....r....r..
+00001470: 0000 da16 5f70 6172 7365 5f6f 7574 7075  ...._parse_outpu
+00001480: 745f 6669 6c65 6e61 6d65 7e00 0000 7310  t_filename~...s.
+00001490: 0000 0000 0106 010c 0104 010e 0108 0102  ................
+000014a0: 010e ff72 5400 0000 2902 da04 736c 7567  ...rT...)...slug
+000014b0: 723d 0000 0063 0100 0000 0000 0000 0000  r=...c..........
+000014c0: 0000 0300 0000 0500 0000 4300 0000 732a  ..........C...s*
+000014d0: 0000 0074 0044 005d 207d 0174 01a0 027c  ...t.D.] }.t...|
+000014e0: 017c 00a1 027d 027c 0272 047c 02a0 03a1  .|...}.|.r.|....
+000014f0: 0002 0001 0053 0071 0464 0053 0072 2200  .....S.q.d.S.r".
+00001500: 0000 2904 da11 4649 4c45 5f53 4c55 475f  ..)...FILE_SLUG_
+00001510: 5245 4745 5845 5372 3f00 0000 7240 0000  REGEXESr?...r@..
+00001520: 0072 1000 0000 2903 7255 0000 0072 4100  .r....).rU...rA.
+00001530: 0000 7240 0000 0072 0d00 0000 720d 0000  ..r@...r....r...
+00001540: 0072 0e00 0000 da10 5f70 6172 7365 5f66  .r......_parse_f
+00001550: 696c 655f 736c 7567 8900 0000 730a 0000  ile_slug....s...
+00001560: 0000 0108 010c 0104 010e 0272 5700 0000  ...........rW...
+00001570: 2903 7250 0000 00da 0a69 6e64 6578 6966  ).rP.....indexif
+00001580: 6965 7272 3d00 0000 6302 0000 0000 0000  ierr=...c.......
+00001590: 0000 0000 000d 0000 0008 0000 0043 0000  .............C..
+000015a0: 0073 2c01 0000 7400 7c00 8301 0400 7d02  .s,...t.|.....}.
+000015b0: 7d03 7401 7c02 6900 6700 6401 8d03 7d04  }.t.|.i.g.d...}.
+000015c0: 7c04 6a02 a003 7404 a005 7c03 a101 a101  |.j...t...|.....
+000015d0: 0100 7406 7c02 6a07 8301 7d05 7c05 6400  ..t.|.j...}.|.d.
+000015e0: 7500 7252 7408 a009 6402 7c03 9b00 6403  u.rRt...d.|...d.
+000015f0: 9d03 a101 0100 6e60 7c04 6a02 a003 7c05  ......n`|.j...|.
+00001600: a101 0100 7c01 6400 7501 72b2 7a26 7c05  ....|.d.u.r.z&|.
+00001610: 6404 1900 7d06 7c01 a00a 740b 7c06 8301  d...}.|...t.|...
+00001620: a101 7d07 7c04 6a02 a003 7c07 a101 0100  ..}.|.j...|.....
+00001630: 5700 6e24 0400 740c 79b0 0100 0100 0100  W.n$..t.y.......
+00001640: 7408 a009 6405 7c05 9b00 6406 9d03 a101  t...d.|...d.....
+00001650: 0100 5900 6e02 3000 7c00 a00d a100 8f4e  ..Y.n.0.|......N
+00001660: 7d08 740e a00f 7c08 a101 7d09 6407 6408  }.t...|...}.d.d.
+00001670: 8400 7c09 4400 8301 7d0a 7410 7c0a 8301  ..|.D...}.t.|...
+00001680: 6409 6b02 72ea 7c0a 640a 1900 7d0b 6e10  d.k.r.|.d...}.n.
+00001690: 7411 640b 7c00 6a12 9b00 9d02 8301 8201  t.d.|.j.........
+000016a0: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
+000016b0: 9001 7310 3000 0100 0100 0100 5900 0100  ..s.0.......Y...
+000016c0: 7413 7c0b 8301 7d0c 7c0c 7c04 5f14 7c04  t.|...}.|.|._.|.
+000016d0: 5300 290c 4e29 0372 3000 0000 7231 0000  S.).N).r0...r1..
+000016e0: 0072 3200 0000 7a10 436f 756c 6420 6e6f  .r2...z.Could no
+000016f0: 7420 7061 7273 6520 7a38 2061 6761 696e  t parse z8 again
+00001700: 7374 2061 6e79 206d 6174 6368 696e 6720  st any matching 
+00001710: 7265 6765 7865 732e 2047 6f69 6e67 2074  regexes. Going t
+00001720: 6f20 736b 6970 2074 6167 2070 6172 7369  o skip tag parsi
+00001730: 6e67 da09 6a6f 625f 696e 6465 787a 0e50  ng..job_indexz.P
+00001740: 6172 7365 6420 7461 6720 746f 207a 522c  arsed tag to zR,
+00001750: 2061 6e64 2061 7474 656d 7074 6564 2074   and attempted t
+00001760: 6f20 696e 6465 7869 6679 2062 7574 206e  o indexify but n
+00001770: 6f20 6a6f 625f 696e 6465 7820 6b65 7920  o job_index key 
+00001780: 7761 7320 666f 756e 642e 2073 6b69 7070  was found. skipp
+00001790: 696e 6720 616e 6420 6d6f 7669 6e67 206f  ing and moving o
+000017a0: 6e63 0100 0000 0000 0000 0000 0000 0200  nc..............
+000017b0: 0000 0300 0000 5300 0000 7310 0000 0067  ......S...s....g
+000017c0: 007c 005d 087d 017c 0191 0271 0453 0072  .|.].}.|...q.S.r
+000017d0: 0d00 0000 720d 0000 0029 0272 1200 0000  ....r....).r....
+000017e0: da01 7272 0d00 0000 720d 0000 0072 0e00  ..rr....r....r..
+000017f0: 0000 7246 0000 00ae 0000 0072 4700 0000  ..rF.......rG...
+00001800: 7a24 7265 6164 5f6f 7574 7075 745f 6669  z$read_output_fi
+00001810: 6c65 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  le.<locals>.<lis
+00001820: 7463 6f6d 703e 7235 0000 0072 0100 0000  tcomp>r5...r....
+00001830: 7a27 436f 6e66 7573 6564 2061 626f 7574  z'Confused about
+00001840: 2068 6176 696e 6720 6d75 6c74 6970 6c65   having multiple
+00001850: 2072 6f77 7320 696e 2029 1572 5400 0000   rows in ).rT...
+00001860: 722f 0000 0072 3100 0000 da06 7570 6461  r/...r1.....upda
+00001870: 7465 da0b 6461 7461 636c 6173 7365 73da  te..dataclasses.
+00001880: 0661 7364 6963 7472 5700 0000 7204 0000  .asdictrW...r...
+00001890: 00da 075f 6c6f 6767 6572 da07 7761 726e  ..._logger..warn
+000018a0: 696e 67da 0869 6e64 6578 6966 7972 2e00  ing..indexifyr..
+000018b0: 0000 da08 4b65 7945 7272 6f72 da04 6f70  ....KeyError..op
+000018c0: 656e da03 6373 76da 0a44 6963 7452 6561  en..csv..DictRea
+000018d0: 6465 7272 3700 0000 724b 0000 0072 5100  derr7...rK...rQ.
+000018e0: 0000 724f 0000 0072 3200 0000 290d 7250  ..rO...r2...).rP
+000018f0: 0000 0072 5800 0000 5a0f 7061 7273 6564  ...rX...Z.parsed
+00001900: 5f66 696c 656e 616d 65da 0374 6167 da03  _filename..tag..
+00001910: 6f75 745a 0a70 6172 7365 645f 7461 6772  outZ.parsed_tagr
+00001920: 5900 0000 5a0a 696e 6465 7869 6669 6564  Y...Z.indexified
+00001930: 5a0a 696e 7075 745f 6669 6c65 da06 7265  Z.input_file..re
+00001940: 6164 6572 da04 726f 7773 7243 0000 0072  ader..rowsrC...r
+00001950: 3200 0000 720d 0000 0072 0d00 0000 720e  2...r....r....r.
+00001960: 0000 00da 1072 6561 645f 6f75 7470 7574  .....read_output
+00001970: 5f66 696c 6592 0000 0073 3600 0000 0004  _file....s6.....
+00001980: 0c01 0e02 1201 0a01 0801 0401 0aff 0604  ................
+00001990: 0c01 0801 0201 0801 0e01 1001 0c02 0401  ................
+000019a0: 0aff 0a04 0a01 0a01 0e01 0c01 0a02 3001  ..............0.
+000019b0: 0802 0602 7269 0000 0029 0172 3500 0000  ....ri...).r5...
+000019c0: 2920 725c 0000 0072 3f00 0000 7228 0000  ) r\...r?...r(..
+000019d0: 00da 076c 6f67 6769 6e67 da10 6465 6570  ...logging..deep
+000019e0: 646f 672e 696e 6465 7869 6679 da07 6465  dog.indexify..de
+000019f0: 6570 646f 6772 0b00 0000 7263 0000 00da  epdogr....rc....
+00001a00: 0967 6574 4c6f 6767 6572 7206 0000 0072  .getLoggerr....r
+00001a10: 5e00 0000 7252 0000 0072 3e00 0000 7256  ^...rR...r>...rV
+00001a20: 0000 00da 0964 6174 6163 6c61 7373 7202  .....dataclassr.
+00001a30: 0000 0072 0f00 0000 722a 0000 0072 2f00  ...r....r*...r/.
+00001a40: 0000 723b 0000 0072 0900 0000 da08 4f70  ..r;...r......Op
+00001a50: 7469 6f6e 616c 7242 0000 0072 2900 0000  tionalrB...r)...
+00001a60: 7234 0000 0072 4f00 0000 720c 0000 0072  r4...rO...r....r
+00001a70: 5400 0000 7257 0000 0072 6000 0000 da0a  T...rW...r`.....
+00001a80: 496e 6465 7869 6669 6572 7269 0000 0072  Indexifierri...r
+00001a90: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+00001aa0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00001ab0: 0073 3a00 0000 0801 0801 0801 0801 0801  .s:.............
+00001ac0: 0801 0802 0a02 0402 0806 0807 0401 1006  ................
+00001ad0: 0e1a 0401 1006 0401 1006 0a09 0201 08fe  ................
+00001ae0: 0c10 0c01 08fe 0c1e 120b 200a 1001 02fe  .......... .....
```

### Comparing `deepdog-1.1.0/deepdog/subset_simulation/subset_simulation_impl.py` & `deepdog-1.2.0/deepdog/subset_simulation/subset_simulation_impl.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.1.0/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-1.2.0/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-1.1.0/pyproject.toml` & `deepdog-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepdog"
-version = "1.1.0"
+version = "1.2.0"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 pdme = "^1.2.0"
 numpy = "1.22.3"
```


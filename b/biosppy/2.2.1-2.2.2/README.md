# Comparing `tmp/biosppy-2.2.1.tar.gz` & `tmp/biosppy-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosppy-2.2.1.tar", last modified: Tue Apr 23 15:26:31 2024, max compression
+gzip compressed data, was "biosppy-2.2.2.tar", last modified: Thu May  9 12:35:50 2024, max compression
```

## Comparing `biosppy-2.2.1.tar` & `biosppy-2.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.157666 biosppy-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-23 15:26:27.000000 biosppy-2.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-23 15:26:27.000000 biosppy-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-23 15:26:27.000000 biosppy-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-23 15:26:31.157666 biosppy-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-23 15:26:27.000000 biosppy-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.153666 biosppy-2.2.1/biosppy/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63249 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/biometrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    28599 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.153666 biosppy-2.2.1/biosppy/features/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/cepstral.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/phase_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/features/time_freq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.153666 biosppy-2.2.1/biosppy/inter_plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/inter_plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/inter_plotting/acc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/inter_plotting/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    72253 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11234 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/quality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.157666 biosppy-2.2.1/biosppy/signals/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/abp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/acc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/bvp.py
--rw-r--r--   0 runner    (1001) docker     (127)    65972 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/eda.py
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/eeg.py
--rw-r--r--   0 runner    (1001) docker     (127)    41783 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/emg.py
--rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/hrv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/pcg.py
--rw-r--r--   0 runner    (1001) docker     (127)    18044 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/ppg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/resp.py
--rw-r--r--   0 runner    (1001) docker     (127)    58646 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/signals/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    25139 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.157666 biosppy-2.2.1/biosppy/synthesizers/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20118 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/synthesizers/ecg.py
--rw-r--r--   0 runner    (1001) docker     (127)    29270 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/synthesizers/emg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-04-23 15:26:27.000000 biosppy-2.2.1/biosppy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:26:31.157666 biosppy-2.2.1/biosppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 15:26:31.000000 biosppy-2.2.1/biosppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 15:26:31.157666 biosppy-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-23 15:26:27.000000 biosppy-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:50.828125 biosppy-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-09 12:35:37.000000 biosppy-2.2.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-09 12:35:37.000000 biosppy-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 12:35:37.000000 biosppy-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-09 12:35:50.828125 biosppy-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-09 12:35:37.000000 biosppy-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:50.820125 biosppy-2.2.2/biosppy/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63249 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/biometrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28599 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:50.824125 biosppy-2.2.2/biosppy/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/features/cepstral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/features/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/features/phase_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/features/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/features/time_freq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:50.824125 biosppy-2.2.2/biosppy/inter_plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/inter_plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/inter_plotting/acc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/inter_plotting/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72253 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11234 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/quality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:50.828125 biosppy-2.2.2/biosppy/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/abp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/acc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/bvp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65984 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23763 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/eda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/eeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41783 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/emg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29473 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/hrv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/pcg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18044 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/ppg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/resp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58646 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/signals/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9686 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25139 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:50.828125 biosppy-2.2.2/biosppy/synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20118 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/synthesizers/ecg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29270 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/synthesizers/emg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-05-09 12:35:37.000000 biosppy-2.2.2/biosppy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:35:50.828125 biosppy-2.2.2/biosppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-05-09 12:35:50.000000 biosppy-2.2.2/biosppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-09 12:35:50.000000 biosppy-2.2.2/biosppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:35:50.000000 biosppy-2.2.2/biosppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 12:35:50.000000 biosppy-2.2.2/biosppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 12:35:50.000000 biosppy-2.2.2/biosppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 12:35:50.828125 biosppy-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-09 12:35:37.000000 biosppy-2.2.2/setup.py
```

### Comparing `biosppy-2.2.1/AUTHORS.md` & `biosppy-2.2.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/LICENSE` & `biosppy-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/PKG-INFO` & `biosppy-2.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosppy
-Version: 2.2.1
+Version: 2.2.2
 Summary: A toolbox for biosignal processing written in Python.
 Home-page: https://github.com/scientisst/BioSPPy
 Author: Instituto de Telecomunicacoes
 Author-email: developer@scientisst.com
 License: BSD 3-clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -147,14 +147,17 @@
     doi = {https://doi.org/10.1016/j.softx.2024.101712},
     url = {https://www.sciencedirect.com/science/article/pii/S2352711024000839},
 }
 ```
 
 However, if you want to cite a specific version of BioSPPy, you can use Zenodo's DOI:
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11048615.svg)](https://doi.org/10.5281/zenodo.11048615)
+
+
 ## License
 BioSPPy is released under the BSD 3-clause license. See LICENSE for more details.
 
 ## Disclaimer
 
 This program is distributed in the hope it will be useful and provided
 to you "as is", but WITHOUT ANY WARRANTY, without even the implied
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biosppy Version: 2.2.1 Summary: A toolbox for
+Metadata-Version: 2.1 Name: biosppy Version: 2.2.2 Summary: A toolbox for
 biosignal processing written in Python. Home-page: https://github.com/
 scientisst/BioSPPy Author: Instituto de Telecomunicacoes Author-email:
 developer@scientisst.com License: BSD 3-clause Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -52,18 +52,19 @@
 vol. 26, pp. 101712, 2024, doi: 10.1016/j.softx.2024.101712. ```latex @article
 {biosppy, title = {BioSPPy: A Python toolbox for physiological signal
 processing}, author = {PatrÃ­cia Bota and Rafael Silva and Carlos Carreiras and
 Ana Fred and Hugo PlÃ¡cido {da Silva}}, journal = {SoftwareX}, volume = {26},
 pages = {101712}, year = {2024}, issn = {2352-7110}, doi = {https://doi.org/
 10.1016/j.softx.2024.101712}, url = {https://www.sciencedirect.com/science/
 article/pii/S2352711024000839}, } ``` However, if you want to cite a specific
-version of BioSPPy, you can use Zenodo's DOI: ## License BioSPPy is released
-under the BSD 3-clause license. See LICENSE for more details. ## Disclaimer
-This program is distributed in the hope it will be useful and provided to you
-"as is", but WITHOUT ANY WARRANTY, without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is NOT
-intended for medical diagnosis. We expressly disclaim any liability whatsoever
-for any direct, indirect, consequential, incidental or special damages,
-including, without limitation, lost revenues, lost profits, losses resulting
-from business interruption or loss of data, regardless of the form of action or
-legal theory under which the liability may be asserted, even if advised of the
-possibility of such damages.
+version of BioSPPy, you can use Zenodo's DOI: [![DOI](https://zenodo.org/badge/
+DOI/10.5281/zenodo.11048615.svg)](https://doi.org/10.5281/zenodo.11048615) ##
+License BioSPPy is released under the BSD 3-clause license. See LICENSE for
+more details. ## Disclaimer This program is distributed in the hope it will be
+useful and provided to you "as is", but WITHOUT ANY WARRANTY, without even the
+implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This
+program is NOT intended for medical diagnosis. We expressly disclaim any
+liability whatsoever for any direct, indirect, consequential, incidental or
+special damages, including, without limitation, lost revenues, lost profits,
+losses resulting from business interruption or loss of data, regardless of the
+form of action or legal theory under which the liability may be asserted, even
+if advised of the possibility of such damages.
```

### Comparing `biosppy-2.2.1/README.md` & `biosppy-2.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,17 @@
     doi = {https://doi.org/10.1016/j.softx.2024.101712},
     url = {https://www.sciencedirect.com/science/article/pii/S2352711024000839},
 }
 ```
 
 However, if you want to cite a specific version of BioSPPy, you can use Zenodo's DOI:
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11048615.svg)](https://doi.org/10.5281/zenodo.11048615)
+
+
 ## License
 BioSPPy is released under the BSD 3-clause license. See LICENSE for more details.
 
 ## Disclaimer
 
 This program is distributed in the hope it will be useful and provided
 to you "as is", but WITHOUT ANY WARRANTY, without even the implied
```

#### html2text {}

```diff
@@ -35,18 +35,19 @@
 vol. 26, pp. 101712, 2024, doi: 10.1016/j.softx.2024.101712. ```latex @article
 {biosppy, title = {BioSPPy: A Python toolbox for physiological signal
 processing}, author = {PatrÃ­cia Bota and Rafael Silva and Carlos Carreiras and
 Ana Fred and Hugo PlÃ¡cido {da Silva}}, journal = {SoftwareX}, volume = {26},
 pages = {101712}, year = {2024}, issn = {2352-7110}, doi = {https://doi.org/
 10.1016/j.softx.2024.101712}, url = {https://www.sciencedirect.com/science/
 article/pii/S2352711024000839}, } ``` However, if you want to cite a specific
-version of BioSPPy, you can use Zenodo's DOI: ## License BioSPPy is released
-under the BSD 3-clause license. See LICENSE for more details. ## Disclaimer
-This program is distributed in the hope it will be useful and provided to you
-"as is", but WITHOUT ANY WARRANTY, without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is NOT
-intended for medical diagnosis. We expressly disclaim any liability whatsoever
-for any direct, indirect, consequential, incidental or special damages,
-including, without limitation, lost revenues, lost profits, losses resulting
-from business interruption or loss of data, regardless of the form of action or
-legal theory under which the liability may be asserted, even if advised of the
-possibility of such damages.
+version of BioSPPy, you can use Zenodo's DOI: [![DOI](https://zenodo.org/badge/
+DOI/10.5281/zenodo.11048615.svg)](https://doi.org/10.5281/zenodo.11048615) ##
+License BioSPPy is released under the BSD 3-clause license. See LICENSE for
+more details. ## Disclaimer This program is distributed in the hope it will be
+useful and provided to you "as is", but WITHOUT ANY WARRANTY, without even the
+implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This
+program is NOT intended for medical diagnosis. We expressly disclaim any
+liability whatsoever for any direct, indirect, consequential, incidental or
+special damages, including, without limitation, lost revenues, lost profits,
+losses resulting from business interruption or loss of data, regardless of the
+form of action or legal theory under which the liability may be asserted, even
+if advised of the possibility of such damages.
```

### Comparing `biosppy-2.2.1/biosppy/__init__.py` & `biosppy-2.2.2/biosppy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 
 # get version
 from .__version__ import __version__
 
 # allow lazy loading
 from .signals import acc, abp, bvp, ppg, pcg, ecg, eda, eeg, emg, resp, tools, hrv
 from .synthesizers import ecg, emg
-from .inter_plotting import ecg, acc
+# from .inter_plotting import ecg, acc
 from .features import frequency, time, time_freq, cepstral, phase_space
```

### Comparing `biosppy-2.2.1/biosppy/biometrics.py` & `biosppy-2.2.2/biosppy/biometrics.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/clustering.py` & `biosppy-2.2.2/biosppy/clustering.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/features/__init__.py` & `biosppy-2.2.2/biosppy/features/__init__.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/features/cepstral.py` & `biosppy-2.2.2/biosppy/features/cepstral.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/features/frequency.py` & `biosppy-2.2.2/biosppy/features/frequency.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/features/phase_space.py` & `biosppy-2.2.2/biosppy/features/phase_space.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/features/time.py` & `biosppy-2.2.2/biosppy/features/time.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/features/time_freq.py` & `biosppy-2.2.2/biosppy/features/time_freq.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/inter_plotting/acc.py` & `biosppy-2.2.2/biosppy/inter_plotting/acc.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/inter_plotting/ecg.py` & `biosppy-2.2.2/biosppy/inter_plotting/ecg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/metrics.py` & `biosppy-2.2.2/biosppy/metrics.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/plotting.py` & `biosppy-2.2.2/biosppy/plotting.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/quality.py` & `biosppy-2.2.2/biosppy/quality.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/__init__.py` & `biosppy-2.2.2/biosppy/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/abp.py` & `biosppy-2.2.2/biosppy/signals/abp.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/acc.py` & `biosppy-2.2.2/biosppy/signals/acc.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import warnings
 
 # 3rd party
 import numpy as np
 
 # local
 from .. import plotting, utils
-from biosppy.inter_plotting import acc as inter_plotting
 
 
 def acc(signal=None, sampling_rate=100.0, units=None, path=None, show=True, interactive=False):
     """Process a raw ACC signal and extract relevant signal features using
     default parameters.
 
     Parameters
@@ -84,14 +83,15 @@
     length = len(signal)
     T = (length - 1) / sampling_rate
     ts = np.linspace(0, T, length, endpoint=True)
 
     # plot
     if show:
         if interactive:
+            from biosppy.inter_plotting import acc as inter_plotting
             inter_plotting.plot_acc(
                 ts=ts,  # plotting.plot_acc
                 raw=signal,
                 vm=vm_features,
                 sm=sm_features,
                 spectrum={"freq": freq_features, "abs_amp": abs_amp_features},
                 path=path,
```

### Comparing `biosppy-2.2.1/biosppy/signals/bvp.py` & `biosppy-2.2.2/biosppy/signals/bvp.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/ecg.py` & `biosppy-2.2.2/biosppy/signals/ecg.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import scipy.signal as ss
 import matplotlib.pyplot as plt
 from scipy import stats, integrate
 
 # local
 from . import tools as st
 from .. import plotting, utils
-from biosppy.inter_plotting import ecg as inter_plotting
 from scipy.signal import argrelextrema
 
 
 def ecg(signal=None, sampling_rate=1000.0, units=None, path=None, show=True, interactive=False):
     """Process a raw ECG signal and extract relevant signal features using
     default parameters.
 
@@ -119,14 +118,15 @@
     ts = np.linspace(0, T, length, endpoint=True)
     ts_hr = ts[hr_idx]
     ts_tmpl = np.linspace(-0.2, 0.4, templates.shape[1], endpoint=False)
 
     # plot
     if show:
         if interactive:
+            from biosppy.inter_plotting import ecg as inter_plotting
             inter_plotting.plot_ecg(
                 ts=ts,
                 raw=signal,
                 filtered=filtered,
                 rpeaks=rpeaks,
                 templates_ts=ts_tmpl,
                 templates=templates,
```

### Comparing `biosppy-2.2.1/biosppy/signals/eda.py` & `biosppy-2.2.2/biosppy/signals/eda.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from scipy import interpolate
 
 # local
 from . import tools as st
 from .. import plotting, utils
 
 
-def eda(signal=None, sampling_rate=1000., units=None, path=None, show=True):
+def eda(signal=None, sampling_rate=1000., units=None, path=None, show=True, min_amplitude=0.1, size=0.9):
     """Process a raw EDA signal and extract relevant signal features using
     default parameters.
 
     Parameters
     ----------
     signal : array
         Raw EDA signal.
@@ -37,14 +37,18 @@
     units : str, optional
         The units of the input signal. If specified, the plot will have the
         y-axis labeled with the corresponding units.
     path : str, optional
         If provided, the plot will be saved to the specified file.
     show : bool, optional
         If True, show a summary plot.
+    min_amplitude : float, optional
+        Minimum threshold by which to exclude SCRs.
+    size : float, optional
+        Size of the filter applied to exluced SCRs.
 
     Returns
     -------
     ts : array
         Signal time axis reference (seconds).
     filtered : array
         Filtered EDA signal.
@@ -86,15 +90,15 @@
                               kernel="boxzen",
                               size=sm_size,
                               mirror=True)
 
     # get SCR info
     onsets, peaks, amplitudes, phasic_rate, rise_times, half_rec, six_rec = eda_events(signal=filtered,
                                                                                        sampling_rate=sampling_rate,
-                                                                                       min_amplitude=0.1, size=0.9)
+                                                                                       min_amplitude=min_amplitude, size=size)
 
     # get time vectors
     length = len(signal)
     t = (length - 1) / sampling_rate
     ts = np.linspace(0, t, length, endpoint=True)
 
     # get EDR and EDL
@@ -180,14 +184,18 @@
                                       **kwargs)
 
     elif method == "basic":
         onsets, peaks, amps = basic_scr(signal=signal)
 
     else:
         raise TypeError("Please specify a supported method.")
+    
+    # sanity check
+    if len(onsets) == 0:
+        raise ValueError("Could not find SCR pulses.")
 
     # compute phasic rate
     try:
         phasic_rate = sampling_rate * (60. / np.diff(peaks))
     except Exception as e:
         print(e)
         phasic_rate = None
@@ -670,15 +678,18 @@
             
         pk = st.find_extrema(signal=s, mode='max')[0]  # get pk between events
         for p in pk:
             if (s[p] - s[0]) > min_amplitude:  # only count events with minimum amplitude
                 peaks += [zeros[z] + p]
                 onsets += [zeros[z]]
                 amps += [s[p] - s[0]]
-
+    # sanity check
+    if len(onsets) == 0:
+        raise ValueError("Could not find SCR pulses. Try to adjust min_amplitude or the filter size.")
+    
     # convert to array
     onsets, peaks, amps = np.array(onsets), np.array(peaks), np.array(amps)
 
     # output
     args = (onsets, peaks, amps)
     names = ("onsets", "peaks", "amplitudes")
```

### Comparing `biosppy-2.2.1/biosppy/signals/eeg.py` & `biosppy-2.2.2/biosppy/signals/eeg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/emg.py` & `biosppy-2.2.2/biosppy/signals/emg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/hrv.py` & `biosppy-2.2.2/biosppy/signals/hrv.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/pcg.py` & `biosppy-2.2.2/biosppy/signals/pcg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/ppg.py` & `biosppy-2.2.2/biosppy/signals/ppg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/resp.py` & `biosppy-2.2.2/biosppy/signals/resp.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/signals/tools.py` & `biosppy-2.2.2/biosppy/signals/tools.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/stats.py` & `biosppy-2.2.2/biosppy/stats.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/storage.py` & `biosppy-2.2.2/biosppy/storage.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/synthesizers/ecg.py` & `biosppy-2.2.2/biosppy/synthesizers/ecg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/synthesizers/emg.py` & `biosppy-2.2.2/biosppy/synthesizers/emg.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/timing.py` & `biosppy-2.2.2/biosppy/timing.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy/utils.py` & `biosppy-2.2.2/biosppy/utils.py`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/biosppy.egg-info/PKG-INFO` & `biosppy-2.2.2/biosppy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biosppy
-Version: 2.2.1
+Version: 2.2.2
 Summary: A toolbox for biosignal processing written in Python.
 Home-page: https://github.com/scientisst/BioSPPy
 Author: Instituto de Telecomunicacoes
 Author-email: developer@scientisst.com
 License: BSD 3-clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -147,14 +147,17 @@
     doi = {https://doi.org/10.1016/j.softx.2024.101712},
     url = {https://www.sciencedirect.com/science/article/pii/S2352711024000839},
 }
 ```
 
 However, if you want to cite a specific version of BioSPPy, you can use Zenodo's DOI:
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11048615.svg)](https://doi.org/10.5281/zenodo.11048615)
+
+
 ## License
 BioSPPy is released under the BSD 3-clause license. See LICENSE for more details.
 
 ## Disclaimer
 
 This program is distributed in the hope it will be useful and provided
 to you "as is", but WITHOUT ANY WARRANTY, without even the implied
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: biosppy Version: 2.2.1 Summary: A toolbox for
+Metadata-Version: 2.1 Name: biosppy Version: 2.2.2 Summary: A toolbox for
 biosignal processing written in Python. Home-page: https://github.com/
 scientisst/BioSPPy Author: Instituto de Telecomunicacoes Author-email:
 developer@scientisst.com License: BSD 3-clause Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -52,18 +52,19 @@
 vol. 26, pp. 101712, 2024, doi: 10.1016/j.softx.2024.101712. ```latex @article
 {biosppy, title = {BioSPPy: A Python toolbox for physiological signal
 processing}, author = {PatrÃ­cia Bota and Rafael Silva and Carlos Carreiras and
 Ana Fred and Hugo PlÃ¡cido {da Silva}}, journal = {SoftwareX}, volume = {26},
 pages = {101712}, year = {2024}, issn = {2352-7110}, doi = {https://doi.org/
 10.1016/j.softx.2024.101712}, url = {https://www.sciencedirect.com/science/
 article/pii/S2352711024000839}, } ``` However, if you want to cite a specific
-version of BioSPPy, you can use Zenodo's DOI: ## License BioSPPy is released
-under the BSD 3-clause license. See LICENSE for more details. ## Disclaimer
-This program is distributed in the hope it will be useful and provided to you
-"as is", but WITHOUT ANY WARRANTY, without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This program is NOT
-intended for medical diagnosis. We expressly disclaim any liability whatsoever
-for any direct, indirect, consequential, incidental or special damages,
-including, without limitation, lost revenues, lost profits, losses resulting
-from business interruption or loss of data, regardless of the form of action or
-legal theory under which the liability may be asserted, even if advised of the
-possibility of such damages.
+version of BioSPPy, you can use Zenodo's DOI: [![DOI](https://zenodo.org/badge/
+DOI/10.5281/zenodo.11048615.svg)](https://doi.org/10.5281/zenodo.11048615) ##
+License BioSPPy is released under the BSD 3-clause license. See LICENSE for
+more details. ## Disclaimer This program is distributed in the hope it will be
+useful and provided to you "as is", but WITHOUT ANY WARRANTY, without even the
+implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This
+program is NOT intended for medical diagnosis. We expressly disclaim any
+liability whatsoever for any direct, indirect, consequential, incidental or
+special damages, including, without limitation, lost revenues, lost profits,
+losses resulting from business interruption or loss of data, regardless of the
+form of action or legal theory under which the liability may be asserted, even
+if advised of the possibility of such damages.
```

### Comparing `biosppy-2.2.1/biosppy.egg-info/SOURCES.txt` & `biosppy-2.2.2/biosppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biosppy-2.2.1/setup.py` & `biosppy-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # Package meta-data.
 NAME = 'biosppy'
 DESCRIPTION = 'A toolbox for biosignal processing written in Python.'
 URL = 'https://github.com/scientisst/BioSPPy'
 EMAIL = 'developer@scientisst.com'
 AUTHOR = 'Instituto de Telecomunicacoes'
 REQUIRES_PYTHON = '>3.5.2'
-VERSION = '2.2.1'
+VERSION = '2.2.2'
 LICENSE = 'BSD 3-clause'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'bidict',
     'h5py',
     'matplotlib',
```


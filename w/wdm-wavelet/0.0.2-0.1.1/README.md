# Comparing `tmp/wdm-wavelet-0.0.2.tar.gz` & `tmp/wdm_wavelet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wdm-wavelet-0.0.2.tar", last modified: Mon Feb  5 10:55:14 2024, max compression
+gzip compressed data, was "wdm_wavelet-0.1.1.tar", last modified: Thu May  9 08:06:23 2024, max compression
```

## Comparing `wdm-wavelet-0.0.2.tar` & `wdm_wavelet-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:55:14.916170 wdm-wavelet-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    35065 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/Makefile
--rw-r--r--   0 root         (0) root         (0)      642 2024-02-05 10:55:14.916170 wdm-wavelet-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:55:14.912170 wdm-wavelet-0.0.2/notebook/
--rw-rw-rw-   0 root         (0) root         (0)    96555 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/notebook/transform_GW.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-05 10:55:14.917170 wdm-wavelet-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:55:14.912170 wdm-wavelet-0.0.2/test/
--rw-rw-rw-   0 root         (0) root         (0)      301 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/test/test_wdm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:55:14.913170 wdm-wavelet-0.0.2/wdm_wavelet/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/wdm_wavelet/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-02-05 10:55:14.000000 wdm-wavelet-0.0.2/wdm_wavelet/_version.py
--rw-rw-rw-   0 root         (0) root         (0)   106583 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/wdm_wavelet/fourier_coeff.py
--rw-rw-rw-   0 root         (0) root         (0)     5840 2024-02-05 10:54:59.000000 wdm-wavelet-0.0.2/wdm_wavelet/wdm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-05 10:55:14.915170 wdm-wavelet-0.0.2/wdm_wavelet.egg-info/
--rw-r--r--   0 root         (0) root         (0)      642 2024-02-05 10:55:14.000000 wdm-wavelet-0.0.2/wdm_wavelet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2024-02-05 10:55:14.000000 wdm-wavelet-0.0.2/wdm_wavelet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-05 10:55:14.000000 wdm-wavelet-0.0.2/wdm_wavelet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-05 10:55:14.000000 wdm-wavelet-0.0.2/wdm_wavelet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-02-05 10:55:14.000000 wdm-wavelet-0.0.2/wdm_wavelet.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 08:06:23.883456 wdm_wavelet-0.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)      642 2024-05-09 08:06:23.882456 wdm_wavelet-0.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 08:06:23.879456 wdm_wavelet-0.1.1/notebook/
+-rw-rw-rw-   0 root         (0) root         (0)   164420 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/notebook/transform_GW.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 08:06:23.883456 wdm_wavelet-0.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 08:06:23.879456 wdm_wavelet-0.1.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/test/test_wdm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 08:06:23.880456 wdm_wavelet-0.1.1/wdm_wavelet/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/wdm_wavelet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-09 08:06:23.000000 wdm_wavelet-0.1.1/wdm_wavelet/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 08:06:23.881456 wdm_wavelet-0.1.1/wdm_wavelet/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/wdm_wavelet/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/wdm_wavelet/core/get_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2444 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/wdm_wavelet/core/t2w.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/wdm_wavelet/core/w2t.py
+-rw-rw-rw-   0 root         (0) root         (0)   106583 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/wdm_wavelet/fourier_coeff.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 08:06:23.881456 wdm_wavelet-0.1.1/wdm_wavelet/types/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/wdm_wavelet/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/wdm_wavelet/types/time_frequency_map.py
+-rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-09 08:06:17.000000 wdm_wavelet-0.1.1/wdm_wavelet/wdm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 08:06:23.882456 wdm_wavelet-0.1.1/wdm_wavelet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      642 2024-05-09 08:06:23.000000 wdm_wavelet-0.1.1/wdm_wavelet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      569 2024-05-09 08:06:23.000000 wdm_wavelet-0.1.1/wdm_wavelet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 08:06:23.000000 wdm_wavelet-0.1.1/wdm_wavelet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-09 08:06:23.000000 wdm_wavelet-0.1.1/wdm_wavelet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-09 08:06:23.000000 wdm_wavelet-0.1.1/wdm_wavelet.egg-info/top_level.txt
```

### Comparing `wdm-wavelet-0.0.2/.gitlab-ci.yml` & `wdm_wavelet-0.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `wdm-wavelet-0.0.2/LICENSE` & `wdm_wavelet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wdm-wavelet-0.0.2/PKG-INFO` & `wdm_wavelet-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdm-wavelet
-Version: 0.0.2
+Version: 0.1.1
 Summary: A Python package for Wilson-Daubechies-Meyer (WDM) wavelet from coherentWaveBurst
 Home-page: https://git.ligo.org/yumeng.xu/setup.py
 Author: Yumeng Xu
 Author-email: The PycWB team <yumeng.xu@ligo.org>
 Keywords: ligo,wavelet,gravitational waves,burst,DWT,WDM,Wilson-Daubechies-Meyer,cWB
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `wdm-wavelet-0.0.2/pyproject.toml` & `wdm_wavelet-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wdm-wavelet-0.0.2/setup.py` & `wdm_wavelet-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `wdm-wavelet-0.0.2/wdm_wavelet/fourier_coeff.py` & `wdm_wavelet-0.1.1/wdm_wavelet/fourier_coeff.py`

 * *Files identical despite different names*

### Comparing `wdm-wavelet-0.0.2/wdm_wavelet.egg-info/PKG-INFO` & `wdm_wavelet-0.1.1/wdm_wavelet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wdm-wavelet
-Version: 0.0.2
+Version: 0.1.1
 Summary: A Python package for Wilson-Daubechies-Meyer (WDM) wavelet from coherentWaveBurst
 Home-page: https://git.ligo.org/yumeng.xu/setup.py
 Author: Yumeng Xu
 Author-email: The PycWB team <yumeng.xu@ligo.org>
 Keywords: ligo,wavelet,gravitational waves,burst,DWT,WDM,Wilson-Daubechies-Meyer,cWB
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```


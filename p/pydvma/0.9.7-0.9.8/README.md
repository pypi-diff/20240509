# Comparing `tmp/pydvma-0.9.7.tar.gz` & `tmp/pydvma-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydvma-0.9.7.tar", last modified: Tue Mar 26 14:12:55 2024, max compression
+gzip compressed data, was "pydvma-0.9.8.tar", last modified: Thu May  9 09:40:22 2024, max compression
```

## Comparing `pydvma-0.9.7.tar` & `pydvma-0.9.8.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-03-26 14:12:55.670095 pydvma-0.9.7/
--rw-r--r--   0 tore       (501) staff       (20)     1603 2022-01-23 21:29:32.000000 pydvma-0.9.7/LICENSE
--rw-r--r--   0 tore       (501) staff       (20)     3179 2024-03-26 14:12:55.669865 pydvma-0.9.7/PKG-INFO
--rw-r--r--   0 tore       (501) staff       (20)     2977 2023-05-18 13:19:44.000000 pydvma-0.9.7/README.md
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-03-26 14:12:55.668441 pydvma-0.9.7/pydvma/
--rw-r--r--   0 tore       (501) staff       (20)     1151 2024-03-26 09:36:53.000000 pydvma-0.9.7/pydvma/__init__.py
--rw-r--r--   0 tore       (501) staff       (20)    10558 2024-03-01 15:32:42.000000 pydvma-0.9.7/pydvma/acquisition.py
--rw-r--r--   0 tore       (501) staff       (20)    15939 2023-04-19 17:23:29.000000 pydvma-0.9.7/pydvma/analysis.py
--rw-r--r--   0 tore       (501) staff       (20)    29939 2024-03-26 14:12:47.000000 pydvma-0.9.7/pydvma/datastructure.py
--rw-r--r--   0 tore       (501) staff       (20)    18282 2024-03-26 11:24:17.000000 pydvma-0.9.7/pydvma/file.py
--rw-r--r--   0 tore       (501) staff       (20)   125733 2024-03-26 14:12:31.000000 pydvma-0.9.7/pydvma/gui.py
--rw-r--r--   0 tore       (501) staff       (20)     2718 2023-04-13 15:37:51.000000 pydvma-0.9.7/pydvma/gui_tk.py
--rw-r--r--   0 tore       (501) staff       (20)     2718 2024-03-26 12:04:54.000000 pydvma-0.9.7/pydvma/gui_tk_old.py
--rw-r--r--   0 tore       (501) staff       (20)    10266 2023-04-19 17:23:39.000000 pydvma-0.9.7/pydvma/modal.py
--rw-r--r--   0 tore       (501) staff       (20)     8198 2024-03-26 13:51:59.000000 pydvma-0.9.7/pydvma/options.py
--rw-r--r--   0 tore       (501) staff       (20)    14580 2023-04-19 18:02:41.000000 pydvma-0.9.7/pydvma/oscilloscope.py
--rw-r--r--   0 tore       (501) staff       (20)    27099 2023-04-19 17:23:46.000000 pydvma-0.9.7/pydvma/plotting.py
--rw-r--r--   0 tore       (501) staff       (20)    25624 2023-05-01 16:06:38.000000 pydvma-0.9.7/pydvma/streams.py
--rw-r--r--   0 tore       (501) staff       (20)     2778 2023-04-19 17:56:13.000000 pydvma-0.9.7/pydvma/testdata.py
-drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-03-26 14:12:55.669622 pydvma-0.9.7/pydvma.egg-info/
--rw-r--r--   0 tore       (501) staff       (20)     3179 2024-03-26 14:12:55.000000 pydvma-0.9.7/pydvma.egg-info/PKG-INFO
--rw-r--r--   0 tore       (501) staff       (20)      439 2024-03-26 14:12:55.000000 pydvma-0.9.7/pydvma.egg-info/SOURCES.txt
--rw-r--r--   0 tore       (501) staff       (20)        1 2024-03-26 14:12:55.000000 pydvma-0.9.7/pydvma.egg-info/dependency_links.txt
--rw-r--r--   0 tore       (501) staff       (20)       63 2024-03-26 14:12:55.000000 pydvma-0.9.7/pydvma.egg-info/requires.txt
--rw-r--r--   0 tore       (501) staff       (20)        7 2024-03-26 14:12:55.000000 pydvma-0.9.7/pydvma.egg-info/top_level.txt
--rw-r--r--   0 tore       (501) staff       (20)       38 2024-03-26 14:12:55.670235 pydvma-0.9.7/setup.cfg
--rw-r--r--   0 tore       (501) staff       (20)      725 2024-03-26 14:12:40.000000 pydvma-0.9.7/setup.py
+drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-05-09 09:40:22.209403 pydvma-0.9.8/
+-rw-r--r--   0 tore       (501) staff       (20)     1603 2022-01-23 21:29:32.000000 pydvma-0.9.8/LICENSE
+-rw-r--r--   0 tore       (501) staff       (20)     3769 2024-05-09 09:40:22.209133 pydvma-0.9.8/PKG-INFO
+-rw-r--r--   0 tore       (501) staff       (20)     3359 2024-03-26 14:44:13.000000 pydvma-0.9.8/README.md
+drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-05-09 09:40:22.207790 pydvma-0.9.8/pydvma/
+-rw-r--r--   0 tore       (501) staff       (20)     1180 2024-04-09 17:50:25.000000 pydvma-0.9.8/pydvma/__init__.py
+-rw-r--r--   0 tore       (501) staff       (20)    10558 2024-03-01 15:32:42.000000 pydvma-0.9.8/pydvma/acquisition.py
+-rw-r--r--   0 tore       (501) staff       (20)    18901 2024-04-09 17:58:02.000000 pydvma-0.9.8/pydvma/analysis.py
+-rw-r--r--   0 tore       (501) staff       (20)    29939 2024-05-09 09:27:32.000000 pydvma-0.9.8/pydvma/datastructure.py
+-rw-r--r--   0 tore       (501) staff       (20)     3984 2024-04-09 17:50:04.000000 pydvma-0.9.8/pydvma/develop_sonogram_damping function.py
+-rw-r--r--   0 tore       (501) staff       (20)    18282 2024-03-26 11:24:17.000000 pydvma-0.9.8/pydvma/file.py
+-rw-r--r--   0 tore       (501) staff       (20)   127148 2024-05-09 09:26:38.000000 pydvma-0.9.8/pydvma/gui.py
+-rw-r--r--   0 tore       (501) staff       (20)     2718 2023-04-13 15:37:51.000000 pydvma-0.9.8/pydvma/gui_tk.py
+-rw-r--r--   0 tore       (501) staff       (20)     2718 2024-03-26 12:04:54.000000 pydvma-0.9.8/pydvma/gui_tk_old.py
+-rw-r--r--   0 tore       (501) staff       (20)       83 2024-05-09 09:17:32.000000 pydvma-0.9.8/pydvma/logger_tester.py
+-rw-r--r--   0 tore       (501) staff       (20)    10266 2023-04-19 17:23:39.000000 pydvma-0.9.8/pydvma/modal.py
+-rw-r--r--   0 tore       (501) staff       (20)     8198 2024-03-26 13:51:59.000000 pydvma-0.9.8/pydvma/options.py
+-rw-r--r--   0 tore       (501) staff       (20)    14580 2023-04-19 18:02:41.000000 pydvma-0.9.8/pydvma/oscilloscope.py
+-rw-r--r--   0 tore       (501) staff       (20)    27099 2023-04-19 17:23:46.000000 pydvma-0.9.8/pydvma/plotting.py
+-rw-r--r--   0 tore       (501) staff       (20)    25624 2023-05-01 16:06:38.000000 pydvma-0.9.8/pydvma/streams.py
+-rw-r--r--   0 tore       (501) staff       (20)     2778 2023-04-19 17:56:13.000000 pydvma-0.9.8/pydvma/testdata.py
+drwxr-xr-x   0 tore       (501) staff       (20)        0 2024-05-09 09:40:22.208717 pydvma-0.9.8/pydvma.egg-info/
+-rw-r--r--   0 tore       (501) staff       (20)     3769 2024-05-09 09:40:22.000000 pydvma-0.9.8/pydvma.egg-info/PKG-INFO
+-rw-r--r--   0 tore       (501) staff       (20)      507 2024-05-09 09:40:22.000000 pydvma-0.9.8/pydvma.egg-info/SOURCES.txt
+-rw-r--r--   0 tore       (501) staff       (20)        1 2024-05-09 09:40:22.000000 pydvma-0.9.8/pydvma.egg-info/dependency_links.txt
+-rw-r--r--   0 tore       (501) staff       (20)       63 2024-05-09 09:40:22.000000 pydvma-0.9.8/pydvma.egg-info/requires.txt
+-rw-r--r--   0 tore       (501) staff       (20)        7 2024-05-09 09:40:22.000000 pydvma-0.9.8/pydvma.egg-info/top_level.txt
+-rw-r--r--   0 tore       (501) staff       (20)       38 2024-05-09 09:40:22.209462 pydvma-0.9.8/setup.cfg
+-rw-r--r--   0 tore       (501) staff       (20)      776 2024-05-09 09:40:14.000000 pydvma-0.9.8/setup.py
```

### Comparing `pydvma-0.9.7/LICENSE` & `pydvma-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/PKG-INFO` & `pydvma-0.9.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: pydvma
-Version: 0.9.7
-Home-page: https://github.com/torebutlin/pydvma
-Author: Tore Butlin
-Author-email: tb267@cam.ac.uk
-License: BSD 3-Clause License
-License-File: LICENSE
-
 # pydvma
 
 A Python package for dynamics and vibration measurements and analysis.
 
 
 ## About pydvma
 
@@ -27,43 +18,53 @@
 
 The logger is recommended for use with Python 3.10.
 
 ```
 pip install pydvma
 ```
 
-If you would like soundcard acquisition then also install sounddevice:
+Or clone this repository and install using:
 ```
-pip install sounddevice
+python setup.py install
 ```
 
-Or clone this repository and install using:
+Alternatively if you use anaconda then the following creates a Python 3.10 environment with the required packages:
 ```
-python setup.py install
+conda create -n py310 python=3.10
+conda activate py310
+conda install numpy scipy jupyter matplotlib pyqtgraph
+pip install pydvma
 ```
 
-Alternatively you can use the environment yml file provided:
+If you would like soundcard acquisition then also install sounddevice:
+```
+pip install sounddevice
+```
+
+If you would like National Instruments acquisition then you need to install the NIDAQMX v17.6 driver from National Instruments ([here](https://www.ni.com/en/support/downloads/drivers/download.ni-daq-mx.html#288272)) and also install pydaqmx:
 ```
-conda env -name logger create -f logger.yml
-conda activate logger
+pip install pydaqmx
 ```
 
+
+
 ### Running the logger
 
 To get started, open the file:
 ```
 pydvma_template.ipynb
 ```
 
 or within a Jupyter Notebook or Python console:
 ```python
-%gui qt
 import pydvma as dvma
+import matplotlib
+
+%matplotlib qt
 settings = dvma.MySettings()
-osc = dvma.Oscilloscope(settings)
 logger = dvma.Logger(settings)
 ```
 
 ## Roadmap
 
 At present the library has basic functionality for:
 
@@ -94,8 +95,8 @@
 
 - For bug-fixes and refinements: please feel free to clone the repository, make edits and create a pull request with a clear description of changes made.
 
 - If you would like to make a more significant contribution or change, then please be in contact to outline your suggestion.
 
 Please see the documentation for details of the code structure and templates for anticipated applications.
 <!-- pip install git+https://github.com/torebutlin/pydvma.git -->
-<!-- pip install git+https://github.com/js2597/pydvma.git -->
+<!-- pip install git+https://github.com/js2597/pydvma.git -->
```

### Comparing `pydvma-0.9.7/README.md` & `pydvma-0.9.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: pydvma
+Version: 0.9.8
+Home-page: https://github.com/torebutlin/pydvma
+Author: Tore Butlin
+Author-email: tb267@cam.ac.uk
+License: BSD 3-Clause License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: peakutils
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pyqtgraph
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: sounddevice
+
 # pydvma
 
 A Python package for dynamics and vibration measurements and analysis.
 
 
 ## About pydvma
 
@@ -18,43 +35,53 @@
 
 The logger is recommended for use with Python 3.10.
 
 ```
 pip install pydvma
 ```
 
-If you would like soundcard acquisition then also install sounddevice:
+Or clone this repository and install using:
 ```
-pip install sounddevice
+python setup.py install
 ```
 
-Or clone this repository and install using:
+Alternatively if you use anaconda then the following creates a Python 3.10 environment with the required packages:
 ```
-python setup.py install
+conda create -n py310 python=3.10
+conda activate py310
+conda install numpy scipy jupyter matplotlib pyqtgraph
+pip install pydvma
 ```
 
-Alternatively you can use the environment yml file provided:
+If you would like soundcard acquisition then also install sounddevice:
+```
+pip install sounddevice
+```
+
+If you would like National Instruments acquisition then you need to install the NIDAQMX v17.6 driver from National Instruments ([here](https://www.ni.com/en/support/downloads/drivers/download.ni-daq-mx.html#288272)) and also install pydaqmx:
 ```
-conda env -name logger create -f logger.yml
-conda activate logger
+pip install pydaqmx
 ```
 
+
+
 ### Running the logger
 
 To get started, open the file:
 ```
 pydvma_template.ipynb
 ```
 
 or within a Jupyter Notebook or Python console:
 ```python
-%gui qt
 import pydvma as dvma
+import matplotlib
+
+%matplotlib qt
 settings = dvma.MySettings()
-osc = dvma.Oscilloscope(settings)
 logger = dvma.Logger(settings)
 ```
 
 ## Roadmap
 
 At present the library has basic functionality for:
 
@@ -85,8 +112,8 @@
 
 - For bug-fixes and refinements: please feel free to clone the repository, make edits and create a pull request with a clear description of changes made.
 
 - If you would like to make a more significant contribution or change, then please be in contact to outline your suggestion.
 
 Please see the documentation for details of the code structure and templates for anticipated applications.
 <!-- pip install git+https://github.com/torebutlin/pydvma.git -->
-<!-- pip install git+https://github.com/js2597/pydvma.git -->
+<!-- pip install git+https://github.com/js2597/pydvma.git -->
```

### Comparing `pydvma-0.9.7/pydvma/__init__.py` & `pydvma-0.9.8/pydvma/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 from .file import load_data, save_data, save_fig, export_to_matlab_jwlogger, export_to_matlab, export_to_csv
 # from .oscilloscope import Oscilloscope
 from .acquisition import log_data, output_signal, signal_generator, stream_snapshot
 from .datastructure import DataSet, TimeData, FreqData, CrossSpecData, TfData, SonoData, MetaData, ModalData, update_dataset
 from .testdata import create_test_impulse_data, create_test_impulse_ensemble, create_test_noise_data
 from .plotting import PlotData
 from .analysis import calculate_fft, calculate_cross_spectrum_matrix, calculate_cross_spectra_averaged, clean_impulse
-from .analysis import calculate_tf, calculate_tf_averaged, multiply_by_power_of_iw, best_match, calculate_sonogram
+from .analysis import calculate_tf, calculate_tf_averaged, multiply_by_power_of_iw, best_match, calculate_sonogram, calculate_damping_from_sono
 from .streams import Recorder, Recorder_NI, start_stream, REC, setup_output_NI, setup_output_soundcard, list_available_devices, get_devices_NI, get_devices_soundcard
 from .modal import modal_fit_single_channel, modal_fit_all_channels
 # import faulthandler
 # faulthandler.enable()
 # from .gui_tk_test import Logger
```

### Comparing `pydvma-0.9.7/pydvma/acquisition.py` & `pydvma-0.9.8/pydvma/acquisition.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma/analysis.py` & `pydvma-0.9.8/pydvma/analysis.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 """
 
 from . import datastructure
 
 import numpy as np
 from scipy import signal
 import copy
+import peakutils as pu
+from scipy.optimize import curve_fit
+import matplotlib.pyplot as plt
 
 MESSAGE = ''
 
 
 def calculate_fft(time_data,time_range=None,window=None):
     '''
     Args:
@@ -432,24 +435,116 @@
         MESSAGE ='Impulse data already cleaned. No change made.'
         print(MESSAGE)
         return time_data
 
     
     
 #%% SONOGRAM    
-def calculate_sonogram(time_data, nperseg=None):
+def calculate_sonogram(time_data, nperseg=None, noverlap=None):
     
     y = np.copy(time_data.time_data) # handles all channels simultaneously
     if nperseg == None:
         nperseg = int(len(time_data.time_axis)/50) #roughly 50 fft's per time-series not counting overlap
-    f,t,S = signal.spectrogram(y,fs=time_data.settings.fs,window='hann',nperseg=nperseg,noverlap=nperseg//4,axis=0,mode='complex')
+    if noverlap == None:
+        noverlap = nperseg//2
+
+    f,t,S = signal.spectrogram(y,fs=time_data.settings.fs,window='hann',nperseg=nperseg,noverlap=noverlap,axis=0,mode='complex')
     
     # put channel axis at end
     S_all_chans = np.swapaxes(S,1,2)
     
     sono_data = datastructure.SonoData(t,f,S_all_chans,time_data.settings,id_link=time_data.id_link,test_name=time_data.test_name)
     
     return sono_data
 
 #%% CWT
 #def calculate_cwt(time_data):
-#    return None
+#    return None
+
+#%% Damping from sonogram
+
+# define a custom functions for fitting
+def func_real(t, A,B,N):
+    #ensure exp(A) and exp(N) are positive
+    f = np.log(np.exp(A)*np.exp(-B*t) + 1j*np.exp(N))
+    f = np.real(f)
+    return f
+
+def func_imag(t, W, C):
+    f = W*t + C
+    return f
+
+zeta_n = []
+wn_n = []
+def calculate_damping_from_sono(time_data,n_chan=1,nperseg=None,start_time=None):
+
+    sono_data = calculate_sonogram(time_data, nperseg=nperseg,noverlap=0)
+
+    t = sono_data.time_axis
+    f = sono_data.freq_axis
+    S = sono_data.sono_data
+    settings = sono_data.settings
+
+    # find t index closest to t0
+    if start_time == None:
+        try:
+            t0 = 2*sono_data.settings.pretrig_samples/sono_data.settings.fs
+            time_slice = np.argmin(np.abs(t - t0))
+        except:
+            t0 = t[-1]//20
+            time_slice = np.argmin(np.abs(t - t0))
+
+    time_slice_data = np.abs(S[:, time_slice, n_chan])
+    threshold = 10 * np.median(time_slice_data)/np.max(time_slice_data)
+    peaks = pu.indexes(time_slice_data, thres=threshold, min_dist=1)
+
+    print(peaks)
+    plt.plot(time_slice_data)
+    # horizontal line at threshold
+    plt.axhline(threshold * np.max(time_slice_data), color='r')
+
+    for peak in peaks:
+
+        # Extract the real and imaginary parts of S at the peak frequency
+        real_part = np.real(np.log(S[peak, :, n_chan]))
+        imag_part = np.unwrap(np.imag(np.log(S[peak, :, n_chan])))
+
+        # Fit the real part to a custom function
+        popt_real, _ = curve_fit(func_real, t[time_slice:], real_part[time_slice:])
+        real_fit = func_real(t, *popt_real)
+        A = popt_real[0]
+        B = popt_real[1]
+        N = popt_real[2]
+
+        # Identify crossover time when noise starts to dominate
+        t_cross = (A - N)/B
+        # nearest time index
+        time_cross = np.argmin(np.abs(t - t_cross))
+
+        # Fit the imaginary part to a linear function for clean part of the signal
+        t0 = time_slice
+        dt = int(np.ceil(0.9*(time_cross - time_slice)))
+        dt = np.max([2,dt])
+        t1 = t0 + dt
+
+        # Fit the imaginary part to a linear function for clean part of the signal
+        popt_imag,_ = curve_fit(func_imag, t[t0:t1], imag_part[t0:t1])
+        imag_fit = func_imag(t, *popt_imag)
+        W = popt_imag[0]
+        print(W/2/np.pi)
+        W0 = 2*np.pi*f[peak] + W # corrected for the bin frequency
+        C = popt_imag[1]
+        
+        # Calculate the damping factor and frequency from the fit coefficients
+        zeta = B / np.sqrt(W0**2 + B**2)
+        w = W0 / np.sqrt(1 - zeta**2)
+        
+        # Store the results in numpy arrays
+        zeta_n.append(zeta)
+        wn_n.append(w)
+
+    zn = np.array(zeta_n)
+    Qn = 1/(2*zn)
+    wn = np.array(wn_n)
+    fn = wn / (2*np.pi)
+
+    return fn, Qn
```

### Comparing `pydvma-0.9.7/pydvma/datastructure.py` & `pydvma-0.9.8/pydvma/datastructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import numpy as np
 import datetime
 import uuid
 import copy
 
 #%% version
-VERSION = '0.9.7' # keep in sync with setup.py
+VERSION = '0.9.8' # keep in sync with setup.py
 
 def update_dataset(dataset):
     dataset_new = DataSet()
     dataset_new.add_to_dataset(dataset.time_data_list)
     dataset_new.add_to_dataset(dataset.freq_data_list)
     dataset_new.add_to_dataset(dataset.tf_data_list)
     dataset_new.add_to_dataset(dataset.cross_spec_data_list)
```

### Comparing `pydvma-0.9.7/pydvma/file.py` & `pydvma-0.9.8/pydvma/file.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma/gui.py` & `pydvma-0.9.8/pydvma/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,57 +54,61 @@
 #%%
 class BlueButton(QPushButton):
     def __init__(self,text):
         super().__init__(text)
         if flag_darktheme:
             self.setStyleSheet("background-color: hsv(240, 120, 180)")
         else:
-            self.setStyleSheet("background-color: hsv(240, 170, 255)")
+            # set font colour to black
+            self.setStyleSheet("background-color: hsv(240, 170, 255); color: black")
+            
+
+            
         self.setText(text) 
 
 class GreenButton(QPushButton):
     def __init__(self,text):
         super().__init__(text)
         if flag_darktheme:
             self.setStyleSheet("background-color: hsv(120, 120, 180);")
         else:
-            self.setStyleSheet("background-color: hsv(120, 170, 255);")
+            self.setStyleSheet("background-color: hsv(120, 170, 255); color: black")
         self.setText(text)
 
 class RedButton(QPushButton):
     def __init__(self,text):
         super().__init__(text)
         if flag_darktheme:
             self.setStyleSheet("background-color: hsv(0, 120, 180)")
         else:
-            self.setStyleSheet("background-color: hsv(0, 170, 255)")
+            self.setStyleSheet("background-color: hsv(0, 170, 255); color: black")
         self.setText(text)
         
 class OrangeButton(QPushButton):
     def __init__(self,text):
         super().__init__(text)
         if flag_darktheme:
             self.setStyleSheet("background-color: hsv(30, 120, 180)")
         else:
-            self.setStyleSheet("background-color: hsv(30, 170, 255)")
+            self.setStyleSheet("background-color: hsv(30, 170, 255); color: black")
         self.setText(text)
 
 class QHLine(QFrame):
     def __init__(self):
         super(QHLine, self).__init__()
         self.setFrameShape(QFrame.HLine)
         self.setFrameShadow(QFrame.Sunken)
         
 class newComboBox(QComboBox):
     def __init__(self,items_list):
         super().__init__()
         if flag_darktheme:
             self.setStyleSheet('selection-background-color: hsv(240, 120, 180)')
         else:
-            self.setStyleSheet('selection-background-color: hsv(240, 170, 255)')
+            self.setStyleSheet('selection-background-color: hsv(240, 170, 255); color: black')
         self.addItems(items_list)
         
 class boldLabel(QLabel):
     def __init__(self,text):
         super().__init__(text)
         self.setStyleSheet('font: bold')
         
@@ -129,15 +133,15 @@
         self.s.emit(self.d)
         
         
         
 class PreviewWindow():
     def __init__(self,title='Time Data'):
         self.preview_window = QWidget()
-        self.preview_window.setStyleSheet("background-color: white")
+        self.preview_window.setStyleSheet("background-color: white; color: black")
         self.preview_window.setWindowTitle('Output Signal Preview')
         self.preview_window.setWindowIcon(QtGui.QIcon(icon_path))
 
         self.fig = Figure(figsize=(9, 5),dpi=100)
         self.canvas = FigureCanvas(self.fig)
         self.toolbar = NavigationToolbar(self.canvas,None)
         self.toolbar.setOrientation(Qt.Orientation.Horizontal)
@@ -216,15 +220,15 @@
         # else:
         #     self.output_signal = output_signal
         
         # SETUP GUI
         # self.app = app
         # self.app.setStyle(QStyleFactory.create('Fusion'))
         self.window = QWidget()
-        self.window.setStyleSheet("background-color: white")
+        self.window.setStyleSheet("background-color: white; color: black")
         self.window.setWindowTitle('Logger')
         self.window.setWindowIcon(QtGui.QIcon(icon_path))
         # self.window.setAttribute(Qt.WidgetAttribute.WA_DeleteOnClose)
         
         # initiate all interface tool frames
         self.setup_frame_tools()
         self.setup_frame_input()
@@ -944,27 +948,32 @@
         self.input_db_range.editingFinished.connect(self.calc_sono)
         
         self.sono_info = QLabel('')
         
         
         self.button_calc_sono = BlueButton('Calc Sonogram')
         self.button_calc_sono.clicked.connect(self.calc_sono)
+
+        self.button_calc_damping = BlueButton('Calc Damping')
+        self.button_calc_damping.clicked.connect(self.calc_damping)
+
         
         self.layout_tools_sonogram = QGridLayout()
         self.layout_tools_sonogram.addWidget(boldLabel('Calculate Sonogram:'),0,0,1,4)
         self.layout_tools_sonogram.addWidget(QLabel('N frames:'),1,0,1,2)
         self.layout_tools_sonogram.addWidget(self.input_sono_N_frames,1,2,1,2)
         self.layout_tools_sonogram.addWidget(self.slider_sono_N_frames,2,0,1,4)
         self.layout_tools_sonogram.addWidget(self.sono_info,3,0,1,4)
         self.layout_tools_sonogram.addWidget(QLabel('Dynamic Range (dB):'),4,0,1,2)
         self.layout_tools_sonogram.addWidget(self.input_db_range,4,2,1,2)
         self.layout_tools_sonogram.addWidget(QLabel('Set / Chan:'),5,0,1,2)
         self.layout_tools_sonogram.addWidget(self.input_sono_n_set,5,2,1,1)
         self.layout_tools_sonogram.addWidget(self.input_sono_n_chan,5,3,1,1)
         self.layout_tools_sonogram.addWidget(self.button_calc_sono,6,0,1,4)
+        self.layout_tools_sonogram.addWidget(self.button_calc_damping,7,0,1,4)
         
         self.frame_tools_sonogram = QFrame()
         self.frame_tools_sonogram.setLayout(self.layout_tools_sonogram)
         
     def setup_frame_tools_save_export(self):
         #self.button_import_matlab_jwlogger = BlueButton('Import from JW Logger')
         #self.button_import_matlab_jwlogger.clicked.connect(self.import_jwlogger)
@@ -1120,15 +1129,15 @@
         else:
             y = None
 
         
         
         # reset trigger
         self.rec.trigger_detected = False # but need to do this again inside acquisition
-        self.button_log_data.setStyleSheet("background-color: white")
+        self.button_log_data.setStyleSheet("background-color: white; color: black")
         
 #        # show message re trigger
 #        if self.settings.pretrig_samples is None:
 #            message = 'Logging data for {} seconds'.format(self.settings.stored_time)
 #        else:
             #message = 'Logging data for {} seconds, with trigger.\n'.format(self.settings.stored_time)
             
@@ -1188,24 +1197,24 @@
                     selection[ns][nc] = False
         self.selected_channels = selection
         
         # update with final selection and make -1 to 1, change button back to green
         self.auto_xy = 'x'
         self.update_figure()
         self.p.ax.set_ylim([-1,1])
-        self.button_log_data.setStyleSheet('background-color: hsv(120, 170, 255)')
+        self.button_log_data.setStyleSheet('background-color: hsv(120, 170, 255); color: black')
         self.message_timer.stop()
         
         
     def cancel_logging(self):
         self.thread.terminate() # stop thread
         streams.start_stream(self.settings) # reset stream
         self.rec = streams.REC # reset stream
         self.show_message('Logging cancelled')
-        self.button_log_data.setStyleSheet('background-color: hsv(120, 170, 255)')
+        self.button_log_data.setStyleSheet('background-color: hsv(120, 170, 255); color: black')
         self.message_timer.stop() # stop acquisition messages
         self.selected_channels = self.p.get_selected_channels()
 
     def delete_last_data(self):
         self.dataset_backup = copy.deepcopy(self.dataset)
         self.dataset.remove_last_data_item('TimeData')
         self.dataset.freq_data_list = datastructure.FreqDataList()
@@ -2529,14 +2538,31 @@
             text = 'FFT length: {}\n'.format(self.nperseg)
             text += 'Freq resolution: {:5g} (Hz)\n'.format(np.diff(self.dataset.sono_data_list[n_set].freq_axis[[0,1]])[0])
             
             self.sono_info.setText(text)
             if self.current_view != 'Sono Data':
                 self.switch_view('Sono Data')
             self.update_figure()
+
+    def calc_damping(self):
+        if len(self.dataset.time_data_list) == 0:
+            message = 'No time data to calculate damping.'
+            self.show_message(message)
+        else:
+            self.N_frames_sono = int(self.input_sono_N_frames.text())
+            n_set = int(self.input_sono_n_set.text())
+            n_chan = int(self.input_sono_n_chan.text())
+            NT = len(self.dataset.time_data_list[n_set].time_data[:,n_chan])
+            f = 0 # match overlap in sonogram
+            self.nperseg = int(NT // (self.N_frames_sono * (1-f) + f)) # 1/8 is default overlap for spectrogram
+            fn,Qn = analysis.calculate_damping_from_sono(self.dataset.time_data_list[n_set],n_chan=n_chan,nperseg=self.nperseg,start_time=None)
+            message = 'Modes fitted:\n\n'
+            message += 'fn = {} (Hz)\n\n'.format(np.array2string(fn,precision=2))
+            message += 'Qn = 1/(2 zn) = {}\n'.format(np.array2string(Qn,precision=1))
+            self.show_message(message)
             
     def import_jwlogger(self):
         # import data from JW Logger
         self.dataset = file.import_from_matlab_jwlogger()
     
     def export_jwlogger(self):
         # export data to data structure compatible with JW Logger
```

### Comparing `pydvma-0.9.7/pydvma/gui_tk.py` & `pydvma-0.9.8/pydvma/gui_tk.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma/gui_tk_old.py` & `pydvma-0.9.8/pydvma/gui_tk_old.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma/modal.py` & `pydvma-0.9.8/pydvma/modal.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma/options.py` & `pydvma-0.9.8/pydvma/options.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma/oscilloscope.py` & `pydvma-0.9.8/pydvma/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma/plotting.py` & `pydvma-0.9.8/pydvma/plotting.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma/streams.py` & `pydvma-0.9.8/pydvma/streams.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma/testdata.py` & `pydvma-0.9.8/pydvma/testdata.py`

 * *Files identical despite different names*

### Comparing `pydvma-0.9.7/pydvma.egg-info/PKG-INFO` & `pydvma-0.9.8/pydvma.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 Metadata-Version: 2.1
 Name: pydvma
-Version: 0.9.7
+Version: 0.9.8
 Home-page: https://github.com/torebutlin/pydvma
 Author: Tore Butlin
 Author-email: tb267@cam.ac.uk
 License: BSD 3-Clause License
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: peakutils
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pyqtgraph
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: sounddevice
 
 # pydvma
 
 A Python package for dynamics and vibration measurements and analysis.
 
 
 ## About pydvma
@@ -27,43 +35,53 @@
 
 The logger is recommended for use with Python 3.10.
 
 ```
 pip install pydvma
 ```
 
-If you would like soundcard acquisition then also install sounddevice:
+Or clone this repository and install using:
 ```
-pip install sounddevice
+python setup.py install
 ```
 
-Or clone this repository and install using:
+Alternatively if you use anaconda then the following creates a Python 3.10 environment with the required packages:
 ```
-python setup.py install
+conda create -n py310 python=3.10
+conda activate py310
+conda install numpy scipy jupyter matplotlib pyqtgraph
+pip install pydvma
 ```
 
-Alternatively you can use the environment yml file provided:
+If you would like soundcard acquisition then also install sounddevice:
 ```
-conda env -name logger create -f logger.yml
-conda activate logger
+pip install sounddevice
+```
+
+If you would like National Instruments acquisition then you need to install the NIDAQMX v17.6 driver from National Instruments ([here](https://www.ni.com/en/support/downloads/drivers/download.ni-daq-mx.html#288272)) and also install pydaqmx:
+```
+pip install pydaqmx
 ```
 
+
+
 ### Running the logger
 
 To get started, open the file:
 ```
 pydvma_template.ipynb
 ```
 
 or within a Jupyter Notebook or Python console:
 ```python
-%gui qt
 import pydvma as dvma
+import matplotlib
+
+%matplotlib qt
 settings = dvma.MySettings()
-osc = dvma.Oscilloscope(settings)
 logger = dvma.Logger(settings)
 ```
 
 ## Roadmap
 
 At present the library has basic functionality for:
```

### Comparing `pydvma-0.9.7/setup.py` & `pydvma-0.9.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 from setuptools import setup, find_packages
 
 requires = ['peakutils', 'numpy', 'scipy', 'pyqtgraph', 'matplotlib', 'seaborn', 'sounddevice']
 #requires = ['peakutils', 'numpy', 'scipy', 'pyqtgraph', 'matplotlib', 'seaborn', 'sounddevicem', 'qtpy', 'pyqt5', 'qdarktheme']
 
 setup(
     name='pydvma',
-    version='0.9.7', # keep in sync with datastructure.py
+    version='0.9.8', # keep in sync with datastructure.py
     install_requires=requires,
     packages=['pydvma'],
     package_data={'': ['icon.png']},
     license='BSD 3-Clause License',
     long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author='Tore Butlin',
     author_email='tb267@cam.ac.uk',
     url='https://github.com/torebutlin/pydvma'
 )
```


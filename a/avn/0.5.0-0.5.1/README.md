# Comparing `tmp/avn-0.5.0.tar.gz` & `tmp/avn-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avn-0.5.0.tar", max compression
+gzip compressed data, was "avn-0.5.1.tar", max compression
```

## Comparing `avn-0.5.0.tar` & `avn-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0       23 2024-05-05 18:50:43.847140 avn-0.5.0/avn/__init__.py
--rw-r--r--   0        0        0    54839 2024-05-03 17:23:44.188360 avn-0.5.0/avn/acoustics.py
--rw-r--r--   0        0        0        0 2021-05-05 18:05:55.900000 avn-0.5.0/avn/avn.py
--rw-r--r--   0        0        0     7864 2024-05-03 19:22:15.718186 avn-0.5.0/avn/dataloading.py
--rw-r--r--   0        0        0    14928 2021-11-04 18:21:52.806620 avn-0.5.0/avn/plotting.py
--rw-r--r--   0        0        0    83983 2023-03-02 15:05:22.932147 avn-0.5.0/avn/segmentation.py
--rw-r--r--   0        0        0    16984 2024-05-04 22:06:46.883614 avn-0.5.0/avn/similarity.py
--rw-r--r--   0        0        0    90270 2023-03-10 20:40:35.473692 avn-0.5.0/avn/syntax.py
--rw-r--r--   0        0        0    34081 2024-05-03 19:22:15.719186 avn-0.5.0/avn/timing.py
--rw-r--r--   0        0        0        2 2021-04-28 15:46:50.000000 avn-0.5.0/LICENSE
--rw-r--r--   0        0        0      871 2024-05-05 18:50:23.387488 avn-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1373 2024-05-03 19:22:15.717198 avn-0.5.0/README.md
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 avn-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0  3137433 2024-05-05 20:18:01.836340 avn-0.5.1/avn/8D_trained_embedding_model.pth
+-rw-r--r--   0        0        0       25 2024-05-09 01:59:50.821757 avn-0.5.1/avn/__init__.py
+-rw-r--r--   0        0        0    54839 2024-05-03 17:23:44.188360 avn-0.5.1/avn/acoustics.py
+-rw-r--r--   0        0        0        0 2021-05-05 18:05:55.900000 avn-0.5.1/avn/avn.py
+-rw-r--r--   0        0        0     7886 2024-05-06 17:12:00.145273 avn-0.5.1/avn/dataloading.py
+-rw-r--r--   0        0        0    15007 2024-05-08 22:39:48.663123 avn-0.5.1/avn/plotting.py
+-rw-r--r--   0        0        0    83974 2024-05-06 17:48:21.156209 avn-0.5.1/avn/segmentation.py
+-rw-r--r--   0        0        0    17139 2024-05-06 21:18:38.265709 avn-0.5.1/avn/similarity.py
+-rw-r--r--   0        0        0    90291 2024-05-09 01:56:50.996417 avn-0.5.1/avn/syntax.py
+-rw-r--r--   0        0        0    34081 2024-05-05 20:18:01.842390 avn-0.5.1/avn/timing.py
+-rw-r--r--   0        0        0        2 2021-04-28 15:46:50.000000 avn-0.5.1/LICENSE
+-rw-r--r--   0        0        0      871 2024-05-09 01:59:23.227191 avn-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1373 2024-05-05 20:18:01.842049 avn-0.5.1/README.md
+-rw-r--r--   0        0        0     2258 1970-01-01 00:00:00.000000 avn-0.5.1/PKG-INFO
```

### Comparing `avn-0.5.0/avn/acoustics.py` & `avn-0.5.1/avn/acoustics.py`

 * *Files identical despite different names*

### Comparing `avn-0.5.0/avn/dataloading.py` & `avn-0.5.1/avn/dataloading.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         """
 
         #convert timestamps from miliseconds to seconds
         syll_table['onsets'] = syll_table['onsets'] / 1000
         syll_table['offsets'] = syll_table['offsets'] / 1000
         
         #remove .not.mat file extension from file names in files column
-        syll_table['files'] = syll_table['files'].str.split('.not', 1).str[0]
+        syll_table['files'] = syll_table['files'].str.split(pat = '.not', n = 1).str[0]
         
         return syll_table
       
     def add_ev_song_truth_table(seg_data, file_path):
         """
         Loads a 'ground truth' segmentation file generated in evsonganaly, and 
         adds it as a `.true_seg_table` attribute to the provided `seg_data` object. 
@@ -144,15 +144,15 @@
         true_seg_table = pd.read_csv(file_path)
         
         #conver timestamps from miliseconds to seconds
         true_seg_table['onsets'] = true_seg_table['onsets'] / 1000
         true_seg_table['offsets'] = true_seg_table['offsets'] / 1000
         
         #remove .not.mat file extension from file names in file column
-        true_seg_table['files'] = true_seg_table['files'].str.split('.not', 1).str[0]
+        true_seg_table['files'] = true_seg_table['files'].str.split(pat = '.not', n = 1).str[0]
         
         #add reformated ground truth segmentation table as an attribute of seg_data
         seg_data.true_seg_table = true_seg_table
         
         return seg_data
 
     def select_syll(song, onset, offset, padding = 0):
@@ -208,8 +208,8 @@
         #convert onset and offset times to indices
         on_index = int(padded_onset * song.sample_rate)
         off_index = int(padded_offset * song.sample_rate)
 
         #select portion of song data corresponding to indices
         syll_data = song.data[on_index : off_index]
 
-        return syll_data, onset_correction_diff, offset_correction_diff
+        return syll_data, onset_correction_diff, offset_correction_diff
```

### Comparing `avn-0.5.0/avn/plotting.py` & `avn-0.5.1/avn/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     #plot spectrogram
     img = librosa.display.specshow(spectrogram, sr = sample_rate, 
                              hop_length = 512 / 4, 
                              x_axis = 'time', 
                              y_axis = 'hz', 
                              cmap = 'viridis', 
                              ax = ax)
+    return fig
 
 def plot_syntax_raster(syntax_data, syntax_raster_df, figsize = (10, 10), title = None, 
                            palette = 'husl'):
     """
     Plots a syntax_raster_df dataframe. 
 
     Parameters
@@ -131,15 +132,16 @@
     #hide x and y axis lines and ticks
     ax.axes.xaxis.set_visible(False)
     ax.axes.yaxis.set_visible(False)
 
     #add title
     plt.title(title)
 
-    plt.show()
+    #plt.show()
+    return fig
 
 def plot_spectrogram_with_labels(syll_df, song_folder_path, Bird_ID, song_file = None, song_file_index = None, figsize = (80, 10), 
                                  cmap = 'tab20',  add_legend = True, fontsize = 24):
     """
     Plots the sectrogram of a specified file with syllable labels indicated through colored bars overlaid on spectrogram. 
 
     Parameters
@@ -243,14 +245,16 @@
                                          color = color))
     
     #if add_legend == True, add legend
     if add_legend == True: 
         markers  = [plt.Line2D([0, 0], [0, 0],  color = color, marker = 'o', linestyle = '') for color in color_dict.values()]
         ax.legend(markers, color_dict.keys(), numpoints = 1, facecolor = 'black', 
                   labelcolor = 'white', markerscale = 3, fontsize = fontsize, loc = 'upper right')
+        
+    return fig, ax, song_file_name
     
 def plot_syll(song, onset, offset, padding = 0, figsize = (5,5), title = None):
     """
     Plots the spectrogram of a portion of a song spectrogram (generally a single syllable).
 
     Parameters
     ----------
```

### Comparing `avn-0.5.0/avn/segmentation.py` & `avn-0.5.1/avn/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 
 @author: Therese
 """
 
 import glob
 import avn.dataloading as dataloading
 import avn.plotting as plotting
-#import dataloading
-#import plotting
 import numpy as np
 import pandas as pd
 import librosa
 import librosa.display
 import sklearn
+import sklearn.preprocessing
 import os
 import matplotlib.pyplot as plt
 import random
 
 class SegData:
     """
     Syllable segmentation data for many files from a single bird.
```

### Comparing `avn-0.5.0/avn/similarity.py` & `avn-0.5.1/avn/similarity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+# -*- coding: utf-8 -*-
 """
-Created on Fri May 3 2024
+Created on Fri May 3 10:30:22 2024
 
 @author: Therese
 """
 
 import numpy as np
 import pandas as pd
 import librosa
@@ -13,14 +14,15 @@
 import os
 import pandas as pd
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from typing import Any, Callable, cast, Dict, List, Optional, Tuple
 from emd import emd
+import importlib.resources as pkg_resources
 
 
 def _make_embedding_spect(syll_wav, sr, hop_length, win_length, n_fft, amin, ref_db, min_level_db, 
                           low_bandpass = None, high_bandpass = None):
     #make spectrogram of file
     spectrogram = librosa.stft(syll_wav, hop_length = hop_length, win_length = win_length, n_fft = n_fft)
     #convert to db scale
@@ -51,17 +53,15 @@
 
     :param Bird_ID: ID of the current bird to be processed. Will be used to name spectrogram files. 
     :type Bird_ID: str
     :param segmentations: pandas dataframe of syllable segmentations, with one row per syllable, and columns called :
     - 'files' : the name of the .wav file in which a syllable is found, 
     - 'onsets' : the onset of the syllable within the .wav file in seconds, and 
     - 'offsets': the offset of the syllable within the .wav file in seconds. 
-    
     We recommend using [WhisperSeg](https://github.com/nianlonggu/WhisperSeg) to automatically segment song syllables and generate this type of table.
-
     :type segmentations: pd.DataFrame
     :param song_folder_path: path to the folder containing all wav files from `segmentations`.
     :type song_folder_path: str
     :param out_dir: path to the folder where you want to save all the spectrograms. Each bird's spectrograms must be saved to a unique directory 
         for use with embedding model. 
     :type out_dir: str
     :param n_files: maximum number of files from which to make spectrograms. By default, spectrograms of all syllables will be made. 
@@ -86,14 +86,15 @@
     :param min_level_db: minimum decibel value for normalization of db spectrogram, defaults to -28
     :type min_level_db: int, optional
     :param pad_length: dimension of output spectrogram in frames, defaults to 70. spectrograms longer than 70 frames will 
         be clipped to 70 frames, and spectrograms shorter than 70 frames will be padded to 70 frames.
     :type pad_length: int>0, optional
     :return: None
     :rtype: None
+
     """
     #initialize df for audio
     syllable_dfs = pd.DataFrame()
 
     #if n_files is specified, sample n_files. Otherwise use all files
     if n_files is not None: 
         if len(segmentations.files.unique()) > n_files:
@@ -272,20 +273,21 @@
         else: 
             device = 'cpu'
         print('Device set to: ' + device)
 
     #specify model architecture 
     model = EmbeddingNet()
     #load model weights
-    model.load_state_dict(torch.load('..\\8D_trained_embedding_model.pth', map_location = torch.device(device)))
-    model.to(device)
-    model.device = device
-    model.eval()
+    with pkg_resources.path('avn', '8D_trained_embedding_model.pth') as model_path: 
+        model.load_state_dict(torch.load(model_path, map_location = torch.device(device)))
+        model.to(device)
+        model.device = device
+        model.eval()
 
-    return model
+        return model
 
 
 
 class CustomDatasetFolderNoClass(datasets.DatasetFolder):
     """creates dataset compatible with embedding net evaluation functions for unlabeled syllable spectrograms. 
     
     """
@@ -387,8 +389,8 @@
     :param bird_1_embedding: array of shape (n_syllables, 8) with syllable embeddings from one bird to be compared
     :type bird_1_embedding: np.array
     :param bird_2_embedding: array of shape (n_syllables, 8) with syllable embeddings from the other bird to be compared
     :type bird_2_embedding: np.array
     :return: emd score
     :rtype: float
     """
-    return emd(bird_1_embedding, bird_2_embedding)
+    return emd(bird_1_embedding, bird_2_embedding)
```

### Comparing `avn-0.5.0/avn/syntax.py` & `avn-0.5.1/avn/syntax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1075,15 +1075,16 @@
         #hide x and y axis lines and ticks
         ax.axes.xaxis.set_visible(False)
         ax.axes.yaxis.set_visible(False)
 
         #add title
         plt.title(title)
 
-        plt.show()
+        #plt.show()
+        return fig
 
     def _get_sylls_in_short_bouts(self, syll_df, max_short_bout_len = 2):
         """
         Creates a list of all syllable labels as they occur in bouts of duration 
         `max_short_bout_len` or shorter. This list can then be used to count the 
         total number of times a syllable type is produced in a short bout, which 
         can be useful for identifying calls.
```

### Comparing `avn-0.5.0/avn/timing.py` & `avn-0.5.1/avn/timing.py`

 * *Files identical despite different names*

### Comparing `avn-0.5.0/pyproject.toml` & `avn-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "avn"
-version = "0.5.0"
+version = "0.5.1"
+
 description = "Package for zebra finch song analysis."
 authors = ["Therese Koch"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 documentation = "https://avn.readthedocs.io/en/latest/"
 homepage = "https://github.com/theresekoch/avn"
 repository = "https://github.com/theresekoch/avn"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.10"
+python = ">=3.8,<3.10"
 pandas = ">=1.3.3"
 numpy = ">=1.20.2"
 scikit-learn = "^0.24.2"
 matplotlib = "^3.4.1"
 scipy = "^1.6.3"
 librosa = "0.10.2"
-seaborn = "^0.11.2"
+seaborn = "^0.13.1"
 more_itertools = "^8.5.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.0.1"
 nbsphinx = "^0.8.4"
 ipykernel = "^5.5.4"
 sphinxcontrib-napoleon = "^0.7"
```

### Comparing `avn-0.5.0/README.md` & `avn-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `avn-0.5.0/PKG-INFO` & `avn-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: avn
-Version: 0.5.0
+Version: 0.5.1
 Summary: Package for zebra finch song analysis.
 Home-page: https://github.com/theresekoch/avn
 License: GNU General Public License v3.0
 Author: Therese Koch
-Requires-Python: >=3.7.1,<3.10
+Requires-Python: >=3.8,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: librosa (==0.10.2)
 Requires-Dist: matplotlib (>=3.4.1,<4.0.0)
 Requires-Dist: more_itertools (>=8.5.0,<9.0.0)
 Requires-Dist: numpy (>=1.20.2)
 Requires-Dist: pandas (>=1.3.3)
 Requires-Dist: scikit-learn (>=0.24.2,<0.25.0)
 Requires-Dist: scipy (>=1.6.3,<2.0.0)
-Requires-Dist: seaborn (>=0.11.2,<0.12.0)
+Requires-Dist: seaborn (>=0.13.1,<0.14.0)
 Project-URL: Documentation, https://avn.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/theresekoch/avn
 Description-Content-Type: text/markdown
 
 # avn 
 
 [![Python](https://img.shields.io/badge/python-3.9-blue)]()
```


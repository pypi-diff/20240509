# Comparing `tmp/keras-visualizer-3.1.2.tar.gz` & `tmp/keras_visualizer-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-visualizer-3.1.2.tar", last modified: Tue Apr 11 08:41:11 2023, max compression
+gzip compressed data, was "keras_visualizer-3.2.0.tar", last modified: Thu May  9 21:30:36 2024, max compression
```

## Comparing `keras-visualizer-3.1.2.tar` & `keras_visualizer-3.2.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:41:11.708169 keras-visualizer-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-11 08:41:02.000000 keras-visualizer-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-11 08:41:11.704169 keras-visualizer-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-11 08:41:02.000000 keras-visualizer-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:41:11.704169 keras-visualizer-3.1.2/keras_visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-11 08:41:02.000000 keras-visualizer-3.1.2/keras_visualizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:41:11.704169 keras-visualizer-3.1.2/keras_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 08:41:11.000000 keras-visualizer-3.1.2/keras_visualizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:41:11.708169 keras-visualizer-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-11 08:41:02.000000 keras-visualizer-3.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:30:36.141384 keras_visualizer-3.2.0/
+-rw-rw-rw-   0        0        0     1078 2023-03-01 19:54:21.000000 keras_visualizer-3.2.0/LICENSE
+-rw-rw-rw-   0        0        0     7559 2024-05-09 21:30:36.141384 keras_visualizer-3.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7062 2023-04-11 08:31:30.000000 keras_visualizer-3.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 21:30:36.135382 keras_visualizer-3.2.0/examples/
+-rw-rw-rw-   0        0        0     2304 2023-03-08 09:51:42.000000 keras_visualizer-3.2.0/examples/example1.ipynb
+-rw-rw-rw-   0        0        0      331 2023-03-08 09:32:08.000000 keras_visualizer-3.2.0/examples/example1.py
+-rw-rw-rw-   0        0        0   602473 2023-03-08 08:59:18.000000 keras_visualizer-3.2.0/examples/example1_output.png
+-rw-rw-rw-   0        0        0     2426 2023-03-08 09:51:42.000000 keras_visualizer-3.2.0/examples/example2.ipynb
+-rw-rw-rw-   0        0        0      437 2023-03-08 09:04:51.000000 keras_visualizer-3.2.0/examples/example2.py
+-rw-rw-rw-   0        0        0    71311 2023-03-08 09:05:59.000000 keras_visualizer-3.2.0/examples/example2_output.png
+drwxrwxrwx   0        0        0        0 2024-05-09 21:30:36.135382 keras_visualizer-3.2.0/keras_visualizer/
+-rw-rw-rw-   0        0        0    14815 2024-05-09 21:13:35.000000 keras_visualizer-3.2.0/keras_visualizer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 21:30:36.140380 keras_visualizer-3.2.0/keras_visualizer.egg-info/
+-rw-rw-rw-   0        0        0     7559 2024-05-09 21:30:36.000000 keras_visualizer-3.2.0/keras_visualizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      402 2024-05-09 21:30:36.000000 keras_visualizer-3.2.0/keras_visualizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 21:30:36.000000 keras_visualizer-3.2.0/keras_visualizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 21:30:36.000000 keras_visualizer-3.2.0/keras_visualizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-09 21:30:36.000000 keras_visualizer-3.2.0/keras_visualizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 21:30:36.141384 keras_visualizer-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-05-09 21:18:02.000000 keras_visualizer-3.2.0/setup.py
```

### Comparing `keras-visualizer-3.1.2/PKG-INFO` & `keras_visualizer-3.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,276 +1,277 @@
-Metadata-Version: 2.1
-Name: keras-visualizer
-Version: 3.1.2
-Summary: A Keras Model Visualizer
-Home-page: https://github.com/lordmahyar/keras-visualizer
-Author: Mahyar Amiri
-Author-email: mmaahhyyaarr@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Keras Visualizer
-
-![LOGO](logo.png)
-
-[![PyPI](https://img.shields.io/pypi/v/keras-visualizer?label=PyPI&logo=pypi&logoColor=FFE873)](https://pypi.org/project/keras-visualizer)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-visualizer?label=Downloads&color=blue)](https://pypistats.org/packages/keras-visualizer)
-[![GitHub - License](https://img.shields.io/github/license/mahyar-amiri/django-comment-system?label=License&color=blue)](LICENSE)
-[![Virgool.io](https://img.shields.io/static/v1?label=Virgool.io&message=keras-visualizer&color=blue)](https://vrgl.ir/5KSoN)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahyar-amiri/keras-visualizer/)
-
-A Python Library for Visualizing Keras Models.
-
-## Table of Contents
-
-<!-- TOC -->
-
-* [Keras Visualizer](#keras-visualizer)
-    * [Table of Contents](#table-of-contents)
-    * [Installation](#installation)
-        * [Install](#install)
-        * [Upgrade](#upgrade)
-    * [Usage](#usage)
-    * [Parameters](#parameters)
-    * [Settings](#settings)
-    * [Examples](#examples)
-        * [Example 1](#example-1)
-        * [Example 2](#example-2)
-        * [Example 3](#example-3)
-    * [Supported layers](#supported-layers)
-
-<!-- TOC -->
-
-## Installation
-
-### Install
-
-Use python package manager (pip) to install Keras Visualizer.
-
-```bash
-pip install keras-visualizer
-```
-
-### Upgrade
-
-Use python package manager (pip) to upgrade Keras Visualizer.
-
-```bash
-pip install keras-visualizer --upgrade
-```
-
-## Usage
-
-```python
-from keras_visualizer import visualizer
-
-# create your model here
-# model = ...
-
-visualizer(model, file_format='png')
-```
-
-## Parameters
-
-```python
-visualizer(model, file_name='graph', file_format=None, view=False, settings=None)
-```
-
-- `model` : a Keras model instance.
-- `file_name` : where to save the visualization.
-- `file_format` : file format to save 'pdf', 'png'.
-- `view` : open file after process if True.
-- `settings` : a dictionary of available settings.
-
-> **Note :**
-> - set `file_format='png'` or `file_format='pdf'` to save visualization file.
-> - use `view=True` to open visualization file.
-> - use [settings](#settings) to customize output image.
-
-## Settings
-
-you can customize settings for your output image. here is the default settings dictionary:
-
-```python
-settings = {
-    # ALL LAYERS
-    'MAX_NEURONS': 10,
-    'ARROW_COLOR': '#707070',
-    # INPUT LAYERS
-    'INPUT_DENSE_COLOR': '#2ecc71',
-    'INPUT_EMBEDDING_COLOR': 'black',
-    'INPUT_EMBEDDING_FONT': 'white',
-    'INPUT_GRAYSCALE_COLOR': 'black:white',
-    'INPUT_GRAYSCALE_FONT': 'white',
-    'INPUT_RGB_COLOR': '#e74c3c:#3498db',
-    'INPUT_RGB_FONT': 'white',
-    'INPUT_LAYER_COLOR': 'black',
-    'INPUT_LAYER_FONT': 'white',
-    # HIDDEN LAYERS
-    'HIDDEN_DENSE_COLOR': '#3498db',
-    'HIDDEN_CONV_COLOR': '#5faad0',
-    'HIDDEN_CONV_FONT': 'black',
-    'HIDDEN_POOLING_COLOR': '#8e44ad',
-    'HIDDEN_POOLING_FONT': 'white',
-    'HIDDEN_FLATTEN_COLOR': '#2c3e50',
-    'HIDDEN_FLATTEN_FONT': 'white',
-    'HIDDEN_DROPOUT_COLOR': '#f39c12',
-    'HIDDEN_DROPOUT_FONT': 'black',
-    'HIDDEN_ACTIVATION_COLOR': '#00b894',
-    'HIDDEN_ACTIVATION_FONT': 'black',
-    'HIDDEN_LAYER_COLOR': 'black',
-    'HIDDEN_LAYER_FONT': 'white',
-    # OUTPUT LAYER
-    'OUTPUT_DENSE_COLOR': '#e74c3c',
-    'OUTPUT_LAYER_COLOR': 'black',
-    'OUTPUT_LAYER_FONT': 'white',
-}
-```
-
-**Note**:
-
-* set `'MAX_NEURONS': None` to disable max neurons constraint.
-* see list of color names [here](https://graphviz.org/doc/info/colors.html).
-
-```python
-from keras_visualizer import visualizer
-
-my_settings = {
-    'MAX_NEURONS': None,
-    'INPUT_DENSE_COLOR': 'teal',
-    'HIDDEN_DENSE_COLOR': 'gray',
-    'OUTPUT_DENSE_COLOR': 'crimson'
-}
-
-# model = ...
-
-visualizer(model, file_format='png', settings=my_settings)
-```
-
-## Examples
-
-you can use simple examples as `.py` or `.ipynb` format in [examples directory](examples).
-
-### Example 1
-
-```python
-from keras import models, layers
-from keras_visualizer import visualizer
-
-model = models.Sequential([
-    layers.Dense(64, activation='relu', input_shape=(8,)),
-    layers.Dense(6, activation='softmax'),
-    layers.Dense(32),
-    layers.Dense(9, activation='sigmoid')
-])
-
-visualizer(model, file_format='png', view=True)
-```
-
-![example 1](examples/example1_output.png)
-
----
-
-### Example 2
-
-```python
-from keras import models, layers
-from keras_visualizer import visualizer
-
-model = models.Sequential()
-model.add(layers.Conv2D(64, (3, 3), input_shape=(28, 28, 3), activation='relu'))
-model.add(layers.MaxPooling2D((2, 2)))
-model.add(layers.Flatten())
-model.add(layers.Dense(3))
-model.add(layers.Dropout(0.5))
-model.add(layers.Activation('sigmoid'))
-model.add(layers.Dense(1))
-
-visualizer(model, file_format='png', view=True)
-```
-
-![example 2](examples/example2_output.png)
-
----
-
-### Example 3
-
-```python
-from keras import models, layers
-from keras_visualizer import visualizer
-
-model = models.Sequential()
-model.add(layers.Embedding(64, output_dim=256))
-model.add(layers.LSTM(128))
-model.add(layers.Dense(1, activation='sigmoid'))
-
-visualizer(model, file_format='png', view=True)
-```
-
-![example 3](examples/example3_output.png)
-
-## Supported layers
-
-[Explore list of **keras layers**](https://keras.io/api/layers/)
-
-1. Core layers
-    - [x] Input object
-    - [x] Dense layer
-    - [x] Activation layer
-    - [ ] Embedding layer
-    - [ ] Masking layer
-    - [ ] Lambda layer
-
-2. Convolution layers
-    - [x] Conv1D layer
-    - [x] Conv2D layer
-    - [x] Conv3D layer
-    - [x] SeparableConv1D layer
-    - [x] SeparableConv2D layer
-    - [x] DepthwiseConv2D layer
-    - [x] Conv1DTranspose layer
-    - [x] Conv2DTranspose layer
-    - [x] Conv3DTranspose layer
-
-3. Pooling layers
-    - [x] MaxPooling1D layer
-    - [x] MaxPooling2D layer
-    - [x] MaxPooling3D layer
-    - [x] AveragePooling1D layer
-    - [x] AveragePooling2D layer
-    - [x] AveragePooling3D layer
-    - [x] GlobalMaxPooling1D layer
-    - [x] GlobalMaxPooling2D layer
-    - [x] GlobalMaxPooling3D layer
-    - [x] GlobalAveragePooling1D layer
-    - [x] GlobalAveragePooling2D layer
-    - [x] GlobalAveragePooling3D layer
-
-4. Reshaping layers
-    - [ ] Reshape layer
-    - [x] Flatten layer
-    - [ ] RepeatVector layer
-    - [ ] Permute layer
-    - [ ] Cropping1D layer
-    - [ ] Cropping2D layer
-    - [ ] Cropping3D layer
-    - [ ] UpSampling1D layer
-    - [ ] UpSampling2D layer
-    - [ ] UpSampling3D layer
-    - [ ] ZeroPadding1D layer
-    - [ ] ZeroPadding2D layer
-    - [ ] ZeroPadding3D layer
-
-5. Regularization layers
-    - [x] Dropout layer
-    - [x] SpatialDropout1D layer
-    - [x] SpatialDropout2D layer
-    - [x] SpatialDropout3D layer
-    - [x] GaussianDropout layer
-    - [ ] GaussianNoise layer
-    - [ ] ActivityRegularization layer
-    - [x] AlphaDropout layer
+Metadata-Version: 2.1
+Name: keras-visualizer
+Version: 3.2.0
+Summary: A Keras Model Visualizer
+Home-page: https://github.com/lordmahyar/keras-visualizer
+Author: Mahyar Amiri
+Author-email: mmaahhyyaarr@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: graphviz
+
+# Keras Visualizer
+
+![LOGO](logo.png)
+
+[![PyPI](https://img.shields.io/pypi/v/keras-visualizer?label=PyPI&logo=pypi&logoColor=FFE873)](https://pypi.org/project/keras-visualizer)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-visualizer?label=Downloads&color=blue)](https://pypistats.org/packages/keras-visualizer)
+[![GitHub - License](https://img.shields.io/github/license/mahyar-amiri/django-comment-system?label=License&color=blue)](LICENSE)
+[![Virgool.io](https://img.shields.io/static/v1?label=Virgool.io&message=keras-visualizer&color=blue)](https://vrgl.ir/5KSoN)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahyar-amiri/keras-visualizer/)
+
+A Python Library for Visualizing Keras Models.
+
+## Table of Contents
+
+<!-- TOC -->
+
+* [Keras Visualizer](#keras-visualizer)
+    * [Table of Contents](#table-of-contents)
+    * [Installation](#installation)
+        * [Install](#install)
+        * [Upgrade](#upgrade)
+    * [Usage](#usage)
+    * [Parameters](#parameters)
+    * [Settings](#settings)
+    * [Examples](#examples)
+        * [Example 1](#example-1)
+        * [Example 2](#example-2)
+        * [Example 3](#example-3)
+    * [Supported layers](#supported-layers)
+
+<!-- TOC -->
+
+## Installation
+
+### Install
+
+Use python package manager (pip) to install Keras Visualizer.
+
+```bash
+pip install keras-visualizer
+```
+
+### Upgrade
+
+Use python package manager (pip) to upgrade Keras Visualizer.
+
+```bash
+pip install keras-visualizer --upgrade
+```
+
+## Usage
+
+```python
+from keras_visualizer import visualizer
+
+# create your model here
+# model = ...
+
+visualizer(model, file_format='png')
+```
+
+## Parameters
+
+```python
+visualizer(model, file_name='graph', file_format=None, view=False, settings=None)
+```
+
+- `model` : a Keras model instance.
+- `file_name` : where to save the visualization.
+- `file_format` : file format to save 'pdf', 'png'.
+- `view` : open file after process if True.
+- `settings` : a dictionary of available settings.
+
+> **Note :**
+> - set `file_format='png'` or `file_format='pdf'` to save visualization file.
+> - use `view=True` to open visualization file.
+> - use [settings](#settings) to customize output image.
+
+## Settings
+
+you can customize settings for your output image. here is the default settings dictionary:
+
+```python
+settings = {
+    # ALL LAYERS
+    'MAX_NEURONS': 10,
+    'ARROW_COLOR': '#707070',
+    # INPUT LAYERS
+    'INPUT_DENSE_COLOR': '#2ecc71',
+    'INPUT_EMBEDDING_COLOR': 'black',
+    'INPUT_EMBEDDING_FONT': 'white',
+    'INPUT_GRAYSCALE_COLOR': 'black:white',
+    'INPUT_GRAYSCALE_FONT': 'white',
+    'INPUT_RGB_COLOR': '#e74c3c:#3498db',
+    'INPUT_RGB_FONT': 'white',
+    'INPUT_LAYER_COLOR': 'black',
+    'INPUT_LAYER_FONT': 'white',
+    # HIDDEN LAYERS
+    'HIDDEN_DENSE_COLOR': '#3498db',
+    'HIDDEN_CONV_COLOR': '#5faad0',
+    'HIDDEN_CONV_FONT': 'black',
+    'HIDDEN_POOLING_COLOR': '#8e44ad',
+    'HIDDEN_POOLING_FONT': 'white',
+    'HIDDEN_FLATTEN_COLOR': '#2c3e50',
+    'HIDDEN_FLATTEN_FONT': 'white',
+    'HIDDEN_DROPOUT_COLOR': '#f39c12',
+    'HIDDEN_DROPOUT_FONT': 'black',
+    'HIDDEN_ACTIVATION_COLOR': '#00b894',
+    'HIDDEN_ACTIVATION_FONT': 'black',
+    'HIDDEN_LAYER_COLOR': 'black',
+    'HIDDEN_LAYER_FONT': 'white',
+    # OUTPUT LAYER
+    'OUTPUT_DENSE_COLOR': '#e74c3c',
+    'OUTPUT_LAYER_COLOR': 'black',
+    'OUTPUT_LAYER_FONT': 'white',
+}
+```
+
+**Note**:
+
+* set `'MAX_NEURONS': None` to disable max neurons constraint.
+* see list of color names [here](https://graphviz.org/doc/info/colors.html).
+
+```python
+from keras_visualizer import visualizer
+
+my_settings = {
+    'MAX_NEURONS': None,
+    'INPUT_DENSE_COLOR': 'teal',
+    'HIDDEN_DENSE_COLOR': 'gray',
+    'OUTPUT_DENSE_COLOR': 'crimson'
+}
+
+# model = ...
+
+visualizer(model, file_format='png', settings=my_settings)
+```
+
+## Examples
+
+you can use simple examples as `.py` or `.ipynb` format in [examples directory](examples).
+
+### Example 1
+
+```python
+from keras import models, layers
+from keras_visualizer import visualizer
+
+model = models.Sequential([
+    layers.Dense(64, activation='relu', input_shape=(8,)),
+    layers.Dense(6, activation='softmax'),
+    layers.Dense(32),
+    layers.Dense(9, activation='sigmoid')
+])
+
+visualizer(model, file_format='png', view=True)
+```
+
+![example 1](examples/example1_output.png)
+
+---
+
+### Example 2
+
+```python
+from keras import models, layers
+from keras_visualizer import visualizer
+
+model = models.Sequential()
+model.add(layers.Conv2D(64, (3, 3), input_shape=(28, 28, 3), activation='relu'))
+model.add(layers.MaxPooling2D((2, 2)))
+model.add(layers.Flatten())
+model.add(layers.Dense(3))
+model.add(layers.Dropout(0.5))
+model.add(layers.Activation('sigmoid'))
+model.add(layers.Dense(1))
+
+visualizer(model, file_format='png', view=True)
+```
+
+![example 2](examples/example2_output.png)
+
+---
+
+### Example 3
+
+```python
+from keras import models, layers
+from keras_visualizer import visualizer
+
+model = models.Sequential()
+model.add(layers.Embedding(64, output_dim=256))
+model.add(layers.LSTM(128))
+model.add(layers.Dense(1, activation='sigmoid'))
+
+visualizer(model, file_format='png', view=True)
+```
+
+![example 3](examples/example3_output.png)
+
+## Supported layers
+
+[Explore list of **keras layers**](https://keras.io/api/layers/)
+
+1. Core layers
+    - [x] Input object
+    - [x] Dense layer
+    - [x] Activation layer
+    - [ ] Embedding layer
+    - [ ] Masking layer
+    - [ ] Lambda layer
+
+2. Convolution layers
+    - [x] Conv1D layer
+    - [x] Conv2D layer
+    - [x] Conv3D layer
+    - [x] SeparableConv1D layer
+    - [x] SeparableConv2D layer
+    - [x] DepthwiseConv2D layer
+    - [x] Conv1DTranspose layer
+    - [x] Conv2DTranspose layer
+    - [x] Conv3DTranspose layer
+
+3. Pooling layers
+    - [x] MaxPooling1D layer
+    - [x] MaxPooling2D layer
+    - [x] MaxPooling3D layer
+    - [x] AveragePooling1D layer
+    - [x] AveragePooling2D layer
+    - [x] AveragePooling3D layer
+    - [x] GlobalMaxPooling1D layer
+    - [x] GlobalMaxPooling2D layer
+    - [x] GlobalMaxPooling3D layer
+    - [x] GlobalAveragePooling1D layer
+    - [x] GlobalAveragePooling2D layer
+    - [x] GlobalAveragePooling3D layer
+
+4. Reshaping layers
+    - [ ] Reshape layer
+    - [x] Flatten layer
+    - [ ] RepeatVector layer
+    - [ ] Permute layer
+    - [ ] Cropping1D layer
+    - [ ] Cropping2D layer
+    - [ ] Cropping3D layer
+    - [ ] UpSampling1D layer
+    - [ ] UpSampling2D layer
+    - [ ] UpSampling3D layer
+    - [ ] ZeroPadding1D layer
+    - [ ] ZeroPadding2D layer
+    - [ ] ZeroPadding3D layer
+
+5. Regularization layers
+    - [x] Dropout layer
+    - [x] SpatialDropout1D layer
+    - [x] SpatialDropout2D layer
+    - [x] SpatialDropout3D layer
+    - [x] GaussianDropout layer
+    - [ ] GaussianNoise layer
+    - [ ] ActivityRegularization layer
+    - [x] AlphaDropout layer
```

### Comparing `keras-visualizer-3.1.2/README.md` & `keras_visualizer-3.2.0/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-# Keras Visualizer
-
-![LOGO](logo.png)
-
-[![PyPI](https://img.shields.io/pypi/v/keras-visualizer?label=PyPI&logo=pypi&logoColor=FFE873)](https://pypi.org/project/keras-visualizer)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-visualizer?label=Downloads&color=blue)](https://pypistats.org/packages/keras-visualizer)
-[![GitHub - License](https://img.shields.io/github/license/mahyar-amiri/django-comment-system?label=License&color=blue)](LICENSE)
-[![Virgool.io](https://img.shields.io/static/v1?label=Virgool.io&message=keras-visualizer&color=blue)](https://vrgl.ir/5KSoN)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahyar-amiri/keras-visualizer/)
-
-A Python Library for Visualizing Keras Models.
-
-## Table of Contents
-
-<!-- TOC -->
-
-* [Keras Visualizer](#keras-visualizer)
-    * [Table of Contents](#table-of-contents)
-    * [Installation](#installation)
-        * [Install](#install)
-        * [Upgrade](#upgrade)
-    * [Usage](#usage)
-    * [Parameters](#parameters)
-    * [Settings](#settings)
-    * [Examples](#examples)
-        * [Example 1](#example-1)
-        * [Example 2](#example-2)
-        * [Example 3](#example-3)
-    * [Supported layers](#supported-layers)
-
-<!-- TOC -->
-
-## Installation
-
-### Install
-
-Use python package manager (pip) to install Keras Visualizer.
-
-```bash
-pip install keras-visualizer
-```
-
-### Upgrade
-
-Use python package manager (pip) to upgrade Keras Visualizer.
-
-```bash
-pip install keras-visualizer --upgrade
-```
-
-## Usage
-
-```python
-from keras_visualizer import visualizer
-
-# create your model here
-# model = ...
-
-visualizer(model, file_format='png')
-```
-
-## Parameters
-
-```python
-visualizer(model, file_name='graph', file_format=None, view=False, settings=None)
-```
-
-- `model` : a Keras model instance.
-- `file_name` : where to save the visualization.
-- `file_format` : file format to save 'pdf', 'png'.
-- `view` : open file after process if True.
-- `settings` : a dictionary of available settings.
-
-> **Note :**
-> - set `file_format='png'` or `file_format='pdf'` to save visualization file.
-> - use `view=True` to open visualization file.
-> - use [settings](#settings) to customize output image.
-
-## Settings
-
-you can customize settings for your output image. here is the default settings dictionary:
-
-```python
-settings = {
-    # ALL LAYERS
-    'MAX_NEURONS': 10,
-    'ARROW_COLOR': '#707070',
-    # INPUT LAYERS
-    'INPUT_DENSE_COLOR': '#2ecc71',
-    'INPUT_EMBEDDING_COLOR': 'black',
-    'INPUT_EMBEDDING_FONT': 'white',
-    'INPUT_GRAYSCALE_COLOR': 'black:white',
-    'INPUT_GRAYSCALE_FONT': 'white',
-    'INPUT_RGB_COLOR': '#e74c3c:#3498db',
-    'INPUT_RGB_FONT': 'white',
-    'INPUT_LAYER_COLOR': 'black',
-    'INPUT_LAYER_FONT': 'white',
-    # HIDDEN LAYERS
-    'HIDDEN_DENSE_COLOR': '#3498db',
-    'HIDDEN_CONV_COLOR': '#5faad0',
-    'HIDDEN_CONV_FONT': 'black',
-    'HIDDEN_POOLING_COLOR': '#8e44ad',
-    'HIDDEN_POOLING_FONT': 'white',
-    'HIDDEN_FLATTEN_COLOR': '#2c3e50',
-    'HIDDEN_FLATTEN_FONT': 'white',
-    'HIDDEN_DROPOUT_COLOR': '#f39c12',
-    'HIDDEN_DROPOUT_FONT': 'black',
-    'HIDDEN_ACTIVATION_COLOR': '#00b894',
-    'HIDDEN_ACTIVATION_FONT': 'black',
-    'HIDDEN_LAYER_COLOR': 'black',
-    'HIDDEN_LAYER_FONT': 'white',
-    # OUTPUT LAYER
-    'OUTPUT_DENSE_COLOR': '#e74c3c',
-    'OUTPUT_LAYER_COLOR': 'black',
-    'OUTPUT_LAYER_FONT': 'white',
-}
-```
-
-**Note**:
-
-* set `'MAX_NEURONS': None` to disable max neurons constraint.
-* see list of color names [here](https://graphviz.org/doc/info/colors.html).
-
-```python
-from keras_visualizer import visualizer
-
-my_settings = {
-    'MAX_NEURONS': None,
-    'INPUT_DENSE_COLOR': 'teal',
-    'HIDDEN_DENSE_COLOR': 'gray',
-    'OUTPUT_DENSE_COLOR': 'crimson'
-}
-
-# model = ...
-
-visualizer(model, file_format='png', settings=my_settings)
-```
-
-## Examples
-
-you can use simple examples as `.py` or `.ipynb` format in [examples directory](examples).
-
-### Example 1
-
-```python
-from keras import models, layers
-from keras_visualizer import visualizer
-
-model = models.Sequential([
-    layers.Dense(64, activation='relu', input_shape=(8,)),
-    layers.Dense(6, activation='softmax'),
-    layers.Dense(32),
-    layers.Dense(9, activation='sigmoid')
-])
-
-visualizer(model, file_format='png', view=True)
-```
-
-![example 1](examples/example1_output.png)
-
----
-
-### Example 2
-
-```python
-from keras import models, layers
-from keras_visualizer import visualizer
-
-model = models.Sequential()
-model.add(layers.Conv2D(64, (3, 3), input_shape=(28, 28, 3), activation='relu'))
-model.add(layers.MaxPooling2D((2, 2)))
-model.add(layers.Flatten())
-model.add(layers.Dense(3))
-model.add(layers.Dropout(0.5))
-model.add(layers.Activation('sigmoid'))
-model.add(layers.Dense(1))
-
-visualizer(model, file_format='png', view=True)
-```
-
-![example 2](examples/example2_output.png)
-
----
-
-### Example 3
-
-```python
-from keras import models, layers
-from keras_visualizer import visualizer
-
-model = models.Sequential()
-model.add(layers.Embedding(64, output_dim=256))
-model.add(layers.LSTM(128))
-model.add(layers.Dense(1, activation='sigmoid'))
-
-visualizer(model, file_format='png', view=True)
-```
-
-![example 3](examples/example3_output.png)
-
-## Supported layers
-
-[Explore list of **keras layers**](https://keras.io/api/layers/)
-
-1. Core layers
-    - [x] Input object
-    - [x] Dense layer
-    - [x] Activation layer
-    - [ ] Embedding layer
-    - [ ] Masking layer
-    - [ ] Lambda layer
-
-2. Convolution layers
-    - [x] Conv1D layer
-    - [x] Conv2D layer
-    - [x] Conv3D layer
-    - [x] SeparableConv1D layer
-    - [x] SeparableConv2D layer
-    - [x] DepthwiseConv2D layer
-    - [x] Conv1DTranspose layer
-    - [x] Conv2DTranspose layer
-    - [x] Conv3DTranspose layer
-
-3. Pooling layers
-    - [x] MaxPooling1D layer
-    - [x] MaxPooling2D layer
-    - [x] MaxPooling3D layer
-    - [x] AveragePooling1D layer
-    - [x] AveragePooling2D layer
-    - [x] AveragePooling3D layer
-    - [x] GlobalMaxPooling1D layer
-    - [x] GlobalMaxPooling2D layer
-    - [x] GlobalMaxPooling3D layer
-    - [x] GlobalAveragePooling1D layer
-    - [x] GlobalAveragePooling2D layer
-    - [x] GlobalAveragePooling3D layer
-
-4. Reshaping layers
-    - [ ] Reshape layer
-    - [x] Flatten layer
-    - [ ] RepeatVector layer
-    - [ ] Permute layer
-    - [ ] Cropping1D layer
-    - [ ] Cropping2D layer
-    - [ ] Cropping3D layer
-    - [ ] UpSampling1D layer
-    - [ ] UpSampling2D layer
-    - [ ] UpSampling3D layer
-    - [ ] ZeroPadding1D layer
-    - [ ] ZeroPadding2D layer
-    - [ ] ZeroPadding3D layer
-
-5. Regularization layers
-    - [x] Dropout layer
-    - [x] SpatialDropout1D layer
-    - [x] SpatialDropout2D layer
-    - [x] SpatialDropout3D layer
-    - [x] GaussianDropout layer
-    - [ ] GaussianNoise layer
-    - [ ] ActivityRegularization layer
+# Keras Visualizer
+
+![LOGO](logo.png)
+
+[![PyPI](https://img.shields.io/pypi/v/keras-visualizer?label=PyPI&logo=pypi&logoColor=FFE873)](https://pypi.org/project/keras-visualizer)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-visualizer?label=Downloads&color=blue)](https://pypistats.org/packages/keras-visualizer)
+[![GitHub - License](https://img.shields.io/github/license/mahyar-amiri/django-comment-system?label=License&color=blue)](LICENSE)
+[![Virgool.io](https://img.shields.io/static/v1?label=Virgool.io&message=keras-visualizer&color=blue)](https://vrgl.ir/5KSoN)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahyar-amiri/keras-visualizer/)
+
+A Python Library for Visualizing Keras Models.
+
+## Table of Contents
+
+<!-- TOC -->
+
+* [Keras Visualizer](#keras-visualizer)
+    * [Table of Contents](#table-of-contents)
+    * [Installation](#installation)
+        * [Install](#install)
+        * [Upgrade](#upgrade)
+    * [Usage](#usage)
+    * [Parameters](#parameters)
+    * [Settings](#settings)
+    * [Examples](#examples)
+        * [Example 1](#example-1)
+        * [Example 2](#example-2)
+        * [Example 3](#example-3)
+    * [Supported layers](#supported-layers)
+
+<!-- TOC -->
+
+## Installation
+
+### Install
+
+Use python package manager (pip) to install Keras Visualizer.
+
+```bash
+pip install keras-visualizer
+```
+
+### Upgrade
+
+Use python package manager (pip) to upgrade Keras Visualizer.
+
+```bash
+pip install keras-visualizer --upgrade
+```
+
+## Usage
+
+```python
+from keras_visualizer import visualizer
+
+# create your model here
+# model = ...
+
+visualizer(model, file_format='png')
+```
+
+## Parameters
+
+```python
+visualizer(model, file_name='graph', file_format=None, view=False, settings=None)
+```
+
+- `model` : a Keras model instance.
+- `file_name` : where to save the visualization.
+- `file_format` : file format to save 'pdf', 'png'.
+- `view` : open file after process if True.
+- `settings` : a dictionary of available settings.
+
+> **Note :**
+> - set `file_format='png'` or `file_format='pdf'` to save visualization file.
+> - use `view=True` to open visualization file.
+> - use [settings](#settings) to customize output image.
+
+## Settings
+
+you can customize settings for your output image. here is the default settings dictionary:
+
+```python
+settings = {
+    # ALL LAYERS
+    'MAX_NEURONS': 10,
+    'ARROW_COLOR': '#707070',
+    # INPUT LAYERS
+    'INPUT_DENSE_COLOR': '#2ecc71',
+    'INPUT_EMBEDDING_COLOR': 'black',
+    'INPUT_EMBEDDING_FONT': 'white',
+    'INPUT_GRAYSCALE_COLOR': 'black:white',
+    'INPUT_GRAYSCALE_FONT': 'white',
+    'INPUT_RGB_COLOR': '#e74c3c:#3498db',
+    'INPUT_RGB_FONT': 'white',
+    'INPUT_LAYER_COLOR': 'black',
+    'INPUT_LAYER_FONT': 'white',
+    # HIDDEN LAYERS
+    'HIDDEN_DENSE_COLOR': '#3498db',
+    'HIDDEN_CONV_COLOR': '#5faad0',
+    'HIDDEN_CONV_FONT': 'black',
+    'HIDDEN_POOLING_COLOR': '#8e44ad',
+    'HIDDEN_POOLING_FONT': 'white',
+    'HIDDEN_FLATTEN_COLOR': '#2c3e50',
+    'HIDDEN_FLATTEN_FONT': 'white',
+    'HIDDEN_DROPOUT_COLOR': '#f39c12',
+    'HIDDEN_DROPOUT_FONT': 'black',
+    'HIDDEN_ACTIVATION_COLOR': '#00b894',
+    'HIDDEN_ACTIVATION_FONT': 'black',
+    'HIDDEN_LAYER_COLOR': 'black',
+    'HIDDEN_LAYER_FONT': 'white',
+    # OUTPUT LAYER
+    'OUTPUT_DENSE_COLOR': '#e74c3c',
+    'OUTPUT_LAYER_COLOR': 'black',
+    'OUTPUT_LAYER_FONT': 'white',
+}
+```
+
+**Note**:
+
+* set `'MAX_NEURONS': None` to disable max neurons constraint.
+* see list of color names [here](https://graphviz.org/doc/info/colors.html).
+
+```python
+from keras_visualizer import visualizer
+
+my_settings = {
+    'MAX_NEURONS': None,
+    'INPUT_DENSE_COLOR': 'teal',
+    'HIDDEN_DENSE_COLOR': 'gray',
+    'OUTPUT_DENSE_COLOR': 'crimson'
+}
+
+# model = ...
+
+visualizer(model, file_format='png', settings=my_settings)
+```
+
+## Examples
+
+you can use simple examples as `.py` or `.ipynb` format in [examples directory](examples).
+
+### Example 1
+
+```python
+from keras import models, layers
+from keras_visualizer import visualizer
+
+model = models.Sequential([
+    layers.Dense(64, activation='relu', input_shape=(8,)),
+    layers.Dense(6, activation='softmax'),
+    layers.Dense(32),
+    layers.Dense(9, activation='sigmoid')
+])
+
+visualizer(model, file_format='png', view=True)
+```
+
+![example 1](examples/example1_output.png)
+
+---
+
+### Example 2
+
+```python
+from keras import models, layers
+from keras_visualizer import visualizer
+
+model = models.Sequential()
+model.add(layers.Conv2D(64, (3, 3), input_shape=(28, 28, 3), activation='relu'))
+model.add(layers.MaxPooling2D((2, 2)))
+model.add(layers.Flatten())
+model.add(layers.Dense(3))
+model.add(layers.Dropout(0.5))
+model.add(layers.Activation('sigmoid'))
+model.add(layers.Dense(1))
+
+visualizer(model, file_format='png', view=True)
+```
+
+![example 2](examples/example2_output.png)
+
+---
+
+### Example 3
+
+```python
+from keras import models, layers
+from keras_visualizer import visualizer
+
+model = models.Sequential()
+model.add(layers.Embedding(64, output_dim=256))
+model.add(layers.LSTM(128))
+model.add(layers.Dense(1, activation='sigmoid'))
+
+visualizer(model, file_format='png', view=True)
+```
+
+![example 3](examples/example3_output.png)
+
+## Supported layers
+
+[Explore list of **keras layers**](https://keras.io/api/layers/)
+
+1. Core layers
+    - [x] Input object
+    - [x] Dense layer
+    - [x] Activation layer
+    - [ ] Embedding layer
+    - [ ] Masking layer
+    - [ ] Lambda layer
+
+2. Convolution layers
+    - [x] Conv1D layer
+    - [x] Conv2D layer
+    - [x] Conv3D layer
+    - [x] SeparableConv1D layer
+    - [x] SeparableConv2D layer
+    - [x] DepthwiseConv2D layer
+    - [x] Conv1DTranspose layer
+    - [x] Conv2DTranspose layer
+    - [x] Conv3DTranspose layer
+
+3. Pooling layers
+    - [x] MaxPooling1D layer
+    - [x] MaxPooling2D layer
+    - [x] MaxPooling3D layer
+    - [x] AveragePooling1D layer
+    - [x] AveragePooling2D layer
+    - [x] AveragePooling3D layer
+    - [x] GlobalMaxPooling1D layer
+    - [x] GlobalMaxPooling2D layer
+    - [x] GlobalMaxPooling3D layer
+    - [x] GlobalAveragePooling1D layer
+    - [x] GlobalAveragePooling2D layer
+    - [x] GlobalAveragePooling3D layer
+
+4. Reshaping layers
+    - [ ] Reshape layer
+    - [x] Flatten layer
+    - [ ] RepeatVector layer
+    - [ ] Permute layer
+    - [ ] Cropping1D layer
+    - [ ] Cropping2D layer
+    - [ ] Cropping3D layer
+    - [ ] UpSampling1D layer
+    - [ ] UpSampling2D layer
+    - [ ] UpSampling3D layer
+    - [ ] ZeroPadding1D layer
+    - [ ] ZeroPadding2D layer
+    - [ ] ZeroPadding3D layer
+
+5. Regularization layers
+    - [x] Dropout layer
+    - [x] SpatialDropout1D layer
+    - [x] SpatialDropout2D layer
+    - [x] SpatialDropout3D layer
+    - [x] GaussianDropout layer
+    - [ ] GaussianNoise layer
+    - [ ] ActivityRegularization layer
     - [x] AlphaDropout layer
```

### Comparing `keras-visualizer-3.1.2/keras_visualizer/__init__.py` & `keras_visualizer-3.2.0/keras_visualizer/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,266 +1,295 @@
-def visualizer(model, file_name='graph', file_format=None, view=False, settings=None):
-    """Visualize a Sequential model.
-
-    # Arguments
-
-        model: a Keras model instance.
-
-        file_name: where to save the visualization.
-
-        file_format: file format to save 'pdf', 'png'.
-
-        view: open file after process if True.
-
-        settings: dictionary of valid configurations.
-
-    * change format to 'png' or 'pdf' to save visualization file
-    """
-    from graphviz import Digraph
-
-    main_settings = {
-        # ALL LAYERS
-        'MAX_NEURONS': 10,
-        'ARROW_COLOR': '#707070',
-        # INPUT LAYERS
-        'INPUT_DENSE_COLOR': '#2ecc71',
-        'INPUT_EMBEDDING_COLOR': 'black',
-        'INPUT_EMBEDDING_FONT': 'white',
-        'INPUT_GRAYSCALE_COLOR': 'black:white',
-        'INPUT_GRAYSCALE_FONT': 'white',
-        'INPUT_RGB_COLOR': '#e74c3c:#3498db',
-        'INPUT_RGB_FONT': 'white',
-        'INPUT_LAYER_COLOR': 'black',
-        'INPUT_LAYER_FONT': 'white',
-        # HIDDEN LAYERS
-        'HIDDEN_DENSE_COLOR': '#3498db',
-        'HIDDEN_CONV_COLOR': '#5faad0',
-        'HIDDEN_CONV_FONT': 'black',
-        'HIDDEN_POOLING_COLOR': '#8e44ad',
-        'HIDDEN_POOLING_FONT': 'white',
-        'HIDDEN_FLATTEN_COLOR': '#2c3e50',
-        'HIDDEN_FLATTEN_FONT': 'white',
-        'HIDDEN_DROPOUT_COLOR': '#f39c12',
-        'HIDDEN_DROPOUT_FONT': 'black',
-        'HIDDEN_ACTIVATION_COLOR': '#00b894',
-        'HIDDEN_ACTIVATION_FONT': 'black',
-        'HIDDEN_LAYER_COLOR': 'black',
-        'HIDDEN_LAYER_FONT': 'white',
-        # OUTPUT LAYER
-        'OUTPUT_DENSE_COLOR': '#e74c3c',
-        'OUTPUT_LAYER_COLOR': 'black',
-        'OUTPUT_LAYER_FONT': 'white',
-    }
-
-    settings = {**main_settings, **settings} if settings is not None else {**main_settings}
-    max_neurons = settings['MAX_NEURONS']
-
-    input_layer = 0
-    hidden_layers_nr = 0
-    layer_types = []
-    hidden_layers = []
-    output_layer = 0
-
-    for num, layer in enumerate(model.layers, 1):
-        if num == 1:
-            input_layer = layer.input_shape[1] if type(layer.input_shape) == tuple else layer.input_shape[0][1]
-        if num == len(model.layers):
-            output_layer = layer.output_shape[1]
-        else:
-            hidden_layers_nr += 1
-            hidden_layers.append(layer.output_shape[1] if layer.__class__.__name__ == 'Dense' else 1)
-            layer_types.append(f'{layer.__class__.__name__}')
-
-        last_layer_nodes = input_layer
-        nodes_up = input_layer
-
-        if model.layers[0].__class__.__name__ != 'Dense':
-            last_layer_nodes = 1
-            nodes_up = 1
-            input_layer = 1
-
-        # VISUALIZE MODEL
-        graph = Digraph('Graph', filename=file_name)
-        n = 0
-        graph.graph_attr.update(
-            nodesep='1',  # X-SPACE
-            ranksep='2',  # Y-SPACE
-            splines='false'
-        )
-
-        # Input Layer
-        with graph.subgraph(name='cluster_input') as c:
-            # DENSE LAYER INPUT
-            layer = model.layers[0]
-            if layer.__class__.__name__ == 'Dense':
-                input_units = layer.input_shape[1]
-                label_dense_input = f'Input Units: {input_units}'
-                if max_neurons is not None and input_units > max_neurons:
-                    label_dense_input += f' (+{input_units - max_neurons} more)'
-                    input_layer = max_neurons
-                label_dense_input += f'\nActivation: {layer.get_config()["activation"]}'
-                c.attr(color='white')
-                for i in range(0, input_layer):
-                    n += 1
-                    c.node(str(n))
-                    c.attr(rank='same')
-                    c.node_attr.update(shape='circle', style='filled', color=settings['INPUT_DENSE_COLOR'], fontcolor=settings['INPUT_DENSE_COLOR'])
-                c.node(str(n + 1) * 3, label_dense_input, shape='rectangle', fontsize='18', color='white', fontcolor='black')
-            # EMBEDDING LAYER INPUT
-            elif layer.__class__.__name__ == 'Embedding':
-                input_dim = layer.input_dim
-                output_dim = layer.output_dim
-                n += 1
-                c.node(str(n), label=f'Embedding\nInput Dim: {input_dim}\nOutput Dim: {output_dim}', shape='square', style='filled', fillcolor=settings['INPUT_EMBEDDING_COLOR'], fontcolor=settings['INPUT_EMBEDDING_FONT'])
-            # CONV2D LAYER INPUT (IMAGE)
-            elif 'Conv' in layer.__class__.__name__:
-                pxls = layer.input_shape
-                clr = pxls[-1]
-                node_color = 'white'
-                node_font = 'black'
-                if clr == 1:
-                    clrmap = 'Grayscale'
-                    node_color = settings['INPUT_GRAYSCALE_COLOR']
-                    node_font = settings['INPUT_GRAYSCALE_FONT']
-                elif clr == 3:
-                    clrmap = 'RGB'
-                    node_color = settings['INPUT_RGB_COLOR']
-                    node_font = settings['INPUT_RGB_FONT']
-                else:
-                    clrmap = ''
-                n += 1
-                c.node(str(n), label=f'Image\n{pxls[-3]} x {pxls[-2]} pixels\n{clrmap}', shape='square', style='filled', fillcolor=node_color, fontcolor=node_font)
-            else:
-                # raise ValueError('[Keras Visualizer] Input Layer is not supported for visualizing')
-                c.attr(color='white')
-                n += 1
-                input_layer = layer.input_shape[1] if type(layer.input_shape) == tuple else layer.input_shape[0][1]
-                label_layer = f'{layer.__class__.__name__}\nshape= {input_layer}'
-                c.node(str(n), label=label_layer, shape='egg', style='filled', fillcolor=settings['INPUT_LAYER_COLOR'], fontcolor=settings['INPUT_LAYER_FONT'])
-
-        # Hidden Layers
-        for i in range(0, hidden_layers_nr):
-            with graph.subgraph(name='cluster_' + str(i + 1)) as c:
-                # Dense Layer
-                if layer_types[i] == 'Dense':
-                    c.attr(color='white')
-                    c.attr(rank='same')
-                    # If hidden_layers[i] > MAX_NEURONS, dont include all
-                    units = model.layers[i].output_shape[1]
-                    label_dense = f'Units: {units}'
-                    if max_neurons is not None and units > max_neurons:
-                        label_dense += f' (+{units - max_neurons} more)'
-                        hidden_layers[i] = max_neurons
-                    label_dense += f'\nActivation: {model.layers[i].get_config()["activation"]}'
-                    c.node(str(n) * 3, label_dense, shape='rectangle', fontsize='18', color='white', fontcolor='black')
-                    for j in range(0, hidden_layers[i]):
-                        n += 1
-                        c.node(str(n), shape='circle', style='filled', color=settings['HIDDEN_DENSE_COLOR'], fontcolor=settings['HIDDEN_DENSE_COLOR'])
-                        for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
-                            graph.edge(str(h), str(n))
-                    last_layer_nodes = hidden_layers[i]
-                    nodes_up += hidden_layers[i]
-                # Convolutional Layer
-                elif 'Conv' in layer_types[i]:
-                    c.attr(style='filled', color=settings['HIDDEN_CONV_COLOR'])
-                    n += 1
-                    activation = model.layers[0].get_config().get('activation')
-                    kernel_size = model.layers[i].get_config().get('kernel_size')
-                    filters = model.layers[i].get_config().get('filters', 0)
-                    label_conv = f'{layer_types[i]} Layer\nKernel Size: {kernel_size}\nFilters: {filters}\nActivation: {activation}'
-                    c.node('conv_' + str(n), label=label_conv, shape='square', fontcolor=settings['HIDDEN_CONV_FONT'])
-                    c.node(str(n), label=f'{filters}\nFeature Maps', shape='square', fontcolor=settings['HIDDEN_CONV_FONT'])
-                    graph.edge('conv_' + str(n), str(n))
-                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
-                        graph.edge(str(h), 'conv_' + str(n))
-                    last_layer_nodes = 1
-                    nodes_up += 1
-                # Pooling Layer
-                elif 'Pooling' in layer_types[i]:
-                    c.attr(color='white')
-                    n += 1
-                    pool_size = model.layers[i].get_config().get('pool_size', None)
-                    label_pooling = f'{layer_types[i]}' + (f'\nPool Size: {pool_size}' if pool_size is not None else '')
-                    c.node(str(n), label=label_pooling, shape='invtrapezium', style='filled', fillcolor=settings['HIDDEN_POOLING_COLOR'], fontcolor=settings['HIDDEN_POOLING_FONT'])
-                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
-                        graph.edge(str(h), str(n))
-                    last_layer_nodes = 1
-                    nodes_up += 1
-                # Flatten Layer
-                elif layer_types[i] == 'Flatten':
-                    n += 1
-                    c.attr(color='white')
-                    c.node(str(n), label='Flattening', shape='triangle', style='filled', fillcolor=settings['HIDDEN_FLATTEN_COLOR'], fontcolor=settings['HIDDEN_FLATTEN_FONT'])
-                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
-                        graph.edge(str(h), str(n))
-                    last_layer_nodes = 1
-                    nodes_up += 1
-                # Dropout Layer
-                elif 'Dropout' in layer_types[i]:
-                    n += 1
-                    c.attr(color='white')
-                    rate = model.layers[i].get_config().get('rate', None)
-                    label_dropout = f'{layer_types[i]}\nRate: {rate}'
-                    c.node(str(n), label=label_dropout, shape='Mcircle', style='filled', fillcolor=settings['HIDDEN_DROPOUT_COLOR'], fontcolor=settings['HIDDEN_DROPOUT_FONT'])
-                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
-                        graph.edge(str(h), str(n))
-                    last_layer_nodes = 1
-                    nodes_up += 1
-                # Activation Layer
-                elif layer_types[i] == 'Activation':
-                    n += 1
-                    c.attr(color='white')
-                    fnc = model.layers[i].get_config().get('activation')
-                    c.node(str(n), label=f'Activation Layer\nFunction: {fnc}', shape='octagon', style='filled', fillcolor=settings['HIDDEN_ACTIVATION_COLOR'], fontcolor=settings['HIDDEN_ACTIVATION_FONT'])
-                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
-                        graph.edge(str(h), str(n))
-                    last_layer_nodes = 1
-                    nodes_up += 1
-                # OTHER Layers
-                else:
-                    c.attr(color='white')
-                    n += 1
-                    label_layer = f'{layer_types[i]} Layer'
-                    c.node(str(n), label=label_layer, shape='egg', style='filled', fillcolor=settings['HIDDEN_LAYER_COLOR'], fontcolor=settings['HIDDEN_LAYER_FONT'])
-                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
-                        graph.edge(str(h), str(n))
-                    last_layer_nodes = 1
-                    nodes_up += 1
-
-        # Output Layer
-        with graph.subgraph(name='cluster_output') as c:
-            if model.layers[-1].__class__.__name__ == 'Dense':
-                output_units = model.layers[-1].output_shape[1]
-                label_dense_output = f'Output Units: {output_units}'
-                if max_neurons is not None and output_units > max_neurons:
-                    label_dense_output += f' (+{output_units - max_neurons} more)'
-                    output_layer = max_neurons
-                label_dense_output += f'\nActivation: {model.layers[-1].get_config()["activation"]}'
-                c.node(str(n) * 3, label_dense_output, shape='rectangle', fontsize='18', color='white', fontcolor='black')
-                c.attr(color='white')
-                c.attr(rank='same')
-                c.attr(labeljust='1')
-                for i in range(1, output_layer + 1):
-                    n += 1
-                    c.node(str(n), shape='circle', style='filled', color=settings['OUTPUT_DENSE_COLOR'], fontcolor=settings['OUTPUT_DENSE_COLOR'])
-                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
-                        graph.edge(str(h), str(n))
-                # c.node_attr.update(color='#2ecc71', style='filled', fontcolor='#2ecc71', shape='circle')
-            else:
-                # raise ValueError('[Keras Visualizer] Output layer is not supported for visualizing')
-                c.attr(color='white')
-                n += 1
-                output_layer = layer.output_shape[1] if type(layer.output_shape) == tuple else layer.output_shape[0][1]
-                label_layer = f'{layer.__class__.__name__}\nshape= {output_layer}'
-                c.node(str(n), label=label_layer, shape='egg', style='filled', fillcolor=settings['OUTPUT_LAYER_COLOR'], fontcolor=settings['OUTPUT_LAYER_FONT'])
-
-        graph.attr(arrowShape='none')
-        graph.edge_attr.update(arrowhead='none', color=settings['ARROW_COLOR'])
-
-    # SAVE GRAPH
-    try:
-        if file_format is not None:
-            graph.render(format=file_format, view=view)
-        else:
-            graph.save()
-    except Exception:
-        raise ValueError(f'[Keras Visualizer] Error while visualizing: {Exception}')
+def visualizer(model, file_name='graph', file_format=None, view=False, settings=None):
+    """Visualize a Sequential model.
+
+    # Arguments
+
+        model: a Keras model instance.
+
+        file_name: where to save the visualization.
+
+        file_format: file format to save 'pdf', 'png'.
+
+        view: open file after process if True.
+
+        settings: dictionary of valid configurations.
+
+    * change format to 'png' or 'pdf' to save visualization file
+    """
+    from graphviz import Digraph
+
+    main_settings = {
+        # ALL LAYERS
+        'MAX_NEURONS': 10,
+        'ARROW_COLOR': '#707070',
+        # INPUT LAYERS
+        'INPUT_DENSE_COLOR': '#2ecc71',
+        'INPUT_EMBEDDING_COLOR': 'black',
+        'INPUT_EMBEDDING_FONT': 'white',
+        'INPUT_GRAYSCALE_COLOR': 'black:white',
+        'INPUT_GRAYSCALE_FONT': 'white',
+        'INPUT_RGB_COLOR': '#e74c3c:#3498db',
+        'INPUT_RGB_FONT': 'white',
+        'INPUT_LAYER_COLOR': 'black',
+        'INPUT_LAYER_FONT': 'white',
+        # HIDDEN LAYERS
+        'HIDDEN_DENSE_COLOR': '#3498db',
+        'HIDDEN_CONV_COLOR': '#5faad0',
+        'HIDDEN_CONV_FONT': 'black',
+        'HIDDEN_POOLING_COLOR': '#8e44ad',
+        'HIDDEN_POOLING_FONT': 'white',
+        'HIDDEN_FLATTEN_COLOR': '#2c3e50',
+        'HIDDEN_FLATTEN_FONT': 'white',
+        'HIDDEN_DROPOUT_COLOR': '#f39c12',
+        'HIDDEN_DROPOUT_FONT': 'black',
+        'HIDDEN_ACTIVATION_COLOR': '#00b894',
+        'HIDDEN_ACTIVATION_FONT': 'black',
+        'HIDDEN_LAYER_COLOR': 'black',
+        'HIDDEN_LAYER_FONT': 'white',
+        # OUTPUT LAYER
+        'OUTPUT_DENSE_COLOR': '#e74c3c',
+        'OUTPUT_LAYER_COLOR': 'black',
+        'OUTPUT_LAYER_FONT': 'white',
+    }
+
+    settings = {**main_settings, **settings} if settings is not None else {**main_settings}
+    max_neurons = settings['MAX_NEURONS']
+
+    input_layer = 0
+    hidden_layers_nr = 0
+    layer_types = []
+    hidden_layers = []
+    output_layer = 0
+
+    for num, layer in enumerate(model.layers, 1):
+        if num == 1:
+            try:
+                inp_shp = layer.input_shape
+            except:
+                inp_shp = layer.input.shape
+            input_layer = inp_shp[1] if type(inp_shp) == tuple else inp_shp[0][1]
+        if num == len(model.layers):
+            try:
+                otp_shp = layer.output_shape
+            except:
+                otp_shp = layer.output.shape
+            output_layer = otp_shp[1]
+        else:
+            hidden_layers_nr += 1
+            try:
+                otp_shp = layer.output_shape
+            except:
+                otp_shp = layer.output.shape
+            hidden_layers.append(otp_shp[1] if layer.__class__.__name__ == 'Dense' else 1)
+            layer_types.append(f'{layer.__class__.__name__}')
+
+        last_layer_nodes = input_layer
+        nodes_up = input_layer
+
+        if model.layers[0].__class__.__name__ != 'Dense':
+            last_layer_nodes = 1
+            nodes_up = 1
+            input_layer = 1
+
+        # VISUALIZE MODEL
+        graph = Digraph('Graph', filename=file_name)
+        n = 0
+        graph.graph_attr.update(
+            nodesep='1',  # X-SPACE
+            ranksep='2',  # Y-SPACE
+            splines='false'
+        )
+
+        # Input Layer
+        with graph.subgraph(name='cluster_input') as c:
+            # DENSE LAYER INPUT
+            layer = model.layers[0]
+            if layer.__class__.__name__ == 'Dense':
+                try:
+                    inp_shp = layer.input_shape
+                except:
+                    inp_shp = layer.input.shape
+                input_units = inp_shp[1]
+                label_dense_input = f'Input Units: {input_units}'
+                if max_neurons is not None and input_units > max_neurons:
+                    label_dense_input += f' (+{input_units - max_neurons} more)'
+                    input_layer = max_neurons
+                label_dense_input += f'\nActivation: {layer.get_config()["activation"]}'
+                c.attr(color='white')
+                for i in range(0, input_layer):
+                    n += 1
+                    c.node(str(n))
+                    c.attr(rank='same')
+                    c.node_attr.update(shape='circle', style='filled', color=settings['INPUT_DENSE_COLOR'], fontcolor=settings['INPUT_DENSE_COLOR'])
+                c.node(str(n + 1) * 3, label_dense_input, shape='rectangle', fontsize='18', color='white', fontcolor='black')
+            # EMBEDDING LAYER INPUT
+            elif layer.__class__.__name__ == 'Embedding':
+                input_dim = layer.input_dim
+                output_dim = layer.output_dim
+                n += 1
+                c.node(str(n), label=f'Embedding\nInput Dim: {input_dim}\nOutput Dim: {output_dim}', shape='square', style='filled', fillcolor=settings['INPUT_EMBEDDING_COLOR'], fontcolor=settings['INPUT_EMBEDDING_FONT'])
+            # CONV2D LAYER INPUT (IMAGE)
+            elif 'Conv' in layer.__class__.__name__:
+                try:
+                    inp_shp = layer.input_shape
+                except:
+                    inp_shp = layer.input.shape
+                clr = inp_shp[-1]
+                node_color = 'white'
+                node_font = 'black'
+                if clr == 1:
+                    clrmap = 'Grayscale'
+                    node_color = settings['INPUT_GRAYSCALE_COLOR']
+                    node_font = settings['INPUT_GRAYSCALE_FONT']
+                elif clr == 3:
+                    clrmap = 'RGB'
+                    node_color = settings['INPUT_RGB_COLOR']
+                    node_font = settings['INPUT_RGB_FONT']
+                else:
+                    clrmap = ''
+                n += 1
+                c.node(str(n), label=f'Image\n{inp_shp[-3]} x {inp_shp[-2]} pixels\n{clrmap}', shape='square', style='filled', fillcolor=node_color, fontcolor=node_font)
+            else:
+                # raise ValueError('[Keras Visualizer] Input Layer is not supported for visualizing')
+                c.attr(color='white')
+                n += 1
+                input_layer = inp_shp[1] if type(inp_shp) == tuple else inp_shp[0][1]
+                label_layer = f'{layer.__class__.__name__}\nshape= {input_layer}'
+                c.node(str(n), label=label_layer, shape='egg', style='filled', fillcolor=settings['INPUT_LAYER_COLOR'], fontcolor=settings['INPUT_LAYER_FONT'])
+
+        # Hidden Layers
+        for i in range(0, hidden_layers_nr):
+            with graph.subgraph(name='cluster_' + str(i + 1)) as c:
+                # Dense Layer
+                if layer_types[i] == 'Dense':
+                    c.attr(color='white')
+                    c.attr(rank='same')
+                    # If hidden_layers[i] > MAX_NEURONS, dont include all
+                    try:
+                        units = model.layers[i].output_shape[1]
+                    except:
+                        units = model.layers[i].output.shape[1]
+                    label_dense = f'Units: {units}'
+                    if max_neurons is not None and units > max_neurons:
+                        label_dense += f' (+{units - max_neurons} more)'
+                        hidden_layers[i] = max_neurons
+                    label_dense += f'\nActivation: {model.layers[i].get_config()["activation"]}'
+                    c.node(str(n) * 3, label_dense, shape='rectangle', fontsize='18', color='white', fontcolor='black')
+                    for j in range(0, hidden_layers[i]):
+                        n += 1
+                        c.node(str(n), shape='circle', style='filled', color=settings['HIDDEN_DENSE_COLOR'], fontcolor=settings['HIDDEN_DENSE_COLOR'])
+                        for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
+                            graph.edge(str(h), str(n))
+                    last_layer_nodes = hidden_layers[i]
+                    nodes_up += hidden_layers[i]
+                # Convolutional Layer
+                elif 'Conv' in layer_types[i]:
+                    c.attr(style='filled', color=settings['HIDDEN_CONV_COLOR'])
+                    n += 1
+                    activation = model.layers[0].get_config().get('activation')
+                    kernel_size = model.layers[i].get_config().get('kernel_size')
+                    filters = model.layers[i].get_config().get('filters', 0)
+                    label_conv = f'{layer_types[i]} Layer\nKernel Size: {kernel_size}\nFilters: {filters}\nActivation: {activation}'
+                    c.node('conv_' + str(n), label=label_conv, shape='square', fontcolor=settings['HIDDEN_CONV_FONT'])
+                    c.node(str(n), label=f'{filters}\nFeature Maps', shape='square', fontcolor=settings['HIDDEN_CONV_FONT'])
+                    graph.edge('conv_' + str(n), str(n))
+                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
+                        graph.edge(str(h), 'conv_' + str(n))
+                    last_layer_nodes = 1
+                    nodes_up += 1
+                # Pooling Layer
+                elif 'Pooling' in layer_types[i]:
+                    c.attr(color='white')
+                    n += 1
+                    pool_size = model.layers[i].get_config().get('pool_size', None)
+                    label_pooling = f'{layer_types[i]}' + (f'\nPool Size: {pool_size}' if pool_size is not None else '')
+                    c.node(str(n), label=label_pooling, shape='invtrapezium', style='filled', fillcolor=settings['HIDDEN_POOLING_COLOR'], fontcolor=settings['HIDDEN_POOLING_FONT'])
+                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
+                        graph.edge(str(h), str(n))
+                    last_layer_nodes = 1
+                    nodes_up += 1
+                # Flatten Layer
+                elif layer_types[i] == 'Flatten':
+                    n += 1
+                    c.attr(color='white')
+                    c.node(str(n), label='Flattening', shape='triangle', style='filled', fillcolor=settings['HIDDEN_FLATTEN_COLOR'], fontcolor=settings['HIDDEN_FLATTEN_FONT'])
+                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
+                        graph.edge(str(h), str(n))
+                    last_layer_nodes = 1
+                    nodes_up += 1
+                # Dropout Layer
+                elif 'Dropout' in layer_types[i]:
+                    n += 1
+                    c.attr(color='white')
+                    rate = model.layers[i].get_config().get('rate', None)
+                    label_dropout = f'{layer_types[i]}\nRate: {rate}'
+                    c.node(str(n), label=label_dropout, shape='Mcircle', style='filled', fillcolor=settings['HIDDEN_DROPOUT_COLOR'], fontcolor=settings['HIDDEN_DROPOUT_FONT'])
+                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
+                        graph.edge(str(h), str(n))
+                    last_layer_nodes = 1
+                    nodes_up += 1
+                # Activation Layer
+                elif layer_types[i] == 'Activation':
+                    n += 1
+                    c.attr(color='white')
+                    fnc = model.layers[i].get_config().get('activation')
+                    c.node(str(n), label=f'Activation Layer\nFunction: {fnc}', shape='octagon', style='filled', fillcolor=settings['HIDDEN_ACTIVATION_COLOR'], fontcolor=settings['HIDDEN_ACTIVATION_FONT'])
+                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
+                        graph.edge(str(h), str(n))
+                    last_layer_nodes = 1
+                    nodes_up += 1
+                # OTHER Layers
+                else:
+                    c.attr(color='white')
+                    n += 1
+                    label_layer = f'{layer_types[i]} Layer'
+                    c.node(str(n), label=label_layer, shape='egg', style='filled', fillcolor=settings['HIDDEN_LAYER_COLOR'], fontcolor=settings['HIDDEN_LAYER_FONT'])
+                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
+                        graph.edge(str(h), str(n))
+                    last_layer_nodes = 1
+                    nodes_up += 1
+
+        # Output Layer
+        with graph.subgraph(name='cluster_output') as c:
+            if model.layers[-1].__class__.__name__ == 'Dense':
+                try:
+                    output_units = model.layers[-1].output_shape[1]
+                except:
+                    output_units = model.layers[-1].output.shape[1]
+                label_dense_output = f'Output Units: {output_units}'
+                if max_neurons is not None and output_units > max_neurons:
+                    label_dense_output += f' (+{output_units - max_neurons} more)'
+                    output_layer = max_neurons
+                label_dense_output += f'\nActivation: {model.layers[-1].get_config()["activation"]}'
+                c.node(str(n) * 3, label_dense_output, shape='rectangle', fontsize='18', color='white', fontcolor='black')
+                c.attr(color='white')
+                c.attr(rank='same')
+                c.attr(labeljust='1')
+                for i in range(1, output_layer + 1):
+                    n += 1
+                    c.node(str(n), shape='circle', style='filled', color=settings['OUTPUT_DENSE_COLOR'], fontcolor=settings['OUTPUT_DENSE_COLOR'])
+                    for h in range(nodes_up - last_layer_nodes + 1, nodes_up + 1):
+                        graph.edge(str(h), str(n))
+                # c.node_attr.update(color='#2ecc71', style='filled', fontcolor='#2ecc71', shape='circle')
+            else:
+                # raise ValueError('[Keras Visualizer] Output layer is not supported for visualizing')
+                c.attr(color='white')
+                n += 1
+                try:
+                    otp_shp = layer.output_shape
+                except:
+                    otp_shp = layer.output.shape
+                output_layer = otp_shp[1] if type(otp_shp) == tuple else otp_shp[0][1]
+                label_layer = f'{layer.__class__.__name__}\nshape= {output_layer}'
+                c.node(str(n), label=label_layer, shape='egg', style='filled', fillcolor=settings['OUTPUT_LAYER_COLOR'], fontcolor=settings['OUTPUT_LAYER_FONT'])
+
+        graph.attr(arrowShape='none')
+        graph.edge_attr.update(arrowhead='none', color=settings['ARROW_COLOR'])
+
+    # SAVE GRAPH
+    try:
+        if file_format is not None:
+            graph.render(format=file_format, view=view)
+        else:
+            graph.save()
+    except Exception:
+        raise ValueError(f'[Keras Visualizer] Error while visualizing: {Exception}')
```

### Comparing `keras-visualizer-3.1.2/keras_visualizer.egg-info/PKG-INFO` & `keras_visualizer-3.2.0/keras_visualizer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,276 +1,277 @@
-Metadata-Version: 2.1
-Name: keras-visualizer
-Version: 3.1.2
-Summary: A Keras Model Visualizer
-Home-page: https://github.com/lordmahyar/keras-visualizer
-Author: Mahyar Amiri
-Author-email: mmaahhyyaarr@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Keras Visualizer
-
-![LOGO](logo.png)
-
-[![PyPI](https://img.shields.io/pypi/v/keras-visualizer?label=PyPI&logo=pypi&logoColor=FFE873)](https://pypi.org/project/keras-visualizer)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-visualizer?label=Downloads&color=blue)](https://pypistats.org/packages/keras-visualizer)
-[![GitHub - License](https://img.shields.io/github/license/mahyar-amiri/django-comment-system?label=License&color=blue)](LICENSE)
-[![Virgool.io](https://img.shields.io/static/v1?label=Virgool.io&message=keras-visualizer&color=blue)](https://vrgl.ir/5KSoN)
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahyar-amiri/keras-visualizer/)
-
-A Python Library for Visualizing Keras Models.
-
-## Table of Contents
-
-<!-- TOC -->
-
-* [Keras Visualizer](#keras-visualizer)
-    * [Table of Contents](#table-of-contents)
-    * [Installation](#installation)
-        * [Install](#install)
-        * [Upgrade](#upgrade)
-    * [Usage](#usage)
-    * [Parameters](#parameters)
-    * [Settings](#settings)
-    * [Examples](#examples)
-        * [Example 1](#example-1)
-        * [Example 2](#example-2)
-        * [Example 3](#example-3)
-    * [Supported layers](#supported-layers)
-
-<!-- TOC -->
-
-## Installation
-
-### Install
-
-Use python package manager (pip) to install Keras Visualizer.
-
-```bash
-pip install keras-visualizer
-```
-
-### Upgrade
-
-Use python package manager (pip) to upgrade Keras Visualizer.
-
-```bash
-pip install keras-visualizer --upgrade
-```
-
-## Usage
-
-```python
-from keras_visualizer import visualizer
-
-# create your model here
-# model = ...
-
-visualizer(model, file_format='png')
-```
-
-## Parameters
-
-```python
-visualizer(model, file_name='graph', file_format=None, view=False, settings=None)
-```
-
-- `model` : a Keras model instance.
-- `file_name` : where to save the visualization.
-- `file_format` : file format to save 'pdf', 'png'.
-- `view` : open file after process if True.
-- `settings` : a dictionary of available settings.
-
-> **Note :**
-> - set `file_format='png'` or `file_format='pdf'` to save visualization file.
-> - use `view=True` to open visualization file.
-> - use [settings](#settings) to customize output image.
-
-## Settings
-
-you can customize settings for your output image. here is the default settings dictionary:
-
-```python
-settings = {
-    # ALL LAYERS
-    'MAX_NEURONS': 10,
-    'ARROW_COLOR': '#707070',
-    # INPUT LAYERS
-    'INPUT_DENSE_COLOR': '#2ecc71',
-    'INPUT_EMBEDDING_COLOR': 'black',
-    'INPUT_EMBEDDING_FONT': 'white',
-    'INPUT_GRAYSCALE_COLOR': 'black:white',
-    'INPUT_GRAYSCALE_FONT': 'white',
-    'INPUT_RGB_COLOR': '#e74c3c:#3498db',
-    'INPUT_RGB_FONT': 'white',
-    'INPUT_LAYER_COLOR': 'black',
-    'INPUT_LAYER_FONT': 'white',
-    # HIDDEN LAYERS
-    'HIDDEN_DENSE_COLOR': '#3498db',
-    'HIDDEN_CONV_COLOR': '#5faad0',
-    'HIDDEN_CONV_FONT': 'black',
-    'HIDDEN_POOLING_COLOR': '#8e44ad',
-    'HIDDEN_POOLING_FONT': 'white',
-    'HIDDEN_FLATTEN_COLOR': '#2c3e50',
-    'HIDDEN_FLATTEN_FONT': 'white',
-    'HIDDEN_DROPOUT_COLOR': '#f39c12',
-    'HIDDEN_DROPOUT_FONT': 'black',
-    'HIDDEN_ACTIVATION_COLOR': '#00b894',
-    'HIDDEN_ACTIVATION_FONT': 'black',
-    'HIDDEN_LAYER_COLOR': 'black',
-    'HIDDEN_LAYER_FONT': 'white',
-    # OUTPUT LAYER
-    'OUTPUT_DENSE_COLOR': '#e74c3c',
-    'OUTPUT_LAYER_COLOR': 'black',
-    'OUTPUT_LAYER_FONT': 'white',
-}
-```
-
-**Note**:
-
-* set `'MAX_NEURONS': None` to disable max neurons constraint.
-* see list of color names [here](https://graphviz.org/doc/info/colors.html).
-
-```python
-from keras_visualizer import visualizer
-
-my_settings = {
-    'MAX_NEURONS': None,
-    'INPUT_DENSE_COLOR': 'teal',
-    'HIDDEN_DENSE_COLOR': 'gray',
-    'OUTPUT_DENSE_COLOR': 'crimson'
-}
-
-# model = ...
-
-visualizer(model, file_format='png', settings=my_settings)
-```
-
-## Examples
-
-you can use simple examples as `.py` or `.ipynb` format in [examples directory](examples).
-
-### Example 1
-
-```python
-from keras import models, layers
-from keras_visualizer import visualizer
-
-model = models.Sequential([
-    layers.Dense(64, activation='relu', input_shape=(8,)),
-    layers.Dense(6, activation='softmax'),
-    layers.Dense(32),
-    layers.Dense(9, activation='sigmoid')
-])
-
-visualizer(model, file_format='png', view=True)
-```
-
-![example 1](examples/example1_output.png)
-
----
-
-### Example 2
-
-```python
-from keras import models, layers
-from keras_visualizer import visualizer
-
-model = models.Sequential()
-model.add(layers.Conv2D(64, (3, 3), input_shape=(28, 28, 3), activation='relu'))
-model.add(layers.MaxPooling2D((2, 2)))
-model.add(layers.Flatten())
-model.add(layers.Dense(3))
-model.add(layers.Dropout(0.5))
-model.add(layers.Activation('sigmoid'))
-model.add(layers.Dense(1))
-
-visualizer(model, file_format='png', view=True)
-```
-
-![example 2](examples/example2_output.png)
-
----
-
-### Example 3
-
-```python
-from keras import models, layers
-from keras_visualizer import visualizer
-
-model = models.Sequential()
-model.add(layers.Embedding(64, output_dim=256))
-model.add(layers.LSTM(128))
-model.add(layers.Dense(1, activation='sigmoid'))
-
-visualizer(model, file_format='png', view=True)
-```
-
-![example 3](examples/example3_output.png)
-
-## Supported layers
-
-[Explore list of **keras layers**](https://keras.io/api/layers/)
-
-1. Core layers
-    - [x] Input object
-    - [x] Dense layer
-    - [x] Activation layer
-    - [ ] Embedding layer
-    - [ ] Masking layer
-    - [ ] Lambda layer
-
-2. Convolution layers
-    - [x] Conv1D layer
-    - [x] Conv2D layer
-    - [x] Conv3D layer
-    - [x] SeparableConv1D layer
-    - [x] SeparableConv2D layer
-    - [x] DepthwiseConv2D layer
-    - [x] Conv1DTranspose layer
-    - [x] Conv2DTranspose layer
-    - [x] Conv3DTranspose layer
-
-3. Pooling layers
-    - [x] MaxPooling1D layer
-    - [x] MaxPooling2D layer
-    - [x] MaxPooling3D layer
-    - [x] AveragePooling1D layer
-    - [x] AveragePooling2D layer
-    - [x] AveragePooling3D layer
-    - [x] GlobalMaxPooling1D layer
-    - [x] GlobalMaxPooling2D layer
-    - [x] GlobalMaxPooling3D layer
-    - [x] GlobalAveragePooling1D layer
-    - [x] GlobalAveragePooling2D layer
-    - [x] GlobalAveragePooling3D layer
-
-4. Reshaping layers
-    - [ ] Reshape layer
-    - [x] Flatten layer
-    - [ ] RepeatVector layer
-    - [ ] Permute layer
-    - [ ] Cropping1D layer
-    - [ ] Cropping2D layer
-    - [ ] Cropping3D layer
-    - [ ] UpSampling1D layer
-    - [ ] UpSampling2D layer
-    - [ ] UpSampling3D layer
-    - [ ] ZeroPadding1D layer
-    - [ ] ZeroPadding2D layer
-    - [ ] ZeroPadding3D layer
-
-5. Regularization layers
-    - [x] Dropout layer
-    - [x] SpatialDropout1D layer
-    - [x] SpatialDropout2D layer
-    - [x] SpatialDropout3D layer
-    - [x] GaussianDropout layer
-    - [ ] GaussianNoise layer
-    - [ ] ActivityRegularization layer
-    - [x] AlphaDropout layer
+Metadata-Version: 2.1
+Name: keras-visualizer
+Version: 3.2.0
+Summary: A Keras Model Visualizer
+Home-page: https://github.com/lordmahyar/keras-visualizer
+Author: Mahyar Amiri
+Author-email: mmaahhyyaarr@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: graphviz
+
+# Keras Visualizer
+
+![LOGO](logo.png)
+
+[![PyPI](https://img.shields.io/pypi/v/keras-visualizer?label=PyPI&logo=pypi&logoColor=FFE873)](https://pypi.org/project/keras-visualizer)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/keras-visualizer?label=Downloads&color=blue)](https://pypistats.org/packages/keras-visualizer)
+[![GitHub - License](https://img.shields.io/github/license/mahyar-amiri/django-comment-system?label=License&color=blue)](LICENSE)
+[![Virgool.io](https://img.shields.io/static/v1?label=Virgool.io&message=keras-visualizer&color=blue)](https://vrgl.ir/5KSoN)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahyar-amiri/keras-visualizer/)
+
+A Python Library for Visualizing Keras Models.
+
+## Table of Contents
+
+<!-- TOC -->
+
+* [Keras Visualizer](#keras-visualizer)
+    * [Table of Contents](#table-of-contents)
+    * [Installation](#installation)
+        * [Install](#install)
+        * [Upgrade](#upgrade)
+    * [Usage](#usage)
+    * [Parameters](#parameters)
+    * [Settings](#settings)
+    * [Examples](#examples)
+        * [Example 1](#example-1)
+        * [Example 2](#example-2)
+        * [Example 3](#example-3)
+    * [Supported layers](#supported-layers)
+
+<!-- TOC -->
+
+## Installation
+
+### Install
+
+Use python package manager (pip) to install Keras Visualizer.
+
+```bash
+pip install keras-visualizer
+```
+
+### Upgrade
+
+Use python package manager (pip) to upgrade Keras Visualizer.
+
+```bash
+pip install keras-visualizer --upgrade
+```
+
+## Usage
+
+```python
+from keras_visualizer import visualizer
+
+# create your model here
+# model = ...
+
+visualizer(model, file_format='png')
+```
+
+## Parameters
+
+```python
+visualizer(model, file_name='graph', file_format=None, view=False, settings=None)
+```
+
+- `model` : a Keras model instance.
+- `file_name` : where to save the visualization.
+- `file_format` : file format to save 'pdf', 'png'.
+- `view` : open file after process if True.
+- `settings` : a dictionary of available settings.
+
+> **Note :**
+> - set `file_format='png'` or `file_format='pdf'` to save visualization file.
+> - use `view=True` to open visualization file.
+> - use [settings](#settings) to customize output image.
+
+## Settings
+
+you can customize settings for your output image. here is the default settings dictionary:
+
+```python
+settings = {
+    # ALL LAYERS
+    'MAX_NEURONS': 10,
+    'ARROW_COLOR': '#707070',
+    # INPUT LAYERS
+    'INPUT_DENSE_COLOR': '#2ecc71',
+    'INPUT_EMBEDDING_COLOR': 'black',
+    'INPUT_EMBEDDING_FONT': 'white',
+    'INPUT_GRAYSCALE_COLOR': 'black:white',
+    'INPUT_GRAYSCALE_FONT': 'white',
+    'INPUT_RGB_COLOR': '#e74c3c:#3498db',
+    'INPUT_RGB_FONT': 'white',
+    'INPUT_LAYER_COLOR': 'black',
+    'INPUT_LAYER_FONT': 'white',
+    # HIDDEN LAYERS
+    'HIDDEN_DENSE_COLOR': '#3498db',
+    'HIDDEN_CONV_COLOR': '#5faad0',
+    'HIDDEN_CONV_FONT': 'black',
+    'HIDDEN_POOLING_COLOR': '#8e44ad',
+    'HIDDEN_POOLING_FONT': 'white',
+    'HIDDEN_FLATTEN_COLOR': '#2c3e50',
+    'HIDDEN_FLATTEN_FONT': 'white',
+    'HIDDEN_DROPOUT_COLOR': '#f39c12',
+    'HIDDEN_DROPOUT_FONT': 'black',
+    'HIDDEN_ACTIVATION_COLOR': '#00b894',
+    'HIDDEN_ACTIVATION_FONT': 'black',
+    'HIDDEN_LAYER_COLOR': 'black',
+    'HIDDEN_LAYER_FONT': 'white',
+    # OUTPUT LAYER
+    'OUTPUT_DENSE_COLOR': '#e74c3c',
+    'OUTPUT_LAYER_COLOR': 'black',
+    'OUTPUT_LAYER_FONT': 'white',
+}
+```
+
+**Note**:
+
+* set `'MAX_NEURONS': None` to disable max neurons constraint.
+* see list of color names [here](https://graphviz.org/doc/info/colors.html).
+
+```python
+from keras_visualizer import visualizer
+
+my_settings = {
+    'MAX_NEURONS': None,
+    'INPUT_DENSE_COLOR': 'teal',
+    'HIDDEN_DENSE_COLOR': 'gray',
+    'OUTPUT_DENSE_COLOR': 'crimson'
+}
+
+# model = ...
+
+visualizer(model, file_format='png', settings=my_settings)
+```
+
+## Examples
+
+you can use simple examples as `.py` or `.ipynb` format in [examples directory](examples).
+
+### Example 1
+
+```python
+from keras import models, layers
+from keras_visualizer import visualizer
+
+model = models.Sequential([
+    layers.Dense(64, activation='relu', input_shape=(8,)),
+    layers.Dense(6, activation='softmax'),
+    layers.Dense(32),
+    layers.Dense(9, activation='sigmoid')
+])
+
+visualizer(model, file_format='png', view=True)
+```
+
+![example 1](examples/example1_output.png)
+
+---
+
+### Example 2
+
+```python
+from keras import models, layers
+from keras_visualizer import visualizer
+
+model = models.Sequential()
+model.add(layers.Conv2D(64, (3, 3), input_shape=(28, 28, 3), activation='relu'))
+model.add(layers.MaxPooling2D((2, 2)))
+model.add(layers.Flatten())
+model.add(layers.Dense(3))
+model.add(layers.Dropout(0.5))
+model.add(layers.Activation('sigmoid'))
+model.add(layers.Dense(1))
+
+visualizer(model, file_format='png', view=True)
+```
+
+![example 2](examples/example2_output.png)
+
+---
+
+### Example 3
+
+```python
+from keras import models, layers
+from keras_visualizer import visualizer
+
+model = models.Sequential()
+model.add(layers.Embedding(64, output_dim=256))
+model.add(layers.LSTM(128))
+model.add(layers.Dense(1, activation='sigmoid'))
+
+visualizer(model, file_format='png', view=True)
+```
+
+![example 3](examples/example3_output.png)
+
+## Supported layers
+
+[Explore list of **keras layers**](https://keras.io/api/layers/)
+
+1. Core layers
+    - [x] Input object
+    - [x] Dense layer
+    - [x] Activation layer
+    - [ ] Embedding layer
+    - [ ] Masking layer
+    - [ ] Lambda layer
+
+2. Convolution layers
+    - [x] Conv1D layer
+    - [x] Conv2D layer
+    - [x] Conv3D layer
+    - [x] SeparableConv1D layer
+    - [x] SeparableConv2D layer
+    - [x] DepthwiseConv2D layer
+    - [x] Conv1DTranspose layer
+    - [x] Conv2DTranspose layer
+    - [x] Conv3DTranspose layer
+
+3. Pooling layers
+    - [x] MaxPooling1D layer
+    - [x] MaxPooling2D layer
+    - [x] MaxPooling3D layer
+    - [x] AveragePooling1D layer
+    - [x] AveragePooling2D layer
+    - [x] AveragePooling3D layer
+    - [x] GlobalMaxPooling1D layer
+    - [x] GlobalMaxPooling2D layer
+    - [x] GlobalMaxPooling3D layer
+    - [x] GlobalAveragePooling1D layer
+    - [x] GlobalAveragePooling2D layer
+    - [x] GlobalAveragePooling3D layer
+
+4. Reshaping layers
+    - [ ] Reshape layer
+    - [x] Flatten layer
+    - [ ] RepeatVector layer
+    - [ ] Permute layer
+    - [ ] Cropping1D layer
+    - [ ] Cropping2D layer
+    - [ ] Cropping3D layer
+    - [ ] UpSampling1D layer
+    - [ ] UpSampling2D layer
+    - [ ] UpSampling3D layer
+    - [ ] ZeroPadding1D layer
+    - [ ] ZeroPadding2D layer
+    - [ ] ZeroPadding3D layer
+
+5. Regularization layers
+    - [x] Dropout layer
+    - [x] SpatialDropout1D layer
+    - [x] SpatialDropout2D layer
+    - [x] SpatialDropout3D layer
+    - [x] GaussianDropout layer
+    - [ ] GaussianNoise layer
+    - [ ] ActivityRegularization layer
+    - [x] AlphaDropout layer
```

### Comparing `keras-visualizer-3.1.2/setup.py` & `keras_visualizer-3.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import setuptools
-
-VERSION = '3.1.2'
-
-with open('README.md', 'r') as f:
-    long_description = f.read()
-
-setuptools.setup(
-    name='keras-visualizer',
-    version=VERSION,
-    license='MIT',
-    author='Mahyar Amiri',
-    author_email='mmaahhyyaarr@gmail.com',
-    description='A Keras Model Visualizer',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/lordmahyar/keras-visualizer',
-    packages=setuptools.find_packages(),
-    install_requires=['graphviz'],
-    classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-    ],
-    python_requires='>=3.6',
-)
+import setuptools
+
+VERSION = '3.2.0'
+
+with open('README.md', 'r') as f:
+    long_description = f.read()
+
+setuptools.setup(
+    name='keras-visualizer',
+    version=VERSION,
+    license='MIT',
+    author='Mahyar Amiri',
+    author_email='mmaahhyyaarr@gmail.com',
+    description='A Keras Model Visualizer',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/lordmahyar/keras-visualizer',
+    packages=setuptools.find_packages(),
+    install_requires=['graphviz'],
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+    python_requires='>=3.6',
+)
```


# Comparing `tmp/data_transformation_wizzard-0.1.0.tar.gz` & `tmp/data_transformation_wizzard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_wizzard-0.1.0.tar", max compression
+gzip compressed data, was "data_transformation_wizzard-0.1.1.tar", max compression
```

## Comparing `data_transformation_wizzard-0.1.0.tar` & `data_transformation_wizzard-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      444 2024-04-27 17:34:46.653476 data_transformation_wizzard-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1890 2024-04-27 17:36:21.514779 data_transformation_wizzard-0.1.0/README.md
--rw-r--r--   0        0        0      125 2024-04-27 10:42:27.871672 data_transformation_wizzard-0.1.0/src/data_transformation_wizzard/__init__.py
--rw-r--r--   0        0        0     2771 2024-04-25 09:45:04.983556 data_transformation_wizzard-0.1.0/src/data_transformation_wizzard/cross_correlation.py
--rw-r--r--   0        0        0     3013 2024-04-25 09:45:05.144938 data_transformation_wizzard-0.1.0/src/data_transformation_wizzard/time_series_windowing.py
--rw-r--r--   0        0        0     1717 2024-04-25 09:45:05.327534 data_transformation_wizzard-0.1.0/src/data_transformation_wizzard/transpose.py
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 data_transformation_wizzard-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      444 2024-05-08 22:39:58.172227 data_transformation_wizzard-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1941 2024-05-07 11:08:41.881080 data_transformation_wizzard-0.1.1/README.md
+-rw-r--r--   0        0        0      127 2024-05-07 11:08:41.884358 data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/__init__.py
+-rw-r--r--   0        0        0     2785 2024-05-08 22:19:41.742323 data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/cross_correlation.py
+-rw-r--r--   0        0        0     2269 2024-05-08 22:19:41.726657 data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/time_series_windowing.py
+-rw-r--r--   0        0        0     1294 2024-05-08 22:19:41.742323 data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/transpose.py
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 data_transformation_wizzard-0.1.1/PKG-INFO
```

### Comparing `data_transformation_wizzard-0.1.0/README.md` & `data_transformation_wizzard-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: data_transformation_wizzard
+Version: 0.1.1
+Summary: Transpose.Windowing.Convolution
+License: Edgaras Gacionis
+Author: Edgaras Gacionis
+Requires-Python: ==3.11.5
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Description-Content-Type: text/markdown
+
 
 # Data Wizzard Library
 
 ## Overview
 The Data Wizzard Library is a Python package designed to simplify and streamline data transformation tasks. It provides a set of functions that perform common operations such as 2D transposition, 1D windowing, and 2D convolution. These functions are optimized for performance and ease of use, making it easier to manipulate and analyze data in Python.
 
 ## Features
@@ -45,7 +57,8 @@
 ```python
 from data_transformation_wizzard import convolution2d
 input_matrix = [[0, 1, 2], [3, 4, 5], [6, 7, 8]]
 kernel = [[0, 1], [2, 3]]
 stride = 1
 print(convolution2d(input_matrix, kernel, stride))
 ```
+
```

### Comparing `data_transformation_wizzard-0.1.0/src/data_transformation_wizzard/cross_correlation.py` & `data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/cross_correlation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import numpy as np
 
-import numpy as np
-
 
 def convolution2d(
     input_matrix: list | np.ndarray, kernel: list | np.ndarray, stride: int = 1
 ) -> np.ndarray:
     """
     Apply 2D convolution to an input matrix with a given kernel and stride.
 
@@ -15,15 +13,15 @@
     stride (int, optional): The stride, an integer that is greater than 0. Default is 1.
 
     Returns:
     np.ndarray: The output matrix, a 2D Numpy array.
 
     Raises:
     TypeError: If input_matrix or kernel is not a list or numpy array.
-    ValueError: If input_matrix or kernel does not contain only integers or floats, or if stride is not a positive integer.
+    ValueError: If input_matrix or kernel does not contain only integers or floats, or if stride is not a positive int.
 
     Example:
     >>> input_matrix = np.array([[0, 1, 2], [3, 4, 5], [6, 7, 8]])
     >>> kernel = np.array([[0, 1], [2, 3]])
     >>> stride = 1
     >>> convolution2d(input_matrix, kernel, stride)
     array([[19., 25.],
@@ -38,15 +36,17 @@
         for sublist in input_matrix
         for i in sublist
     ):
         raise ValueError("input_matrix must contain only numbers")
     if not isinstance(kernel, (list, np.ndarray)):
         raise TypeError("kernel must be a list or numpy array")
     if not all(
-        isinstance(i, (int, float, np.number)) for sublist in kernel for i in sublist
+        isinstance(i, (int, float, np.number))
+        for sublist in kernel
+        for i in sublist
     ):
         raise ValueError("kernel must contain only numbers")
     if not isinstance(stride, int) or stride < 1:
         raise ValueError("stride must be a positive integer")
 
     # Convert input_matrix and kernel to numpy arrays if they're not
     if not isinstance(input_matrix, np.ndarray):
@@ -66,13 +66,14 @@
     output_matrix = np.zeros((x_out, y_out))
 
     # Apply convolution
     for i in range(0, x_out):
         for j in range(0, y_out):
             output_matrix[i, j] = np.sum(
                 input_matrix[
-                    i * stride : i * stride + x_kern, j * stride : j * stride + y_kern
+                    i * stride : i * stride + x_kern,
+                    j * stride : j * stride + y_kern,
                 ]
                 * kernel
             )
 
     return output_matrix
```

### Comparing `data_transformation_wizzard-0.1.0/src/data_transformation_wizzard/time_series_windowing.py` & `data_transformation_wizzard-0.1.1/src/data_transformation_wizzard/time_series_windowing.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,36 +39,13 @@
     # Convert input_array to numpy array if it's not
     input_array = np.array(input_array, dtype=float)
 
     # Initialize the output list
     output = []
 
     # Iterate over the input_array with a step size of shift
-    for i in range(0, len(input_array) - size * stride + 1, shift):
+    for i in range(0, len(input_array) - size + 1, shift):
         window = input_array[i : i + size : stride]
         output.append(window)
 
     # Return the output list
     return output
-
-
-# Test the function
-if __name__ == "__main__":
-    try:
-        length = int(input("Enter the length of the array: "))
-        size = int(input("Enter the window size: "))
-        shift = int(input("Enter the window shift size: "))
-        stride = int(input("Enter the window stride size: "))
-
-        array = []
-        for i in range(length):
-            array.append(float(input(f"Enter element at position {i + 1}: ")))
-
-        print("Original Array:")
-        print(array)
-
-        print("\nWindowed Array:")
-        windowed_array = window1d(array, size, shift, stride)
-        for window in windowed_array:
-            print(window)
-    except Exception as e:
-        print(f"An error occurred: {e}")
```

### Comparing `data_transformation_wizzard-0.1.0/PKG-INFO` & `data_transformation_wizzard-0.1.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,51 @@
-Metadata-Version: 2.1
-Name: data_transformation_wizzard
-Version: 0.1.0
-Summary: Transpose.Windowing.Convolution
-License: Edgaras Gacionis
-Author: Edgaras Gacionis
-Requires-Python: ==3.11.5
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Description-Content-Type: text/markdown
-
-
-# Data Wizzard Library
-
-## Overview
-The Data Wizzard Library is a Python package designed to simplify and streamline data transformation tasks. It provides a set of functions that perform common operations such as 2D transposition, 1D windowing, and 2D convolution. These functions are optimized for performance and ease of use, making it easier to manipulate and analyze data in Python.
-
-## Features
-
-### transpose2d
-This function transposes a 2D matrix, effectively flipping it over its diagonal, switching the matrix's row and column indices. This is particularly useful in numerical and matrix computations.
-
-### window1d
-The `window1d` function applies windowing operations to 1-dimensional arrays. This is useful in signal processing where segmenting data into overlapping or non-overlapping windows is required.
-
-### convolution2d
-Performs 2D convolution on an input matrix with a specified kernel and stride. This function is essential for image processing, feature extraction, and machine learning applications involving convolutional neural networks.
-
-## Installation
-You can install the library using pip:
-```
-pip install data-transformation-wizzard
-```
-
-## Usage
-To use the functions in the Data Wizzard Library, you first need to import the necessary functions. Below are some examples of how to use each feature:
-
-### Using `transpose2d`
-```python
-from data_transformation_wizzard import transpose2d
-matrix = [[1, 2], [3, 4]]
-print(transpose2d(matrix))
-```
-
-### Using `window1d`
-```python
-from data_transformation_wizzard import window1d
-array = [1, 2, 3, 4, 5, 6]
-size = 3
-shift = 1
-stride = 1
-print(window1d(array, size, shift, stride))
-```
-
-### Using `convolution2d`
-```python
-from data_transformation_wizzard import convolution2d
-input_matrix = [[0, 1, 2], [3, 4, 5], [6, 7, 8]]
-kernel = [[0, 1], [2, 3]]
-stride = 1
-print(convolution2d(input_matrix, kernel, stride))
-```
-
+
+# Data Wizzard Library
+
+## Overview
+The Data Wizzard Library is a Python package designed to simplify and streamline data transformation tasks. It provides a set of functions that perform common operations such as 2D transposition, 1D windowing, and 2D convolution. These functions are optimized for performance and ease of use, making it easier to manipulate and analyze data in Python.
+
+## Features
+
+### transpose2d
+This function transposes a 2D matrix, effectively flipping it over its diagonal, switching the matrix's row and column indices. This is particularly useful in numerical and matrix computations.
+
+### window1d
+The `window1d` function applies windowing operations to 1-dimensional arrays. This is useful in signal processing where segmenting data into overlapping or non-overlapping windows is required.
+
+### convolution2d
+Performs 2D convolution on an input matrix with a specified kernel and stride. This function is essential for image processing, feature extraction, and machine learning applications involving convolutional neural networks.
+
+## Installation
+You can install the library using pip:
+```
+pip install data-transformation-wizzard
+```
+
+## Usage
+To use the functions in the Data Wizzard Library, you first need to import the necessary functions. Below are some examples of how to use each feature:
+
+### Using `transpose2d`
+```python
+from data_transformation_wizzard import transpose2d
+matrix = [[1, 2], [3, 4]]
+print(transpose2d(matrix))
+```
+
+### Using `window1d`
+```python
+from data_transformation_wizzard import window1d
+array = [1, 2, 3, 4, 5, 6]
+size = 3
+shift = 1
+stride = 1
+print(window1d(array, size, shift, stride))
+```
+
+### Using `convolution2d`
+```python
+from data_transformation_wizzard import convolution2d
+input_matrix = [[0, 1, 2], [3, 4, 5], [6, 7, 8]]
+kernel = [[0, 1], [2, 3]]
+stride = 1
+print(convolution2d(input_matrix, kernel, stride))
+```
```


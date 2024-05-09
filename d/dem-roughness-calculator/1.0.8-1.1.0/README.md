# Comparing `tmp/dem_roughness_calculator-1.0.8.tar.gz` & `tmp/dem_roughness_calculator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dem_roughness_calculator-1.0.8.tar", last modified: Mon Apr 22 11:25:00 2024, max compression
+gzip compressed data, was "dem_roughness_calculator-1.1.0.tar", last modified: Thu May  9 14:48:39 2024, max compression
```

## Comparing `dem_roughness_calculator-1.0.8.tar` & `dem_roughness_calculator-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:25:00.690560 dem_roughness_calculator-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-22 11:25:00.690560 dem_roughness_calculator-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5417 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:25:00.690560 dem_roughness_calculator-1.0.8/dem_roughness_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-22 11:25:00.000000 dem_roughness_calculator-1.0.8/dem_roughness_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-22 11:25:00.000000 dem_roughness_calculator-1.0.8/dem_roughness_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 11:25:00.000000 dem_roughness_calculator-1.0.8/dem_roughness_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-22 11:25:00.000000 dem_roughness_calculator-1.0.8/dem_roughness_calculator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-22 11:25:00.000000 dem_roughness_calculator-1.0.8/dem_roughness_calculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 11:25:00.000000 dem_roughness_calculator-1.0.8/dem_roughness_calculator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:25:00.686560 dem_roughness_calculator-1.0.8/roughness_calculator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/roughness_calculator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:25:00.690560 dem_roughness_calculator-1.0.8/roughness_calculator/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/roughness_calculator/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/roughness_calculator/classes/application_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    24761 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/roughness_calculator/classes/geo_tiff_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/roughness_calculator/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/roughness_calculator/gui_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/roughness_calculator/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 11:25:00.690560 dem_roughness_calculator-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:25:00.690560 dem_roughness_calculator-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 11:24:50.000000 dem_roughness_calculator-1.0.8/tests/test_application_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 14:48:38.000000 dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:38.999421 dem_roughness_calculator-1.1.0/roughness_calculator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:38.999421 dem_roughness_calculator-1.1.0/roughness_calculator/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/classes/application_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/classes/geo_tiff_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/classes/processing_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21398 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/gui_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/log_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:38.999421 dem_roughness_calculator-1.1.0/roughness_calculator/old_entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/old_entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/old_entry_points/demcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/roughness_calculator/old_entry_points/demgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:39.003421 dem_roughness_calculator-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-09 14:48:28.000000 dem_roughness_calculator-1.1.0/tests/test_application_driver.py
```

### Comparing `dem_roughness_calculator-1.0.8/LICENSE` & `dem_roughness_calculator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dem_roughness_calculator-1.0.8/PKG-INFO` & `dem_roughness_calculator-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dem-roughness-calculator
-Version: 1.0.8
+Version: 1.1.0
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/dem-roughness-calculator
 Author: lbatschelet
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dem_roughness_calculator-1.0.8/README.md` & `dem_roughness_calculator-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,41 @@
-# DEM Roughness Calculator
+# DEM Surface Roughness Calculator
 
 The DEM Roughness Calculator is a comprehensive tool designed for geospatial analysis, allowing users to calculate the surface roughness of Digital Elevation Models (DEMs) using the standard deviation of height within a specified window size. The tool is equipped with both a graphical user interface (GUI) and a command-line interface (CLI), making it versatile for different user preferences and workflows.
 
 ## Features
 
 - **GeoTIFF Support**: Load and process DEM data directly from GeoTIFF files.
 - **Flexible Window Sizes**: Specify the window size in meters for roughness calculations.
 - **Advanced Thresholding**: Configure high value and categorical thresholds to refine processing.
 - **Dual Interface**: Operate through a user-friendly GUI or a powerful CLI.
 - **Dynamic Previews**: Generate and view pseudo-colored previews of the processed DEM within the GUI.
 - **Selective Saving**: Choose when to save processed outputs after reviewing results.
 
 ## Documentation
 
-For more detailed information about the tool's capabilities and additional configurations, please refer to the [Wiki](https://github.com/lbatschelet/dem-roughness-calculator/wiki).
-
+For more detailed information about the tool's capabilities and additional configurations, 
+please refer to the [Project's Wiki](https://github.com/lbatschelet/dem-roughness-calculator/wiki).
 
 ## Installation Guide for DEM Roughness Calculator
 
-This guide provides detailed steps for installing the DEM Roughness Calculator on Windows, macOS, and Linux systems. Please follow the instructions specific to your operating system.
+Follow these steps to install the DEM Roughness Calculator on your system. The program is available
+as a Python package and can therefore be installed on any major operating system.
+
+> [!TIP]
+> If you are not that experienced using command line tools or experience any problems during installation, please refer to the [Getting Started Wiki Page](https://github.com/lbatschelet/dem-roughness-calculator/wiki/Getting-Started) for a more detailed and OS specific installation guide.
 
 ### Prerequisites
 
 Before you begin, ensure that your system meets the following requirements:
 - **Python 3.12 or later**: The software is built to run with Python 3.12 and above.
 - **pip**: Python's package installer, used to install the DEM Roughness Calculator.
 
 ### Step-by-Step Installation
 
-Follow these steps to install the DEM Roughness Calculator on your system. The software supports Windows, macOS, and Linux.
-
 #### 1. Install Python
 Ensure you have Python 3.12 or later installed on your computer:
 - **Windows**: Download from the [official Python website](https://www.python.org/downloads/). Make sure to add Python to PATH during installation.
 - **macOS**: Install using Homebrew with `brew install python@3.12`.
 - **Linux**: Use your package manager, e.g., for Ubuntu: `sudo apt install python3.12 python3-pip`.
 
 #### 2. Verify Installation
@@ -45,54 +47,54 @@
 
 #### 3. Install DEM Roughness Calculator
 Install the package via pip:
 ```bash
 pip3 install dem-roughness-calculator
 ```
 
-For more detailed instructions on getting started with the DEM Roughness Calculator, including how to run the software and troubleshoot common issues, please refer to our [Getting Started page](https://github.com/lbatschelet/dem-roughness-calculator/wiki/Getting-Started).
 ## Usage
 
 ### GUI Application
 
 To launch the GUI, simply run the following command in your terminal:
 
 ```bash
-demgui
+surface-roughness
 ```
 
 The graphical interface allows you to browse for input files, set processing parameters, and view the roughness map interactively before deciding to save the output.
 
 ### CLI Application
 
 For those who prefer working in a command-line environment, the CLI provides a robust solution. Here’s how to use it:
 
 ```bash
-demcli --input_path "path/to/input.tif" --output_dir "path/to/output" --window_size 1.0 --band_number 1 --high_value_threshold 1.0 --categorical_thresholds 0.1 0.2 0.3
+surface-roughness --input_path "path/to/input.tif" --output_dir "path/to/output" --window_size 1.0 --band_number 1 --high_value_threshold 1.0 --categorical_thresholds 0.1, 0.2, 0.3
 ```
 
 ### Parameters
 
 - **`--input_path`**: Path to the input GeoTIFF file.
 - **`--output_dir`**: Directory where the output files will be saved.
 - **`--window_size`** (optional): The size of the window in meters for calculating roughness.
 - **`--band_number`** (optional): The specific band of the DEM to process.
 - **`--high_value_threshold`** (optional): Threshold to filter out high elevation values.
 - **`--categorical_thresholds`** (optional): Set of thresholds to categorize the elevation data.
 
-## Contributing
-
-We welcome contributions! If you have suggestions or want to report bugs, please use the [Issues](https://github.com/lbatschelet/dem-roughness-calculator/issues) section of this repository.
-
 ## Disclaimer
 
-### AI-Assisted Development
-
-This project leverages artificial intelligence, including OpenAI's GPT-4 and GitHub Copilot, to assist in generating parts of the code and documentation. These tools provide suggestions that enhance the development process and help in crafting more robust and comprehensive materials. While AI tools have been instrumental in accelerating development and improving productivity, the final decisions on the inclusion and modification of the generated content rest solely with the human developers. This ensures that each aspect of the project aligns with our quality standards and functional requirements.
+> [!NOTE]
+> **AI-Assisted Development**
+> 
+> This project leverages artificial intelligence, including OpenAI's GPT-4 and GitHub Copilot, to assist in generating parts of the code and documentation. These tools provide suggestions that enhance the development process and help in crafting more robust and comprehensive materials. While AI tools have been instrumental in accelerating development and improving productivity, the final decisions on the inclusion and modification of the generated content rest solely with the human developers. This ensures that each aspect of the project aligns with our quality standards and functional requirements. 
+> 
+> Please note that while AI has contributed to the project, it may not capture the full complexity or context of the development practices. As such, any anomalies or errors introduced by AI-generated content have been reviewed and rectified to the best of our capabilities. However, users should exercise their judgment and discretion when using or modifying this software. 
+> 
+> For any concerns or questions about the AI-generated content within this project, please feel free to contact us through the repository's issues section.
 
-Please note that while AI has contributed to the project, it may not capture the full complexity or context of the development practices. As such, any anomalies or errors introduced by AI-generated content have been reviewed and rectified to the best of our capabilities. However, users should exercise their judgment and discretion when using or modifying this software.
+## Contributing
 
-For any concerns or questions about the AI-generated content within this project, please feel free to contact us through the repository's issues section or directly via the contact methods provided on this page.
+We welcome contributions! If you have suggestions or want to report bugs, please use the [Issues](https://github.com/lbatschelet/dem-roughness-calculator/issues) section of this repository.
 
 ## License
 
-This project is licensed under the GPL-3.0 License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the GPL-3.0 License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `dem_roughness_calculator-1.0.8/dem_roughness_calculator.egg-info/PKG-INFO` & `dem_roughness_calculator-1.1.0/dem_roughness_calculator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dem-roughness-calculator
-Version: 1.0.8
+Version: 1.1.0
 Summary: A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI
 Home-page: https://github.com/lbatschelet/dem-roughness-calculator
 Author: lbatschelet
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dem_roughness_calculator-1.0.8/roughness_calculator/classes/application_driver.py` & `dem_roughness_calculator-1.1.0/roughness_calculator/classes/application_driver.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """
 application_driver.py
 ---------------------
-Version: 1.0.8
+Version: 1.1.0
 Author: Lukas Batschelet
-Date: 22.04.2024
+Date: 09.05.2024
 ---------------------
 This module contains the ApplicationDriver class which is responsible for running the application.
 It acts as a sort of interface between the calling User Interface (UI) and the GeoTIFFProcessor class.
 This enables the separation of concerns and allows for easier testing and maintenance of the code.
 (i.e. the UI does not need to know how the processing is done, it just needs to know how to call the processing.)
 """
-from typing import List, Optional, Union
 import datetime
+import logging
 import os
+from typing import Union
 
+import matplotlib.pyplot as plt
 import numpy as np
 import rasterio
 from PIL import Image
-import matplotlib.pyplot as plt
 
 from .geo_tiff_processor import GeoTIFFProcessor
-
-import logging
+from .processing_parameters import ProcessingParameters
 from ..log_config import setup_logging
 
 # Ensure the logger is set up (optional if you know `log_config.py` is already imported elsewhere)
 setup_logging()
 
 logger = logging.getLogger(__name__)
 
@@ -60,69 +60,42 @@
     # If the value is a positive number, log a confirmation message
     logging.info(f"Valid {parameter_name}: {value}")
 
     return value
 
 
 class ApplicationDriver:
-    def __init__(
-            self,
-            input_path: str,
-            output_dir: Optional[str] = None,
-            window_size: Optional[float] = None,
-            band_number: Optional[int] = None,
-            high_value_threshold: Optional[float] = None,
-            category_thresholds: Optional[List[float]] = None
-    ):
+    def __init__(self, params: ProcessingParameters):
         """
         Initializes the ApplicationDriver with necessary parameters for processing a GeoTIFF file.
 
         Args:
-            input_path (str): Path to the input GeoTIFF file.
-            output_dir (str, optional): Path to the output directory. If None, data is processed but not saved.
-            window_size (float, optional): Side length of the square window in meters for roughness calculation.
-            band_number (int, optional): Specific band number to process.
-            high_value_threshold (float, optional): Threshold value to filter out high data values.
-            category_thresholds (List[float], optional): Thresholds for categorizing data values.
+            params (ProcessingParameters): The processing parameters for the ApplicationDriver.
 
         Raises:
             FileNotFoundError: If the input path or output directory is not valid.
         """
 
-        self.input_path = input_path  # Store the path to the input GeoTIFF file
-        self.output_dir = output_dir  # Store the path to the output directory if provided
+        self.input_path = params.input_path  # Store the path to the input GeoTIFF file
+        self.output_dir = params.output_dir  # Store the path to the output directory if provided
 
         # Attempt to create an output filename if an output directory is provided
-        self.output_path = self.create_output_filename() if output_dir else None
+        self.output_path = self.create_output_filename() if params.output_dir else None
 
         # Store additional processing parameters
-        self.window_size = window_size
-        self.band_number = band_number
-        self.high_value_threshold = high_value_threshold
-        self.category_thresholds = category_thresholds
+        self.window_size = params.window_size
+        self.band_number = params.band_number
+        self.high_value_threshold = params.high_value_threshold
+        self.category_thresholds = params.category_thresholds
 
         self.processed_data = None  # This will hold the processed data after running the processor
         self.preview = None  # This will hold the image preview of the processed data
 
-        # Validate the input path and output directory if provided
-        self.check_input_path()
-        if output_dir:
-            self.check_output_dir()
-
-        # Create a dictionary of processing parameters, excluding None values
-        params = {
-            'window_size': window_size,
-            'band_number': band_number,
-            'high_value_threshold': high_value_threshold,
-            'category_thresholds': category_thresholds
-        }
-        filtered_params = {k: v for k, v in params.items() if v is not None}
-
-        # Initialize the GeoTIFFProcessor with filtered parameters
-        self.processor = GeoTIFFProcessor(input_path, **filtered_params)
+        # Initialize the GeoTIFFProcessor with the parameters
+        self.processor = GeoTIFFProcessor(params)
 
     def run(self) -> None:
         """
         Initiates the processing of the GeoTIFF file.
 
         This method is responsible for initiating the processing of the GeoTIFF file. It logs the start and end of the
         processing, as well as the input and output paths. If an output directory is provided,
@@ -138,57 +111,22 @@
         logging.info(f"Output dir: {self.output_dir}")
 
         # Process the GeoTIFF file and store the result in self.processed_data
         self.processed_data = self.processor.process_tiff()
 
         # If an output directory is provided or running in CLI mode, save the processed data immediately
         if self.output_dir:
-            self.save_processed_data(self.processed_data)
+            self.save_processed_data(self.output_dir)
 
         # Otherwise, generate a preview of the processed data
         else:
             self.produce_preview()
 
         logging.info("Processing completed.")
 
-    def check_input_path(self) -> None:
-        """
-        Checks if the input path is valid.
-        If the input path is not valid, it logs an error message and raises a FileNotFoundError.
-
-        Raises:
-            FileNotFoundError: If the input path is not valid.
-        """
-        # Check if the input path is a file
-        if not os.path.isfile(self.input_path):
-            # If the input path is not a file, log and raise an error message
-            logging.error(f"Invalid input path: {self.input_path}")
-            raise FileNotFoundError(f"No file found at specified input path: {self.input_path}")
-
-        logging.info(f"Valid input path: {self.input_path}")
-
-    def check_output_dir(self) -> None:
-        """
-        Checks if the output directory exists.
-        If the output directory does not exist, it logs an error message and raises a FileNotFoundError.
-
-        Raises:
-            FileNotFoundError: If the output directory does not exist.
-        """
-        # Extract the directory name from the output directory path
-        output_dir = os.path.dirname(self.output_dir)
-
-        # Check if the directory exists
-        if not os.path.isdir(output_dir):
-            # If the directory does not exist, log an error and raise an exception
-            logging.error(f"Invalid output directory: {output_dir}")
-            raise FileNotFoundError(f"The directory for the output path does not exist: {output_dir}")
-
-        logging.info(f"Valid output directory: {output_dir}")
-
     def produce_preview(self, nodata_value: int = -9999) -> None:
         """
         Generates a preview image from the processed data stored in self.processed_data.
         This method avoids re-reading the data from file, making it more efficient.
         Uses pseudo-color to represent the data visually, ensuring nodata values are transparent.
 
         Args:
```

### Comparing `dem_roughness_calculator-1.0.8/roughness_calculator/cli_main.py` & `dem_roughness_calculator-1.1.0/roughness_calculator/cli_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,95 @@
 """
 cli_main.py
 -----------
-Version: 1.0.8
+Version: 1.1.0
 Author: Lukas Batschelet
-Date: 22.04.2024
+Date: 09.05.2024
 -----------
 """
-from roughness_calculator.classes.application_driver import ApplicationDriver
+import argparse
 import logging
+import sys
+
+from roughness_calculator.classes.application_driver import ApplicationDriver
+from roughness_calculator.classes.processing_parameters import ProcessingParameters
 from .log_config import setup_logging
-import argparse
-from typing import NoReturn
 
 # Ensure the logger is set up (optional if you know `log_config.py` is already imported elsewhere)
 setup_logging()
 
 logger = logging.getLogger(__name__)
 
 
 class CLIMain:
-    def __init__(self) -> NoReturn:
+    def __init__(self) -> None:
         """
         Initialize the command line interface for the application.
-
-        This method sets up the argument parser for the command line interface.
-
-        Returns:
-            None
         """
-        # Initialize the argument parser with a description
         self.parser = argparse.ArgumentParser(
-            description="CLI tool for processing GeoTIFF files to calculate surface roughness."
+            description="Tool for processing GeoTIFF DEM files to calculate and categorize surface roughness. \n"
+                        "Running the command without any arguments will start a Graphical User Interface."
+
         )
-        # Set up the command line arguments
         self.setup_arguments()
 
     def setup_arguments(self) -> None:
         """
-        Set up command line arguments.
-
-        This method configures the command line arguments for the application.
-
-        Returns:
-            None
+        Set up command line arguments for the application.
         """
-        # Add argument for the input GeoTIFF file path
-        self.parser.add_argument('input_path', type=str, help='The path to the input GeoTIFF file.')
-
-        # Add argument for the output directory path
-        self.parser.add_argument('output_dir', type=str, help='The path to the output directory.')
-
-        # Add optional argument for the window size with a default value of 1.0
-        self.parser.add_argument('--window_size', type=float, default=1.0,
-                                 help='The side length of the square window in meters. Default is 1.')
-
-        # Add optional argument for the band number to be processed with a default value of 1
-        self.parser.add_argument('--band_number', type=int, default=1,
-                                 help='The band number to be processed. Default is 1.')
-
-        # Add optional argument for the high value threshold with a default value of 1.0
-        self.parser.add_argument('--high_value_threshold', type=float, default=1.0,
-                                 help='The threshold for high values to be filtered out. Default is 1.0.')
-
-        # Add optional argument for the category thresholds
-        self.parser.add_argument('--category_thresholds', type=float, nargs='+',
-                                 help='List of thresholds to categorize data.')
+        # Mandatory arguments
+        self.parser.add_argument('input_path', type=str,
+                                 help='The path to the input GeoTIFF file.')
+        self.parser.add_argument('output_dir', type=str,
+                                 help='The path to the output directory.')
+
+        # Optional arguments with defaults managed in the ProcessingParameters class
+        self.parser.add_argument('--window_size', type=float,
+                                 help='The side length of the square window in meters.')
+        self.parser.add_argument('--band_number', type=int,
+                                 help='The band number to be processed.')
+        self.parser.add_argument('--high_value_threshold', type=float,
+                                 help='The threshold for high values to be filtered out.')
+        self.parser.add_argument('--category_thresholds', type=str,
+                                 help='Comma-separated thresholds to categorize data.')
 
     def run(self) -> None:
         """
         Execute the command line interface.
-
-        This method parses the command line arguments and initializes the ApplicationDriver with these arguments.
-        It then runs the ApplicationDriver.
-
-        Returns:
-            None
         """
-        # Parse the command line arguments
         args = self.parser.parse_args()
 
-        # Initialize the ApplicationDriver with the parsed arguments
-        driver = ApplicationDriver(
-            input_path=args.input_path,
-            output_dir=args.output_dir,
-            window_size=args.window_size,
-            band_number=args.band_number,
-            high_value_threshold=args.high_value_threshold,
-            category_thresholds=args.category_thresholds
-        )
-
-        # Run the ApplicationDriver
-        driver.run()
+        # Convert the args to a dictionary and create ProcessingParameters
+        params_dict = {
+            'input_path': args.input_path,
+            'output_dir': args.output_dir,
+            'window_size': args.window_size,
+            'band_number': args.band_number,
+            'high_value_threshold': args.high_value_threshold,
+            'category_thresholds': args.category_thresholds
+        }
+        # Remove None values explicitly to handle optional parameters correctly
+        filtered_params = {k: v for k, v in params_dict.items() if v is not None}
+
+        try:
+            # Create ProcessingParameters instance using the factory method
+            processing_params = ProcessingParameters.create_from_dict(filtered_params)
+
+            # Initialize and run the application driver with the validated and converted parameters
+            driver = ApplicationDriver(processing_params)
+            driver.run()
+
+        except Exception as e:
+            print(f"Error: {e}", file=sys.stderr)
+            sys.exit(1)
+
+
+if __name__ == '__main__':
+    cli = CLIMain()
+    cli.run()
 
 
 def main() -> None:
     """
     Entry point for the CLI.
 
     This method initializes the CLIMain class and runs it.
```

### Comparing `dem_roughness_calculator-1.0.8/roughness_calculator/gui_main.py` & `dem_roughness_calculator-1.1.0/roughness_calculator/gui_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 gui_main.py
 -----------
-Version: 1.0.8
+Version: 1.1.0
 Author: Lukas Batschelet
-Date: 22.04.2024
+Date: 09.05.2024
 -----------
 This module contains the ApplicationGUI class which is
 responsible for creating the graphical user interface (GUI) of the application.
 """
 from PIL import Image, ImageTk
 
 from roughness_calculator.classes.application_driver import ApplicationDriver
 
 import tkinter as tk
 from tkinter import filedialog, messagebox, Label, Button, Entry, Frame
 import logging
+
+from roughness_calculator.classes.processing_parameters import ProcessingParameters
 from .log_config import setup_logging
 
 # Ensure the logger is set up (optional if you know `log_config.py` is already imported elsewhere)
 setup_logging()
 
 logger = logging.getLogger(__name__)
 
@@ -127,15 +129,15 @@
             # band_number
             (Label(options_frame, text="Band Number: (Default is 1, only in rare cases different)").
              grid(row=2, column=0, sticky='e'))
             self.band_number_entry = Entry(options_frame, width=15)
             self.band_number_entry.grid(row=2, column=1, sticky='e')
 
             # high_value_threshold
-            (Label(options_frame, text="High Value Threshold: (Default is 1.0, should often be lower, rarely higher)").
+            (Label(options_frame, text="High Value Threshold: (Default is 10.0, used to cut off crazy values at file borders)").
              grid(row=3, column=0, sticky='e'))
             self.high_value_threshold_entry = Entry(options_frame, width=15)
             self.high_value_threshold_entry.grid(row=3, column=1, sticky='e')
 
             # category_thresholds
             (Label(options_frame, text="category Thresholds (comma-separated): (Default is None)").
              grid(row=4, column=0, sticky='e'))
@@ -228,51 +230,42 @@
             logging.error("Error setting output directory: " + str(e))
             raise RuntimeError("Error setting output directory: " + str(e))
 
     def start_processing(self) -> None:
         """
         Starts the processing of the GeoTIFF file with the provided parameters.
 
-        This method gathers the parameters from the GUI, filters out None values,
-        and creates an instance of the ApplicationDriver class with these parameters.
-        It then runs the application driver and handles any exceptions that might occur.
+        This method gathers the parameters from the GUI, creates an instance of the ProcessingParameters class,
+        initializes the ApplicationDriver with these parameters, and manages the processing flow,
+        including displaying results and handling errors.
 
         Raises:
             FileNotFoundError: If the input file is not found.
             ValueError: If an invalid value is provided for a parameter.
             RuntimeError: If there's an error during processing.
         """
         try:
-            # Get the input path from the GUI
-            input_path = self.input_path_entry.get()
-            if not input_path:
-                messagebox.showerror("Error", "Input path is required.")
-                return
-
-            # Gather parameters from the GUI, setting to None if not provided
-            output_dir = self.output_dir_entry.get() or None
-            window_size = float(self.window_size_entry.get()) if self.window_size_entry.get() else None
-            band_number = int(self.band_number_entry.get()) if self.band_number_entry.get() else None
-            high_value_threshold = float(
-                self.high_value_threshold_entry.get()) if self.high_value_threshold_entry.get() else None
-            thresholds_text = self.category_thresholds_entry.get()
-            category_thresholds = [float(x) for x in thresholds_text.split(',')] if thresholds_text else None
-
-            # Filter parameters to exclude None values, allowing for flexible argument passing
-            params = {
-                'output_dir': output_dir,
-                'window_size': window_size,
-                'band_number': band_number,
-                'high_value_threshold': high_value_threshold,
-                'category_thresholds': category_thresholds
+            # Gather parameters from the GUI
+            params_dict = {
+                "input_path": self.input_path_entry.get() or None,
+                "output_dir": self.output_dir_entry.get() or None,
+                "window_size": self.window_size_entry.get() or None,
+                "band_number": self.band_number_entry.get() or None,
+                "high_value_threshold": self.high_value_threshold_entry.get() or None,
+                "category_thresholds": self.category_thresholds_entry.get() or None
             }
-            filtered_params = {k: v for k, v in params.items() if v is not None}
 
-            # Create and run the application driver with provided arguments
-            self.driver = ApplicationDriver(input_path, **filtered_params)
+            # Filter out None values to allow optional parameters to use defaults
+            filtered_params = {k: v for k, v in params_dict.items() if v is not None}
+
+            # Create ProcessingParameters instance using the factory method
+            processing_params = ProcessingParameters.create_from_dict(filtered_params)
+
+            # Initialize and run the application driver with the validated and converted parameters
+            self.driver = ApplicationDriver(processing_params)
             self.driver.run()
 
             # Get the preview of the processed data
             preview = self.driver.get_preview()
             if preview:
                 self.display_preview(preview)
                 if 'output_dir' not in filtered_params:
```

### Comparing `dem_roughness_calculator-1.0.8/roughness_calculator/log_config.py` & `dem_roughness_calculator-1.1.0/roughness_calculator/log_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+"""
+log_comnfig.py
+-----------
+Version: 1.0.9
+Author: Lukas Batschelet
+Date: 08.05.2024
+-----------
+This module sets up the logging for the application.
+"""
+
 import os
 import logging
 
 
 def setup_logging() -> None:
     """
     Sets up the logging for the application.
```

### Comparing `dem_roughness_calculator-1.0.8/setup.py` & `dem_roughness_calculator-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 # Read the contents of your requirements file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='dem-roughness-calculator',
-    version='1.0.8',
+    version='1.1.0',
     packages=find_packages(),  # Automatically find all packages in the directory
     url='https://github.com/lbatschelet/dem-roughness-calculator',
     license='GPL-3.0',
     author='lbatschelet',
     description='A package for calculating surface roughness using GeoTIFF DEM files with a GUI and CLI',
     install_requires=requirements,  # Install dependencies from requirements.txt
     python_requires='>=3.12',  # Specify Python version requirement
     entry_points={
         'console_scripts': [
-            'demgui=roughness_calculator.gui_main:main',
-            'demcli=roughness_calculator.cli_main:main'
+            'surface-roughness=roughness_calculator.main:main',
+            'demgui=roughness_calculator.old_entry_points.demgui:main',
+            'demcli=roughness_calculator.old_entry_points.demcli:main',
         ]
     },
     classifiers=[
         'Development Status :: 4 - Beta',  # Update as appropriate for your release cycle
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
```


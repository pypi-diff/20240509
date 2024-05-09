# Comparing `tmp/automlapp-0.1.71.tar.gz` & `tmp/automlapp-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automlapp-0.1.71.tar", last modified: Wed May  8 06:46:24 2024, max compression
+gzip compressed data, was "automlapp-0.1.72.tar", last modified: Thu May  9 09:14:11 2024, max compression
```

## Comparing `automlapp-0.1.71.tar` & `automlapp-0.1.72.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:46:24.436371 automlapp-0.1.71/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:46:24.436371 automlapp-0.1.71/AutoMLApp.egg-info/
--rw-rw-rw-   0        0        0     5052 2024-05-08 06:46:24.000000 automlapp-0.1.71/AutoMLApp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2024-05-08 06:46:24.000000 automlapp-0.1.71/AutoMLApp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:46:24.000000 automlapp-0.1.71/AutoMLApp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-08 06:46:24.000000 automlapp-0.1.71/AutoMLApp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      268 2024-05-08 06:46:24.000000 automlapp-0.1.71/AutoMLApp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-08 06:46:24.000000 automlapp-0.1.71/AutoMLApp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.71/LICENSE
--rw-rw-rw-   0        0        0     5052 2024-05-08 06:46:24.436371 automlapp-0.1.71/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2024-04-12 09:40:36.000000 automlapp-0.1.71/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 06:46:24.418579 automlapp-0.1.71/automlapp/
--rw-rw-rw-   0        0        0        0 2024-05-08 06:45:40.000000 automlapp-0.1.71/automlapp/__init__.py
--rw-rw-rw-   0        0        0    60971 2024-05-08 06:34:59.000000 automlapp-0.1.71/automlapp/app.py
--rw-rw-rw-   0        0        0      212 2024-05-08 06:29:45.000000 automlapp-0.1.71/automlapp/launcher.py
--rw-rw-rw-   0        0        0   109179 2024-02-26 11:55:20.000000 automlapp-0.1.71/automlapp/logo.png
-drwxrwxrwx   0        0        0        0 2024-05-08 06:46:24.436371 automlapp-0.1.71/automlapp/modules/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.71/automlapp/modules/__init__.py
--rw-rw-rw-   0        0        0     5467 2024-05-08 06:33:17.000000 automlapp-0.1.71/automlapp/modules/data_cleaning.py
--rw-rw-rw-   0        0        0     2509 2024-05-08 06:33:24.000000 automlapp-0.1.71/automlapp/modules/data_input.py
--rw-rw-rw-   0        0        0     3330 2024-05-08 06:33:30.000000 automlapp-0.1.71/automlapp/modules/data_preprocessing.py
--rw-rw-rw-   0        0        0     1072 2024-05-08 06:33:34.000000 automlapp-0.1.71/automlapp/modules/data_summarization.py
--rw-rw-rw-   0        0        0     3431 2024-05-08 06:33:50.000000 automlapp-0.1.71/automlapp/modules/data_visualization.py
--rw-rw-rw-   0        0        0     3648 2024-05-08 06:34:07.000000 automlapp-0.1.71/automlapp/modules/data_woeiv.py
--rw-rw-rw-   0        0        0     9479 2024-05-08 06:34:12.000000 automlapp-0.1.71/automlapp/modules/hyperparameter_tuning.py
--rw-rw-rw-   0        0        0    14621 2024-05-08 06:34:22.000000 automlapp-0.1.71/automlapp/modules/model_evaluation.py
--rw-rw-rw-   0        0        0     5532 2024-05-08 06:34:28.000000 automlapp-0.1.71/automlapp/modules/model_training.py
--rw-rw-rw-   0        0        0     6453 2024-05-08 06:34:32.000000 automlapp-0.1.71/automlapp/modules/train_user_params.py
--rwxrwxrwx   0        0        0      266 2024-05-08 06:32:01.000000 automlapp-0.1.71/automlapp/runtool.bat
-drwxrwxrwx   0        0        0        0 2024-05-08 06:46:24.436371 automlapp-0.1.71/automlapp/utils/
--rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.71/automlapp/utils/__init__.py
--rw-rw-rw-   0        0        0      197 2024-05-08 06:34:51.000000 automlapp-0.1.71/automlapp/utils/print_utils.py
--rw-rw-rw-   0        0        0      857 2024-05-07 11:32:56.000000 automlapp-0.1.71/automlapp/utils/streamlit_utils.py
--rw-rw-rw-   0        0        0       42 2024-05-08 06:46:24.450138 automlapp-0.1.71/setup.cfg
--rw-rw-rw-   0        0        0     1529 2024-05-08 06:46:14.000000 automlapp-0.1.71/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 09:14:11.828177 automlapp-0.1.72/
+drwxrwxrwx   0        0        0        0 2024-05-09 09:14:11.820583 automlapp-0.1.72/AutoMLApp.egg-info/
+-rw-rw-rw-   0        0        0     5253 2024-05-09 09:14:11.000000 automlapp-0.1.72/AutoMLApp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      827 2024-05-09 09:14:11.000000 automlapp-0.1.72/AutoMLApp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 09:14:11.000000 automlapp-0.1.72/AutoMLApp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-09 09:14:11.000000 automlapp-0.1.72/AutoMLApp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      227 2024-05-09 09:14:11.000000 automlapp-0.1.72/AutoMLApp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 09:14:11.000000 automlapp-0.1.72/AutoMLApp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2024-05-03 11:39:36.000000 automlapp-0.1.72/LICENSE
+-rw-rw-rw-   0        0        0     5253 2024-05-09 09:14:11.825404 automlapp-0.1.72/PKG-INFO
+-rw-rw-rw-   0        0        0     4346 2024-05-09 09:13:47.000000 automlapp-0.1.72/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 09:14:11.687377 automlapp-0.1.72/automlapp/
+-rw-rw-rw-   0        0        0        0 2024-05-08 06:45:40.000000 automlapp-0.1.72/automlapp/__init__.py
+-rw-rw-rw-   0        0        0    60971 2024-05-08 06:34:59.000000 automlapp-0.1.72/automlapp/app.py
+-rw-rw-rw-   0        0        0      212 2024-05-08 06:29:45.000000 automlapp-0.1.72/automlapp/launcher.py
+-rw-rw-rw-   0        0        0   109179 2024-02-26 11:55:20.000000 automlapp-0.1.72/automlapp/logo.png
+drwxrwxrwx   0        0        0        0 2024-05-09 09:14:11.799145 automlapp-0.1.72/automlapp/modules/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:32.000000 automlapp-0.1.72/automlapp/modules/__init__.py
+-rw-rw-rw-   0        0        0     5467 2024-05-08 06:33:17.000000 automlapp-0.1.72/automlapp/modules/data_cleaning.py
+-rw-rw-rw-   0        0        0     2509 2024-05-08 06:33:24.000000 automlapp-0.1.72/automlapp/modules/data_input.py
+-rw-rw-rw-   0        0        0     3330 2024-05-08 06:33:30.000000 automlapp-0.1.72/automlapp/modules/data_preprocessing.py
+-rw-rw-rw-   0        0        0     1072 2024-05-08 06:33:34.000000 automlapp-0.1.72/automlapp/modules/data_summarization.py
+-rw-rw-rw-   0        0        0     3431 2024-05-08 06:33:50.000000 automlapp-0.1.72/automlapp/modules/data_visualization.py
+-rw-rw-rw-   0        0        0     3648 2024-05-08 06:34:07.000000 automlapp-0.1.72/automlapp/modules/data_woeiv.py
+-rw-rw-rw-   0        0        0     9479 2024-05-08 06:34:12.000000 automlapp-0.1.72/automlapp/modules/hyperparameter_tuning.py
+-rw-rw-rw-   0        0        0    14621 2024-05-08 06:34:22.000000 automlapp-0.1.72/automlapp/modules/model_evaluation.py
+-rw-rw-rw-   0        0        0     5532 2024-05-08 06:34:28.000000 automlapp-0.1.72/automlapp/modules/model_training.py
+-rw-rw-rw-   0        0        0     6453 2024-05-08 06:34:32.000000 automlapp-0.1.72/automlapp/modules/train_user_params.py
+-rwxrwxrwx   0        0        0      266 2024-05-08 06:32:01.000000 automlapp-0.1.72/automlapp/runtool.bat
+drwxrwxrwx   0        0        0        0 2024-05-09 09:14:11.817898 automlapp-0.1.72/automlapp/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:09:13.000000 automlapp-0.1.72/automlapp/utils/__init__.py
+-rw-rw-rw-   0        0        0      197 2024-05-08 06:34:51.000000 automlapp-0.1.72/automlapp/utils/print_utils.py
+-rw-rw-rw-   0        0        0      857 2024-05-07 11:32:56.000000 automlapp-0.1.72/automlapp/utils/streamlit_utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 09:14:11.828177 automlapp-0.1.72/setup.cfg
+-rw-rw-rw-   0        0        0     1538 2024-05-09 08:59:42.000000 automlapp-0.1.72/setup.py
```

### Comparing `automlapp-0.1.71/AutoMLApp.egg-info/PKG-INFO` & `automlapp-0.1.72/AutoMLApp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.71
+Version: 0.1.72
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
-Author: Shivam Nikam
+Author: Think360.ai
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,20 +16,16 @@
 Requires-Dist: streamlit==1.32.0
 Requires-Dist: streamlit-extras==0.4.0
 Requires-Dist: streamlit-modal==0.1.2
 Requires-Dist: plotly==5.18.0
 Requires-Dist: scikit-learn==1.4.1.post1
 Requires-Dist: lightgbm==4.3.0
 Requires-Dist: xgboost==2.0.3
-Requires-Dist: openpyxl==3.0.10
+Requires-Dist: openpyxl==3.1.0
 Requires-Dist: scorecardpy==0.1.9.7
-Provides-Extra: dev
-Requires-Dist: pytest>=5.2; extra == "dev"
-Requires-Dist: check-manifest; extra == "dev"
-Requires-Dist: twine; extra == "dev"
 
 ## Introduction
 
 **Overview**
 
 The AutoML Web App revolutionizes the credit underwriting process by automating critical steps, including data preprocessing, model fitting, and hyperparameter tuning, to ensure accurate risk assessments. Designed to streamline the workflow, it significantly enhances efficiency and precision in lending risk management for both individuals and businesses.
 
@@ -55,36 +51,47 @@
 
 A basic understanding of Python and the use of virtual environments for managing package dependencies is also recommended.
 
 ### Installation:
 
 To install the AutoML Web App, follow these steps:
 
-1. **Clone the Repository**: Begin by cloning the AutoML Web App repository to your local machine with Git:
+1. **Navigate to Local Directory**: Begin by navigating to Local Directory on your local machine cli:
    ```bash
-   git clone https://github.com/Adityaa2805/AutoMLApp.git
-   cd AutoMLApp
+   cd "direcoty"
    ```
 
 2. **Create a Virtual Environment** (Optional but Recommended): To prevent potential conflicts with existing Python packages on your system, it is advisable to create a virtual environment within the cloned directory:
    ```bash
    python3 -m venv venv
    # Activate the virtual environment
    # On Windows
    venv\Scripts\activate
    # On macOS and Linux
    source venv/bin/activate
    ```
 
-3. **Install Dependencies**: Install all necessary Python packages using the provided `requirements.txt`:
+3. **Install Wheel File**: Install all necessary Python packages using the provided `AuotMLApp.whl` file or directly installing the python package:
    ```bash
-   pip install -r requirements.txt
+   pip install AutoMLApp
+   pip install "path to wheelfile"
    ```
 
-4. **Start the App**: After installing the dependencies, you can launch the AutoML Web App by executing:
+4. **Check Package**: After installing the package, you can see the properties by executing:
+   ```bash
+   pip show AutoMLApp
+   ```
+
+5. **Change the directory to Application's directory**: After copying the dependencies, you need to navigate to the AutoML Web App by executing:
+   ```bash
+   cd "copied location"
+   cd automlapp
+   ```
+
+6. **Start the App**: After installing the dependencies, you can launch the AutoML Web App by executing:
    ```bash
    streamlit run app.py
    ```
 
    This command initiates the app and should automatically open it in your default web browser. If the app does not open automatically, a URL will be displayed in your terminal, which you can use to access the app manually.
```

### Comparing `automlapp-0.1.71/AutoMLApp.egg-info/SOURCES.txt` & `automlapp-0.1.72/AutoMLApp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/LICENSE` & `automlapp-0.1.72/LICENSE`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/PKG-INFO` & `automlapp-0.1.72/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: AutoMLApp
-Version: 0.1.71
+Version: 0.1.72
 Summary: An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.
-Author: Shivam Nikam
+Author: Think360.ai
 Author-email: shivam.nikam@think360.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,20 +16,16 @@
 Requires-Dist: streamlit==1.32.0
 Requires-Dist: streamlit-extras==0.4.0
 Requires-Dist: streamlit-modal==0.1.2
 Requires-Dist: plotly==5.18.0
 Requires-Dist: scikit-learn==1.4.1.post1
 Requires-Dist: lightgbm==4.3.0
 Requires-Dist: xgboost==2.0.3
-Requires-Dist: openpyxl==3.0.10
+Requires-Dist: openpyxl==3.1.0
 Requires-Dist: scorecardpy==0.1.9.7
-Provides-Extra: dev
-Requires-Dist: pytest>=5.2; extra == "dev"
-Requires-Dist: check-manifest; extra == "dev"
-Requires-Dist: twine; extra == "dev"
 
 ## Introduction
 
 **Overview**
 
 The AutoML Web App revolutionizes the credit underwriting process by automating critical steps, including data preprocessing, model fitting, and hyperparameter tuning, to ensure accurate risk assessments. Designed to streamline the workflow, it significantly enhances efficiency and precision in lending risk management for both individuals and businesses.
 
@@ -55,36 +51,47 @@
 
 A basic understanding of Python and the use of virtual environments for managing package dependencies is also recommended.
 
 ### Installation:
 
 To install the AutoML Web App, follow these steps:
 
-1. **Clone the Repository**: Begin by cloning the AutoML Web App repository to your local machine with Git:
+1. **Navigate to Local Directory**: Begin by navigating to Local Directory on your local machine cli:
    ```bash
-   git clone https://github.com/Adityaa2805/AutoMLApp.git
-   cd AutoMLApp
+   cd "direcoty"
    ```
 
 2. **Create a Virtual Environment** (Optional but Recommended): To prevent potential conflicts with existing Python packages on your system, it is advisable to create a virtual environment within the cloned directory:
    ```bash
    python3 -m venv venv
    # Activate the virtual environment
    # On Windows
    venv\Scripts\activate
    # On macOS and Linux
    source venv/bin/activate
    ```
 
-3. **Install Dependencies**: Install all necessary Python packages using the provided `requirements.txt`:
+3. **Install Wheel File**: Install all necessary Python packages using the provided `AuotMLApp.whl` file or directly installing the python package:
    ```bash
-   pip install -r requirements.txt
+   pip install AutoMLApp
+   pip install "path to wheelfile"
    ```
 
-4. **Start the App**: After installing the dependencies, you can launch the AutoML Web App by executing:
+4. **Check Package**: After installing the package, you can see the properties by executing:
+   ```bash
+   pip show AutoMLApp
+   ```
+
+5. **Change the directory to Application's directory**: After copying the dependencies, you need to navigate to the AutoML Web App by executing:
+   ```bash
+   cd "copied location"
+   cd automlapp
+   ```
+
+6. **Start the App**: After installing the dependencies, you can launch the AutoML Web App by executing:
    ```bash
    streamlit run app.py
    ```
 
    This command initiates the app and should automatically open it in your default web browser. If the app does not open automatically, a URL will be displayed in your terminal, which you can use to access the app manually.
```

### Comparing `automlapp-0.1.71/README.md` & `automlapp-0.1.72/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,36 +26,47 @@
 
 A basic understanding of Python and the use of virtual environments for managing package dependencies is also recommended.
 
 ### Installation:
 
 To install the AutoML Web App, follow these steps:
 
-1. **Clone the Repository**: Begin by cloning the AutoML Web App repository to your local machine with Git:
+1. **Navigate to Local Directory**: Begin by navigating to Local Directory on your local machine cli:
    ```bash
-   git clone https://github.com/Adityaa2805/AutoMLApp.git
-   cd AutoMLApp
+   cd "direcoty"
    ```
 
 2. **Create a Virtual Environment** (Optional but Recommended): To prevent potential conflicts with existing Python packages on your system, it is advisable to create a virtual environment within the cloned directory:
    ```bash
    python3 -m venv venv
    # Activate the virtual environment
    # On Windows
    venv\Scripts\activate
    # On macOS and Linux
    source venv/bin/activate
    ```
 
-3. **Install Dependencies**: Install all necessary Python packages using the provided `requirements.txt`:
+3. **Install Wheel File**: Install all necessary Python packages using the provided `AuotMLApp.whl` file or directly installing the python package:
    ```bash
-   pip install -r requirements.txt
+   pip install AutoMLApp
+   pip install "path to wheelfile"
    ```
 
-4. **Start the App**: After installing the dependencies, you can launch the AutoML Web App by executing:
+4. **Check Package**: After installing the package, you can see the properties by executing:
+   ```bash
+   pip show AutoMLApp
+   ```
+
+5. **Change the directory to Application's directory**: After copying the dependencies, you need to navigate to the AutoML Web App by executing:
+   ```bash
+   cd "copied location"
+   cd automlapp
+   ```
+
+6. **Start the App**: After installing the dependencies, you can launch the AutoML Web App by executing:
    ```bash
    streamlit run app.py
    ```
 
    This command initiates the app and should automatically open it in your default web browser. If the app does not open automatically, a URL will be displayed in your terminal, which you can use to access the app manually.
```

### Comparing `automlapp-0.1.71/automlapp/app.py` & `automlapp-0.1.72/automlapp/app.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/logo.png` & `automlapp-0.1.72/automlapp/logo.png`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/data_cleaning.py` & `automlapp-0.1.72/automlapp/modules/data_cleaning.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/data_input.py` & `automlapp-0.1.72/automlapp/modules/data_input.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/data_preprocessing.py` & `automlapp-0.1.72/automlapp/modules/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/data_summarization.py` & `automlapp-0.1.72/automlapp/modules/data_summarization.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/data_visualization.py` & `automlapp-0.1.72/automlapp/modules/data_visualization.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/data_woeiv.py` & `automlapp-0.1.72/automlapp/modules/data_woeiv.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/hyperparameter_tuning.py` & `automlapp-0.1.72/automlapp/modules/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/model_evaluation.py` & `automlapp-0.1.72/automlapp/modules/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/model_training.py` & `automlapp-0.1.72/automlapp/modules/model_training.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/modules/train_user_params.py` & `automlapp-0.1.72/automlapp/modules/train_user_params.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/automlapp/utils/streamlit_utils.py` & `automlapp-0.1.72/automlapp/utils/streamlit_utils.py`

 * *Files identical despite different names*

### Comparing `automlapp-0.1.71/setup.py` & `automlapp-0.1.72/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="AutoMLApp",
-    version="0.1.71",
-    author="Shivam Nikam",
+    version="0.1.72",
+    author="Think360.ai",
     author_email="shivam.nikam@think360.ai",
     description="An automated machine learning application designed for efficient model training, evaluation, and hyperparameter tuning.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     #url="https://github.com/YourGithub/AutoMLApp",
     packages=find_packages(),
     classifiers=[
@@ -23,26 +23,26 @@
         'streamlit==1.32.0',
         'streamlit-extras==0.4.0',
         'streamlit-modal==0.1.2',
         'plotly==5.18.0',
         'scikit-learn==1.4.1.post1',
         'lightgbm==4.3.0',
         'xgboost==2.0.3',
-        'openpyxl==3.0.10',
+        'openpyxl==3.1.0',
         'scorecardpy==0.1.9.7'  # Added to match your requirements.txt
     ],
-    extras_require={
-        "dev": [
-            "pytest>=5.2",
-            "check-manifest",
-            "twine",
-        ],
-    },
+    # extras_require={
+    #     "dev": [
+    #         "pytest>=5.2",
+    #         "check-manifest",
+    #         "twine",
+    #     ],
+    #},
     package_data={
         'automlapp': ['logo.png', 'runtool.bat'],  # Specify relative path to package root
     },
     entry_points={
         "console_scripts": [
             "fetchdir=automlapp.launcher:fetch",
         ],
     }
-)
+)
```


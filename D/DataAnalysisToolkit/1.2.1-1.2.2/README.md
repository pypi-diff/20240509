# Comparing `tmp/dataanalysistoolkit-1.2.1.tar.gz` & `tmp/dataanalysistoolkit-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataanalysistoolkit-1.2.1.tar", last modified: Mon May  6 20:50:57 2024, max compression
+gzip compressed data, was "dataanalysistoolkit-1.2.2.tar", max compression
```

## Comparing `dataanalysistoolkit-1.2.1.tar` & `dataanalysistoolkit-1.2.2.tar`

### file list

```diff
@@ -1,46 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.371404 dataanalysistoolkit-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-06 20:50:57.371404 dataanalysistoolkit-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:50:57.371404 dataanalysistoolkit-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.363404 dataanalysistoolkit-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/src/DataAnalysisToolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-06 20:50:57.000000 dataanalysistoolkit-1.2.1/src/DataAnalysisToolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-06 20:50:57.000000 dataanalysistoolkit-1.2.1/src/DataAnalysisToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:50:57.000000 dataanalysistoolkit-1.2.1/src/DataAnalysisToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 20:50:57.000000 dataanalysistoolkit-1.2.1/src/DataAnalysisToolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-06 20:50:57.000000 dataanalysistoolkit-1.2.1/src/DataAnalysisToolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.363404 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_analysis_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_sources/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_sources/api_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_sources/excel_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_sources/sql_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/formatters/data_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/generators/csv_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/generators/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/generators/report_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/integrators/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/integrators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/integrators/data_integrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/model/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/model/feature_engineer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/model/model_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/preprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/preprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/preprocessor/data_prep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/utils/data_imputer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/visualizer/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/visualizer/data_visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:50:57.367404 dataanalysistoolkit-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-06 20:50:42.000000 dataanalysistoolkit-1.2.1/tests/test_data_analysis_toolkit.py
+-rw-r--r--   0        0        0     4493 2024-05-09 04:56:11.129322 dataanalysistoolkit-1.2.2/README.md
+-rw-r--r--   0        0        0     2832 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      343 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/.conf/plot_config.json
+-rw-r--r--   0        0        0     3992 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/__init__.py
+-rw-r--r--   0        0        0    10814 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/data_analysis_toolkit.py
+-rw-r--r--   0        0        0      152 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/data_sources/__init__.py
+-rw-r--r--   0        0        0     4260 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/data_sources/api_connector.py
+-rw-r--r--   0        0        0     2768 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/data_sources/excel_connector.py
+-rw-r--r--   0        0        0     7654 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/data_sources/sql_connector.py
+-rw-r--r--   0        0        0       68 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/formatters/__init__.py
+-rw-r--r--   0        0        0     3784 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/formatters/data_formatter.py
+-rw-r--r--   0        0        0      157 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/generators/__init__.py
+-rw-r--r--   0        0        0     5810 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/generators/csv_data_generator.py
+-rw-r--r--   0        0        0     1777 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/generators/generate_data.py
+-rw-r--r--   0        0        0     4993 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/generators/report_generator.py
+-rw-r--r--   0        0        0       70 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/integrators/__init__.py
+-rw-r--r--   0        0        0     4769 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/integrators/data_integrator.py
+-rw-r--r--   0        0        0      112 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/model/__init__.py
+-rw-r--r--   0        0        0     2993 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/model/feature_engineer.py
+-rw-r--r--   0        0        0     3392 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/model/model_evaluator.py
+-rw-r--r--   0        0        0       68 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/preprocessor/__init__.py
+-rw-r--r--   0        0        0     2032 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/preprocessor/data_prep.py
+-rw-r--r--   0        0        0       58 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/utils/__init__.py
+-rw-r--r--   0        0        0     5297 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/utils/data_imputer.py
+-rw-r--r--   0        0        0       69 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/visualizer/__init__.py
+-rw-r--r--   0        0        0     8770 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/visualizer/data_visualizer.py
+-rw-r--r--   0        0        0    63515 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/tests/data/gen_test.csv
+-rw-r--r--   0        0        0     5365 2024-05-09 04:56:11.133322 dataanalysistoolkit-1.2.2/tests/data/test_random.csv
+-rw-r--r--   0        0        0     7675 1970-01-01 00:00:00.000000 dataanalysistoolkit-1.2.2/PKG-INFO
```

### Comparing `dataanalysistoolkit-1.2.1/README.md` & `dataanalysistoolkit-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/pyproject.toml` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,129 @@
-[build-system]
-requires = ["setuptools", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "DataAnalysisToolkit"
-dynamic = ["version"]
-description = "The DataAnalysisToolkit project is a Python-based data analysis tool designed to streamline various data analysis tasks. It allows users to load data from CSV files and perform operations such as statistical calculations, outlier detection, data cleaning, and visualization."
-authors = [
-    { name = "Thaddeus Thomas", email = "thaddeus.r.thomas@gmail.com" }
-]
-readme = "README.md"
-license = { file = "LICENSE" }
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
-    "Environment :: Console",
-    "Framework :: Jupyter",
-    "Intended Audience :: End Users/Desktop",
-    "Intended Audience :: Education",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: Scientific/Engineering :: Information Analysis"
-]
-requires-python = ">=3.8"
-keywords = ["data analysis", "CSV", "statistics", "data cleaning", "data visualization"]
-# include = ["src/**/*.py", "docs/**/*.md"]
-# exclude = ["tests/", "examples/"]
-dependencies = [
-    "backports.tarfile==1.1.1",
-    "build==1.2.1",
-    "certifi==2024.2.2",
-    "charset-normalizer==3.3.2",
-    "click==8.1.7",
-    "colorama==0.4.6",
-    "contourpy==1.2.1",
-    "cycler==0.12.1",
-    "docutils==0.21.2",
-    "fonttools==4.51.0",
-    "greenlet==3.0.3",
-    "idna==3.7",
-    "importlib_metadata==7.1.0",
-    "jaraco.classes==3.4.0",
-    "jaraco.context==5.3.0",
-    "jaraco.functools==4.0.1",
-    "joblib==1.4.2",
-    "keyring==25.2.0",
-    "kiwisolver==1.4.5",
-    "markdown-it-py==3.0.0",
-    "matplotlib==3.8.4",
-    "mdurl==0.1.2",
-    "more-itertools==10.2.0",
-    "nh3==0.2.17",
-    "nltk==3.8.1",
-    "numpy==1.26.4",
-    "packaging==24.0",
-    "pandas==2.2.2",
-    "pillow==10.3.0",
-    "pkginfo==1.10.0",
-    "Pygments==2.18.0",
-    "pyparsing==3.1.2",
-    "pyproject_hooks==1.1.0",
-    "python-dateutil==2.9.0.post0",
-    "pytz==2024.1",
-    "pywin32-ctypes==0.2.2",
-    "readme_renderer==43.0",
-    "regex==2024.4.28",
-    "requests==2.31.0",
-    "requests-toolbelt==1.0.0",
-    "rfc3986==2.0.0",
-    "rich==13.7.1",
-    "scikit-learn==1.4.2",
-    "scipy==1.13.0",
-    "seaborn==0.13.2",
-    "six==1.16.0",
-    "SQLAlchemy==2.0.30",
-    "threadpoolctl==3.5.0",
-    "tqdm==4.66.4",
-    "twine==5.0.0",
-    "typing_extensions==4.11.0",
-    "tzdata==2024.1",
-    "urllib3==2.2.1",
-    "zipp==3.18.1"
-]
+# __init__.py
+
+# MIT License
+#
+# Copyright (c) 2023 Thaddeus Thomas
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+# Metadata about the package
+__version__ = '1.2.2'
+__author__ = 'Thaddeus Thomas'
+__email__ = 'thaddeus@vcwtech.com'
+
+import logging
+import sys
+
+# Convenience imports for users
+from .data_analysis_toolkit import DataAnalysisToolkit
+from .utils import DataImputer
+from .model import FeatureEngineer, ModelEvaluator
+from .preprocessor import DataPreprocessor
+from .generators import ReportGenerator
+from .visualizer import DataVisualizer
+
+# Dependency checks
+required_packages = {
+    "certifi": "2024.2.2",
+    "charset-normalizer": "3.3.2",
+    "click": "8.1.7",
+    "colorama": "0.4.6",
+    "contourpy": "1.2.1",
+    "cycler": "0.12.1",
+    "docutils": "0.21.2",
+    "fonttools": "4.51.0",
+    "greenlet": "3.0.3",
+    "idna": "3.7",
+    "importlib_metadata": "7.1.0",
+    "joblib": "1.4.2",
+    "keyring": "25.2.0",
+    "kiwisolver": "1.4.5",
+    "markdown-it-py": "3.0.0",
+    "matplotlib": "3.8.4",
+    "mdurl": "0.1.2",
+    "more-itertools": "10.2.0",
+    "nh3": "0.2.17",
+    "nltk": "3.8.1",
+    "numpy": "1.26.4",
+    "packaging": "24.0",
+    "pandas": "2.2.2",
+    "pillow": "10.3.0",
+    "pkginfo": "1.10.0",
+    "Pygments": "2.18.0",
+    "pyparsing": "3.1.2",
+    "pyproject_hooks": "1.1.0",
+    "python-dateutil": "2.9.0.post0",
+    "pytz": "2024.1",
+    "pywin32-ctypes": "0.2.2",
+    "readme_renderer": "43.0",
+    "regex": "2024.4.28",
+    "requests": "2.31.0",
+    "requests-toolbelt": "1.0.0",
+    "rfc3986": "2.0.0",
+    "rich": "13.7.1",
+    "scikit-learn": "1.4.2",
+    "scipy": "1.13.0",
+    "seaborn": "0.13.2",
+    "six": "1.16.0",
+    "SQLAlchemy": "2.0.30",
+    "threadpoolctl": "3.5.0",
+    "tqdm": "4.66.4",
+    "typing_extensions": "4.11.0",
+    "tzdata": "2024.1",
+    "urllib3": "2.2.1",
+    "zipp": "3.18.1",
+}
 
-[project.optional-dependencies]
-dev = ["pytest", "pytest-mock", "check-manifest"]
-docs = ["myst-parser", "sphinx", "nbsphinx", "sphinx-rtd-theme", "sphinxcontrib-websupport"]
-
-[tool.setuptools.dynamic]
-version = {attr = "dataanalysistoolkit.__version__"}
-
-[project.urls]
-Repository = "https://github.com/thomasthaddeus/dataanalysistoolkit"
-Issues = "https://github.com/thomasthaddeus/dataanalysistoolkit/issues"
-Documentation = "https://dataanalysistoolkit.readthedocs.io/en/latest/"
+missing_packages = []
+
+# for lib, version in required_packages.items():
+#     try:
+#         pkg = __import__(lib)
+#         # Safely get the version or None if not available
+#         pkg_version = getattr(pkg, __version__, None)
+#         if not pkg_version or pkg_version < version:
+#             missing_packages.append(f"{lib}>= {version}")
+#     except ImportError:
+#         missing_packages.append(f"{lib}>= {version}")
+
+if missing_packages:
+    sys.exit("Missing required packages: " + ', '.join(missing_packages))
+
+# Configure logging
+logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
+
+logger.info("Initializing DataAnalysisToolkit package")
+
+# Initialization code that runs on package import, if any
+def _init_package():
+    # Put any package-wide initialization logic here
+    logger.debug("Package initialized successfully")
+
+_init_package()
+
+# Ensure that this module only exposes the intended public interface
+__all__ = [
+    "DataAnalysisToolkit",
+    "DataImputer",
+    "DataVisualizer",
+    "FeatureEngineer",
+    "ModelEvaluator",
+    "DataPreprocessor",
+    "ReportGenerator"
+]
```

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_analysis_toolkit.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/data_analysis_toolkit.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_sources/api_connector.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/data_sources/api_connector.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_sources/excel_connector.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/data_sources/excel_connector.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/data_sources/sql_connector.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/data_sources/sql_connector.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/formatters/data_formatter.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/formatters/data_formatter.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/generators/csv_data_generator.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/generators/csv_data_generator.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/generators/generate_data.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/generators/generate_data.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/generators/report_generator.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/generators/report_generator.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/integrators/data_integrator.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/integrators/data_integrator.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/model/feature_engineer.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/model/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/model/model_evaluator.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/model/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/preprocessor/data_prep.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/preprocessor/data_prep.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/utils/data_imputer.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/utils/data_imputer.py`

 * *Files identical despite different names*

### Comparing `dataanalysistoolkit-1.2.1/src/dataanalysistoolkit/visualizer/data_visualizer.py` & `dataanalysistoolkit-1.2.2/src/dataanalysistoolkit/visualizer/data_visualizer.py`

 * *Files identical despite different names*


# Comparing `tmp/autoviml-0.1.721.tar.gz` & `tmp/autoviml-0.1.722.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviml-0.1.721.tar", last modified: Tue May  7 11:44:14 2024, max compression
+gzip compressed data, was "autoviml-0.1.722.tar", last modified: Thu May  9 11:12:50 2024, max compression
```

## Comparing `autoviml-0.1.721.tar` & `autoviml-0.1.722.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-07 11:44:14.529837 autoviml-0.1.721/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11558 2023-03-07 03:28:42.000000 autoviml-0.1.721/LICENSE
--rwxrwxrwx   0 ram       (1000) ram       (1000)    13936 2024-05-07 11:44:14.514216 autoviml-0.1.721/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    13180 2024-05-06 12:07:37.000000 autoviml-0.1.721/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-07 11:44:14.404836 autoviml-0.1.721/autoviml/
--rwxrwxrwx   0 ram       (1000) ram       (1000)   102454 2024-05-06 12:07:37.000000 autoviml-0.1.721/autoviml/Auto_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   336710 2024-05-07 11:26:46.000000 autoviml-0.1.721/autoviml/Auto_ViML.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12981 2024-05-06 12:07:38.000000 autoviml-0.1.721/autoviml/QuickML_Ensembling.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    10750 2024-05-06 12:07:38.000000 autoviml-0.1.721/autoviml/QuickML_Stacking.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     6703 2024-05-06 12:07:38.000000 autoviml-0.1.721/autoviml/Transform_KM_Features.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1798 2024-05-06 13:22:49.000000 autoviml-0.1.721/autoviml/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      411 2024-05-07 11:43:32.000000 autoviml-0.1.721/autoviml/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    18694 2024-05-06 12:07:38.000000 autoviml-0.1.721/autoviml/classify_method.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     4767 2024-05-06 12:07:38.000000 autoviml-0.1.721/autoviml/custom_scores.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     8277 2024-05-06 12:07:38.000000 autoviml-0.1.721/autoviml/custom_scores_HO.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    29284 2024-05-06 12:44:52.000000 autoviml-0.1.721/autoviml/feature_engineering.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    15179 2024-05-06 12:37:45.000000 autoviml-0.1.721/autoviml/sulov_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-07 11:44:14.514216 autoviml-0.1.721/autoviml.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    13936 2024-05-07 11:44:13.000000 autoviml-0.1.721/autoviml.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      517 2024-05-07 11:44:13.000000 autoviml-0.1.721/autoviml.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2024-05-07 11:44:13.000000 autoviml-0.1.721/autoviml.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      261 2024-05-07 11:44:13.000000 autoviml-0.1.721/autoviml.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        9 2024-05-07 11:44:13.000000 autoviml-0.1.721/autoviml.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2024-05-07 11:44:14.529837 autoviml-0.1.721/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1240 2024-05-07 11:43:13.000000 autoviml-0.1.721/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 11:12:50.738192 autoviml-0.1.722/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11558 2023-03-07 03:28:42.000000 autoviml-0.1.722/LICENSE
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    13944 2024-05-09 11:12:50.738192 autoviml-0.1.722/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    13180 2024-05-06 12:07:37.000000 autoviml-0.1.722/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 11:12:50.537624 autoviml-0.1.722/autoviml/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   102454 2024-05-06 12:07:37.000000 autoviml-0.1.722/autoviml/Auto_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   336710 2024-05-07 11:26:46.000000 autoviml-0.1.722/autoviml/Auto_ViML.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    12981 2024-05-06 12:07:38.000000 autoviml-0.1.722/autoviml/QuickML_Ensembling.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    10750 2024-05-06 12:07:38.000000 autoviml-0.1.722/autoviml/QuickML_Stacking.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     6703 2024-05-06 12:07:38.000000 autoviml-0.1.722/autoviml/Transform_KM_Features.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1798 2024-05-06 13:22:49.000000 autoviml-0.1.722/autoviml/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      411 2024-05-09 11:10:59.000000 autoviml-0.1.722/autoviml/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    18694 2024-05-06 12:07:38.000000 autoviml-0.1.722/autoviml/classify_method.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     4767 2024-05-06 12:07:38.000000 autoviml-0.1.722/autoviml/custom_scores.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     8277 2024-05-06 12:07:38.000000 autoviml-0.1.722/autoviml/custom_scores_HO.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    29284 2024-05-06 12:44:52.000000 autoviml-0.1.722/autoviml/feature_engineering.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15179 2024-05-06 12:37:45.000000 autoviml-0.1.722/autoviml/sulov_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2024-05-09 11:12:50.722568 autoviml-0.1.722/autoviml.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    13944 2024-05-09 11:12:49.000000 autoviml-0.1.722/autoviml.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      517 2024-05-09 11:12:49.000000 autoviml-0.1.722/autoviml.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2024-05-09 11:12:49.000000 autoviml-0.1.722/autoviml.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      269 2024-05-09 11:12:49.000000 autoviml-0.1.722/autoviml.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        9 2024-05-09 11:12:49.000000 autoviml-0.1.722/autoviml.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2024-05-09 11:12:50.753824 autoviml-0.1.722/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1248 2024-05-09 11:10:42.000000 autoviml-0.1.722/setup.py
```

### Comparing `autoviml-0.1.721/LICENSE` & `autoviml-0.1.722/LICENSE`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/PKG-INFO` & `autoviml-0.1.722/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: autoviml
-Version: 0.1.721
+Version: 0.1.722
 Summary: Automatically Build Variant Interpretable ML models fast - now with CatBoost!
 Home-page: https://github.com/AutoViML/Auto_ViML
 Author: Ram Seshadri
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<=1.19.5
+Requires-Dist: numpy>=1.24
 Requires-Dist: pandas<2.0,>=1.1.3
 Requires-Dist: xlrd
-Requires-Dist: matplotlib
+Requires-Dist: matplotlib>3.7.4
 Requires-Dist: beautifulsoup4
 Requires-Dist: emoji
 Requires-Dist: ipython
 Requires-Dist: jupyter
 Requires-Dist: seaborn
 Requires-Dist: catboost
 Requires-Dist: textblob
 Requires-Dist: nltk
 Requires-Dist: regex
-Requires-Dist: xgboost<=1.6.2
+Requires-Dist: xgboost<1.7,>=0.82
 Requires-Dist: vaderSentiment
 Requires-Dist: imbalanced-learn>=0.10.1
 Requires-Dist: shap>=0.36.0
 Requires-Dist: imbalanced_ensemble>=0.2.0
 Requires-Dist: scikit-learn<=1.2.2,>=0.24
 Requires-Dist: lightgbm>=3.0.0
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: autoviml Version: 0.1.721 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviml Version: 0.1.722 Summary: Automatically
 Build Variant Interpretable ML models fast - now with CatBoost! Home-page:
 https://github.com/AutoViML/Auto_ViML Author: Ram Seshadri License: Apache
 License 2.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: numpy<=1.19.5 Requires-Dist:
-pandas<2.0,>=1.1.3 Requires-Dist: xlrd Requires-Dist: matplotlib Requires-Dist:
-beautifulsoup4 Requires-Dist: emoji Requires-Dist: ipython Requires-Dist:
-jupyter Requires-Dist: seaborn Requires-Dist: catboost Requires-Dist: textblob
-Requires-Dist: nltk Requires-Dist: regex Requires-Dist: xgboost<=1.6.2
-Requires-Dist: vaderSentiment Requires-Dist: imbalanced-learn>=0.10.1 Requires-
-Dist: shap>=0.36.0 Requires-Dist: imbalanced_ensemble>=0.2.0 Requires-Dist:
-scikit-learn<=1.2.2,>=0.24 Requires-Dist: lightgbm>=3.0.0 # Auto-ViML ![banner]
-(logo.png)
+License-File: LICENSE Requires-Dist: numpy>=1.24 Requires-Dist:
+pandas<2.0,>=1.1.3 Requires-Dist: xlrd Requires-Dist: matplotlib>3.7.4
+Requires-Dist: beautifulsoup4 Requires-Dist: emoji Requires-Dist: ipython
+Requires-Dist: jupyter Requires-Dist: seaborn Requires-Dist: catboost Requires-
+Dist: textblob Requires-Dist: nltk Requires-Dist: regex Requires-Dist:
+xgboost<1.7,>=0.82 Requires-Dist: vaderSentiment Requires-Dist: imbalanced-
+learn>=0.10.1 Requires-Dist: shap>=0.36.0 Requires-Dist:
+imbalanced_ensemble>=0.2.0 Requires-Dist: scikit-learn<=1.2.2,>=0.24 Requires-
+Dist: lightgbm>=3.0.0 # Auto-ViML ![banner](logo.png)
 Automatically Build Various Interpretable ML models fast!
 [![Downloads](https://pepy.tech/badge/autoviml/week)](https://pepy.tech/
 project/autoviml/week) [![Downloads](https://pepy.tech/badge/autoviml/month)]
 (https://pepy.tech/project/autoviml/month) [![Downloads](https://pepy.tech/
 badge/autoviml)](https://pepy.tech/project/autoviml) [![standard-readme
 compliant](https://img.shields.io/badge/standard--readme-OK-
 green.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
```

### Comparing `autoviml-0.1.721/README.md` & `autoviml-0.1.722/README.md`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/Auto_NLP.py` & `autoviml-0.1.722/autoviml/Auto_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/Auto_ViML.py` & `autoviml-0.1.722/autoviml/Auto_ViML.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/QuickML_Ensembling.py` & `autoviml-0.1.722/autoviml/QuickML_Ensembling.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/QuickML_Stacking.py` & `autoviml-0.1.722/autoviml/QuickML_Stacking.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/Transform_KM_Features.py` & `autoviml-0.1.722/autoviml/Transform_KM_Features.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/__init__.py` & `autoviml-0.1.722/autoviml/__init__.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/classify_method.py` & `autoviml-0.1.722/autoviml/classify_method.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/custom_scores.py` & `autoviml-0.1.722/autoviml/custom_scores.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/custom_scores_HO.py` & `autoviml-0.1.722/autoviml/custom_scores_HO.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/feature_engineering.py` & `autoviml-0.1.722/autoviml/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml/sulov_method.py` & `autoviml-0.1.722/autoviml/sulov_method.py`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/autoviml.egg-info/PKG-INFO` & `autoviml-0.1.722/autoviml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: autoviml
-Version: 0.1.721
+Version: 0.1.722
 Summary: Automatically Build Variant Interpretable ML models fast - now with CatBoost!
 Home-page: https://github.com/AutoViML/Auto_ViML
 Author: Ram Seshadri
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy<=1.19.5
+Requires-Dist: numpy>=1.24
 Requires-Dist: pandas<2.0,>=1.1.3
 Requires-Dist: xlrd
-Requires-Dist: matplotlib
+Requires-Dist: matplotlib>3.7.4
 Requires-Dist: beautifulsoup4
 Requires-Dist: emoji
 Requires-Dist: ipython
 Requires-Dist: jupyter
 Requires-Dist: seaborn
 Requires-Dist: catboost
 Requires-Dist: textblob
 Requires-Dist: nltk
 Requires-Dist: regex
-Requires-Dist: xgboost<=1.6.2
+Requires-Dist: xgboost<1.7,>=0.82
 Requires-Dist: vaderSentiment
 Requires-Dist: imbalanced-learn>=0.10.1
 Requires-Dist: shap>=0.36.0
 Requires-Dist: imbalanced_ensemble>=0.2.0
 Requires-Dist: scikit-learn<=1.2.2,>=0.24
 Requires-Dist: lightgbm>=3.0.0
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: autoviml Version: 0.1.721 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviml Version: 0.1.722 Summary: Automatically
 Build Variant Interpretable ML models fast - now with CatBoost! Home-page:
 https://github.com/AutoViML/Auto_ViML Author: Ram Seshadri License: Apache
 License 2.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: numpy<=1.19.5 Requires-Dist:
-pandas<2.0,>=1.1.3 Requires-Dist: xlrd Requires-Dist: matplotlib Requires-Dist:
-beautifulsoup4 Requires-Dist: emoji Requires-Dist: ipython Requires-Dist:
-jupyter Requires-Dist: seaborn Requires-Dist: catboost Requires-Dist: textblob
-Requires-Dist: nltk Requires-Dist: regex Requires-Dist: xgboost<=1.6.2
-Requires-Dist: vaderSentiment Requires-Dist: imbalanced-learn>=0.10.1 Requires-
-Dist: shap>=0.36.0 Requires-Dist: imbalanced_ensemble>=0.2.0 Requires-Dist:
-scikit-learn<=1.2.2,>=0.24 Requires-Dist: lightgbm>=3.0.0 # Auto-ViML ![banner]
-(logo.png)
+License-File: LICENSE Requires-Dist: numpy>=1.24 Requires-Dist:
+pandas<2.0,>=1.1.3 Requires-Dist: xlrd Requires-Dist: matplotlib>3.7.4
+Requires-Dist: beautifulsoup4 Requires-Dist: emoji Requires-Dist: ipython
+Requires-Dist: jupyter Requires-Dist: seaborn Requires-Dist: catboost Requires-
+Dist: textblob Requires-Dist: nltk Requires-Dist: regex Requires-Dist:
+xgboost<1.7,>=0.82 Requires-Dist: vaderSentiment Requires-Dist: imbalanced-
+learn>=0.10.1 Requires-Dist: shap>=0.36.0 Requires-Dist:
+imbalanced_ensemble>=0.2.0 Requires-Dist: scikit-learn<=1.2.2,>=0.24 Requires-
+Dist: lightgbm>=3.0.0 # Auto-ViML ![banner](logo.png)
 Automatically Build Various Interpretable ML models fast!
 [![Downloads](https://pepy.tech/badge/autoviml/week)](https://pepy.tech/
 project/autoviml/week) [![Downloads](https://pepy.tech/badge/autoviml/month)]
 (https://pepy.tech/project/autoviml/month) [![Downloads](https://pepy.tech/
 badge/autoviml)](https://pepy.tech/project/autoviml) [![standard-readme
 compliant](https://img.shields.io/badge/standard--readme-OK-
 green.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
```

### Comparing `autoviml-0.1.721/autoviml.egg-info/SOURCES.txt` & `autoviml-0.1.722/autoviml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoviml-0.1.721/setup.py` & `autoviml-0.1.722/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autoviml",
-    version="0.1.721",
+    version="0.1.722",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Build Variant Interpretable ML models fast - now with CatBoost!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/Auto_ViML",
     packages=setuptools.find_packages(exclude=("tests",)),
     install_requires=[
-        "numpy<=1.19.5",
+        "numpy>=1.24",
         "pandas>=1.1.3, <2.0",
         "xlrd",
-        "matplotlib",
+        "matplotlib>3.7.4",
         "beautifulsoup4",
         "emoji",
         "ipython",
         "jupyter",
         "seaborn",
         "catboost",
         "textblob",
         "nltk",
         "regex",
-        "xgboost<=1.6.2",
+        "xgboost>=0.82,<1.7",
         "vaderSentiment",
         "imbalanced-learn>=0.10.1",
         "shap>=0.36.0",
         "imbalanced_ensemble>=0.2.0",
         "scikit-learn>=0.24,<=1.2.2",
         "lightgbm>=3.0.0",
     ],
```


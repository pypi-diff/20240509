# Comparing `tmp/e-models-1.8.8.1.tar.gz` & `tmp/e-models-1.8.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.8.8.1.tar", last modified: Tue Apr 16 18:24:11 2024, max compression
+gzip compressed data, was "e-models-1.8.8.2.tar", last modified: Thu May  9 17:34:48 2024, max compression
```

## Comparing `e-models-1.8.8.1.tar` & `e-models-1.8.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 18:24:11.411363 e-models-1.8.8.1/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.8.8.1/LICENSE
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-04-16 18:24:11.411363 e-models-1.8.8.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12478 2024-02-27 17:55:52.000000 e-models-1.8.8.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 18:24:11.403362 e-models-1.8.8.1/e_models.egg-info/
--rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-04-16 18:24:11.000000 e-models-1.8.8.1/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-04-16 18:24:11.000000 e-models-1.8.8.1/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-04-16 18:24:11.000000 e-models-1.8.8.1/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-04-16 18:24:11.000000 e-models-1.8.8.1/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-04-16 18:24:11.000000 e-models-1.8.8.1/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 18:24:11.403362 e-models-1.8.8.1/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2024-04-16 18:23:39.000000 e-models-1.8.8.1/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      340 2023-11-06 19:18:12.000000 e-models-1.8.8.1/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 18:24:11.407363 e-models-1.8.8.1/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.8.8.1/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e-models-1.8.8.1/emodels/datasets/hugging.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    21262 2024-04-16 18:22:34.000000 e-models-1.8.8.1/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e-models-1.8.8.1/emodels/datasets/stypes.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e-models-1.8.8.1/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e-models-1.8.8.1/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 18:24:11.407363 e-models-1.8.8.1/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.8.8.1/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.8.8.1/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.8.8.1/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.8.8.1/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.8.8.1/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.8.8.1/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 18:24:11.407363 e-models-1.8.8.1/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e-models-1.8.8.1/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4734 2024-02-27 12:04:53.000000 e-models-1.8.8.1/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e-models-1.8.8.1/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.8.8.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-04-16 18:24:11.411363 e-models-1.8.8.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1088 2024-04-16 18:23:29.000000 e-models-1.8.8.1/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-04-16 18:24:11.407363 e-models-1.8.8.1/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e-models-1.8.8.1/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e-models-1.8.8.1/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.579804 e-models-1.8.8.2/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.8.8.2/LICENSE
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-05-09 17:34:48.579804 e-models-1.8.8.2/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12478 2024-02-27 17:55:52.000000 e-models-1.8.8.2/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.571804 e-models-1.8.8.2/e_models.egg-info/
+-rw-r--r--   0 molveyra  (1001) molveyra  (1001)    13332 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      710 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      104 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2024-05-09 17:34:48.000000 e-models-1.8.8.2/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2024-05-09 17:30:26.000000 e-models-1.8.8.2/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      340 2023-11-06 19:18:12.000000 e-models-1.8.8.2/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.8.8.2/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    16404 2023-11-03 19:09:54.000000 e-models-1.8.8.2/emodels/datasets/hugging.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    21433 2024-04-18 23:00:27.000000 e-models-1.8.8.2/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      374 2023-08-31 18:27:15.000000 e-models-1.8.8.2/emodels/datasets/stypes.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2299 2024-03-14 19:03:35.000000 e-models-1.8.8.2/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12361 2024-03-18 21:52:08.000000 e-models-1.8.8.2/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.8.8.2/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.8.8.2/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-08-04 13:47:09.000000 e-models-1.8.8.2/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4734 2024-02-27 12:04:53.000000 e-models-1.8.8.2/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6339 2024-02-27 17:16:48.000000 e-models-1.8.8.2/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.8.8.2/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2024-05-09 17:34:48.579804 e-models-1.8.8.2/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1088 2024-05-09 17:30:09.000000 e-models-1.8.8.2/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2024-05-09 17:34:48.575804 e-models-1.8.8.2/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6355 2023-08-04 13:47:35.000000 e-models-1.8.8.2/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12999 2024-02-27 17:16:48.000000 e-models-1.8.8.2/tests/test_scrapyutils.py
```

### Comparing `e-models-1.8.8.1/LICENSE` & `e-models-1.8.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/PKG-INFO` & `e-models-1.8.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.8.1
+Version: 1.8.8.2
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.8.8.1/README.md` & `e-models-1.8.8.2/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/e_models.egg-info/PKG-INFO` & `e-models-1.8.8.2/e_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.8.8.1
+Version: 1.8.8.2
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.8.8.1/e_models.egg-info/SOURCES.txt` & `e-models-1.8.8.2/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/emodels/datasets/hugging.py` & `e-models-1.8.8.2/emodels/datasets/hugging.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/emodels/datasets/models.py` & `e-models-1.8.8.2/emodels/datasets/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,28 +142,31 @@
         obj.Y_train = df_Y_train
         obj.Y_test = df_Y_test
 
         return obj
 
 
 class ModelWithDataset(Generic[SAMPLE, E], ABC):
-    FSHELPER: FSHelper | None = None
     datasets: DatasetsPandas[E] | None = None
 
     scraped_samples: Dict[DatasetBucket, DatasetFilename[SAMPLE]] = dict()
     scraped_label: str
 
+    FSHELPER: FSHelper | None = None
     dataset_repository: DatasetFilename[E]
     features: Tuple[str, ...]
 
     target_label: str
     project: str
     _self: Self | None = None
 
     def __new__(cls):
+        """
+        Ensure singleton per class
+        """
         if cls._self is None:
             cls._self = super().__new__(cls)
         return cls._self
 
     @classmethod
     @abstractmethod
     def build_fshelper(cls, settings) -> FSHelper:
@@ -207,40 +210,43 @@
     @classmethod
     def get_dataset(cls) -> DatasetsPandas[E]:
         if cls.datasets is None:
             cls.datasets = cls.load_dataset()
         return cls.datasets
 
     @classmethod
-    def reset(cls):
+    def reset_datasets(cls):
         cls.delete_model_files(cls.dataset_repository)
+        cls.datasets = None
+
+    @classmethod
+    def reset(cls):
+        cls.reset_datasets()
 
     @classmethod
     def delete_model_files(cls, repository: Filename):
         for fname in (repository, repository.local(cls.project)):
-            try:
+            if cls._fshelper().exists(fname):
                 cls._fshelper().rm_file(fname)
                 LOGGER.info(f"Deleted {fname}")
-            except FileNotFoundError:
-                pass
 
     @classmethod
     def get_row_from_sample(cls, sample: SAMPLE) -> pd.Series:
         sd: E = cls.get_sample_data_from_sample(sample)
         return pd.Series(sd)
 
     @classmethod
     @abstractmethod
     def get_sample_data_from_sample(cls, sample: SAMPLE) -> E:
         ...
 
     @classmethod
     def append_sample(cls, sample: SAMPLE, bucket: DatasetBucket):
         """
-        Add sample to the specified dataset in cls.scraped_samples list.
+        Add sample (SAMPLE) to the specified scraped dataset in cls.scraped_samples list.
         """
         dsample = cls.get_sample_data_from_sample(sample)
         cls._check_sample(dsample)
         cls.scraped_samples[bucket].append(sample)
 
     @classmethod
     def rebalance_samples(cls, bucket: DatasetBucket):
@@ -309,15 +315,15 @@
             cls.vectorizer = cls.load_vectorizer()
         return cls.vectorizer
 
     @classmethod
     def reset(cls):
         if hasattr(cls, "vectorizer_repository"):
             cls.delete_model_files(cls.vectorizer_repository)
-            cls.vectorizer = None
+        cls.vectorizer = None
         super().reset()
 
     @classmethod
     @abstractmethod
     def get_features_from_dataframe_row(cls, row: pd.Series) -> Tuple[DF]:
         """
         The most common implementation is just:
@@ -450,14 +456,15 @@
     def instance_new_lowlevel_model(cls) -> M:
         ...
 
     @classmethod
     def reset(cls):
         """Remove datasets and model files, so a retrain will be forced."""
         cls.delete_model_files(cls.model_repository)
+        cls.model = None
         super().reset()
 
 
 class ClassifierModel(Generic[SAMPLE, E, M], TrainableModel[SAMPLE, E, M], ModelWithDataset[SAMPLE, E]):
     @classmethod
     @abstractmethod
     def classify_from_row(cls, row: pd.Series, proba: int = -1) -> float:
```

### Comparing `e-models-1.8.8.1/emodels/datasets/tokenizers.py` & `e-models-1.8.8.2/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/emodels/datasets/utils.py` & `e-models-1.8.8.2/emodels/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/emodels/html2text/__init__.py` & `e-models-1.8.8.2/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/emodels/html2text/config.py` & `e-models-1.8.8.2/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/emodels/html2text/utils.py` & `e-models-1.8.8.2/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/emodels/scrapyutils/loader.py` & `e-models-1.8.8.2/emodels/scrapyutils/loader.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/emodels/scrapyutils/response.py` & `e-models-1.8.8.2/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/setup.py` & `e-models-1.8.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.8.8.1',
+    version      = '1.8.8.2',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
```

### Comparing `e-models-1.8.8.1/tests/test_html2text.py` & `e-models-1.8.8.2/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.8.8.1/tests/test_scrapyutils.py` & `e-models-1.8.8.2/tests/test_scrapyutils.py`

 * *Files identical despite different names*


# Comparing `tmp/saf_nlp-0.5.0.tar.gz` & `tmp/saf_nlp-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saf_nlp-0.5.0.tar", last modified: Wed May  8 14:07:48 2024, max compression
+gzip compressed data, was "saf_nlp-0.5.1.tar", last modified: Thu May  9 15:24:47 2024, max compression
```

## Comparing `saf_nlp-0.5.0.tar` & `saf_nlp-0.5.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.778972 saf_nlp-0.5.0/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)    35141 2023-03-13 13:27:52.000000 saf_nlp-0.5.0/LICENSE
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4842 2024-05-08 14:07:48.778805 saf_nlp-0.5.0/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4244 2024-05-08 13:01:03.000000 saf_nlp-0.5.0/README.md
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      569 2024-05-08 14:04:57.000000 saf_nlp-0.5.0/pyproject.toml
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.771931 saf_nlp-0.5.0/saf/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      321 2024-02-12 13:42:33.000000 saf_nlp-0.5.0/saf/__init__.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.772363 saf_nlp-0.5.0/saf/annotators/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      106 2022-08-02 17:53:18.000000 saf_nlp-0.5.0/saf/annotators/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      847 2024-05-07 13:50:23.000000 saf_nlp-0.5.0/saf/annotators/annotator.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.772870 saf_nlp-0.5.0/saf/constants/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       61 2022-08-02 17:53:18.000000 saf_nlp-0.5.0/saf/constants/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     2178 2024-05-07 13:52:47.000000 saf_nlp-0.5.0/saf/constants/annotation.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.774617 saf_nlp-0.5.0/saf/data_model/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       34 2022-08-02 17:53:18.000000 saf_nlp-0.5.0/saf/data_model/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      449 2023-03-10 13:16:53.000000 saf_nlp-0.5.0/saf/data_model/annotable.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      987 2023-11-29 15:50:35.000000 saf_nlp-0.5.0/saf/data_model/document.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1263 2024-05-07 14:00:48.000000 saf_nlp-0.5.0/saf/data_model/sentence.py
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      609 2024-02-09 14:43:07.000000 saf_nlp-0.5.0/saf/data_model/sequence.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      653 2023-11-29 15:50:25.000000 saf_nlp-0.5.0/saf/data_model/term.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      509 2023-11-29 15:47:20.000000 saf_nlp-0.5.0/saf/data_model/token.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     7156 2023-08-21 12:13:33.000000 saf_nlp-0.5.0/saf/data_model/vocabulary.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.775308 saf_nlp-0.5.0/saf/formatters/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       34 2022-08-02 17:53:18.000000 saf_nlp-0.5.0/saf/formatters/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     3986 2024-05-07 21:57:53.000000 saf_nlp-0.5.0/saf/formatters/conll.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      908 2024-05-07 21:59:40.000000 saf_nlp-0.5.0/saf/formatters/plain.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.776772 saf_nlp-0.5.0/saf/importers/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      181 2024-05-08 12:35:23.000000 saf_nlp-0.5.0/saf/importers/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     3104 2024-05-08 12:22:11.000000 saf_nlp-0.5.0/saf/importers/conll.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     1342 2024-05-07 16:10:50.000000 saf_nlp-0.5.0/saf/importers/importer.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     2284 2024-05-07 20:51:46.000000 saf_nlp-0.5.0/saf/importers/morphodb.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      848 2024-05-08 12:19:40.000000 saf_nlp-0.5.0/saf/importers/plain.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.777129 saf_nlp-0.5.0/saf/importers/tokenizers/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       34 2022-08-02 17:53:18.000000 saf_nlp-0.5.0/saf/importers/tokenizers/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)      292 2022-08-02 17:53:18.000000 saf_nlp-0.5.0/saf/importers/tokenizers/conll.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     2599 2024-05-08 12:19:51.000000 saf_nlp-0.5.0/saf/importers/webanno.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.777812 saf_nlp-0.5.0/saf/test/
--rw-------   0 dsilvadecarvalho   (505) staff       (20)       34 2022-08-02 17:53:18.000000 saf_nlp-0.5.0/saf/test/__init__.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     5110 2022-08-02 17:53:18.000000 saf_nlp-0.5.0/saf/test/test_formatters.py
--rw-------   0 dsilvadecarvalho   (505) staff       (20)     4364 2022-08-02 17:53:18.000000 saf_nlp-0.5.0/saf/test/test_importers.py
-drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-08 14:07:48.778621 saf_nlp-0.5.0/saf_nlp.egg-info/
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     4842 2024-05-08 14:07:48.000000 saf_nlp-0.5.0/saf_nlp.egg-info/PKG-INFO
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      903 2024-05-08 14:07:48.000000 saf_nlp-0.5.0/saf_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-08 14:07:48.000000 saf_nlp-0.5.0/saf_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       11 2024-05-08 14:07:48.000000 saf_nlp-0.5.0/saf_nlp.egg-info/requires.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        4 2024-05-08 14:07:48.000000 saf_nlp-0.5.0/saf_nlp.egg-info/top_level.txt
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-08 14:07:48.779013 saf_nlp-0.5.0/setup.cfg
--rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      468 2024-05-08 14:05:52.000000 saf_nlp-0.5.0/setup.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.389062 saf_nlp-0.5.1/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)    35141 2023-03-13 13:27:52.000000 saf_nlp-0.5.1/LICENSE
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     7218 2024-05-09 15:24:47.388883 saf_nlp-0.5.1/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     6524 2024-05-09 15:15:09.000000 saf_nlp-0.5.1/README.md
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      641 2024-05-09 13:53:41.000000 saf_nlp-0.5.1/pyproject.toml
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.379335 saf_nlp-0.5.1/saf/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      321 2024-02-12 13:42:33.000000 saf_nlp-0.5.1/saf/__init__.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.379984 saf_nlp-0.5.1/saf/annotators/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      106 2022-08-02 17:53:18.000000 saf_nlp-0.5.1/saf/annotators/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      847 2024-05-07 13:50:23.000000 saf_nlp-0.5.1/saf/annotators/annotator.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.380655 saf_nlp-0.5.1/saf/constants/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       61 2022-08-02 17:53:18.000000 saf_nlp-0.5.1/saf/constants/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     2178 2024-05-07 13:52:47.000000 saf_nlp-0.5.1/saf/constants/annotation.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.382870 saf_nlp-0.5.1/saf/data_model/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       34 2022-08-02 17:53:18.000000 saf_nlp-0.5.1/saf/data_model/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      449 2023-03-10 13:16:53.000000 saf_nlp-0.5.1/saf/data_model/annotable.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      987 2023-11-29 15:50:35.000000 saf_nlp-0.5.1/saf/data_model/document.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     1263 2024-05-07 14:00:48.000000 saf_nlp-0.5.1/saf/data_model/sentence.py
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      609 2024-02-09 14:43:07.000000 saf_nlp-0.5.1/saf/data_model/sequence.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      653 2023-11-29 15:50:25.000000 saf_nlp-0.5.1/saf/data_model/term.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      509 2023-11-29 15:47:20.000000 saf_nlp-0.5.1/saf/data_model/token.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     7156 2023-08-21 12:13:33.000000 saf_nlp-0.5.1/saf/data_model/vocabulary.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.383855 saf_nlp-0.5.1/saf/formatters/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       34 2022-08-02 17:53:18.000000 saf_nlp-0.5.1/saf/formatters/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     3986 2024-05-07 21:57:53.000000 saf_nlp-0.5.1/saf/formatters/conll.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      908 2024-05-07 21:59:40.000000 saf_nlp-0.5.1/saf/formatters/plain.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.385756 saf_nlp-0.5.1/saf/importers/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      181 2024-05-08 12:35:23.000000 saf_nlp-0.5.1/saf/importers/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     3104 2024-05-08 12:22:11.000000 saf_nlp-0.5.1/saf/importers/conll.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     1342 2024-05-07 16:10:50.000000 saf_nlp-0.5.1/saf/importers/importer.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     2284 2024-05-07 20:51:46.000000 saf_nlp-0.5.1/saf/importers/morphodb.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      848 2024-05-08 12:19:40.000000 saf_nlp-0.5.1/saf/importers/plain.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.386254 saf_nlp-0.5.1/saf/importers/tokenizers/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       34 2022-08-02 17:53:18.000000 saf_nlp-0.5.1/saf/importers/tokenizers/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)      292 2022-08-02 17:53:18.000000 saf_nlp-0.5.1/saf/importers/tokenizers/conll.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     2599 2024-05-08 12:19:51.000000 saf_nlp-0.5.1/saf/importers/webanno.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.387804 saf_nlp-0.5.1/saf/test/
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)       34 2022-08-02 17:53:18.000000 saf_nlp-0.5.1/saf/test/__init__.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     5110 2022-08-02 17:53:18.000000 saf_nlp-0.5.1/saf/test/test_formatters.py
+-rw-------   0 dsilvadecarvalho   (505) staff       (20)     4364 2022-08-02 17:53:18.000000 saf_nlp-0.5.1/saf/test/test_importers.py
+drwxr-xr-x   0 dsilvadecarvalho   (505) staff       (20)        0 2024-05-09 15:24:47.388693 saf_nlp-0.5.1/saf_nlp.egg-info/
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)     7218 2024-05-09 15:24:47.000000 saf_nlp-0.5.1/saf_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      903 2024-05-09 15:24:47.000000 saf_nlp-0.5.1/saf_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        1 2024-05-09 15:24:47.000000 saf_nlp-0.5.1/saf_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       11 2024-05-09 15:24:47.000000 saf_nlp-0.5.1/saf_nlp.egg-info/requires.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)        4 2024-05-09 15:24:47.000000 saf_nlp-0.5.1/saf_nlp.egg-info/top_level.txt
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)       38 2024-05-09 15:24:47.389112 saf_nlp-0.5.1/setup.cfg
+-rw-r--r--   0 dsilvadecarvalho   (505) staff       (20)      512 2024-05-09 13:52:32.000000 saf_nlp-0.5.1/setup.py
```

### Comparing `saf_nlp-0.5.0/LICENSE` & `saf_nlp-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/PKG-INFO` & `saf_nlp-0.5.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: saf-nlp
-Version: 0.5.0
+Version: 0.5.1
 Summary: Simple Annotation Framework
 Home-page: 
-Author: Danilo S. Carvalho
+Author: ['Danilo S. Carvalho', 'Vu Duc Tran']
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>, Vu Duc Tran <vu.tran@jaist.ac.jp>
 Project-URL: Homepage, https://github.com/dscarvalho/saf
 Project-URL: Issues, https://github.com/dscarvalho/saf/issues
 Keywords: annotation,nlp
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nltk
 Requires-Dist: regex
 
 # Simple Annotation Framework (SAF)
 
 The Simple Annotation Framework (SAF) is a lightweight Python library for annotating text data. It provides a simple and flexible way to create, manipulate, and export annotations in various formats.
 
-![](saf_diag.svg)
+![](https://github.com/dscarvalho/saf/raw/master/saf_diag.svg)
 
 SAF is built upon a minimalistic data model, accessible through its API. This data model is flexible enough to be used by most types of linguistic annotation, and can store other types of data associated to the language items (e.g., statistics, data sources, schemas, etc.)
 
-![](saf_class_diag.svg)
+![](https://github.com/dscarvalho/saf/raw/master/saf_class_diag.svg)
 
 ## Installation
 
 To install SAF, you can use pip:
 
 ```bash
 pip install saf
@@ -130,11 +131,61 @@
 
 conll_formatter = CoNLLFormatter(field_list=[annotation.ID])
 conll_formatted_doc = conll_formatter.dumps(doc)
 
 print(conll_formatted_doc)
 ```
 
+### Working with vocabularies
+
+Vocabulary objects can be used to quickly index and manage symbols in documents or sentence collections.  They facilitate vectorization for language model training, specially with label supervision. 
+
+```python
+from saf import Document
+from saf.constants import annotation
+from saf.importers.conll import CoNLLImporter
+from saf import Vocabulary
+
+conll_doc = """
+# sent_id = 1
+# text = They buy and sell books.
+1   They     they    PRON    PRP    Case=Nom|Number=Plur               2   nsubj   2:nsubj|4:nsubj   _
+2   buy      buy     VERB    VBP    Number=Plur|Person=3|Tense=Pres    0   root    0:root            _
+3   and      and     CCONJ   CC     _                                  4   cc      4:cc              _
+4   sell     sell    VERB    VBP    Number=Plur|Person=3|Tense=Pres    2   conj    0:root|2:conj     _
+5   books    book    NOUN    NNS    Number=Plur                        2   obj     2:obj|4:obj       SpaceAfter=No
+6   .        .       PUNCT   .      _                                  2   punct   2:punct           _
+
+# sent_id = 2
+# text = I have no clue.
+1   I       I       PRON    PRP   Case=Nom|Number=Sing|Person=1     2   nsubj   _   _
+2   have    have    VERB    VBP   Number=Sing|Person=1|Tense=Pres   0   root    _   _
+3   no      no      DET     DT    PronType=Neg                      4   det     _   _
+4   clue    clue    NOUN    NN    Number=Sing                       2   obj     _   SpaceAfter=No
+5   .       .       PUNCT   .     _                                 2   punct   _   _
+"""
+
+conll_importer = CoNLLImporter(field_list=[annotation.LEMMA, annotation.UPOS, annotation.POS])
+doc = conll_importer.import_document(conll_doc)
+
+token_vocab = Vocabulary(doc.sentences, lowercase=False)
+upos_vocab = Vocabulary(doc.sentences, source="UPOS", lowercase=False)
+
+# Converting sentences to indices for both tokens and annotations
+print(token_vocab.to_indices(doc.sentences))
+# [[2, 5, 3, 9, 4, 0], [1, 7, 8, 6, 0]]
+
+print(upos_vocab.to_indices(doc.sentences))
+# [[3, 5, 0, 5, 2, 4], [3, 5, 1, 2, 4]]
+
+# Retrieving tokens and annotations from indices
+token_vocab.get_symbol(4)
+# books
+
+upos_vocab.get_symbol(2)
+# NOUN
+```
+
 
 ## License
 
 This project is licensed under the GNU General Public License Version 3 - see the [LICENSE](https://github.com/dscarvalho/saf/blob/master/LICENSE) file for details.
```

### Comparing `saf_nlp-0.5.0/README.md` & `saf_nlp-0.5.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Simple Annotation Framework (SAF)
 
 The Simple Annotation Framework (SAF) is a lightweight Python library for annotating text data. It provides a simple and flexible way to create, manipulate, and export annotations in various formats.
 
-![](saf_diag.svg)
+![](https://github.com/dscarvalho/saf/raw/master/saf_diag.svg)
 
 SAF is built upon a minimalistic data model, accessible through its API. This data model is flexible enough to be used by most types of linguistic annotation, and can store other types of data associated to the language items (e.g., statistics, data sources, schemas, etc.)
 
-![](saf_class_diag.svg)
+![](https://github.com/dscarvalho/saf/raw/master/saf_class_diag.svg)
 
 ## Installation
 
 To install SAF, you can use pip:
 
 ```bash
 pip install saf
@@ -112,11 +112,61 @@
 
 conll_formatter = CoNLLFormatter(field_list=[annotation.ID])
 conll_formatted_doc = conll_formatter.dumps(doc)
 
 print(conll_formatted_doc)
 ```
 
+### Working with vocabularies
+
+Vocabulary objects can be used to quickly index and manage symbols in documents or sentence collections.  They facilitate vectorization for language model training, specially with label supervision. 
+
+```python
+from saf import Document
+from saf.constants import annotation
+from saf.importers.conll import CoNLLImporter
+from saf import Vocabulary
+
+conll_doc = """
+# sent_id = 1
+# text = They buy and sell books.
+1   They     they    PRON    PRP    Case=Nom|Number=Plur               2   nsubj   2:nsubj|4:nsubj   _
+2   buy      buy     VERB    VBP    Number=Plur|Person=3|Tense=Pres    0   root    0:root            _
+3   and      and     CCONJ   CC     _                                  4   cc      4:cc              _
+4   sell     sell    VERB    VBP    Number=Plur|Person=3|Tense=Pres    2   conj    0:root|2:conj     _
+5   books    book    NOUN    NNS    Number=Plur                        2   obj     2:obj|4:obj       SpaceAfter=No
+6   .        .       PUNCT   .      _                                  2   punct   2:punct           _
+
+# sent_id = 2
+# text = I have no clue.
+1   I       I       PRON    PRP   Case=Nom|Number=Sing|Person=1     2   nsubj   _   _
+2   have    have    VERB    VBP   Number=Sing|Person=1|Tense=Pres   0   root    _   _
+3   no      no      DET     DT    PronType=Neg                      4   det     _   _
+4   clue    clue    NOUN    NN    Number=Sing                       2   obj     _   SpaceAfter=No
+5   .       .       PUNCT   .     _                                 2   punct   _   _
+"""
+
+conll_importer = CoNLLImporter(field_list=[annotation.LEMMA, annotation.UPOS, annotation.POS])
+doc = conll_importer.import_document(conll_doc)
+
+token_vocab = Vocabulary(doc.sentences, lowercase=False)
+upos_vocab = Vocabulary(doc.sentences, source="UPOS", lowercase=False)
+
+# Converting sentences to indices for both tokens and annotations
+print(token_vocab.to_indices(doc.sentences))
+# [[2, 5, 3, 9, 4, 0], [1, 7, 8, 6, 0]]
+
+print(upos_vocab.to_indices(doc.sentences))
+# [[3, 5, 0, 5, 2, 4], [3, 5, 1, 2, 4]]
+
+# Retrieving tokens and annotations from indices
+token_vocab.get_symbol(4)
+# books
+
+upos_vocab.get_symbol(2)
+# NOUN
+```
+
 
 ## License
 
 This project is licensed under the GNU General Public License Version 3 - see the [LICENSE](https://github.com/dscarvalho/saf/blob/master/LICENSE) file for details.
```

### Comparing `saf_nlp-0.5.0/pyproject.toml` & `saf_nlp-0.5.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "saf-nlp"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Danilo S. Carvalho", email="danilo.carvalho@manchester.ac.uk" },
   { name="Vu Duc Tran", email="vu.tran@jaist.ac.jp" }
 ]
 description = "Simple Annotation Framework"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 keywords = ["annotation", "nlp"]
 dependencies = [
   "nltk",
   "regex",
 ]
```

### Comparing `saf_nlp-0.5.0/saf/annotators/annotator.py` & `saf_nlp-0.5.1/saf/annotators/annotator.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/constants/annotation.py` & `saf_nlp-0.5.1/saf/constants/annotation.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/data_model/document.py` & `saf_nlp-0.5.1/saf/data_model/document.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/data_model/sentence.py` & `saf_nlp-0.5.1/saf/data_model/sentence.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/data_model/sequence.py` & `saf_nlp-0.5.1/saf/data_model/sequence.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/data_model/term.py` & `saf_nlp-0.5.1/saf/data_model/term.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/data_model/vocabulary.py` & `saf_nlp-0.5.1/saf/data_model/vocabulary.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/formatters/conll.py` & `saf_nlp-0.5.1/saf/formatters/conll.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/formatters/plain.py` & `saf_nlp-0.5.1/saf/formatters/plain.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/importers/conll.py` & `saf_nlp-0.5.1/saf/importers/conll.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/importers/importer.py` & `saf_nlp-0.5.1/saf/importers/importer.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/importers/morphodb.py` & `saf_nlp-0.5.1/saf/importers/morphodb.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/importers/plain.py` & `saf_nlp-0.5.1/saf/importers/plain.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/importers/webanno.py` & `saf_nlp-0.5.1/saf/importers/webanno.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/test/test_formatters.py` & `saf_nlp-0.5.1/saf/test/test_formatters.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf/test/test_importers.py` & `saf_nlp-0.5.1/saf/test/test_importers.py`

 * *Files identical despite different names*

### Comparing `saf_nlp-0.5.0/saf_nlp.egg-info/PKG-INFO` & `saf_nlp-0.5.1/saf_nlp.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: saf-nlp
-Version: 0.5.0
+Version: 0.5.1
 Summary: Simple Annotation Framework
 Home-page: 
-Author: Danilo S. Carvalho
+Author: ['Danilo S. Carvalho', 'Vu Duc Tran']
 Author-email: "Danilo S. Carvalho" <danilo.carvalho@manchester.ac.uk>, Vu Duc Tran <vu.tran@jaist.ac.jp>
 Project-URL: Homepage, https://github.com/dscarvalho/saf
 Project-URL: Issues, https://github.com/dscarvalho/saf/issues
 Keywords: annotation,nlp
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nltk
 Requires-Dist: regex
 
 # Simple Annotation Framework (SAF)
 
 The Simple Annotation Framework (SAF) is a lightweight Python library for annotating text data. It provides a simple and flexible way to create, manipulate, and export annotations in various formats.
 
-![](saf_diag.svg)
+![](https://github.com/dscarvalho/saf/raw/master/saf_diag.svg)
 
 SAF is built upon a minimalistic data model, accessible through its API. This data model is flexible enough to be used by most types of linguistic annotation, and can store other types of data associated to the language items (e.g., statistics, data sources, schemas, etc.)
 
-![](saf_class_diag.svg)
+![](https://github.com/dscarvalho/saf/raw/master/saf_class_diag.svg)
 
 ## Installation
 
 To install SAF, you can use pip:
 
 ```bash
 pip install saf
@@ -130,11 +131,61 @@
 
 conll_formatter = CoNLLFormatter(field_list=[annotation.ID])
 conll_formatted_doc = conll_formatter.dumps(doc)
 
 print(conll_formatted_doc)
 ```
 
+### Working with vocabularies
+
+Vocabulary objects can be used to quickly index and manage symbols in documents or sentence collections.  They facilitate vectorization for language model training, specially with label supervision. 
+
+```python
+from saf import Document
+from saf.constants import annotation
+from saf.importers.conll import CoNLLImporter
+from saf import Vocabulary
+
+conll_doc = """
+# sent_id = 1
+# text = They buy and sell books.
+1   They     they    PRON    PRP    Case=Nom|Number=Plur               2   nsubj   2:nsubj|4:nsubj   _
+2   buy      buy     VERB    VBP    Number=Plur|Person=3|Tense=Pres    0   root    0:root            _
+3   and      and     CCONJ   CC     _                                  4   cc      4:cc              _
+4   sell     sell    VERB    VBP    Number=Plur|Person=3|Tense=Pres    2   conj    0:root|2:conj     _
+5   books    book    NOUN    NNS    Number=Plur                        2   obj     2:obj|4:obj       SpaceAfter=No
+6   .        .       PUNCT   .      _                                  2   punct   2:punct           _
+
+# sent_id = 2
+# text = I have no clue.
+1   I       I       PRON    PRP   Case=Nom|Number=Sing|Person=1     2   nsubj   _   _
+2   have    have    VERB    VBP   Number=Sing|Person=1|Tense=Pres   0   root    _   _
+3   no      no      DET     DT    PronType=Neg                      4   det     _   _
+4   clue    clue    NOUN    NN    Number=Sing                       2   obj     _   SpaceAfter=No
+5   .       .       PUNCT   .     _                                 2   punct   _   _
+"""
+
+conll_importer = CoNLLImporter(field_list=[annotation.LEMMA, annotation.UPOS, annotation.POS])
+doc = conll_importer.import_document(conll_doc)
+
+token_vocab = Vocabulary(doc.sentences, lowercase=False)
+upos_vocab = Vocabulary(doc.sentences, source="UPOS", lowercase=False)
+
+# Converting sentences to indices for both tokens and annotations
+print(token_vocab.to_indices(doc.sentences))
+# [[2, 5, 3, 9, 4, 0], [1, 7, 8, 6, 0]]
+
+print(upos_vocab.to_indices(doc.sentences))
+# [[3, 5, 0, 5, 2, 4], [3, 5, 1, 2, 4]]
+
+# Retrieving tokens and annotations from indices
+token_vocab.get_symbol(4)
+# books
+
+upos_vocab.get_symbol(2)
+# NOUN
+```
+
 
 ## License
 
 This project is licensed under the GNU General Public License Version 3 - see the [LICENSE](https://github.com/dscarvalho/saf/blob/master/LICENSE) file for details.
```

### Comparing `saf_nlp-0.5.0/saf_nlp.egg-info/SOURCES.txt` & `saf_nlp-0.5.1/saf_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/spyder_index-0.1.0.tar.gz` & `tmp/spyder_index-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder_index-0.1.0.tar", last modified: Wed May  8 01:51:40 2024, max compression
+gzip compressed data, was "spyder_index-0.1.1.tar", last modified: Wed May  8 15:36:30 2024, max compression
```

## Comparing `spyder_index-0.1.0.tar` & `spyder_index-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.973811 spyder_index-0.1.0/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1071 2024-05-07 19:51:35.000000 spyder_index-0.1.0/LICENSE
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     7062 2024-05-08 01:51:40.970528 spyder_index-0.1.0/PKG-INFO
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     5862 2024-05-07 22:45:10.000000 spyder_index-0.1.0/README.md
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1272 2024-05-08 01:51:32.000000 spyder_index-0.1.0/pyproject.toml
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       38 2024-05-08 01:51:40.974096 spyder_index-0.1.0/setup.cfg
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.923567 spyder_index-0.1.0/spyder_index/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       21 2024-04-28 19:56:40.000000 spyder_index-0.1.0/spyder_index/__init__.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.911308 spyder_index-0.1.0/spyder_index/core/
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.939130 spyder_index-0.1.0/spyder_index/core/document/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       83 2024-05-07 19:52:45.000000 spyder_index-0.1.0/spyder_index/core/document/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     3047 2024-05-07 20:01:23.000000 spyder_index-0.1.0/spyder_index/core/document/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.945400 spyder_index-0.1.0/spyder_index/core/embeddings/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       89 2024-05-07 19:53:08.000000 spyder_index-0.1.0/spyder_index/core/embeddings/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      728 2024-05-07 20:19:50.000000 spyder_index-0.1.0/spyder_index/core/embeddings/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.948836 spyder_index-0.1.0/spyder_index/core/vector_stores/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      116 2024-05-07 19:53:25.000000 spyder_index-0.1.0/spyder_index/core/vector_stores/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      256 2024-05-07 19:53:31.000000 spyder_index-0.1.0/spyder_index/core/vector_stores/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.952721 spyder_index-0.1.0/spyder_index/embeddings/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      117 2024-05-07 19:54:12.000000 spyder_index-0.1.0/spyder_index/embeddings/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     2024 2024-05-07 20:24:21.000000 spyder_index-0.1.0/spyder_index/embeddings/huggingface.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.956322 spyder_index-0.1.0/spyder_index/ingestion/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      109 2024-05-07 19:54:34.000000 spyder_index-0.1.0/spyder_index/ingestion/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1124 2024-05-07 19:54:41.000000 spyder_index-0.1.0/spyder_index/ingestion/directory_file.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.962171 spyder_index-0.1.0/spyder_index/text_splitters/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      200 2024-05-07 19:55:01.000000 spyder_index-0.1.0/spyder_index/text_splitters/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1832 2024-05-07 19:55:07.000000 spyder_index-0.1.0/spyder_index/text_splitters/semantic.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1511 2024-05-07 19:55:15.000000 spyder_index-0.1.0/spyder_index/text_splitters/sentence.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.966693 spyder_index-0.1.0/spyder_index/vector_stores/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      128 2024-05-07 19:55:30.000000 spyder_index-0.1.0/spyder_index/vector_stores/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     7619 2024-05-07 19:55:41.000000 spyder_index-0.1.0/spyder_index/vector_stores/elasticsearch.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 01:51:40.969049 spyder_index-0.1.0/spyder_index.egg-info/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     7062 2024-05-08 01:51:40.000000 spyder_index-0.1.0/spyder_index.egg-info/PKG-INFO
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      826 2024-05-08 01:51:40.000000 spyder_index-0.1.0/spyder_index.egg-info/SOURCES.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)        1 2024-05-08 01:51:40.000000 spyder_index-0.1.0/spyder_index.egg-info/dependency_links.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      266 2024-05-08 01:51:40.000000 spyder_index-0.1.0/spyder_index.egg-info/requires.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       13 2024-05-08 01:51:40.000000 spyder_index-0.1.0/spyder_index.egg-info/top_level.txt
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.236616 spyder_index-0.1.1/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1071 2024-05-07 19:51:35.000000 spyder_index-0.1.1/LICENSE
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     8027 2024-05-08 15:36:30.235027 spyder_index-0.1.1/PKG-INFO
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     6729 2024-05-08 15:30:10.000000 spyder_index-0.1.1/README.md
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1373 2024-05-08 15:36:04.000000 spyder_index-0.1.1/pyproject.toml
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       38 2024-05-08 15:36:30.237197 spyder_index-0.1.1/setup.cfg
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.194281 spyder_index-0.1.1/spyder_index/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       21 2024-05-08 15:13:30.000000 spyder_index-0.1.1/spyder_index/__init__.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.189481 spyder_index-0.1.1/spyder_index/core/
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.202751 spyder_index-0.1.1/spyder_index/core/document/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       83 2024-05-07 19:52:45.000000 spyder_index-0.1.1/spyder_index/core/document/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     3082 2024-05-08 14:49:50.000000 spyder_index-0.1.1/spyder_index/core/document/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.205938 spyder_index-0.1.1/spyder_index/core/embeddings/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       89 2024-05-07 19:53:08.000000 spyder_index-0.1.1/spyder_index/core/embeddings/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      728 2024-05-07 20:19:50.000000 spyder_index-0.1.1/spyder_index/core/embeddings/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.209312 spyder_index-0.1.1/spyder_index/core/vector_stores/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      116 2024-05-07 19:53:25.000000 spyder_index-0.1.1/spyder_index/core/vector_stores/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      256 2024-05-07 19:53:31.000000 spyder_index-0.1.1/spyder_index/core/vector_stores/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.212498 spyder_index-0.1.1/spyder_index/embeddings/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      117 2024-05-07 19:54:12.000000 spyder_index-0.1.1/spyder_index/embeddings/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     2024 2024-05-07 20:24:21.000000 spyder_index-0.1.1/spyder_index/embeddings/huggingface.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.218450 spyder_index-0.1.1/spyder_index/ingestion/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      184 2024-05-08 14:13:38.000000 spyder_index-0.1.1/spyder_index/ingestion/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1191 2024-05-08 14:42:42.000000 spyder_index-0.1.1/spyder_index/ingestion/directory_file.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1408 2024-05-08 14:47:33.000000 spyder_index-0.1.1/spyder_index/ingestion/ibm_cos.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.224234 spyder_index-0.1.1/spyder_index/text_splitters/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      200 2024-05-07 19:55:01.000000 spyder_index-0.1.1/spyder_index/text_splitters/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1832 2024-05-07 19:55:07.000000 spyder_index-0.1.1/spyder_index/text_splitters/semantic.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1511 2024-05-07 19:55:15.000000 spyder_index-0.1.1/spyder_index/text_splitters/sentence.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.228069 spyder_index-0.1.1/spyder_index/vector_stores/
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      128 2024-05-07 19:55:30.000000 spyder_index-0.1.1/spyder_index/vector_stores/__init__.py
+-rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     7619 2024-05-07 19:55:41.000000 spyder_index-0.1.1/spyder_index/vector_stores/elasticsearch.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-08 15:36:30.232919 spyder_index-0.1.1/spyder_index.egg-info/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     8027 2024-05-08 15:36:30.000000 spyder_index-0.1.1/spyder_index.egg-info/PKG-INFO
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      860 2024-05-08 15:36:30.000000 spyder_index-0.1.1/spyder_index.egg-info/SOURCES.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)        1 2024-05-08 15:36:30.000000 spyder_index-0.1.1/spyder_index.egg-info/dependency_links.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      286 2024-05-08 15:36:30.000000 spyder_index-0.1.1/spyder_index.egg-info/requires.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       13 2024-05-08 15:36:30.000000 spyder_index-0.1.1/spyder_index.egg-info/top_level.txt
```

### Comparing `spyder_index-0.1.0/LICENSE` & `spyder_index-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.0/PKG-INFO` & `spyder_index-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: spyder-index
-Version: 0.1.0
-Summary: Framework for your LLM applications
+Version: 0.1.1
+Summary: Spyder Index is an open-source framework for building your LLM applications
 Author: Leonardo Furnielis
 License: MIT License
 Project-URL: Homepage, https://github.com/leonardofurnielis/spyder_index
 Project-URL: Issues, https://github.com/leonardofurnielis/spyder_index/issues
-Keywords: framework,RAG,index,data
+Keywords: framework,RAG,index,data,LLM,AI,semantic search
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
@@ -22,136 +22,160 @@
 Requires-Dist: langchain-text-splitters~=0.0.1
 Requires-Dist: langchain-experimental~=0.0.57
 Requires-Dist: sentence-transformers~=2.7.0
 Requires-Dist: pydantic~=2.7.1
 Requires-Dist: pypdf~=4.2.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: elasticsearch~=8.13.0
+Requires-Dist: ibm-cos-sdk~=2.13.2
 
 # Spyder Index
 
 ## Table of Contents
 
 - Embeddings
   - [HuggingFace](#embeddings-huggingface)
 - Ingestion
   - [Directory Files](#ingestion-directory-files)
+  - [IBM Cloud Object Storage (s3)](#ingestion-ibm-cloud-object-store-s3)
 - Text Splitter
   - [Semantic Splitter](#text-splitter-semantic-splitter)
   - [Sentence Splitter](#text-splitter-sentence-splitter)
 - Vector Store
   - [Elasticsearch](#vector-store-elasticsearch)
 
 ## Embeddings: HuggingFace
 
 ### Overview
 Class for computing text embeddings using HuggingFace models.
 
 ### API Reference
 
-**`HuggingFaceEmbeddings(model_name: str= "sentence-transformers/all-MiniLM-L6-v2", device: Literal["cpu", "cuda"] = "cpu")`**
+##### **`HuggingFaceEmbeddings(model_name: str= "sentence-transformers/all-MiniLM-L6-v2", device: Literal["cpu", "cuda"] = "cpu")`**
 
 Initialize a HuggingFaceEmbeddings object.
 
 - `model_name` (str, optional): Name of the HuggingFace model to be used. Defaults to "sentence-transformers/all-MiniLM-L6-v2".
 - `device` (Literal["cpu", "cuda"], optional): Device to run the model on. Defaults to "cpu".
 
-**`get_query_embedding(query: str) -> List[float]`**
+##### **`get_query_embedding(query: str) -> List[float]`**
 
 Compute embedding for a query.
 
 - `text` (str): Input query to compute embedding.
 
-**`get_embedding_from_texts(texts: List[str]) -> List[List[float]]`**
+##### **`get_embedding_from_texts(texts: List[str]) -> List[List[float]]`**
 
 Compute embeddings for a list of texts.
 
 - `texts` (List[str])
 
-**`get_documents_embedding(documents: List[str]) -> List[List[float]]`**
+##### **`get_documents_embedding(documents: List[str]) -> List[List[float]]`**
 
 Compute embeddings for a list of Documents.
 
 - `documents` (List[Documents])
 
 ## Ingestion: Directory Files
 
 ### Overview
 This class provides functionality to load documents from a directory using various file loaders.
 
 ### API Reference
 
-**`load_data(self, dir) -> List[Document]`**
+##### **`load_data(dir: str) -> List[Document]`**
 
 Loads data from the specified directory.
 
 - `dir` (str): The directory path from which to load the documents.
+- `metadata` (Optional[dict]): Additional metadata to include in the document.
+
+## Ingestion: IBM Cloud Object Store (s3)
+
+### Overview
+Loads data from IBM Cloud Object Storage (COS) using S3 interface.
+
+### API Reference
+
+##### **`IBMS3Loader(bucket: str, ibm_api_key_id: str, ibm_service_instance_id: str, s3_endpoint_url: str)`**
+
+Initialize an IBMS3Loader object.
+
+- `bucket` (str): The name of the IBM COS bucket.
+- `ibm_api_key_id` (str): The IBM Cloud API key ID for accessing the bucket.
+- `ibm_service_instance_id` (str): The service instance ID for the IBM COS.
+- `s3_endpoint_url` (str): The endpoint URL for the IBM COS S3 service.
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
 
 ## Text Splitter: Semantic Splitter
 
 ### Overview
 Semantic Splitter is a Python class designed to split text into chunks using semantic understanding. It utilizes pre-trained embeddings to identify breakpoints in the text and divide it into meaningful segments.
 
 ### API Reference
 
-**`SemanticSplitter(model_name: str = "sentence-transformers/all-MiniLM-L6-v2", buffer_size: int = 1, breakpoint_threshold_amount: int = 95, device: Literal["cpu", "cuda"] = "cpu") -> None`**
+##### **`SemanticSplitter(model_name: str = "sentence-transformers/all-MiniLM-L6-v2", buffer_size: int = 1, breakpoint_threshold_amount: int = 95, device: Literal["cpu", "cuda"] = "cpu") -> None`**
 
 Initialize the SemanticSplitter instance.
+
 - `model_name`: Name of the pre-trained embeddings model to use. Default is "sentence-transformers/all-MiniLM-L6-v2".
 - `buffer_size`: Size of the buffer for semantic chunking. Default is 1.
 - `breakpoint_threshold_amount`: Threshold percentage for detecting breakpoints. Default is 95.
 - `device`: Device to use for processing, either "cpu" or "cuda". Default is "cpu".
 
-**`from_text(self, text: str) -> List[str]`**
+##### **`from_text(text: str) -> List[str]`**
 
 Split text into chunks.
 - `text`: Input text to split.
 
-**`from_documents(self, documents: List[Document]) -> List[Document]`**
+##### **`from_documents(documents: List[Document]) -> List[Document]`**
 
 Split text from a list of documents into chunks.
 - `documents`: List of Documents.
 
 ## Text Splitter: Sentence Splitter
 
 ### Overview
 This Python class `SentenceSplitter` is designed to split input text into smaller chunks, particularly useful for processing large documents or texts. It provides methods to split text into chunks and to split a list of documents into chunks.
 
 ### API Reference
 
-**`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, length_function = len, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
+##### **`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, length_function = len, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
 
 Creates a new instance of the `SentenceSplitter` class.
 
 - `chunk_size` (int, optional): Size of each chunk. Default is 512.
 - `chunk_overlap` (int, optional): Amount of overlap between chunks. Default is 256.
 - `length_function` (function, optional): Function to compute the length of the text. Default is `len`.
 - `separators` (List[str], optional): List of separators used to split the text into chunks. Default separators are `["\n\n", "\n", " ", ""]`.
 
 
-**`from_text(self, text: str) -> List[str]`**
+##### **`from_text(text: str) -> List[str]`**
 
 Splits the input text into chunks.
 
 - `text` (str): Input text to split.
 
-**`from_documents(self, documents: List[Document]) -> List[Document]`**
+##### **`from_documents(documents: List[Document]) -> List[Document]`**
 
 Splits a list of documents into chunks.
 
 - `documents` (List[Document]): List of Document objects.
 
 ## Vector Store: Elasticsearch
 
 ### Overview
 The `ElasticsearchVectorStore` class provides functionality to interact with Elasticsearch for storing and querying document embeddings. It facilitates adding documents, performing similarity searches, and deleting documents from an Elasticsearch index.
 
 ### API Reference
 
-**`ElasticsearchVectorStore(index_name, es_hostname, es_user, es_password, dims_length, embedding, batch_size=200, ssl=False, distance_strategy="cosine", text_field="text", vector_field="embedding")`**
+##### **`ElasticsearchVectorStore(index_name, es_hostname, es_user, es_password, dims_length, embedding, batch_size=200, ssl=False, distance_strategy="cosine", text_field="text", vector_field="embedding")`**
 
 Initializes the ElasticsearchVectorStore instance.
 
 - `index_name`: The name of the Elasticsearch index.
 - `es_hostname`: The hostname of the Elasticsearch instance.
 - `es_user`: The username for authentication.
 - `es_password`: The password for authentication.
@@ -159,28 +183,26 @@
 - `embedding`: An instance of embeddings.
 - `batch_size`: The batch size for bulk operations. Defaults to 200.
 - `ssl`: Whether to use SSL. Defaults to False.
 - `distance_strategy`: The distance strategy for similarity search. Defaults to "cosine".
 - `text_field`: The name of the field containing text. Defaults to "text".
 - `vector_field`: The name of the field containing vector embeddings. Defaults to "embedding".
 
-**`add_documents(documents, create_index_if_not_exists=True)`**
+##### **`add_documents(documents, create_index_if_not_exists=True)`**
 
 Adds documents to the Elasticsearch index.
 
 - `documents`: A list of Document objects to add to the index.
 - `create_index_if_not_exists`: Whether to create the index if it doesn't exist. Defaults to True.
 
-**`similarity_search(query, top_k=4)`**
+##### **`similarity_search(query, top_k=4)`**
 
 Performs a similarity search based on the documents most similar to the query.
 
 - `query`: The query text.
 - `top_k`: The number of top results to return. Defaults to 4.
 
-**`delete(ids=None)`**
+##### **`delete(ids=None)`**
 
 Deletes documents from the Elasticsearch index.
 
 - `ids`: A list of document IDs to delete. Defaults to None.
-
-
```

### Comparing `spyder_index-0.1.0/README.md` & `spyder_index-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,127 +2,150 @@
 
 ## Table of Contents
 
 - Embeddings
   - [HuggingFace](#embeddings-huggingface)
 - Ingestion
   - [Directory Files](#ingestion-directory-files)
+  - [IBM Cloud Object Storage (s3)](#ingestion-ibm-cloud-object-store-s3)
 - Text Splitter
   - [Semantic Splitter](#text-splitter-semantic-splitter)
   - [Sentence Splitter](#text-splitter-sentence-splitter)
 - Vector Store
   - [Elasticsearch](#vector-store-elasticsearch)
 
 ## Embeddings: HuggingFace
 
 ### Overview
 Class for computing text embeddings using HuggingFace models.
 
 ### API Reference
 
-**`HuggingFaceEmbeddings(model_name: str= "sentence-transformers/all-MiniLM-L6-v2", device: Literal["cpu", "cuda"] = "cpu")`**
+##### **`HuggingFaceEmbeddings(model_name: str= "sentence-transformers/all-MiniLM-L6-v2", device: Literal["cpu", "cuda"] = "cpu")`**
 
 Initialize a HuggingFaceEmbeddings object.
 
 - `model_name` (str, optional): Name of the HuggingFace model to be used. Defaults to "sentence-transformers/all-MiniLM-L6-v2".
 - `device` (Literal["cpu", "cuda"], optional): Device to run the model on. Defaults to "cpu".
 
-**`get_query_embedding(query: str) -> List[float]`**
+##### **`get_query_embedding(query: str) -> List[float]`**
 
 Compute embedding for a query.
 
 - `text` (str): Input query to compute embedding.
 
-**`get_embedding_from_texts(texts: List[str]) -> List[List[float]]`**
+##### **`get_embedding_from_texts(texts: List[str]) -> List[List[float]]`**
 
 Compute embeddings for a list of texts.
 
 - `texts` (List[str])
 
-**`get_documents_embedding(documents: List[str]) -> List[List[float]]`**
+##### **`get_documents_embedding(documents: List[str]) -> List[List[float]]`**
 
 Compute embeddings for a list of Documents.
 
 - `documents` (List[Documents])
 
 ## Ingestion: Directory Files
 
 ### Overview
 This class provides functionality to load documents from a directory using various file loaders.
 
 ### API Reference
 
-**`load_data(self, dir) -> List[Document]`**
+##### **`load_data(dir: str) -> List[Document]`**
 
 Loads data from the specified directory.
 
 - `dir` (str): The directory path from which to load the documents.
+- `metadata` (Optional[dict]): Additional metadata to include in the document.
+
+## Ingestion: IBM Cloud Object Store (s3)
+
+### Overview
+Loads data from IBM Cloud Object Storage (COS) using S3 interface.
+
+### API Reference
+
+##### **`IBMS3Loader(bucket: str, ibm_api_key_id: str, ibm_service_instance_id: str, s3_endpoint_url: str)`**
+
+Initialize an IBMS3Loader object.
+
+- `bucket` (str): The name of the IBM COS bucket.
+- `ibm_api_key_id` (str): The IBM Cloud API key ID for accessing the bucket.
+- `ibm_service_instance_id` (str): The service instance ID for the IBM COS.
+- `s3_endpoint_url` (str): The endpoint URL for the IBM COS S3 service.
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
 
 ## Text Splitter: Semantic Splitter
 
 ### Overview
 Semantic Splitter is a Python class designed to split text into chunks using semantic understanding. It utilizes pre-trained embeddings to identify breakpoints in the text and divide it into meaningful segments.
 
 ### API Reference
 
-**`SemanticSplitter(model_name: str = "sentence-transformers/all-MiniLM-L6-v2", buffer_size: int = 1, breakpoint_threshold_amount: int = 95, device: Literal["cpu", "cuda"] = "cpu") -> None`**
+##### **`SemanticSplitter(model_name: str = "sentence-transformers/all-MiniLM-L6-v2", buffer_size: int = 1, breakpoint_threshold_amount: int = 95, device: Literal["cpu", "cuda"] = "cpu") -> None`**
 
 Initialize the SemanticSplitter instance.
+
 - `model_name`: Name of the pre-trained embeddings model to use. Default is "sentence-transformers/all-MiniLM-L6-v2".
 - `buffer_size`: Size of the buffer for semantic chunking. Default is 1.
 - `breakpoint_threshold_amount`: Threshold percentage for detecting breakpoints. Default is 95.
 - `device`: Device to use for processing, either "cpu" or "cuda". Default is "cpu".
 
-**`from_text(self, text: str) -> List[str]`**
+##### **`from_text(text: str) -> List[str]`**
 
 Split text into chunks.
 - `text`: Input text to split.
 
-**`from_documents(self, documents: List[Document]) -> List[Document]`**
+##### **`from_documents(documents: List[Document]) -> List[Document]`**
 
 Split text from a list of documents into chunks.
 - `documents`: List of Documents.
 
 ## Text Splitter: Sentence Splitter
 
 ### Overview
 This Python class `SentenceSplitter` is designed to split input text into smaller chunks, particularly useful for processing large documents or texts. It provides methods to split text into chunks and to split a list of documents into chunks.
 
 ### API Reference
 
-**`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, length_function = len, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
+##### **`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, length_function = len, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
 
 Creates a new instance of the `SentenceSplitter` class.
 
 - `chunk_size` (int, optional): Size of each chunk. Default is 512.
 - `chunk_overlap` (int, optional): Amount of overlap between chunks. Default is 256.
 - `length_function` (function, optional): Function to compute the length of the text. Default is `len`.
 - `separators` (List[str], optional): List of separators used to split the text into chunks. Default separators are `["\n\n", "\n", " ", ""]`.
 
 
-**`from_text(self, text: str) -> List[str]`**
+##### **`from_text(text: str) -> List[str]`**
 
 Splits the input text into chunks.
 
 - `text` (str): Input text to split.
 
-**`from_documents(self, documents: List[Document]) -> List[Document]`**
+##### **`from_documents(documents: List[Document]) -> List[Document]`**
 
 Splits a list of documents into chunks.
 
 - `documents` (List[Document]): List of Document objects.
 
 ## Vector Store: Elasticsearch
 
 ### Overview
 The `ElasticsearchVectorStore` class provides functionality to interact with Elasticsearch for storing and querying document embeddings. It facilitates adding documents, performing similarity searches, and deleting documents from an Elasticsearch index.
 
 ### API Reference
 
-**`ElasticsearchVectorStore(index_name, es_hostname, es_user, es_password, dims_length, embedding, batch_size=200, ssl=False, distance_strategy="cosine", text_field="text", vector_field="embedding")`**
+##### **`ElasticsearchVectorStore(index_name, es_hostname, es_user, es_password, dims_length, embedding, batch_size=200, ssl=False, distance_strategy="cosine", text_field="text", vector_field="embedding")`**
 
 Initializes the ElasticsearchVectorStore instance.
 
 - `index_name`: The name of the Elasticsearch index.
 - `es_hostname`: The hostname of the Elasticsearch instance.
 - `es_user`: The username for authentication.
 - `es_password`: The password for authentication.
@@ -130,28 +153,26 @@
 - `embedding`: An instance of embeddings.
 - `batch_size`: The batch size for bulk operations. Defaults to 200.
 - `ssl`: Whether to use SSL. Defaults to False.
 - `distance_strategy`: The distance strategy for similarity search. Defaults to "cosine".
 - `text_field`: The name of the field containing text. Defaults to "text".
 - `vector_field`: The name of the field containing vector embeddings. Defaults to "embedding".
 
-**`add_documents(documents, create_index_if_not_exists=True)`**
+##### **`add_documents(documents, create_index_if_not_exists=True)`**
 
 Adds documents to the Elasticsearch index.
 
 - `documents`: A list of Document objects to add to the index.
 - `create_index_if_not_exists`: Whether to create the index if it doesn't exist. Defaults to True.
 
-**`similarity_search(query, top_k=4)`**
+##### **`similarity_search(query, top_k=4)`**
 
 Performs a similarity search based on the documents most similar to the query.
 
 - `query`: The query text.
 - `top_k`: The number of top results to return. Defaults to 4.
 
-**`delete(ids=None)`**
+##### **`delete(ids=None)`**
 
 Deletes documents from the Elasticsearch index.
 
 - `ids`: A list of document IDs to delete. Defaults to None.
-
-
```

### Comparing `spyder_index-0.1.0/pyproject.toml` & `spyder_index-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [build-system]
 requires = ["setuptools >= 61.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spyder-index"
-version = "0.1.0"
-description = "Framework for your LLM applications"
+version = "0.1.1"
+description = "Spyder Index is an open-source framework for building your LLM applications"
 readme = "README.md"
 authors = [{ name = "Leonardo Furnielis" }]
 license = {text = "MIT License"}
-keywords = ["framework", "RAG", "index", "data"]
+keywords = ["framework", "RAG", "index", "data", "LLM", "AI", "semantic search"]
 dependencies = [
     "llama-index-core ~= 0.10.30",
     "llama-index-readers-file ~= 0.1.19",
     "langchain-core ~= 0.1.48",
     "langchain-community ~= 0.0.36",
     "langchain-text-splitters ~= 0.0.1",
     "langchain-experimental ~= 0.0.57",
     "sentence-transformers ~= 2.7.0",
     "pydantic ~= 2.7.1",
     "pypdf ~= 4.2.0",
     "torch == 2.1.0",
     "elasticsearch ~= 8.13.0",
+    "ibm-cos-sdk ~= 2.13.2"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
```

### Comparing `spyder_index-0.1.0/spyder_index/core/document/base.py` & `spyder_index-0.1.1/spyder_index/core/document/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import uuid
 import mimetypes
-from typing import TYPE_CHECKING, Literal
+from typing import TYPE_CHECKING, Literal, Optional
 from datetime import datetime
 from pydantic import BaseModel, Field
 
 if TYPE_CHECKING:
     from llama_index.core.schema import Document as LlamaIndexDocument
     from langchain_core.documents import Document as LangchainDocument
 
@@ -14,19 +14,14 @@
     text: str = Field(default="")
     metadata: dict = Field(default={})
 
     @classmethod
     def class_name(cls) -> str:
         return "Document"
 
-    def set_content(self, text: str, metadata: dict = {}) -> None:
-        """Set the text content and metadata of the document."""
-        self.text = text
-        self.metadata = metadata
-
     def get_text(self) -> str:
         """Get the text content of the document."""
         return self.text
     
     def get_metadata(self) -> dict:
         """Get the metadata of the document."""
         return self.metadata
@@ -71,20 +66,24 @@
             Document: Converted document.
         """
         
         converted_metadata = cls._convert_metadata(doc.metadata, "langchain")
         return cls(text=doc.page_content, metadata=converted_metadata)
     
     @classmethod
-    def _from_llama_index_format(cls, doc: "LlamaIndexDocument") -> "Document":
+    def _from_llama_index_format(cls, doc: "LlamaIndexDocument", metadata: Optional[dict]) -> "Document":
         """
         Convert a document from LlamaIndex format to spyder_index Document format.
 
         Args:
             doc (LlamaIndexDocument): Document in LlamaIndex format.
+            metadata (Optional[dict]): Additional metadata to include in the converted document.
 
         Returns:
             Document: Converted document.
         """
-
         converted_metadata = cls._convert_metadata(doc.metadata, "llama_index")
+        
+        if metadata:
+            converted_metadata = metadata | converted_metadata
+
         return cls(text=doc.text, metadata=converted_metadata)
```

### Comparing `spyder_index-0.1.0/spyder_index/core/embeddings/base.py` & `spyder_index-0.1.1/spyder_index/core/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.0/spyder_index/embeddings/huggingface.py` & `spyder_index-0.1.1/spyder_index/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.0/spyder_index/ingestion/directory_file.py` & `spyder_index-0.1.1/spyder_index/ingestion/directory_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 from spyder_index.core.document import Document
 
 from llama_index.readers.file import PDFReader
 from llama_index.readers.file import DocxReader
 # from llama_index.readers.file import PptxReader
 from llama_index.readers.file import HTMLTagReader
@@ -18,15 +18,15 @@
         '.pdf': PDFReader(),
         '.docx': DocxReader(), 
         # '.pptx': PptxReader(), #download_loader('PptxReader'),
         '.html': HTMLTagReader(), 
         # '.txt': download_loader('UnstructuredReader'),
         }
 
-    def load_data(self, dir) -> List[Document]: 
+    def load_data(self, dir: str, metadata: Optional[dict]) -> List[Document]:
 
         llama_documents = SimpleDirectoryReader(
             input_dir=Path(dir).absolute(), 
             file_extractor=self.supported_file_loader, 
             required_exts= list(self.supported_file_loader.keys())).load_data()
-
-        return [Document()._from_llama_index_format(doc=doc) for doc in llama_documents]
+        
+        return [Document()._from_llama_index_format(doc=doc, metadata=metadata) for doc in llama_documents]
```

### Comparing `spyder_index-0.1.0/spyder_index/text_splitters/semantic.py` & `spyder_index-0.1.1/spyder_index/text_splitters/semantic.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.0/spyder_index/text_splitters/sentence.py` & `spyder_index-0.1.1/spyder_index/text_splitters/sentence.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.0/spyder_index/vector_stores/elasticsearch.py` & `spyder_index-0.1.1/spyder_index/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.1.0/spyder_index.egg-info/PKG-INFO` & `spyder_index-0.1.1/spyder_index.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: spyder-index
-Version: 0.1.0
-Summary: Framework for your LLM applications
+Version: 0.1.1
+Summary: Spyder Index is an open-source framework for building your LLM applications
 Author: Leonardo Furnielis
 License: MIT License
 Project-URL: Homepage, https://github.com/leonardofurnielis/spyder_index
 Project-URL: Issues, https://github.com/leonardofurnielis/spyder_index/issues
-Keywords: framework,RAG,index,data
+Keywords: framework,RAG,index,data,LLM,AI,semantic search
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
@@ -22,136 +22,160 @@
 Requires-Dist: langchain-text-splitters~=0.0.1
 Requires-Dist: langchain-experimental~=0.0.57
 Requires-Dist: sentence-transformers~=2.7.0
 Requires-Dist: pydantic~=2.7.1
 Requires-Dist: pypdf~=4.2.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: elasticsearch~=8.13.0
+Requires-Dist: ibm-cos-sdk~=2.13.2
 
 # Spyder Index
 
 ## Table of Contents
 
 - Embeddings
   - [HuggingFace](#embeddings-huggingface)
 - Ingestion
   - [Directory Files](#ingestion-directory-files)
+  - [IBM Cloud Object Storage (s3)](#ingestion-ibm-cloud-object-store-s3)
 - Text Splitter
   - [Semantic Splitter](#text-splitter-semantic-splitter)
   - [Sentence Splitter](#text-splitter-sentence-splitter)
 - Vector Store
   - [Elasticsearch](#vector-store-elasticsearch)
 
 ## Embeddings: HuggingFace
 
 ### Overview
 Class for computing text embeddings using HuggingFace models.
 
 ### API Reference
 
-**`HuggingFaceEmbeddings(model_name: str= "sentence-transformers/all-MiniLM-L6-v2", device: Literal["cpu", "cuda"] = "cpu")`**
+##### **`HuggingFaceEmbeddings(model_name: str= "sentence-transformers/all-MiniLM-L6-v2", device: Literal["cpu", "cuda"] = "cpu")`**
 
 Initialize a HuggingFaceEmbeddings object.
 
 - `model_name` (str, optional): Name of the HuggingFace model to be used. Defaults to "sentence-transformers/all-MiniLM-L6-v2".
 - `device` (Literal["cpu", "cuda"], optional): Device to run the model on. Defaults to "cpu".
 
-**`get_query_embedding(query: str) -> List[float]`**
+##### **`get_query_embedding(query: str) -> List[float]`**
 
 Compute embedding for a query.
 
 - `text` (str): Input query to compute embedding.
 
-**`get_embedding_from_texts(texts: List[str]) -> List[List[float]]`**
+##### **`get_embedding_from_texts(texts: List[str]) -> List[List[float]]`**
 
 Compute embeddings for a list of texts.
 
 - `texts` (List[str])
 
-**`get_documents_embedding(documents: List[str]) -> List[List[float]]`**
+##### **`get_documents_embedding(documents: List[str]) -> List[List[float]]`**
 
 Compute embeddings for a list of Documents.
 
 - `documents` (List[Documents])
 
 ## Ingestion: Directory Files
 
 ### Overview
 This class provides functionality to load documents from a directory using various file loaders.
 
 ### API Reference
 
-**`load_data(self, dir) -> List[Document]`**
+##### **`load_data(dir: str) -> List[Document]`**
 
 Loads data from the specified directory.
 
 - `dir` (str): The directory path from which to load the documents.
+- `metadata` (Optional[dict]): Additional metadata to include in the document.
+
+## Ingestion: IBM Cloud Object Store (s3)
+
+### Overview
+Loads data from IBM Cloud Object Storage (COS) using S3 interface.
+
+### API Reference
+
+##### **`IBMS3Loader(bucket: str, ibm_api_key_id: str, ibm_service_instance_id: str, s3_endpoint_url: str)`**
+
+Initialize an IBMS3Loader object.
+
+- `bucket` (str): The name of the IBM COS bucket.
+- `ibm_api_key_id` (str): The IBM Cloud API key ID for accessing the bucket.
+- `ibm_service_instance_id` (str): The service instance ID for the IBM COS.
+- `s3_endpoint_url` (str): The endpoint URL for the IBM COS S3 service.
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
 
 ## Text Splitter: Semantic Splitter
 
 ### Overview
 Semantic Splitter is a Python class designed to split text into chunks using semantic understanding. It utilizes pre-trained embeddings to identify breakpoints in the text and divide it into meaningful segments.
 
 ### API Reference
 
-**`SemanticSplitter(model_name: str = "sentence-transformers/all-MiniLM-L6-v2", buffer_size: int = 1, breakpoint_threshold_amount: int = 95, device: Literal["cpu", "cuda"] = "cpu") -> None`**
+##### **`SemanticSplitter(model_name: str = "sentence-transformers/all-MiniLM-L6-v2", buffer_size: int = 1, breakpoint_threshold_amount: int = 95, device: Literal["cpu", "cuda"] = "cpu") -> None`**
 
 Initialize the SemanticSplitter instance.
+
 - `model_name`: Name of the pre-trained embeddings model to use. Default is "sentence-transformers/all-MiniLM-L6-v2".
 - `buffer_size`: Size of the buffer for semantic chunking. Default is 1.
 - `breakpoint_threshold_amount`: Threshold percentage for detecting breakpoints. Default is 95.
 - `device`: Device to use for processing, either "cpu" or "cuda". Default is "cpu".
 
-**`from_text(self, text: str) -> List[str]`**
+##### **`from_text(text: str) -> List[str]`**
 
 Split text into chunks.
 - `text`: Input text to split.
 
-**`from_documents(self, documents: List[Document]) -> List[Document]`**
+##### **`from_documents(documents: List[Document]) -> List[Document]`**
 
 Split text from a list of documents into chunks.
 - `documents`: List of Documents.
 
 ## Text Splitter: Sentence Splitter
 
 ### Overview
 This Python class `SentenceSplitter` is designed to split input text into smaller chunks, particularly useful for processing large documents or texts. It provides methods to split text into chunks and to split a list of documents into chunks.
 
 ### API Reference
 
-**`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, length_function = len, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
+##### **`SentenceSplitter(chunk_size: int = 512, chunk_overlap: int = 256, length_function = len, separators: List[str] = ["\n\n", "\n", " ", ""]) -> None`**
 
 Creates a new instance of the `SentenceSplitter` class.
 
 - `chunk_size` (int, optional): Size of each chunk. Default is 512.
 - `chunk_overlap` (int, optional): Amount of overlap between chunks. Default is 256.
 - `length_function` (function, optional): Function to compute the length of the text. Default is `len`.
 - `separators` (List[str], optional): List of separators used to split the text into chunks. Default separators are `["\n\n", "\n", " ", ""]`.
 
 
-**`from_text(self, text: str) -> List[str]`**
+##### **`from_text(text: str) -> List[str]`**
 
 Splits the input text into chunks.
 
 - `text` (str): Input text to split.
 
-**`from_documents(self, documents: List[Document]) -> List[Document]`**
+##### **`from_documents(documents: List[Document]) -> List[Document]`**
 
 Splits a list of documents into chunks.
 
 - `documents` (List[Document]): List of Document objects.
 
 ## Vector Store: Elasticsearch
 
 ### Overview
 The `ElasticsearchVectorStore` class provides functionality to interact with Elasticsearch for storing and querying document embeddings. It facilitates adding documents, performing similarity searches, and deleting documents from an Elasticsearch index.
 
 ### API Reference
 
-**`ElasticsearchVectorStore(index_name, es_hostname, es_user, es_password, dims_length, embedding, batch_size=200, ssl=False, distance_strategy="cosine", text_field="text", vector_field="embedding")`**
+##### **`ElasticsearchVectorStore(index_name, es_hostname, es_user, es_password, dims_length, embedding, batch_size=200, ssl=False, distance_strategy="cosine", text_field="text", vector_field="embedding")`**
 
 Initializes the ElasticsearchVectorStore instance.
 
 - `index_name`: The name of the Elasticsearch index.
 - `es_hostname`: The hostname of the Elasticsearch instance.
 - `es_user`: The username for authentication.
 - `es_password`: The password for authentication.
@@ -159,28 +183,26 @@
 - `embedding`: An instance of embeddings.
 - `batch_size`: The batch size for bulk operations. Defaults to 200.
 - `ssl`: Whether to use SSL. Defaults to False.
 - `distance_strategy`: The distance strategy for similarity search. Defaults to "cosine".
 - `text_field`: The name of the field containing text. Defaults to "text".
 - `vector_field`: The name of the field containing vector embeddings. Defaults to "embedding".
 
-**`add_documents(documents, create_index_if_not_exists=True)`**
+##### **`add_documents(documents, create_index_if_not_exists=True)`**
 
 Adds documents to the Elasticsearch index.
 
 - `documents`: A list of Document objects to add to the index.
 - `create_index_if_not_exists`: Whether to create the index if it doesn't exist. Defaults to True.
 
-**`similarity_search(query, top_k=4)`**
+##### **`similarity_search(query, top_k=4)`**
 
 Performs a similarity search based on the documents most similar to the query.
 
 - `query`: The query text.
 - `top_k`: The number of top results to return. Defaults to 4.
 
-**`delete(ids=None)`**
+##### **`delete(ids=None)`**
 
 Deletes documents from the Elasticsearch index.
 
 - `ids`: A list of document IDs to delete. Defaults to None.
-
-
```

### Comparing `spyder_index-0.1.0/spyder_index.egg-info/SOURCES.txt` & `spyder_index-0.1.1/spyder_index.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,12 +13,13 @@
 spyder_index/core/embeddings/base.py
 spyder_index/core/vector_stores/__init__.py
 spyder_index/core/vector_stores/base.py
 spyder_index/embeddings/__init__.py
 spyder_index/embeddings/huggingface.py
 spyder_index/ingestion/__init__.py
 spyder_index/ingestion/directory_file.py
+spyder_index/ingestion/ibm_cos.py
 spyder_index/text_splitters/__init__.py
 spyder_index/text_splitters/semantic.py
 spyder_index/text_splitters/sentence.py
 spyder_index/vector_stores/__init__.py
 spyder_index/vector_stores/elasticsearch.py
```


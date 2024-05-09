# Comparing `tmp/triton_bert-0.3.0.tar.gz` & `tmp/triton_bert-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triton_bert-0.3.0.tar", max compression
+gzip compressed data, was "triton_bert-0.3.2.tar", max compression
```

## Comparing `triton_bert-0.3.0.tar` & `triton_bert-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0     1092 2023-12-29 14:58:07.229796 triton_bert-0.3.0/LICENSE
--rw-r--r--   0        0        0     5466 2024-02-21 03:05:00.922465 triton_bert-0.3.0/README.md
--rw-r--r--   0        0        0      838 2024-02-21 03:06:50.506453 triton_bert-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-29 14:58:07.297592 triton_bert-0.3.0/triton_bert/__init__.py
--rw-r--r--   0        0        0     3423 2024-02-20 07:14:31.041576 triton_bert-0.3.0/triton_bert/model_4_triton.py
--rw-r--r--   0        0        0     3000 2024-02-21 02:54:36.595841 triton_bert-0.3.0/triton_bert/pgvector_triton.py
--rw-r--r--   0        0        0        0 2024-02-20 07:31:10.466866 triton_bert-0.3.0/triton_bert/tests/__init__.py
--rw-r--r--   0        0        0    13564 2024-02-21 01:38:19.780109 triton_bert-0.3.0/triton_bert/tests/dataset/medical_qa.jsonl
--rw-r--r--   0        0        0     1326 2024-02-20 07:32:07.969224 triton_bert-0.3.0/triton_bert/tests/test_biencoder.py
--rw-r--r--   0        0        0      755 2023-12-29 14:58:07.254385 triton_bert-0.3.0/triton_bert/tests/test_chitchat.py
--rw-r--r--   0        0        0      810 2024-02-20 07:30:21.595536 triton_bert-0.3.0/triton_bert/tests/test_crossencoder.py
--rw-r--r--   0        0        0     2377 2024-02-20 07:09:35.660852 triton_bert-0.3.0/triton_bert/tests/test_generate_bgem3_triton_model.py
--rw-r--r--   0        0        0      362 2024-02-20 06:52:48.761566 triton_bert-0.3.0/triton_bert/tests/test_generate_triton_model.py
--rw-r--r--   0        0        0     2761 2024-02-21 02:54:03.474534 triton_bert-0.3.0/triton_bert/tests/test_pgvector_triton.py
--rw-r--r--   0        0        0      662 2024-02-20 09:51:38.926387 triton_bert-0.3.0/triton_bert/tests/test_triton_bert.py
--rw-r--r--   0        0        0     5772 2024-02-20 09:50:47.307788 triton_bert-0.3.0/triton_bert/triton_bert.py
--rw-r--r--   0        0        0     6484 1970-01-01 00:00:00.000000 triton_bert-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-12-29 14:58:07.229796 triton_bert-0.3.2/LICENSE
+-rw-r--r--   0        0        0     5344 2024-04-26 06:51:34.511018 triton_bert-0.3.2/README.md
+-rw-r--r--   0        0        0      676 2024-05-09 11:54:53.862224 triton_bert-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-29 14:58:07.297592 triton_bert-0.3.2/triton_bert/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-09 11:31:57.839165 triton_bert-0.3.2/triton_bert/model/bge_m3.py
+-rw-r--r--   0        0        0     3468 2024-05-09 03:23:16.722289 triton_bert-0.3.2/triton_bert/model/model_4_triton.py
+-rw-r--r--   0        0        0        0 2024-02-20 07:31:10.466866 triton_bert-0.3.2/triton_bert/tests/__init__.py
+-rw-r--r--   0        0        0    13564 2024-02-21 01:38:19.780109 triton_bert-0.3.2/triton_bert/tests/dataset/medical_qa.jsonl
+-rw-r--r--   0        0        0      141 2024-04-19 08:49:36.927506 triton_bert-0.3.2/triton_bert/tests/get_onnx_output.py
+-rw-r--r--   0        0        0      452 2024-05-09 11:21:39.630993 triton_bert-0.3.2/triton_bert/tests/test_bge_m3.py
+-rw-r--r--   0        0        0     1307 2024-04-26 06:54:52.778743 triton_bert-0.3.2/triton_bert/tests/test_biencoder.py
+-rw-r--r--   0        0        0      755 2023-12-29 14:58:07.254385 triton_bert-0.3.2/triton_bert/tests/test_chitchat.py
+-rw-r--r--   0        0        0      810 2024-02-20 07:30:21.595536 triton_bert-0.3.2/triton_bert/tests/test_crossencoder.py
+-rw-r--r--   0        0        0     2378 2024-05-09 03:05:47.883874 triton_bert-0.3.2/triton_bert/tests/test_generate_bgem3_triton_model.py
+-rw-r--r--   0        0        0      290 2024-04-19 01:59:48.443054 triton_bert-0.3.2/triton_bert/tests/test_generate_triton_bert.py
+-rw-r--r--   0        0        0      395 2024-04-26 06:54:52.778467 triton_bert-0.3.2/triton_bert/tests/test_generate_triton_model.py
+-rw-r--r--   0        0        0     2566 2024-04-26 06:50:28.804221 triton_bert-0.3.2/triton_bert/tests/test_pgvector_triton.py
+-rw-r--r--   0        0        0      644 2024-04-26 06:54:52.778416 triton_bert-0.3.2/triton_bert/tests/test_triton_bert.py
+-rw-r--r--   0        0        0     5799 2024-05-09 11:25:20.679637 triton_bert-0.3.2/triton_bert/triton_bert.py
+-rw-r--r--   0        0        0     3000 2024-02-21 02:54:36.595841 triton_bert-0.3.2/triton_bert/vector_db/pgvector_triton.py
+-rw-r--r--   0        0        0     6342 1970-01-01 00:00:00.000000 triton_bert-0.3.2/PKG-INFO
```

### Comparing `triton_bert-0.3.0/LICENSE` & `triton_bert-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `triton_bert-0.3.0/README.md` & `triton_bert-0.3.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 embedding output from model can be used directly.
 so no need to override the proprocess function.
 
 ```python
 from triton_bert.triton_bert import TritonBert
 
 if __name__ == "__main__":
-    model = TritonBert(triton_host="30.171.160.44", model="sbert_onnx", 
-                       vocab="/Users/yanyongwen712/.cache/torch/sentence_transformers/sentence-transformers_all-MiniLM-L6-v2")
+    model = TritonBert(triton_host="127.0.0.1", model="sbert_onnx", 
+                       vocab="/Users/xxx/.cache/torch/sentence_transformers/sentence-transformers_all-MiniLM-L6-v2")
 
     # batch inferences
     vectors = model(["基金的收益率是多少？", "我有个朋友的股票天天涨停"])
     # or
     vectors = model.encode(["基金的收益率是多少？", "我有个朋友的股票天天涨停"])
     assert len(vectors) == 2
 
@@ -109,41 +109,41 @@
 
 ```
 
 # run examples
 ## run triton server
 ```bash
 # for example
-docker run -d  --name triton-server   --shm-size=1g --ulimit memlock=-1 --ulimit stack=67108864  --rm -p 8000:8000 -p 8001:8001 -p 8002:8002 -v /home/yanyongwen712/triton_models:/models  nvcr.io/nvidia/tritonserver::22.08-py3 tritonserver --model-repository=/models  --model-control-mode=poll  --exit-on-error=false --log-verbose 1
+docker run -d  --name triton-server   --shm-size=1g --ulimit memlock=-1 --ulimit stack=67108864  --rm -p 8000:8000 -p 8001:8001 -p 8002:8002 -v /home/xxxx/triton_models:/models  nvcr.io/nvidia/tritonserver::22.08-py3 tritonserver --model-repository=/models  --model-control-mode=poll  --exit-on-error=false --log-verbose 1
 # configure triton model folder
 ```
 ## prepare model for triton server
 See the tests for more examples.
 
 Example:
 ```python
 from triton_bert.model_4_triton import Model4TritonServer
 
 if __name__ == "__main__":
-    pretrained_model = "/Users/yanyongwen712/.cache/torch/sentence_transformers/simcse-chinese-roberta-wwm-ext"
+    pretrained_model = "/Users/xxxxx/.cache/torch/sentence_transformers/simcse-chinese-roberta-wwm-ext"
     model = Model4TritonServer(pretrained_model=pretrained_model)
     model.save_torchscript("model/simcse_model.pt")
     model.save_onnx("model/simcse_model.onnx")
 
 ```
 
 # Semantic Retrieval with Postgresql/pgvector
 Example 1
 ```python
 
-    instance = PgvectorTriton(db_user="budevadmin", db_password='eimdmPOSTGRESQL@2023',
-                              db_instance="D0PEIMDMINFO-postgresql.dbdev.paic.com.cn", db_port="3671",
-                   db_schema="pivotoperation", create_table=True,
-                   triton_host="30.171.160.44", model="bge-m3",
-                   vocab="/Users/yanyongwen712/Codes/pingan_health_rag/models/bge-m3",
+    instance = PgvectorTriton(db_user="xxx", db_password='xxxx',
+                              db_instance="xxxx", db_port="3671",
+                   db_schema="xxx", create_table=True,
+                   triton_host="xxx", model="bge-m3",
+                   vocab="/Users/xxx/Codes/pingan_health_rag/models/bge-m3",
                               table_model=Sentence
                    )
 
     # insert
     qas = instance.load_texts("dataset/medical_qa.jsonl")
     answers = [qa['answers'][0] for qa in qas]
     instance.insert_vectors(answers)
```

### Comparing `triton_bert-0.3.0/pyproject.toml` & `triton_bert-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "triton-bert"
-version = "0.3.0"
+version = "0.3.2"
 description = "easy to use bert with nvidia triton inference server"
-authors = ["yanyongwen712 <yanyongwen712@pingan.com.cn>"]
+authors = ["yyw794 <yyw794@126.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 tritonclient = {extras = ["grpc", "http"], version = "^2.41.0"}
 transformers = "^4.36.2"
@@ -14,20 +14,14 @@
 protobuf = "^4.23"
 pgvector = "^0.2.4"
 sqlmodel = "^0.0.14"
 onnx = "^1.15.0"
 psycopg2-binary = "^2.9.9"
 jsonlines = "^4.0.0"
 
-[tool.poetry.group.dev.dependencies]
-sentence-transformers = "^2.2.2"
-flagembedding = "^1.2.3"
-grequests = "^0.7.0"
-pycryptodome = "^3.20.0"
-
 
 [[tool.poetry.source]]
 name = "aliyun"
 url = "http://mirrors.aliyun.com/pypi/simple/"
 priority = "primary"
 
 [build-system]
```

### Comparing `triton_bert-0.3.0/triton_bert/model_4_triton.py` & `triton_bert-0.3.2/triton_bert/model/model_4_triton.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import torch
 import torch.nn as nn
 from transformers import AutoTokenizer, AutoModel
 
 
 class Model4TritonServer(nn.Module):
-    def __init__(self, pretrained_model:Optional[str]=None, gpu_mode: bool=False, model=None, tokenizer=None, model_eval=True):
+    def __init__(self, pretrained_model:Optional[str]=None, gpu_mode: bool=False, model=None, tokenizer=None, model_eval=True, torch_dtype='auto'):
         if pretrained_model is None and (model is None or tokenizer is None):
             raise Exception("pretrained_model and (model, tokenizer) must not be both None")
         super(Model4TritonServer, self).__init__()
         if model is None and pretrained_model is not None:
-            self.model = AutoModel.from_pretrained(pretrained_model, torchscript=True)
+            self.model = AutoModel.from_pretrained(pretrained_model, torchscript=True, torch_dtype=torch_dtype)
         elif model is not None:
             self.model = model
 
         if tokenizer is None and pretrained_model is not None:
             self.tokenizer = AutoTokenizer.from_pretrained(pretrained_model)
         elif tokenizer is not None:
             self.tokenizer = tokenizer
```

### Comparing `triton_bert-0.3.0/triton_bert/pgvector_triton.py` & `triton_bert-0.3.2/triton_bert/vector_db/pgvector_triton.py`

 * *Files identical despite different names*

### Comparing `triton_bert-0.3.0/triton_bert/tests/dataset/medical_qa.jsonl` & `triton_bert-0.3.2/triton_bert/tests/dataset/medical_qa.jsonl`

 * *Files identical despite different names*

### Comparing `triton_bert-0.3.0/triton_bert/tests/test_biencoder.py` & `triton_bert-0.3.2/triton_bert/tests/test_biencoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         if self.normalize_vector:
             #if you use IP, you must normalize the vector which is the same as cosine
             return [(x /np.linalg.norm(x)).tolist() for x in triton_output[0]]
         #milvus accept list type vector
         return triton_output[0].tolist()
 
 if __name__ == "__main__":
-    model = Biencoder(triton_host="30.171.160.44", model="sbert_onnx",
-                       vocab="/Users/yanyongwen712/.cache/torch/sentence_transformers/sentence-transformers_all-MiniLM-L6-v2")
+    model = Biencoder(triton_host="xxx", model="sbert_onnx",
+                       vocab="/Users/xxxx/.cache/torch/sentence_transformers/sentence-transformers_all-MiniLM-L6-v2")
 
     # batch inferences
     vectors = model(["基金的收益率是多少？", "我有个朋友的股票天天涨停"])
     # or
     # vectors = model.encodes(["基金的收益率是多少？", "我有个朋友的股票天天涨停"])
     assert len(vectors) == 2
```

### Comparing `triton_bert-0.3.0/triton_bert/tests/test_chitchat.py` & `triton_bert-0.3.2/triton_bert/tests/test_chitchat.py`

 * *Files identical despite different names*

### Comparing `triton_bert-0.3.0/triton_bert/tests/test_crossencoder.py` & `triton_bert-0.3.2/triton_bert/tests/test_crossencoder.py`

 * *Files identical despite different names*

### Comparing `triton_bert-0.3.0/triton_bert/tests/test_generate_bgem3_triton_model.py` & `triton_bert-0.3.2/triton_bert/tests/test_generate_bgem3_triton_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,9 +45,9 @@
         return torch.nn.functional.normalize(dense_vecs, dim=-1) if self.normlized else dense_vecs
 
 if __name__ == "__main__":
     pretrained_model = "BAAI/bge-m3"
     n = BGEM3ForTritonInference(pretrained_model)
 
     model = Model4TritonServer(model=n.model, tokenizer=n.tokenizer)
-    model.save_torchscript("model/bgem3_model.pt")
+    #model.save_torchscript("model/bgem3_model.pt")
     model.save_onnx("model/bgem3_model.onnx")
```

### Comparing `triton_bert-0.3.0/triton_bert/tests/test_pgvector_triton.py` & `triton_bert-0.3.2/triton_bert/tests/test_pgvector_triton.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,19 +29,19 @@
         return [self.TABLE_MODEL(answer=text, embedding=embedding, question=question) for text, embedding, question in zip(texts, embeddings, kwargs['questions']) ]
 
 
 if __name__ == "__main__":
     '''
     TEST 1
     '''
-    instance = PgvectorTriton(db_user="budevadmin", db_password='eimdmPOSTGRESQL@2023',
-                              db_instance="D0PEIMDMINFO-postgresql.dbdev.paic.com.cn", db_port="3671",
-                   db_schema="pivotoperation", create_table=True,
-                   triton_host="30.171.160.44", model="bge-m3",
-                   vocab="/Users/yanyongwen712/Codes/pingan_health_rag/models/bge-m3",
+    instance = PgvectorTriton(db_user="xx", db_password='xxx',
+                              db_instance="xxx", db_port="3671",
+                   db_schema="xx", create_table=True,
+                   triton_host="xx", model="bge-m3",
+                   vocab="/Users/xx/Codes/pingan_health_rag/models/bge-m3",
                               table_model=Sentence
                    )
 
     '''
     qas = instance.load_texts("dataset/medical_qa.jsonl")
     answers = [qa['answers'][0] for qa in qas]
     instance.insert_vectors(answers)
@@ -50,19 +50,19 @@
     recalls: List[Sentence] = instance.retrieval_vectors("我喉咙有些干")
 
     print(recalls[0].sentence)
 
     '''
     TEST 2
     '''
-    instance = PgvectorTritonCustomized(db_user="budevadmin", db_password='eimdmPOSTGRESQL@2023',
-                              db_instance="D0PEIMDMINFO-postgresql.dbdev.paic.com.cn", db_port="3671",
-                   db_schema="pivotoperation", create_table=True,
-                   triton_host="30.171.160.44", model="bge-m3",
-                   vocab="/Users/yanyongwen712/Codes/pingan_health_rag/models/bge-m3",
+    instance = PgvectorTritonCustomized(db_user="xx", db_password='xxx',
+                              db_instance="xx", db_port="3671",
+                   db_schema="xx", create_table=True,
+                   triton_host="xx", model="bge-m3",
+                   vocab="/Users/xx/Codes/pingan_health_rag/models/bge-m3",
                               table_model=QA)
 
     qas = instance.load_texts("dataset/medical_qa.jsonl")
     answers = [qa['answers'][0] for qa in qas]
     questions = [qa['questions'][0][0] for qa in qas]
     instance.insert_vectors(answers, questions=questions)
```

### Comparing `triton_bert-0.3.0/triton_bert/tests/test_triton_bert.py` & `triton_bert-0.3.2/triton_bert/tests/test_triton_bert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from triton_bert.triton_bert import TritonBert
 
 if __name__ == "__main__":
-    model = TritonBert(triton_host="30.171.160.44", model="sbert_onnx", vocab="/Users/yanyongwen712/.cache/torch/sentence_transformers/sentence-transformers_all-MiniLM-L6-v2")
+    model = TritonBert(triton_host="xxx", model="sbert_onnx", vocab="/Users/xxxxx/.cache/torch/sentence_transformers/sentence-transformers_all-MiniLM-L6-v2")
 
     #use for batch inference
     vectors = model(["基金的收益率是多少？", "我有个朋友的股票天天涨停"])
     assert len(vectors) == 2
     vectors = model.encode(["基金的收益率是多少？", "我有个朋友的股票天天涨停"])
     assert len(vectors) == 2
```

### Comparing `triton_bert-0.3.0/triton_bert/triton_bert.py` & `triton_bert-0.3.2/triton_bert/triton_bert.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 from transformers.tokenization_utils_base import TruncationStrategy
 from tritonclient.utils import InferenceServerException, triton_to_np_dtype
 
 class TritonBert:
     def __init__(self, model: str, vocab: str, triton_host: str="localhost", triton_grpc_port: int=8001, 
         model_max_len: int=512, padding: Optional[PaddingStrategy]=None, 
         truncation: TruncationStrategy=TruncationStrategy.LONGEST_FIRST):
+        
+        self.tokenizer = AutoTokenizer.from_pretrained(vocab)
+        
         self.triton_url = f"{triton_host}:{triton_grpc_port}"
         self.connect_triton()
         
         self.model = model
         self.model_max_len = model_max_len
         self.padding = padding
         self.truncation = truncation
         self.parse_triton_model_config()
 
-        self.tokenizer = AutoTokenizer.from_pretrained(vocab)
+        
 
     def connect_triton(self):
         self.triton_client = grpcclient.InferenceServerClient(url=self.triton_url)
 
     def parse_triton_model_config(self):
         model_config = self.triton_client.get_model_config(self.model, as_json=True)
         self.model_config = model_config
```

### Comparing `triton_bert-0.3.0/PKG-INFO` & `triton_bert-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: triton-bert
-Version: 0.3.0
+Version: 0.3.2
 Summary: easy to use bert with nvidia triton inference server
 License: MIT
-Author: yanyongwen712
-Author-email: yanyongwen712@pingan.com.cn
+Author: yyw794
+Author-email: yyw794@126.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -42,16 +42,16 @@
 embedding output from model can be used directly.
 so no need to override the proprocess function.
 
 ```python
 from triton_bert.triton_bert import TritonBert
 
 if __name__ == "__main__":
-    model = TritonBert(triton_host="30.171.160.44", model="sbert_onnx", 
-                       vocab="/Users/yanyongwen712/.cache/torch/sentence_transformers/sentence-transformers_all-MiniLM-L6-v2")
+    model = TritonBert(triton_host="127.0.0.1", model="sbert_onnx", 
+                       vocab="/Users/xxx/.cache/torch/sentence_transformers/sentence-transformers_all-MiniLM-L6-v2")
 
     # batch inferences
     vectors = model(["基金的收益率是多少？", "我有个朋友的股票天天涨停"])
     # or
     vectors = model.encode(["基金的收益率是多少？", "我有个朋友的股票天天涨停"])
     assert len(vectors) == 2
 
@@ -135,41 +135,41 @@
 
 ```
 
 # run examples
 ## run triton server
 ```bash
 # for example
-docker run -d  --name triton-server   --shm-size=1g --ulimit memlock=-1 --ulimit stack=67108864  --rm -p 8000:8000 -p 8001:8001 -p 8002:8002 -v /home/yanyongwen712/triton_models:/models  nvcr.io/nvidia/tritonserver::22.08-py3 tritonserver --model-repository=/models  --model-control-mode=poll  --exit-on-error=false --log-verbose 1
+docker run -d  --name triton-server   --shm-size=1g --ulimit memlock=-1 --ulimit stack=67108864  --rm -p 8000:8000 -p 8001:8001 -p 8002:8002 -v /home/xxxx/triton_models:/models  nvcr.io/nvidia/tritonserver::22.08-py3 tritonserver --model-repository=/models  --model-control-mode=poll  --exit-on-error=false --log-verbose 1
 # configure triton model folder
 ```
 ## prepare model for triton server
 See the tests for more examples.
 
 Example:
 ```python
 from triton_bert.model_4_triton import Model4TritonServer
 
 if __name__ == "__main__":
-    pretrained_model = "/Users/yanyongwen712/.cache/torch/sentence_transformers/simcse-chinese-roberta-wwm-ext"
+    pretrained_model = "/Users/xxxxx/.cache/torch/sentence_transformers/simcse-chinese-roberta-wwm-ext"
     model = Model4TritonServer(pretrained_model=pretrained_model)
     model.save_torchscript("model/simcse_model.pt")
     model.save_onnx("model/simcse_model.onnx")
 
 ```
 
 # Semantic Retrieval with Postgresql/pgvector
 Example 1
 ```python
 
-    instance = PgvectorTriton(db_user="budevadmin", db_password='eimdmPOSTGRESQL@2023',
-                              db_instance="D0PEIMDMINFO-postgresql.dbdev.paic.com.cn", db_port="3671",
-                   db_schema="pivotoperation", create_table=True,
-                   triton_host="30.171.160.44", model="bge-m3",
-                   vocab="/Users/yanyongwen712/Codes/pingan_health_rag/models/bge-m3",
+    instance = PgvectorTriton(db_user="xxx", db_password='xxxx',
+                              db_instance="xxxx", db_port="3671",
+                   db_schema="xxx", create_table=True,
+                   triton_host="xxx", model="bge-m3",
+                   vocab="/Users/xxx/Codes/pingan_health_rag/models/bge-m3",
                               table_model=Sentence
                    )
 
     # insert
     qas = instance.load_texts("dataset/medical_qa.jsonl")
     answers = [qa['answers'][0] for qa in qas]
     instance.insert_vectors(answers)
```


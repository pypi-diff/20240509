# Comparing `tmp/tweets_to_topic_network-0.1.3.tar.gz` & `tmp/tweets_to_topic_network-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweets_to_topic_network-0.1.3.tar", max compression
+gzip compressed data, was "tweets_to_topic_network-0.1.4.tar", max compression
```

## Comparing `tweets_to_topic_network-0.1.3.tar` & `tweets_to_topic_network-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2024-04-11 12:12:13.477841 tweets_to_topic_network-0.1.3/LICENSE
--rw-r--r--   0        0        0    13264 2024-04-16 17:38:24.238044 tweets_to_topic_network-0.1.3/README.md
--rw-r--r--   0        0        0      738 2024-04-16 17:41:26.586531 tweets_to_topic_network-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-16 17:41:11.397030 tweets_to_topic_network-0.1.3/tweets_to_topic_network/__init__.py
--rw-r--r--   0        0        0     8171 2024-04-16 15:33:49.288519 tweets_to_topic_network-0.1.3/tweets_to_topic_network/data.py
--rw-r--r--   0        0        0    10831 2024-04-11 12:12:13.484495 tweets_to_topic_network-0.1.3/tweets_to_topic_network/network.py
--rw-r--r--   0        0        0     8697 2024-04-16 16:14:51.525205 tweets_to_topic_network-0.1.3/tweets_to_topic_network/topic.py
--rw-r--r--   0        0        0    14188 1970-01-01 00:00:00.000000 tweets_to_topic_network-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 12:12:13.477841 tweets_to_topic_network-0.1.4/LICENSE
+-rw-r--r--   0        0        0    13380 2024-05-09 17:14:43.252015 tweets_to_topic_network-0.1.4/README.md
+-rw-r--r--   0        0        0      799 2024-05-09 17:14:53.182988 tweets_to_topic_network-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-04-16 17:41:11.397030 tweets_to_topic_network-0.1.4/tweets_to_topic_network/__init__.py
+-rw-r--r--   0        0        0     7924 2024-04-18 11:53:20.230781 tweets_to_topic_network-0.1.4/tweets_to_topic_network/data.py
+-rw-r--r--   0        0        0    10831 2024-04-11 12:12:13.484495 tweets_to_topic_network-0.1.4/tweets_to_topic_network/network.py
+-rw-r--r--   0        0        0     9952 2024-05-09 17:13:26.067271 tweets_to_topic_network-0.1.4/tweets_to_topic_network/topic.py
+-rw-r--r--   0        0        0    14428 1970-01-01 00:00:00.000000 tweets_to_topic_network-0.1.4/PKG-INFO
```

### Comparing `tweets_to_topic_network-0.1.3/LICENSE` & `tweets_to_topic_network-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.3/README.md` & `tweets_to_topic_network-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 
 
 ```
 
 # Classes
 The pipeline is divided into three classes, each of them is independent and can be used separately.
 
-- *Data_processor*: takes the two json files (or just one) and creates a pandas dataframe with all the tweets in english. It also creates a cache of the dataframe in csv and pickle format.
+- *Data_processor*: takes the two json files (or just one) and creates a pandas dataframe with all the tweets . It also creates a cache of the dataframe in csv and pickle format.
 
 - *Topic_modeler*: takes a dataframe and labels the tweets with a topic using BERTopic. It also creates a cache of the labeled dataframe in csv and pickle format.
 
 - *Network_creator*: takes a dataframe of tweets and creates a network from it. It can create a retweet network, a temporal text network, and a multilayer network. The networks are saved in gml format.
 
 
 ## Data Processor
@@ -182,15 +182,16 @@
 ```python
 tm = Topic_modeler(data.df_original, name = data.name, embedder_name='all-MiniLM-L6-v2', path_cache = data.path_cache)
 df_labeled = tm.get_topics()
 
 
 ```
 ### label topics (todo)
-we use openai gpt3.5turbo model to label the topic using the putput of the cTFIDF and some representative tweets. 
+we use openai gpt3.5turbo model to label the topic using the putput of the cTFIDF and some representative tweets. if you want to use openai api, you need an env variable with the api key, otherwise it will not work. 
+OPENAI_API_KEY=sk-xxxxx
 
 ## Network Creator
 Finally we can create the networks using the full dataframe with topic labels. there are 3 possible types of network you can create
 
 ```python
 nw = Network_creator(df_retweet_labeled, name = data.name, path = data.folder)
 ```
```

### Comparing `tweets_to_topic_network-0.1.3/pyproject.toml` & `tweets_to_topic_network-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tweets-to-topic-network"
-version = "0.1.3"
+version = "0.1.4"
 description = "start from a set of tweets and create a multilayer network where each layer is a topic"
 authors = ["alessiogandelli <alessiogandelli99@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tweets_to_topic_network"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
@@ -15,14 +15,17 @@
 openai = "^1.17.0"
 typing-extensions = "^4.11.0"
 qdrant-client = "^1.8.2"
 uunet = "^2.1.1"
 networkx = "^3.3"
 igraph = "^0.11.4"
 fastembed = "^0.2.6"
+umap-learn = "^0.5.6"
+langchain = "^0.1.16"
+flask = "^3.0.3"
 
 
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 
 [build-system]
```

### Comparing `tweets_to_topic_network-0.1.3/tweets_to_topic_network/data.py` & `tweets_to_topic_network-0.1.4/tweets_to_topic_network/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,40 +96,37 @@
 
         df_user = pd.DataFrame(users).T
         return df_user
 
     def _load_tweets_json(self, users):
         print('looking into tweets json file')
         tweets = {}
-        attachments = 0
         with jsonlines.open(self.file_tweets) as reader: # open file
             for obj in reader:
-                if obj.get('attachments') is  None : # avoid tweets with attachments (should be analyzed with )
-                    tweets[obj.get('id', 0)] = {'author': obj['author_id'], 
-                                                'author_name': users.get(obj['author_id'], {}).get('username'),
-                                                'text': obj.get('text', ''), 
-                                                'date': obj.get('created_at', ''),
-                                                'lang':obj.get('lang', ''),
-                                                # 'reply_count': obj.get('public_metrics', {}).get('reply_count', 0), 
-                                                # 'retweet_count': obj.get('public_metrics', {}).get('retweet_count', 0), 
-                                                # 'like_count': obj.get('public_metrics', {}).get('like_count', 0), 
-                                                # 'quote_count': obj.get('public_metrics', {}).get('quote_count', 0),
-                                                #'impression_count': obj['public_metrics']['impression_count'],
-                                                'conversation_id': obj.get('conversation_id', None),
-                                                'referenced_type': obj.get('referenced_tweets', [{}])[0].get('type', None),
-                                                'referenced_id': obj.get('referenced_tweets', [{}])[0].get('id', None),
-                                                'mentions_name': [ann.get('username', '') for ann in obj.get('entities',  {}).get('mentions', [])],
-                                                'mentions_id': [ann.get('id', '') for ann in obj.get('entities',  {}).get('mentions', [])],
-                                                'cop':  self.n_cop
-                                                # 'context_annotations': [ann.get('entity').get('name') for ann in obj.get('context_annotations', [])]
-                                                }
-                else:
-                    attachments+=1
+                tweets[obj.get('id', 0)] = {'author': obj['author_id'], 
+                                            'author_name': users.get(obj['author_id'], {}).get('username'),
+                                            'text': obj.get('text', ''), 
+                                            'date': obj.get('created_at', ''),
+                                            'lang':obj.get('lang', ''),
+                                            # 'reply_count': obj.get('public_metrics', {}).get('reply_count', 0), 
+                                            # 'retweet_count': obj.get('public_metrics', {}).get('retweet_count', 0), 
+                                            # 'like_count': obj.get('public_metrics', {}).get('like_count', 0), 
+                                            # 'quote_count': obj.get('public_metrics', {}).get('quote_count', 0),
+                                            #'impression_count': obj['public_metrics']['impression_count'],
+                                            'conversation_id': obj.get('conversation_id', None),
+                                            'referenced_type': obj.get('referenced_tweets', [{}])[0].get('type', None),
+                                            'referenced_id': obj.get('referenced_tweets', [{}])[0].get('id', None),
+                                            'mentions_name': [ann.get('username', '') for ann in obj.get('entities',  {}).get('mentions', [])],
+                                            'mentions_id': [ann.get('id', '') for ann in obj.get('entities',  {}).get('mentions', [])],
+                                            'attachments': obj.get('attachments', None),
+                                            'cop':  self.n_cop
+                                            # 'context_annotations': [ann.get('entity').get('name') for ann in obj.get('context_annotations', [])]
+                                            }
+
 
-            print('discarded ',attachments ,'tweets with attachments')
 
         df_tweets = pd.DataFrame(tweets).T
         return df_tweets
     
     def _log_info(self):
         print('Data processed')
         print('Tweets:', self.df_tweets.shape[0])
```

### Comparing `tweets_to_topic_network-0.1.3/tweets_to_topic_network/network.py` & `tweets_to_topic_network-0.1.4/tweets_to_topic_network/network.py`

 * *Files identical despite different names*

### Comparing `tweets_to_topic_network-0.1.3/tweets_to_topic_network/topic.py` & `tweets_to_topic_network-0.1.4/tweets_to_topic_network/topic.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,46 +3,54 @@
 import numpy as np
 import datetime
 import re
 from sentence_transformers import SentenceTransformer
 from bertopic import BERTopic
 from sklearn.feature_extraction.text import CountVectorizer
 from bertopic.vectorizers import ClassTfidfTransformer
-import openai
 from qdrant_client import QdrantClient, models
 from fastembed import TextEmbedding
-from bertopic.representation import OpenAI
 import pickle 
+from umap import UMAP
+from langchain import PromptTemplate
+from langchain.llms import OpenAI as LLMOpenAI
+from bertopic.representation import OpenAI as BERTOpenAI
+
+from langchain.chains import LLMChain
+from openai import OpenAI
+
+try:
+    openai_client = OpenAI()
+except:
+    openai_client = None
 
 
 
 os.environ['TOKENIZERS_PARALLELISM'] = 'false' # to avoid a warning 
-openai.api_key = os.getenv("OPENAI_API_KEY")    
 qdrant_client = QdrantClient(os.getenv("QDRANT_URL")) # vector database saved in memory
-openai_client = openai.OpenAI(api_key=os.getenv("OPENAI_API_KEY")) # openai api key
-
 collection_name = 'cop'
 
 
 class Topic_modeler:
 
     def __init__(self, df, embedder_name = 'all-MiniLM-L6-v2', path_cache = '/cache', name = 'cop') -> None:
         self.df = df
         self.path_cache = path_cache
         self.embedder_name = embedder_name
         self.name = name
 
-        self.df_labeled_path = os.path.join(self.path_cache, 'data' ,'tweets_'+self.name+'_topics.pkl')
         self.tm_path = os.path.join(self.path_cache,'tm', self.embedder_name)
+        self.df_labeled_path = os.path.join(self.tm_path,'tweets_'+self.name+'_labeled.pkl')
         self.model_path = os.path.join( self.tm_path, 'model_'+self.name)
         self.embeddings_path = os.path.join( self.tm_path ,'embeddings_'+self.name+'.pkl')
         self.topic_path = os.path.join( self.tm_path ,'topics_'+self.name+'.csv')
 
         self.model = None
         self.embeddings = None
+        self.docs = None
         
 
     def get_topics(self):
         """
         Main function of the class, get the topics of the original tweets and updates the dataframe with the topics and topic probabilities. 
         then save the embeddings in qdrant and save the labeled dataframe in the cache folder.
 
@@ -53,25 +61,29 @@
             os.makedirs(self.path_cache)
         
         if not os.path.exists(self.tm_path):
             os.makedirs(self.tm_path)
 
         
         # if pkl file of the labeled df exists, load it from the cache
-        if os.path.exists(self.df_labeled_path) and os.path.exists(self.model_path) and os.path.exists(self.embeddings_path):
+        if os.path.exists(self.df_labeled_path) and os.path.exists(self.model_path) :
             print('using cached topics')
             self.df = pd.read_pickle(self.df_labeled_path)
             self.model = BERTopic.load(self.model_path)
-            self.embeddings = pickle.load(open(self.embeddings_path, 'rb'))
+            self.docs = self.df['new_text'].tolist()
         else:
             print('running topic modeling')
     
             docs = self._preprocess()
             print( '    ',datetime.datetime.now() - time, ' for preprocessing')
-            self._get_embeddings(docs)
+            if os.path.exists(self.embeddings_path):
+                print('   loading embeddings from cache')
+                self.embeddings = pickle.load(open(self.embeddings_path, 'rb'))
+            else:
+                self._get_embeddings(docs)
             print( '    ',datetime.datetime.now() - time, ' for embeddings')
             self._use_BERTopic(docs)
             print( '    ',datetime.datetime.now() - time, ' for bertopic')
             self._save_embeddings(docs)
             print( '    ',datetime.datetime.now() - time, ' for saving embeddings')
             self._save_files()
             print( '    ',datetime.datetime.now() - time, ' for saving files')
@@ -92,66 +104,68 @@
         self.df['new_text'] =  self.df['new_text'].str.replace(r"\n", "")
         self.df['new_text'] =  self.df['new_text'].str.strip()
 
         # if new text is empty delete the row
         self.df = self.df[self.df['new_text'] != '']
 
         docs = self.df['new_text'].tolist()
+        self.docs = docs
 
         
         return docs
 
     def _get_embeddings(self, docs):
 
-        embeddings_file = os.path.join(self.path_cache, 'embeddings_' + self.name + '.pkl')
 
-        if os.path.exists(embeddings_file):
+        if os.path.exists(self.embeddings_path):
             try:
-                self.embeddings = pickle.load(open(embeddings_file, 'rb'))
+                self.embeddings = pickle.load(open(self.embeddings_path, 'rb'))
                 return
             except Exception as e:
                 print(f"Error loading embeddings from cache: {e}")
 
         print('     Embeddings not found in cache, using' + self.embedder_name + ' to get embeddings')
 
 
-        if(self.embedder_name == 'text-embedding-ada-002'):
-            embs = openai.Embedding.create(input = docs, model="text-embedding-ada-002")['data']
-            self.embedder = None
-            self.embeddings = np.array([np.array(emb['embedding']) for emb in embs])
-        elif(self.embedder_name == 'text-embedding-3-large'):
-            embs = openai.Embedding.create(input = docs, model="text-embedding-3-large")['data']
-            self.embedder = None
-            self.embeddings = np.array([np.array(emb['embedding']) for emb in embs])
-        
-        elif(self.embedder_name == 'text-embedding-3-small'):
-            embs = openai.Embedding.create(input = docs, model="text-embedding-3-small")['data']
+        if(self.embedder_name.startswith('text-embedding')):
+            print('         using openai')
+
+            batch_size = 1000
+            num_batches = len(self.docs) // batch_size + (len(self.docs) % batch_size != 0)
+            self.embeddings = []
+
+            for i in range(num_batches):
+                print(f'         batch {i+1}/{num_batches}')
+                batch = self.docs[i*batch_size:(i+1)*batch_size]
+                print(batch[:5])
+                embs = openai_client.embeddings.create(input = batch, model=self.embedder_name).data
+                self.embeddings.extend([np.array(emb.embedding) for emb in embs])
+
             self.embedder = None
-            self.embeddings = np.array([np.array(emb['embedding']) for emb in embs])
+            self.embeddings = np.array(self.embeddings)
         else:
             self.embedder = SentenceTransformer(self.embedder_name)
             self.embeddings = self.embedder.encode(docs)
         
                 #save embeddings to pickle file
-        with open(embeddings_file, 'wb') as f:
+        with open(self.embeddings_path, 'wb') as f:
             pickle.dump(self.embeddings, f)
 
     def _use_BERTopic(self, docs):
         vectorizer_model = CountVectorizer(stop_words="english") 
         # we can also change some parameter of the cTFIDF model https://maartengr.github.io/BERTopic/getting_started/ctfidf/ctfidf.html#reduce_frequent_words
         ctfidf_model = ClassTfidfTransformer(reduce_frequent_words=True)
-        representation_model = OpenAI(openai_client, model="gpt-3.5-turbo", delay_in_seconds=10, chat=True)
+        representation_model = BERTOpenAI(openai_client, model="gpt-3.5-turbo", chat=True)
 
         model = BERTopic( 
                             vectorizer_model =   vectorizer_model,
                             ctfidf_model      =   ctfidf_model,
                             nr_topics        =  'auto',
                             min_topic_size   =   max(int(len(docs)/800),10),
-                            embedding_model  = self.embedder,
-                            #representation_model = representation_model
+                            representation_model = representation_model
                         )
         print('         model created')
         
         try:
             topics ,probs = model.fit_transform(docs, embeddings = self.embeddings)
             self.df['topic'] = topics    
             self.df['topic_prob'] = probs   
@@ -201,23 +215,55 @@
 
         except(Exception) as e:
             print(e)
             print('error in saving vectors in qdrant')
 
     def _save_files(self):
         self.df.to_pickle(self.df_labeled_path)
-        self.model.save(self.model_path, serialization="safetensors", save_ctfidf=True)
+        self.model.save(self.model_path, serialization="safetensors", save_ctfidf=True, save_embedding_model=self.embedder_name)
 
     def label_topics(self):
-        prompt = """
+        template = """
         I have a topic that contains the following documents: 
-        [DOCUMENTS]
-        The topic is described by the following keywords: [KEYWORDS]
+        [{DOCUMENTS}]
+        The topic is described by the following keywords: [{KEYWORDS}]
 
         Based on the information above, extract a short topic label in the following format:
         topic: <topic label>
         """
+        llm = LLMOpenAI(temperature=0.3)
 
+        prompt = PromptTemplate(
+            input_variables=["DOCUMENTS", 'KEYWORDS'],
+            template=template
+        )
+
+        chain = LLMChain(llm=llm, prompt=prompt)
 
 
         pass
-       
+    
+    def visualize_topics(self):
+        return self.model.visualize_topics()
+    
+    def visualize_hierarchical_topics(self):
+        hierarchical_topics =  self.model.hierarchical_topics(self.docs)
+        self.model.visualize_hierarchy()
+
+    def get_topic_tree(self):
+        hierarchical_topics =  self.model.hierarchical_topics(self.docs)
+        return self.model.get_topic_tree(hierarchical_topics)
+    
+    def visualize_docs(self):
+        # Reduce dimensionality of embeddings, this step is optional but much faster to perform iteratively:
+        reduced_embeddings = UMAP(n_neighbors=10, n_components=2, min_dist=0.0, metric='cosine').fit_transform(self.embeddings)
+        return self.model.visualize_documents(self.docs, reduced_embeddings=reduced_embeddings)
+    
+    def visualize_topic_similarity(self):
+        return self.model.visualize_heatmap()
+    
+    def visualize_terms(self):
+        return self.model.visualize_barchart()
+    
+
+
+
```

### Comparing `tweets_to_topic_network-0.1.3/PKG-INFO` & `tweets_to_topic_network-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: tweets-to-topic-network
-Version: 0.1.3
+Version: 0.1.4
 Summary: start from a set of tweets and create a multilayer network where each layer is a topic
 Author: alessiogandelli
 Author-email: alessiogandelli99@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bertopic (>=0.16.0,<0.17.0)
 Requires-Dist: fastembed (>=0.2.6,<0.3.0)
+Requires-Dist: flask (>=3.0.3,<4.0.0)
 Requires-Dist: igraph (>=0.11.4,<0.12.0)
 Requires-Dist: jsonlines (>=4.0.0,<5.0.0)
+Requires-Dist: langchain (>=0.1.16,<0.2.0)
 Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: openai (>=1.17.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: qdrant-client (>=1.8.2,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.6.1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
+Requires-Dist: umap-learn (>=0.5.6,<0.6.0)
 Requires-Dist: uunet (>=2.1.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # tweets-to-network
 ```bash
 pip install tweets-to-topic-network
 ```
@@ -167,15 +170,15 @@
 
 
 ```
 
 # Classes
 The pipeline is divided into three classes, each of them is independent and can be used separately.
 
-- *Data_processor*: takes the two json files (or just one) and creates a pandas dataframe with all the tweets in english. It also creates a cache of the dataframe in csv and pickle format.
+- *Data_processor*: takes the two json files (or just one) and creates a pandas dataframe with all the tweets . It also creates a cache of the dataframe in csv and pickle format.
 
 - *Topic_modeler*: takes a dataframe and labels the tweets with a topic using BERTopic. It also creates a cache of the labeled dataframe in csv and pickle format.
 
 - *Network_creator*: takes a dataframe of tweets and creates a network from it. It can create a retweet network, a temporal text network, and a multilayer network. The networks are saved in gml format.
 
 
 ## Data Processor
@@ -205,15 +208,16 @@
 ```python
 tm = Topic_modeler(data.df_original, name = data.name, embedder_name='all-MiniLM-L6-v2', path_cache = data.path_cache)
 df_labeled = tm.get_topics()
 
 
 ```
 ### label topics (todo)
-we use openai gpt3.5turbo model to label the topic using the putput of the cTFIDF and some representative tweets. 
+we use openai gpt3.5turbo model to label the topic using the putput of the cTFIDF and some representative tweets. if you want to use openai api, you need an env variable with the api key, otherwise it will not work. 
+OPENAI_API_KEY=sk-xxxxx
 
 ## Network Creator
 Finally we can create the networks using the full dataframe with topic labels. there are 3 possible types of network you can create
 
 ```python
 nw = Network_creator(df_retweet_labeled, name = data.name, path = data.folder)
 ```
```


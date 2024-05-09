# Comparing `tmp/answerrocket_client-0.2.0.tar.gz` & `tmp/answerrocket_client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "answerrocket_client-0.2.0.tar", last modified: Fri May  3 17:14:37 2024, max compression
+gzip compressed data, was "answerrocket_client-0.2.1.tar", last modified: Thu May  9 15:21:00 2024, max compression
```

## Comparing `answerrocket_client-0.2.0.tar` & `answerrocket_client-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.170405 answerrocket_client-0.2.0/answer_rocket/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12592 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/answer_rocket/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/graphql/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    45437 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/graphql/sdk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/skill.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/answer_rocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/answerrocket_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 17:14:37.000000 answerrocket_client-0.2.0/answerrocket_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:14:37.174406 answerrocket_client-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-03 17:14:33.000000 answerrocket_client-0.2.0/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:21:00.281471 answerrocket_client-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-09 15:21:00.281471 answerrocket_client-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:21:00.281471 answerrocket_client-0.2.1/answer_rocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12592 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:21:00.281471 answerrocket_client-0.2.1/answer_rocket/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/graphql/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46555 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/graphql/sdk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/answer_rocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:21:00.281471 answerrocket_client-0.2.1/answerrocket_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-09 15:21:00.000000 answerrocket_client-0.2.1/answerrocket_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-09 15:21:00.000000 answerrocket_client-0.2.1/answerrocket_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:21:00.000000 answerrocket_client-0.2.1/answerrocket_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 15:21:00.000000 answerrocket_client-0.2.1/answerrocket_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 15:21:00.000000 answerrocket_client-0.2.1/answerrocket_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:21:00.281471 answerrocket_client-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:21:00.281471 answerrocket_client-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 15:20:37.000000 answerrocket_client-0.2.1/test/test_client.py
```

### Comparing `answerrocket_client-0.2.0/PKG-INFO` & `answerrocket_client-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.0/answer_rocket/auth.py` & `answerrocket_client-0.2.1/answer_rocket/auth.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.0/answer_rocket/chat.py` & `answerrocket_client-0.2.1/answer_rocket/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from sgqlc.types import Variable, non_null, String, Arg, Boolean, list_of
 from sgqlc.operation import Fragment
 
 from answer_rocket.auth import AuthHelper
 from answer_rocket.graphql.client import GraphQlClient
 from answer_rocket.graphql.schema import (LLMApiConfig, AzureOpenaiCompletionLLMApiConfig,
                                           AzureOpenaiEmbeddingLLMApiConfig, OpenaiCompletionLLMApiConfig,
-                                          OpenaiEmbeddingLLMApiConfig, UUID, Int, DateTime, ChatDryRunType)
+                                          OpenaiEmbeddingLLMApiConfig, UUID, Int, DateTime, ChatDryRunType,
+                                          MaxChatEntry, MaxChatThread)
 from answer_rocket.graphql.sdk_operations import Operations
 
 
 logger = logging.getLogger(__name__)
 
 ModelType = Literal['COMPLETION', 'EMBEDDING']
 ApiType = Literal['AZURE', 'OPENAI']
@@ -145,15 +146,14 @@
             except Exception as e:
                 time.sleep(retry_sleep_time)
                 last_error = e
                 retry_sleep_time *= error_backoff_multiplier
 
         return False, str(last_error)
 
-
     def ask_question(self, copilot_id: str, question: str, thread_id: str = None, skip_report_cache: bool = False, dry_run_type: str = None):
         """
         Calls the Max chat pipeline to answer a natural language question and receive analysis and insights
         in response.
         :param copilot_id: the ID of the copilot to run the question against
         :param question: The natural language question to ask the engine.
         :param thread_id: (optional) ID of the thread/conversation to run the question on. The question and answer will
@@ -260,14 +260,77 @@
             evals=Variable('evals'),
         )
 
         result = self.gql_client.submit(operation, evaluate_entry_mutation_args)
 
         return result.evaluate_chat_question
 
+    def get_chat_entry(self, entry_id: str) -> MaxChatEntry:
+        get_chat_entry_args = {
+            'id': UUID(entry_id),
+        }
+
+        op = Operations.query.chat_entry
+        result = self.gql_client.submit(op, get_chat_entry_args)
+        return result.chat_entry
+
+    def get_chat_thread(self, thread_id: str) -> MaxChatThread:
+        get_chat_thread_args = {
+            'id': UUID(thread_id),
+        }
+
+        op = Operations.query.chat_thread
+        result = self.gql_client.submit(op, get_chat_thread_args)
+        return result.chat_thread
+
+    def create_new_thread(self, copilot_id: str) -> MaxChatThread:
+        create_chat_thread_args = {
+            'copilotId': copilot_id,
+        }
+
+        op = Operations.mutation.create_chat_thread
+        result = self.gql_client.submit(op, create_chat_thread_args)
+        return result.create_chat_thread
+
+    def queue_chat_question(self, question: str, thread_id: str, skip_cache: bool = False) -> MaxChatEntry:
+        """
+        This queues up a question for processing. Unlike ask_question, this will not wait for the processing to
+        complete. It will immediately return a shell entry with an id you can use to query for the results.
+        :param question: the text of the user's question
+        :param thread_id: id of the thread the question is being sent to.
+        :param skip_cache: Set to true to force a fresh run of the question, ignoring any existing skill result caches.
+        :return:
+        """
+        queue_chat_question_args = {
+            'question': question,
+            'skipCache': skip_cache,
+            'threadId': thread_id
+        }
+
+        op = Operations.mutation.queue_chat_question
+
+        result = self.gql_client.submit(op, queue_chat_question_args)
+
+        return result.queue_chat_question
+
+    def cancel_chat_question(self, entry_id: str) -> MaxChatEntry:
+        """
+        This deletes the entry from its thread and attempts to abandon the question's processing if it is still ongoing.
+        :param entry_id: the id of the chat entry
+        :return: the deleted entry
+        """
+        cancel_chat_question_args = {
+            'entryId': entry_id,
+        }
+
+        op = Operations.mutation.cancel_chat_question
+
+        result = self.gql_client.submit(op, cancel_chat_question_args)
+
+        return result.cancel_chat_question
 
 
 def _create_llm_config_fragments():
     azure_completion_fragment = Fragment(AzureOpenaiCompletionLLMApiConfig, 'AzureCompletionFragment')
     azure_completion_fragment.__fields__(__exclude__=['id', 'api_type', 'model_type', 'model_name'])
 
     azure_embedding_fragment = Fragment(AzureOpenaiEmbeddingLLMApiConfig, 'AzureEmbeddingFragment')
```

### Comparing `answerrocket_client-0.2.0/answer_rocket/client.py` & `answerrocket_client-0.2.1/answer_rocket/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.0/answer_rocket/config.py` & `answerrocket_client-0.2.1/answer_rocket/config.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.0/answer_rocket/data.py` & `answerrocket_client-0.2.1/answer_rocket/data.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.0/answer_rocket/graphql/client.py` & `answerrocket_client-0.2.1/answer_rocket/graphql/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.0/answer_rocket/graphql/schema.py` & `answerrocket_client-0.2.1/answer_rocket/graphql/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,57 +143,14 @@
     hide_from_user = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='hideFromUser')
     misc_info = sgqlc.types.Field(String, graphql_name='miscInfo')
     db_table = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='dbTable')
     derived_table_sql = sgqlc.types.Field(String, graphql_name='derivedTableSql')
     attributes = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MaxDomainAttribute))), graphql_name='attributes')
 
 
-class ChatEntry(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('id', 'thread_id', 'answer')
-    id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='id')
-    thread_id = sgqlc.types.Field(UUID, graphql_name='threadId')
-    answer = sgqlc.types.Field('ChatResult', graphql_name='answer')
-
-
-class ChatResult(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('answer_id', 'answered_at', 'copilot_skill_id', 'has_finished', 'error', 'is_new_thread', 'message', 'report_results', 'thread_id', 'user_id')
-    answer_id = sgqlc.types.Field(UUID, graphql_name='answerId')
-    answered_at = sgqlc.types.Field(DateTime, graphql_name='answeredAt')
-    copilot_skill_id = sgqlc.types.Field(UUID, graphql_name='copilotSkillId')
-    has_finished = sgqlc.types.Field(Boolean, graphql_name='hasFinished')
-    error = sgqlc.types.Field(String, graphql_name='error')
-    is_new_thread = sgqlc.types.Field(Boolean, graphql_name='isNewThread')
-    message = sgqlc.types.Field(String, graphql_name='message')
-    report_results = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('ReportResult')), graphql_name='reportResults')
-    thread_id = sgqlc.types.Field(UUID, graphql_name='threadId')
-    user_id = sgqlc.types.Field(UUID, graphql_name='userId')
-
-
-class ChatThread(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('id', 'entry_count', 'title', 'pinned_dataset')
-    id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='id')
-    entry_count = sgqlc.types.Field(Int, graphql_name='entryCount', args=sgqlc.types.ArgDict((
-        ('most_recent_entry_inclusive', sgqlc.types.Arg(UUID, graphql_name='mostRecentEntryInclusive', default=None)),
-))
-    )
-    title = sgqlc.types.Field(String, graphql_name='title')
-    pinned_dataset = sgqlc.types.Field(UUID, graphql_name='pinnedDataset')
-
-
-class ContentBlock(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('id', 'title', 'payload')
-    id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='id')
-    title = sgqlc.types.Field(String, graphql_name='title')
-    payload = sgqlc.types.Field(String, graphql_name='payload')
-
-
 class CopilotSkillArtifact(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('copilot_skill_artifact_id', 'copilot_id', 'copilot_skill_id', 'artifact_path', 'artifact', 'description', 'created_user_id', 'created_utc', 'last_modified_user_id', 'last_modified_utc', 'version', 'is_active', 'is_deleted')
     copilot_skill_artifact_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotSkillArtifactId')
     copilot_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotId')
     copilot_skill_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId')
     artifact_path = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='artifactPath')
@@ -286,14 +243,55 @@
     __field_names__ = ('success', 'code', 'error', 'data')
     success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
     code = sgqlc.types.Field(String, graphql_name='code')
     error = sgqlc.types.Field(String, graphql_name='error')
     data = sgqlc.types.Field(JSON, graphql_name='data')
 
 
+class MaxChatEntry(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('id', 'thread_id', 'question', 'answer')
+    id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='id')
+    thread_id = sgqlc.types.Field(UUID, graphql_name='threadId')
+    question = sgqlc.types.Field('MaxChatQuestion', graphql_name='question')
+    answer = sgqlc.types.Field('MaxChatResult', graphql_name='answer')
+
+
+class MaxChatQuestion(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('asked_at', 'nl')
+    asked_at = sgqlc.types.Field(DateTime, graphql_name='askedAt')
+    nl = sgqlc.types.Field(String, graphql_name='nl')
+
+
+class MaxChatResult(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('answer_id', 'answered_at', 'copilot_skill_id', 'has_finished', 'error', 'is_new_thread', 'message', 'report_results', 'thread_id', 'user_id')
+    answer_id = sgqlc.types.Field(UUID, graphql_name='answerId')
+    answered_at = sgqlc.types.Field(DateTime, graphql_name='answeredAt')
+    copilot_skill_id = sgqlc.types.Field(UUID, graphql_name='copilotSkillId')
+    has_finished = sgqlc.types.Field(Boolean, graphql_name='hasFinished')
+    error = sgqlc.types.Field(String, graphql_name='error')
+    is_new_thread = sgqlc.types.Field(Boolean, graphql_name='isNewThread')
+    message = sgqlc.types.Field(String, graphql_name='message')
+    report_results = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null('MaxReportResult')), graphql_name='reportResults')
+    thread_id = sgqlc.types.Field(UUID, graphql_name='threadId')
+    user_id = sgqlc.types.Field(UUID, graphql_name='userId')
+
+
+class MaxChatThread(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('id', 'entry_count', 'title', 'copilot_id', 'entries')
+    id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='id')
+    entry_count = sgqlc.types.Field(Int, graphql_name='entryCount')
+    title = sgqlc.types.Field(String, graphql_name='title')
+    copilot_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotId')
+    entries = sgqlc.types.Field(sgqlc.types.list_of(MaxChatEntry), graphql_name='entries')
+
+
 class MaxColumn(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('name', 'jdbc_type', 'length', 'precision', 'scale')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     jdbc_type = sgqlc.types.Field(String, graphql_name='jdbcType')
     length = sgqlc.types.Field(Int, graphql_name='length')
     precision = sgqlc.types.Field(Int, graphql_name='precision')
@@ -423,24 +421,42 @@
     __schema__ = schema
     __field_names__ = ('success', 'code', 'error')
     success = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='success')
     code = sgqlc.types.Field(String, graphql_name='code')
     error = sgqlc.types.Field(String, graphql_name='error')
 
 
+class MaxReportParamsAndValues(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('key', 'values', 'label', 'color')
+    key = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='key')
+    values = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='values')
+    label = sgqlc.types.Field(String, graphql_name='label')
+    color = sgqlc.types.Field(String, graphql_name='color')
+
+
+class MaxReportResult(sgqlc.types.Type):
+    __schema__ = schema
+    __field_names__ = ('title', 'report_name', 'parameters', 'custom_payload')
+    title = sgqlc.types.Field(String, graphql_name='title')
+    report_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='reportName')
+    parameters = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(MaxReportParamsAndValues)), graphql_name='parameters')
+    custom_payload = sgqlc.types.Field(JSON, graphql_name='customPayload')
+
+
 class MaxTable(sgqlc.types.Type):
     __schema__ = schema
     __field_names__ = ('name', 'columns')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
     columns = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(MaxColumn))), graphql_name='columns')
 
 
 class Mutation(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('create_max_copilot_skill_chat_question', 'update_max_copilot_skill_chat_question', 'delete_max_copilot_skill_chat_question', 'create_max_copilot_question', 'update_max_copilot_question', 'delete_max_copilot_question', 'update_chat_answer_payload', 'ask_chat_question', 'evaluate_chat_question')
+    __field_names__ = ('create_max_copilot_skill_chat_question', 'update_max_copilot_skill_chat_question', 'delete_max_copilot_skill_chat_question', 'create_max_copilot_question', 'update_max_copilot_question', 'delete_max_copilot_question', 'update_chat_answer_payload', 'ask_chat_question', 'evaluate_chat_question', 'queue_chat_question', 'cancel_chat_question', 'create_chat_thread')
     create_max_copilot_skill_chat_question = sgqlc.types.Field(sgqlc.types.non_null(CreateMaxCopilotSkillChatQuestionResponse), graphql_name='createMaxCopilotSkillChatQuestion', args=sgqlc.types.ArgDict((
         ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
         ('copilot_skill_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId', default=None)),
         ('question', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='question', default=None)),
         ('expected_completion_response', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='expectedCompletionResponse', default=None)),
 ))
     )
@@ -475,32 +491,46 @@
 ))
     )
     update_chat_answer_payload = sgqlc.types.Field(JSON, graphql_name='updateChatAnswerPayload', args=sgqlc.types.ArgDict((
         ('answer_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='answerId', default=None)),
         ('payload', sgqlc.types.Arg(sgqlc.types.non_null(JSON), graphql_name='payload', default=None)),
 ))
     )
-    ask_chat_question = sgqlc.types.Field(ChatEntry, graphql_name='askChatQuestion', args=sgqlc.types.ArgDict((
+    ask_chat_question = sgqlc.types.Field(MaxChatEntry, graphql_name='askChatQuestion', args=sgqlc.types.ArgDict((
         ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
         ('question', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='question', default=None)),
         ('thread_id', sgqlc.types.Arg(UUID, graphql_name='threadId', default=None)),
         ('skip_report_cache', sgqlc.types.Arg(Boolean, graphql_name='skipReportCache', default=None)),
         ('dry_run_type', sgqlc.types.Arg(ChatDryRunType, graphql_name='dryRunType', default=None)),
 ))
     )
     evaluate_chat_question = sgqlc.types.Field(sgqlc.types.non_null(EvaluateChatQuestionResponse), graphql_name='evaluateChatQuestion', args=sgqlc.types.ArgDict((
         ('entry_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='entryId', default=None)),
         ('evals', sgqlc.types.Arg(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='evals', default=None)),
 ))
     )
+    queue_chat_question = sgqlc.types.Field(MaxChatEntry, graphql_name='queueChatQuestion', args=sgqlc.types.ArgDict((
+        ('thread_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='threadId', default=None)),
+        ('question', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='question', default=None)),
+        ('skip_cache', sgqlc.types.Arg(Boolean, graphql_name='skipCache', default=None)),
+))
+    )
+    cancel_chat_question = sgqlc.types.Field(MaxChatEntry, graphql_name='cancelChatQuestion', args=sgqlc.types.ArgDict((
+        ('entry_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='entryId', default=None)),
+))
+    )
+    create_chat_thread = sgqlc.types.Field(MaxChatThread, graphql_name='createChatThread', args=sgqlc.types.ArgDict((
+        ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
+))
+    )
 
 
 class Query(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('ping', 'get_copilot_skill_artifact_by_path', 'get_copilot_info', 'get_copilot_skill', 'run_copilot_skill', 'execute_sql_query', 'execute_rql_query', 'get_dataset_id', 'get_dataset', 'get_domain_object', 'get_domain_object_by_name', 'llmapi_config_for_sdk', 'user_chat_threads', 'user_chat_entries')
+    __field_names__ = ('ping', 'get_copilot_skill_artifact_by_path', 'get_copilot_info', 'get_copilot_skill', 'run_copilot_skill', 'execute_sql_query', 'execute_rql_query', 'get_dataset_id', 'get_dataset', 'get_domain_object', 'get_domain_object_by_name', 'llmapi_config_for_sdk', 'user_chat_threads', 'user_chat_entries', 'chat_thread', 'chat_entry')
     ping = sgqlc.types.Field(String, graphql_name='ping')
     get_copilot_skill_artifact_by_path = sgqlc.types.Field(CopilotSkillArtifact, graphql_name='getCopilotSkillArtifactByPath', args=sgqlc.types.ArgDict((
         ('copilot_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotId', default=None)),
         ('copilot_skill_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId', default=None)),
         ('artifact_path', sgqlc.types.Arg(sgqlc.types.non_null(String), graphql_name='artifactPath', default=None)),
 ))
     )
@@ -566,35 +596,22 @@
     )
     user_chat_entries = sgqlc.types.Field(sgqlc.types.list_of(JSON), graphql_name='userChatEntries', args=sgqlc.types.ArgDict((
         ('thread_id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='threadId', default=None)),
         ('offset', sgqlc.types.Arg(Int, graphql_name='offset', default=None)),
         ('limit', sgqlc.types.Arg(Int, graphql_name='limit', default=None)),
 ))
     )
-
-
-class ReportParamsAndValues(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('key', 'values', 'label', 'type', 'color')
-    key = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='key')
-    values = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(String))), graphql_name='values')
-    label = sgqlc.types.Field(String, graphql_name='label')
-    type = sgqlc.types.Field(String, graphql_name='type')
-    color = sgqlc.types.Field(String, graphql_name='color')
-
-
-class ReportResult(sgqlc.types.Type):
-    __schema__ = schema
-    __field_names__ = ('id', 'title', 'report_name', 'run_id', 'parameters', 'content_blocks')
-    id = sgqlc.types.Field(UUID, graphql_name='id')
-    title = sgqlc.types.Field(String, graphql_name='title')
-    report_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='reportName')
-    run_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='runId')
-    parameters = sgqlc.types.Field(sgqlc.types.list_of(sgqlc.types.non_null(ReportParamsAndValues)), graphql_name='parameters')
-    content_blocks = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of(sgqlc.types.non_null(ContentBlock))), graphql_name='contentBlocks')
+    chat_thread = sgqlc.types.Field(MaxChatThread, graphql_name='chatThread', args=sgqlc.types.ArgDict((
+        ('id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='id', default=None)),
+))
+    )
+    chat_entry = sgqlc.types.Field(MaxChatEntry, graphql_name='chatEntry', args=sgqlc.types.ArgDict((
+        ('id', sgqlc.types.Arg(sgqlc.types.non_null(UUID), graphql_name='id', default=None)),
+))
+    )
 
 
 class AzureOpenaiCompletionLLMApiConfig(sgqlc.types.Type, LLMApiConfig):
     __schema__ = schema
     __field_names__ = ('api_base_url', 'api_version', 'openai_model_name', 'max_tokens_content_generation', 'temperature', 'top_p', 'presence_penalty', 'frequency_penalty')
     api_base_url = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='apiBaseUrl')
     api_version = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='apiVersion')
```

### Comparing `answerrocket_client-0.2.0/answer_rocket/output.py` & `answerrocket_client-0.2.1/answer_rocket/output.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.0/answer_rocket/skill.py` & `answerrocket_client-0.2.1/answer_rocket/skill.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.0/answerrocket_client.egg-info/PKG-INFO` & `answerrocket_client-0.2.1/answerrocket_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.0/answerrocket_client.egg-info/SOURCES.txt` & `answerrocket_client-0.2.1/answerrocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.0/readme.md` & `answerrocket_client-0.2.1/readme.md`

 * *Files identical despite different names*


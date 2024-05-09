# Comparing `tmp/ai21-2.2.3.tar.gz` & `tmp/ai21-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-2.2.3.tar", max compression
+gzip compressed data, was "ai21-2.2.4.tar", max compression
```

## Comparing `ai21-2.2.3.tar` & `ai21-2.2.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0    11357 2024-04-25 14:02:55.464870 ai21-2.2.3/LICENSE
--rw-r--r--   0        0        0    11868 2024-04-25 14:02:55.464870 ai21-2.2.3/README.md
--rw-r--r--   0        0        0     1575 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/ai21_env_config.py
--rw-r--r--   0        0        0     2626 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/ai21_http_client.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/bedrock/__init__.py
--rw-r--r--   0        0        0      844 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/bedrock/ai21_bedrock_client.py
--rw-r--r--   0        0        0       92 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/bedrock/bedrock_model_id.py
--rw-r--r--   0        0        0     2414 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/bedrock/bedrock_session.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/bedrock/resources/__init__.py
--rw-r--r--   0        0        0     1996 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/bedrock/resources/bedrock_completion.py
--rw-r--r--   0        0        0      522 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/bedrock/resources/bedrock_resource.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/__init__.py
--rw-r--r--   0        0        0      829 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/answer_base.py
--rw-r--r--   0        0        0     3670 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/chat_base.py
--rw-r--r--   0        0        0     4172 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/completion_base.py
--rw-r--r--   0        0        0     1594 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/custom_model_base.py
--rw-r--r--   0        0        0     1846 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/dataset_base.py
--rw-r--r--   0        0        0      868 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/embed_base.py
--rw-r--r--   0        0        0      557 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/gec_base.py
--rw-r--r--   0        0        0      751 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/improvements_base.py
--rw-r--r--   0        0        0     1438 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/paraphrase_base.py
--rw-r--r--   0        0        0      786 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/segmentation_base.py
--rw-r--r--   0        0        0     1177 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/summarize_base.py
--rw-r--r--   0        0        0     1103 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/common/summarize_by_segment_base.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/__init__.py
--rw-r--r--   0        0        0     1545 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/ai21_sagemaker_client.py
--rw-r--r--   0        0        0      154 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/constants.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/resources/__init__.py
--rw-r--r--   0        0        0      498 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/resources/sagemaker_answer.py
--rw-r--r--   0        0        0     3194 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/resources/sagemaker_completion.py
--rw-r--r--   0        0        0      399 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/resources/sagemaker_gec.py
--rw-r--r--   0        0        0      789 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
--rw-r--r--   0        0        0      484 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/resources/sagemaker_resource.py
--rw-r--r--   0        0        0      810 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/resources/sagemaker_summarize.py
--rw-r--r--   0        0        0     2522 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/sagemaker/sagemaker_session.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/__init__.py
--rw-r--r--   0        0        0     3496 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/ai21_client.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/__init__.py
--rw-r--r--   0        0        0      101 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/chat/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/chat/chat_completions.py
--rw-r--r--   0        0        0      564 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_answer.py
--rw-r--r--   0        0        0     2039 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_chat.py
--rw-r--r--   0        0        0     1974 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_completion.py
--rw-r--r--   0        0        0     1268 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_custom_model.py
--rw-r--r--   0        0        0     1485 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_dataset.py
--rw-r--r--   0        0        0      574 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_embed.py
--rw-r--r--   0        0        0      462 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_gec.py
--rw-r--r--   0        0        0      729 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_improvements.py
--rw-r--r--   0        0        0     3594 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_library.py
--rw-r--r--   0        0        0      851 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_paraphrase.py
--rw-r--r--   0        0        0     1096 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_resource.py
--rw-r--r--   0        0        0      602 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_segmentation.py
--rw-r--r--   0        0        0      869 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_summarize.py
--rw-r--r--   0        0        0      760 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/clients/studio/resources/studio_summarize_by_segment.py
--rw-r--r--   0        0        0       64 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/constants.py
--rw-r--r--   0        0        0     2615 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/errors.py
--rw-r--r--   0        0        0     4868 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/http_client.py
--rw-r--r--   0        0        0      484 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/logger.py
--rw-r--r--   0        0        0     2633 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/__init__.py
--rw-r--r--   0        0        0      262 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/ai21_base_model_mixin.py
--rw-r--r--   0        0        0      343 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/chat/__init__.py
--rw-r--r--   0        0        0      592 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/chat/chat_completion_response.py
--rw-r--r--   0        0        0      219 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/chat/chat_message.py
--rw-r--r--   0        0        0       97 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/chat/role_type.py
--rw-r--r--   0        0        0      233 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/chat_message.py
--rw-r--r--   0        0        0       89 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/document_type.py
--rw-r--r--   0        0        0       96 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/embed_type.py
--rw-r--r--   0        0        0      286 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/improvement_type.py
--rw-r--r--   0        0        0      410 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/logprobs.py
--rw-r--r--   0        0        0      168 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/paraphrase_style_type.py
--rw-r--r--   0        0        0      503 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/penalty.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.464870 ai21-2.2.3/ai21/models/responses/__init__.py
--rw-r--r--   0        0        0      273 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/answer_response.py
--rw-r--r--   0        0        0      518 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/chat_response.py
--rw-r--r--   0        0        0      786 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/completion_response.py
--rw-r--r--   0        0        0      713 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/custom_model_response.py
--rw-r--r--   0        0        0      376 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/dataset_response.py
--rw-r--r--   0        0        0      300 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/embed_response.py
--rw-r--r--   0        0        0      550 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/file_response.py
--rw-r--r--   0        0        0      635 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/gec_response.py
--rw-r--r--   0        0        0      401 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/improvement_response.py
--rw-r--r--   0        0        0      469 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/library_answer_response.py
--rw-r--r--   0        0        0      450 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/library_search_response.py
--rw-r--r--   0        0        0      294 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/paraphrase_response.py
--rw-r--r--   0        0        0      317 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/segmentation_response.py
--rw-r--r--   0        0        0      564 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/summarize_by_segment_response.py
--rw-r--r--   0        0        0      187 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/responses/summarize_response.py
--rw-r--r--   0        0        0      139 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/summary_method.py
--rw-r--r--   0        0        0      222 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/models/usage_info.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/py.typed
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/services/__init__.py
--rw-r--r--   0        0        0     2296 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/services/sagemaker.py
--rw-r--r--   0        0        0      123 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/tokenizers/__init__.py
--rw-r--r--   0        0        0      608 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/tokenizers/ai21_tokenizer.py
--rw-r--r--   0        0        0      628 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/tokenizers/factory.py
--rw-r--r--   0        0        0      722 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/types.py
--rw-r--r--   0        0        0        0 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/utils/__init__.py
--rw-r--r--   0        0        0      668 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/utils/typing.py
--rw-r--r--   0        0        0       18 2024-04-25 14:02:55.468870 ai21-2.2.3/ai21/version.py
--rw-r--r--   0        0        0     2261 2024-04-25 14:02:55.468870 ai21-2.2.3/pyproject.toml
--rw-r--r--   0        0        0    12581 1970-01-01 00:00:00.000000 ai21-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-09 10:37:12.541003 ai21-2.2.4/LICENSE
+-rw-r--r--   0        0        0    11868 2024-05-09 10:37:12.541003 ai21-2.2.4/README.md
+-rw-r--r--   0        0        0     1575 2024-05-09 10:37:12.541003 ai21-2.2.4/ai21/__init__.py
+-rw-r--r--   0        0        0     1014 2024-05-09 10:37:12.541003 ai21-2.2.4/ai21/ai21_env_config.py
+-rw-r--r--   0        0        0     2626 2024-05-09 10:37:12.541003 ai21-2.2.4/ai21/ai21_http_client.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/__init__.py
+-rw-r--r--   0        0        0      844 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/ai21_bedrock_client.py
+-rw-r--r--   0        0        0       92 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/bedrock_model_id.py
+-rw-r--r--   0        0        0     2414 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/bedrock_session.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/resources/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/resources/bedrock_completion.py
+-rw-r--r--   0        0        0      522 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/bedrock/resources/bedrock_resource.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/answer_base.py
+-rw-r--r--   0        0        0     3710 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/chat_base.py
+-rw-r--r--   0        0        0     4216 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/completion_base.py
+-rw-r--r--   0        0        0     1634 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/custom_model_base.py
+-rw-r--r--   0        0        0     1886 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/dataset_base.py
+-rw-r--r--   0        0        0      888 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/embed_base.py
+-rw-r--r--   0        0        0      577 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/gec_base.py
+-rw-r--r--   0        0        0      771 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/improvements_base.py
+-rw-r--r--   0        0        0     1478 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/paraphrase_base.py
+-rw-r--r--   0        0        0      806 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/segmentation_base.py
+-rw-r--r--   0        0        0     1217 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/summarize_base.py
+-rw-r--r--   0        0        0     1143 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/common/summarize_by_segment_base.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/__init__.py
+-rw-r--r--   0        0        0     1545 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/ai21_sagemaker_client.py
+-rw-r--r--   0        0        0      154 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/constants.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_answer.py
+-rw-r--r--   0        0        0     3194 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_completion.py
+-rw-r--r--   0        0        0      399 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_gec.py
+-rw-r--r--   0        0        0      789 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
+-rw-r--r--   0        0        0      484 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_resource.py
+-rw-r--r--   0        0        0      810 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_summarize.py
+-rw-r--r--   0        0        0     2522 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/sagemaker/sagemaker_session.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/__init__.py
+-rw-r--r--   0        0        0     3496 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/ai21_client.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2435 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/chat/chat_completions.py
+-rw-r--r--   0        0        0      574 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_answer.py
+-rw-r--r--   0        0        0     2061 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_chat.py
+-rw-r--r--   0        0        0     1996 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_completion.py
+-rw-r--r--   0        0        0     1290 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_custom_model.py
+-rw-r--r--   0        0        0     1507 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_dataset.py
+-rw-r--r--   0        0        0      584 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_embed.py
+-rw-r--r--   0        0        0      472 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_gec.py
+-rw-r--r--   0        0        0      739 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_improvements.py
+-rw-r--r--   0        0        0     3670 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_library.py
+-rw-r--r--   0        0        0      873 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_paraphrase.py
+-rw-r--r--   0        0        0     1096 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_resource.py
+-rw-r--r--   0        0        0      612 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_segmentation.py
+-rw-r--r--   0        0        0      891 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_summarize.py
+-rw-r--r--   0        0        0      782 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/clients/studio/resources/studio_summarize_by_segment.py
+-rw-r--r--   0        0        0       64 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/constants.py
+-rw-r--r--   0        0        0     2615 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/errors.py
+-rw-r--r--   0        0        0     4868 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/http_client.py
+-rw-r--r--   0        0        0      484 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/logger.py
+-rw-r--r--   0        0        0     2633 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/ai21_base_model_mixin.py
+-rw-r--r--   0        0        0      343 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat/__init__.py
+-rw-r--r--   0        0        0      592 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat/chat_completion_response.py
+-rw-r--r--   0        0        0      219 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat/chat_message.py
+-rw-r--r--   0        0        0       97 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat/role_type.py
+-rw-r--r--   0        0        0      233 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/chat_message.py
+-rw-r--r--   0        0        0       89 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/document_type.py
+-rw-r--r--   0        0        0       96 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/embed_type.py
+-rw-r--r--   0        0        0      286 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/improvement_type.py
+-rw-r--r--   0        0        0      410 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/logprobs.py
+-rw-r--r--   0        0        0      168 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/paraphrase_style_type.py
+-rw-r--r--   0        0        0      503 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/penalty.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/answer_response.py
+-rw-r--r--   0        0        0      518 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/chat_response.py
+-rw-r--r--   0        0        0      786 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/completion_response.py
+-rw-r--r--   0        0        0      713 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/custom_model_response.py
+-rw-r--r--   0        0        0      376 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/dataset_response.py
+-rw-r--r--   0        0        0      300 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/embed_response.py
+-rw-r--r--   0        0        0      550 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/file_response.py
+-rw-r--r--   0        0        0      635 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/gec_response.py
+-rw-r--r--   0        0        0      401 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/improvement_response.py
+-rw-r--r--   0        0        0      469 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/library_answer_response.py
+-rw-r--r--   0        0        0      450 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/library_search_response.py
+-rw-r--r--   0        0        0      294 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/paraphrase_response.py
+-rw-r--r--   0        0        0      317 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/segmentation_response.py
+-rw-r--r--   0        0        0      564 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/summarize_by_segment_response.py
+-rw-r--r--   0        0        0      187 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/responses/summarize_response.py
+-rw-r--r--   0        0        0      139 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/summary_method.py
+-rw-r--r--   0        0        0      222 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/models/usage_info.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/py.typed
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/services/__init__.py
+-rw-r--r--   0        0        0     2296 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/services/sagemaker.py
+-rw-r--r--   0        0        0      123 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/tokenizers/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/tokenizers/ai21_tokenizer.py
+-rw-r--r--   0        0        0      628 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/tokenizers/factory.py
+-rw-r--r--   0        0        0      722 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/types.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/utils/__init__.py
+-rw-r--r--   0        0        0      668 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/utils/typing.py
+-rw-r--r--   0        0        0       18 2024-05-09 10:37:12.545003 ai21-2.2.4/ai21/version.py
+-rw-r--r--   0        0        0     2261 2024-05-09 10:37:12.549003 ai21-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0    12581 1970-01-01 00:00:00.000000 ai21-2.2.4/PKG-INFO
```

### Comparing `ai21-2.2.3/LICENSE` & `ai21-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/README.md` & `ai21-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/__init__.py` & `ai21-2.2.4/ai21/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/ai21_env_config.py` & `ai21-2.2.4/ai21/ai21_env_config.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/ai21_http_client.py` & `ai21-2.2.4/ai21/ai21_http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/bedrock/ai21_bedrock_client.py` & `ai21-2.2.4/ai21/clients/bedrock/ai21_bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/bedrock/bedrock_session.py` & `ai21-2.2.4/ai21/clients/bedrock/bedrock_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/bedrock/resources/bedrock_completion.py` & `ai21-2.2.4/ai21/clients/bedrock/resources/bedrock_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/bedrock/resources/bedrock_resource.py` & `ai21-2.2.4/ai21/clients/bedrock/resources/bedrock_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/common/answer_base.py` & `ai21-2.2.4/ai21/clients/common/answer_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,9 +25,10 @@
     def _json_to_response(self, json: Dict[str, Any]) -> AnswerResponse:
         return AnswerResponse.from_dict(json)
 
     def _create_body(
         self,
         context: str,
         question: str,
+        **kwargs,
     ) -> Dict[str, Any]:
-        return {"context": context, "question": question}
+        return {"context": context, "question": question, **kwargs}
```

### Comparing `ai21-2.2.3/ai21/clients/common/chat_base.py` & `ai21-2.2.4/ai21/clients/common/chat_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
         min_tokens: Optional[int] = 0,
         top_p: Optional[float] = 1.0,
         top_k_return: Optional[int] = 0,
         stop_sequences: Optional[List[str]] = None,
         frequency_penalty: Optional[Penalty] = None,
         presence_penalty: Optional[Penalty] = None,
         count_penalty: Optional[Penalty] = None,
+        **kwargs,
     ) -> Dict[str, Any]:
         return {
             "model": model,
             "system": system,
             "messages": [message.to_dict() for message in messages],
             "temperature": temperature,
             "maxTokens": max_tokens,
@@ -82,8 +83,9 @@
             "numResults": num_results,
             "topP": top_p,
             "topKReturn": top_k_return,
             "stopSequences": stop_sequences,
             "frequencyPenalty": None if frequency_penalty is None else frequency_penalty.to_dict(),
             "presencePenalty": None if presence_penalty is None else presence_penalty.to_dict(),
             "countPenalty": None if count_penalty is None else count_penalty.to_dict(),
+            **kwargs,
         }
```

### Comparing `ai21-2.2.3/ai21/clients/common/completion_base.py` & `ai21-2.2.4/ai21/clients/common/completion_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         custom_model: str | NotGiven,
         stop_sequences: List[str] | NotGiven,
         frequency_penalty: Penalty | NotGiven,
         presence_penalty: Penalty | NotGiven,
         count_penalty: Penalty | NotGiven,
         epoch: int | NotGiven,
         logit_bias: Dict[str, float] | NotGiven,
+        **kwargs,
     ):
         return remove_not_given(
             {
                 "model": model,
                 "customModel": custom_model,
                 "prompt": prompt,
                 "maxTokens": max_tokens,
@@ -89,9 +90,10 @@
                 "topKReturn": top_k_return,
                 "stopSequences": stop_sequences,
                 "frequencyPenalty": NOT_GIVEN if frequency_penalty is NOT_GIVEN else frequency_penalty.to_dict(),
                 "presencePenalty": NOT_GIVEN if presence_penalty is NOT_GIVEN else presence_penalty.to_dict(),
                 "countPenalty": NOT_GIVEN if count_penalty is NOT_GIVEN else count_penalty.to_dict(),
                 "epoch": epoch,
                 "logitBias": logit_bias,
+                **kwargs,
             }
         )
```

### Comparing `ai21-2.2.3/ai21/clients/common/custom_model_base.py` & `ai21-2.2.4/ai21/clients/common/custom_model_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     def _create_body(
         self,
         dataset_id: str,
         model_name: str,
         model_type: str,
         learning_rate: Optional[float],
         num_epochs: Optional[int],
+        **kwargs,
     ) -> Dict[str, Any]:
         return {
             "dataset_id": dataset_id,
             "model_name": model_name,
             "model_type": model_type,
             "learning_rate": learning_rate,
             "num_epochs": num_epochs,
+            **kwargs,
         }
```

### Comparing `ai21-2.2.3/ai21/clients/common/dataset_base.py` & `ai21-2.2.4/ai21/clients/common/dataset_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,17 @@
     def _create_body(
         self,
         dataset_name: str,
         selected_columns: Optional[str],
         approve_whitespace_correction: Optional[bool],
         delete_long_rows: Optional[bool],
         split_ratio: Optional[float],
+        **kwargs,
     ) -> Dict[str, Any]:
         return {
             "dataset_name": dataset_name,
             "selected_columns": selected_columns,
             "approve_whitespace_correction": approve_whitespace_correction,
             "delete_long_rows": delete_long_rows,
             "split_ratio": split_ratio,
+            **kwargs,
         }
```

### Comparing `ai21-2.2.3/ai21/clients/common/embed_base.py` & `ai21-2.2.4/ai21/clients/common/embed_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,9 +18,9 @@
         :return:
         """
         pass
 
     def _json_to_response(self, json: Dict[str, Any]) -> EmbedResponse:
         return EmbedResponse.from_dict(json)
 
-    def _create_body(self, texts: List[str], type: Optional[str]) -> Dict[str, Any]:
-        return {"texts": texts, "type": type}
+    def _create_body(self, texts: List[str], type: Optional[str], **kwargs) -> Dict[str, Any]:
+        return {"texts": texts, "type": type, **kwargs}
```

### Comparing `ai21-2.2.3/ai21/clients/common/gec_base.py` & `ai21-2.2.4/ai21/clients/common/gec_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,9 +16,9 @@
         :return:
         """
         pass
 
     def _json_to_response(self, json: Dict[str, Any]) -> GECResponse:
         return GECResponse.from_dict(json)
 
-    def _create_body(self, text: str) -> Dict[str, Any]:
-        return {"text": text}
+    def _create_body(self, text: str, **kwargs) -> Dict[str, Any]:
+        return {"text": text, **kwargs}
```

### Comparing `ai21-2.2.3/ai21/clients/common/improvements_base.py` & `ai21-2.2.4/ai21/clients/common/improvements_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,9 +17,9 @@
         :return:
         """
         pass
 
     def _json_to_response(self, json: Dict[str, Any]) -> ImprovementsResponse:
         return ImprovementsResponse.from_dict(json)
 
-    def _create_body(self, text: str, types: List[str]) -> Dict[str, Any]:
-        return {"text": text, "types": types}
+    def _create_body(self, text: str, types: List[str], **kwargs) -> Dict[str, Any]:
+        return {"text": text, "types": types, **kwargs}
```

### Comparing `ai21-2.2.3/ai21/clients/common/paraphrase_base.py` & `ai21-2.2.4/ai21/clients/common/paraphrase_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
     def _create_body(
         self,
         text: str,
         style: Optional[str],
         start_index: Optional[int],
         end_index: Optional[int],
+        **kwargs,
     ) -> Dict[str, Any]:
         return {
             "text": text,
             "style": style,
             "startIndex": start_index,
             "endIndex": end_index,
+            **kwargs,
         }
```

### Comparing `ai21-2.2.3/ai21/clients/common/segmentation_base.py` & `ai21-2.2.4/ai21/clients/common/segmentation_base.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,9 +17,9 @@
         :return:
         """
         pass
 
     def _json_to_response(self, json: Dict[str, Any]) -> SegmentationResponse:
         return SegmentationResponse.from_dict(json)
 
-    def _create_body(self, source: str, source_type: str) -> Dict[str, Any]:
-        return {"source": source, "sourceType": source_type}
+    def _create_body(self, source: str, source_type: str, **kwargs) -> Dict[str, Any]:
+        return {"source": source, "sourceType": source_type, **kwargs}
```

### Comparing `ai21-2.2.3/ai21/clients/common/summarize_base.py` & `ai21-2.2.4/ai21/clients/common/summarize_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 
     def _create_body(
         self,
         source: str,
         source_type: str,
         focus: Optional[str],
         summary_method: Optional[str],
+        **kwargs,
     ) -> Dict[str, Any]:
         return {
             "source": source,
             "sourceType": source_type,
             "focus": focus,
             "summaryMethod": summary_method,
+            **kwargs,
         }
```

### Comparing `ai21-2.2.3/ai21/clients/common/summarize_by_segment_base.py` & `ai21-2.2.4/ai21/clients/common/summarize_by_segment_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,13 +30,15 @@
         return SummarizeBySegmentResponse.from_dict(json)
 
     def _create_body(
         self,
         source: str,
         source_type: str,
         focus: Optional[str],
+        **kwargs,
     ) -> Dict[str, Any]:
         return {
             "source": source,
             "sourceType": source_type,
             "focus": focus,
+            **kwargs,
         }
```

### Comparing `ai21-2.2.3/ai21/clients/sagemaker/ai21_sagemaker_client.py` & `ai21-2.2.4/ai21/clients/sagemaker/ai21_sagemaker_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/sagemaker/resources/sagemaker_completion.py` & `ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py` & `ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/sagemaker/resources/sagemaker_summarize.py` & `ai21-2.2.4/ai21/clients/sagemaker/resources/sagemaker_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/sagemaker/sagemaker_session.py` & `ai21-2.2.4/ai21/clients/sagemaker/sagemaker_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/studio/ai21_client.py` & `ai21-2.2.4/ai21/clients/studio/ai21_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/chat/chat_completions.py` & `ai21-2.2.4/ai21/clients/studio/resources/chat/chat_completions.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_answer.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_answer.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,12 +8,12 @@
         self,
         context: str,
         question: str,
         **kwargs,
     ) -> AnswerResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}"
 
-        body = self._create_body(context=context, question=question)
+        body = self._create_body(context=context, question=question, **kwargs)
 
         response = self._post(url=url, body=body)
 
         return self._json_to_response(response)
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_chat.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             min_tokens=min_tokens,
             top_p=top_p,
             top_k_return=top_k_return,
             stop_sequences=stop_sequences,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             count_penalty=count_penalty,
+            **kwargs,
         )
         url = f"{self._client.get_base_url()}/{model}/{self._module_name}"
         response = self._post(url=url, body=body)
         return self._json_to_response(response)
 
     @property
     def completions(self) -> ChatCompletions:
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_completion.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_completion.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,9 +47,10 @@
             custom_model=custom_model,
             stop_sequences=stop_sequences,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             count_penalty=count_penalty,
             epoch=epoch,
             logit_bias=logit_bias,
+            **kwargs,
         )
         return self._json_to_response(self._post(url=url, body=body))
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_custom_model.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_custom_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         url = f"{self._client.get_base_url()}/{self._module_name}"
         body = self._create_body(
             dataset_id=dataset_id,
             model_name=model_name,
             model_type=model_type,
             learning_rate=learning_rate,
             num_epochs=num_epochs,
+            **kwargs,
         )
         self._post(url=url, body=body)
 
     def list(self) -> List[CustomBaseModelResponse]:
         url = f"{self._client.get_base_url()}/{self._module_name}"
         response = self._get(url=url)
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_dataset.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         files = {"dataset_file": open(file_path, "rb")}
         body = self._create_body(
             dataset_name=dataset_name,
             selected_columns=selected_columns,
             approve_whitespace_correction=approve_whitespace_correction,
             delete_long_rows=delete_long_rows,
             split_ratio=split_ratio,
+            **kwargs,
         )
         return self._post(
             url=self._base_url(),
             body=body,
             files=files,
         )
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_embed.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_embed.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 from ai21.clients.studio.resources.studio_resource import StudioResource
 from ai21.models import EmbedType, EmbedResponse
 
 
 class StudioEmbed(StudioResource, Embed):
     def create(self, texts: List[str], type: Optional[EmbedType] = None, **kwargs) -> EmbedResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}"
-        body = self._create_body(texts=texts, type=type)
+        body = self._create_body(texts=texts, type=type, **kwargs)
         response = self._post(url=url, body=body)
 
         return self._json_to_response(response)
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_improvements.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_improvements.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 class StudioImprovements(StudioResource, Improvements):
     def create(self, text: str, types: List[ImprovementType], **kwargs) -> ImprovementsResponse:
         if len(types) == 0:
             raise EmptyMandatoryListError("types")
 
         url = f"{self._client.get_base_url()}/{self._module_name}"
-        body = self._create_body(text=text, types=types)
+        body = self._create_body(text=text, types=types, **kwargs)
         response = self._post(url=url, body=body)
 
         return self._json_to_response(response)
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_library.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         path: Optional[str] = None,
         labels: Optional[List[str]] = None,
         public_url: Optional[str] = None,
         **kwargs,
     ) -> str:
         url = f"{self._client.get_base_url()}/{self._module_name}"
         files = {"file": open(file_path, "rb")}
-        body = {"path": path, "labels": labels, "publicUrl": public_url}
+        body = {"path": path, "labels": labels, "publicUrl": public_url, **kwargs}
 
         raw_response = self._post(url=url, files=files, body=body)
 
         return raw_response["fileId"]
 
     def get(self, file_id: str) -> FileResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}/{file_id}"
@@ -62,14 +62,15 @@
         labels: Optional[List[str]] = None,
         **kwargs,
     ) -> None:
         url = f"{self._client.get_base_url()}/{self._module_name}/{file_id}"
         body = {
             "publicUrl": public_url,
             "labels": labels,
+            **kwargs,
         }
         self._put(url=url, body=body)
 
     def delete(self, file_id: str) -> None:
         url = f"{self._client.get_base_url()}/{self._module_name}/{file_id}"
         self._delete(url=url)
 
@@ -88,14 +89,15 @@
     ) -> LibrarySearchResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}"
         body = {
             "query": query,
             "path": path,
             "fieldIds": field_ids,
             "maxSegments": max_segments,
+            **kwargs,
         }
         raw_response = self._post(url=url, body=body)
         return LibrarySearchResponse.from_dict(raw_response)
 
 
 class LibraryAnswer(StudioResource):
     _module_name = "library/answer"
@@ -111,10 +113,11 @@
     ) -> LibraryAnswerResponse:
         url = f"{self._client.get_base_url()}/{self._module_name}"
         body = {
             "question": question,
             "path": path,
             "fieldIds": field_ids,
             "labels": labels,
+            **kwargs,
         }
         raw_response = self._post(url=url, body=body)
         return LibraryAnswerResponse.from_dict(raw_response)
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_paraphrase.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_paraphrase.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,12 +16,13 @@
         **kwargs,
     ) -> ParaphraseResponse:
         body = self._create_body(
             text=text,
             style=style,
             start_index=start_index,
             end_index=end_index,
+            **kwargs,
         )
         url = f"{self._client.get_base_url()}/{self._module_name}"
         response = self._post(url=url, body=body)
 
         return self._json_to_response(response)
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_resource.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_segmentation.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_segmentation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ai21.clients.common.segmentation_base import Segmentation
 from ai21.clients.studio.resources.studio_resource import StudioResource
 from ai21.models import DocumentType, SegmentationResponse
 
 
 class StudioSegmentation(StudioResource, Segmentation):
     def create(self, source: str, source_type: DocumentType, **kwargs) -> SegmentationResponse:
-        body = self._create_body(source=source, source_type=source_type.value)
+        body = self._create_body(source=source, source_type=source_type.value, **kwargs)
         url = f"{self._client.get_base_url()}/{self._module_name}"
         raw_response = self._post(url=url, body=body)
 
         return self._json_to_response(raw_response)
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_summarize.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_summarize.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,12 +18,13 @@
         **kwargs,
     ) -> SummarizeResponse:
         body = self._create_body(
             source=source,
             source_type=source_type,
             focus=focus,
             summary_method=summary_method,
+            **kwargs,
         )
         url = f"{self._client.get_base_url()}/{self._module_name}"
         response = self._post(url=url, body=body)
 
         return self._json_to_response(response)
```

### Comparing `ai21-2.2.3/ai21/clients/studio/resources/studio_summarize_by_segment.py` & `ai21-2.2.4/ai21/clients/studio/resources/studio_summarize_by_segment.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,11 +9,12 @@
     def create(
         self, source: str, source_type: DocumentType, *, focus: Optional[str] = None, **kwargs
     ) -> SummarizeBySegmentResponse:
         body = self._create_body(
             source=source,
             source_type=source_type,
             focus=focus,
+            **kwargs,
         )
         url = f"{self._client.get_base_url()}/{self._module_name}"
         response = self._post(url=url, body=body)
         return self._json_to_response(response)
```

### Comparing `ai21-2.2.3/ai21/errors.py` & `ai21-2.2.4/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/http_client.py` & `ai21-2.2.4/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/models/__init__.py` & `ai21-2.2.4/ai21/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/models/chat/chat_completion_response.py` & `ai21-2.2.4/ai21/models/chat/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/models/responses/chat_response.py` & `ai21-2.2.4/ai21/models/responses/chat_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/models/responses/completion_response.py` & `ai21-2.2.4/ai21/models/responses/completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/models/responses/custom_model_response.py` & `ai21-2.2.4/ai21/models/responses/custom_model_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/models/responses/file_response.py` & `ai21-2.2.4/ai21/models/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/models/responses/gec_response.py` & `ai21-2.2.4/ai21/models/responses/gec_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/models/responses/summarize_by_segment_response.py` & `ai21-2.2.4/ai21/models/responses/summarize_by_segment_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/services/sagemaker.py` & `ai21-2.2.4/ai21/services/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/tokenizers/ai21_tokenizer.py` & `ai21-2.2.4/ai21/tokenizers/ai21_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/tokenizers/factory.py` & `ai21-2.2.4/ai21/tokenizers/factory.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/types.py` & `ai21-2.2.4/ai21/types.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/ai21/utils/typing.py` & `ai21-2.2.4/ai21/utils/typing.py`

 * *Files identical despite different names*

### Comparing `ai21-2.2.3/pyproject.toml` & `ai21-2.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "if typing.TYPE_CHECKING:"
 ]
 
 [tool.poetry]
 name = "ai21"
-version = "2.2.3"
+version = "2.2.4"
 description = ""
 authors = ["AI21 Labs"]
 readme = "README.md"
 packages = [
     { include = "ai21" }
 ]
```

### Comparing `ai21-2.2.3/PKG-INFO` & `ai21-2.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 2.2.3
+Version: 2.2.4
 Summary: 
 Author: AI21 Labs
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ai21 Version: 2.2.3 Summary: Author: AI21 Labs
+Metadata-Version: 2.1 Name: ai21 Version: 2.2.4 Summary: Author: AI21 Labs
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: aws Requires-Dist: ai21-tokenizer
 (>=0.9.0,<0.10.0) Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0) Requires-Dist: requests
```


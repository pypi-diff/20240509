# Comparing `tmp/haystack_ai-2.1.0rc2.tar.gz` & `tmp/haystack_ai-2.1.1rc1.tar.gz`

## Comparing `haystack_ai-2.1.0rc2.tar` & `haystack_ai-2.1.1rc1.tar`

### file list

```diff
@@ -1,188 +1,188 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/VERSION.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/errors.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/lazy_imports.py
--rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/logging.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/audio/__init__.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/audio/whisper_local.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/audio/whisper_remote.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/builders/__init__.py
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/builders/answer_builder.py
--rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/builders/dynamic_chat_prompt_builder.py
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/builders/dynamic_prompt_builder.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/builders/prompt_builder.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/caching/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/caching/cache_checker.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/classifiers/__init__.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/classifiers/document_language_classifier.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/connectors/__init__.py
--rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/connectors/openapi_service.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/__init__.py
--rw-r--r--   0        0        0    24642 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/azure.py
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/html.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/markdown.py
--rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/openapi_functions.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/output_adapter.py
--rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/pdfminer.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/pypdf.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/tika.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/txt.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/converters/utils.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/__init__.py
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/azure_document_embedder.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/azure_text_embedder.py
--rw-r--r--   0        0        0    10897 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/hugging_face_api_document_embedder.py
--rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/hugging_face_api_text_embedder.py
--rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/hugging_face_tei_document_embedder.py
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/hugging_face_tei_text_embedder.py
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/openai_document_embedder.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/openai_text_embedder.py
--rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/sentence_transformers_document_embedder.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/sentence_transformers_text_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/backends/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/embedders/backends/sentence_transformers_backend.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/evaluators/__init__.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/evaluators/answer_exact_match.py
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/evaluators/context_relevance.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/evaluators/document_map.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/evaluators/document_mrr.py
--rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/evaluators/document_recall.py
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/evaluators/faithfulness.py
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/evaluators/llm_evaluator.py
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/evaluators/sas_evaluator.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/extractors/__init__.py
--rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/extractors/named_entity_extractor.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/fetchers/__init__.py
--rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/fetchers/link_content.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/__init__.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/azure.py
--rw-r--r--   0        0        0     9907 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/hugging_face_api.py
--rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/hugging_face_local.py
--rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/hugging_face_tgi.py
--rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/openai.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/utils.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/chat/__init__.py
--rw-r--r--   0        0        0     9791 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/chat/azure.py
--rw-r--r--   0        0        0    11186 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/chat/hugging_face_api.py
--rw-r--r--   0        0        0    17793 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/chat/hugging_face_local.py
--rw-r--r--   0        0        0    15851 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/chat/hugging_face_tgi.py
--rw-r--r--   0        0        0    16934 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/generators/chat/openai.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/joiners/__init__.py
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/joiners/document_joiner.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/others/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/others/multiplexer.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/preprocessors/__init__.py
--rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/preprocessors/document_cleaner.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/preprocessors/document_splitter.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/preprocessors/text_cleaner.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/rankers/__init__.py
--rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/rankers/lost_in_the_middle.py
--rw-r--r--   0        0        0    17048 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/rankers/meta_field.py
--rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/rankers/sentence_transformers_diversity.py
--rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/rankers/transformers_similarity.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/readers/__init__.py
--rw-r--r--   0        0        0    28699 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/readers/extractive.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/retrievers/__init__.py
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/retrievers/filter_retriever.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/retrievers/in_memory/__init__.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/retrievers/in_memory/bm25_retriever.py
--rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/retrievers/in_memory/embedding_retriever.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/routers/__init__.py
--rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/routers/conditional_router.py
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/routers/file_type_router.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/routers/metadata_router.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/routers/text_language_router.py
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/routers/zero_shot_text_router.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/samplers/__init__.py
--rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/samplers/top_p.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/validators/__init__.py
--rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/validators/json_schema.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/websearch/__init__.py
--rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/websearch/searchapi.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/websearch/serper_dev.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/writers/__init__.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/components/writers/document_writer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/errors.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/serialization.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/type_utils.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/component/__init__.py
--rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/component/component.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/component/sockets.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/component/types.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/pipeline/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/pipeline/descriptions.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/pipeline/draw.py
--rw-r--r--   0        0        0    56764 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/pipeline/pipeline.py
--rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/pipeline/template.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/pipeline/predefined/indexing.yaml.jinja2
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/core/pipeline/predefined/rag.yaml.jinja2
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/dataclasses/__init__.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/dataclasses/answer.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/dataclasses/byte_stream.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/dataclasses/chat_message.py
--rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/dataclasses/document.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/dataclasses/sparse_embedding.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/dataclasses/streaming_chunk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/document_stores/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/document_stores/errors/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/document_stores/errors/errors.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/document_stores/in_memory/__init__.py
--rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/document_stores/in_memory/document_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/document_stores/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/document_stores/types/policy.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/document_stores/types/protocol.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/evaluation/__init__.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/evaluation/eval_run_result.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/marshal/__init__.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/marshal/protocol.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/marshal/yaml.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/telemetry/__init__.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/telemetry/_environment.py
--rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/telemetry/_telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/__init__.py
--rw-r--r--   0        0        0    63152 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/document_store.py
--rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/factory.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/test_utils.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/accumulate.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/add_value.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/concatenate.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/double.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/fstring.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/greet.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/hello.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/joiner.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/parity.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/remainder.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/repeat.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/self_loop.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/subtract.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/sum.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/text_splitter.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/testing/sample_components/threshold.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/tracing/__init__.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/tracing/datadog.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/tracing/opentelemetry.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/tracing/tracer.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/tracing/utils.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/__init__.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/auth.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/callable_serialization.py
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/device.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/expit.py
--rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/filters.py
--rw-r--r--   0        0        0    15510 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/hf.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/jupyter.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/requests_utils.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/type_serialization.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/haystack/utils/url_validation.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/LICENSE
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/README.md
--rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/VERSION.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/errors.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/lazy_imports.py
+-rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/logging.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/audio/__init__.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/audio/whisper_local.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/audio/whisper_remote.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/__init__.py
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/answer_builder.py
+-rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
+-rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/dynamic_prompt_builder.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/builders/prompt_builder.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/caching/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/caching/cache_checker.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/classifiers/__init__.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/classifiers/document_language_classifier.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/connectors/__init__.py
+-rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/connectors/openapi_service.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/__init__.py
+-rw-r--r--   0        0        0    24642 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/azure.py
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/html.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/markdown.py
+-rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/openapi_functions.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/output_adapter.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/pdfminer.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/pypdf.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/tika.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/txt.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/converters/utils.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/__init__.py
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/azure_document_embedder.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/azure_text_embedder.py
+-rw-r--r--   0        0        0    10902 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_api_document_embedder.py
+-rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_api_text_embedder.py
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/openai_document_embedder.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/openai_text_embedder.py
+-rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/backends/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/__init__.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/answer_exact_match.py
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/context_relevance.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/document_map.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/document_mrr.py
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/document_recall.py
+-rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/faithfulness.py
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/evaluators/sas_evaluator.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/extractors/__init__.py
+-rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/extractors/named_entity_extractor.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/fetchers/__init__.py
+-rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/fetchers/link_content.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/__init__.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/azure.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_api.py
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_local.py
+-rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_tgi.py
+-rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/openai.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/utils.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/__init__.py
+-rw-r--r--   0        0        0     9791 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/azure.py
+-rw-r--r--   0        0        0    11191 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_api.py
+-rw-r--r--   0        0        0    17793 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_local.py
+-rw-r--r--   0        0        0    15851 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_tgi.py
+-rw-r--r--   0        0        0    16934 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/generators/chat/openai.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/joiners/__init__.py
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/joiners/document_joiner.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/others/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/others/multiplexer.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/preprocessors/__init__.py
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/preprocessors/document_cleaner.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/preprocessors/document_splitter.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/preprocessors/text_cleaner.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/__init__.py
+-rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/lost_in_the_middle.py
+-rw-r--r--   0        0        0    17048 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/meta_field.py
+-rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/sentence_transformers_diversity.py
+-rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/rankers/transformers_similarity.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/readers/__init__.py
+-rw-r--r--   0        0        0    28699 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/readers/extractive.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/__init__.py
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/filter_retriever.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/__init__.py
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
+-rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/__init__.py
+-rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/conditional_router.py
+-rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/file_type_router.py
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/metadata_router.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/text_language_router.py
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/routers/zero_shot_text_router.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/samplers/__init__.py
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/samplers/top_p.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/validators/__init__.py
+-rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/validators/json_schema.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/websearch/__init__.py
+-rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/websearch/searchapi.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/websearch/serper_dev.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/writers/__init__.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/components/writers/document_writer.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/errors.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/serialization.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/type_utils.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/component/__init__.py
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/component/component.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/component/sockets.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/component/types.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/__init__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/descriptions.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/draw.py
+-rw-r--r--   0        0        0    56764 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/template.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/__init__.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/answer.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/byte_stream.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/chat_message.py
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/document.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/sparse_embedding.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/dataclasses/streaming_chunk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/errors/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/errors/errors.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/in_memory/__init__.py
+-rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/in_memory/document_store.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/types/policy.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/document_stores/types/protocol.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/evaluation/__init__.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/evaluation/eval_run_result.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/marshal/__init__.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/marshal/protocol.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/marshal/yaml.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/telemetry/__init__.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/telemetry/_environment.py
+-rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/telemetry/_telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/__init__.py
+-rw-r--r--   0        0        0    63152 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/document_store.py
+-rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/factory.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/test_utils.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/accumulate.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/add_value.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/concatenate.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/double.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/fstring.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/greet.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/hello.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/joiner.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/parity.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/remainder.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/repeat.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/self_loop.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/subtract.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/sum.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/text_splitter.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/testing/sample_components/threshold.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/datadog.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/opentelemetry.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/tracer.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/tracing/utils.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/__init__.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/auth.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/callable_serialization.py
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/device.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/expit.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/filters.py
+-rw-r--r--   0        0        0    15510 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/hf.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/jupyter.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/requests_utils.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/type_serialization.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/haystack/utils/url_validation.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/LICENSE
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/README.md
+-rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.1rc1/PKG-INFO
```

### Comparing `haystack_ai-2.1.0rc2/haystack/__init__.py` & `haystack_ai-2.1.1rc1/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/lazy_imports.py` & `haystack_ai-2.1.1rc1/haystack/lazy_imports.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/logging.py` & `haystack_ai-2.1.1rc1/haystack/logging.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/audio/whisper_local.py` & `haystack_ai-2.1.1rc1/haystack/components/audio/whisper_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/audio/whisper_remote.py` & `haystack_ai-2.1.1rc1/haystack/components/audio/whisper_remote.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/builders/answer_builder.py` & `haystack_ai-2.1.1rc1/haystack/components/builders/answer_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/builders/dynamic_chat_prompt_builder.py` & `haystack_ai-2.1.1rc1/haystack/components/builders/dynamic_chat_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/builders/dynamic_prompt_builder.py` & `haystack_ai-2.1.1rc1/haystack/components/builders/dynamic_prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/builders/prompt_builder.py` & `haystack_ai-2.1.1rc1/haystack/components/builders/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/caching/cache_checker.py` & `haystack_ai-2.1.1rc1/haystack/components/caching/cache_checker.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/classifiers/document_language_classifier.py` & `haystack_ai-2.1.1rc1/haystack/components/classifiers/document_language_classifier.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/connectors/openapi_service.py` & `haystack_ai-2.1.1rc1/haystack/components/connectors/openapi_service.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/__init__.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/azure.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/html.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/html.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/markdown.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/markdown.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/openapi_functions.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/openapi_functions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/output_adapter.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/output_adapter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/pdfminer.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/pdfminer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/pypdf.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/pypdf.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/tika.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/tika.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/txt.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/txt.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/converters/utils.py` & `haystack_ai-2.1.1rc1/haystack/components/converters/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/__init__.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/azure_document_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/azure_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/azure_text_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/azure_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/hugging_face_api_document_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_api_document_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
-            api_type=self.api_type,
+            api_type=str(self.api_type),
             api_params=self.api_params,
             prefix=self.prefix,
             suffix=self.suffix,
             token=self.token.to_dict() if self.token else None,
             truncate=self.truncate,
             normalize=self.normalize,
             batch_size=self.batch_size,
```

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/hugging_face_api_text_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_api_text_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
-            api_type=self.api_type,
+            api_type=str(self.api_type),
             api_params=self.api_params,
             prefix=self.prefix,
             suffix=self.suffix,
             token=self.token.to_dict() if self.token else None,
             truncate=self.truncate,
             normalize=self.normalize,
         )
```

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/hugging_face_tei_document_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/hugging_face_tei_text_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/openai_document_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/openai_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/openai_text_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/openai_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/sentence_transformers_document_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/sentence_transformers_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/sentence_transformers_text_embedder.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/sentence_transformers_text_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/embedders/backends/sentence_transformers_backend.py` & `haystack_ai-2.1.1rc1/haystack/components/embedders/backends/sentence_transformers_backend.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/evaluators/__init__.py` & `haystack_ai-2.1.1rc1/haystack/components/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/evaluators/answer_exact_match.py` & `haystack_ai-2.1.1rc1/haystack/components/evaluators/answer_exact_match.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/evaluators/context_relevance.py` & `haystack_ai-2.1.1rc1/haystack/components/evaluators/context_relevance.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/evaluators/document_map.py` & `haystack_ai-2.1.1rc1/haystack/components/evaluators/document_map.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/evaluators/document_mrr.py` & `haystack_ai-2.1.1rc1/haystack/components/evaluators/document_mrr.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/evaluators/document_recall.py` & `haystack_ai-2.1.1rc1/haystack/components/evaluators/document_recall.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 from typing import Any, Dict, List, Union
 
-from haystack.core.component import component
+from haystack import component, default_to_dict
 from haystack.dataclasses import Document
 
 
 class RecallMode(Enum):
     """
     Enum for the mode to use for calculating the recall score.
     """
@@ -70,14 +70,15 @@
             Mode to use for calculating the recall score.
         """
         if isinstance(mode, str):
             mode = RecallMode.from_str(mode)
 
         mode_functions = {RecallMode.SINGLE_HIT: self._recall_single_hit, RecallMode.MULTI_HIT: self._recall_multi_hit}
         self.mode_function = mode_functions[mode]
+        self.mode = mode
 
     def _recall_single_hit(self, ground_truth_documents: List[Document], retrieved_documents: List[Document]) -> float:
         unique_truths = {g.content for g in ground_truth_documents}
         unique_retrievals = {p.content for p in retrieved_documents}
         retrieved_ground_truths = unique_truths.intersection(unique_retrievals)
 
         return float(len(retrieved_ground_truths) > 0)
@@ -113,7 +114,16 @@
 
         scores = []
         for ground_truth, retrieved in zip(ground_truth_documents, retrieved_documents):
             score = self.mode_function(ground_truth, retrieved)
             scores.append(score)
 
         return {"score": sum(scores) / len(retrieved_documents), "individual_scores": scores}
+
+    def to_dict(self) -> Dict[str, Any]:
+        """
+        Serializes the component to a dictionary.
+
+        :returns:
+            Dictionary with serialized data.
+        """
+        return default_to_dict(self, mode=str(self.mode))
```

### Comparing `haystack_ai-2.1.0rc2/haystack/components/evaluators/faithfulness.py` & `haystack_ai-2.1.1rc1/haystack/components/evaluators/faithfulness.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/evaluators/llm_evaluator.py` & `haystack_ai-2.1.1rc1/haystack/components/evaluators/llm_evaluator.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/evaluators/sas_evaluator.py` & `haystack_ai-2.1.1rc1/haystack/components/evaluators/sas_evaluator.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/extractors/named_entity_extractor.py` & `haystack_ai-2.1.1rc1/haystack/components/extractors/named_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/fetchers/link_content.py` & `haystack_ai-2.1.1rc1/haystack/components/fetchers/link_content.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/__init__.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/azure.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/hugging_face_api.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
         :returns:
             A dictionary containing the serialized component.
         """
         callback_name = serialize_callable(self.streaming_callback) if self.streaming_callback else None
         return default_to_dict(
             self,
-            api_type=self.api_type,
+            api_type=str(self.api_type),
             api_params=self.api_params,
             token=self.token.to_dict() if self.token else None,
             generation_kwargs=self.generation_kwargs,
             streaming_callback=callback_name,
         )
 
     @classmethod
```

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/hugging_face_local.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/hugging_face_tgi.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/hugging_face_tgi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/openai.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/utils.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/chat/__init__.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/chat/azure.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/chat/azure.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/chat/hugging_face_api.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 
         :returns:
             A dictionary containing the serialized component.
         """
         callback_name = serialize_callable(self.streaming_callback) if self.streaming_callback else None
         return default_to_dict(
             self,
-            api_type=self.api_type,
+            api_type=str(self.api_type),
             api_params=self.api_params,
             token=self.token.to_dict() if self.token else None,
             generation_kwargs=self.generation_kwargs,
             streaming_callback=callback_name,
         )
 
     @classmethod
```

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/chat/hugging_face_local.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/chat/hugging_face_tgi.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/chat/hugging_face_tgi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/generators/chat/openai.py` & `haystack_ai-2.1.1rc1/haystack/components/generators/chat/openai.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/joiners/document_joiner.py` & `haystack_ai-2.1.1rc1/haystack/components/joiners/document_joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/others/multiplexer.py` & `haystack_ai-2.1.1rc1/haystack/components/others/multiplexer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/preprocessors/document_cleaner.py` & `haystack_ai-2.1.1rc1/haystack/components/preprocessors/document_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/preprocessors/document_splitter.py` & `haystack_ai-2.1.1rc1/haystack/components/preprocessors/document_splitter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/preprocessors/text_cleaner.py` & `haystack_ai-2.1.1rc1/haystack/components/preprocessors/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/rankers/lost_in_the_middle.py` & `haystack_ai-2.1.1rc1/haystack/components/rankers/lost_in_the_middle.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/rankers/meta_field.py` & `haystack_ai-2.1.1rc1/haystack/components/rankers/meta_field.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/rankers/sentence_transformers_diversity.py` & `haystack_ai-2.1.1rc1/haystack/components/rankers/sentence_transformers_diversity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/rankers/transformers_similarity.py` & `haystack_ai-2.1.1rc1/haystack/components/rankers/transformers_similarity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/readers/extractive.py` & `haystack_ai-2.1.1rc1/haystack/components/readers/extractive.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/retrievers/filter_retriever.py` & `haystack_ai-2.1.1rc1/haystack/components/retrievers/filter_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/retrievers/in_memory/bm25_retriever.py` & `haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/retrievers/in_memory/embedding_retriever.py` & `haystack_ai-2.1.1rc1/haystack/components/retrievers/in_memory/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/routers/__init__.py` & `haystack_ai-2.1.1rc1/haystack/components/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/routers/conditional_router.py` & `haystack_ai-2.1.1rc1/haystack/components/routers/conditional_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/routers/file_type_router.py` & `haystack_ai-2.1.1rc1/haystack/components/routers/file_type_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/routers/metadata_router.py` & `haystack_ai-2.1.1rc1/haystack/components/routers/metadata_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/routers/text_language_router.py` & `haystack_ai-2.1.1rc1/haystack/components/routers/text_language_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/routers/zero_shot_text_router.py` & `haystack_ai-2.1.1rc1/haystack/components/routers/zero_shot_text_router.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/samplers/top_p.py` & `haystack_ai-2.1.1rc1/haystack/components/samplers/top_p.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/validators/json_schema.py` & `haystack_ai-2.1.1rc1/haystack/components/validators/json_schema.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/websearch/searchapi.py` & `haystack_ai-2.1.1rc1/haystack/components/websearch/searchapi.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/websearch/serper_dev.py` & `haystack_ai-2.1.1rc1/haystack/components/websearch/serper_dev.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/components/writers/document_writer.py` & `haystack_ai-2.1.1rc1/haystack/components/writers/document_writer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/errors.py` & `haystack_ai-2.1.1rc1/haystack/core/errors.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/serialization.py` & `haystack_ai-2.1.1rc1/haystack/core/serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/type_utils.py` & `haystack_ai-2.1.1rc1/haystack/core/type_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/component/component.py` & `haystack_ai-2.1.1rc1/haystack/core/component/component.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/component/sockets.py` & `haystack_ai-2.1.1rc1/haystack/core/component/sockets.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/component/types.py` & `haystack_ai-2.1.1rc1/haystack/core/component/types.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/pipeline/descriptions.py` & `haystack_ai-2.1.1rc1/haystack/core/pipeline/descriptions.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/pipeline/draw.py` & `haystack_ai-2.1.1rc1/haystack/core/pipeline/draw.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/pipeline/pipeline.py` & `haystack_ai-2.1.1rc1/haystack/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/pipeline/template.py` & `haystack_ai-2.1.1rc1/haystack/core/pipeline/template.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2` & `haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2` & `haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/pipeline/predefined/indexing.yaml.jinja2` & `haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/core/pipeline/predefined/rag.yaml.jinja2` & `haystack_ai-2.1.1rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/dataclasses/__init__.py` & `haystack_ai-2.1.1rc1/haystack/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/dataclasses/answer.py` & `haystack_ai-2.1.1rc1/haystack/dataclasses/answer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/dataclasses/byte_stream.py` & `haystack_ai-2.1.1rc1/haystack/dataclasses/byte_stream.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/dataclasses/chat_message.py` & `haystack_ai-2.1.1rc1/haystack/dataclasses/chat_message.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/dataclasses/document.py` & `haystack_ai-2.1.1rc1/haystack/dataclasses/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,17 +135,14 @@
         """
         data = asdict(self)
         if (dataframe := data.get("dataframe")) is not None:
             data["dataframe"] = dataframe.to_json()
         if (blob := data.get("blob")) is not None:
             data["blob"] = {"data": list(blob["data"]), "mime_type": blob["mime_type"]}
 
-        if (sparse_embedding := data.get("sparse_embedding")) is not None:
-            data["sparse_embedding"] = sparse_embedding.to_dict()
-
         if flatten:
             meta = data.pop("meta")
             return {**data, **meta}
 
         return data
 
     @classmethod
```

### Comparing `haystack_ai-2.1.0rc2/haystack/dataclasses/sparse_embedding.py` & `haystack_ai-2.1.1rc1/haystack/dataclasses/sparse_embedding.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-from typing import List
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
 
+from dataclasses import asdict, dataclass
+from typing import Any, Dict, List
 
+
+@dataclass
 class SparseEmbedding:
     """
     Class representing a sparse embedding.
+
+    :param indices: List of indices of non-zero elements in the embedding.
+    :param values: List of values of non-zero elements in the embedding.
     """
 
-    def __init__(self, indices: List[int], values: List[float]):
-        """
-        Initialize a SparseEmbedding object.
+    indices: List[int]
+    values: List[float]
 
-        :param indices: List of indices of non-zero elements in the embedding.
-        :param values: List of values of non-zero elements in the embedding.
+    def __post_init__(self):
+        """
+        Checks if the indices and values lists are of the same length.
 
-        :raises ValueError: If the indices and values lists are not of the same length.
+        Raises a ValueError if they are not.
         """
-        if len(indices) != len(values):
+        if len(self.indices) != len(self.values):
             raise ValueError("Length of indices and values must be the same.")
-        self.indices = indices
-        self.values = values
-
-    def __eq__(self, other):
-        return self.indices == other.indices and self.values == other.values
 
-    def to_dict(self):
+    def to_dict(self) -> Dict[str, Any]:
         """
         Convert the SparseEmbedding object to a dictionary.
 
         :returns:
             Serialized sparse embedding.
         """
-        return {"indices": self.indices, "values": self.values}
+        return asdict(self)
 
     @classmethod
-    def from_dict(cls, sparse_embedding_dict):
+    def from_dict(cls, sparse_embedding_dict: Dict[str, Any]) -> "SparseEmbedding":
         """
         Deserializes the sparse embedding from a dictionary.
 
         :param sparse_embedding_dict:
             Dictionary to deserialize from.
         :returns:
             Deserialized sparse embedding.
         """
-        return cls(indices=sparse_embedding_dict["indices"], values=sparse_embedding_dict["values"])
+        return cls(**sparse_embedding_dict)
```

### Comparing `haystack_ai-2.1.0rc2/haystack/dataclasses/streaming_chunk.py` & `haystack_ai-2.1.1rc1/haystack/dataclasses/streaming_chunk.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/document_stores/in_memory/document_store.py` & `haystack_ai-2.1.1rc1/haystack/document_stores/in_memory/document_store.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/document_stores/types/protocol.py` & `haystack_ai-2.1.1rc1/haystack/document_stores/types/protocol.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/evaluation/eval_run_result.py` & `haystack_ai-2.1.1rc1/haystack/evaluation/eval_run_result.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/telemetry/_environment.py` & `haystack_ai-2.1.1rc1/haystack/telemetry/_environment.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/telemetry/_telemetry.py` & `haystack_ai-2.1.1rc1/haystack/telemetry/_telemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/document_store.py` & `haystack_ai-2.1.1rc1/haystack/testing/document_store.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/factory.py` & `haystack_ai-2.1.1rc1/haystack/testing/factory.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/test_utils.py` & `haystack_ai-2.1.1rc1/haystack/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/__init__.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/accumulate.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/accumulate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/add_value.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/add_value.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/concatenate.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/concatenate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/fstring.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/fstring.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/greet.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/greet.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/joiner.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/joiner.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/parity.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/parity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/remainder.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/remainder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/self_loop.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/self_loop.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/subtract.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/subtract.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/testing/sample_components/threshold.py` & `haystack_ai-2.1.1rc1/haystack/testing/sample_components/threshold.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/tracing/datadog.py` & `haystack_ai-2.1.1rc1/haystack/tracing/datadog.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/tracing/opentelemetry.py` & `haystack_ai-2.1.1rc1/haystack/tracing/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/tracing/tracer.py` & `haystack_ai-2.1.1rc1/haystack/tracing/tracer.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/tracing/utils.py` & `haystack_ai-2.1.1rc1/haystack/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/utils/__init__.py` & `haystack_ai-2.1.1rc1/haystack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/utils/auth.py` & `haystack_ai-2.1.1rc1/haystack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/utils/callable_serialization.py` & `haystack_ai-2.1.1rc1/haystack/utils/callable_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/utils/device.py` & `haystack_ai-2.1.1rc1/haystack/utils/device.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/utils/filters.py` & `haystack_ai-2.1.1rc1/haystack/utils/filters.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/utils/hf.py` & `haystack_ai-2.1.1rc1/haystack/utils/hf.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/utils/jupyter.py` & `haystack_ai-2.1.1rc1/haystack/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/utils/requests_utils.py` & `haystack_ai-2.1.1rc1/haystack/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/haystack/utils/type_serialization.py` & `haystack_ai-2.1.1rc1/haystack/utils/type_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/.gitignore` & `haystack_ai-2.1.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/LICENSE` & `haystack_ai-2.1.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/README.md` & `haystack_ai-2.1.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/pyproject.toml` & `haystack_ai-2.1.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.1.0rc2/PKG-INFO` & `haystack_ai-2.1.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haystack-ai
-Version: 2.1.0rc2
+Version: 2.1.1rc1
 Summary: LLM framework to build customizable, production-ready LLM applications. Connect components (models, vector DBs, file converters) to pipelines or agents that can interact with your data.
 Project-URL: CI: GitHub, https://github.com/deepset-ai/haystack/actions
 Project-URL: Docs: RTD, https://haystack.deepset.ai/overview/intro
 Project-URL: GitHub: issues, https://github.com/deepset-ai/haystack/issues
 Project-URL: GitHub: repo, https://github.com/deepset-ai/haystack
 Project-URL: Homepage, https://github.com/deepset-ai/haystack
 Author-email: "deepset.ai" <malte.pietsch@deepset.ai>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: haystack-ai Version: 2.1.0rc2 Summary: LLM
+Metadata-Version: 2.3 Name: haystack-ai Version: 2.1.1rc1 Summary: LLM
 framework to build customizable, production-ready LLM applications. Connect
 components (models, vector DBs, file converters) to pipelines or agents that
 can interact with your data. Project-URL: CI: GitHub, https://github.com/
 deepset-ai/haystack/actions Project-URL: Docs: RTD, https://
 haystack.deepset.ai/overview/intro Project-URL: GitHub: issues, https://
 github.com/deepset-ai/haystack/issues Project-URL: GitHub: repo, https://
 github.com/deepset-ai/haystack Project-URL: Homepage, https://github.com/
```


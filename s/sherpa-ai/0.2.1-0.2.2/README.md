# Comparing `tmp/sherpa_ai-0.2.1.tar.gz` & `tmp/sherpa_ai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa_ai-0.2.1.tar", max compression
+gzip compressed data, was "sherpa_ai-0.2.2.tar", max compression
```

## Comparing `sherpa_ai-0.2.1.tar` & `sherpa_ai-0.2.2.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0     1279 2024-04-24 02:25:14.174706 sherpa_ai-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-09-07 18:58:13.889346 sherpa_ai-0.2.1/README.md
--rw-r--r--   0        0        0       23 2023-09-07 18:58:13.896351 sherpa_ai-0.2.1/sherpa_ai/__init__.py
--rw-r--r--   0        0        0      203 2023-10-22 21:42:20.082581 sherpa_ai-0.2.1/sherpa_ai/action_planner/__init__.py
--rw-r--r--   0        0        0     3888 2023-12-19 19:27:04.507940 sherpa_ai-0.2.1/sherpa_ai/action_planner/action_planner.py
--rw-r--r--   0        0        0      285 2023-12-19 19:27:04.507940 sherpa_ai-0.2.1/sherpa_ai/action_planner/base.py
--rw-r--r--   0        0        0     1427 2023-11-22 04:28:04.077007 sherpa_ai-0.2.1/sherpa_ai/action_planner/selective_planner.py
--rw-r--r--   0        0        0       66 2023-10-22 21:42:20.092581 sherpa_ai-0.2.1/sherpa_ai/action_planner/simple_planner.py
--rw-r--r--   0        0        0      409 2024-04-11 01:46:59.690575 sherpa_ai-0.2.1/sherpa_ai/actions/__init__.py
--rw-r--r--   0        0        0     1684 2024-02-28 14:01:30.482499 sherpa_ai-0.2.1/sherpa_ai/actions/arxiv_search.py
--rw-r--r--   0        0        0      482 2023-12-19 19:27:04.509940 sherpa_ai-0.2.1/sherpa_ai/actions/base.py
--rw-r--r--   0        0        0     1787 2023-12-19 19:27:04.510941 sherpa_ai-0.2.1/sherpa_ai/actions/context_search.py
--rw-r--r--   0        0        0     1331 2023-12-19 19:27:04.510941 sherpa_ai-0.2.1/sherpa_ai/actions/deliberation.py
--rw-r--r--   0        0        0     2918 2024-02-28 14:01:30.482499 sherpa_ai-0.2.1/sherpa_ai/actions/google_search.py
--rw-r--r--   0        0        0     5641 2023-12-19 19:27:04.512941 sherpa_ai-0.2.1/sherpa_ai/actions/planning.py
--rw-r--r--   0        0        0     1918 2024-03-01 16:22:17.952293 sherpa_ai-0.2.1/sherpa_ai/actions/synthesize.py
--rw-r--r--   0        0        0      493 2024-02-20 04:55:11.807341 sherpa_ai-0.2.1/sherpa_ai/agents/__init__.py
--rw-r--r--   0        0        0     1177 2023-11-22 02:47:37.184142 sherpa_ai-0.2.1/sherpa_ai/agents/agent_pool.py
--rw-r--r--   0        0        0     4886 2024-03-01 16:17:05.632211 sherpa_ai-0.2.1/sherpa_ai/agents/base.py
--rw-r--r--   0        0        0     5146 2023-12-19 19:27:04.514940 sherpa_ai-0.2.1/sherpa_ai/agents/critic.py
--rw-r--r--   0        0        0     2895 2024-02-28 14:01:30.483423 sherpa_ai-0.2.1/sherpa_ai/agents/ml_engineer.py
--rw-r--r--   0        0        0     2581 2024-02-28 14:01:30.483423 sherpa_ai-0.2.1/sherpa_ai/agents/physicist.py
--rw-r--r--   0        0        0     2849 2023-12-19 19:27:04.515940 sherpa_ai-0.2.1/sherpa_ai/agents/planner.py
--rw-r--r--   0        0        0     4838 2024-04-08 03:33:58.816371 sherpa_ai-0.2.1/sherpa_ai/agents/qa_agent.py
--rw-r--r--   0        0        0     1665 2023-10-22 21:42:20.116222 sherpa_ai-0.2.1/sherpa_ai/agents/user.py
--rw-r--r--   0        0        0     3984 2024-04-24 02:25:02.470359 sherpa_ai-0.2.1/sherpa_ai/config/__init__.py
--rw-r--r--   0        0        0     3025 2024-01-17 05:47:33.698412 sherpa_ai-0.2.1/sherpa_ai/config/task_config.py
--rw-r--r--   0        0        0     4220 2024-04-24 02:25:02.472359 sherpa_ai-0.2.1/sherpa_ai/connectors/chroma_vector_store.py
--rw-r--r--   0        0        0     2547 2024-04-24 02:25:02.470359 sherpa_ai-0.2.1/sherpa_ai/connectors/ChromaVectorStore.py
--rw-r--r--   0        0        0     1424 2023-09-14 14:00:23.450118 sherpa_ai-0.2.1/sherpa_ai/connectors/scripts/load_dump_to_chroma.py
--rw-r--r--   0        0        0     1249 2023-09-14 14:00:23.451116 sherpa_ai-0.2.1/sherpa_ai/connectors/scripts/query_chroma.py
--rw-r--r--   0        0        0     6843 2024-02-07 04:00:13.352018 sherpa_ai-0.2.1/sherpa_ai/connectors/vectorstores.py
--rw-r--r--   0        0        0      102 2023-09-07 18:58:13.900426 sherpa_ai-0.2.1/sherpa_ai/database/__init__.py
--rw-r--r--   0        0        0    15320 2024-04-24 02:25:02.475359 sherpa_ai-0.2.1/sherpa_ai/database/user_usage_tracker.py
--rw-r--r--   0        0        0      111 2023-09-07 18:58:13.901553 sherpa_ai-0.2.1/sherpa_ai/error_handling/__init__.py
--rw-r--r--   0        0        0     1762 2023-09-07 18:58:13.901553 sherpa_ai-0.2.1/sherpa_ai/error_handling/agent_error_handler.py
--rw-r--r--   0        0        0      861 2024-04-24 02:25:02.476359 sherpa_ai-0.2.1/sherpa_ai/events.py
--rw-r--r--   0        0        0      141 2023-10-22 21:42:20.118096 sherpa_ai-0.2.1/sherpa_ai/memory/__init__.py
--rw-r--r--   0        0        0     5441 2024-04-24 02:25:02.479359 sherpa_ai-0.2.1/sherpa_ai/memory/belief.py
--rw-r--r--   0        0        0     2171 2024-02-28 14:01:30.484418 sherpa_ai-0.2.1/sherpa_ai/memory/shared_memory.py
--rw-r--r--   0        0        0     2170 2024-04-24 02:25:02.481359 sherpa_ai-0.2.1/sherpa_ai/memory/shared_memory_with_vectordb.py
--rw-r--r--   0        0        0      181 2023-09-07 18:58:13.902558 sherpa_ai-0.2.1/sherpa_ai/models/__init__.py
--rw-r--r--   0        0        0     2066 2024-02-15 02:06:06.152905 sherpa_ai-0.2.1/sherpa_ai/models/chat_model_with_logging.py
--rw-r--r--   0        0        0     3224 2024-02-20 04:55:11.812339 sherpa_ai-0.2.1/sherpa_ai/models/sherpa_base_chat_model.py
--rw-r--r--   0        0        0     1510 2024-04-03 04:17:33.589955 sherpa_ai-0.2.1/sherpa_ai/models/sherpa_base_model.py
--rw-r--r--   0        0        0     4402 2023-10-22 21:42:20.122097 sherpa_ai-0.2.1/sherpa_ai/orchestrator.py
--rw-r--r--   0        0        0     1616 2023-09-07 18:58:13.904341 sherpa_ai-0.2.1/sherpa_ai/output_parser.py
--rw-r--r--   0        0        0      474 2024-02-28 14:01:30.485416 sherpa_ai-0.2.1/sherpa_ai/output_parsers/__init__.py
--rw-r--r--   0        0        0     1953 2024-02-28 14:01:30.485416 sherpa_ai-0.2.1/sherpa_ai/output_parsers/base.py
--rw-r--r--   0        0        0    11374 2024-04-24 02:25:02.483363 sherpa_ai-0.2.1/sherpa_ai/output_parsers/citation_validation.py
--rw-r--r--   0        0        0     4165 2024-02-15 02:06:06.155286 sherpa_ai-0.2.1/sherpa_ai/output_parsers/link_parse.py
--rw-r--r--   0        0        0     1485 2024-02-15 02:06:06.155286 sherpa_ai-0.2.1/sherpa_ai/output_parsers/md_to_slack_parse.py
--rw-r--r--   0        0        0     2062 2024-04-04 20:47:25.540942 sherpa_ai-0.2.1/sherpa_ai/output_parsers/number_validation.py
--rw-r--r--   0        0        0      715 2024-04-03 04:17:33.590956 sherpa_ai-0.2.1/sherpa_ai/output_parsers/validation_result.py
--rw-r--r--   0        0        0      274 2023-09-07 18:58:13.905751 sherpa_ai-0.2.1/sherpa_ai/post_processors.py
--rw-r--r--   0        0        0     2834 2024-02-15 02:06:06.156687 sherpa_ai-0.2.1/sherpa_ai/prompt.py
--rw-r--r--   0        0        0     6810 2023-09-07 18:58:13.906764 sherpa_ai-0.2.1/sherpa_ai/prompt_generator.py
--rw-r--r--   0        0        0     2700 2023-09-07 18:58:13.906764 sherpa_ai-0.2.1/sherpa_ai/reflection.py
--rw-r--r--   0        0        0     3226 2024-03-07 04:24:18.869369 sherpa_ai-0.2.1/sherpa_ai/scrape/extract_github_readme.py
--rw-r--r--   0        0        0     5252 2024-04-03 04:17:33.591954 sherpa_ai-0.2.1/sherpa_ai/scrape/file_scraper.py
--rw-r--r--   0        0        0     3588 2024-04-03 04:17:33.591954 sherpa_ai-0.2.1/sherpa_ai/scrape/prompt_reconstructor.py
--rw-r--r--   0        0        0    10509 2024-02-15 02:06:06.156687 sherpa_ai-0.2.1/sherpa_ai/task_agent.py
--rw-r--r--   0        0        0      327 2024-02-28 14:01:30.486415 sherpa_ai-0.2.1/sherpa_ai/test_utils/data.py
--rw-r--r--   0        0        0     1752 2024-03-07 05:54:44.991058 sherpa_ai-0.2.1/sherpa_ai/test_utils/llms.py
--rw-r--r--   0        0        0      755 2023-12-19 20:27:38.204282 sherpa_ai-0.2.1/sherpa_ai/test_utils/loggers.py
--rw-r--r--   0        0        0    10200 2024-04-16 16:58:00.924883 sherpa_ai-0.2.1/sherpa_ai/tools.py
--rw-r--r--   0        0        0    13170 2024-04-04 20:47:25.541939 sherpa_ai-0.2.1/sherpa_ai/utils.py
--rw-r--r--   0        0        0      238 2024-02-15 02:06:06.158160 sherpa_ai-0.2.1/sherpa_ai/verbose_loggers/__init__.py
--rw-r--r--   0        0        0      141 2023-09-07 18:58:13.910518 sherpa_ai-0.2.1/sherpa_ai/verbose_loggers/base.py
--rw-r--r--   0        0        0     1012 2023-11-20 05:23:41.530778 sherpa_ai-0.2.1/sherpa_ai/verbose_loggers/verbose_loggers.py
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 sherpa_ai-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1283 2024-05-09 20:02:46.580171 sherpa_ai-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-09-07 18:58:13.889346 sherpa_ai-0.2.2/README.md
+-rw-r--r--   0        0        0       23 2023-09-07 18:58:13.896351 sherpa_ai-0.2.2/sherpa_ai/__init__.py
+-rw-r--r--   0        0        0      205 2024-05-09 19:39:19.720388 sherpa_ai-0.2.2/sherpa_ai/action_planner/__init__.py
+-rw-r--r--   0        0        0     3890 2024-05-09 19:39:19.720388 sherpa_ai-0.2.2/sherpa_ai/action_planner/action_planner.py
+-rw-r--r--   0        0        0      285 2024-05-09 19:39:19.721388 sherpa_ai-0.2.2/sherpa_ai/action_planner/base.py
+-rw-r--r--   0        0        0     1427 2024-05-09 19:39:19.721388 sherpa_ai-0.2.2/sherpa_ai/action_planner/selective_planner.py
+-rw-r--r--   0        0        0       66 2024-05-09 19:39:19.722391 sherpa_ai-0.2.2/sherpa_ai/action_planner/simple_planner.py
+-rw-r--r--   0        0        0      411 2024-05-06 03:04:54.059411 sherpa_ai-0.2.2/sherpa_ai/actions/__init__.py
+-rw-r--r--   0        0        0     1888 2024-05-09 20:02:46.581179 sherpa_ai-0.2.2/sherpa_ai/actions/arxiv_search.py
+-rw-r--r--   0        0        0     1216 2024-05-09 20:02:46.581179 sherpa_ai-0.2.2/sherpa_ai/actions/base.py
+-rw-r--r--   0        0        0     2023 2024-05-07 20:39:30.696736 sherpa_ai-0.2.2/sherpa_ai/actions/context_search.py
+-rw-r--r--   0        0        0     1333 2024-05-06 03:04:54.060480 sherpa_ai-0.2.2/sherpa_ai/actions/deliberation.py
+-rw-r--r--   0        0        0     2301 2024-05-09 20:02:46.582170 sherpa_ai-0.2.2/sherpa_ai/actions/google_search.py
+-rw-r--r--   0        0        0     5643 2024-05-06 03:04:54.061421 sherpa_ai-0.2.2/sherpa_ai/actions/planning.py
+-rw-r--r--   0        0        0     1918 2024-05-06 03:04:54.061421 sherpa_ai-0.2.2/sherpa_ai/actions/synthesize.py
+-rw-r--r--   0        0        0      495 2024-05-06 03:04:54.062428 sherpa_ai-0.2.2/sherpa_ai/agents/__init__.py
+-rw-r--r--   0        0        0     1177 2023-11-22 02:47:37.184142 sherpa_ai-0.2.2/sherpa_ai/agents/agent_pool.py
+-rw-r--r--   0        0        0     5678 2024-05-09 19:39:19.722391 sherpa_ai-0.2.2/sherpa_ai/agents/base.py
+-rw-r--r--   0        0        0     5148 2024-05-06 03:04:54.062428 sherpa_ai-0.2.2/sherpa_ai/agents/critic.py
+-rw-r--r--   0        0        0     2897 2024-05-09 19:39:19.723389 sherpa_ai-0.2.2/sherpa_ai/agents/ml_engineer.py
+-rw-r--r--   0        0        0     2583 2024-05-09 19:39:19.723389 sherpa_ai-0.2.2/sherpa_ai/agents/physicist.py
+-rw-r--r--   0        0        0     2850 2024-05-06 03:04:54.063492 sherpa_ai-0.2.2/sherpa_ai/agents/planner.py
+-rw-r--r--   0        0        0     4783 2024-05-09 19:39:19.723389 sherpa_ai-0.2.2/sherpa_ai/agents/qa_agent.py
+-rw-r--r--   0        0        0     1665 2023-10-22 21:42:20.116222 sherpa_ai-0.2.2/sherpa_ai/agents/user.py
+-rw-r--r--   0        0        0     5186 2024-05-09 20:02:46.583170 sherpa_ai-0.2.2/sherpa_ai/config/__init__.py
+-rw-r--r--   0        0        0     3025 2024-01-17 05:47:33.698412 sherpa_ai-0.2.2/sherpa_ai/config/task_config.py
+-rw-r--r--   0        0        0     4220 2024-04-24 02:25:02.472359 sherpa_ai-0.2.2/sherpa_ai/connectors/chroma_vector_store.py
+-rw-r--r--   0        0        0     2635 2024-05-06 03:04:54.065452 sherpa_ai-0.2.2/sherpa_ai/connectors/ChromaVectorStore.py
+-rw-r--r--   0        0        0     1424 2023-09-14 14:00:23.450118 sherpa_ai-0.2.2/sherpa_ai/connectors/scripts/load_dump_to_chroma.py
+-rw-r--r--   0        0        0     1249 2023-09-14 14:00:23.451116 sherpa_ai-0.2.2/sherpa_ai/connectors/scripts/query_chroma.py
+-rw-r--r--   0        0        0     6843 2024-02-07 04:00:13.352018 sherpa_ai-0.2.2/sherpa_ai/connectors/vectorstores.py
+-rw-r--r--   0        0        0      104 2024-05-06 03:04:54.065452 sherpa_ai-0.2.2/sherpa_ai/database/__init__.py
+-rw-r--r--   0        0        0    15195 2024-05-07 20:39:30.698736 sherpa_ai-0.2.2/sherpa_ai/database/user_usage_tracker.py
+-rw-r--r--   0        0        0      113 2024-05-06 03:04:54.065452 sherpa_ai-0.2.2/sherpa_ai/error_handling/__init__.py
+-rw-r--r--   0        0        0     1762 2023-09-07 18:58:13.901553 sherpa_ai-0.2.2/sherpa_ai/error_handling/agent_error_handler.py
+-rw-r--r--   0        0        0      861 2024-04-24 02:25:02.476359 sherpa_ai-0.2.2/sherpa_ai/events.py
+-rw-r--r--   0        0        0      143 2024-05-06 03:04:54.066434 sherpa_ai-0.2.2/sherpa_ai/memory/__init__.py
+-rw-r--r--   0        0        0     5441 2024-04-24 02:25:02.479359 sherpa_ai-0.2.2/sherpa_ai/memory/belief.py
+-rw-r--r--   0        0        0     2173 2024-05-06 03:04:54.066434 sherpa_ai-0.2.2/sherpa_ai/memory/shared_memory.py
+-rw-r--r--   0        0        0     2170 2024-04-24 02:25:02.481359 sherpa_ai-0.2.2/sherpa_ai/memory/shared_memory_with_vectordb.py
+-rw-r--r--   0        0        0      183 2024-05-06 03:04:54.066434 sherpa_ai-0.2.2/sherpa_ai/models/__init__.py
+-rw-r--r--   0        0        0     2066 2024-02-15 02:06:06.152905 sherpa_ai-0.2.2/sherpa_ai/models/chat_model_with_logging.py
+-rw-r--r--   0        0        0     3224 2024-02-20 04:55:11.812339 sherpa_ai-0.2.2/sherpa_ai/models/sherpa_base_chat_model.py
+-rw-r--r--   0        0        0     1542 2024-05-06 03:04:54.066434 sherpa_ai-0.2.2/sherpa_ai/models/sherpa_base_model.py
+-rw-r--r--   0        0        0     4402 2023-10-22 21:42:20.122097 sherpa_ai-0.2.2/sherpa_ai/orchestrator.py
+-rw-r--r--   0        0        0     1616 2023-09-07 18:58:13.904341 sherpa_ai-0.2.2/sherpa_ai/output_parser.py
+-rw-r--r--   0        0        0      574 2024-05-06 03:04:54.066434 sherpa_ai-0.2.2/sherpa_ai/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1953 2024-02-28 14:01:30.485416 sherpa_ai-0.2.2/sherpa_ai/output_parsers/base.py
+-rw-r--r--   0        0        0    11270 2024-05-09 20:02:46.583170 sherpa_ai-0.2.2/sherpa_ai/output_parsers/citation_validation.py
+-rw-r--r--   0        0        0     4510 2024-05-06 03:04:54.067499 sherpa_ai-0.2.2/sherpa_ai/output_parsers/entity_validation.py
+-rw-r--r--   0        0        0     4165 2024-02-15 02:06:06.155286 sherpa_ai-0.2.2/sherpa_ai/output_parsers/link_parse.py
+-rw-r--r--   0        0        0     1485 2024-02-15 02:06:06.155286 sherpa_ai-0.2.2/sherpa_ai/output_parsers/md_to_slack_parse.py
+-rw-r--r--   0        0        0     2072 2024-05-06 03:04:54.067499 sherpa_ai-0.2.2/sherpa_ai/output_parsers/number_validation.py
+-rw-r--r--   0        0        0      715 2024-04-03 04:17:33.590956 sherpa_ai-0.2.2/sherpa_ai/output_parsers/validation_result.py
+-rw-r--r--   0        0        0      274 2023-09-07 18:58:13.905751 sherpa_ai-0.2.2/sherpa_ai/post_processors.py
+-rw-r--r--   0        0        0     2834 2024-02-15 02:06:06.156687 sherpa_ai-0.2.2/sherpa_ai/prompt.py
+-rw-r--r--   0        0        0     6812 2024-05-06 03:04:54.068411 sherpa_ai-0.2.2/sherpa_ai/prompt_generator.py
+-rw-r--r--   0        0        0     2700 2023-09-07 18:58:13.906764 sherpa_ai-0.2.2/sherpa_ai/reflection.py
+-rw-r--r--   0        0        0     3372 2024-05-07 20:39:30.699736 sherpa_ai-0.2.2/sherpa_ai/scrape/extract_github_readme.py
+-rw-r--r--   0        0        0     5330 2024-05-07 20:39:30.700735 sherpa_ai-0.2.2/sherpa_ai/scrape/file_scraper.py
+-rw-r--r--   0        0        0     3588 2024-04-03 04:17:33.591954 sherpa_ai-0.2.2/sherpa_ai/scrape/prompt_reconstructor.py
+-rw-r--r--   0        0        0    10509 2024-05-09 19:39:19.724388 sherpa_ai-0.2.2/sherpa_ai/task_agent.py
+-rw-r--r--   0        0        0      327 2024-02-28 14:01:30.486415 sherpa_ai-0.2.2/sherpa_ai/test_utils/data.py
+-rw-r--r--   0        0        0     1752 2024-03-07 05:54:44.991058 sherpa_ai-0.2.2/sherpa_ai/test_utils/llms.py
+-rw-r--r--   0        0        0      755 2023-12-19 20:27:38.204282 sherpa_ai-0.2.2/sherpa_ai/test_utils/loggers.py
+-rw-r--r--   0        0        0    10741 2024-05-09 20:02:46.584171 sherpa_ai-0.2.2/sherpa_ai/tools.py
+-rw-r--r--   0        0        0    21444 2024-05-07 20:39:30.703244 sherpa_ai-0.2.2/sherpa_ai/utils.py
+-rw-r--r--   0        0        0      240 2024-05-06 03:04:54.069409 sherpa_ai-0.2.2/sherpa_ai/verbose_loggers/__init__.py
+-rw-r--r--   0        0        0      141 2023-09-07 18:58:13.910518 sherpa_ai-0.2.2/sherpa_ai/verbose_loggers/base.py
+-rw-r--r--   0        0        0     1012 2023-11-20 05:23:41.530778 sherpa_ai-0.2.2/sherpa_ai/verbose_loggers/verbose_loggers.py
+-rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 sherpa_ai-0.2.2/PKG-INFO
```

### Comparing `sherpa_ai-0.2.1/pyproject.toml` & `sherpa_ai-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "sherpa-ai"
-version = "0.2.1"
+version = "0.2.2"
 description = "Sherpa: AI-augmented thinking companion"
 authors = []
 readme = "README.md"
 repository = "https://github.com/Aggregate-Intellect/sherpa"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 langchain = "0.0.332"
 python-dotenv = "^1.0.0"
 unstructured = "^0.10.11"
 openai = "^0.28.0"
 chromadb = "^0.4.8"
-tiktoken = "^0.4.0"
+tiktoken = ">=0.6.0,<1.0"
 pinecone-client = "^2.2.2"
 beautifulsoup4 = "4.12.2"
 markdown = ">=3.4.4,<3.5.0"
 loguru = ">=0.7.0,<0.8.0"
 boto3 = "^1.28.77"
 pypdf = "^3.17.0"
 transformers = "^4.35.2"
@@ -28,18 +28,20 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "7.4.0"
 pytest-cov = "^4.1.0"
 
 
 [tool.poetry.group.lint.dependencies]
-black = "23.7.0"
-flake8 = "6.1.0"
-isort = "5.12.0"
-flake8-pyproject = "1.2.3"
+bandit = "^1.7.8"
+black = "^23.7.0"
+flake8 = "^6.1.0"
+isort = "^5.12.0"
+flake8-pyproject = "^1.2.3"
+mypy = "^1.9.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = [
@@ -50,15 +52,12 @@
 ]
 
 [tool.black]
 line-length = 88
 
 [tool.flake8]
 max-line-length = 88
-ignore  = ['F401', 'W503']
-per-file-ignores = [
-    'bolt_app.py:E402',
-]
+ignore  = ['F401', 'W503', 'E501']
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/action_planner/action_planner.py` & `sherpa_ai-0.2.2/sherpa_ai/action_planner/action_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import TYPE_CHECKING, Optional, Tuple
 
 from langchain.base_language import BaseLanguageModel
 from loguru import logger
 
 from sherpa_ai.action_planner.base import BaseActionPlanner
 
+
 if TYPE_CHECKING:
     from sherpa_ai.memory.belief import Belief
 
 SELECTION_DESCRIPTION = """{role_description}
 
 {output_instruction}
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/action_planner/selective_planner.py` & `sherpa_ai-0.2.2/sherpa_ai/action_planner/selective_planner.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/actions/arxiv_search.py` & `sherpa_ai-0.2.2/sherpa_ai/actions/arxiv_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from langchain.base_language import BaseLanguageModel
 
-from sherpa_ai.actions.base import BaseAction
-from sherpa_ai.tools import SearchArxivTool, SearchTool
+from sherpa_ai.actions.base import ActionResource, BaseAction
+from sherpa_ai.tools import SearchArxivTool
+
 
 SEARCH_SUMMARY_DESCRIPTION = """Role Description: {role_description}
 Task: {task}
 
 Relevant Paper Title and Summary:
 {paper_title_summary}
 
@@ -26,19 +27,21 @@
     ):
         self.role_description = role_description
         self.task = task
 
         self.description = description
         self.llm = llm
         self.max_results = max_results
+        self.action_resources = []
 
         self.search_tool = SearchArxivTool()
 
     def execute(self, query) -> str:
-        result = self.search_tool._run(query)
+        result, resources = self.search_tool._run(query, return_resources=True)
+        self.add_resources(resources)
 
         prompt = self.description.format(
             task=self.task,
             paper_title_summary=result,
             n=self.max_results,
             role_description=self.role_description,
         )
@@ -50,7 +53,11 @@
     @property
     def name(self) -> str:
         return "ArxivSearch"
 
     @property
     def args(self) -> dict:
         return {"query": "string"}
+
+    @property
+    def resources(self) -> list:
+        return self.action_resources
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/actions/context_search.py` & `sherpa_ai-0.2.2/sherpa_ai/actions/context_search.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from langchain.base_language import BaseLanguageModel
 from loguru import logger
 
-from sherpa_ai.actions.base import BaseAction
+from sherpa_ai.actions.base import ActionResource, BaseAction
 from sherpa_ai.connectors.vectorstores import get_vectordb
 from sherpa_ai.tools import ContextTool
 
+
 SEARCH_SUMMARY_DESCRIPTION = """Role Description: {role_description}
 Task: {task}
 
 Relevant Documents:
 {documents}
 
 
@@ -28,19 +29,23 @@
     ):
         self.role_description = role_description
         self.task = task
 
         self.description = description
         self.llm = llm
         self.n = n
+        self.action_resources = []
 
         self.context = ContextTool(memory=get_vectordb())
 
     def execute(self, query) -> str:
-        result = self.context._run(query)
+        result, resources = self.context._run(query, return_resources=True)
+
+        self.add_resources(resources)
+
         # result = "Context Search"
         logger.debug("Context Search Result: {}", result)
 
         prompt = self.description.format(
             task=self.task,
             documents=result,
             n=self.n,
@@ -54,7 +59,11 @@
     @property
     def name(self) -> str:
         return "Context Search"
 
     @property
     def args(self) -> dict:
         return {"query": "string"}
+
+    @property
+    def resources(self) -> list[ActionResource]:
+        return self.action_resources
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/actions/deliberation.py` & `sherpa_ai-0.2.2/sherpa_ai/actions/deliberation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from langchain.base_language import BaseLanguageModel
 
 from sherpa_ai.actions.base import BaseAction
 
+
 DELIBERATION_DESCRIPTION = """Role Description: {role_description}
 Task Description: {task}
 
 Please deliberate on the task and generate a solution that is:
 
 Highly Detailed: Break down components and elements clearly.
 Quality-Oriented: Ensure top-notch performance and longevity.
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/actions/google_search.py` & `sherpa_ai-0.2.2/sherpa_ai/actions/google_search.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from langchain.base_language import BaseLanguageModel
 from loguru import logger
 
-from sherpa_ai.actions.base import BaseAction
+from sherpa_ai.actions.base import ActionResource, BaseAction
 from sherpa_ai.config.task_config import AgentConfig
 from sherpa_ai.tools import SearchTool
 
+
 # TODO check for prompt that keep orginal snetnences
 SEARCH_SUMMARY_DESCRIPTION = """Role Description: {role_description}
 Task: {task}
 
 Relevant Documents:
 {documents}
 
@@ -34,52 +35,37 @@
         self,
         role_description: str,
         task: str,
         llm: BaseLanguageModel,
         description: str = SEARCH_SUMMARY_DESCRIPTION,
         config: AgentConfig = AgentConfig(),
         n: int = 5,
-        include_metadata=False,
     ):
         self.role_description = role_description
         self.task = task
 
         self.description = description
         self.llm = llm
         self.n = n
 
         self.search_tool = SearchTool(config=config)
-        self.meta = []
-        self.include_metadata = include_metadata
+        self.action_resources = []
 
     def execute(self, query) -> str:
-        if self.include_metadata:
-            result, meta = self.search_tool._run(query, self.include_metadata)
-            self.meta.append(meta)
-        else:
-            result = self.search_tool._run(query)
-        logger.debug("Search Result: {}", result)
-
-        return result
+        result, resources = self.search_tool._run(query, return_resources=True)
+        self.add_resources(resources)
 
-        # the code block below is not currently used because the single google search result
-        # is short enough to fit into the context.
-        # Maybe get back to use the LLM to summarize the google search result again if the result beocme
-        # too long to handle in the context.
-
-        # prompt = self.description.format(
-        #     task=self.task,
-        #     documents=result,
-        #     n=self.n,
-        #     role_description=self.role_description,
-        # )
+        logger.debug("Search Result: {}", result)
 
-        # result = self.llm.predict(prompt)
         return result
 
     @property
     def name(self) -> str:
         return "Google Search"
 
     @property
     def args(self) -> dict:
         return {"query": "string"}
+
+    @property
+    def resources(self) -> list[ActionResource]:
+        return self.action_resources
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/actions/planning.py` & `sherpa_ai-0.2.2/sherpa_ai/actions/planning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import List, Optional
 
 from langchain.llms.base import LLM
 from loguru import logger
 
 from sherpa_ai.actions.base import BaseAction
 
+
 PLANNING_PROMPT = """You are a **task decomposition assistant** who simplifies complex tasks into sequential steps, assigning roles or agents to each.
 By analyzing user-defined tasks and agent capabilities, you provides structured plans, enhancing project clarity and efficiency.
 Your adaptability ensures customized solutions for diverse needs.
 
 A good plan is concise, detailed, feasible and efficient.
 
 Task: **{task}**
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/actions/synthesize.py` & `sherpa_ai-0.2.2/sherpa_ai/actions/synthesize.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from langchain.base_language import BaseLanguageModel
 from loguru import logger
 
 from sherpa_ai.actions.base import BaseAction
 
+
 SYNTHESIZE_DESCRIPTION = """{role_description}
 
 Context: {context}
 
 Action - Result History:
 {history}
 
@@ -48,15 +49,14 @@
             task=task,
             context=context,
             history=history,
             role_description=self.role_description,
         )
 
         logger.debug("Prompt: {}", prompt)
-
         result = self.llm.predict(prompt)
         return result
 
     @property
     def name(self) -> str:
         return "SynthesizeOutput"
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/agents/agent_pool.py` & `sherpa_ai-0.2.2/sherpa_ai/agents/agent_pool.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/agents/base.py` & `sherpa_ai-0.2.2/sherpa_ai/agents/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from sherpa_ai.action_planner import ActionPlanner
 from sherpa_ai.actions.base import BaseAction
 from sherpa_ai.events import EventType
 from sherpa_ai.output_parsers.base import BaseOutputProcessor
 from sherpa_ai.verbose_loggers.base import BaseVerboseLogger
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
+
 # Avoid circular import
 if TYPE_CHECKING:
     from sherpa_ai.memory import Belief, SharedMemory
 
 
 class BaseAgent(ABC):
     def __init__(
@@ -101,39 +102,58 @@
 
         logger.debug(f"```🤖{self.name} wrote: {result}```")
 
         self.shared_memory.add(EventType.result, self.name, result)
         return result
 
     def validate_output(self):
-        last_failed_validation = None
+        """
+        Validate the synthesized output through a series of validation steps.
 
-        for _ in range(self.validation_steps):
-            result = self.synthesize_output()
-            self.belief.update_internal(EventType.result, self.name, result)
-            is_valid = True
-            for validation in self.validations:
-                validation_result = validation.process_output(result, self.belief)
+        This method iterates through each validation in the 'validations' list, and for each validation,
+        it performs 'validation_steps' attempts to synthesize output using 'synthesize_output' method.
+        If the output doesn't pass validation, feedback is incorporated into the belief system.
+
+        If a validation fails after all attempts, the error messages from the last failed validation
+        are appended to the final result.
+
+        Returns:
+            str: The synthesized output after validation.
+        """
+        failed_validation = []
+        result = self.synthesize_output()
+        for validation in self.validations:
+            for count in range(self.validation_steps):
+                self.belief.update_internal(EventType.result, self.name, result)
+
+                validation_result = validation.process_output(
+                    text=result, belief=self.belief, iteration_count=count
+                )
 
-                if not validation_result.is_valid:
-                    is_valid = False
+                if validation_result.is_valid:
+                    result = validation_result.result
+                    break
+                else:
                     self.belief.update_internal(
                         EventType.feedback,
                         self.feedback_agent_name,
                         validation_result.feedback,
                     )
-                    last_failed_validation = validation
-                    break
-                result = validation_result.result
-            if is_valid:
-                return result
+                    result = self.synthesize_output()
 
-        if last_failed_validation is not None:
+            if count >= self.validation_steps:
+                failed_validation.append(validation)
+
+        if len(failed_validation) > 0:
             # if the validation failed after all steps, append the error messages to the result
-            result = result + "\n" + last_failed_validation.get_failure_message()
+            result += "\n".join(
+                failed_validation.get_failure_message()
+                for failed_validation in failed_validation
+            )
+
         self.belief.update_internal(EventType.result, self.name, result)
         return result
 
     def observe(self):
         return self.shared_memory.observe(self.belief)
 
     def act(self, action, inputs):
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/agents/critic.py` & `sherpa_ai-0.2.2/sherpa_ai/agents/critic.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from loguru import logger
 
 from sherpa_ai.agents.base import BaseAgent
 from sherpa_ai.events import EventType
 from sherpa_ai.memory import Belief, SharedMemory
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
+
 DESCRIPTION_PROMPT = """
 You are a Critic agent that receive a plan from the planner to execuate a task from user.
 Your goal is to output the {} most necessary feedback given the corrent plan to solve the task.
 """  # noqa: E501
 IMPORTANCE_PROMPT = """The plan you should be necessary and important to complete the task.
 Evaluate if the content of plan and selected actions/ tools are important and necessary.
 Output format:
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/agents/ml_engineer.py` & `sherpa_ai-0.2.2/sherpa_ai/agents/ml_engineer.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from sherpa_ai.actions import Deliberation, GoogleSearch, SynthesizeOutput
 from sherpa_ai.actions.arxiv_search import ArxivSearch
 from sherpa_ai.actions.base import BaseAction
 from sherpa_ai.agents.base import BaseAgent
 from sherpa_ai.memory import Belief, SharedMemory
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
+
 ACTION_PLAN_DESCRIPTION = "Given your specialized expertise, historical context, and your mission to facilitate Machine-Learning-based solutions, determine which action and its corresponding arguments would be the most scientifically sound and efficient approach to achieve the described task."  # noqa: E501
 
 
 ML_ENGINEER_DESCRIPTION = """You are a skilled machine learning engineer with a deep-rooted expertise in understanding and analyzing various Machine Learnng algorithm and use it to solve practical problems. \
 Your primary role is to assist individuals, organizations, and researchers in using machine learning models to solve Machine-Learning-Related chalenges, \
 using your knowledge to guide decisions and ensure the accuracy and reliability of outcomes.\
 If you encounter a question or challenge outside your current knowledge base, you acknowledge your limitations and seek assistance or additional resources to fill the gaps. \
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/agents/physicist.py` & `sherpa_ai-0.2.2/sherpa_ai/agents/physicist.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from sherpa_ai.action_planner import ActionPlanner
 from sherpa_ai.actions import Deliberation, GoogleSearch, SynthesizeOutput
 from sherpa_ai.actions.base import BaseAction
 from sherpa_ai.agents.base import BaseAgent
 from sherpa_ai.memory import Belief, SharedMemory
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
+
 PHYSICIST_DESCRIPTION = "You are a physicist with a deep-rooted expertise in understanding and analyzing the fundamental principles of the universe, spanning from the tiniest subatomic particles to vast cosmic phenomena. Your primary role is to assist individuals, organizations, and researchers in navigating and resolving complex physics-related challenges, using your knowledge to guide decisions and ensure the accuracy and reliability of outcomes."  # noqa: E501
 
 ACTION_PLAN_DESCRIPTION = "Given your specialized expertise, historical context, and your mission to facilitate physics-based solutions, determine which action and its corresponding arguments would be the most scientifically sound and efficient approach to achieve the described task."  # noqa: E501
 
 
 class Physicist(BaseAgent):
     """
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/agents/planner.py` & `sherpa_ai-0.2.2/sherpa_ai/agents/planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from sherpa_ai.actions.planning import TaskPlanning
 from sherpa_ai.agents.agent_pool import AgentPool
 from sherpa_ai.agents.base import BaseAgent
 from sherpa_ai.events import Event, EventType
 from sherpa_ai.memory import Belief, SharedMemory
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
+
 PLANNER_DESCRIPTION = """You are a **task decomposition assistant** who simplifies complex tasks into sequential steps, assigning roles or agents to each.
 By analyzing user-defined tasks and agent capabilities, you provide structured plans, enhancing project clarity and efficiency.
-Your adaptability ensures customized solutions for diverse needs. 
+Your adaptability ensures customized solutions for diverse needs.
 """  # noqa: E501
 
 
 class Planner(BaseAgent):
     def __init__(
         self,
         agent_pool: AgentPool,
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/agents/qa_agent.py` & `sherpa_ai-0.2.2/sherpa_ai/agents/qa_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from sherpa_ai.memory import Belief
 from sherpa_ai.memory.shared_memory import SharedMemory
 from sherpa_ai.output_parsers.base import BaseOutputProcessor
 from sherpa_ai.output_parsers.citation_validation import CitationValidation
 from sherpa_ai.verbose_loggers.base import BaseVerboseLogger
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
+
 # TODO: QA Agent only contains partial implementation from the original
 # task agent, more investigation is needed to add more content to it.
 # Some of the feature may be added to the agent base class, such as
 # the verbose logger.
 
 ACTION_PLAN_DESCRIPTION = "Given your specialized expertise, historical context, and your mission to facilitate Machine-Learning-based solutions, determine which action and its corresponding arguments would be the most scientifically sound and efficient approach to achieve the described task."  # noqa: E501
 
@@ -86,15 +87,14 @@
     def create_actions(self) -> List[BaseAction]:
         return [
             GoogleSearch(
                 self.description,
                 self.belief.current_task,
                 self.llm,
                 config=self.config,
-                include_metadata=self.citation_enabled,
             ),
         ]
 
     def synthesize_output(self) -> str:
         synthesize_action = SynthesizeOutput(
             self.description, self.llm, add_citation=self.citation_enabled
         )
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/agents/user.py` & `sherpa_ai-0.2.2/sherpa_ai/agents/user.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/config/task_config.py` & `sherpa_ai-0.2.2/sherpa_ai/config/task_config.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/connectors/chroma_vector_store.py` & `sherpa_ai-0.2.2/sherpa_ai/connectors/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/connectors/ChromaVectorStore.py` & `sherpa_ai-0.2.2/sherpa_ai/connectors/ChromaVectorStore.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,78 @@
+import uuid
+
 import chromadb
 from chromadb.utils import embedding_functions
-from langchain.text_splitter import CharacterTextSplitter
 from langchain.docstore.document import Document
-import uuid
+from langchain.text_splitter import CharacterTextSplitter
+
 import sherpa_ai.config as cfg
 
+
 class ChromaVectorStore:
     def __init__(self, db) -> None:
         self.db = db
-    
+
     @classmethod
-    def chroma_from_texts(cls, texts, embedding=None , meta_datas=None):
+    def chroma_from_texts(cls, texts, embedding=None, meta_datas=None):
         openai_ef = embedding_functions.OpenAIEmbeddingFunction(
-                    model_name="text-embedding-ada-002"
-                )
+            model_name="text-embedding-ada-002"
+        )
         embeded_data = openai_ef(texts)
         meta_datas = [] if meta_datas is None else meta_datas
-        client =chromadb.PersistentClient(path="./db")
-        db = client.get_or_create_collection(name=cfg.INDEX_NAME_FILE_STORAGE,embedding_function=openai_ef)
+        client = chromadb.PersistentClient(path="./db")
+        db = client.get_or_create_collection(
+            name=cfg.INDEX_NAME_FILE_STORAGE, embedding_function=openai_ef
+        )
         db.add(
-            embeddings = embeded_data,
-            documents = texts,
-            metadatas = meta_datas,
-            ids = [str(uuid.uuid1()) for text in texts]
-        )
-      
-        return cls(db) 
-    
+            embeddings=embeded_data,
+            documents=texts,
+            metadatas=meta_datas,
+            ids=[str(uuid.uuid1()) for text in texts],
+        )
+
+        return cls(db)
+
     @classmethod
     def chroma_from_existing(cls):
         openai_ef = embedding_functions.OpenAIEmbeddingFunction(
-                    model_name="text-embedding-ada-002"
-                )
-                
-        client =chromadb.PersistentClient(path="./db")
-        db = client.get_or_create_collection(name=cfg.INDEX_NAME_FILE_STORAGE,embedding_function=openai_ef)
-       
-        return cls(db) 
+            model_name="text-embedding-ada-002"
+        )
+
+        client = chromadb.PersistentClient(path="./db")
+        db = client.get_or_create_collection(
+            name=cfg.INDEX_NAME_FILE_STORAGE, embedding_function=openai_ef
+        )
+
+        return cls(db)
 
     @classmethod
-    def file_text_splitter(cls,data , meta_data):
+    def file_text_splitter(cls, data, meta_data):
         text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
         texts = text_splitter.split_text(data)
         metadatas = []
         temp_texts = []
         for doc in texts:
             metadatas.append(meta_data)
             temp_texts.append(f"""'file_content': '{doc}' ,{meta_data}""")
         texts = temp_texts
 
-        return {'texts':texts ,'meta_datas':metadatas}
-
+        return {"texts": texts, "meta_datas": metadatas}
 
-    def similarity_search(self, query: str="", session_id: str = None):
+    def similarity_search(self, query: str = "", session_id: str = None):
         filter = {} if session_id is None else {"session_id": session_id}
         results = self.db.query(
             query_texts=[query],
             n_results=2,
             where=filter,
-            include=['documents','metadatas'],
-            )
+            include=["documents", "metadatas"],
+        )
         documents = []
         if results is not None:
-            for i in range(0,len(results['documents'][0])):
-                documents.append(Document(metadata=results['metadatas'][0][i],page_content=results['documents'][0][i]))
+            for i in range(0, len(results["documents"][0])):
+                documents.append(
+                    Document(
+                        metadata=results["metadatas"][0][i],
+                        page_content=results["documents"][0][i],
+                    )
+                )
         return documents
-
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/connectors/scripts/load_dump_to_chroma.py` & `sherpa_ai-0.2.2/sherpa_ai/connectors/scripts/load_dump_to_chroma.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/connectors/scripts/query_chroma.py` & `sherpa_ai-0.2.2/sherpa_ai/connectors/scripts/query_chroma.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/connectors/vectorstores.py` & `sherpa_ai-0.2.2/sherpa_ai/connectors/vectorstores.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/database/user_usage_tracker.py` & `sherpa_ai-0.2.2/sherpa_ai/database/user_usage_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import time
 
 import boto3
+import sqlalchemy.orm
 from anyio import Path
 from sqlalchemy import TIMESTAMP, Boolean, Column, Integer, String, create_engine
-from sqlalchemy.orm import sessionmaker
-from sqlalchemy import Boolean, Column, Integer, String, create_engine
 from sqlalchemy.orm import declarative_base, sessionmaker
 
 import sherpa_ai.config as cfg
 from sherpa_ai.verbose_loggers.base import BaseVerboseLogger
 from sherpa_ai.verbose_loggers.verbose_loggers import DummyVerboseLogger
 
-import boto3
-import sqlalchemy.orm
+
 Base = sqlalchemy.orm.declarative_base()
 
 
 class UsageTracker(Base):
     """SQLAlchemy base model for tracking LLM token usage on per-user basis"""
 
     __tablename__ = "usage_tracker"
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/error_handling/agent_error_handler.py` & `sherpa_ai-0.2.2/sherpa_ai/error_handling/agent_error_handler.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/events.py` & `sherpa_ai-0.2.2/sherpa_ai/events.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/memory/belief.py` & `sherpa_ai-0.2.2/sherpa_ai/memory/belief.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/memory/shared_memory.py` & `sherpa_ai-0.2.2/sherpa_ai/memory/shared_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import TYPE_CHECKING, List, Optional
 
 from sherpa_ai.actions.planning import Plan
 from sherpa_ai.events import Event, EventType
 from sherpa_ai.memory.belief import Belief
 
+
 if TYPE_CHECKING:
     from sherpa_ai.agents import AgentPool
 
 
 class SharedMemory:
     def __init__(self, objective: str, agent_pool: AgentPool = None):
         self.objective = objective
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/memory/shared_memory_with_vectordb.py` & `sherpa_ai-0.2.2/sherpa_ai/memory/shared_memory_with_vectordb.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/models/chat_model_with_logging.py` & `sherpa_ai-0.2.2/sherpa_ai/models/chat_model_with_logging.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/models/sherpa_base_chat_model.py` & `sherpa_ai-0.2.2/sherpa_ai/models/sherpa_base_chat_model.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/models/sherpa_base_model.py` & `sherpa_ai-0.2.2/sherpa_ai/models/sherpa_base_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain.chat_models import ChatOpenAI
 from langchain.chat_models.base import BaseChatModel
 from langchain.schema import BaseMessage, ChatResult
+from pydantic import BaseModel
 
 from sherpa_ai.database.user_usage_tracker import UserUsageTracker
 
 
 class SherpaOpenAI(ChatOpenAI):
     team_id: typing.Optional[str] = None
     user_id: typing.Optional[str] = None
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/orchestrator.py` & `sherpa_ai-0.2.2/sherpa_ai/orchestrator.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/output_parser.py` & `sherpa_ai-0.2.2/sherpa_ai/output_parser.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/output_parsers/base.py` & `sherpa_ai-0.2.2/sherpa_ai/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/output_parsers/citation_validation.py` & `sherpa_ai-0.2.2/sherpa_ai/output_parsers/citation_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import nltk
+from loguru import logger
 from nltk.tokenize import sent_tokenize, word_tokenize
 
+from sherpa_ai.actions.base import ActionResource
 from sherpa_ai.memory import Belief
 from sherpa_ai.output_parsers.base import BaseOutputProcessor
 from sherpa_ai.output_parsers.validation_result import ValidationResult
 
+
 # download the punkt tokenizer. This is necessary for the sent_tokenize in NLTK.
 # The download will only happen once and the result will be cached.
 nltk.download("punkt")
 
 
 class CitationValidation(BaseOutputProcessor):
     """
@@ -147,45 +150,41 @@
 
         Returns:
             list[str]: A list of sentences extracted from the input paragraph.
         """
         sentences = sent_tokenize(paragraph)
         return sentences
 
-    def resources_from_belief(self, belief: Belief) -> list[dict]:
+    def resources_from_belief(self, belief: Belief) -> list[ActionResource]:
         """
         Returns a list of all resources within belief.actions.
         """
         resources = []
         for action in belief.actions:
-            if hasattr(action, "meta") and action.meta is not None and len(action.meta) > 0:
-                resources.extend(action.meta[-1])
+            resources.extend(action.resources)
         return resources
 
-    def process_output(self, text: str, belief: Belief) -> ValidationResult:
+    def process_output(self, text: str, belief: Belief, **kwargs) -> ValidationResult:
         """
          Add citations to sentences in the generated text using resources based on fact checking model.
 
          Args:
              text (str): The text which needs citations/references added
              belief (Belief): Belief of the agent that generated `text`
 
          Returns:
              ValidationResult: The result of citation processing.
              `is_valid` is True when citation processing succeeds or no citation resources are provided,
              False otherwise.
              `result` contains the formatted text with citations.
              `feedback` providing additional optional information.
 
-         Note:
-             The 'resources' list should contain dictionaries with "Document" and "Source" keys.
-
         Typical usage example:
          ```python
-         resources = [{"Document": "Some reference text.", "Source": "http://example.com/source1"}]
+         resources = ActionResource(source="http://example.com/source1", content="Some reference text.")]
          citation_parser = CitationValidation()
          result = citation_parser.parse_output("Text needing citations.", resources)
          ```
         """
         resources = self.resources_from_belief(belief)
 
         if len(resources) == 0:
@@ -194,15 +193,15 @@
                 is_valid=True,
                 result=text,
                 feedback="",
             )
 
         return self.add_citations(text, resources)
 
-    def add_citation_to_sentence(self, sentence: str, resources: list[dict]):
+    def add_citation_to_sentence(self, sentence: str, resources: list[ActionResource]):
         """
         Uses a list of resources to add citations to a sentence
 
         Returns:
             citation_ids: a list of citation identifiers
             citation_links: a list of citation links (URLs)
         """
@@ -210,16 +209,16 @@
         citation_links = []
 
         if len(sentence) <= 5:
             return citation_ids, citation_links
 
         for index, resource in enumerate(resources):
             cited = False
-            resource_link = resource["Source"]
-            resource_text = resource["Document"]
+            resource_link = resource.source
+            resource_text = resource.content
             resource_sentences = resource_text.split(".")
             # TODO: verify that splitting each sentence on newlines improves citation results
             nested_sentence_lines = [s.split("\n") for s in resource_sentences]
             resource_lines = self.flatten_nested_list(nested_sentence_lines)
 
             for resource_line in resource_lines:
                 if not cited and not (resource_link in citation_links):
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/output_parsers/link_parse.py` & `sherpa_ai-0.2.2/sherpa_ai/output_parsers/link_parse.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/output_parsers/md_to_slack_parse.py` & `sherpa_ai-0.2.2/sherpa_ai/output_parsers/md_to_slack_parse.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/output_parsers/number_validation.py` & `sherpa_ai-0.2.2/sherpa_ai/output_parsers/number_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ```python
     number_validator = NumberValidation(source="document")
     result = number_validator.process_output("The document contains important numbers: 123, 456.")
     ```
 
     """
 
-    def process_output(self, text: str, belief: Belief) -> ValidationResult:
+    def process_output(self, text: str, belief: Belief, **kwargs) -> ValidationResult:
         """
         Verifies that all numbers within `text` exist in the `belief` source text.
 
         Args:
             text: The text to be analyzed
             belief: Belief of the Agent that generated `text`
         Returns:
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/output_parsers/validation_result.py` & `sherpa_ai-0.2.2/sherpa_ai/output_parsers/validation_result.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/prompt.py` & `sherpa_ai-0.2.2/sherpa_ai/prompt.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/prompt_generator.py` & `sherpa_ai-0.2.2/sherpa_ai/prompt_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from typing import List
 
 from langchain.tools.base import BaseTool
 
+
 FINISH_NAME = "finish"
 
 
 class PromptGenerator:
     """A class for generating custom prompt strings.
 
     Does this based on constraints, commands, resources, and performance evaluations.
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/reflection.py` & `sherpa_ai-0.2.2/sherpa_ai/reflection.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/scrape/extract_github_readme.py` & `sherpa_ai-0.2.2/sherpa_ai/scrape/extract_github_readme.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from langchain.embeddings.openai import OpenAIEmbeddings
 from loguru import logger
 
 import sherpa_ai.config as cfg
 from sherpa_ai.connectors.vectorstores import ConversationStore
 
 
+GITHUB_REQUEST_TIMEOUT = 2.5
+
+
 def get_owner_and_repo(url):
     """
     Extracts the owner and repository name from a GitHub repository URL.
 
     Parameters:
     - url (str): The GitHub repository URL.
 
@@ -45,15 +48,17 @@
         token = cfg.GITHUB_AUTH_TOKEN
         github_api_url = f"https://api.github.com/repos/{owner}/{repo}/contents"
         headers = {
             "Authorization": f"token {token}",
             "X-GitHub-Api-Version": "2022-11-28",
         }
 
-        response = requests.get(github_api_url, headers=headers)
+        response = requests.get(
+            github_api_url, headers=headers, timeout=GITHUB_REQUEST_TIMEOUT
+        )
 
         files = response.json()
         if type(files) is dict and files["message"].lower() == "bad credentials":
             return None
         matching_files = [
             file["name"]
             for file in files
@@ -68,15 +73,17 @@
         path = matching_files[0]
         github_api_url = f"https://api.github.com/repos/{owner}/{repo}/contents/{path}"
         headers = {
             "Authorization": f"token {token}",
             "X-GitHub-Api-Version": "2022-11-28",
         }
 
-        response = requests.get(github_api_url, headers=headers)
+        response = requests.get(
+            github_api_url, headers=headers, timeout=GITHUB_REQUEST_TIMEOUT
+        )
         data = response.json()
         if "content" in data:
             content = base64.b64decode(data["content"]).decode("utf-8")
             metadata = [{"type": "github", "url": repo_url}]
             save_to_pine_cone(content, metadata)
             return content
         else:
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/scrape/file_scraper.py` & `sherpa_ai-0.2.2/sherpa_ai/scrape/file_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     chunk_and_summarize_file,
     count_string_tokens,
     extract_text_from_pdf,
     question_with_file_reconstructor,
 )
 
 
+DOWNLOAD_TIMEOUT = 2.5
+
+
 class QuestionWithFileHandler:
     def __init__(self, question, files, token, user_id, team_id):
         """
         Initializes the QuestionWithFileHandler instance.
 
         currently works for one file only.
 
@@ -62,15 +65,17 @@
         Returns:
             dict: A dictionary with status and downloaded file content.
         """
         headers = {
             "Authorization": f"Bearer {self.token}",
             "Accept": file["mimetype"],
         }
-        response = requests.get(file["url_private_download"], headers=headers)
+        response = requests.get(
+            file["url_private_download"], headers=headers, timeout=DOWNLOAD_TIMEOUT
+        )
         destination = file["id"] + file["filetype"]
 
         # Check if the request was successful (HTTP status code 200)
         if response.status_code == 200:
             content_data = ""
             if file["filetype"] == "pdf":
                 # Open the local file and write the content of the downloaded file
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/scrape/prompt_reconstructor.py` & `sherpa_ai-0.2.2/sherpa_ai/scrape/prompt_reconstructor.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/task_agent.py` & `sherpa_ai-0.2.2/sherpa_ai/task_agent.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/test_utils/llms.py` & `sherpa_ai-0.2.2/sherpa_ai/test_utils/llms.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/test_utils/loggers.py` & `sherpa_ai-0.2.2/sherpa_ai/test_utils/loggers.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/sherpa_ai/tools.py` & `sherpa_ai-0.2.2/sherpa_ai/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-import os
 import re
-import urllib
 import urllib.parse
-import urllib.request
 from typing import Any, List, Tuple, Union
-from urllib.parse import urlparse
 
 import requests
-from bs4 import BeautifulSoup
-from langchain.chains import LLMChain
-from langchain.prompts import Prompt
 from langchain.tools import BaseTool
 from langchain.utilities import GoogleSerperAPIWrapper
 from langchain.vectorstores.base import VectorStoreRetriever
 from loguru import logger
 from typing_extensions import Literal
 
 import sherpa_ai.config as cfg
 from sherpa_ai.config.task_config import AgentConfig
-from sherpa_ai.output_parser import TaskAction
+
+
+HTTP_GET_TIMEOUT = 2.5
 
 
 def get_tools(memory, config):
     tools = []
 
     # tools.append(ContextTool(memory=memory))
     tools.append(UserInputTool())
@@ -41,42 +36,60 @@
 class SearchArxivTool(BaseTool):
     name = "Arxiv Search"
     description = (
         "Access all the papers from Arxiv to search for domain-specific scientific publication."  # noqa: E501
         "Only use this tool when you need information in the scientific paper."
     )
 
-    def _run(self, query: str) -> str:
+    def _run(
+        self, query: str, return_resources=False
+    ) -> Union[str, Tuple[str, List[dict]]]:
         top_k = 10
 
         logger.debug(f"Search query: {query}")
         query = urllib.parse.quote_plus(query)
         url = (
             "http://export.arxiv.org/api/query?search_query=all:"
             + query.strip()
             + "&start=0&max_results="
             + str(top_k)
         )
-        data = urllib.request.urlopen(url)
-        xml_content = data.read().decode("utf-8")
+        data = requests.get(url, timeout=HTTP_GET_TIMEOUT)
+        xml_content = data.text
 
         summary_pattern = r"<summary>(.*?)</summary>"
         summaries = re.findall(summary_pattern, xml_content, re.DOTALL)
         title_pattern = r"<title>(.*?)</title>"
         titles = re.findall(title_pattern, xml_content, re.DOTALL)
+        id_pattern = r"<id>(.*?)</id>"
+        ids = re.findall(id_pattern, xml_content, re.DOTALL)
 
         result_list = []
         for i in range(len(titles)):
             result_list.append(
-                "Title: " + titles[i] + "\n" + "Summary: " + summaries[i]
+                "Title: " + titles[i] + "\n" + "Summary: " + summaries[i] + "\n"
+            )
+        result = "\n".join(result_list)
+
+        # add resources for citation
+        resources = []
+        for i in range(len(titles)):
+            resources.append(
+                {
+                    "Document": "Title: " + titles[i] + "\nSummary: " + summaries[i],
+                    "Source": ids[i],
+                }
             )
 
         logger.debug(f"Arxiv Search Result: {result_list}")
 
-        return " ".join(result_list)
+        if return_resources:
+            return result, resources
+        else:
+            return result
 
     def _arun(self, query: str) -> str:
         raise NotImplementedError("SearchArxivTool does not support async run")
 
 
 class SearchTool(BaseTool):
     name = "Search"
@@ -84,20 +97,21 @@
     top_k: int = 10
     description = (
         "Access the internet to search for the information. Only use this tool when "
         "you cannot find the information using internal search."
     )
 
     def _run(
-        self, query: str, require_meta=False
+        self, query: str, return_resources=False
     ) -> Union[str, Tuple[str, List[dict]]]:
         result = ""
         if self.config.search_domains:
             query_list = [
-                self.formulate_site_search(query, str(i)) for i in self.config.search_domains
+                self.formulate_site_search(query, str(i))
+                for i in self.config.search_domains
             ]
             if len(query_list) >= 5:
                 query_list = query_list[:5]
                 result = (
                     result
                     + "Warning: Only the first 5 URLs are taken into consideration.\n"
                 )  # noqa: E501
@@ -107,36 +121,36 @@
             invalid_domain_string = ", ".join(self.config.invalid_domains)
             result = (
                 result
                 + f"Warning: The doman {invalid_domain_string} is invalid and is not taken into consideration.\n"  # noqa: E501
             )  # noqa: E501
 
         top_k = int(self.top_k / len(query_list))
-        if require_meta:
-            meta = []
+        if return_resources:
+            resources = []
 
         for query in query_list:
-            cur_result = self._run_single_query(query, top_k, require_meta)
+            cur_result = self._run_single_query(query, top_k, return_resources)
 
-            if require_meta:
+            if return_resources:
                 result += "\n" + cur_result[0]
-                meta.extend(cur_result[1])
+                resources.extend(cur_result[1])
             else:
                 result += "\n" + cur_result
 
-        if require_meta:
-            result = (result, meta)
+        if return_resources:
+            result = (result, resources)
 
         return result
-    
+
     def formulate_site_search(self, query: str, site: str) -> str:
         return query + " site:" + site
 
     def _run_single_query(
-        self, query: str, top_k: int, require_meta=False
+        self, query: str, top_k: int, return_resources=False
     ) -> Union[str, Tuple[str, List[dict]]]:
         logger.debug(f"Search query: {query}")
         google_serper = GoogleSerperAPIWrapper()
         search_results = google_serper._google_serper_api_results(query)
         logger.debug(f"Google Search Result: {search_results}")
 
         # case 1: answerBox in the result dictionary
@@ -149,15 +163,15 @@
             elif answer_box.get("snippetHighlighted"):
                 answer = answer_box.get("snippetHighlighted")
             title = search_results["organic"][0]["title"]
             link = search_results["organic"][0]["link"]
 
             response = "Answer: " + answer
             meta = [{"Document": answer, "Source": link}]
-            if require_meta:
+            if return_resources:
                 return response, meta
             else:
                 return response + "\nLink:" + link
 
         # case 2: knowledgeGraph in the result dictionary
         snippets = []
         if search_results.get("knowledgeGraph", False):
@@ -188,26 +202,26 @@
                 snippets.append(f"{attribute}: {value}.")
 
             if len(snippets) == 0:
                 return ["No good Google Search Result was found"]
 
         result = []
 
-        meta = []
+        resources = []
         for i in range(len(search_results["organic"][:top_k])):
             r = search_results["organic"][i]
             single_result = r["title"] + r["snippet"]
 
             # If the links are not considered explicitly, add it to the search result
             # so that it can be considered by the LLM
-            if not require_meta:
+            if not return_resources:
                 single_result += "\nLink:" + r["link"]
 
             result.append(single_result)
-            meta.append(
+            resources.append(
                 {
                     "Document": "Description: " + r["title"] + r["snippet"],
                     "Source": r["link"],
                 }
             )
         full_result = "\n".join(result)
 
@@ -221,16 +235,16 @@
                 "Description: "
                 + search_results["knowledgeGraph"]["title"]
                 + search_results["knowledgeGraph"]["description"]
                 + "\nLink:"
                 + search_results["knowledgeGraph"]["descriptionLink"]
             )
             full_result = answer + "\n\n" + full_result
-        if require_meta:
-            return full_result, meta
+        if return_resources:
+            return full_result, resources
         else:
             return full_result
 
     def _arun(self, query: str) -> str:
         raise NotImplementedError("SearchTool does not support async run")
 
 
@@ -239,36 +253,38 @@
     description = (
         "Access internal technical documentation for AI related projects, including"
         + "Fixie, LangChain, GPT index, GPTCache, GPT4ALL, autoGPT, db-GPT, AgentGPT, sherpa."  # noqa: E501
         + "Only use this tool if you need information for these projects specifically."
     )
     memory: VectorStoreRetriever
 
-    def _run(self, query: str, need_meta=False) -> str:
+    def _run(
+        self, query: str, return_resources=False
+    ) -> Union[str, Tuple[str, List[dict]]]:
         docs = self.memory.get_relevant_documents(query)
         result = ""
-        metadata = []
+        resources = []
         for doc in docs:
             result += (
                 "Document"
                 + doc.page_content
                 + "\nLink:"
                 + doc.metadata.get("source", "")
                 + "\n"
             )
-            if need_meta:
-                metadata.append(
+            if return_resources:
+                resources.append(
                     {
                         "Document": doc.page_content,
                         "Source": doc.metadata.get("source", ""),
                     }
                 )
 
-        if need_meta:
-            return result, metadata
+        if return_resources:
+            return result, resources
         else:
             return result
 
     def _arun(self, query: str) -> str:
         raise NotImplementedError("ContextTool does not support async run")
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/utils.py` & `sherpa_ai-0.2.2/sherpa_ai/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+import json
 import re
 from typing import List, Optional, Union
 from urllib.parse import urlparse
 
 import requests
 import spacy
 import tiktoken
 from bs4 import BeautifulSoup
 from langchain.docstore.document import Document
 from langchain.document_loaders import UnstructuredMarkdownLoader, UnstructuredPDFLoader
 from langchain.llms import OpenAI
 from langchain.text_splitter import TokenTextSplitter
 from loguru import logger
+from nltk.metrics import edit_distance, jaccard_distance
 from pypdf import PdfReader
 from word2number import w2n
 
 import sherpa_ai.config as cfg
+from sherpa_ai.database.user_usage_tracker import UserUsageTracker
 from sherpa_ai.models.sherpa_base_model import SherpaOpenAI
 
 
+HTTP_GET_TIMEOUT = 2.5
+
+
 def load_files(files: List[str]) -> List[Document]:
     documents = []
     loader = None
     for f in files:
         (f"Loading file {f}")
         if f.endswith(".pdf"):
             loader = UnstructuredPDFLoader(f)
@@ -74,15 +80,15 @@
                                 links.append(
                                     {"url": newUrl, "base_url": get_base_url(newUrl)}
                                 )
     return links
 
 
 def scrape_with_url(url: str):
-    response = requests.get(url)
+    response = requests.get(url, timeout=HTTP_GET_TIMEOUT)
     soup = BeautifulSoup(response.content, "html.parser")
     data = soup.get_text(strip=True)
     status = response.status_code
     if response.status_code == 200:
         return {"data": data, "status": status}
     else:
         return {"data": "", "status": status}
@@ -278,33 +284,29 @@
     # Extract URLs using urllib.parse
     urls = [word for word in words if urlparse(word).scheme in ["http", "https"]]
 
     return urls
 
 
 def check_url(url):
-    # check whether a url is valid
-    # return True is url is valid
-
-    try:
-        html = urlopen(url)
+    """
+    Performs an HTTP GET request on `url` to test its validity.
 
-    # except block to catch
-    # exception
-    # and identify error
-    except HTTPError as e:
-        print("HTTP error", e)
-        return False
-
-    except URLError as e:
-        print("Opps ! Page not found!", e)
-        return False
+    Returns True if GET succeeds, False otherwise.
+    """
 
+    if urlparse(url).scheme in ["http", "https"]:
+        try:
+            _ = requests.get(url, timeout=HTTP_GET_TIMEOUT)
+            return True
+        except Exception as e:
+            logger.info(f"{e} - {url}")
+            return False
     else:
-        return True
+        raise ValueError(f"URL must conform to HTTP(S) scheme: {url}")
 
 
 def extract_numbers_from_text(text):
     """Returns a list, possibly empty, of the strings of digits within text"""
     if text is not None:
         text = text.lower()
         text_without_commas = re.sub(",", "", text)
@@ -405,7 +407,234 @@
     incorrect_candidates = candidate_numbers - source_numbers
 
     if len(incorrect_candidates) > 0:
         joined_numbers = ", ".join(incorrect_candidates)
         message = f"Don't use the numbers {joined_numbers} to answer the question. Instead, stick to the numbers mentioned in the context."
         return False, message
     return True, None
+
+
+def check_if_number_exist(result: str, source: str):
+    check_numbers = extract_numbers_from_text(result)
+    source_numbers = extract_numbers_from_text(source)
+    error_numbers = []
+    message = ""
+    for data in check_numbers:
+        if data not in source_numbers:
+            error_numbers.append(data)
+    error_numbers = set(error_numbers)
+    if len(error_numbers) > 0:
+        for numbers in error_numbers:
+            message += numbers + ", "
+        message = f"Don't use the numbers {message} to answer the question instead stick to the numbers mentioned in the context."
+        return {"number_exists": False, "messages": message}
+    return {"number_exists": True, "messages": message}
+
+
+def string_comparison_with_jaccard_and_levenshtein(word1, word2, levenshtein_constant):
+    """
+    Calculate a combined similarity metric using Jaccard similarity and normalized Levenshtein distance.
+
+    Args:
+    - word1 (str): First input string.
+    - word2 (str): Second input string.
+    - levenshtein_constant (float): Weight for the Levenshtein distance in the combined metric.
+
+    Returns:
+    float: Combined similarity metric.
+    """
+
+    word1_set = set(word1)
+    word2_set = set(word2)
+
+    lev_distance = edit_distance(word1, word2)
+    jaccard_sim = 1 - jaccard_distance(word1_set, word2_set)
+    long_len = max(len(word1), len(word2))
+    # This will give a value between 0 and 1, where 0 represents identical words and 1 represents completely different words.
+    normalized_levenshtein = 1 - (lev_distance / long_len)
+    # The weight is determined by the levenshtein_constant variable,
+    # which should be a value between 0 and 1.
+    # A higher weight gives more importance to the Levenshtein distance,
+    # while a lower weight gives more importance to the Jaccard similarity.
+    combined_metric = (levenshtein_constant * normalized_levenshtein) + (
+        (1 - levenshtein_constant) * jaccard_sim
+    )
+
+    return combined_metric
+
+
+def extract_entities(text):
+    """
+    Extract entities of specific types
+        NORP (Nationalities or Religious or Political Groups),
+        ORG (Organization),
+        GPE (Geopolitical Entity),
+        LOC (Location) using spaCy.
+    Args:
+    - text (str): Input text.
+
+    Returns:
+    List[str]: List of extracted entities.
+    """
+
+    nlp = spacy.load("en_core_web_sm")
+    doc = nlp(text)
+    entity_types = ["NORP", "ORG", "GPE", "LOC"]
+    filtered_entities = [ent.text for ent in doc.ents if ent.label_ in entity_types]
+
+    return filtered_entities
+
+
+def json_from_text(text: str):
+    """
+    Extract and parse JSON data from a text.
+
+    Args:
+    - text (str): Input text containing JSON data.
+
+    Returns:
+    dict: Parsed JSON data.
+    """
+    if isinstance(text, str):
+        text = text.replace("\n", "")
+        json_pattern = r"\{.*\}"
+        json_match = re.search(json_pattern, text)
+
+        if json_match:
+            json_data = json_match.group()
+            try:
+                parsed_json = json.loads(json_data)
+                return parsed_json
+            except json.JSONDecodeError:
+                return {}
+        else:
+            return {}
+    else:
+        return {}
+
+
+def text_similarity_by_llm(
+    source_entity: List[str],
+    source,
+    result,
+    user_id=None,
+    team_id=None,
+):
+    """
+    Check if entities from a question are mentioned in some form inside the answer using a language model.
+
+    Args:
+    - source_entity (List[str]): List of entities from the question.
+    - source (str): Question text.
+    - result (str): Answer text.
+    - user_id (str): User ID (optional).
+    - team_id (str): Team ID (optional).
+
+    Returns:
+    dict: Result of the check containing 'entity_exist' and 'messages'.
+    """
+
+    llm = SherpaOpenAI(
+        temperature=cfg.TEMPERATURE,
+        openai_api_key=cfg.OPENAI_API_KEY,
+        user_id=user_id,
+        team_id=team_id,
+    )
+
+    instruction = f"""
+        I have a question and an answer. I want you to confirm whether the entities from the question are all mentioned in some form within the answer.
+
+        Question = {source}
+        Entities inside the question = {source_entity}
+
+        Answer = {result}
+       """
+    prompt = (
+        instruction
+        + """
+           only return {"entity_exist": true , "messages":"" } if all entities are mentioned inside the answer in
+           only return {"entity_exist": false , "messages": " Entity x hasn't been mentioned inside the answer"} if the entity is not mentioned properly .
+          """
+    )
+
+    llm_result = llm.predict(prompt)
+    checkup_json = json_from_text(llm_result)
+
+    return checkup_json.get("entity_exist", False), checkup_json.get("messages", "")
+
+
+def text_similarity_by_metrics(check_entity: List[str], source_entity: List[str]):
+    """
+    Check entity similarity based on Jaccard and Levenshtein metrics.
+
+    Args:
+    - check_entity (List[str]): List of entities to check.
+    - source_entity (List[str]): List of reference entities.
+
+    Returns:
+    dict: Result of the check containing 'entity_exist' and 'messages'.
+    """
+
+    check_entity_lower = [s.lower() for s in check_entity]
+    source_entity_lower = [s.lower() for s in source_entity]
+
+    threshold = 0.75
+    error_entity = []
+    message = ""
+    levenshtein_constant = 0.5
+
+    # for each entity in the source entity list, check if it is similar to any entity in the check entity list
+    # if similarity is below the threshold, add the entity to the error_entity list
+    # else return True means all entities are similar
+    for source_entity_val in source_entity_lower:
+        metrics_value = 0
+        for check_entity_val in check_entity_lower:
+            word1 = source_entity_val
+            word2 = check_entity_val
+
+            # Calculate the combined similarity metric using Jaccard similarity and normalized Levenshtein distance
+            combined_similarity = string_comparison_with_jaccard_and_levenshtein(
+                word1=word1, word2=word2, levenshtein_constant=levenshtein_constant
+            )
+
+            if metrics_value < combined_similarity:
+                metrics_value = combined_similarity
+        if metrics_value < threshold:
+            # If the metrics value is below the threshold, add the entity to the error_entity list
+            index_of_entity = source_entity_lower.index(source_entity_val)
+            error_entity.append(source_entity[index_of_entity])
+
+    if len(error_entity) > 0:
+        # If there are error entities, create a message to address them in the final answer
+        for entity in error_entity:
+            message += entity + ", "
+        message = f"Remember to address these entities {message} in the final answer."
+        return False, message
+    return True, message
+
+
+def text_similarity(check_entity: List[str], source_entity: List[str]):
+    """
+    Check if entities from a reference list are present in another list.
+
+    Args:
+    - check_entity ([str]): List of entities to check.
+    - source_entity ([str]): List of reference entities.
+
+    Returns:
+    dict: Result of the check containing 'entity_exist' and 'messages'.
+    """
+
+    error_entity = []
+    message = ""
+    check_entity_lower = [s.lower() for s in check_entity]
+    source_entity_lower = [s.lower() for s in source_entity]
+    for entity in source_entity_lower:
+        if entity not in check_entity_lower:
+            index_of_entity = source_entity_lower.index(entity)
+            error_entity.append(source_entity[index_of_entity])
+    if len(error_entity) > 0:
+        for entity in error_entity:
+            message += entity + ", "
+        message = f"remember to address these entities {message} in final the answer."
+        return False, message
+    return True, message
```

### Comparing `sherpa_ai-0.2.1/sherpa_ai/verbose_loggers/verbose_loggers.py` & `sherpa_ai-0.2.2/sherpa_ai/verbose_loggers/verbose_loggers.py`

 * *Files identical despite different names*

### Comparing `sherpa_ai-0.2.1/PKG-INFO` & `sherpa_ai-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-ai
-Version: 0.2.1
+Version: 0.2.2
 Summary: Sherpa: AI-augmented thinking companion
 Home-page: https://github.com/Aggregate-Intellect/sherpa
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,15 +18,15 @@
 Requires-Dist: markdown (>=3.4.4,<3.5.0)
 Requires-Dist: openai (>=0.28.0,<0.29.0)
 Requires-Dist: pinecone-client (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pypdf (>=3.17.0,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: spacy (>=3.7.4,<4.0.0)
-Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: tiktoken (>=0.6.0,<1.0)
 Requires-Dist: transformers (>=4.35.2,<5.0.0)
 Requires-Dist: unstructured (>=0.10.11,<0.11.0)
 Requires-Dist: word2number (>=1.1,<2.0)
 Project-URL: Repository, https://github.com/Aggregate-Intellect/sherpa
 Description-Content-Type: text/markdown
 
 **To see the documentation, visit: https://sherpa-ai.readthedocs.io/**
```


# Comparing `tmp/gpt-researcher-0.3.2.tar.gz` & `tmp/gpt-researcher-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.3.2.tar", last modified: Thu May  9 06:41:49 2024, max compression
+gzip compressed data, was "gpt-researcher-0.3.3.tar", last modified: Thu May  9 06:47:07 2024, max compression
```

## Comparing `gpt-researcher-0.3.2.tar` & `gpt-researcher-0.3.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.255187 gpt-researcher-0.3.2/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 06:41:49.254464 gpt-researcher-0.3.2/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    10003 2024-05-08 07:24:47.000000 gpt-researcher-0.3.2/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.205497 gpt-researcher-0.3.2/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.206109 gpt-researcher-0.3.2/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.207373 gpt-researcher-0.3.2/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.208505 gpt-researcher-0.3.2/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.3.2/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.3.2/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.209149 gpt-researcher-0.3.2/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.3.2/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.213432 gpt-researcher-0.3.2/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.3.2/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.215603 gpt-researcher-0.3.2/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.3.2/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.3.2/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.216574 gpt-researcher-0.3.2/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.218408 gpt-researcher-0.3.2/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.220152 gpt-researcher-0.3.2/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.221785 gpt-researcher-0.3.2/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.3.2/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.225763 gpt-researcher-0.3.2/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.3.2/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     8928 2024-05-05 07:01:28.000000 gpt-researcher-0.3.2/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.3.2/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.3.2/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.227656 gpt-researcher-0.3.2/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.3.2/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.3.2/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.228465 gpt-researcher-0.3.2/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.229917 gpt-researcher-0.3.2/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.231066 gpt-researcher-0.3.2/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.232425 gpt-researcher-0.3.2/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.233914 gpt-researcher-0.3.2/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.235539 gpt-researcher-0.3.2/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.236843 gpt-researcher-0.3.2/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.237881 gpt-researcher-0.3.2/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.239349 gpt-researcher-0.3.2/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1541 2024-05-09 06:41:04.000000 gpt-researcher-0.3.2/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.241104 gpt-researcher-0.3.2/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.242659 gpt-researcher-0.3.2/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.244284 gpt-researcher-0.3.2/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.245964 gpt-researcher-0.3.2/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.247966 gpt-researcher-0.3.2/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.249825 gpt-researcher-0.3.2/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.3.2/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.253277 gpt-researcher-0.3.2/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.2/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.3.2/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:41:49.212177 gpt-researcher-0.3.2/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 06:41:49.000000 gpt-researcher-0.3.2/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-09 06:41:49.000000 gpt-researcher-0.3.2/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-09 06:41:49.000000 gpt-researcher-0.3.2/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-09 06:41:49.000000 gpt-researcher-0.3.2/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-09 06:41:49.000000 gpt-researcher-0.3.2/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.3.2/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-09 06:41:49.255392 gpt-researcher-0.3.2/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-09 06:41:26.000000 gpt-researcher-0.3.2/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.572160 gpt-researcher-0.3.3/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 06:47:07.571435 gpt-researcher-0.3.3/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    10003 2024-05-08 07:24:47.000000 gpt-researcher-0.3.3/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.529889 gpt-researcher-0.3.3/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.530496 gpt-researcher-0.3.3/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.531795 gpt-researcher-0.3.3/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.533109 gpt-researcher-0.3.3/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.3.3/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.3.3/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.533945 gpt-researcher-0.3.3/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.3.3/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.538102 gpt-researcher-0.3.3/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.3.3/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.540017 gpt-researcher-0.3.3/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.3.3/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.3.3/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.540551 gpt-researcher-0.3.3/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.541785 gpt-researcher-0.3.3/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.542803 gpt-researcher-0.3.3/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.543783 gpt-researcher-0.3.3/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.546321 gpt-researcher-0.3.3/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.3.3/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     8928 2024-05-05 07:01:28.000000 gpt-researcher-0.3.3/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.3.3/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.3.3/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.547977 gpt-researcher-0.3.3/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.3.3/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.3.3/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.548681 gpt-researcher-0.3.3/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.549834 gpt-researcher-0.3.3/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.551079 gpt-researcher-0.3.3/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.552112 gpt-researcher-0.3.3/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.553097 gpt-researcher-0.3.3/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.554269 gpt-researcher-0.3.3/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.555606 gpt-researcher-0.3.3/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.556599 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.558027 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1675 2024-05-09 06:46:00.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.559731 gpt-researcher-0.3.3/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.561475 gpt-researcher-0.3.3/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.563098 gpt-researcher-0.3.3/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.564583 gpt-researcher-0.3.3/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.566113 gpt-researcher-0.3.3/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.567873 gpt-researcher-0.3.3/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.570708 gpt-researcher-0.3.3/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.536906 gpt-researcher-0.3.3/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.3.3/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-09 06:47:07.572384 gpt-researcher-0.3.3/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-09 06:46:43.000000 gpt-researcher-0.3.3/setup.py
```

### Comparing `gpt-researcher-0.3.2/LICENSE` & `gpt-researcher-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/PKG-INFO` & `gpt-researcher-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.3.2
+Version: 0.3.3
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.3.2/README.md` & `gpt-researcher-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.3.3/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.3.3/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/backend/server.py` & `gpt-researcher-0.3.3/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/backend/utils.py` & `gpt-researcher-0.3.3/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/backend/websocket_manager.py` & `gpt-researcher-0.3.3/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/config/config.py` & `gpt-researcher-0.3.3/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/context/compression.py` & `gpt-researcher-0.3.3/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/context/retriever.py` & `gpt-researcher-0.3.3/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.3.3/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.3.3/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.3.3/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/master/agent.py` & `gpt-researcher-0.3.3/gpt_researcher/master/agent.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/master/functions.py` & `gpt-researcher-0.3.3/gpt_researcher/master/functions.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/master/prompts.py` & `gpt-researcher-0.3.3/gpt_researcher/master/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.3.3/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.3.3/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.3.3/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.3.3/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.3.3/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.3.3/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,17 @@
         Searches the query
         Returns:
 
         """
         try:
             # Search the query
             results = self.client.search(self.query, search_depth="basic", max_results=max_results)
+            sources = results.get("results", [])
+            if not sources:
+                raise Exception("No results found with Tavily API search.")
             # Return the results
-            search_response = [{"href": obj["url"], "body": obj["content"]} for obj in results.get("results", [])]
+            search_response = [{"href": obj["url"], "body": obj["content"]} for obj in sources]
         except Exception as e: # Fallback in case overload on Tavily Search API
             print(f"Error: {e}. Fallback to DuckDuckGo Search API...")
             ddg = DDGS()
             search_response = ddg.text(self.query, region='wt-wt', max_results=max_results)
         return search_response
```

### Comparing `gpt-researcher-0.3.2/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.3.3/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.3.3/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.3.3/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.3.3/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.3.3/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.3.3/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher/utils/llm.py` & `gpt-researcher-0.3.3/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.3.3/gpt_researcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.3.2
+Version: 0.3.3
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.3.2/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.3.3/gpt_researcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/pyproject.toml` & `gpt-researcher-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.2/setup.py` & `gpt-researcher-0.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.3.2",
+    version="0.3.3",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```


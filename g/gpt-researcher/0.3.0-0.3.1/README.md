# Comparing `tmp/gpt-researcher-0.3.0.tar.gz` & `tmp/gpt-researcher-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.3.0.tar", last modified: Sun May  5 07:06:29 2024, max compression
+gzip compressed data, was "gpt-researcher-0.3.1.tar", last modified: Thu May  9 06:29:54 2024, max compression
```

## Comparing `gpt-researcher-0.3.0.tar` & `gpt-researcher-0.3.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.857440 gpt-researcher-0.3.0/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    10552 2024-05-05 07:06:29.856570 gpt-researcher-0.3.0/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     9829 2024-05-01 07:22:17.000000 gpt-researcher-0.3.0/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.788803 gpt-researcher-0.3.0/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.789859 gpt-researcher-0.3.0/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.791400 gpt-researcher-0.3.0/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.793029 gpt-researcher-0.3.0/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.3.0/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.3.0/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.794044 gpt-researcher-0.3.0/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.3.0/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.799909 gpt-researcher-0.3.0/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.3.0/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.804047 gpt-researcher-0.3.0/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.3.0/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.3.0/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.805315 gpt-researcher-0.3.0/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.807450 gpt-researcher-0.3.0/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.809572 gpt-researcher-0.3.0/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.811729 gpt-researcher-0.3.0/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.816261 gpt-researcher-0.3.0/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.3.0/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     8928 2024-05-05 07:01:28.000000 gpt-researcher-0.3.0/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12476 2024-05-05 07:01:28.000000 gpt-researcher-0.3.0/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    13399 2024-05-05 06:59:59.000000 gpt-researcher-0.3.0/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.818637 gpt-researcher-0.3.0/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.3.0/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.819959 gpt-researcher-0.3.0/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.821473 gpt-researcher-0.3.0/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.823144 gpt-researcher-0.3.0/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.825330 gpt-researcher-0.3.0/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.827634 gpt-researcher-0.3.0/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.829744 gpt-researcher-0.3.0/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.831965 gpt-researcher-0.3.0/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.834300 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.836685 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.839407 gpt-researcher-0.3.0/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.841497 gpt-researcher-0.3.0/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.843839 gpt-researcher-0.3.0/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.846041 gpt-researcher-0.3.0/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.848111 gpt-researcher-0.3.0/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.850280 gpt-researcher-0.3.0/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.855037 gpt-researcher-0.3.0/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.798035 gpt-researcher-0.3.0/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    10552 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.3.0/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-05 07:06:29.857689 gpt-researcher-0.3.0/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-05 07:05:54.000000 gpt-researcher-0.3.0/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.880943 gpt-researcher-0.3.1/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 06:29:54.880381 gpt-researcher-0.3.1/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    10003 2024-05-08 07:24:47.000000 gpt-researcher-0.3.1/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.827546 gpt-researcher-0.3.1/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.828687 gpt-researcher-0.3.1/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.830153 gpt-researcher-0.3.1/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.831568 gpt-researcher-0.3.1/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.3.1/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.3.1/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.832667 gpt-researcher-0.3.1/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.3.1/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.837789 gpt-researcher-0.3.1/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.3.1/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.840652 gpt-researcher-0.3.1/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.3.1/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.3.1/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.841685 gpt-researcher-0.3.1/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.843180 gpt-researcher-0.3.1/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.844573 gpt-researcher-0.3.1/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.845820 gpt-researcher-0.3.1/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.3.1/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.849824 gpt-researcher-0.3.1/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.3.1/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     8928 2024-05-05 07:01:28.000000 gpt-researcher-0.3.1/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.3.1/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.3.1/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.852515 gpt-researcher-0.3.1/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.3.1/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:26:23.000000 gpt-researcher-0.3.1/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.853433 gpt-researcher-0.3.1/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.855661 gpt-researcher-0.3.1/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.857989 gpt-researcher-0.3.1/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.859496 gpt-researcher-0.3.1/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.861057 gpt-researcher-0.3.1/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.862584 gpt-researcher-0.3.1/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.864068 gpt-researcher-0.3.1/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.865495 gpt-researcher-0.3.1/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.866945 gpt-researcher-0.3.1/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.868926 gpt-researcher-0.3.1/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.870304 gpt-researcher-0.3.1/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.872001 gpt-researcher-0.3.1/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.873405 gpt-researcher-0.3.1/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.874684 gpt-researcher-0.3.1/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.876224 gpt-researcher-0.3.1/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.3.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.879351 gpt-researcher-0.3.1/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.1/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.3.1/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:29:54.836165 gpt-researcher-0.3.1/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 06:29:54.000000 gpt-researcher-0.3.1/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-09 06:29:54.000000 gpt-researcher-0.3.1/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-09 06:29:54.000000 gpt-researcher-0.3.1/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-09 06:29:54.000000 gpt-researcher-0.3.1/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-09 06:29:54.000000 gpt-researcher-0.3.1/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.3.1/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-09 06:29:54.881118 gpt-researcher-0.3.1/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-09 06:29:35.000000 gpt-researcher-0.3.1/setup.py
```

### Comparing `gpt-researcher-0.3.0/LICENSE` & `gpt-researcher-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/PKG-INFO` & `gpt-researcher-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.3.0
+Version: 0.3.1
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -24,16 +24,16 @@
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/assafelovic/gpt-researcher?style=for-the-badge&color=orange
 
--  [English](README.md)
--  [中文](README-zh_CN.md)
+-  [English](https://github.com/assafelovic/gpt-researcher/blob/master/README.md)
+-  [中文](https://github.com/assafelovic/gpt-researcher/blob/master/README-zh_CN.md)
 
 **GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.** 
 
 The agent can produce detailed, factual and unbiased research reports, with customization options for focusing on relevant resources, outlines, and lessons. Inspired by the recent [Plan-and-Solve](https://arxiv.org/abs/2305.04091) and [RAG](https://arxiv.org/abs/2005.11401) papers, GPT Researcher addresses issues of speed, determinism and reliability, offering a more stable performance and increased speed through parallelized agent work, as opposed to synchronous operations.
 
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
@@ -152,15 +152,15 @@
 report = await researcher.write_report()
 ```
 
 **For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
 
 
 ## 🚀 Contributing
-We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
+We highly welcome contributions! Please check out [contributing](https://github.com/assafelovic/gpt-researcher/blob/master/CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
 - Our email: assafelovic@gmail.com
```

### Comparing `gpt-researcher-0.3.0/README.md` & `gpt-researcher-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/assafelovic/gpt-researcher?style=for-the-badge&color=orange
 
--  [English](README.md)
--  [中文](README-zh_CN.md)
+-  [English](https://github.com/assafelovic/gpt-researcher/blob/master/README.md)
+-  [中文](https://github.com/assafelovic/gpt-researcher/blob/master/README-zh_CN.md)
 
 **GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.** 
 
 The agent can produce detailed, factual and unbiased research reports, with customization options for focusing on relevant resources, outlines, and lessons. Inspired by the recent [Plan-and-Solve](https://arxiv.org/abs/2305.04091) and [RAG](https://arxiv.org/abs/2005.11401) papers, GPT Researcher addresses issues of speed, determinism and reliability, offering a more stable performance and increased speed through parallelized agent work, as opposed to synchronous operations.
 
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
@@ -134,15 +134,15 @@
 report = await researcher.write_report()
 ```
 
 **For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
 
 
 ## 🚀 Contributing
-We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
+We highly welcome contributions! Please check out [contributing](https://github.com/assafelovic/gpt-researcher/blob/master/CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
 - Our email: assafelovic@gmail.com
```

### Comparing `gpt-researcher-0.3.0/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.3.1/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.3.1/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/backend/server.py` & `gpt-researcher-0.3.1/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/backend/utils.py` & `gpt-researcher-0.3.1/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/backend/websocket_manager.py` & `gpt-researcher-0.3.1/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/config/config.py` & `gpt-researcher-0.3.1/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/context/compression.py` & `gpt-researcher-0.3.1/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/context/retriever.py` & `gpt-researcher-0.3.1/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.3.1/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.3.1/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.3.1/gpt_researcher/llm_provider/openai/openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,37 +12,50 @@
         temperature,
         max_tokens
     ):
         self.model = model
         self.temperature = temperature
         self.max_tokens = max_tokens
         self.api_key = self.get_api_key()
+        self.base_url = self.get_base_url()
         self.llm = self.get_llm_model()
 
     def get_api_key(self):
         """
         Gets the OpenAI API key
         Returns:
 
         """
         try:
             api_key = os.environ["OPENAI_API_KEY"]
-        except:
+        except KeyError:
             raise Exception(
                 "OpenAI API key not found. Please set the OPENAI_API_KEY environment variable.")
         return api_key
 
+    def get_base_url(self):
+        """
+        Gets the OpenAI Base URL from the environment variable if defined otherwise use the default one
+        Returns:
+
+        """
+        base_url = os.environ.get("OPENAI_BASE_URL", None)
+        return base_url
+
+
     def get_llm_model(self):
         # Initializing the chat model
         llm = ChatOpenAI(
             model=self.model,
             temperature=self.temperature,
             max_tokens=self.max_tokens,
             api_key=self.api_key
         )
+        if self.base_url:
+            llm.base_url = self.base_url
 
         return llm
 
     async def get_chat_response(self, messages, stream, websocket=None):
         if not stream:
             # Getting output from the model chain using ainvoke for asynchronous invoking
             output = await self.llm.ainvoke(messages)
@@ -64,9 +77,9 @@
                 paragraph += content
                 if "\n" in paragraph:
                     if websocket is not None:
                         await websocket.send_json({"type": "report", "output": paragraph})
                     else:
                         print(f"{Fore.GREEN}{paragraph}{Style.RESET_ALL}")
                     paragraph = ""
-                    
+
         return response
```

### Comparing `gpt-researcher-0.3.0/gpt_researcher/master/agent.py` & `gpt-researcher-0.3.1/gpt_researcher/master/agent.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/master/functions.py` & `gpt-researcher-0.3.1/gpt_researcher/master/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,21 +281,21 @@
                 {"role": "user", "content": generate_report_introduction(query, context)}],
             temperature=0,
             llm_provider=config.llm_provider,
             stream=True,
             websocket=websocket,
             max_tokens=config.smart_token_limit
         )
-        
+
         return introduction
     except Exception as e:
         print(f"{Fore.RED}Error in generating report introduction: {e}{Style.RESET_ALL}")
 
     return ""
-    
+
 def extract_headers(markdown_text: str):
     # Function to extract headers from markdown text
 
     headers = []
     parsed_md = markdown.markdown(markdown_text)  # Parse markdown text
     lines = parsed_md.split("\n")  # Split text into lines
 
@@ -354,15 +354,15 @@
     except Exception as e:
         print("table_of_contents Exception : ", e)  # Print exception if any
         return markdown_text  # Return original markdown text if an exception occurs
 
 def add_source_urls(report_markdown: str, visited_urls: set):
     """
     This function takes a Markdown report and a set of visited URLs as input parameters.
-    
+
     Args:
       report_markdown (str): The `add_source_urls` function takes in two parameters:
       visited_urls (set): Visited_urls is a set that contains URLs that have already been visited. This
     parameter is used to keep track of which URLs have already been included in the report_markdown to
     avoid duplication.
     """
     try:
```

### Comparing `gpt-researcher-0.3.0/gpt_researcher/master/prompts.py` & `gpt-researcher-0.3.1/gpt_researcher/master/prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
 def generate_subtopic_report_prompt(
     current_subtopic,
     existing_headers,
     main_topic,
     context,
     report_format="apa",
-    total_words=1000,
+    total_words=800,
     max_subsections=5,
 ) -> str:
 
     return f"""
     "Context":
     "{context}"
```

### Comparing `gpt-researcher-0.3.0/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.3.1/gpt_researcher/memory/embeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         _embeddings = None
         match embedding_provider:
             case "ollama":
                 from langchain.embeddings import OllamaEmbeddings
                 _embeddings = OllamaEmbeddings(model="llama2")
             case "openai":
                 from langchain_openai import OpenAIEmbeddings
-                _embeddings = OpenAIEmbeddings()
+                _embeddings = OpenAIEmbeddings(model="text-embedding-3-small")
             case "azureopenai":
                 from langchain_openai import AzureOpenAIEmbeddings
                 _embeddings = AzureOpenAIEmbeddings(deployment=os.environ["AZURE_EMBEDDING_MODEL"], chunk_size=16)
             case "huggingface":
                 from langchain.embeddings import HuggingFaceEmbeddings
                 _embeddings = HuggingFaceEmbeddings()
```

### Comparing `gpt-researcher-0.3.0/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.3.1/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.3.1/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.3.1/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.3.1/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.3.1/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.3.1/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.3.1/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.3.1/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.3.1/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.3.1/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.3.1/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.3.1/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.3.1/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher/utils/llm.py` & `gpt-researcher-0.3.1/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.3.1/gpt_researcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.3.0
+Version: 0.3.1
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -24,16 +24,16 @@
 [![Twitter Follow](https://img.shields.io/twitter/follow/assaf_elovic?style=social)](https://twitter.com/assaf_elovic)
 [![PyPI version](https://badge.fury.io/py/gpt-researcher.svg)](https://badge.fury.io/py/gpt-researcher)
 
 <!-- MARKDOWN LINKS & IMAGES -->
 <!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
 [contributors-shield]: https://img.shields.io/github/contributors/assafelovic/gpt-researcher?style=for-the-badge&color=orange
 
--  [English](README.md)
--  [中文](README-zh_CN.md)
+-  [English](https://github.com/assafelovic/gpt-researcher/blob/master/README.md)
+-  [中文](https://github.com/assafelovic/gpt-researcher/blob/master/README-zh_CN.md)
 
 **GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.** 
 
 The agent can produce detailed, factual and unbiased research reports, with customization options for focusing on relevant resources, outlines, and lessons. Inspired by the recent [Plan-and-Solve](https://arxiv.org/abs/2305.04091) and [RAG](https://arxiv.org/abs/2005.11401) papers, GPT Researcher addresses issues of speed, determinism and reliability, offering a more stable performance and increased speed through parallelized agent work, as opposed to synchronous operations.
 
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
@@ -152,15 +152,15 @@
 report = await researcher.write_report()
 ```
 
 **For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
 
 
 ## 🚀 Contributing
-We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
+We highly welcome contributions! Please check out [contributing](https://github.com/assafelovic/gpt-researcher/blob/master/CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
 - Our email: assafelovic@gmail.com
```

### Comparing `gpt-researcher-0.3.0/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.3.1/gpt_researcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/pyproject.toml` & `gpt-researcher-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.0/setup.py` & `gpt-researcher-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.3.0",
+    version="0.3.1",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```


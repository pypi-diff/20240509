# Comparing `tmp/gpt-researcher-0.3.3.tar.gz` & `tmp/gpt-researcher-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.3.3.tar", last modified: Thu May  9 06:47:07 2024, max compression
+gzip compressed data, was "gpt-researcher-0.3.4.tar", last modified: Thu May  9 12:22:38 2024, max compression
```

## Comparing `gpt-researcher-0.3.3.tar` & `gpt-researcher-0.3.4.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.572160 gpt-researcher-0.3.3/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 06:47:07.571435 gpt-researcher-0.3.3/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)    10003 2024-05-08 07:24:47.000000 gpt-researcher-0.3.3/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.529889 gpt-researcher-0.3.3/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.530496 gpt-researcher-0.3.3/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.531795 gpt-researcher-0.3.3/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.533109 gpt-researcher-0.3.3/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.3.3/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.3.3/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.533945 gpt-researcher-0.3.3/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.3.3/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.538102 gpt-researcher-0.3.3/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.3.3/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.540017 gpt-researcher-0.3.3/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.3.3/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.3.3/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.540551 gpt-researcher-0.3.3/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.541785 gpt-researcher-0.3.3/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.542803 gpt-researcher-0.3.3/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.543783 gpt-researcher-0.3.3/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.3.3/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.546321 gpt-researcher-0.3.3/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.3.3/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     8928 2024-05-05 07:01:28.000000 gpt-researcher-0.3.3/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.3.3/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.3.3/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.547977 gpt-researcher-0.3.3/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.3.3/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.3.3/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.548681 gpt-researcher-0.3.3/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.549834 gpt-researcher-0.3.3/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.551079 gpt-researcher-0.3.3/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.552112 gpt-researcher-0.3.3/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.553097 gpt-researcher-0.3.3/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.554269 gpt-researcher-0.3.3/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.555606 gpt-researcher-0.3.3/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.556599 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.558027 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1675 2024-05-09 06:46:00.000000 gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.559731 gpt-researcher-0.3.3/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.561475 gpt-researcher-0.3.3/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.563098 gpt-researcher-0.3.3/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.564583 gpt-researcher-0.3.3/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.566113 gpt-researcher-0.3.3/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.567873 gpt-researcher-0.3.3/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.3.3/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.570708 gpt-researcher-0.3.3/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.3/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.3.3/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 06:47:07.536906 gpt-researcher-0.3.3/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-09 06:47:07.000000 gpt-researcher-0.3.3/gpt_researcher.egg-info/top_level.txt
--rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.3.3/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-09 06:47:07.572384 gpt-researcher-0.3.3/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-09 06:46:43.000000 gpt-researcher-0.3.3/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.112118 gpt-researcher-0.3.4/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 12:22:38.111378 gpt-researcher-0.3.4/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)    10003 2024-05-08 07:24:47.000000 gpt-researcher-0.3.4/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.049240 gpt-researcher-0.3.4/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.050224 gpt-researcher-0.3.4/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.051755 gpt-researcher-0.3.4/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.053115 gpt-researcher-0.3.4/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.3.4/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.3.4/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.054409 gpt-researcher-0.3.4/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.3.4/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.060305 gpt-researcher-0.3.4/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.3.4/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.063482 gpt-researcher-0.3.4/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.3.4/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.3.4/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.064503 gpt-researcher-0.3.4/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.065961 gpt-researcher-0.3.4/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.067613 gpt-researcher-0.3.4/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.069485 gpt-researcher-0.3.4/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2450 2024-05-08 07:24:47.000000 gpt-researcher-0.3.4/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.074229 gpt-researcher-0.3.4/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.3.4/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     9302 2024-05-09 12:16:45.000000 gpt-researcher-0.3.4/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12460 2024-05-08 07:24:47.000000 gpt-researcher-0.3.4/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    13398 2024-05-06 06:02:27.000000 gpt-researcher-0.3.4/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.076403 gpt-researcher-0.3.4/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.3.4/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1077 2024-05-09 06:30:45.000000 gpt-researcher-0.3.4/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.077360 gpt-researcher-0.3.4/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.079470 gpt-researcher-0.3.4/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.081841 gpt-researcher-0.3.4/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-05-06 05:46:56.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.083632 gpt-researcher-0.3.4/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.085716 gpt-researcher-0.3.4/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.088103 gpt-researcher-0.3.4/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.090185 gpt-researcher-0.3.4/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.091847 gpt-researcher-0.3.4/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.093551 gpt-researcher-0.3.4/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1675 2024-05-09 06:46:00.000000 gpt-researcher-0.3.4/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.095797 gpt-researcher-0.3.4/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.097443 gpt-researcher-0.3.4/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.099343 gpt-researcher-0.3.4/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.101139 gpt-researcher-0.3.4/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.103273 gpt-researcher-0.3.4/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.105472 gpt-researcher-0.3.4/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.3.4/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.109904 gpt-researcher-0.3.4/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.4/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.3.4/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-09 12:22:38.058335 gpt-researcher-0.3.4/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    10726 2024-05-09 12:22:37.000000 gpt-researcher-0.3.4/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-09 12:22:37.000000 gpt-researcher-0.3.4/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-09 12:22:37.000000 gpt-researcher-0.3.4/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-09 12:22:37.000000 gpt-researcher-0.3.4/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-09 12:22:37.000000 gpt-researcher-0.3.4/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.3.4/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-09 12:22:38.112436 gpt-researcher-0.3.4/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-09 12:22:15.000000 gpt-researcher-0.3.4/setup.py
```

### Comparing `gpt-researcher-0.3.3/LICENSE` & `gpt-researcher-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/PKG-INFO` & `gpt-researcher-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.3.3
+Version: 0.3.4
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.3.3/README.md` & `gpt-researcher-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.3.4/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.3.4/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/backend/server.py` & `gpt-researcher-0.3.4/backend/server.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/backend/utils.py` & `gpt-researcher-0.3.4/backend/utils.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/backend/websocket_manager.py` & `gpt-researcher-0.3.4/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/config/config.py` & `gpt-researcher-0.3.4/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/context/compression.py` & `gpt-researcher-0.3.4/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/context/retriever.py` & `gpt-researcher-0.3.4/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.3.4/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.3.4/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.3.4/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/master/agent.py` & `gpt-researcher-0.3.4/gpt_researcher/master/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         source_urls=None,
         config_path=None,
         websocket=None,
         agent=None,
         role=None,
         parent_query: str = "",
         subtopics: list = [],
-        visited_urls: set = set()
+        visited_urls: set = set(),
+        verbose: bool = True,
     ):
         """
         Initialize the GPT Researcher class.
         Args:
             query: str,
             report_type: str
             source_urls
@@ -48,34 +49,38 @@
         self.websocket = websocket
         self.cfg = Config(config_path)
         self.retriever = get_retriever(self.cfg.retriever)
         self.context = []
         self.source_urls = source_urls
         self.memory = Memory(self.cfg.embedding_provider)
         self.visited_urls = visited_urls
+        self.verbose = verbose
 
         # Only relevant for DETAILED REPORTS
         # --------------------------------------
 
         # Stores the main query of the detailed report
         self.parent_query = parent_query
 
         # Stores all the user provided subtopics
         self.subtopics = subtopics
 
     async def conduct_research(self):
         """
         Runs the GPT Researcher to conduct research
         """
-        print(f"🔎 Running research for '{self.query}'...")
+        if self.verbose:
+            await stream_output("logs", f"🔎 Starting the research task for '{self.query}'...", self.websocket)
         
         # Generate Agent
         if not (self.agent and self.role):
             self.agent, self.role = await choose_agent(self.query, self.cfg, self.parent_query)
-        await stream_output("logs", self.agent, self.websocket)
+
+        if self.verbose:
+            await stream_output("logs", self.agent, self.websocket)
 
         # If specified, the researcher will use the given urls as the context for the research.
         if self.source_urls:
             self.context = await self.get_context_by_urls(self.source_urls)
         else:
             self.context = await self.get_context_by_search(self.query)
 
@@ -84,16 +89,16 @@
     async def write_report(self, existing_headers: list = []):
         """
         Writes the report based on research conducted
 
         Returns:
             str: The report
         """
-
-        await stream_output("logs", f"✍️ Writing summary for research task: {self.query}...", self.websocket)
+        if self.verbose:
+            await stream_output("logs", f"✍️ Writing summary for research task: {self.query}...", self.websocket)
 
         if self.report_type == "custom_report":
             self.role = self.cfg.agent_role if self.cfg.agent_role else self.role
         elif self.report_type == "subtopic_report":
             report = await generate_report(
                 query=self.query,
                 context=self.context,
@@ -117,15 +122,16 @@
         return report
 
     async def get_context_by_urls(self, urls):
         """
             Scrapes and compresses the context from the given urls
         """
         new_search_urls = await self.get_new_urls(urls)
-        await stream_output("logs",
+        if self.verbose:
+            await stream_output("logs",
                             f"🧠 I will conduct my research based on the following urls: {new_search_urls}...",
                             self.websocket)
         scraped_sites = scrape_urls(new_search_urls, self.cfg)
         return await self.get_similar_content_by_query(self.query, scraped_sites)
 
     async def get_context_by_search(self, query):
         """
@@ -137,55 +143,57 @@
         # Generate Sub-Queries including original query
         sub_queries = await get_sub_queries(query, self.role, self.cfg, self.parent_query, self.report_type)
 
         # If this is not part of a sub researcher, add original query to research for better results
         if self.report_type != "subtopic_report":
             sub_queries.append(query)
 
-        await stream_output("logs",
-                            f"🧠 I will conduct my research based on the following queries: {sub_queries}...",
-                            self.websocket)
+        if self.verbose:
+            await stream_output("logs",
+                                f"🧠 I will conduct my research based on the following queries: {sub_queries}...",
+                                self.websocket)
 
         # Using asyncio.gather to process the sub_queries asynchronously
         context = await asyncio.gather(*[self.process_sub_query(sub_query) for sub_query in sub_queries])
         return context
 
     async def process_sub_query(self, sub_query: str):
         """Takes in a sub query and scrapes urls based on it and gathers context.
 
         Args:
             sub_query (str): The sub-query generated from the original query
 
         Returns:
             str: The context gathered from search
         """
-        await stream_output("logs", f"\n🔎 Running research for '{sub_query}'...", self.websocket)
+        if self.verbose:
+            await stream_output("logs", f"\n🔎 Running research for '{sub_query}'...", self.websocket)
 
         scraped_sites = await self.scrape_sites_by_query(sub_query)
         content = await self.get_similar_content_by_query(sub_query, scraped_sites)
 
-        if content:
+        if content and self.verbose:
             await stream_output("logs", f"📃 {content}", self.websocket)
-        else:
+        elif self.verbose:
             await stream_output("logs", f"🤷 No content found for '{sub_query}'...", self.websocket)
         return content
 
     async def get_new_urls(self, url_set_input):
         """ Gets the new urls from the given url set.
         Args: url_set_input (set[str]): The url set to get the new urls from
         Returns: list[str]: The new urls from the given url set
         """
 
         new_urls = []
         for url in url_set_input:
             if url not in self.visited_urls:
-                await stream_output("logs", f"✅ Adding source url to research: {url}\n", self.websocket)
-
                 self.visited_urls.add(url)
                 new_urls.append(url)
+                if self.verbose:
+                    await stream_output("logs", f"✅ Added source url to research: {url}\n", self.websocket)
 
         return new_urls
 
     async def scrape_sites_by_query(self, sub_query):
         """
         Runs a sub-query
         Args:
@@ -197,21 +205,22 @@
         # Get Urls
         retriever = self.retriever(sub_query)
         search_results = retriever.search(
             max_results=self.cfg.max_search_results_per_query)
         new_search_urls = await self.get_new_urls([url.get("href") for url in search_results])
 
         # Scrape Urls
-        # await stream_output("logs", f"📝Scraping urls {new_search_urls}...\n", self.websocket)
-        await stream_output("logs", f"🤔 Researching for relevant information...\n", self.websocket)
+        if self.verbose:
+            await stream_output("logs", f"🤔 Researching for relevant information...\n", self.websocket)
         scraped_content_results = scrape_urls(new_search_urls, self.cfg)
         return scraped_content_results
 
     async def get_similar_content_by_query(self, query, pages):
-        await stream_output("logs", f"📝 Getting relevant content based on query: {query}...", self.websocket)
+        if self.verbose:
+            await stream_output("logs", f"📝 Getting relevant content based on query: {query}...", self.websocket)
         # Summarize Raw Data
         context_compressor = ContextCompressor(
             documents=pages, embeddings=self.memory.get_embeddings())
         # Run Tasks
         return context_compressor.get_context(query, max_results=8)
 
     ########################################################################################
@@ -228,20 +237,22 @@
         """
         This async function generates subtopics based on user input and other parameters.
 
         Returns:
           The `get_subtopics` function is returning the `subtopics` that are generated by the
         `construct_subtopics` function.
         """
-        await stream_output("logs", f"🤔 Generating subtopics...", self.websocket)
+        if self.verbose:
+            await stream_output("logs", f"🤔 Generating subtopics...", self.websocket)
 
         subtopics = await construct_subtopics(
             task=self.query,
             data=self.context,
             config=self.cfg,
             # This is a list of user provided subtopics
             subtopics=self.subtopics,
         )
 
-        await stream_output("logs", f"📋Subtopics: {subtopics}", self.websocket)
+        if self.verbose:
+            await stream_output("logs", f"📋Subtopics: {subtopics}", self.websocket)
 
         return subtopics
```

### Comparing `gpt-researcher-0.3.3/gpt_researcher/master/functions.py` & `gpt-researcher-0.3.4/gpt_researcher/master/functions.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/master/prompts.py` & `gpt-researcher-0.3.4/gpt_researcher/master/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.3.4/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.3.4/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.3.4/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.3.4/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.3.4/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.3.4/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.3.4/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.3.4/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.3.4/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.3.4/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.3.4/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.3.4/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.3.4/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.3.4/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher/utils/llm.py` & `gpt-researcher-0.3.4/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.3.4/gpt_researcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.3.3
+Version: 0.3.4
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `gpt-researcher-0.3.3/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.3.4/gpt_researcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/pyproject.toml` & `gpt-researcher-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.3.3/setup.py` & `gpt-researcher-0.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.3.3",
+    version="0.3.4",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```


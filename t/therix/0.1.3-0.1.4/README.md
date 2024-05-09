# Comparing `tmp/therix-0.1.3.tar.gz` & `tmp/therix-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "therix-0.1.3.tar", max compression
+gzip compressed data, was "therix-0.1.4.tar", max compression
```

## Comparing `therix-0.1.3.tar` & `therix-0.1.4.tar`

### file list

```diff
@@ -1,99 +1,105 @@
--rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.3/LICENSE
--rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.3/README.md
--rw-r--r--   0        0        0     1023 2024-05-03 13:10:49.072394 therix-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.3/therix/__init__.py
--rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.3/therix/alembic/README
--rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.3/therix/alembic/env.py
--rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.3/therix/alembic/script.py.mako
--rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.3/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
--rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.3/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
--rw-r--r--   0        0        0      838 2024-05-03 12:50:17.295642 therix-0.1.3/therix/alembic/versions/2024_05_03_1637-04b509a2f1cc_added_chat_history_fix.py
--rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.3/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
--rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.3/therix/alembic.ini
--rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.3/therix/core/JSONLoader.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.3/therix/core/__init__.py
--rw-r--r--   0        0        0     2371 2024-05-03 05:53:02.645943 therix-0.1.3/therix/core/cache.py
--rw-r--r--   0        0        0     1408 2024-05-03 12:50:17.295817 therix-0.1.3/therix/core/chat_history/base_chat_history.py
--rw-r--r--   0        0        0     1649 2024-05-03 12:50:17.296463 therix-0.1.3/therix/core/constants.py
--rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.3/therix/core/data_sources.py
--rw-r--r--   0        0        0     1676 2024-04-16 12:12:31.276049 therix-0.1.3/therix/core/embedding_models.py
--rw-r--r--   0        0        0     2374 2024-05-03 13:10:49.072728 therix-0.1.3/therix/core/inference_models.py
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.3/therix/core/output_source.py
--rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.3/therix/core/pii_filter_config.py
--rw-r--r--   0        0        0     5711 2024-05-03 12:50:17.297034 therix-0.1.3/therix/core/pipeline.py
--rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.3/therix/core/pipeline_component.py
--rw-r--r--   0        0        0      248 2024-05-03 05:53:02.646834 therix-0.1.3/therix/core/response.py
--rw-r--r--   0        0        0      588 2024-04-26 09:41:57.772788 therix-0.1.3/therix/core/summarizer_config.py
--rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.3/therix/core/trace.py
--rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.3/therix/db/__init__.py
--rw-r--r--   0        0        0     3757 2024-04-29 11:17:18.463868 therix-0.1.3/therix/db/db_manager.py
--rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.3/therix/db/session.py
--rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.3/therix/db/tests/__init__.py
--rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.3/therix/db/tests/test_db_manager.py
--rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.3/therix/docs/.gitignore
--rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.3/therix/docs/README.md
--rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.3/therix/docs/babel.config.js
--rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.3/therix/docs/blog/2019-05-28-first-blog-post.md
--rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.3/therix/docs/blog/2019-05-29-long-blog-post.md
--rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.3/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
--rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.3/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.3/therix/docs/blog/2021-08-26-welcome/index.md
--rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.3/therix/docs/blog/authors.yml
--rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.3/therix/docs/docs/LLM-Proxy/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.3/therix/docs/docs/LLM-Proxy/index.md
--rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.3/therix/docs/docs/core-components/_category_.json
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/_category_.json
--rw-r--r--   0        0        0     1460 2024-05-03 05:53:02.648669 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/caching.md
--rw-r--r--   0        0        0       91 2024-05-03 05:53:02.648747 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
--rw-r--r--   0        0        0       97 2024-05-03 05:53:02.648823 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
--rw-r--r--   0        0        0       81 2024-05-03 05:53:02.649008 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/index.md
--rw-r--r--   0        0        0       98 2024-05-03 05:53:02.649150 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
--rw-r--r--   0        0        0       78 2024-05-03 05:53:02.649233 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations/trace.md
--rw-r--r--   0        0        0       97 2024-05-03 05:53:02.648360 therix-0.1.3/therix/docs/docs/core-components/pipeline-configurations.md
--rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.3/therix/docs/docs/core-components/pipeline-templates.md
--rw-r--r--   0        0        0       67 2024-05-03 05:53:02.649417 therix-0.1.3/therix/docs/docs/core-components/pipeline.md
--rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.3/therix/docs/docs/introduction/_category_.json
--rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.3/therix/docs/docs/introduction/getting-started.md
--rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.3/therix/docs/docs/introduction/index.md
--rw-r--r--   0        0        0      435 2024-05-03 05:53:02.649793 therix-0.1.3/therix/docs/docs/introduction/installation.md
--rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.3/therix/docs/docs/observability/_category_.json
--rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.3/therix/docs/docs/observability/index.md
--rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.3/therix/docs/docs/squad/_category_.json
--rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.3/therix/docs/docs/squad/index.md
--rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.3/therix/docs/docs/usage/_category_.json
--rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.3/therix/docs/docs/usage/index.md
--rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.3/therix/docs/docs/use-cases/_category_.json
--rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.3/therix/docs/docs/use-cases/faq.md
--rw-r--r--   0        0        0     4371 2024-05-03 05:53:02.651405 therix-0.1.3/therix/docs/docs/use-cases/summarizer_doc.md
--rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.3/therix/docs/docusaurus.config.js
--rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.3/therix/docs/package-lock.json
--rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.3/therix/docs/package.json
--rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.3/therix/docs/sidebars.js
--rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.3/therix/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.3/therix/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.3/therix/docs/src/css/custom.css
--rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.3/therix/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.3/therix/docs/src/pages/markdown-page.md
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.3/therix/docs/static/.nojekyll
--rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.3/therix/docs/static/img/coditas.png
--rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.3/therix/docs/static/img/coditasLogo.svg
--rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.3/therix/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.3/therix/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.3/therix/docs/static/img/favicon.ico
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.3/therix/docs/static/img/icon.svg
--rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.3/therix/docs/static/img/logo.png
--rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.3/therix/docs/static/img/logo.svg
--rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.3/therix/docs/static/img/therix-logo.png
--rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.3/therix/docs/static/img/undraw_docusaurus_mountain.svg
--rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.3/therix/docs/static/img/undraw_docusaurus_react.svg
--rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.3/therix/docs/static/img/undraw_docusaurus_tree.svg
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.3/therix/entities/__init__.py
--rw-r--r--   0        0        0     2535 2024-05-03 12:50:17.297755 therix-0.1.3/therix/entities/models.py
--rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.3/therix/pylintrc
--rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.3/therix/services/__init__.py
--rw-r--r--   0        0        0     4426 2024-04-26 09:41:57.774292 therix-0.1.3/therix/services/pipeline_service.py
--rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.3/therix/services/web_crawling.py
--rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.3/therix/utils/pii_filter.py
--rw-r--r--   0        0        0    10397 2024-05-03 12:50:17.298312 therix-0.1.3/therix/utils/rag.py
--rw-r--r--   0        0        0     4051 2024-04-26 09:41:57.774560 therix-0.1.3/therix/utils/summarizer.py
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 therix-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-20 09:19:32.105170 therix-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1218 2024-04-16 12:12:31.272029 therix-0.1.4/README.md
+-rw-r--r--   0        0        0     1023 2024-05-09 12:13:10.309807 therix-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275037 therix-0.1.4/therix/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-26 09:41:57.771370 therix-0.1.4/therix/alembic/README
+-rw-r--r--   0        0        0     2912 2024-04-26 09:41:57.771506 therix-0.1.4/therix/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-04-26 09:41:57.771730 therix-0.1.4/therix/alembic/script.py.mako
+-rw-r--r--   0        0        0     2619 2024-04-29 11:17:18.463236 therix-0.1.4/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py
+-rw-r--r--   0        0        0     2131 2024-05-03 12:50:17.295513 therix-0.1.4/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py
+-rw-r--r--   0        0        0      880 2024-05-08 11:24:55.867083 therix-0.1.4/therix/alembic/versions/2024_05_06_1524-1e7f3dc15e9c_added_chat_history_fix.py
+-rw-r--r--   0        0        0     3092 2024-04-26 10:10:45.584242 therix-0.1.4/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py
+-rw-r--r--   0        0        0     3599 2024-04-26 09:41:57.771233 therix-0.1.4/therix/alembic.ini
+-rw-r--r--   0        0        0     2083 2024-04-16 12:12:31.275418 therix-0.1.4/therix/core/JSONLoader.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.275458 therix-0.1.4/therix/core/__init__.py
+-rw-r--r--   0        0        0     2371 2024-05-08 11:24:55.868083 therix-0.1.4/therix/core/cache.py
+-rw-r--r--   0        0        0     1408 2024-05-03 12:50:17.295817 therix-0.1.4/therix/core/chat_history/base_chat_history.py
+-rw-r--r--   0        0        0     1649 2024-05-03 12:50:17.296463 therix-0.1.4/therix/core/constants.py
+-rw-r--r--   0        0        0      854 2024-04-16 12:12:31.275897 therix-0.1.4/therix/core/data_sources.py
+-rw-r--r--   0        0        0     1676 2024-04-16 12:12:31.276049 therix-0.1.4/therix/core/embedding_models.py
+-rw-r--r--   0        0        0     2374 2024-05-03 13:10:49.072728 therix-0.1.4/therix/core/inference_models.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.276202 therix-0.1.4/therix/core/output_source.py
+-rw-r--r--   0        0        0      251 2024-04-26 09:41:57.772340 therix-0.1.4/therix/core/pii_filter_config.py
+-rw-r--r--   0        0        0     5653 2024-05-09 12:03:13.869241 therix-0.1.4/therix/core/pipeline.py
+-rw-r--r--   0        0        0     1153 2024-04-16 12:12:31.276619 therix-0.1.4/therix/core/pipeline_component.py
+-rw-r--r--   0        0        0      238 2024-05-08 11:24:55.868662 therix-0.1.4/therix/core/response.py
+-rw-r--r--   0        0        0      588 2024-04-26 09:41:57.772788 therix-0.1.4/therix/core/summarizer_config.py
+-rw-r--r--   0        0        0      299 2024-04-16 12:12:31.276847 therix-0.1.4/therix/core/trace.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:07:48.247669 therix-0.1.4/therix/db/__init__.py
+-rw-r--r--   0        0        0     3757 2024-04-29 11:17:18.463868 therix-0.1.4/therix/db/db_manager.py
+-rw-r--r--   0        0        0      412 2024-04-26 09:41:57.773326 therix-0.1.4/therix/db/session.py
+-rw-r--r--   0        0        0        0 2024-04-26 09:41:57.773383 therix-0.1.4/therix/db/tests/__init__.py
+-rw-r--r--   0        0        0     1895 2024-04-26 09:41:57.773575 therix-0.1.4/therix/db/tests/test_db_manager.py
+-rw-r--r--   0        0        0      235 2024-05-03 05:53:02.647293 therix-0.1.4/therix/docs/.gitignore
+-rw-r--r--   0        0        0      768 2024-04-16 12:12:31.278162 therix-0.1.4/therix/docs/README.md
+-rw-r--r--   0        0        0       89 2024-04-16 12:12:31.278296 therix-0.1.4/therix/docs/babel.config.js
+-rw-r--r--   0        0        0      389 2024-04-16 12:12:31.278633 therix-0.1.4/therix/docs/blog/2019-05-28-first-blog-post.md
+-rw-r--r--   0        0        0     3116 2024-04-16 12:12:31.278892 therix-0.1.4/therix/docs/blog/2019-05-29-long-blog-post.md
+-rw-r--r--   0        0        0      439 2024-04-16 12:12:31.279136 therix-0.1.4/therix/docs/blog/2021-08-01-mdx-blog-post.mdx
+-rw-r--r--   0        0        0    96122 2024-04-16 12:12:31.280182 therix-0.1.4/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-r--r--   0        0        0      783 2024-04-16 12:12:31.280655 therix-0.1.4/therix/docs/blog/2021-08-26-welcome/index.md
+-rw-r--r--   0        0        0      447 2024-04-16 12:12:31.280914 therix-0.1.4/therix/docs/blog/authors.yml
+-rw-r--r--   0        0        0      162 2024-05-03 05:53:02.647798 therix-0.1.4/therix/docs/docs/LLM-Proxy/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.647994 therix-0.1.4/therix/docs/docs/LLM-Proxy/index.md
+-rw-r--r--   0        0        0      168 2024-05-03 05:53:02.648275 therix-0.1.4/therix/docs/docs/core-components/_category_.json
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.648495 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/_category_.json
+-rw-r--r--   0        0        0     3533 2024-05-08 11:24:55.869158 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/caching.md
+-rw-r--r--   0        0        0     1288 2024-05-08 11:24:55.869292 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/data-sources.md
+-rw-r--r--   0        0        0     3959 2024-05-08 11:24:55.869587 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/embedding-model.md
+-rw-r--r--   0        0        0       81 2024-05-03 05:53:02.649008 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/index.md
+-rw-r--r--   0        0        0     5496 2024-05-08 11:24:55.869807 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/inference-model.md
+-rw-r--r--   0        0        0   101843 2024-05-08 11:24:55.870971 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_dashboard.JPG
+-rw-r--r--   0        0        0    87594 2024-05-08 11:24:55.871966 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/screenshots/trace_settings_dashboard.JPG
+-rw-r--r--   0        0        0     1835 2024-05-08 11:24:55.872168 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations/trace.md
+-rw-r--r--   0        0        0     1377 2024-05-08 11:24:55.868823 therix-0.1.4/therix/docs/docs/core-components/pipeline-configurations.md
+-rw-r--r--   0        0        0       88 2024-05-03 05:53:02.649320 therix-0.1.4/therix/docs/docs/core-components/pipeline-templates.md
+-rw-r--r--   0        0        0     3488 2024-05-08 11:24:55.872304 therix-0.1.4/therix/docs/docs/core-components/pipeline.md
+-rw-r--r--   0        0        0      182 2024-05-03 05:53:02.649540 therix-0.1.4/therix/docs/docs/introduction/_category_.json
+-rw-r--r--   0        0        0     1266 2024-05-03 05:53:02.649620 therix-0.1.4/therix/docs/docs/introduction/getting-started.md
+-rw-r--r--   0        0        0      701 2024-05-03 05:53:02.649715 therix-0.1.4/therix/docs/docs/introduction/index.md
+-rw-r--r--   0        0        0     1813 2024-05-08 11:24:55.872443 therix-0.1.4/therix/docs/docs/introduction/installation.md
+-rw-r--r--   0        0        0      166 2024-05-03 05:53:02.649919 therix-0.1.4/therix/docs/docs/observability/_category_.json
+-rw-r--r--   0        0        0       66 2024-05-03 05:53:02.649997 therix-0.1.4/therix/docs/docs/observability/index.md
+-rw-r--r--   0        0        0      158 2024-05-03 05:53:02.650150 therix-0.1.4/therix/docs/docs/squad/_category_.json
+-rw-r--r--   0        0        0       50 2024-05-03 05:53:02.650236 therix-0.1.4/therix/docs/docs/squad/index.md
+-rw-r--r--   0        0        0      171 2024-05-03 05:53:02.650401 therix-0.1.4/therix/docs/docs/usage/_category_.json
+-rw-r--r--   0        0        0       76 2024-05-03 05:53:02.650498 therix-0.1.4/therix/docs/docs/usage/index.md
+-rw-r--r--   0        0        0      183 2024-05-03 05:53:02.650644 therix-0.1.4/therix/docs/docs/use-cases/_category_.json
+-rw-r--r--   0        0        0       64 2024-05-03 05:53:02.650837 therix-0.1.4/therix/docs/docs/use-cases/faq.md
+-rw-r--r--   0        0        0     4156 2024-05-08 11:24:55.872787 therix-0.1.4/therix/docs/docs/use-cases/summarizer.md
+-rw-r--r--   0        0        0     3888 2024-05-03 05:53:02.652039 therix-0.1.4/therix/docs/docusaurus.config.js
+-rw-r--r--   0        0        0   574450 2024-05-03 05:53:02.654343 therix-0.1.4/therix/docs/package-lock.json
+-rw-r--r--   0        0        0     1140 2024-05-03 05:53:02.654731 therix-0.1.4/therix/docs/package.json
+-rw-r--r--   0        0        0      779 2024-04-16 12:12:31.287120 therix-0.1.4/therix/docs/sidebars.js
+-rw-r--r--   0        0        0     1721 2024-04-16 12:12:31.287531 therix-0.1.4/therix/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      181 2024-05-03 05:53:02.654898 therix-0.1.4/therix/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     2282 2024-05-03 05:53:02.655058 therix-0.1.4/therix/docs/src/css/custom.css
+-rw-r--r--   0        0        0      365 2024-04-16 12:12:31.288118 therix-0.1.4/therix/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0      118 2024-04-16 12:12:31.288266 therix-0.1.4/therix/docs/src/pages/markdown-page.md
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.288338 therix-0.1.4/therix/docs/static/.nojekyll
+-rw-r--r--   0        0        0    21038 2024-04-16 12:12:31.288709 therix-0.1.4/therix/docs/static/img/coditas.png
+-rw-r--r--   0        0        0     5277 2024-04-16 12:12:31.289101 therix-0.1.4/therix/docs/static/img/coditasLogo.svg
+-rw-r--r--   0        0        0    55746 2024-04-16 12:12:31.289498 therix-0.1.4/therix/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0     5142 2024-04-16 12:12:31.289848 therix-0.1.4/therix/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0     3902 2024-05-03 05:53:02.655308 therix-0.1.4/therix/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655524 therix-0.1.4/therix/docs/static/img/icon.svg
+-rw-r--r--   0        0        0      996 2024-05-03 05:53:02.655671 therix-0.1.4/therix/docs/static/img/logo.png
+-rw-r--r--   0        0        0      553 2024-05-03 05:53:02.655859 therix-0.1.4/therix/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     2713 2024-05-03 05:53:02.656025 therix-0.1.4/therix/docs/static/img/therix-logo.png
+-rw-r--r--   0        0        0    31486 2024-04-16 12:12:31.290706 therix-0.1.4/therix/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-r--r--   0        0        0    36002 2024-04-16 12:12:31.290979 therix-0.1.4/therix/docs/static/img/undraw_docusaurus_react.svg
+-rw-r--r--   0        0        0    11887 2024-04-16 12:12:31.291206 therix-0.1.4/therix/docs/static/img/undraw_docusaurus_tree.svg
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291242 therix-0.1.4/therix/entities/__init__.py
+-rw-r--r--   0        0        0     2535 2024-05-03 12:50:17.297755 therix-0.1.4/therix/entities/models.py
+-rw-r--r--   0        0        0     2490 2024-05-08 11:24:55.873082 therix-0.1.4/therix/examples/cache_config_example.py
+-rw-r--r--   0        0        0     1745 2024-05-08 11:24:55.873332 therix-0.1.4/therix/examples/pii_filter_example.py
+-rw-r--r--   0        0        0     6206 2024-05-08 11:24:55.873927 therix-0.1.4/therix/examples/summarizer_example.py
+-rw-r--r--   0        0        0    21547 2024-04-26 09:41:57.773928 therix-0.1.4/therix/pylintrc
+-rw-r--r--   0        0        0        0 2024-04-16 12:12:31.291387 therix-0.1.4/therix/services/__init__.py
+-rw-r--r--   0        0        0     4434 2024-05-09 12:03:21.346863 therix-0.1.4/therix/services/pipeline_service.py
+-rw-r--r--   0        0        0     1434 2024-04-16 12:12:31.291740 therix-0.1.4/therix/services/web_crawling.py
+-rw-r--r--   0        0        0      602 2024-05-08 11:24:55.874269 therix-0.1.4/therix/tests/test_pii_filter.py
+-rw-r--r--   0        0        0      812 2024-04-26 09:41:57.774428 therix-0.1.4/therix/utils/pii_filter.py
+-rw-r--r--   0        0        0    10916 2024-05-09 12:03:21.347328 therix-0.1.4/therix/utils/rag.py
+-rw-r--r--   0        0        0     4074 2024-05-08 11:24:55.875542 therix-0.1.4/therix/utils/summarizer.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 therix-0.1.4/PKG-INFO
```

### Comparing `therix-0.1.3/LICENSE` & `therix-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/README.md` & `therix-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/pyproject.toml` & `therix-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "therix"
-version = "0.1.3"
+version = "0.1.4"
 description = "Therix is the SDK for langchain based applications."
 authors = ["Ajinath"]
 license = "MIT"
 readme = "README.md"
 include = ["alembic/**/*", "alembic.ini"]
 
 [tool.poetry.dependencies]
```

### Comparing `therix-0.1.3/therix/alembic/env.py` & `therix-0.1.4/therix/alembic/env.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/alembic/script.py.mako` & `therix-0.1.4/therix/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py` & `therix-0.1.4/therix/alembic/versions/2024_04_26_0914-739c7981bdd8_added_config_type_for_cache_config.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py` & `therix-0.1.4/therix/alembic/versions/2024_04_26_1644-b8fe483b5a71_add_type_column_in_pipeline_table.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py` & `therix-0.1.4/therix/alembic/versions/f5fb392e6b0a_initial_database_setup.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/alembic.ini` & `therix-0.1.4/therix/alembic.ini`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/core/JSONLoader.py` & `therix-0.1.4/therix/core/JSONLoader.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/core/cache.py` & `therix-0.1.4/therix/core/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,15 @@
         session = db_manager.get_session()
         query = session.query(FulltextLLMCache).filter(
             FulltextLLMCache.question == question,
             FulltextLLMCache.pipeline_id == pipeline_id
         )
         result = query.first()
         session.close()
-        return result
-        
+        return result.response
         
     
     
     def update(self, prompt: str, llm_string: str, answer, pipeline_id: str) -> None:
         session = db_manager.get_session()
         cache_entry = FulltextLLMCache(
             question=prompt,
```

### Comparing `therix-0.1.3/therix/core/chat_history/base_chat_history.py` & `therix-0.1.4/therix/core/chat_history/base_chat_history.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/core/constants.py` & `therix-0.1.4/therix/core/constants.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/core/data_sources.py` & `therix-0.1.4/therix/core/data_sources.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/core/embedding_models.py` & `therix-0.1.4/therix/core/embedding_models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/core/inference_models.py` & `therix-0.1.4/therix/core/inference_models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/core/pipeline.py` & `therix-0.1.4/therix/core/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     def load(self, pipeline_id):
         self.pipeline_data = self.pipeline_service.get_pipeline(pipeline_id)
         self.id = self.pipeline_data.id
         self.name = self.pipeline_data.name
         return self.pipeline_data
 
     def preprocess_data(self):
-        self.pipeline_service.preprocess_data(self.pipeline_data.id)
+       return self.pipeline_service.preprocess_data(self.pipeline_data.id)
 
     def invoke(self, question, session_id=None):
             cached_response = None
             therix_cache = TherixCache(engine)
             inference_model = self.pipeline_service.get_pipeline_configuraitons_by_type(self.pipeline_data.id, ConfigType.INFERENCE_MODEL)
 
             if session_id is None:
@@ -111,16 +111,15 @@
             pipeline_type = self.pipeline_service.get_pipeline(self.pipeline_data.id).type.value
             model_response = ModelResponse()
 
             if pipeline_type == PipelineTypeMaster.RAG.value:
                 if add_cache:
                     cached_response = therix_cache.lookup(question, inference_model[0].name, self.pipeline_data.id)
                 if cached_response:
-                    print("from cache", cached_response)
-                    return ModelResponse(cached_response.response, session_id).create_response
+                    return ModelResponse(cached_response, session_id).create_response()
                 answer = self.pipeline_service.invoke_pipeline(
                     self.pipeline_data.id, question, session_id, trace_details
                 )
                 if add_cache:
                     therix_cache.update(question, inference_model[0].name, answer, self.pipeline_data.id)
             elif pipeline_type == PipelineTypeMaster.SUMMARIZER.value:
                 answer = self.pipeline_service.invoke_summarizer_pipeline(self.pipeline_data.id, text=question)
```

### Comparing `therix-0.1.3/therix/core/pipeline_component.py` & `therix-0.1.4/therix/core/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/core/summarizer_config.py` & `therix-0.1.4/therix/core/summarizer_config.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/db/db_manager.py` & `therix-0.1.4/therix/db/db_manager.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/db/tests/test_db_manager.py` & `therix-0.1.4/therix/db/tests/test_db_manager.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/README.md` & `therix-0.1.4/therix/docs/README.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/blog/2019-05-29-long-blog-post.md` & `therix-0.1.4/therix/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `therix-0.1.4/therix/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/blog/2021-08-26-welcome/index.md` & `therix-0.1.4/therix/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/docs/introduction/getting-started.md` & `therix-0.1.4/therix/docs/docs/introduction/getting-started.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/docs/introduction/index.md` & `therix-0.1.4/therix/docs/docs/introduction/index.md`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/docs/use-cases/summarizer_doc.md` & `therix-0.1.4/therix/docs/docs/use-cases/summarizer.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,89 @@
 ---
 slug: /use-cases/summarizer
 sidebar_position: 2
 ---
 
 # Summarizer
 
-In Therix, the "Summarizer" topic serves as a fundamental component designed to condense lengthy texts into concise summaries. This versatile tool streamlines information retrieval and aids in comprehension across various applications.
+The Summarizer tool in Therix condenses lengthy texts into concise summaries. It analyzes documents, extracts key information, and generates coherent summaries, enabling users to grasp core content efficiently.
 
-Within the realm of the Summarizer topic, we delve into two distinct methodologies: "Extractive" and "Abstractive" summarization techniques. These approaches cater to different use cases and preferences, offering flexibility and precision in summarization tasks.
+The Summarizer uses two main methods: "Extractive" and "Abstractive" summarization. They work differently but both help make summaries, depending on what you need.
 
-**Steps to follow:**
+## Summarizer - Abtractive
 
-Import Necessary Modules: Begin by importing the required modules for configuring the Summarizer.
+Abstractive Summarization in Therix is a smart way to make short summaries from long texts. Unlike Extractive Summarization that just rearranges the text, Abstractive Summarization really understands the text. It figures out the main ideas and context, then writes original summaries that capture those ideas in a new way.
 
+This method lets you be creative in summarizing and isn't limited by how the original text is structured. Abstractive Summarization is great for simplifying complex information, making it easier to understand for making decisions and sharing knowledge in different areas.
+
+**Sample Output:**
+```python
+{'answer': '\nBeets are a root vegetable rich in fiber, folate, manganese, and antioxidants, and can improve athletic performance and reduce blood pressure. More research is needed to fully understand their health benefits.', 'session_id': UUID('b9548328-6982-40e9-9cea-06208090f25f')}
+```
+
+## Summarizer - Extractive
+
+In the Extractive Summarizer of Therix, the aim is to make a brief summary of a text in a JSON format. It picks out important sentences or phrases from the text and puts them in a structured way in JSON.
+
+If you don't specify a Pydantic model, the system itself decides how to organize the summary in JSON, making sure it's clear and concise.
+But users can also give a Pydantic model to customize how the information is organized in the JSON. This gives more control over how the summary looks.
+
+Whether using the default JSON setup or a customized Pydantic model, the result is a neat and informative summary in JSON. This helps in understanding big chunks of text quickly and making decisions based on them in different fields.
+
+The sample model used here is extended from the BaseModel of Pydantic.
+```python
+from langchain_core.pydantic_v1 import BaseModel
+
+class TopicModel(BaseModel):
+    mainTopic: str
+    subTopic1: str
+    subTopic2: str
+```
+
+**Sample Output:**
+```python
+{'answer': {"mainTopic": "Superfoods", "subTopic1": "Health Benefits", "subTopic2": "10 Superfoods"} , 'session_id': UUID('3f2d3cef-8091-4e0d-accd-71b6387938c7')}
 ```
+
+## How you can integrate summarizer in your code:
+
+- Import Necessary Modules: Begin by importing the required modules for configuring the Summarizer.
+
+```python
 from therix.summarizer import SummarizerConfig, SummarizerTypeMaster
 from your_model_module import TopicModel  # Import your Pydantic model if needed
 ```
 
-Instantiate SummarizerConfig:
+- Instantiate SummarizerConfig:
 
 Create an instance of the SummarizerConfig class by specifying the type of summarizer and, optionally, the Pydantic model for structuring the JSON output.
 
-**For Extractive Summarizer with custom Pydantic model**
-```
+- **For Extractive Summarizer with custom Pydantic model**
+```python
 summarizer_config = SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE.value, TopicModel)
 ```
 
-**For Abstractive Summarizer**
-```
+- **For Abstractive Summarizer**
+```python
 summarizer_config = SummarizerConfig(SummarizerTypeMaster.ABSTRACTIVE.value)
 ```
 
-Add Summarizer Configuration to Pipeline: Use the .add() method to add the SummarizerConfig to your Therix pipeline.
+- Add Summarizer Configuration to Pipeline: Use the .add() method to add the SummarizerConfig to your Therix pipeline.
 
-```
+```python
 pipeline.add(summarizer_config)
 ```
 
-# Example
+## Example
 
-```
+```python
 pipeline = Pipeline(name="Summarizer Pipeline")
     (pipeline
     .add(SummarizerConfig(SummarizerTypeMaster.EXTRACTIVE.value,TopicModel))
     .add(// Any other configuration you want to add)
     .save())
 
     pipeline.publish()
-    print(pipeline.id)
-    ans = pipeline.invoke(text,'SUMMARIZER')
+    answer = pipeline.invoke(text)
 ```
 
 By following these steps and adjusting the parameters as needed, you can seamlessly integrate the Summarizer into your Therix pipeline. Whether you require Extractive or Abstractive summarization, with or without a custom Pydantic model, Therix provides the flexibility and functionality to meet your summarization needs effectively.
-
-# Summarizer - Extractive
-
-In the Extractive Summarizer type of Therix, the primary goal is to distill the essence of a given text into a JSON format while maintaining the integrity of the original content. This process involves selecting key sentences or phrases from the input text that encapsulate its main ideas and conveying them in a structured JSON representation. 
-
-When utilizing the Extractive Summarizer without specifying a Pydantic model, the system employs an internal logic to generate a JSON structure suitable for the content. This structure aims to organize the extracted information in a coherent manner, ensuring that the resulting JSON format provides a concise yet informative summary of the input text.
-
-However, users also have the option to supply a Pydantic model to customize the structure of the extracted information according to their specific requirements. By providing a Pydantic model, users can define the fields and data types they wish to include in the JSON output, allowing for greater flexibility and control over the summarization process.
-
-Whether utilizing the default JSON structure generated by the Extractive Summarizer or supplying a custom Pydantic model, the end result is a well-organized and informative summary in JSON format that captures the key elements of the input text. This capability enables users to easily extract valuable insights from large volumes of text data, facilitating decision-making and information retrieval across various domains.
-
-# Summarizer - Abtractive
-
-Abstractive Summarization in Therix is a sophisticated technique that simplifies text into concise summaries. Unlike Extractive Summarization, which rearranges existing content, Abstractive Summarization goes a step further. It understands the input text deeply, grasping its meaning, context, and core ideas. By doing so, it generates original summaries that capture the essence of the text in a new way. This method allows for creativity in summarizing, providing summaries that are not limited by the original text's structure. Abstractive Summarization is valuable for distilling complex information into easy-to-understand summaries, making it useful for decision-making and knowledge sharing in various fields.
```

### Comparing `therix-0.1.3/therix/docs/docusaurus.config.js` & `therix-0.1.4/therix/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/package-lock.json` & `therix-0.1.4/therix/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/package.json` & `therix-0.1.4/therix/docs/package.json`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/sidebars.js` & `therix-0.1.4/therix/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/src/components/HomepageFeatures/index.js` & `therix-0.1.4/therix/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/src/css/custom.css` & `therix-0.1.4/therix/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/coditas.png` & `therix-0.1.4/therix/docs/static/img/coditas.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/coditasLogo.svg` & `therix-0.1.4/therix/docs/static/img/coditasLogo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/docusaurus-social-card.jpg` & `therix-0.1.4/therix/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/docusaurus.png` & `therix-0.1.4/therix/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/favicon.ico` & `therix-0.1.4/therix/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/icon.svg` & `therix-0.1.4/therix/docs/static/img/icon.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/logo.png` & `therix-0.1.4/therix/docs/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/logo.svg` & `therix-0.1.4/therix/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/therix-logo.png` & `therix-0.1.4/therix/docs/static/img/therix-logo.png`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/undraw_docusaurus_mountain.svg` & `therix-0.1.4/therix/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/undraw_docusaurus_react.svg` & `therix-0.1.4/therix/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/docs/static/img/undraw_docusaurus_tree.svg` & `therix-0.1.4/therix/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/entities/models.py` & `therix-0.1.4/therix/entities/models.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/pylintrc` & `therix-0.1.4/therix/pylintrc`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/services/pipeline_service.py` & `therix-0.1.4/therix/services/pipeline_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,27 +64,28 @@
             website_url = data_sources[0].config["website"]
             web_content = crawl_website(website_url)
             domain_name = urllib.parse.urlparse(website_url).netloc
             output_file = f"{domain_name}_data.json"
             with open(output_file, "w") as f:
                 json.dump(web_content, f, indent=4)
             data_sources[0].config["files"] = [output_file]
+        if "website" in data_sources[0].config:
+            os.remove(output_file)
         embedding_model = self.get_pipeline_configuraitons_by_type(
             pipeline_id, "EMBEDDING_MODEL"
         )
-        create_embeddings(data_sources, embedding_model[0], str(pipeline_id))
-        if "website" in data_sources[0].config:
-            os.remove(output_file)
+        return create_embeddings(data_sources, embedding_model[0], str(pipeline_id))
 
     def invoke_pipeline(self, pipeline_id, question, session_id, trace_details=None):
         embedding_model = self.get_pipeline_configuraitons_by_type(
             pipeline_id, "EMBEDDING_MODEL"
         )
         store = get_vectorstore(embedding_model[0], str(pipeline_id))
         retreiver = store.as_retriever()
+
         inference_model = self.get_pipeline_configuraitons_by_type(
             pipeline_id, "INFERENCE_MODEL"
         )
         result = chat(
             question,
             retreiver,
             inference_model[0],
```

### Comparing `therix-0.1.3/therix/services/web_crawling.py` & `therix-0.1.4/therix/services/web_crawling.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/utils/pii_filter.py` & `therix-0.1.4/therix/utils/pii_filter.py`

 * *Files identical despite different names*

### Comparing `therix-0.1.3/therix/utils/rag.py` & `therix-0.1.4/therix/utils/rag.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json
+import json, uuid
 from operator import itemgetter
 from pathlib import Path
 from urllib import response
 from langchain.docstore.document import Document
 from langchain_community.document_loaders import TextLoader, PyPDFLoader
 from langchain_community.vectorstores.pgvector import PGVector
 from langchain_openai import OpenAIEmbeddings, ChatOpenAI
@@ -154,24 +154,32 @@
             region_name=config["bedrock_region_name"],
         )
     else:
         raise ValueError(f"Unknown inference model: {inference_model_name}")
 
 
 def create_embeddings(data_sources, embedding_model, collection_name):
+
     store = get_vectorstore(embedding_model, collection_name)
+    doc_id = uuid.uuid4()
     for data_source in data_sources:
         # data_source = {'name': 'PDF', 'config': {'files': ['path/to/file', 'path/to/file']}}
         for file_path in data_source.config["files"]:
             loader = get_loader(data_source.name, file_path, data_source.config)
+            extra_metadata = [
+                ("configId", str(doc_id)),
+            ]
             pages = loader.load_and_split()
+            for page_content in pages:
+                for key, value in extra_metadata:
+                    page_content.metadata[key] = value
+            # document.text = mask_data(document.text)
             # text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=0)
-
             store.add_documents(pages)
-            return "embedding created"
+            return {"message" : "embedding created" , "config_id" : str(doc_id)}
 
 
 def get_vectorstore(embedding_model, collection_name):
     embeddings = get_embedding_model(embedding_model.name, embedding_model.config)
     store = PGVector(
         collection_name=collection_name,
         connection_string=SQLALCHEMY_DATABASE_URL,
@@ -186,16 +194,15 @@
     inference_model,
     embed_model,
     session_id,
     pipeline_id,
     trace_details=None,
 ):
 
-    print(trace_details)
-
+    # print(trace_details)
     chain_callbacks = []
     if trace_details is not None:
         langfuse_handler = CallbackHandler(
             secret_key=trace_details["secret_key"],
             public_key=trace_details["public_key"],
             host=trace_details["host"],
             trace_name=trace_details["identifier"],
@@ -206,29 +213,31 @@
         str(session_id),
         str(pipeline_id),
         SQLALCHEMY_DATABASE_URL,
         table_name="chat_history",
     )
     chat_history = history.messages
 
-    template = """Answer the question based only on the following context:
-                     {context}
+    template = """Answer the question based only on the following context and do not reply anything that is out of context, reply with "I am sorry, I cannot help you with that" and do not add any more message to it.
+    Context: 
+    {context}
 
-                    Question: {question}
-                    """
+    Question: {question}
+    """
     ANSWER_PROMPT = ChatPromptTemplate.from_template(template)
     _template = """Given the following conversation and a follow up question, rephrase the follow up question to be a standalone question, in its original language.
                     Chat History:
                     {chat_history}
                     Follow Up Input: {question}
                     Standalone question:"""
 
     CONDENSE_QUESTION_PROMPT = PromptTemplate.from_template(_template)
     DEFAULT_DOCUMENT_PROMPT = PromptTemplate.from_template(template="{page_content}")
 
+
     def _combine_documents(
         docs, document_prompt=DEFAULT_DOCUMENT_PROMPT, document_separator="\n\n"
     ):
         doc_strings = [format_document(doc, document_prompt) for doc in docs]
         return document_separator.join(doc_strings)
 
     model = get_inference_model(inference_model.name, inference_model.config)
@@ -243,15 +252,16 @@
     )
     _context = {
         "context": itemgetter("standalone_question") | retriever | _combine_documents,
         "question": lambda x: x["standalone_question"],
     }
     conversational_qa_chain = _inputs | _context | ANSWER_PROMPT | model
     result = conversational_qa_chain.invoke(
-        {"question": question, "chat_history": chat_history}
+        {"question": question, "chat_history": chat_history},
+        config={"callbacks": [langfuse_handler]}
     )
     
     response=json.loads(result.json())["content"]
     
     history.add_message("user",question,pipeline_id,session_id)
     history.add_message("system",response,pipeline_id,session_id)
     return response
```

### Comparing `therix-0.1.3/therix/utils/summarizer.py` & `therix-0.1.4/therix/utils/summarizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from enum import Enum
+import json
 from therix.utils.rag import get_inference_model
 from langchain.chains.llm import LLMChain
 from langchain_core.prompts import PromptTemplate
 from langchain.chains.combine_documents.stuff import StuffDocumentsChain
 from langchain.text_splitter import CharacterTextSplitter
 from langchain.docstore.document import Document
 from langchain.chains import (
@@ -99,11 +100,11 @@
         template=PROMPT_TEMPLATE[summarization_type],
         input_variables=["context"],
         partial_variables={"response_schema_json": pydantic_prompt},
     )
     
     if summarization_type == SummarizerTypeMaster.EXTRACTIVE.value:
         chain = prompt | llm | parser
-        return  chain.invoke({"context": summary})
+        return json.dumps(chain.invoke({"context": summary}))
     else:
         chain = prompt | llm
         return  chain.invoke({"context": summary}).content
```

### Comparing `therix-0.1.3/PKG-INFO` & `therix-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: therix
-Version: 0.1.3
+Version: 0.1.4
 Summary: Therix is the SDK for langchain based applications.
 License: MIT
 Author: Ajinath
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
```


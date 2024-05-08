# Comparing `tmp/sageworks-0.6.1.tar.gz` & `tmp/sageworks-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.6.1.tar", last modified: Tue Apr 23 23:36:08 2024, max compression
+gzip compressed data, was "sageworks-0.6.2.tar", last modified: Wed May  8 22:04:08 2024, max compression
```

## Comparing `sageworks-0.6.1.tar` & `sageworks-0.6.2.tar`

### file list

```diff
@@ -1,540 +1,552 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.067395 sageworks-0.6.1/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.008852 sageworks-0.6.1/.github/
--rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.1/.github/dependabot.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.009121 sageworks-0.6.1/.github/workflows/
--rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.1/.github/workflows/deploy-docs.yml
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.1/.github/workflows/python-lint.yml
--rw-r--r--   0 briford    (501) staff       (20)     2008 2023-12-24 17:18:24.000000 sageworks-0.6.1/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.1/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.1/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.1/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     4117 2024-04-23 23:36:08.067330 sageworks-0.6.1/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     2694 2024-04-16 15:58:18.000000 sageworks-0.6.1/README.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.1/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:07.999337 sageworks-0.6.1/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.010309 sageworks-0.6.1/applications/aws_dashboard/
--rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-23 22:25:52.000000 sageworks-0.6.1/applications/aws_dashboard/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.1/applications/aws_dashboard/Dockerfile_plugins
--rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.1/applications/aws_dashboard/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.1/applications/aws_dashboard/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.010958 sageworks-0.6.1/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.1/applications/aws_dashboard/assets/bootstrap_darkly.min.css
--rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.1/applications/aws_dashboard/assets/default.css
--rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.1/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.1/applications/aws_dashboard/assets/trash.png
--rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-23 23:26:58.000000 sageworks-0.6.1/applications/aws_dashboard/dashboard
--rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.1/applications/aws_dashboard/nginx.conf
--rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.1/applications/aws_dashboard/open_source_config.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:07.999258 sageworks-0.6.1/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.011346 sageworks-0.6.1/applications/aws_dashboard/pages/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.1/applications/aws_dashboard/pages/data_sources/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.1/applications/aws_dashboard/pages/data_sources/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.1/applications/aws_dashboard/pages/data_sources/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.011751 sageworks-0.6.1/applications/aws_dashboard/pages/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)     4212 2024-04-16 15:58:18.000000 sageworks-0.6.1/applications/aws_dashboard/pages/endpoints/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.1/applications/aws_dashboard/pages/endpoints/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2458 2024-04-23 23:23:47.000000 sageworks-0.6.1/applications/aws_dashboard/pages/endpoints/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.012143 sageworks-0.6.1/applications/aws_dashboard/pages/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.1/applications/aws_dashboard/pages/feature_sets/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.1/applications/aws_dashboard/pages/feature_sets/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.1/applications/aws_dashboard/pages/feature_sets/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.012525 sageworks-0.6.1/applications/aws_dashboard/pages/main/
--rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.1/applications/aws_dashboard/pages/main/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2899 2024-03-28 17:23:43.000000 sageworks-0.6.1/applications/aws_dashboard/pages/main/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.1/applications/aws_dashboard/pages/main/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.012926 sageworks-0.6.1/applications/aws_dashboard/pages/models/
--rw-r--r--   0 briford    (501) staff       (20)     3954 2024-04-23 23:23:47.000000 sageworks-0.6.1/applications/aws_dashboard/pages/models/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2132 2024-04-16 15:58:18.000000 sageworks-0.6.1/applications/aws_dashboard/pages/models/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2152 2024-04-23 23:23:47.000000 sageworks-0.6.1/applications/aws_dashboard/pages/models/page.py
--rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-06 16:51:44.000000 sageworks-0.6.1/applications/aws_dashboard/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.1/applications/aws_dashboard/supervisord.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:07.999390 sageworks-0.6.1/applications/experiments/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.013799 sageworks-0.6.1/applications/experiments/compound_explorer/
--rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.1/applications/experiments/compound_explorer/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.1/applications/experiments/compound_explorer/README.md
--rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.1/applications/experiments/compound_explorer/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.014068 sageworks-0.6.1/applications/experiments/compound_explorer/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.1/applications/experiments/compound_explorer/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.1/applications/experiments/compound_explorer/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.1/applications/experiments/compound_explorer/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.1/applications/experiments/compound_explorer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.1/applications/experiments/compound_explorer/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.014483 sageworks-0.6.1/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/aws_identity_check.py
--rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.014615 sageworks-0.6.1/aws_setup/event_bridge/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/event_bridge/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.015158 sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/cdk.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.015318 sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/lambda/
--rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
--rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.016269 sageworks-0.6.1/aws_setup/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_core/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_core/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_core/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_core/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_core/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.1/aws_setup/sageworks_core/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.016521 sageworks-0.6.1/aws_setup/sageworks_core/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/aws_setup/sageworks_core/sageworks_core/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_core/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.016678 sageworks-0.6.1/aws_setup/sageworks_core/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_core/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.016892 sageworks-0.6.1/aws_setup/sageworks_core/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_core/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.017814 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.018041 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-16 15:58:18.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.018170 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.018374 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.019014 sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.019240 sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-23 22:32:55.000000 sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.019826 sageworks-0.6.1/data/
--rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.1/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.1/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.1/data/test_data.json
--rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.1/data/wine_dataset.csv
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.019958 sageworks-0.6.1/docs/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.020222 sageworks-0.6.1/docs/admin/
--rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.1/docs/admin/docker_push.md
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/admin/pypi_release.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.021255 sageworks-0.6.1/docs/api_classes/
--rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.1/docs/api_classes/data_source.md
--rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/api_classes/endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/api_classes/feature_set.md
--rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.1/docs/api_classes/meta.md
--rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/api_classes/model.md
--rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/api_classes/monitor.md
--rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/api_classes/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.1/docs/api_classes/pipelines.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.022032 sageworks-0.6.1/docs/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/aws_setup/aws_access_management.md
--rw-r--r--   0 briford    (501) staff       (20)     7836 2024-01-23 15:36:53.000000 sageworks-0.6.1/docs/aws_setup/aws_tips_and_tricks.md
--rw-r--r--   0 briford    (501) staff       (20)     4229 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/aws_setup/core_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/aws_setup/dashboard_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.1/docs/aws_setup/full_pipeline.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.022188 sageworks-0.6.1/docs/concepts/
--rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.6.1/docs/concepts/model_monitoring.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.022346 sageworks-0.6.1/docs/core_classes/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.023594 sageworks-0.6.1/docs/core_classes/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.1/docs/core_classes/artifacts/artifact.md
--rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/artifacts/athena_source.md
--rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.1/docs/core_classes/artifacts/data_source_abstract.md
--rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/artifacts/endpoint_core.md
--rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/artifacts/feature_set_core.md
--rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/artifacts/model_core.md
--rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/artifacts/monitor_core.md
--rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/artifacts/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.024815 sageworks-0.6.1/docs/core_classes/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/transforms/data_loaders_heavy.md
--rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/transforms/data_loaders_light.md
--rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/core_classes/transforms/data_to_features.md
--rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/transforms/features_to_model.md
--rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/transforms/model_to_endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/core_classes/transforms/overview.md
--rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.1/docs/core_classes/transforms/pandas_transforms.md
--rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.1/docs/core_classes/transforms/transform.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.024962 sageworks-0.6.1/docs/glue/
--rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/glue/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.027163 sageworks-0.6.1/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.1/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)     3417 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.027861 sageworks-0.6.1/docs/misc/
--rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/misc/faq.md
--rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/misc/general_info.md
--rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/misc/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.1/docs/misc/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.028132 sageworks-0.6.1/docs/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.1/docs/plugins/index.md
--rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.1/docs/plugins/plugin_api_changes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.028278 sageworks-0.6.1/docs/repl/
--rw-r--r--   0 briford    (501) staff       (20)     2081 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/repl/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.028560 sageworks-0.6.1/docs/research/
--rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/research/eda.md
--rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.1/docs/research/htg.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.028690 sageworks-0.6.1/examples/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.028820 sageworks-0.6.1/examples/ag-grid/
--rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.1/examples/ag-grid/hello_world.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.029509 sageworks-0.6.1/examples/datasource/
--rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.1/examples/datasource/datasource_from_df.py
--rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.1/examples/datasource/datasource_from_s3.py
--rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.1/examples/datasource/datasource_query.py
--rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.1/examples/datasource/datasource_stats.py
--rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.1/examples/datasource/datasource_to_featureset.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.029925 sageworks-0.6.1/examples/endpoint/
--rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.1/examples/endpoint/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/endpoint/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.1/examples/endpoint/endpoint_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.030362 sageworks-0.6.1/examples/featureset/
--rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.1/examples/featureset/featureset_eda.py
--rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/featureset/featureset_query.py
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.1/examples/featureset/featureset_to_model.py
--rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/full_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.030789 sageworks-0.6.1/examples/glue/
--rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.1/examples/glue/glue_hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.1/examples/glue/glue_hello_world_with_log.py
--rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.1/examples/glue/glue_load_s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.031202 sageworks-0.6.1/examples/meta/
--rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.1/examples/meta/meta_list_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.1/examples/meta/meta_list_models.py
--rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.1/examples/meta/meta_model_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.031458 sageworks-0.6.1/examples/model/
--rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/model/model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.1/examples/model/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.031733 sageworks-0.6.1/examples/monitor/
--rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.1/examples/monitor/monitor_setup.py
--rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.1/examples/monitor/monitor_usage.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.032528 sageworks-0.6.1/examples/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.1/examples/pipelines/abalone_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.1/examples/pipelines/abalone_pipeline_v2.json
--rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.1/examples/pipelines/aqsol_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.1/examples/pipelines/pipeline_details.py
--rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.1/examples/pipelines/pipeline_execute.py
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.1/examples/pipelines/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.002605 sageworks-0.6.1/examples/plugins/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.033066 sageworks-0.6.1/examples/plugins/pages/
--rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.1/examples/plugins/pages/my_plugin_page.py
--rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.1/examples/plugins/pages/plugin_page_1.py
--rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.1/examples/plugins/pages/plugin_page_2.py
--rw-r--r--   0 briford    (501) staff       (20)     4528 2024-04-16 15:58:18.000000 sageworks-0.6.1/examples/plugins/pages/plugin_page_3.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.033352 sageworks-0.6.1/examples/plugins/views/
--rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.1/examples/plugins/views/model_plugin_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.1/examples/plugins/views/my_view_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.034013 sageworks-0.6.1/examples/plugins/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.1/examples/plugins/web_components/custom_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.1/examples/plugins/web_components/endpoint_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.1/examples/plugins/web_components/endpoint_turbo.py
--rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.1/examples/plugins/web_components/model_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.1/examples/plugins/web_components/model_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.034649 sageworks-0.6.1/examples/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.1/examples/storage/data_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.1/examples/storage/data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/hello_world_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.1/examples/storage/plugin_page_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.035039 sageworks-0.6.1/examples/storage/sagemaker_pipelines/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/sagemaker_pipelines/all_steps.py
--rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/sagemaker_pipelines/hello.py
--rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/sagemaker_pipelines/ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.002873 sageworks-0.6.1/examples/storage/sagemaker_pipelines/storage/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.035709 sageworks-0.6.1/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.1/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
--rw-r--r--   0 briford    (501) staff       (20)     2792 2024-04-16 21:08:28.000000 sageworks-0.6.1/mkdocs.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.036448 sageworks-0.6.1/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.6.1/notebooks/ML_Pipeline_with_SageWorks.ipynb
--rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.6.1/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
--rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.6.1/notebooks/Outliers_in_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.038017 sageworks-0.6.1/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.1/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.1/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.1/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.1/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.1/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.1/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-06 16:51:44.000000 sageworks-0.6.1/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.039388 sageworks-0.6.1/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.1/scripts/ag_table_row_selection.py
--rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.1/scripts/athena_ddl_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.1/scripts/copy_data_catalog_db.py
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.1/scripts/create_glue_workflow_with_trigger.py
--rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.1/scripts/delete_redis_keys.py
--rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.1/scripts/glue_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.1/scripts/model_endpoint_sanity_check.py
--rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.1/scripts/onboard_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.1/scripts/onboard_models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.039644 sageworks-0.6.1/scripts/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.1/scripts/storage/dns_data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.1/scripts/storage/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.1/scripts/test_feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)      533 2024-04-23 23:36:08.067732 sageworks-0.6.1/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.6.1/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.003332 sageworks-0.6.1/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.039777 sageworks-0.6.1/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.040834 sageworks-0.6.1/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.1/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.041791 sageworks-0.6.1/src/sageworks/algorithms/dataframe/
--rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.1/src/sageworks/algorithms/dataframe/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/dataframe/aggregation.py
--rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/dataframe/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
--rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/dataframe/feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/dataframe/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/dataframe/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.003665 sageworks-0.6.1/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.041921 sageworks-0.6.1/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.1/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.042051 sageworks-0.6.1/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.1/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.042182 sageworks-0.6.1/src/sageworks/algorithms/spark/
--rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.1/src/sageworks/algorithms/spark/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.043153 sageworks-0.6.1/src/sageworks/algorithms/sql/
--rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.1/src/sageworks/algorithms/sql/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/sql/column_stats.py
--rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/sql/correlations.py
--rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/sql/descriptive_stats.py
--rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/sql/outliers.py
--rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/sql/sample_rows.py
--rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/algorithms/sql/value_counts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.044397 sageworks-0.6.1/src/sageworks/api/
--rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.1/src/sageworks/api/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/api/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/api/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/api/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.1/src/sageworks/api/meta.py
--rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/api/model.py
--rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/api/monitor.py
--rw-r--r--   0 briford    (501) staff       (20)     7016 2024-04-22 20:46:36.000000 sageworks-0.6.1/src/sageworks/api/pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     6731 2024-04-19 14:53:21.000000 sageworks-0.6.1/src/sageworks/api/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.044673 sageworks-0.6.1/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)    10908 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.045775 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.045921 sageworks-0.6.1/src/sageworks/core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.047194 sageworks-0.6.1/src/sageworks/core/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.1/src/sageworks/core/artifacts/artifact.py
--rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/core/artifacts/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/artifacts/data_source_abstract.py
--rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/artifacts/data_source_factory.py
--rw-r--r--   0 briford    (501) staff       (20)    36630 2024-04-21 18:44:59.000000 sageworks-0.6.1/src/sageworks/core/artifacts/endpoint_core.py
--rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.1/src/sageworks/core/artifacts/feature_set_core.py
--rw-r--r--   0 briford    (501) staff       (20)    35498 2024-04-22 20:58:40.000000 sageworks-0.6.1/src/sageworks/core/artifacts/model_core.py
--rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/artifacts/monitor_core.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.047333 sageworks-0.6.1/src/sageworks/core/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     6928 2024-04-22 20:46:36.000000 sageworks-0.6.1/src/sageworks/core/pipelines/pipeline_executor.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.047708 sageworks-0.6.1/src/sageworks/core/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.047842 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.048080 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.048642 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.048794 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.048963 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.049090 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.049261 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.049752 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.049915 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.050033 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.050250 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/chunk/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.050400 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.050548 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.050693 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/storage/
--rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.051077 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.051223 sageworks-0.6.1/src/sageworks/core/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.005603 sageworks-0.6.1/src/sageworks/core/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.051334 sageworks-0.6.1/src/sageworks/core/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.051467 sageworks-0.6.1/src/sageworks/core/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.051709 sageworks-0.6.1/src/sageworks/core/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.051995 sageworks-0.6.1/src/sageworks/core/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.1/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.052246 sageworks-0.6.1/src/sageworks/core/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/core/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.053123 sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
--rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/core/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.053275 sageworks-0.6.1/src/sageworks/experiments/
--rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/experiments/view_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.053528 sageworks-0.6.1/src/sageworks/repl/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/repl/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.1/src/sageworks/repl/sageworks_shell.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.053791 sageworks-0.6.1/src/sageworks/resources/
--rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.1/src/sageworks/resources/open_source_api.key
--rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/resources/signature_verify_pub.pem
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.058148 sageworks-0.6.1/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.1/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/utils/aws_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/chem_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/utils/config_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/dashboard_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/utils/datetime_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/docker_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.1/src/sageworks/utils/ecs_info.py
--rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/endpoint_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/extract_model_artifact.py
--rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/glue_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5757 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/license_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/utils/markdown_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.1/src/sageworks/utils/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/utils/plugin_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/repl_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/s3_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/sageworks_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/sageworks_sqs.py
--rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.1/src/sageworks/utils/symbols.py
--rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/test_data_generator.py
--rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.1/src/sageworks/utils/trace_calls.py
--rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/utils/type_abbrev.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.059162 sageworks-0.6.1/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.1/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     7008 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/views/endpoint_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/views/feature_set_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/views/model_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.061002 sageworks-0.6.1/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     5862 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/component_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/correlation_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/web_components/data_details_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-06 16:51:44.000000 sageworks-0.6.1/src/sageworks/web_components/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/endpoint_metric_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.062293 sageworks-0.6.1/src/sageworks/web_components/experiments/
--rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/experiments/color_maps.py
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/web_components/experiments/compound_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/experiments/dashboard_metric_plots.py
--rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/experiments/data_table.py
--rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/web_components/experiments/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/experiments/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/web_components/experiments/outlier_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/experiments/plugin_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.1/src/sageworks/web_components/experiments/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     8690 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/model_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     7079 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/plugin_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3155 2024-04-19 21:25:54.000000 sageworks-0.6.1/src/sageworks/web_components/plugin_unit_test.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.062572 sageworks-0.6.1/src/sageworks/web_components/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     2862 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/plugins/ag_table.py
--rw-r--r--   0 briford    (501) staff       (20)     9653 2024-04-15 13:43:00.000000 sageworks-0.6.1/src/sageworks/web_components/plugins/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2945 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/regression_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6547 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.1/src/sageworks/web_components/violin_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.066874 sageworks-0.6.1/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     4117 2024-04-23 23:36:07.000000 sageworks-0.6.1/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)    18445 2024-04-23 23:36:07.000000 sageworks-0.6.1/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2024-04-23 23:36:07.000000 sageworks-0.6.1/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)       74 2024-04-23 23:36:07.000000 sageworks-0.6.1/src/sageworks.egg-info/entry_points.txt
--rw-r--r--   0 briford    (501) staff       (20)      408 2024-04-23 23:36:07.000000 sageworks-0.6.1/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2024-04-23 23:36:07.000000 sageworks-0.6.1/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.063434 sageworks-0.6.1/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.063961 sageworks-0.6.1/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.1/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.064227 sageworks-0.6.1/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.1/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.1/tests/aws_account/aws_service_broker_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.065004 sageworks-0.6.1/tests/connectors/
--rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/connectors/s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)     5408 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/create_aqsol_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/create_basic_test_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/create_realtime_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.1/tests/create_training_adjusted_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/create_wine_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.1/tests/delete_test_artifacts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.065134 sageworks-0.6.1/tests/plugin_tests/
--rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.1/tests/plugin_tests/crashing_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.065390 sageworks-0.6.1/tests/specific/
--rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/specific/capital_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/specific/deletion_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.066228 sageworks-0.6.1/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     5142 2024-04-20 00:25:37.000000 sageworks-0.6.1/tests/transforms/model_metrics_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.1/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.1/tests/transforms/pandas_to_data_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-23 23:36:08.066655 sageworks-0.6.1/tests/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.1/tests/web_components/confusion_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.1/tests/web_components/correlation_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.1/tests/web_components/plugin_interface_test.py
--rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.6.1/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.636184 sageworks-0.6.2/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.528100 sageworks-0.6.2/.github/
+-rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.2/.github/dependabot.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.528592 sageworks-0.6.2/.github/workflows/
+-rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.2/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.2/.github/workflows/python-lint.yml
+-rw-r--r--   0 briford    (501) staff       (20)     2008 2023-12-24 17:18:24.000000 sageworks-0.6.2/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.2/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.2/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.2/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.2/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     4942 2024-05-08 22:04:08.636116 sageworks-0.6.2/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     3519 2024-05-04 22:17:44.000000 sageworks-0.6.2/README.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.2/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.517327 sageworks-0.6.2/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.531045 sageworks-0.6.2/applications/aws_dashboard/
+-rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-23 23:37:03.000000 sageworks-0.6.2/applications/aws_dashboard/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/Dockerfile_plugins
+-rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.2/applications/aws_dashboard/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.2/applications/aws_dashboard/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.532906 sageworks-0.6.2/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/aws_dashboard/assets/bootstrap_darkly.min.css
+-rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/aws_dashboard/assets/default.css
+-rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/aws_dashboard/assets/trash.png
+-rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-26 21:03:22.000000 sageworks-0.6.2/applications/aws_dashboard/dashboard
+-rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/aws_dashboard/nginx.conf
+-rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/open_source_config.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.517255 sageworks-0.6.2/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.533610 sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.534289 sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)     4212 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2458 2024-04-23 23:23:47.000000 sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.534990 sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.535742 sageworks-0.6.2/applications/aws_dashboard/pages/main/
+-rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/aws_dashboard/pages/main/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2899 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/main/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/aws_dashboard/pages/main/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.536488 sageworks-0.6.2/applications/aws_dashboard/pages/models/
+-rw-r--r--   0 briford    (501) staff       (20)     3954 2024-04-23 23:23:47.000000 sageworks-0.6.2/applications/aws_dashboard/pages/models/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2234 2024-04-27 20:59:25.000000 sageworks-0.6.2/applications/aws_dashboard/pages/models/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2152 2024-04-23 23:23:47.000000 sageworks-0.6.2/applications/aws_dashboard/pages/models/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.537225 sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1791 2024-04-26 21:07:33.000000 sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2664 2024-04-26 20:07:24.000000 sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1927 2024-04-26 21:04:41.000000 sageworks-0.6.2/applications/aws_dashboard/pages/pipelines/page.py
+-rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/aws_dashboard/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/aws_dashboard/supervisord.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.517380 sageworks-0.6.2/applications/experiments/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.538591 sageworks-0.6.2/applications/experiments/compound_explorer/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.2/applications/experiments/compound_explorer/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.539051 sageworks-0.6.2/applications/experiments/compound_explorer/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.2/applications/experiments/compound_explorer/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.2/applications/experiments/compound_explorer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.2/applications/experiments/compound_explorer/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.539539 sageworks-0.6.2/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/aws_identity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.539699 sageworks-0.6.2/aws_setup/event_bridge/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/event_bridge/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.540451 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/cdk.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.540696 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/lambda/
+-rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
+-rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.541943 sageworks-0.6.2/aws_setup/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_core/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.2/aws_setup/sageworks_core/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.542237 sageworks-0.6.2/aws_setup/sageworks_core/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/aws_setup/sageworks_core/sageworks_core/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.542670 sageworks-0.6.2/aws_setup/sageworks_core/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.542868 sageworks-0.6.2/aws_setup/sageworks_core/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.544501 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.544753 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-24 21:53:47.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.545006 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.545224 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.546022 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.546272 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-23 23:39:47.000000 sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.547574 sageworks-0.6.2/data/
+-rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.2/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.2/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.2/data/test_data.json
+-rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.2/data/wine_dataset.csv
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.547868 sageworks-0.6.2/docs/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.548467 sageworks-0.6.2/docs/admin/
+-rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.2/docs/admin/docker_push.md
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/admin/pypi_release.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.550355 sageworks-0.6.2/docs/api_classes/
+-rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/api_classes/data_source.md
+-rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/api_classes/endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/api_classes/feature_set.md
+-rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.2/docs/api_classes/meta.md
+-rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/api_classes/model.md
+-rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/api_classes/monitor.md
+-rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/api_classes/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.2/docs/api_classes/pipelines.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.551859 sageworks-0.6.2/docs/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/aws_setup/aws_access_management.md
+-rw-r--r--   0 briford    (501) staff       (20)     5610 2024-05-06 14:50:56.000000 sageworks-0.6.2/docs/aws_setup/aws_tips_and_tricks.md
+-rw-r--r--   0 briford    (501) staff       (20)     4229 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/aws_setup/core_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/aws_setup/dashboard_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/aws_setup/full_pipeline.md
+-rw-r--r--   0 briford    (501) staff       (20)     3270 2024-05-06 16:57:43.000000 sageworks-0.6.2/docs/aws_setup/sso_setup.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.552279 sageworks-0.6.2/docs/concepts/
+-rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/concepts/model_monitoring.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.552525 sageworks-0.6.2/docs/core_classes/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.554329 sageworks-0.6.2/docs/core_classes/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/core_classes/artifacts/artifact.md
+-rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/athena_source.md
+-rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/core_classes/artifacts/data_source_abstract.md
+-rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/endpoint_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/feature_set_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/model_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/monitor_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/artifacts/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.556078 sageworks-0.6.2/docs/core_classes/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/data_loaders_heavy.md
+-rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/data_loaders_light.md
+-rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/core_classes/transforms/data_to_features.md
+-rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/features_to_model.md
+-rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/model_to_endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/core_classes/transforms/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/core_classes/transforms/pandas_transforms.md
+-rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.2/docs/core_classes/transforms/transform.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.556894 sageworks-0.6.2/docs/enterprise/
+-rw-r--r--   0 briford    (501) staff       (20)     4075 2024-04-28 19:13:56.000000 sageworks-0.6.2/docs/enterprise/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      786 2024-04-28 17:52:09.000000 sageworks-0.6.2/docs/enterprise/project_branding.md
+-rw-r--r--   0 briford    (501) staff       (20)      892 2024-04-28 18:00:11.000000 sageworks-0.6.2/docs/enterprise/themes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.557171 sageworks-0.6.2/docs/glue/
+-rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/glue/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.562078 sageworks-0.6.2/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.2/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)     4380 2024-05-06 15:24:03.000000 sageworks-0.6.2/docs/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.563702 sageworks-0.6.2/docs/misc/
+-rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/misc/faq.md
+-rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/misc/general_info.md
+-rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/misc/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.2/docs/misc/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.564195 sageworks-0.6.2/docs/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.2/docs/plugins/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.2/docs/plugins/plugin_api_changes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.564437 sageworks-0.6.2/docs/repl/
+-rw-r--r--   0 briford    (501) staff       (20)     2081 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/repl/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.564851 sageworks-0.6.2/docs/research/
+-rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/research/eda.md
+-rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.2/docs/research/htg.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.565175 sageworks-0.6.2/examples/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.565328 sageworks-0.6.2/examples/ag-grid/
+-rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/ag-grid/hello_world.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.566570 sageworks-0.6.2/examples/datasource/
+-rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/datasource/datasource_from_df.py
+-rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/datasource/datasource_from_s3.py
+-rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/datasource/datasource_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/datasource/datasource_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/datasource/datasource_to_featureset.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.567263 sageworks-0.6.2/examples/endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/endpoint/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/endpoint/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/endpoint/endpoint_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.567758 sageworks-0.6.2/examples/featureset/
+-rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/featureset/featureset_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/featureset/featureset_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.2/examples/featureset/featureset_to_model.py
+-rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/full_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.568596 sageworks-0.6.2/examples/glue/
+-rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/glue/glue_hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/glue/glue_hello_world_with_log.py
+-rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.2/examples/glue/glue_load_s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.569305 sageworks-0.6.2/examples/meta/
+-rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/meta/meta_list_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/meta/meta_list_models.py
+-rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/meta/meta_model_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.570005 sageworks-0.6.2/examples/model/
+-rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/model/model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.2/examples/model/model_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      705 2024-05-08 21:58:54.000000 sageworks-0.6.2/examples/model/onboard_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.570653 sageworks-0.6.2/examples/monitor/
+-rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/monitor/monitor_setup.py
+-rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.2/examples/monitor/monitor_usage.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.572610 sageworks-0.6.2/examples/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.2/examples/pipelines/abalone_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.2/examples/pipelines/abalone_pipeline_v2.json
+-rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.2/examples/pipelines/aqsol_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.2/examples/pipelines/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.2/examples/pipelines/pipeline_execute.py
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.2/examples/pipelines/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.520572 sageworks-0.6.2/examples/plugins/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.573726 sageworks-0.6.2/examples/plugins/pages/
+-rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.2/examples/plugins/pages/my_plugin_page.py
+-rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/pages/plugin_page_1.py
+-rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/pages/plugin_page_2.py
+-rw-r--r--   0 briford    (501) staff       (20)     4528 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/pages/plugin_page_3.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.574168 sageworks-0.6.2/examples/plugins/views/
+-rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/plugins/views/model_plugin_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.2/examples/plugins/views/my_view_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.574997 sageworks-0.6.2/examples/plugins/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/custom_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/endpoint_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/endpoint_turbo.py
+-rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/model_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/plugins/web_components/model_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.576220 sageworks-0.6.2/examples/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.2/examples/storage/data_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.2/examples/storage/data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/hello_world_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.2/examples/storage/plugin_page_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.576759 sageworks-0.6.2/examples/storage/sagemaker_pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/all_steps.py
+-rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.520840 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.577671 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     3011 2024-05-06 15:23:23.000000 sageworks-0.6.2/mkdocs.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.578763 sageworks-0.6.2/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.6.2/notebooks/ML_Pipeline_with_SageWorks.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.6.2/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.6.2/notebooks/Outliers_in_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.586843 sageworks-0.6.2/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.2/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-06 16:51:44.000000 sageworks-0.6.2/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.591081 sageworks-0.6.2/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.2/scripts/ag_table_row_selection.py
+-rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/athena_ddl_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.2/scripts/copy_data_catalog_db.py
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.2/scripts/create_glue_workflow_with_trigger.py
+-rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.2/scripts/delete_redis_keys.py
+-rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/glue_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/model_endpoint_sanity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/onboard_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/onboard_models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.591563 sageworks-0.6.2/scripts/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.2/scripts/storage/dns_data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.2/scripts/storage/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.2/scripts/test_feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)      533 2024-05-08 22:04:08.636497 sageworks-0.6.2/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.6.2/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.521345 sageworks-0.6.2/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.591796 sageworks-0.6.2/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.592790 sageworks-0.6.2/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.594524 sageworks-0.6.2/src/sageworks/algorithms/dataframe/
+-rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/aggregation.py
+-rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
+-rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/dataframe/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.521715 sageworks-0.6.2/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.594727 sageworks-0.6.2/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.596238 sageworks-0.6.2/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.596493 sageworks-0.6.2/src/sageworks/algorithms/spark/
+-rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/spark/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.597971 sageworks-0.6.2/src/sageworks/algorithms/sql/
+-rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/column_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/correlations.py
+-rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/descriptive_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/outliers.py
+-rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/sample_rows.py
+-rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/algorithms/sql/value_counts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.600219 sageworks-0.6.2/src/sageworks/api/
+-rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.2/src/sageworks/api/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/api/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/api/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/api/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.2/src/sageworks/api/meta.py
+-rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/api/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/api/monitor.py
+-rw-r--r--   0 briford    (501) staff       (20)     6953 2024-04-26 21:22:37.000000 sageworks-0.6.2/src/sageworks/api/pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     6659 2024-04-26 21:22:37.000000 sageworks-0.6.2/src/sageworks/api/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.600954 sageworks-0.6.2/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)    11203 2024-05-08 21:03:14.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.602245 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.602398 sageworks-0.6.2/src/sageworks/core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.604969 sageworks-0.6.2/src/sageworks/core/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.2/src/sageworks/core/artifacts/artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/core/artifacts/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/artifacts/data_source_abstract.py
+-rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/artifacts/data_source_factory.py
+-rw-r--r--   0 briford    (501) staff       (20)    36630 2024-04-21 18:44:59.000000 sageworks-0.6.2/src/sageworks/core/artifacts/endpoint_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.2/src/sageworks/core/artifacts/feature_set_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    36993 2024-05-08 21:53:45.000000 sageworks-0.6.2/src/sageworks/core/artifacts/model_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/artifacts/monitor_core.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.605414 sageworks-0.6.2/src/sageworks/core/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     6919 2024-04-26 21:22:37.000000 sageworks-0.6.2/src/sageworks/core/pipelines/pipeline_executor.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.605990 sageworks-0.6.2/src/sageworks/core/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.606292 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.606638 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.607550 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.607799 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.607916 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.608024 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.608305 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.608882 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609104 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609204 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609416 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609667 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609830 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.609995 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.610468 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.610716 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.523780 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.610818 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.610972 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.611216 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.611753 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.612139 sageworks-0.6.2/src/sageworks/core/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/core/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.613401 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
+-rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/core/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.613565 sageworks-0.6.2/src/sageworks/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/experiments/view_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.613993 sageworks-0.6.2/src/sageworks/repl/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/repl/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.2/src/sageworks/repl/sageworks_shell.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.614506 sageworks-0.6.2/src/sageworks/resources/
+-rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.2/src/sageworks/resources/open_source_api.key
+-rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/resources/signature_verify_pub.pem
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.621348 sageworks-0.6.2/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.2/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/utils/aws_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/chem_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/utils/config_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/dashboard_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/utils/datetime_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/docker_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.2/src/sageworks/utils/ecs_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/endpoint_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/extract_model_artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/glue_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5757 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/license_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/utils/markdown_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.2/src/sageworks/utils/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/utils/plugin_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/repl_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/s3_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/sageworks_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.2/src/sageworks/utils/symbols.py
+-rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/test_data_generator.py
+-rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.2/src/sageworks/utils/trace_calls.py
+-rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.623129 sageworks-0.6.2/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.2/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     7780 2024-04-28 17:17:45.000000 sageworks-0.6.2/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/views/endpoint_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/views/model_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.626413 sageworks-0.6.2/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     5916 2024-04-25 23:06:38.000000 sageworks-0.6.2/src/sageworks/web_components/component_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/correlation_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/web_components/data_details_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-06 16:51:44.000000 sageworks-0.6.2/src/sageworks/web_components/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/endpoint_metric_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.628307 sageworks-0.6.2/src/sageworks/web_components/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/color_maps.py
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/compound_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/dashboard_metric_plots.py
+-rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/data_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/outlier_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/plugin_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.2/src/sageworks/web_components/experiments/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     8690 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/model_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     7169 2024-04-25 21:53:16.000000 sageworks-0.6.2/src/sageworks/web_components/plugin_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3530 2024-04-25 23:09:25.000000 sageworks-0.6.2/src/sageworks/web_components/plugin_unit_test.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.628708 sageworks-0.6.2/src/sageworks/web_components/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     2786 2024-04-26 21:04:42.000000 sageworks-0.6.2/src/sageworks/web_components/plugins/ag_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     9653 2024-04-15 13:43:00.000000 sageworks-0.6.2/src/sageworks/web_components/plugins/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2945 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/regression_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6838 2024-05-06 17:24:24.000000 sageworks-0.6.2/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.2/src/sageworks/web_components/violin_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.635730 sageworks-0.6.2/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     4942 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)    18783 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)       74 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/entry_points.txt
+-rw-r--r--   0 briford    (501) staff       (20)      408 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2024-05-08 22:04:08.000000 sageworks-0.6.2/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.630058 sageworks-0.6.2/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.630962 sageworks-0.6.2/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.2/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.631353 sageworks-0.6.2/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.2/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.2/tests/aws_account/aws_service_broker_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.632561 sageworks-0.6.2/tests/connectors/
+-rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/connectors/s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)     5618 2024-04-26 21:04:42.000000 sageworks-0.6.2/tests/create_aqsol_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/create_basic_test_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/create_realtime_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.2/tests/create_training_adjusted_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/create_wine_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/delete_test_artifacts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.632707 sageworks-0.6.2/tests/plugin_tests/
+-rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/plugin_tests/crashing_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.633008 sageworks-0.6.2/tests/specific/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/specific/capital_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/specific/deletion_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.634305 sageworks-0.6.2/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     5142 2024-04-20 00:25:37.000000 sageworks-0.6.2/tests/transforms/model_metrics_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.2/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.2/tests/transforms/pandas_to_data_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.634987 sageworks-0.6.2/tests/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/web_components/confusion_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/web_components/correlation_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.2/tests/web_components/plugin_interface_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.6.2/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-08 22:04:08.635418 sageworks-0.6.2/ui_testing/
+-rw-r--r--   0 briford    (501) staff       (20)     4591 2024-05-06 17:49:54.000000 sageworks-0.6.2/ui_testing/table_comparison.py
```

### Comparing `sageworks-0.6.1/.github/PULL_REQUEST_TEMPLATE.md` & `sageworks-0.6.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/.github/workflows/deploy-docs.yml` & `sageworks-0.6.2/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/.github/workflows/python-lint.yml` & `sageworks-0.6.2/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/.gitignore` & `sageworks-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/CONTRIBUTING.md` & `sageworks-0.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/LICENSE` & `sageworks-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/Makefile` & `sageworks-0.6.2/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/PKG-INFO` & `sageworks-0.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.6.1
+Version: 0.6.2
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
@@ -38,31 +38,36 @@
 Requires-Dist: setuptools>=69.0.2
 Requires-Dist: pyreadline3; sys_platform == "win32"
 
 
 # Welcome to SageWorks
 The SageWorks framework makes AWS® both easier to use and more powerful. SageWorks handles all the details around updating and managing a complex set of AWS Services. With a simple-to-use Python API and a beautiful set of web interfaces, SageWorks makes creating AWS ML pipelines a snap. It also dramatically improves both the usability and visibility across the entire spectrum of services: Glue Job, Athena, Feature Store, Models, and Endpoints, SageWorks makes it easy to build production ready, AWS powered, machine learning pipelines.
 
-<img align="right" width="500" alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/ed2ed1bd-e2d8-49a1-b350-b2e19e2b7832">
+<img align="right" width="480" alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/ed2ed1bd-e2d8-49a1-b350-b2e19e2b7832">
 
 ### Full AWS ML OverView
 - Health Monitoring 🟢
 - Dynamic Updates
 - High Level Summary
 
 ### Drill-Down Views
 - Incoming Data
 - Glue Jobs
 - DataSources
 - FeatureSets
 - Models
 - Endpoints
 
+## Private SaaS Architecture
+*Secure your Data, Empower your ML Pipelines*
 
-### Installation
+SageWorks is architected as a **Private SaaS**. This hybrid architecture is the ultimate solution for businesses that prioritize data control and security. SageWorks deploys as an AWS Stack within your own cloud environment, ensuring compliance with stringent corporate and regulatory standards. It offers the flexibility to tailor solutions to your specific business needs through our comprehensive plugin support, both components and full web interfaces. By using SageWorks, you maintain absolute control over your data while benefiting from the power, security, and scalability of AWS cloud services. [SageWorks Private SaaS Architecture](https://docs.google.com/presentation/d/1f_1gmE4-UAeUDDsoNdzK_d_MxALFXIkxORZwbJBjPq4/edit?usp=sharing)
+
+
+### API Installation
 
 - ```pip install sageworks```  Installs SageWorks
 
 - ```sageworks``` Runs the SageWorks REPL/Initial Setup
 
 For the full instructions for connecting your AWS Account see:
```

### Comparing `sageworks-0.6.1/applications/aws_dashboard/Dockerfile` & `sageworks-0.6.2/applications/aws_dashboard/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 RUN pip install --no-cache-dir -r requirements.txt
 
 # Copy the Nginx and Supervisor configuration files
 COPY nginx.conf /etc/nginx/sites-available/default
 COPY supervisord.conf /etc/supervisor/conf.d/supervisord.conf
 
 # Install Sageworks (changes often)
-RUN pip install --no-cache-dir sageworks==0.6.0
+RUN pip install --no-cache-dir sageworks==0.6.1
 
 # Copy the current directory contents into the container at /app
 COPY . /app
 
 # Grab the config file from build args, copy, and set ENV var
 ARG SAGEWORKS_CONFIG
 COPY $SAGEWORKS_CONFIG /app/sageworks_config.json
```

### Comparing `sageworks-0.6.1/applications/aws_dashboard/README.md` & `sageworks-0.6.2/applications/aws_dashboard/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/app.py` & `sageworks-0.6.2/applications/aws_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/assets/bootstrap_darkly.min.css` & `sageworks-0.6.2/applications/aws_dashboard/assets/bootstrap_darkly.min.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/assets/default.css` & `sageworks-0.6.2/applications/aws_dashboard/assets/default.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/assets/favicon.ico` & `sageworks-0.6.2/applications/aws_dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/assets/trash.png` & `sageworks-0.6.2/applications/aws_dashboard/assets/trash.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/dashboard` & `sageworks-0.6.2/applications/aws_dashboard/dashboard`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/open_source_config.json` & `sageworks-0.6.2/applications/aws_dashboard/open_source_config.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/data_sources/callbacks.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/data_sources/layout.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/data_sources/page.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/data_sources/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/endpoints/callbacks.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/endpoints/layout.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/endpoints/page.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/endpoints/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/feature_sets/callbacks.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/feature_sets/layout.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/feature_sets/page.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/feature_sets/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/main/callbacks.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/main/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/main/layout.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/main/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/main/page.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/main/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/models/callbacks.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/models/layout.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/models/layout.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         for component_id, plugin in kwargs.items()
     ]
     layout = html.Div(
         children=[
             dbc.Row(
                 [
                     html.H2("SageWorks: Models"),
+                    # html.H2("Project Awesome", style={'color': '#88cc88', 'font-style': 'italic'}),
                     dbc.Row(style={"padding": "30px 0px 0px 0px"}),
                     html.Div(id="dev_null", style={"display": "none"}),  # Output for callbacks without outputs
                 ]
             ),
             # A table that lists out all the Models
             dbc.Row(models_table),
             # Model Details, and Plugins
```

### Comparing `sageworks-0.6.1/applications/aws_dashboard/pages/models/page.py` & `sageworks-0.6.2/applications/aws_dashboard/pages/models/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/experiments/compound_explorer/app.py` & `sageworks-0.6.2/applications/experiments/compound_explorer/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/experiments/compound_explorer/assets/custom.css` & `sageworks-0.6.2/applications/experiments/compound_explorer/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/experiments/compound_explorer/callbacks.py` & `sageworks-0.6.2/applications/experiments/compound_explorer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/applications/experiments/compound_explorer/layout.py` & `sageworks-0.6.2/applications/experiments/compound_explorer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/aws_account_check.py` & `sageworks-0.6.2/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/aws_identity_check.py` & `sageworks-0.6.2/aws_setup/aws_identity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/build_ml_pipeline.py` & `sageworks-0.6.2/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/app.py` & `sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/cdk.json` & `sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py` & `sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py` & `sageworks-0.6.2/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_core/README.md` & `sageworks-0.6.2/aws_setup/sageworks_core/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_core/app.py` & `sageworks-0.6.2/aws_setup/sageworks_core/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_core/cdk.json` & `sageworks-0.6.2/aws_setup/sageworks_core/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py` & `sageworks-0.6.2/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.6.2/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_dashboard_full/README.md` & `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_dashboard_full/app.py` & `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_dashboard_full/cdk.json` & `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py` & `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from aws_cdk.aws_ec2 import Subnet
 from aws_cdk.aws_certificatemanager import Certificate
 from aws_cdk.aws_ecs_patterns import ApplicationLoadBalancedFargateService
 from constructs import Construct
 
 # When you want a different version change this line
-dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_4_amd64"
+dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_6_1_amd64"
 
 
 class SageworksDashboardStackProps(StackProps):
     def __init__(
         self,
         sageworks_bucket: str,
         sageworks_api_key: str,
```

### Comparing `sageworks-0.6.1/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py` & `sageworks-0.6.2/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/README.md` & `sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/app.py` & `sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/cdk.json` & `sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py` & `sageworks-0.6.2/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     aws_logs as logs,
 )
 from aws_cdk.aws_certificatemanager import Certificate
 from aws_cdk.aws_ecs_patterns import ApplicationLoadBalancedFargateService
 from constructs import Construct
 
 # When you want a different version change this line
-dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_6_0_amd64"
+dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_6_1_amd64"
 
 
 class SageworksDashboardStackProps(StackProps):
     def __init__(
         self,
         sageworks_bucket: str,
         sageworks_api_key: str,
```

### Comparing `sageworks-0.6.1/data/abalone.csv` & `sageworks-0.6.2/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/data/test_data.csv` & `sageworks-0.6.2/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/data/test_data.json` & `sageworks-0.6.2/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/data/wine_dataset.csv` & `sageworks-0.6.2/data/wine_dataset.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/admin/docker_push.md` & `sageworks-0.6.2/docs/admin/docker_push.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/admin/pypi_release.md` & `sageworks-0.6.2/docs/admin/pypi_release.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/api_classes/data_source.md` & `sageworks-0.6.2/docs/api_classes/data_source.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/api_classes/endpoint.md` & `sageworks-0.6.2/docs/api_classes/endpoint.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/api_classes/feature_set.md` & `sageworks-0.6.2/docs/api_classes/feature_set.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/api_classes/meta.md` & `sageworks-0.6.2/docs/api_classes/meta.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/api_classes/model.md` & `sageworks-0.6.2/docs/api_classes/model.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/api_classes/monitor.md` & `sageworks-0.6.2/docs/api_classes/monitor.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/api_classes/overview.md` & `sageworks-0.6.2/docs/api_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/api_classes/pipelines.md` & `sageworks-0.6.2/docs/api_classes/pipelines.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/aws_setup/aws_access_management.md` & `sageworks-0.6.2/docs/aws_setup/aws_access_management.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/aws_setup/aws_tips_and_tricks.md` & `sageworks-0.6.2/docs/aws_setup/aws_tips_and_tricks.md`

 * *Files 18% similar despite different names*

```diff
@@ -64,95 +64,15 @@
 <img width="600" alt="Screenshot 2023-05-03 at 9 32 28 AM" src="https://user-images.githubusercontent.com/4806709/235967585-d772d2f9-13ac-4795-aca3-429fbb1b7311.png">
 
 ### AWS Console
 Now when the user logs onto the AWS Console they should see something like this:
 <img width="800" alt="Screenshot 2023-05-03 at 9 21 27 AM" src="https://user-images.githubusercontent.com/4806709/235970829-d1fdf1a8-84a2-46ca-a20e-143664715531.png">
 
 ### SSO Setup for Command Line/Python Usage
-For full instructions see [SSO Command Line/Python Configure](https://docs.aws.amazon.com/cli/latest/userguide/sso-configure-profile-token.html). But here's a quick summary
-#### Get some information
-  - Goto your AWS Identity Center in the AWS Console
-  - On the right side there will be two important pieces of information
-    - Region
-    - Start URL
-#### Install AWS CLI
-- Mac: `brew install awscli`
-- Linus: TBD
-- Windows: TBD
-
-#### Running the SSO Configuration 
-**Note:** You only need to do this once!
-```
-aws configure sso --profile <the name of the new profile> (something like bob_sso)
-SSO session name (Recommended): my-sso
-SSO start URL []: <the Start URL from info above>
-SSO region []: <the Region from info above>
-SSO registration scopes [sso:account:access]:
-```
-
-You will get a browser open/redirect at this point and get a list of available accounts.. something like below, just pick the correct account
-
-```
-There are 2 AWS accounts available to you.
-> SCP_Sandbox, briford+sandbox@supercowpowers.com (XXXX40646YYY)
-  SCP_Main, briford@supercowpowers.com (XXX576391YYY)
-```
-
-Now pick the role that you're going to use
-
-```
-There are 2 roles available to you.
-> DataScientist
-  AdministratorAccess
-```
-
-## Setting up some aliases for bash/zsh
-Edit your favorite ~/.bashrc ~/.zshrc and add these nice aliases/helper
-
-```
-# AWS Aliases
-alias bob_sso='export AWS_PROFILE=bob_sso'
-
-# Default AWS Profile
-export AWS_PROFILE=bob_sso
-```
-
-## Testing your new AWS Profile
-Make sure your profile is active/set
-
-```
-env | grep AWS
-AWS_PROFILE=<bob_sso or whatever>
-```
-Now you can list the S3 buckets in the AWS Account
-
-```
-aws ls s3
-```
-If you get some message like this...
-
-```
-The SSO session associated with this profile has
-expired or is otherwise invalid. To refresh this SSO
-session run aws sso login with the corresponding
-profile.
-```
-
-This is fine/good, a browser will open up and you can refresh your SSO Token.
-
-After that you should get a listing of the S3 buckets without needed to refresh your token.
-
-```
-aws s3 ls
-❯ aws s3 ls
-2023-03-20 20:06:53 aws-athena-query-results-XXXYYY-us-west-2
-2023-03-30 13:22:28 sagemaker-studio-XXXYYY-dbgyvq8ruka
-2023-03-24 22:05:55 sagemaker-us-west-2-XXXYYY
-2023-04-30 13:43:29 scp-sageworks-artifacts
-```
+Please see our [SSO Setup](sso_setup.md)
 
  
 ## AWS Resources
 - [AWS Identity Center](https://docs.aws.amazon.com/singlesignon/latest/userguide/what-is.html)
 - [Users and Groups](https://docs.aws.amazon.com/singlesignon/latest/userguide/users-groups-provisioning.html)
 - [Permission Sets](https://docs.aws.amazon.com/singlesignon/latest/userguide/permissionsetsconcept.html)
 - [SSO Command Line/Python Configure](https://docs.aws.amazon.com/cli/latest/userguide/sso-configure-profile-token.html)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sageworks-0.6.1/docs/aws_setup/core_stack.md` & `sageworks-0.6.2/docs/aws_setup/core_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/aws_setup/dashboard_stack.md` & `sageworks-0.6.2/docs/aws_setup/dashboard_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/aws_setup/full_pipeline.md` & `sageworks-0.6.2/docs/aws_setup/full_pipeline.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/concepts/model_monitoring.md` & `sageworks-0.6.2/docs/concepts/model_monitoring.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/core_classes/artifacts/overview.md` & `sageworks-0.6.2/docs/core_classes/artifacts/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/core_classes/overview.md` & `sageworks-0.6.2/docs/core_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/core_classes/transforms/overview.md` & `sageworks-0.6.2/docs/core_classes/transforms/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/core_classes/transforms/pandas_transforms.md` & `sageworks-0.6.2/docs/core_classes/transforms/pandas_transforms.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/core_classes/transforms/transform.md` & `sageworks-0.6.2/docs/core_classes/transforms/transform.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/glue/index.md` & `sageworks-0.6.2/docs/glue/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/big_spider.png` & `sageworks-0.6.2/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/graph_representation.png` & `sageworks-0.6.2/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/powered_aws_dark_blue.png` & `sageworks-0.6.2/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/powered_aws_transparent.png` & `sageworks-0.6.2/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/powered_aws_white.png` & `sageworks-0.6.2/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.6.2/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/sageworks.png` & `sageworks-0.6.2/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/sageworks_concepts.png` & `sageworks-0.6.2/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/scp.png` & `sageworks-0.6.2/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/scp_labs.png` & `sageworks-0.6.2/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/images/small_spider.png` & `sageworks-0.6.2/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/index.md` & `sageworks-0.6.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,53 @@
+
 # Welcome to SageWorks
-The SageWorks framework makes AWS® both easier to use and more powerful. SageWorks handles all the details around updating and managing a complex set of AWS Services. With a simple-to-use Python API and a beautiful set of web interfaces, SageWorks makes creating AWS ML pipelines a snap. It also dramatically improves both the usability and visibility across the entire spectrum of services: Glue Jobs, Athena, Feature Store, Models, and Endpoints. SageWorks makes it easy to build production ready, AWS powered, machine learning pipelines.
+The SageWorks framework makes AWS® both easier to use and more powerful. SageWorks handles all the details around updating and managing a complex set of AWS Services. With a simple-to-use Python API and a beautiful set of web interfaces, SageWorks makes creating AWS ML pipelines a snap. It also dramatically improves both the usability and visibility across the entire spectrum of services: Glue Job, Athena, Feature Store, Models, and Endpoints, SageWorks makes it easy to build production ready, AWS powered, machine learning pipelines.
 
-<figure style="float: right; width: 500px;">
-<img alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/5f8b32a2-ed72-45f2-bd96-91b7bbbccff4">
-<figcaption>SageWorks Dashboard: AWS Pipelines in a Whole New Light!</figcaption>
-</figure>
+<img align="right" width="480" alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/ed2ed1bd-e2d8-49a1-b350-b2e19e2b7832">
 
-### Full AWS OverView
+### Full AWS ML OverView
 - Health Monitoring 🟢
 - Dynamic Updates
 - High Level Summary
 
 ### Drill-Down Views
+- Incoming Data
 - Glue Jobs
 - DataSources
 - FeatureSets
 - Models
 - Endpoints
 
+## Private SaaS Architecture
+*Secure your Data, Empower your ML Pipelines*
 
-## Getting Started
+SageWorks is architected as a **Private SaaS**. This hybrid architecture is the ultimate solution for businesses that prioritize data control and security. SageWorks deploys as an AWS Stack within your own cloud environment, ensuring compliance with stringent corporate and regulatory standards. It offers the flexibility to tailor solutions to your specific business needs through our comprehensive plugin support, both components and full web interfaces. By using SageWorks, you maintain absolute control over your data while benefiting from the power, security, and scalability of AWS cloud services. [SageWorks Private SaaS Architecture](https://docs.google.com/presentation/d/1f_1gmE4-UAeUDDsoNdzK_d_MxALFXIkxORZwbJBjPq4/edit?usp=sharing)
 
-The SageWorks package has two main components, a Web Interface that provides visibility into AWS ML PIpelines and a Python API that makes creation and usage of the AWS ML Services easier than using/learning the services directly.
 
-### Web Interfaces
-The SageWorks Dashboard has a set of web interfaces that give visibility into the AWS Glue and SageMaker Services. There are currently 5 web interfaces available:
+### API Installation
 
+- ```pip install sageworks```  Installs SageWorks
 
-- **Top Level Dashboard:** Shows all AWS ML Artifacts (Glue and SageMaker)
-- **DataSources:** DataSource Column Details, Distributions and Correlations
-- **FeatureSets:** FeatureSet Details, Distributions and Correlations
-- **Model:** Model details, performance metric, and inference plots
-- **Endpoints:** Endpoint details, realtime charts of endpoint performance and latency
+- ```sageworks``` Runs the SageWorks REPL/Initial Setup
 
-### Python API
-SageWorks API Documentation: [SageWorks API Classes](api_classes/overview.md) 
+For the full instructions for connecting your AWS Account see:
 
-The main functionality of the Python API is to encapsulate and manage a set of AWS services underneath a Python Object interface. The Python Classes are used to create and interact with Machine Learning Pipeline Artifacts.
+- Initial Setup/Config: [Initial Setup](https://supercowpowers.github.io/sageworks/#initial-setupconfig) 
+- One time AWS Onboarding: [AWS Setup](https://supercowpowers.github.io/sageworks/aws_setup/core_stack/)
 
-### Initial Setup/Config
-**Note:** Use the SageWorks REPL to setup your AWS connection for both API Usage (Data Scientists/Engineers) and AWS Initial Setup (AWS Folks).
 
-```
-> pip install sageworks
-> sageworks <-- This starts the REPL
 
-Welcome to SageWorks!
-Looks like this is your first time using SageWorks...
-Let's get you set up...
-AWS_PROFILE: my_aws_profile
-SAGEWORKS_BUCKET: my-company-sageworks
-[optional] REDIS_HOST(localhost): my-redis.cache.amazon (or leave blank)
-[optional] REDIS_PORT(6379):
-[optional] REDIS_PASSWORD():
-[optional] SAGEWORKS_API_KEY(open_source): my_api_key (or leave blank)
-```
-**That's It:** You're now all set. This configuration only needs to be **ONCE** :)
+### SageWorks Documentation
+<img align="right" width="340" alt="sageworks_api" style="padding-left: 10px;"  src="https://github.com/SuperCowPowers/sageworks/assets/4806709/bf0e8591-75d4-44c1-be05-4bfdee4b7186">
 
-### AWS Folks (initial setup)
-Setting up SageWorks on your AWS Account: [AWS Setup](aws_setup/core_stack.md)
+[SageWorks Documentation](https://supercowpowers.github.io/sageworks/): The documentation contains examples from the SageWorks source code in this repository under the `examples/` directory. For a full code listing of any example please visit our [SageWorks Examples](https://github.com/SuperCowPowers/sageworks/blob/main/examples)
 
-### Data Scientists/Engineers
-- SageWorks REPL: [SageWorks REPL](repl/index.md)
-- Using SageWorks for ML Pipelines: [SageWorks API Classes](api_classes/overview.md)
-- SCP SageWorks Github: [Github Repo](https://github.com/SuperCowPowers/sageworks)
 
+### SageWorks Beta Program
+Using SageWorks will minimize the time and manpower needed to incorporate AWS ML into your organization. If your company would like to be a SageWorks Beta Tester, contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
-## Additional Resources
+### Contributions
+If you'd like to contribute to the SageWorks project, you're more than welcome. All contributions will fall under the existing project [license](https://github.com/SuperCowPowers/sageworks/blob/main/LICENSE). If you are interested in contributing or have questions please feel free to contact us at [sageworks@supercowpowers.com](mailto:sageworks@supercowpowers.com).
 
-<img align="right" src="images/scp.png" width="180">
+<img align="right" src="docs/images/scp.png" width="180">
 
-- SageWorks Core Classes: [Core Classes](core_classes/overview.md)
-- Consulting Available: [SuperCowPowers LLC](https://www.supercowpowers.com)
+® Amazon Web Services, AWS, the Powered by AWS logo, are trademarks of Amazon.com, Inc. or its affiliates
```

### Comparing `sageworks-0.6.1/docs/misc/faq.md` & `sageworks-0.6.2/docs/misc/faq.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/misc/general_info.md` & `sageworks-0.6.2/docs/misc/general_info.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/misc/sageworks_classes_concepts.md` & `sageworks-0.6.2/docs/misc/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/misc/scp_consulting.md` & `sageworks-0.6.2/docs/misc/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/plugins/index.md` & `sageworks-0.6.2/docs/plugins/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/plugins/plugin_api_changes.md` & `sageworks-0.6.2/docs/plugins/plugin_api_changes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/repl/index.md` & `sageworks-0.6.2/docs/repl/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/research/eda.md` & `sageworks-0.6.2/docs/research/eda.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/docs/research/htg.md` & `sageworks-0.6.2/docs/research/htg.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/datasource/datasource_query.py` & `sageworks-0.6.2/examples/datasource/datasource_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/datasource/datasource_stats.py` & `sageworks-0.6.2/examples/datasource/datasource_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/endpoint/endpoint_inference.py` & `sageworks-0.6.2/examples/endpoint/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/featureset/featureset_eda.py` & `sageworks-0.6.2/examples/featureset/featureset_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/featureset/featureset_query.py` & `sageworks-0.6.2/examples/featureset/featureset_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/full_ml_pipeline.py` & `sageworks-0.6.2/examples/full_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/glue/glue_hello_world.py` & `sageworks-0.6.2/examples/glue/glue_hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/glue/glue_hello_world_with_log.py` & `sageworks-0.6.2/examples/glue/glue_hello_world_with_log.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/glue/glue_load_s3_bucket.py` & `sageworks-0.6.2/examples/glue/glue_load_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/meta/meta_model_metrics.py` & `sageworks-0.6.2/examples/meta/meta_model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/model/model_metrics.py` & `sageworks-0.6.2/examples/model/model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/monitor/monitor_usage.py` & `sageworks-0.6.2/examples/monitor/monitor_usage.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/pipelines/abalone_pipeline_v1.json` & `sageworks-0.6.2/examples/pipelines/abalone_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/pipelines/abalone_pipeline_v2.json` & `sageworks-0.6.2/examples/pipelines/abalone_pipeline_v2.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/pipelines/aqsol_pipeline_v1.json` & `sageworks-0.6.2/examples/pipelines/aqsol_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/pipelines/pipeline_manager.py` & `sageworks-0.6.2/examples/pipelines/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/pages/my_plugin_page.py` & `sageworks-0.6.2/examples/plugins/pages/my_plugin_page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/pages/plugin_page_1.py` & `sageworks-0.6.2/examples/plugins/pages/plugin_page_1.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/pages/plugin_page_2.py` & `sageworks-0.6.2/examples/plugins/pages/plugin_page_2.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/pages/plugin_page_3.py` & `sageworks-0.6.2/examples/plugins/pages/plugin_page_3.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/views/model_plugin_view.py` & `sageworks-0.6.2/examples/plugins/views/model_plugin_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/views/my_view_plugin.py` & `sageworks-0.6.2/examples/plugins/views/my_view_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/web_components/custom_plugin.py` & `sageworks-0.6.2/examples/plugins/web_components/custom_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/web_components/endpoint_plugin.py` & `sageworks-0.6.2/examples/plugins/web_components/endpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/web_components/endpoint_turbo.py` & `sageworks-0.6.2/examples/plugins/web_components/endpoint_turbo.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/web_components/model_markdown.py` & `sageworks-0.6.2/examples/plugins/web_components/model_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/plugins/web_components/model_plugin.py` & `sageworks-0.6.2/examples/plugins/web_components/model_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/storage/data_to_data.py` & `sageworks-0.6.2/examples/storage/data_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/storage/data_to_features.py` & `sageworks-0.6.2/examples/storage/data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/storage/endpoint_inference.py` & `sageworks-0.6.2/examples/storage/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/storage/hello_world_pipeline.py` & `sageworks-0.6.2/examples/storage/hello_world_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/storage/plugin_page_example.py` & `sageworks-0.6.2/examples/storage/plugin_page_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/storage/sagemaker_pipelines/all_steps.py` & `sageworks-0.6.2/examples/storage/sagemaker_pipelines/all_steps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/storage/sagemaker_pipelines/ml_pipeline.py` & `sageworks-0.6.2/examples/storage/sagemaker_pipelines/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py` & `sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py` & `sageworks-0.6.2/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/mkdocs.yml` & `sageworks-0.6.2/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -30,22 +30,27 @@
       - Features To Model: core_classes/transforms/features_to_model.md
       - Model to Endpoint: core_classes/transforms/model_to_endpoint.md
       - Pandas Transforms: core_classes/transforms/pandas_transforms.md
       - Transform: core_classes/transforms/transform.md
   - Plugins: 
       - OverView: plugins/index.md
       - API Changes: plugins/plugin_api_changes.md
+  - SageWorks Enterprise: 
+      - OverView: enterprise/index.md
+      - Themes: enterprise/themes.md
+      - Project Branding: enterprise/project_branding.md
   - FAQ:  misc/faq.md
   - Research:
       - EDA: research/eda.md
       - HTG: research/htg.md
   - AWS Glue Jobs: glue/index.md 
   - AWS Setup: 
-    - Initial Setup: aws_setup/core_stack.md
+    - Developer SSO Setup: aws_setup/sso_setup.md
     - Full Pipeline Testing: aws_setup/full_pipeline.md
+    - AWS Admin Initial Setup: aws_setup/core_stack.md
     - Dashboard Setup: aws_setup/dashboard_stack.md
     - AWS Tips and Tricks: aws_setup/aws_tips_and_tricks.md
     - AWS Access Management: aws_setup/aws_access_management.md
   - Admin: 
     - PyPI Release:  admin/pypi_release.md
     - Docker Push:  admin/docker_push.md
```

### Comparing `sageworks-0.6.1/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.6.2/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/notebooks/ML_Pipeline_with_SageWorks_2.ipynb` & `sageworks-0.6.2/notebooks/ML_Pipeline_with_SageWorks_2.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/notebooks/Outliers_in_SageWorks.ipynb` & `sageworks-0.6.2/notebooks/Outliers_in_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/notebooks/images/athena_query_aqsol.png` & `sageworks-0.6.2/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.6.2/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.6.2/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/notebooks/images/model_screenshot.png` & `sageworks-0.6.2/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/notebooks/images/sageworks_concepts.png` & `sageworks-0.6.2/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/notebooks/images/scp_labs.png` & `sageworks-0.6.2/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/ag_table_row_selection.py` & `sageworks-0.6.2/scripts/ag_table_row_selection.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/athena_ddl_mixed_case.py` & `sageworks-0.6.2/scripts/athena_ddl_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/copy_data_catalog_db.py` & `sageworks-0.6.2/scripts/copy_data_catalog_db.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/create_glue_workflow_with_trigger.py` & `sageworks-0.6.2/scripts/create_glue_workflow_with_trigger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/delete_redis_keys.py` & `sageworks-0.6.2/scripts/delete_redis_keys.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/glue_mixed_case.py` & `sageworks-0.6.2/scripts/glue_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/model_endpoint_sanity_check.py` & `sageworks-0.6.2/scripts/model_endpoint_sanity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/onboard_endpoints.py` & `sageworks-0.6.2/scripts/onboard_endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/onboard_models.py` & `sageworks-0.6.2/scripts/onboard_models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/storage/dns_data_to_features.py` & `sageworks-0.6.2/scripts/storage/dns_data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/storage/generate_jsonl_data.py` & `sageworks-0.6.2/scripts/storage/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/scripts/test_feature_resolution.py` & `sageworks-0.6.2/scripts/test_feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/setup.cfg` & `sageworks-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/setup.py` & `sageworks-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/__init__.py` & `sageworks-0.6.2/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/dataframe/aggregation.py` & `sageworks-0.6.2/src/sageworks/algorithms/dataframe/aggregation.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/dataframe/data_source_eda.py` & `sageworks-0.6.2/src/sageworks/algorithms/dataframe/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/dataframe/dimensionality_reduction.py` & `sageworks-0.6.2/src/sageworks/algorithms/dataframe/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/dataframe/feature_resolution.py` & `sageworks-0.6.2/src/sageworks/algorithms/dataframe/feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/dataframe/feature_spider.py` & `sageworks-0.6.2/src/sageworks/algorithms/dataframe/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/dataframe/row_tagger.py` & `sageworks-0.6.2/src/sageworks/algorithms/dataframe/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/spark/Readme.md` & `sageworks-0.6.2/src/sageworks/algorithms/spark/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/sql/Readme.md` & `sageworks-0.6.2/src/sageworks/algorithms/sql/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/sql/column_stats.py` & `sageworks-0.6.2/src/sageworks/algorithms/sql/column_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/sql/correlations.py` & `sageworks-0.6.2/src/sageworks/algorithms/sql/correlations.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/sql/descriptive_stats.py` & `sageworks-0.6.2/src/sageworks/algorithms/sql/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/sql/outliers.py` & `sageworks-0.6.2/src/sageworks/algorithms/sql/outliers.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/sql/sample_rows.py` & `sageworks-0.6.2/src/sageworks/algorithms/sql/sample_rows.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/algorithms/sql/value_counts.py` & `sageworks-0.6.2/src/sageworks/algorithms/sql/value_counts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/api/__init__.py` & `sageworks-0.6.2/src/sageworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/api/data_source.py` & `sageworks-0.6.2/src/sageworks/api/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/api/endpoint.py` & `sageworks-0.6.2/src/sageworks/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/api/feature_set.py` & `sageworks-0.6.2/src/sageworks/api/feature_set.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/api/meta.py` & `sageworks-0.6.2/src/sageworks/api/meta.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/api/model.py` & `sageworks-0.6.2/src/sageworks/api/model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/api/monitor.py` & `sageworks-0.6.2/src/sageworks/api/monitor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/api/pipeline.py` & `sageworks-0.6.2/src/sageworks/api/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,49 +15,49 @@
 
 
 class Pipeline:
     """Pipeline: SageWorks Pipeline API Class
 
     Common Usage:
         ```
-        my_pipeline = Pipeline("pipeline_name")
+        my_pipeline = Pipeline("name")
         my_pipeline.details()
         my_pipeline.execute()  # Execute entire pipeline
         my_pipeline.execute_partial(["data_source", "feature_set"])
         my_pipeline.execute_partial(["model", "endpoint"])
         ```
     """
 
     def __init__(self, name: str):
         """Pipeline Init Method"""
         self.log = logging.getLogger("sageworks")
-        self.pipeline_name = name
+        self.name = name
 
         # Grab our SageWorks Bucket from Config
         self.cm = ConfigManager()
         self.sageworks_bucket = self.cm.get_config("SAGEWORKS_BUCKET")
         if self.sageworks_bucket is None:
             self.log = logging.getLogger("sageworks")
             self.log.critical("Could not find ENV var for SAGEWORKS_BUCKET!")
             sys.exit(1)
 
         # Set the S3 Path for this Pipeline
         self.bucket = self.sageworks_bucket
-        self.key = f"pipelines/{self.pipeline_name}.json"
+        self.key = f"pipelines/{self.name}.json"
         self.s3_path = f"s3://{self.bucket}/{self.key}"
 
         # Grab a SageWorks Session (this allows us to assume the SageWorks ExecutionRole)
         self.boto_session = AWSAccountClamp().boto_session()
         self.s3_client = self.boto_session.client("s3")
 
         # If this S3 Path exists, load the Pipeline
         if wr.s3.does_object_exist(self.s3_path):
             self.pipeline = self._get_pipeline()
         else:
-            self.log.warning(f"Pipeline {self.pipeline_name} not found at {self.s3_path}")
+            self.log.warning(f"Pipeline {self.name} not found at {self.s3_path}")
             self.pipeline = None
 
         # Data Storage Cache
         self.data_storage = SageWorksCache(prefix="data_storage")
 
     def set_input(self, input: Union[str, pd.DataFrame], artifact: str = "data_source"):
         """Set the input for the Pipeline
@@ -104,29 +104,29 @@
 
         Args:
         pipeline (dict): pipeline (or sub pipeline) to process.
         path (str): Current path to the key, used for nested dictionaries.
         """
         # Grab the entire pipeline if not provided (first call)
         if not pipeline:
-            self.log.important(f"Checking Pipeline: {self.pipeline_name}...")
+            self.log.important(f"Checking Pipeline: {self.name}...")
             pipeline = self.pipeline
         for key, value in pipeline.items():
             if isinstance(value, dict):
                 # Recurse into sub-dictionary
                 self.report_settable_fields(value, path + key + " -> ")
             elif isinstance(value, str) and value.startswith("<<") and value.endswith(">>"):
                 # Check if required or optional
                 required = "[Required]" if "required" in value else "[Optional]"
                 self.log.important(f"{required} Path: {path + key}")
 
     def delete(self):
         """Pipeline Deletion"""
-        self.log.info(f"Deleting Pipeline: {self.pipeline_name}...")
-        self.data_storage.delete(f"pipeline:{self.pipeline_name}:details")
+        self.log.info(f"Deleting Pipeline: {self.name}...")
+        self.data_storage.delete(f"pipeline:{self.name}:details")
         wr.s3.delete_objects(self.s3_path)
 
     def _get_pipeline(self) -> dict:
         """Internal: Get the pipeline as a JSON object from the specified S3 bucket and key."""
         response = self.s3_client.get_object(Bucket=self.bucket, Key=self.key)
         json_object = json.loads(response["Body"].read())
         return json_object
```

### Comparing `sageworks-0.6.1/src/sageworks/api/pipeline_manager.py` & `sageworks-0.6.2/src/sageworks/api/pipeline_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,35 +95,35 @@
                 pipeline[name]["target_column"] = artifact.target()
                 pipeline[name]["feature_list"] = artifact.features()
 
         # Return the Pipeline
         return pipeline
 
     # Publish a Pipeline to SageWorks
-    def publish_pipeline(self, pipeline_name: str, pipeline: dict):
+    def publish_pipeline(self, name: str, pipeline: dict):
         """Save a Pipeline to S3
 
         Args:
-            pipeline_name (str): The name of the Pipeline
+            name (str): The name of the Pipeline
             pipeline (dict): The Pipeline to save
         """
-        key = f"{self.prefix}{pipeline_name}.json"
-        self.log.important(f"Saving {pipeline_name} to S3: {self.bucket}/{key}...")
+        key = f"{self.prefix}{name}.json"
+        self.log.important(f"Saving {name} to S3: {self.bucket}/{key}...")
 
         # Save the pipeline as an S3 JSON object
         self.s3_client.put_object(Body=json.dumps(pipeline, indent=4), Bucket=self.bucket, Key=key)
 
-    def delete_pipeline(self, pipeline_name: str):
+    def delete_pipeline(self, name: str):
         """Delete a Pipeline from S3
 
         Args:
-            pipeline_name (str): The name of the Pipeline to delete
+            name (str): The name of the Pipeline to delete
         """
-        key = f"{self.prefix}{pipeline_name}.json"
-        self.log.important(f"Deleting {pipeline_name} from S3: {self.bucket}/{key}...")
+        key = f"{self.prefix}{name}.json"
+        self.log.important(f"Deleting {name} from S3: {self.bucket}/{key}...")
 
         # Delete the pipeline object from S3
         self.s3_client.delete_object(Bucket=self.bucket, Key=key)
 
     # Save a Pipeline to a local file
     def save_pipeline_to_file(self, pipeline: dict, filepath: str):
         """Save a Pipeline to a local file
```

### Comparing `sageworks-0.6.1/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,20 @@
     def __class_init__(cls):
         """AWSServiceBroker pulls and collects metadata from a bunch of AWS Services"""
 
         # Grab our SageWorks Bucket
         cm = ConfigManager()
         cls.sageworks_bucket = cm.get_config("SAGEWORKS_BUCKET")
 
+        # Sanity check our SageWorks Bucket
+        if cls.sageworks_bucket is None:
+            cls.log.critical("SAGEWORKS_BUCKET is not defined")
+            cls.log.critical("Run Initial Setup here: https://supercowpowers.github.io/sageworks/#initial-setupconfig ")
+            sys.exit(1)
+
         # Construct bucket paths
         cls.incoming_data_bucket = "s3://" + cls.sageworks_bucket + "/incoming-data/"
         cls.data_sources_bucket = "s3://" + cls.sageworks_bucket + "/data-sources/"
         cls.feature_sets_bucket = "s3://" + cls.sageworks_bucket + "/feature-sets/"
 
         # SageWorks category mapping to AWS Services
         # - incoming_data = S3
```

### Comparing `sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py` & `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.6.2/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/artifacts/__init__.py` & `sageworks-0.6.2/src/sageworks/core/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/artifacts/artifact.py` & `sageworks-0.6.2/src/sageworks/core/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/artifacts/athena_source.py` & `sageworks-0.6.2/src/sageworks/core/artifacts/athena_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/artifacts/data_source_abstract.py` & `sageworks-0.6.2/src/sageworks/core/artifacts/data_source_abstract.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/artifacts/data_source_factory.py` & `sageworks-0.6.2/src/sageworks/core/artifacts/data_source_factory.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/artifacts/endpoint_core.py` & `sageworks-0.6.2/src/sageworks/core/artifacts/endpoint_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/artifacts/feature_set_core.py` & `sageworks-0.6.2/src/sageworks/core/artifacts/feature_set_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/artifacts/model_core.py` & `sageworks-0.6.2/src/sageworks/core/artifacts/model_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         registered_endpoints.add(endpoint_name)
         self.upsert_sageworks_meta({"sageworks_registered_endpoints": list(registered_endpoints)})
 
         # A new endpoint means we need to refresh our inference path
         time.sleep(2)  # Give the AWS Metadata a chance to update
         self.endpoint_inference_path = self.get_endpoint_inference_path()
 
-    def get_endpoints(self) -> list[str]:
+    def endpoints(self) -> list[str]:
         """Get the list of registered endpoints for this Model
 
         Returns:
             list[str]: List of registered endpoints
         """
         return self.sageworks_meta().get("sageworks_registered_endpoints", [])
 
@@ -319,14 +319,30 @@
             endpoint_inference_base = self.endpoints_s3_path + "/inference/"
             endpoint_inference_paths = [endpoint_inference_base + e for e in registered_endpoints]
             return newest_files(endpoint_inference_paths, self.sm_session)
         else:
             self.log.warning(f"No registered endpoints found for {self.model_name}!")
             return None
 
+    def set_target(self, target_column: str):
+        """Set the target for this Model
+
+        Args:
+            target_column (str): Target column for this Model
+        """
+        self.upsert_sageworks_meta({"sageworks_model_target": target_column})
+
+    def set_features(self, feature_columns: list[str]):
+        """Set the features for this Model
+
+        Args:
+            feature_columns (list[str]): List of feature columns
+        """
+        self.upsert_sageworks_meta({"sageworks_model_features": feature_columns})
+
     def target(self) -> Union[str, None]:
         """Return the target for this Model (if supervised, else None)
 
         Returns:
             str: Target column for this Model (if supervised, else None)
         """
         return self.sageworks_meta().get("sageworks_model_target")  # Returns None if not found
@@ -451,61 +467,90 @@
             self._set_model_type(ModelType.UNSUPERVISED)
         elif model_type == "transformer":
             self._set_model_type(ModelType.TRANSFORMER)
         else:
             self.log.warning(f"Unknown Model Type {model_type}!")
             self._set_model_type(ModelType.UNKNOWN)
 
-    def onboard(self, interactive: bool = True) -> bool:
-        """This is a BLOCKING method that will onboard the Model (make it ready)
+    def onboard(self, ask_everything=False) -> bool:
+        """This is an interactive method that will onboard the Model (make it ready)
+
+        Args:
+            ask_everything (bool, optional): Ask for all the details. Defaults to False.
+
+        Returns:
+            bool: True if the Model is successfully onboarded, False otherwise
+        """
+        # Set the status to onboarding
+        self.set_status("onboarding")
+
+        # Determine the Model Type
+        while self.is_model_unknown():
+            self._determine_model_type()
+
+        # Determine the Target Column (can be None)
+        target_column = self.target()
+        if target_column is None or ask_everything:
+            target_column = input("Target Column? (for unsupervised/transformer just type None): ")
+            if target_column in ["None", "none", ""]:
+                target_column = None
+
+        # Determine the Feature Columns
+        feature_columns = self.features()
+        if feature_columns is None or ask_everything:
+            feature_columns = input("Feature Columns? (use commas): ")
+            feature_columns = [e.strip() for e in feature_columns.split(",")]
+            if feature_columns in [["None"], ["none"], [""]]:
+                feature_columns = None
+
+        # Registered Endpoints?
+        endpoints = self.endpoints()
+        if not endpoints or ask_everything:
+            endpoints = input("Register Endpoints? (use commas for multiple): ")
+            endpoints = [e.strip() for e in endpoints.split(",")]
+            if endpoints in [["None"], ["none"], [""]]:
+                endpoints = None
+
+        # Model Owner?
+        owner = self.get_owner()
+        if owner in [None, "unknown"] or ask_everything:
+            owner = input("Model Owner: ")
+            if owner in ["None", "none", ""]:
+                owner = "unknown"
+
+        # Now that we have all the details, let's onboard the Model with all the args
+        return self.onboard_with_args(self.model_type, target_column, feature_columns, endpoints, owner)
+
+    def onboard_with_args(self, model_type: ModelType, target_column: str = None, feature_list: list = None,
+                          endpoints: list = None, owner: str = None) -> bool:
+        """Onboard the Model with the given arguments
 
         Args:
-            interactive (bool, optional): If True, will prompt the user for information. Defaults to True.
+            model_type (ModelType): Model Type
+            target_column (str): Target Column
+            feature_list (list): List of Feature Columns
+            endpoints (list, optional): List of Endpoints. Defaults to None.
+            owner (str, optional): Model Owner. Defaults to None.
         Returns:
             bool: True if the Model is successfully onboarded, False otherwise
         """
         # Set the status to onboarding
         self.set_status("onboarding")
 
-        # Interactive Stuff
-        if interactive:
-            # Determine the Model Type
-            while self.is_model_unknown():
-                self._determine_model_type()
-
-            # Determine the Target Column (can be None)
-            if self.target() is None:
-                target_column = input("Target Column? (for unsupervised/transformer just type None): ")
-                if target_column in ["None", "none", ""]:
-                    target_column = None
-                self.upsert_sageworks_meta({"sageworks_model_target": target_column})
-
-            # Determine the Feature Columns
-            if self.features() is None:
-                feature_columns = input("Feature Columns? (use commas): ")
-                feature_columns = [e.strip() for e in feature_columns.split(",")]
-                if feature_columns not in [["None"], ["none"], [""]]:
-                    self.upsert_sageworks_meta({"sageworks_model_features": feature_columns})
-
-            # Registered Endpoints?
-            if not self.get_endpoints():
-                endpoints = input("Register Endpoints? (use commas for multiple): ")
-                endpoints = [e.strip() for e in endpoints.split(",")]
-                if endpoints not in [["None"], ["none"], [""]]:
-                    for endpoint in endpoints:
-                        self.log.info(f"Registering Endpoint {endpoint}...")
-                        self.register_endpoint(endpoint)
-
-            # Model Owner?
-            if self.get_owner() in [None, "unknown"]:
-                owner = input("Model Owner: ")
-                if owner in ["None", "none", ""]:
-                    self.set_owner("unknown")
-                else:
-                    self.set_owner(owner)
+        # Set All the Details
+        self._set_model_type(model_type)
+        if target_column:
+            self.set_target(target_column)
+        if feature_list:
+            self.set_features(feature_list)
+        if endpoints:
+            for endpoint in endpoints:
+                self.register_endpoint(endpoint)
+        if owner:
+            self.set_owner(owner)
 
         # Load the training metrics and inference metrics
         self._load_training_metrics()
         self._load_inference_metrics()
         self._load_inference_cm()
 
         # Remove the needs_onboard tag
```

### Comparing `sageworks-0.6.1/src/sageworks/core/artifacts/monitor_core.py` & `sageworks-0.6.2/src/sageworks/core/artifacts/monitor_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/pipelines/pipeline_executor.py` & `sageworks-0.6.2/src/sageworks/core/pipelines/pipeline_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         my_pipeline.execute_partial(["model", "endpoint"])
         ```
     """
 
     def __init__(self, pipeline):
         """PipelineExecutor Init Method"""
         self.log = logging.getLogger("sageworks")
-        self.pipeline_name = pipeline.pipeline_name
+        self.pipeline_name = pipeline.name
         self.pipeline = pipeline.pipeline
 
     def execute(self, subset: list = None):
         """Execute the SageWorks Pipeline
 
         Args:
             subset (list): A list of steps to execute. If None, execute the entire pipeline
```

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/Readme.md` & `sageworks-0.6.2/src/sageworks/core/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/light/__init__.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/light/clean_data.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py` & `sageworks-0.6.2/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/features_to_model/features_to_model.py` & `sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.6.2/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.6.2/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/__init__.py` & `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py` & `sageworks-0.6.2/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/core/transforms/transform.py` & `sageworks-0.6.2/src/sageworks/core/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/experiments/view_manager.py` & `sageworks-0.6.2/src/sageworks/experiments/view_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/repl/sageworks_shell.py` & `sageworks-0.6.2/src/sageworks/repl/sageworks_shell.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/aws_utils.py` & `sageworks-0.6.2/src/sageworks/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/cache.py` & `sageworks-0.6.2/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/chem_utils.py` & `sageworks-0.6.2/src/sageworks/utils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/config_manager.py` & `sageworks-0.6.2/src/sageworks/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/dashboard_metrics.py` & `sageworks-0.6.2/src/sageworks/utils/dashboard_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/datetime_utils.py` & `sageworks-0.6.2/src/sageworks/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.6.2/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/docker_utils.py` & `sageworks-0.6.2/src/sageworks/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/ecs_info.py` & `sageworks-0.6.2/src/sageworks/utils/ecs_info.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/endpoint_metrics.py` & `sageworks-0.6.2/src/sageworks/utils/endpoint_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/endpoint_utils.py` & `sageworks-0.6.2/src/sageworks/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/extract_model_artifact.py` & `sageworks-0.6.2/src/sageworks/utils/extract_model_artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/glue_utils.py` & `sageworks-0.6.2/src/sageworks/utils/glue_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/license_manager.py` & `sageworks-0.6.2/src/sageworks/utils/license_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/markdown_utils.py` & `sageworks-0.6.2/src/sageworks/utils/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/pandas_utils.py` & `sageworks-0.6.2/src/sageworks/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/plugin_manager.py` & `sageworks-0.6.2/src/sageworks/utils/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/redis_cache.py` & `sageworks-0.6.2/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/repl_utils.py` & `sageworks-0.6.2/src/sageworks/utils/repl_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/s3_utils.py` & `sageworks-0.6.2/src/sageworks/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/sageworks_cache.py` & `sageworks-0.6.2/src/sageworks/utils/sageworks_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.6.2/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.6.2/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.6.2/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/symbols.py` & `sageworks-0.6.2/src/sageworks/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/test_data_generator.py` & `sageworks-0.6.2/src/sageworks/utils/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/trace_calls.py` & `sageworks-0.6.2/src/sageworks/utils/trace_calls.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/utils/type_abbrev.py` & `sageworks-0.6.2/src/sageworks/utils/type_abbrev.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.6.2/src/sageworks/views/artifacts_text_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/views/artifacts_web_view.py` & `sageworks-0.6.2/src/sageworks/views/artifacts_web_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 
         Returns:
             pd.DataFrame: Summary data about the AWS Glue Jobs
         """
 
         # We get the dataframe from the ArtifactsTextView
         s3_data_df = super().incoming_data_summary()
+
+        # We might get an empty dataframe
+        if s3_data_df.empty:
+            return s3_data_df
+
+        # Add a UUID column
         s3_data_df["uuid"] = s3_data_df["Name"]
 
         # Pull the AWS URLs and construct some hyperlinks
         if add_hyperlinks:
             hyperlinked_names = []
             for name, aws_url in zip(s3_data_df["Name"], s3_data_df["_aws_url"]):
                 hyperlinked_names.append(self.hyperlinks(name, "glue_jobs", aws_url))
@@ -46,14 +52,20 @@
 
         Returns:
             pd.DataFrame: Summary data about the AWS Glue Jobs
         """
 
         # We get the dataframe from the ArtifactsTextView
         glue_df = super().glue_jobs_summary()
+
+        # We might get an empty dataframe
+        if glue_df.empty:
+            return glue_df
+
+        # Add a UUID column
         glue_df["uuid"] = glue_df["Name"]
 
         # Pull the AWS URLs and construct some hyperlinks
         if add_hyperlinks:
             hyperlinked_names = []
             for name, aws_url in zip(glue_df["Name"], glue_df["_aws_url"]):
                 hyperlinked_names.append(self.hyperlinks(name, "glue_jobs", aws_url))
@@ -71,14 +83,20 @@
 
         Returns:
             pd.DataFrame: Summary data about the SageWorks DataSources
         """
 
         # We get the dataframe from the ArtifactsTextView
         data_df = super().data_sources_summary()
+
+        # We might get an empty dataframe
+        if data_df.empty:
+            return data_df
+
+        # Add a UUID column
         data_df["uuid"] = data_df["Name"]
 
         # Pull the AWS URLs and construct some hyperlinks
         if add_hyperlinks:
             hyperlinked_names = []
             for name, aws_url in zip(data_df["Name"], data_df["_aws_url"]):
                 hyperlinked_names.append(self.hyperlinks(name, "data_sources", aws_url))
@@ -96,14 +114,20 @@
 
         Returns:
             pd.DataFrame: Summary data about the SageWorks FeatureSets
         """
 
         # We get the dataframe from the ArtifactsTextView
         feature_df = super().feature_sets_summary()
+
+        # We might get an empty dataframe
+        if feature_df.empty:
+            return feature_df
+
+        # Add a UUID column
         feature_df["uuid"] = feature_df["Feature Group"]
 
         # Pull the AWS URLs and construct some hyperlinks
         if add_hyperlinks:
             hyperlinked_names = []
             for group_name, aws_url in zip(feature_df["Feature Group"], feature_df["_aws_url"]):
                 hyperlinked_names.append(self.hyperlinks(group_name, "feature_sets", aws_url))
@@ -121,14 +145,20 @@
 
         Returns:
             pd.DataFrame: Summary data about the SageWorks Models
         """
 
         # We get the dataframe from the ArtifactsTextView and hyperlink the Model Group column
         model_df = super().models_summary()
+
+        # We might get an empty dataframe
+        if model_df.empty:
+            return model_df
+
+        # Add a UUID column
         model_df["uuid"] = model_df["Model Group"]
         if add_hyperlinks:
             model_df["Model Group"] = model_df["Model Group"].map(lambda x: self.hyperlinks(x, "models", ""))
 
         # Add Health Symbols to the Model Group Name
         if "Health" in model_df.columns:
             model_df["Health"] = model_df["Health"].map(lambda x: tag_symbols(x))
@@ -143,14 +173,20 @@
 
         Returns:
             pd.DataFrame: Summary data about the SageWorks Endpoints
         """
 
         # We get the dataframe from the ArtifactsTextView and hyperlink the Name column
         endpoint_df = super().endpoints_summary()
+
+        # We might get an empty dataframe
+        if endpoint_df.empty:
+            return endpoint_df
+
+        # Add a UUID column
         endpoint_df["uuid"] = endpoint_df["Name"]
         if add_hyperlinks:
             endpoint_df["Name"] = endpoint_df["Name"].map(lambda x: self.hyperlinks(x, "endpoints", ""))
 
         # Add Health Symbols to the Endpoint Name
         if "Health" in endpoint_df.columns:
             endpoint_df["Health"] = endpoint_df["Health"].map(lambda x: tag_symbols(x))
```

### Comparing `sageworks-0.6.1/src/sageworks/views/data_source_web_view.py` & `sageworks-0.6.2/src/sageworks/views/data_source_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/views/endpoint_web_view.py` & `sageworks-0.6.2/src/sageworks/views/endpoint_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/views/feature_set_web_view.py` & `sageworks-0.6.2/src/sageworks/views/feature_set_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/views/model_web_view.py` & `sageworks-0.6.2/src/sageworks/views/model_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/views/view.py` & `sageworks-0.6.2/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/component_interface.py` & `sageworks-0.6.2/src/sageworks/web_components/component_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,29 @@
 import plotly.graph_objects as go
 import pandas as pd
 from dash import dcc
 from dash.development.base_component import Component
 
 # SageWorks Imports
 from sageworks.api import DataSource, FeatureSet, Model, Endpoint
+from sageworks.api.pipeline import Pipeline
 
 log = logging.getLogger("sageworks")
 
 
 class ComponentInterface(ABC):
     """A Abstract Web Component Interface
     Notes:
       - The 'create_container' method create a gcc.Graph, html.Div, etc
       - The 'update_properties' method generates the property values
     """
 
     log = logging.getLogger("sageworks")
 
-    SageworksObject = Union[DataSource, FeatureSet, Model, Endpoint, pd.DataFrame]
+    SageworksObject = Union[DataSource, FeatureSet, Model, Endpoint, Pipeline, pd.DataFrame]
 
     def __init__(self):
         self.component_id = None
         self.container = None
         self.properties = []
         self.signals = []
```

### Comparing `sageworks-0.6.1/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.6.2/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/correlation_matrix.py` & `sageworks-0.6.2/src/sageworks/web_components/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/data_details_markdown.py` & `sageworks-0.6.2/src/sageworks/web_components/data_details_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/endpoint_details.py` & `sageworks-0.6.2/src/sageworks/web_components/endpoint_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/endpoint_metric_plots.py` & `sageworks-0.6.2/src/sageworks/web_components/endpoint_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/experiments/color_maps.py` & `sageworks-0.6.2/src/sageworks/web_components/experiments/color_maps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/experiments/compound_details.py` & `sageworks-0.6.2/src/sageworks/web_components/experiments/compound_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/experiments/dashboard_metric_plots.py` & `sageworks-0.6.2/src/sageworks/web_components/experiments/dashboard_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/experiments/data_table.py` & `sageworks-0.6.2/src/sageworks/web_components/experiments/data_table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/experiments/histogram.py` & `sageworks-0.6.2/src/sageworks/web_components/experiments/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/experiments/line_chart.py` & `sageworks-0.6.2/src/sageworks/web_components/experiments/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/experiments/outlier_plot.py` & `sageworks-0.6.2/src/sageworks/web_components/experiments/outlier_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/experiments/plugin_callbacks.py` & `sageworks-0.6.2/src/sageworks/web_components/experiments/plugin_callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/experiments/scatter_plot.py` & `sageworks-0.6.2/src/sageworks/web_components/experiments/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/model_details.py` & `sageworks-0.6.2/src/sageworks/web_components/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/model_plot.py` & `sageworks-0.6.2/src/sageworks/web_components/model_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/plugin_interface.py` & `sageworks-0.6.2/src/sageworks/web_components/plugin_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 class PluginPage(Enum):
     """Plugin Page: Specify which page will AUTO load the plugin (CUSTOM/NONE = Don't autoload)"""
 
     DATA_SOURCE = "data_source"
     FEATURE_SET = "feature_set"
     MODEL = "model"
     ENDPOINT = "endpoint"
+    PIPELINE = "pipeline"
     CUSTOM = "custom"
     NONE = "none"
 
 
 class PluginInputType(Enum):
     """Plugin Input Type: Specify the type of object that the plugin will receive as input"""
 
     DATA_SOURCE = "data_source"
     FEATURE_SET = "feature_set"
     MODEL = "model"
     ENDPOINT = "endpoint"
+    PIPELINE = "pipeline"
     MODEL_TABLE = "model_table"
+    PIPELINE_TABLE = "pipeline_table"
 
 
 class PluginInterface(ComponentInterface):
     """A Web Plugin Interface
     Notes:
       - The 'create_component' method must be implemented by the child class
       - The 'update_properties' method must be implemented by the child class
```

### Comparing `sageworks-0.6.1/src/sageworks/web_components/plugin_unit_test.py` & `sageworks-0.6.2/src/sageworks/web_components/plugin_unit_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dash
 from dash import html, Output, Input
 
 # SageWorks Imports
 from sageworks.web_components.plugin_interface import PluginInterface, PluginInputType
 from sageworks.api import Model, Endpoint, Meta
+from sageworks.api.pipeline import Pipeline
 
 
 class PluginUnitTest:
     def __init__(self, plugin_class):
         """A class to unit test a PluginInterface class.
 
         Args:
@@ -43,23 +44,27 @@
             [Input("update-button", "n_clicks")],
             prevent_initial_call=True,
         )
         def update_plugin_properties(n_clicks):
             # Simulate updating the plugin with a new Model, Endpoint, or Model Table
             if plugin_input_type == PluginInputType.MODEL:
                 model = Model("abalone-regression")
-                updated_proporties = self.plugin.update_properties(
-                    model, inference_run="training_holdout"
-                )  # Hardcoded for now :)
+                updated_proporties = self.plugin.update_properties(model, inference_run="training_holdout")
             elif plugin_input_type == PluginInputType.ENDPOINT:
                 endpoint = Endpoint("abalone-regression-end")
                 updated_proporties = self.plugin.update_properties(endpoint)
+            elif plugin_input_type == PluginInputType.PIPELINE:
+                pipeline = Pipeline("abalone_pipeline_v1")
+                updated_proporties = self.plugin.update_properties(pipeline)
             elif plugin_input_type == PluginInputType.MODEL_TABLE:
-                model_table = Meta().models()
-                updated_proporties = self.plugin.update_properties(model_table)
+                model_df = Meta().models()
+                updated_proporties = self.plugin.update_properties(model_df)
+            elif plugin_input_type == PluginInputType.PIPELINE_TABLE:
+                pipeline_df = Meta().pipelines()
+                updated_proporties = self.plugin.update_properties(pipeline_df)
             else:
                 raise ValueError(f"Invalid test type: {plugin_input_type}")
 
             # Return the updated properties for the plugin
             return updated_proporties
 
         # Set up callbacks for displaying output signals
```

### Comparing `sageworks-0.6.1/src/sageworks/web_components/plugins/ag_table.py` & `sageworks-0.6.2/src/sageworks/web_components/plugins/ag_table.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,34 +12,30 @@
 
 
 class AGTable(PluginInterface):
     """AGTable Component"""
 
     """Initialize this Plugin Component Class with required attributes"""
     auto_load_page = PluginPage.NONE
-    plugin_input_type = PluginInputType.MODEL_TABLE
+    plugin_input_type = PluginInputType.PIPELINE_TABLE
 
     def create_component(self, component_id: str) -> AgGrid:
         """Create a Table Component without any data.
         Args:
             component_id (str): The ID of the web component
         Returns:
             AgGrid: The Table Component using AG Grid
         """
         self.component_id = component_id
         self.container = AgGrid(
             id=component_id,
             # className="ag-theme-balham-dark",
+            className="ag-theme-alpine-auto-dark",
             columnSize="sizeToFit",
-            dashGridOptions={
-                "rowHeight": None,
-                "domLayout": "normal",
-                "rowSelection": "single",
-                "filter": True,
-            },
+            dashGridOptions={"rowSelection": "single"},
             style={"maxHeight": "200px", "overflow": "auto"},
         )
 
         # Fill in plugin properties
         self.properties = [
             (self.component_id, "columnDefs"),
             (self.component_id, "rowData"),
@@ -50,34 +46,34 @@
         self.signals = [
             (self.component_id, "selectedRows"),
         ]
 
         # Return the container
         return self.container
 
-    def update_properties(self, model_table: pd.DataFrame, **kwargs) -> list:
+    def update_properties(self, table_df: pd.DataFrame, **kwargs) -> list:
         """Update the properties for the plugin.
 
         Args:
-            model_table (pd.DataFrame): A DataFrame with the model table data
+            table_df (pd.DataFrame): A DataFrame with the table data
             **kwargs: Additional keyword arguments (unused)
 
         Returns:
             list: A list of the updated property values for the plugin
         """
-        log.important(f"Updating Table Plugin with a model table and kwargs: {kwargs}")
+        log.important(f"Updating Table Plugin with a table dataframe and kwargs: {kwargs}")
 
         # Convert the DataFrame to a list of dictionaries for AG Grid
-        table_data = model_table.to_dict("records")
+        table_data = table_df.to_dict("records")
 
         # Define column definitions based on the DataFrame
-        column_defs = [{"headerName": col, "field": col, "filter": "agTextColumnFilter"} for col in model_table.columns]
+        column_defs = [{"headerName": col, "field": col, "filter": "agTextColumnFilter"} for col in table_df.columns]
 
         # Select the first row by default
-        selected_rows = {"ids": ["0"]}
+        selected_rows = table_df.head(1).to_dict("records")
 
         # Return the column definitions and table data (must match the plugin properties)
         return [column_defs, table_data, selected_rows]
 
 
 if __name__ == "__main__":
     # Run the Unit Test for the Plugin
```

### Comparing `sageworks-0.6.1/src/sageworks/web_components/plugins/model_details.py` & `sageworks-0.6.2/src/sageworks/web_components/plugins/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/regression_plot.py` & `sageworks-0.6.2/src/sageworks/web_components/regression_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks/web_components/table.py` & `sageworks-0.6.2/src/sageworks/web_components/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,22 @@
             header_color: The color of the table header bar
             row_select (bool): If the table should be row selectable
             max_height (str): The maximum height of the table
             fixed_headers (bool): If the headers should be fixed
         Returns:
             dash_table.DataTable: A Dash DataTable Component
         """
+        # Check for transparency
+        if "transparent" in kwargs and kwargs["transparent"] is False:
+            background_color = "rgb(60, 60, 60)"
+            del kwargs["transparent"]
+        else:
+            background_color = "rgba(60, 60, 60, 0.5)"
+
+        # Create the table component
         table = dash_table.DataTable(
             id=component_id,
             columns=[{"name": "Status", "id": "status"}],
             data=[{"status": "Waiting for data..."}],
             sort_action="native",
             row_selectable=row_select,
             cell_selectable=False,
@@ -62,15 +70,15 @@
                 "backgroundColor": header_color,
                 "backgroundImage": f"linear-gradient(to bottom, {header_color}, rgba(0, 0, 0, 0.5))",
                 "color": "rgb(200, 200, 200)",
                 "border": "0px",
             },
             style_data={
                 "fontSize": 13,
-                "backgroundColor": "rgba(60, 60, 60, 0.5)",
+                "backgroundColor": background_color,
                 "color": "rgb(200, 200, 200)",
                 "border": "0px",
             },
             style_data_conditional=[{"if": {"column_id": "Health"}, "fontSize": 16, "textAlign": "left"}],
             markdown_options={"html": True},
             **kwargs,
         )
```

### Comparing `sageworks-0.6.1/src/sageworks/web_components/violin_plots.py` & `sageworks-0.6.2/src/sageworks/web_components/violin_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.6.2/src/sageworks.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.6.1
+Version: 0.6.2
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
@@ -38,31 +38,36 @@
 Requires-Dist: setuptools>=69.0.2
 Requires-Dist: pyreadline3; sys_platform == "win32"
 
 
 # Welcome to SageWorks
 The SageWorks framework makes AWS® both easier to use and more powerful. SageWorks handles all the details around updating and managing a complex set of AWS Services. With a simple-to-use Python API and a beautiful set of web interfaces, SageWorks makes creating AWS ML pipelines a snap. It also dramatically improves both the usability and visibility across the entire spectrum of services: Glue Job, Athena, Feature Store, Models, and Endpoints, SageWorks makes it easy to build production ready, AWS powered, machine learning pipelines.
 
-<img align="right" width="500" alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/ed2ed1bd-e2d8-49a1-b350-b2e19e2b7832">
+<img align="right" width="480" alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/ed2ed1bd-e2d8-49a1-b350-b2e19e2b7832">
 
 ### Full AWS ML OverView
 - Health Monitoring 🟢
 - Dynamic Updates
 - High Level Summary
 
 ### Drill-Down Views
 - Incoming Data
 - Glue Jobs
 - DataSources
 - FeatureSets
 - Models
 - Endpoints
 
+## Private SaaS Architecture
+*Secure your Data, Empower your ML Pipelines*
 
-### Installation
+SageWorks is architected as a **Private SaaS**. This hybrid architecture is the ultimate solution for businesses that prioritize data control and security. SageWorks deploys as an AWS Stack within your own cloud environment, ensuring compliance with stringent corporate and regulatory standards. It offers the flexibility to tailor solutions to your specific business needs through our comprehensive plugin support, both components and full web interfaces. By using SageWorks, you maintain absolute control over your data while benefiting from the power, security, and scalability of AWS cloud services. [SageWorks Private SaaS Architecture](https://docs.google.com/presentation/d/1f_1gmE4-UAeUDDsoNdzK_d_MxALFXIkxORZwbJBjPq4/edit?usp=sharing)
+
+
+### API Installation
 
 - ```pip install sageworks```  Installs SageWorks
 
 - ```sageworks``` Runs the SageWorks REPL/Initial Setup
 
 For the full instructions for connecting your AWS Account see:
```

### Comparing `sageworks-0.6.1/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.6.2/src/sageworks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 applications/aws_dashboard/pages/feature_sets/page.py
 applications/aws_dashboard/pages/main/callbacks.py
 applications/aws_dashboard/pages/main/layout.py
 applications/aws_dashboard/pages/main/page.py
 applications/aws_dashboard/pages/models/callbacks.py
 applications/aws_dashboard/pages/models/layout.py
 applications/aws_dashboard/pages/models/page.py
+applications/aws_dashboard/pages/pipelines/callbacks.py
+applications/aws_dashboard/pages/pipelines/layout.py
+applications/aws_dashboard/pages/pipelines/page.py
 applications/experiments/compound_explorer/Dockerfile
 applications/experiments/compound_explorer/README.md
 applications/experiments/compound_explorer/app.py
 applications/experiments/compound_explorer/callbacks.py
 applications/experiments/compound_explorer/layout.py
 applications/experiments/compound_explorer/requirements.txt
 applications/experiments/compound_explorer/assets/custom.css
@@ -106,14 +109,15 @@
 docs/api_classes/overview.md
 docs/api_classes/pipelines.md
 docs/aws_setup/aws_access_management.md
 docs/aws_setup/aws_tips_and_tricks.md
 docs/aws_setup/core_stack.md
 docs/aws_setup/dashboard_stack.md
 docs/aws_setup/full_pipeline.md
+docs/aws_setup/sso_setup.md
 docs/concepts/model_monitoring.md
 docs/core_classes/overview.md
 docs/core_classes/artifacts/artifact.md
 docs/core_classes/artifacts/athena_source.md
 docs/core_classes/artifacts/data_source_abstract.md
 docs/core_classes/artifacts/endpoint_core.md
 docs/core_classes/artifacts/feature_set_core.md
@@ -124,14 +128,17 @@
 docs/core_classes/transforms/data_loaders_light.md
 docs/core_classes/transforms/data_to_features.md
 docs/core_classes/transforms/features_to_model.md
 docs/core_classes/transforms/model_to_endpoint.md
 docs/core_classes/transforms/overview.md
 docs/core_classes/transforms/pandas_transforms.md
 docs/core_classes/transforms/transform.md
+docs/enterprise/index.md
+docs/enterprise/project_branding.md
+docs/enterprise/themes.md
 docs/glue/index.md
 docs/images/big_spider.png
 docs/images/graph_representation.png
 docs/images/powered_aws_dark_blue.png
 docs/images/powered_aws_transparent.png
 docs/images/powered_aws_white.png
 docs/images/powered_aws_with_tm_grey.png
@@ -166,14 +173,15 @@
 examples/glue/glue_hello_world_with_log.py
 examples/glue/glue_load_s3_bucket.py
 examples/meta/meta_list_endpoints.py
 examples/meta/meta_list_models.py
 examples/meta/meta_model_metrics.py
 examples/model/model_metrics.py
 examples/model/model_to_endpoint.py
+examples/model/onboard_model.py
 examples/monitor/monitor_setup.py
 examples/monitor/monitor_usage.py
 examples/pipelines/abalone_pipeline_v1.json
 examples/pipelines/abalone_pipeline_v2.json
 examples/pipelines/aqsol_pipeline_v1.json
 examples/pipelines/pipeline_details.py
 examples/pipelines/pipeline_execute.py
@@ -410,8 +418,9 @@
 tests/transforms/data_to_features_tests.py
 tests/transforms/features_to_model_tests.py
 tests/transforms/model_metrics_tests.py
 tests/transforms/model_to_endpoint_tests.py
 tests/transforms/pandas_to_data_tests.py
 tests/web_components/confusion_matrix_test.py
 tests/web_components/correlation_matrix_test.py
-tests/web_components/plugin_interface_test.py
+tests/web_components/plugin_interface_test.py
+ui_testing/table_comparison.py
```

### Comparing `sageworks-0.6.1/tests/artifacts/data_source_tests.py` & `sageworks-0.6.2/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/artifacts/endpoint_tests.py` & `sageworks-0.6.2/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/artifacts/feature_set_tests.py` & `sageworks-0.6.2/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/artifacts/model_tests.py` & `sageworks-0.6.2/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.6.2/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.6.2/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/connectors/data_catalog.py` & `sageworks-0.6.2/tests/connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/connectors/endpoints.py` & `sageworks-0.6.2/tests/connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/connectors/feature_store.py` & `sageworks-0.6.2/tests/connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/connectors/glue_jobs.py` & `sageworks-0.6.2/tests/connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/connectors/model_registry.py` & `sageworks-0.6.2/tests/connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/connectors/s3_bucket.py` & `sageworks-0.6.2/tests/connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/create_aqsol_artifacts.py` & `sageworks-0.6.2/tests/create_aqsol_artifacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,29 @@
     - aqsol_features
 Models:
     - aqsol-regression
 Endpoints:
     - aqsol-regression-end
 """
 
+import logging
 import pandas as pd
 import awswrangler as wr
 
 from sageworks.api.data_source import DataSource
 from sageworks.api.feature_set import FeatureSet
 from sageworks.api.model import Model, ModelType
 from sageworks.api.endpoint import Endpoint
 
 from sageworks.core.transforms.data_to_features.light.molecular_descriptors import MolecularDescriptors
 from sageworks.aws_service_broker.aws_service_broker import AWSServiceBroker
 
+log = logging.getLogger("sageworks")
+
+
 if __name__ == "__main__":
     # This forces a refresh on all the data we get from the AWs Broker
     AWSServiceBroker().get_all_metadata(force_refresh=True)
 
     # Get the path to the dataset in S3
     s3_path = "s3://sageworks-public-data/comp_chem/aqsol_public_data.csv"
 
@@ -90,15 +94,15 @@
     # Molecular Descriptor Artifacts
     #
     # Create the rdkit FeatureSet (this is an example of using lower level classes)
     if recreate or not FeatureSet("aqsol_mol_descriptors").exists():
         rdkit_features = MolecularDescriptors("aqsol_data", "aqsol_mol_descriptors")
         rdkit_features.set_output_tags(["aqsol", "public"])
         query = "SELECT id, solubility, solubility_class, smiles FROM aqsol_data"
-        rdkit_features.transform(target_column="solubility", id_column="id", query=query, auto_one_hot=False)
+        rdkit_features.transform(target_column="solubility", id_column="id", query=query)
 
     # Create the Molecular Descriptor based Regression Model
     if recreate or not Model("aqsol-mol-regression").exists():
         # Compute our features
         feature_set = FeatureSet("aqsol_mol_descriptors")
         exclude = ["id", "smiles", "solubility", "solubility_class"]
         feature_list = [f for f in feature_set.column_names() if f not in exclude]
@@ -125,13 +129,19 @@
             description="AQSol Descriptor Classification Model",
             tags=["aqsol", "classification"],
         )
 
     # Create the Molecular Descriptor Regression Endpoint
     if recreate or not Endpoint("aqsol-mol-regression-end").exists():
         m = Model("aqsol-mol-regression")
-        m.to_endpoint(name="aqsol-mol-regression-end", tags=["aqsol", "mol", "regression"])
+        end = m.to_endpoint(name="aqsol-mol-regression-end", tags=["aqsol", "mol", "regression"])
+
+        # Run inference on the endpoint
+        end.auto_inference(capture=True)
 
     # Create the Molecular Descriptor Classification Endpoint
     if recreate or not Endpoint("aqsol-mol-class-end").exists():
         m = Model("aqsol-mol-class")
-        m.to_endpoint(name="aqsol-mol-class-end", tags=["aqsol", "mol", "classification"])
+        end = m.to_endpoint(name="aqsol-mol-class-end", tags=["aqsol", "mol", "classification"])
+
+        # Run inference on the endpoint
+        end.auto_inference(capture=True)
```

### Comparing `sageworks-0.6.1/tests/create_basic_test_artifacts.py` & `sageworks-0.6.2/tests/create_basic_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/create_realtime_endpoint.py` & `sageworks-0.6.2/tests/create_realtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/create_training_adjusted_artifacts.py` & `sageworks-0.6.2/tests/create_training_adjusted_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/create_wine_artifacts.py` & `sageworks-0.6.2/tests/create_wine_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/delete_test_artifacts.py` & `sageworks-0.6.2/tests/delete_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/plugin_tests/crashing_plugin.py` & `sageworks-0.6.2/tests/plugin_tests/crashing_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/specific/capital_tests.py` & `sageworks-0.6.2/tests/specific/capital_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/specific/deletion_tests.py` & `sageworks-0.6.2/tests/specific/deletion_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/transforms/data_to_data_tests.py` & `sageworks-0.6.2/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/transforms/data_to_features_tests.py` & `sageworks-0.6.2/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/transforms/features_to_model_tests.py` & `sageworks-0.6.2/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/transforms/model_metrics_tests.py` & `sageworks-0.6.2/tests/transforms/model_metrics_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.6.2/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.6.2/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/web_components/confusion_matrix_test.py` & `sageworks-0.6.2/tests/web_components/confusion_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/web_components/correlation_matrix_test.py` & `sageworks-0.6.2/tests/web_components/correlation_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tests/web_components/plugin_interface_test.py` & `sageworks-0.6.2/tests/web_components/plugin_interface_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.1/tox.ini` & `sageworks-0.6.2/tox.ini`

 * *Files identical despite different names*


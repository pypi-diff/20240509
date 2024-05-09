# Comparing `tmp/kbcstorage-0.7.2.tar.gz` & `tmp/kbcstorage-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbcstorage-0.7.2.tar", last modified: Thu Jun  1 17:19:12 2023, max compression
+gzip compressed data, was "kbcstorage-0.9.0.tar", last modified: Thu May  9 12:29:58 2024, max compression
```

## Comparing `kbcstorage-0.7.2.tar` & `kbcstorage-0.9.0.tar`

### file list

```diff
@@ -1,71 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.500666 kbcstorage-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.env.template
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.476666 kbcstorage-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.480666 kbcstorage-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-01 17:19:12.496666 kbcstorage-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.484666 kbcstorage-0.7.2/kbcstorage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23903 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/kbcstorage/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.488666 kbcstorage-0.7.2/kbcstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 17:19:12.000000 kbcstorage-0.7.2/kbcstorage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:19:12.500666 kbcstorage-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.488666 kbcstorage-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/base_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.492666 kbcstorage-0.7.2/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/functional/test_workspaces_abs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:12.496666 kbcstorage-0.7.2/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/branches_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/bucket_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/component_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/configuration_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/job_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/table_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/test_workspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/token_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-01 17:19:01.000000 kbcstorage-0.7.2/tests/mocks/workspace_responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.env.template
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.764406 kbcstorage-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.764406 kbcstorage-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.768406 kbcstorage-0.9.0/kbcstorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/configurations_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24013 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/tables_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/kbcstorage/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/kbcstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 12:29:58.000000 kbcstorage-0.9.0/kbcstorage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.768406 kbcstorage-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/base_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.772406 kbcstorage-0.9.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/functional/test_workspaces_abs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:58.776406 kbcstorage-0.9.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/branches_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/bucket_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/component_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/configuration_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/job_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/table_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/test_workspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/token_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/triggers_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-09 12:29:53.000000 kbcstorage-0.9.0/tests/mocks/workspace_responses.py
```

### Comparing `kbcstorage-0.7.2/.github/workflows/push.yml` & `kbcstorage-0.9.0/.github/workflows/push.yml`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
   DOCKERHUB_USER: "keboolabot"
   DOCKERHUB_TOKEN: ${{ secrets.DOCKERHUB_TOKEN }}
   # Keboola Connection test credentials
   KBC_TEST_TOKEN: ${{ secrets.KBC_TEST_TOKEN }}
   KBC_TEST_API_URL: https://connection.keboola.com
   KBC_AZ_TEST_TOKEN: ${{ secrets.KBC_AZ_TEST_TOKEN }}
   KBC_AZ_TEST_API_URL: https://connection.north-europe.azure.keboola.com
+  KBC_GCP_TEST_TOKEN: ${{ secrets.KBC_GCP_SNOW_TEST_TOKEN }}
+  KBC_GCP_TEST_API_URL: https://connection.europe-west3.gcp.keboola.com
   APP_IMAGE: sapi-python-client
 
 jobs:
   build:
     runs-on: ubuntu-latest
     outputs:
       is_semantic_tag: ${{ steps.tag.outputs.is_semantic_tag }}
@@ -82,18 +84,36 @@
         with:
           image: "sapi-python-client"
 
       - name: Run Tests
         run: |
           docker-compose run --rm -e KBC_TEST_TOKEN=$KBC_AZ_TEST_TOKEN -e KBC_TEST_API_URL=$KBC_AZ_TEST_API_URL -e SKIP_ABS_TESTS=1 ci -m unittest --verbose
 
+  tests_gcp:
+    name: Run tests (GCP)
+    needs: build
+    runs-on: ubuntu-latest
+    steps:
+      - name: Check out the repo
+        uses: actions/checkout@v3
+
+      - name: Download image
+        uses: ishworkh/docker-image-artifact-download@v1
+        with:
+          image: "sapi-python-client"
+
+      - name: Run Tests
+        run: |
+          docker-compose run --rm -e KBC_TEST_TOKEN=$KBC_GCP_TEST_TOKEN -e KBC_TEST_API_URL=$KBC_GCP_TEST_API_URL -e SKIP_ABS_TESTS=1 ci -m unittest --verbose
+
   deploy_to_pypi:
     needs:
       - tests_aws
       - tests_azure
+      - tests_gcp
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags/') && needs.build.outputs.is_semantic_tag == 'true'
     steps:
       - name: Checkout the repo
         uses: actions/checkout@v3
 
       - name: Set up Python
```

### Comparing `kbcstorage-0.7.2/LICENSE` & `kbcstorage-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/PKG-INFO` & `kbcstorage-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbcstorage
-Version: 0.7.2
+Version: 0.9.0
 Summary: Client for Keboola Storage API
 Author-email: Keboola <developers@keboola.com>
 License: MIT License
         
         Copyright (c) Keboola :(){:|:&};: s.r.o.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3
+Requires-Dist: azure-storage-blob
+Requires-Dist: urllib3<2.0.0
+Requires-Dist: requests
+Requires-Dist: responses
+Requires-Dist: python-dotenv
+Requires-Dist: google-cloud-storage==2.16.0
+Requires-Dist: google-auth==2.29.0
 
 [![Build Status](https://travis-ci.org/keboola/sapi-python-client.svg?branch=master)](https://travis-ci.org/keboola/sapi-python-client)
 
 # Python client for the Keboola Storage API
 Client for using [Keboola Connection Storage API](http://docs.keboola.apiary.io/). This API client provides client methods to get data from KBC and store data in KBC. The endpoints 
 for working with buckets, tables and workspaces are covered.
```

### Comparing `kbcstorage-0.7.2/README.md` & `kbcstorage-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/kbcstorage/base.py` & `kbcstorage-0.9.0/kbcstorage/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,40 @@
             r.raise_for_status()
         except requests.HTTPError:
             # Handle different error codes
             raise
         else:
             return r.json()
 
+    def _put(self, *args, **kwargs):
+        """
+        Construct a requests PUT call with args and kwargs and process the
+        results.
+
+        Args:
+            *args: Positional arguments to pass to the post request.
+            **kwargs: Key word arguments to pass to the post request.
+
+        Returns:
+            body: Response body parsed from json.
+
+        Raises:
+            requests.HTTPError: If the API request fails.
+        """
+        headers = kwargs.pop('headers', {})
+        headers.update(self._auth_header)
+        r = requests.put(headers=headers, *args, **kwargs)
+        try:
+            r.raise_for_status()
+        except requests.HTTPError:
+            # Handle different error codes
+            raise
+        else:
+            return r.json()
+
     def _delete(self, *args, **kwargs):
         """
         Construct a requests DELETE call with args and kwargs and process the
         result
 
         Args:
             *args: Positional arguments to pass to the delete request.
```

### Comparing `kbcstorage-0.7.2/kbcstorage/branches.py` & `kbcstorage-0.9.0/kbcstorage/branches.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/kbcstorage/buckets.py` & `kbcstorage-0.9.0/kbcstorage/buckets.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/kbcstorage/client.py` & `kbcstorage-0.9.0/kbcstorage/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """"
 Entry point for the Storage API client.
 """
 from kbcstorage.branches import Branches
 from kbcstorage.buckets import Buckets
 from kbcstorage.components import Components
 from kbcstorage.configurations import Configurations
-from kbcstorage.tokens import Tokens
-from kbcstorage.workspaces import Workspaces
+from kbcstorage.files import Files
 from kbcstorage.jobs import Jobs
 from kbcstorage.tables import Tables
-from kbcstorage.files import Files
+from kbcstorage.tokens import Tokens
+from kbcstorage.triggers import Triggers
+from kbcstorage.workspaces import Workspaces
 
 
 class Client:
     """
     Storage API Client.
     """
 
@@ -36,14 +37,15 @@
         self.jobs = Jobs(self.root_url, self.token)
         self.tables = Tables(self.root_url, self.token)
         self.workspaces = Workspaces(self.root_url, self.token)
         self.components = Components(self.root_url, self.token, self.branch_id)
         self.configurations = Configurations(self.root_url, self.token, self.branch_id)
         self.tokens = Tokens(self.root_url, self.token)
         self.branches = Branches(self.root_url, self.token)
+        self.triggers = Triggers(self.root_url, self.token)
 
     @property
     def token(self):
         return self._token
 
     @property
     def branch_id(self):
```

### Comparing `kbcstorage-0.7.2/kbcstorage/components.py` & `kbcstorage-0.9.0/kbcstorage/components.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/kbcstorage/configurations.py` & `kbcstorage-0.9.0/kbcstorage/configurations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Manages calls to the Storage API relating to configurations
 
 Full documentation https://keboola.docs.apiary.io/#reference/components-and-configurations
 """
+import json
 from kbcstorage.base import Endpoint
+from kbcstorage.configurations_metadata import ConfigurationsMetadata
 
 
 class Configurations(Endpoint):
     """
     Configurations Endpoint
     """
 
@@ -17,14 +19,15 @@
 
         Args:
             root_url (:obj:`str`): The base url for the API.
             token (:obj:`str`): A storage API key.
             branch_id (str): The ID of branch to use, use 'default' to work without branch (in main).
         """
         super().__init__(root_url, f"branch/{branch_id}/components", token)
+        self.metadata = ConfigurationsMetadata(root_url, token, branch_id)
 
     def detail(self, component_id, configuration_id):
         """
         Retrieves information about a given configuration.
 
         Args:
             component_id (str): The id of the component.
@@ -107,10 +110,10 @@
             'description': description,
             'configuration': configuration,
             'state': state,
             'changeDescription': change_description,
             'isDisabled': is_disabled
         }
         if configuration_id:
-            body['id'] = configuration_id
+            body['configurationId'] = configuration_id
         url = '{}/{}/configs'.format(self.base_url, component_id)
-        return self._post(url, data=body)
+        return self._post(url, data=json.dumps(body), headers={'Content-Type': 'application/json'})
```

### Comparing `kbcstorage-0.7.2/kbcstorage/files.py` & `kbcstorage-0.9.0/kbcstorage/files.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import json
 import os
 import boto3
 import requests
 
 from azure.storage.blob import BlobServiceClient, ContentSettings
 from kbcstorage.base import Endpoint
+from google.oauth2 import credentials
+from google.cloud import storage as GCPStorage
 
 
 class Files(Endpoint):
     """
     Buckets Endpoint
     """
     def __init__(self, root_url, token):
@@ -82,14 +84,16 @@
         file_resource = self.prepare_upload(file_name, size, tags, is_public,
                                             is_permanent, is_encrypted,
                                             is_sliced, do_notify, True)
         if file_resource['provider'] == 'azure':
             self.__upload_to_azure(file_resource, file_path)
         elif file_resource['provider'] == 'aws':
             self.__upload_to_aws(file_resource, file_path, is_encrypted)
+        elif file_resource['provider'] == 'gcp':
+            self.__upload_to_gcp(file_resource, file_path)
 
         return file_resource['id']
 
     def prepare_upload(self, name, size_bytes=None, tags=None, is_public=False,
                        is_permanent=False, is_encrypted=True,
                        is_sliced=False, do_notify=False,
                        federation_token=True):
@@ -192,14 +196,24 @@
                 aws_session_token=file_info['credentials']['SessionToken'],
                 region_name=file_info['region']
             )
             if file_info['isSliced']:
                 self.__download_sliced_file_from_aws(file_info, local_file, s3)
             else:
                 self.__download_file_from_aws(file_info, local_file, s3)
+        elif file_info['provider'] == 'gcp':
+            storage_client = self.__get_gcp_client(
+                file_info['gcsCredentials']['access_token'],
+                file_info['gcsCredentials']['projectId'],
+            )
+
+            if file_info['isSliced']:
+                self.__download_sliced_file_from_gcp(file_info, local_file, storage_client)
+            else:
+                self.__download_file_from_gcp(file_info, local_file, storage_client)
         return local_file
 
     def __upload_to_azure(self, preparation_result, file_path):
         blob_client = self.__get_blob_client(
             preparation_result['absUploadParams']['absCredentials']['SASConnectionString'],
             preparation_result['absUploadParams']['container'],
             preparation_result['absUploadParams']['blobName']
@@ -229,14 +243,26 @@
                 encryption = upload_params['x-amz-server-side-encryption']
                 s3_object.put(ACL=upload_params['acl'], Body=file,
                               ContentDisposition=disposition, ServerSideEncryption=encryption)
             else:
                 s3_object.put(ACL=upload_params['acl'], Body=file,
                               ContentDisposition=disposition)
 
+    def __upload_to_gcp(self, preparation_result, file_path):
+        storage_client = self.__get_gcp_client(
+            preparation_result['gcsUploadParams']['access_token'],
+            preparation_result['gcsUploadParams']['projectId']
+        )
+
+        bucket = storage_client.bucket(preparation_result['gcsUploadParams']['bucket'])
+        blob = bucket.blob(preparation_result['gcsUploadParams']['key'])
+
+        with open(file_path, "rb") as blob_data:
+            blob.upload_from_file(blob_data)
+
     def __download_file_from_aws(self, file_info, destination, s3):
         bucket = s3.Bucket(file_info["s3Path"]["bucket"])
         bucket.download_file(file_info["s3Path"]["key"], destination)
 
     def __download_sliced_file_from_aws(self, file_info, destination, s3):
         manifest = requests.get(url=file_info['url']).json()
         file_names = []
@@ -277,18 +303,47 @@
             full_path = entry["url"]
             file_name = full_path.rsplit("/", 1)[1]
             file_names.append(file_name)
             with open(file_name, "wb") as file_slice:
                 file_slice.write(container_client.download_blob(blob_path).readall())
         self.__merge_split_files(file_names, destination)
 
+    def __download_file_from_gcp(self, file_info, destination, storage_client):
+
+        bucket = storage_client.bucket(file_info['gcsPath']['bucket'])
+        blob = bucket.blob(file_info['gcsPath']['key'])
+        blob.download_to_filename(destination)
+
+    def __download_sliced_file_from_gcp(self, file_info, destination, storage_client):
+        manifest = requests.get(url=file_info['url']).json()
+        file_names = []
+        for entry in manifest["entries"]:
+            full_path = entry["url"]
+            file_name = full_path.rsplit("/", 1)[1]
+            file_names.append(file_name)
+            splitted_path = full_path.split("/")
+            file_key = "/".join(splitted_path[3:])
+            bucket = storage_client.bucket(file_info['gcsPath']['bucket'])
+
+            blob = bucket.blob(file_key)
+
+            with open(file_name, "wb") as file_slice:
+                file_slice.write(blob.download_as_bytes())
+
+        self.__merge_split_files(file_names, destination)
+
     def __merge_split_files(self, file_names, destination):
         with open(destination, mode='wb') as out_file:
             for file_name in file_names:
                 with open(file_name, mode='rb') as in_file:
                     for line in in_file:
                         out_file.write(line)
                 os.remove(file_name)
 
     def __get_blob_client(self, connection_string, container, blob_name):
         blob_service_client = BlobServiceClient.from_connection_string(connection_string)
         return blob_service_client.get_blob_client(container=container, blob=blob_name)
+
+    def __get_gcp_client(self, token, project):
+        creds = credentials.Credentials(token=token)
+        gcp_storage_client = GCPStorage.Client(credentials=creds, project=project)
+        return gcp_storage_client
```

### Comparing `kbcstorage-0.7.2/kbcstorage/jobs.py` & `kbcstorage-0.9.0/kbcstorage/jobs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/kbcstorage/tables.py` & `kbcstorage-0.9.0/kbcstorage/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     http://docs.keboola.apiary.io/#reference/tables/
 """
 import tempfile
 import os
 from kbcstorage.base import Endpoint
 from kbcstorage.files import Files
 from kbcstorage.jobs import Jobs
+from kbcstorage.tables_metadata import TablesMetadata
 
 
 class Tables(Endpoint):
     """
     Tables Endpoint
     """
     def __init__(self, root_url, token):
@@ -22,14 +23,15 @@
         Create a Tables endpoint.
 
         Args:
             root_url (:obj:`str`): The base url for the API.
             token (:obj:`str`): A storage API key.
         """
         super().__init__(root_url, 'tables', token)
+        self.metadata = TablesMetadata(root_url, token)
 
     def list(self, include=None):
         """
         List all tables accessible by token.
 
         Args:
             include (list): Properties to list (attributes, columns, buckets)
```

### Comparing `kbcstorage-0.7.2/kbcstorage/tokens.py` & `kbcstorage-0.9.0/kbcstorage/tokens.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/kbcstorage/workspaces.py` & `kbcstorage-0.9.0/kbcstorage/workspaces.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/kbcstorage.egg-info/PKG-INFO` & `kbcstorage-0.9.0/kbcstorage.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbcstorage
-Version: 0.7.2
+Version: 0.9.0
 Summary: Client for Keboola Storage API
 Author-email: Keboola <developers@keboola.com>
 License: MIT License
         
         Copyright (c) Keboola :(){:|:&};: s.r.o.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,14 +29,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: boto3
+Requires-Dist: azure-storage-blob
+Requires-Dist: urllib3<2.0.0
+Requires-Dist: requests
+Requires-Dist: responses
+Requires-Dist: python-dotenv
+Requires-Dist: google-cloud-storage==2.16.0
+Requires-Dist: google-auth==2.29.0
 
 [![Build Status](https://travis-ci.org/keboola/sapi-python-client.svg?branch=master)](https://travis-ci.org/keboola/sapi-python-client)
 
 # Python client for the Keboola Storage API
 Client for using [Keboola Connection Storage API](http://docs.keboola.apiary.io/). This API client provides client methods to get data from KBC and store data in KBC. The endpoints 
 for working with buckets, tables and workspaces are covered.
```

### Comparing `kbcstorage-0.7.2/kbcstorage.egg-info/SOURCES.txt` & `kbcstorage-0.9.0/kbcstorage.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 kbcstorage/__init__.py
 kbcstorage/base.py
 kbcstorage/branches.py
 kbcstorage/buckets.py
 kbcstorage/client.py
 kbcstorage/components.py
 kbcstorage/configurations.py
+kbcstorage/configurations_metadata.py
 kbcstorage/files.py
 kbcstorage/jobs.py
 kbcstorage/tables.py
+kbcstorage/tables_metadata.py
 kbcstorage/tokens.py
+kbcstorage/triggers.py
 kbcstorage/workspaces.py
 kbcstorage.egg-info/PKG-INFO
 kbcstorage.egg-info/SOURCES.txt
 kbcstorage.egg-info/dependency_links.txt
 kbcstorage.egg-info/requires.txt
 kbcstorage.egg-info/top_level.txt
 tests/__init__.py
@@ -35,14 +38,15 @@
 tests/functional/test_buckets.py
 tests/functional/test_client.py
 tests/functional/test_components.py
 tests/functional/test_configurations.py
 tests/functional/test_files.py
 tests/functional/test_tables.py
 tests/functional/test_tokens.py
+tests/functional/test_triggers.py
 tests/functional/test_workspaces.py
 tests/functional/test_workspaces_abs.py
 tests/mocks/__init__.py
 tests/mocks/branches_responses.py
 tests/mocks/bucket_responses.py
 tests/mocks/component_responses.py
 tests/mocks/configuration_responses.py
@@ -52,10 +56,12 @@
 tests/mocks/test_buckets.py
 tests/mocks/test_client.py
 tests/mocks/test_components.py
 tests/mocks/test_configurations.py
 tests/mocks/test_jobs.py
 tests/mocks/test_tables.py
 tests/mocks/test_tokens.py
+tests/mocks/test_triggers.py
 tests/mocks/test_workspaces.py
 tests/mocks/token_responses.py
+tests/mocks/triggers_responses.py
 tests/mocks/workspace_responses.py
```

### Comparing `kbcstorage-0.7.2/pyproject.toml` & `kbcstorage-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -22,12 +22,14 @@
     "boto3",
     "azure-storage-blob",
     "urllib3<2.0.0",  # Frozen until fixed: https://github.com/boto/botocore/issues/2926
     # Dev dependencies
     "requests",
     "responses",
     "python-dotenv",
+    "google-cloud-storage==2.16.0",
+    "google-auth==2.29.0"
 ]
 dynamic = ["version"]
 
 [tool.setuptools-git-versioning]
 enabled = true
```

### Comparing `kbcstorage-0.7.2/tests/base_test_case.py` & `kbcstorage-0.9.0/tests/base_test_case.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/functional/test_base.py` & `kbcstorage-0.9.0/tests/functional/test_base.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/functional/test_buckets.py` & `kbcstorage-0.9.0/tests/functional/test_buckets.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/functional/test_client.py` & `kbcstorage-0.9.0/tests/functional/test_client.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/functional/test_components.py` & `kbcstorage-0.9.0/tests/functional/test_components.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/functional/test_configurations.py` & `kbcstorage-0.9.0/tests/functional/test_configurations.py`

 * *Files 24% similar despite different names*

```diff
@@ -46,7 +46,60 @@
                 self.assertTrue('name' in configuration)
                 self.assertTrue('description' in configuration)
                 self.assertTrue('configuration' in configuration)
 
         with self.subTest():
             with self.assertRaises(exceptions.HTTPError):
                 configurations = self.configurations.list('non-existent-component')
+
+    def testConfigurationMetadata(self):
+        self.configurations.create(
+            component_id=self.TEST_COMPONENT_NAME,
+            configuration_id='test_configuration_metadata',
+            name='test_configuration_metadata',
+        )
+        metadataPayload = [
+            {
+                'key': 'testConfigurationMetadata',
+                'value': 'success',
+            }
+        ]
+        metadataList = self.configurations.metadata.create(
+            component_id=self.TEST_COMPONENT_NAME,
+            configuration_id='test_configuration_metadata',
+            provider='test',
+            metadata=metadataPayload,
+        )
+
+        with (self.subTest('assert metadata create response')):
+            self.assertEqual(1, len(metadataList))
+            metadataItem = metadataList[0]
+            self.assertTrue('id' in metadataItem)
+            # self.assertTrue('provider' in metadata) not yet
+            self.assertTrue('key' in metadataItem)
+            self.assertTrue('value' in metadataItem)
+
+            metadataList = self.configurations.metadata.list(
+                component_id=self.TEST_COMPONENT_NAME,
+                configuration_id='test_configuration_metadata'
+            )
+
+        with (self.subTest('assert metadata list response')):
+            self.assertTrue(len(metadataList) > 0)
+            for metadataList in metadataList:
+                self.assertTrue('id' in metadataList)
+                # self.assertTrue('provider' in metadata) not yet
+                self.assertTrue('key' in metadataList)
+                self.assertTrue('value' in metadataList)
+
+        self.configurations.metadata.delete(
+            component_id=self.TEST_COMPONENT_NAME,
+            configuration_id='test_configuration_metadata',
+            metadata_id=metadataList['id']
+        )
+        metadataList = self.configurations.metadata.list(
+            component_id=self.TEST_COMPONENT_NAME,
+            configuration_id='test_configuration_metadata'
+        )
+
+        with (self.subTest('assert metadata delete means metadata no longer in list')):
+            self.assertTrue(len(metadataList) == 0)
```

### Comparing `kbcstorage-0.7.2/tests/functional/test_files.py` & `kbcstorage-0.9.0/tests/functional/test_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         file_id = self.files.upload_file(path, tags=['py-test', 'file1'])
         os.close(file)
         time.sleep(1)
         file_info = self.files.detail(file_id, federation_token=True)
         with self.subTest():
             self.assertEqual(file_id, file_info['id'])
         with self.subTest():
-            self.assertTrue(file_info['provider'] in ['aws', 'azure'])
+            self.assertTrue(file_info['provider'] in ['aws', 'azure', 'gcp'])
         if file_info['provider'] == 'aws':
             with self.subTest():
                 self.assertTrue('credentials' in file_info)
             with self.subTest():
                 self.assertTrue('AccessKeyId' in file_info['credentials'])
             with self.subTest():
                 self.assertTrue('SecretAccessKey' in file_info['credentials'])
```

### Comparing `kbcstorage-0.7.2/tests/functional/test_tokens.py` & `kbcstorage-0.9.0/tests/functional/test_tokens.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/functional/test_workspaces.py` & `kbcstorage-0.9.0/tests/functional/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/functional/test_workspaces_abs.py` & `kbcstorage-0.9.0/tests/functional/test_workspaces_abs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/bucket_responses.py` & `kbcstorage-0.9.0/tests/mocks/bucket_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/component_responses.py` & `kbcstorage-0.9.0/tests/mocks/component_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/configuration_responses.py` & `kbcstorage-0.9.0/tests/mocks/configuration_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/job_responses.py` & `kbcstorage-0.9.0/tests/mocks/job_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/table_responses.py` & `kbcstorage-0.9.0/tests/mocks/table_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/test_branches.py` & `kbcstorage-0.9.0/tests/mocks/test_branches.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/test_buckets.py` & `kbcstorage-0.9.0/tests/mocks/test_buckets.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/test_client.py` & `kbcstorage-0.9.0/tests/mocks/test_client.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/test_components.py` & `kbcstorage-0.9.0/tests/mocks/test_components.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/test_configurations.py` & `kbcstorage-0.9.0/tests/mocks/test_configurations.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/test_jobs.py` & `kbcstorage-0.9.0/tests/mocks/test_jobs.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/test_tables.py` & `kbcstorage-0.9.0/tests/mocks/test_tables.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/test_tokens.py` & `kbcstorage-0.9.0/tests/mocks/test_tokens.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/test_workspaces.py` & `kbcstorage-0.9.0/tests/mocks/test_workspaces.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/token_responses.py` & `kbcstorage-0.9.0/tests/mocks/token_responses.py`

 * *Files identical despite different names*

### Comparing `kbcstorage-0.7.2/tests/mocks/workspace_responses.py` & `kbcstorage-0.9.0/tests/mocks/workspace_responses.py`

 * *Files identical despite different names*


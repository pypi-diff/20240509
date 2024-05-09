# Comparing `tmp/ape-etherscan-0.7.2.tar.gz` & `tmp/ape-etherscan-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-etherscan-0.7.2.tar", last modified: Fri Mar  8 23:05:58 2024, max compression
+gzip compressed data, was "ape-etherscan-0.7.3.tar", last modified: Thu May  9 01:59:02 2024, max compression
```

## Comparing `ape-etherscan-0.7.2.tar` & `ape-etherscan-0.7.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:05:58.972792 ape-etherscan-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:05:58.968792 ape-etherscan-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:05:58.968792 ape-etherscan-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:05:58.968792 ape-etherscan-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-03-08 23:05:58.972792 ape-etherscan-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:05:58.968792 ape-etherscan-0.7.2/ape_etherscan/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15812 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/ape_etherscan/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-08 23:05:58.000000 ape-etherscan-0.7.2/ape_etherscan/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:05:58.972792 ape-etherscan-0.7.2/ape_etherscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-03-08 23:05:58.000000 ape-etherscan-0.7.2/ape_etherscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-08 23:05:58.000000 ape-etherscan-0.7.2/ape_etherscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 23:05:58.000000 ape-etherscan-0.7.2/ape_etherscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 23:05:58.000000 ape-etherscan-0.7.2/ape_etherscan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-08 23:05:58.000000 ape-etherscan-0.7.2/ape_etherscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-08 23:05:58.000000 ape-etherscan-0.7.2/ape_etherscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-08 23:05:58.972792 ape-etherscan-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:05:58.972792 ape-etherscan-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21787 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 23:05:58.972792 ape-etherscan-0.7.2/tests/mock_responses/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/mock_responses/get_account_transactions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/mock_responses/get_account_transactions_with_ctor_args.json
--rw-r--r--   0 runner    (1001) docker     (127)    85182 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/mock_responses/get_contract_response_flattened.json
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/mock_responses/get_contract_response_json.json
--rw-r--r--   0 runner    (1001) docker     (127)    21603 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/mock_responses/get_contract_response_json_source_code.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/mock_responses/get_contract_response_not_verified.json
--rw-r--r--   0 runner    (1001) docker     (127)    93453 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/mock_responses/get_proxy_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (127)    93483 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/mock_responses/get_vyper_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-03-08 23:04:57.000000 ape-etherscan-0.7.2/tests/test_etherscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.611034 ape-etherscan-0.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.603034 ape-etherscan-0.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.603034 ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.607034 ape-etherscan-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-09 01:59:02.611034 ape-etherscan-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.607034 ape-etherscan-0.7.3/ape_etherscan/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/ape_etherscan/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.607034 ape-etherscan-0.7.3/ape_etherscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 01:59:02.000000 ape-etherscan-0.7.3/ape_etherscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 01:59:02.611034 ape-etherscan-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.607034 ape-etherscan-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:59:02.611034 ape-etherscan-0.7.3/tests/mock_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_account_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_account_transactions_with_ctor_args.json
+-rw-r--r--   0 runner    (1001) docker     (127)    85182 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_flattened.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21603 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_json_source_code.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_not_verified.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93453 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_proxy_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93483 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/mock_responses/get_vyper_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-09 01:58:10.000000 ape-etherscan-0.7.3/tests/test_etherscan.py
```

### Comparing `ape-etherscan-0.7.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-etherscan-0.7.3/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/.github/release-drafter.yml` & `ape-etherscan-0.7.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/.github/workflows/codeql.yml` & `ape-etherscan-0.7.3/.github/workflows/codeql.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       security-events: write
 
     strategy:
       fail-fast: false
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Initialize CodeQL
       uses: github/codeql-action/init@v2
       with:
         languages: python
 
     - name: Autobuild
```

### Comparing `ape-etherscan-0.7.2/.github/workflows/commit.yaml` & `ape-etherscan-0.7.3/.github/workflows/commit.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check commit history
```

### Comparing `ape-etherscan-0.7.2/.github/workflows/prtitle.yaml` & `ape-etherscan-0.7.3/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-etherscan-0.7.2/.github/workflows/publish.yaml` & `ape-etherscan-0.7.3/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ape-etherscan-0.7.2/.github/workflows/stale-prs.yml` & `ape-etherscan-0.7.3/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/.github/workflows/test.yaml` & `ape-etherscan-0.7.3/.github/workflows/test.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,18 @@
   cancel-in-progress: true
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
@@ -38,18 +38,18 @@
         - name: Run mdformat
           run: mdformat . --check
 
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
@@ -58,22 +58,24 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
+                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
@@ -87,18 +89,18 @@
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v2
+#        - uses: actions/checkout@v4
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v2
+#          uses: actions/setup-python@v5
 #          with:
 #              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ape-etherscan-0.7.2/.gitignore` & `ape-etherscan-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/.pre-commit-config.yaml` & `ape-etherscan-0.7.3/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
--   repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.10.1
+-   repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.0
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-PyYAML, types-requests, types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-etherscan-0.7.2/CONTRIBUTING.md` & `ape-etherscan-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/LICENSE` & `ape-etherscan-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/PKG-INFO` & `ape-etherscan-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.7.2
+Version: 0.7.3
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -40,15 +41,15 @@
 - [Snowtrace](https://snowtrace.io) for Avalanche networks.
 - [Basescan](https://basescan.org) for Base networks.
 - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
 - [Blastscan](https://blastscan.io) for Blast networks.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-etherscan-0.7.2/README.md` & `ape-etherscan-0.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - [Snowtrace](https://snowtrace.io) for Avalanche networks.
 - [Basescan](https://basescan.org) for Base networks.
 - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
 - [Blastscan](https://blastscan.io) for Blast networks.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-etherscan-0.7.2/ape_etherscan/__init__.py` & `ape-etherscan-0.7.3/ape_etherscan/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/ape_etherscan/client.py` & `ape-etherscan-0.7.3/ape_etherscan/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,25 +69,27 @@
             if network_name == "mainnet"
             else f"https://{network_name}-optimism.etherscan.io"
         )
     elif ecosystem_name == "polygon-zkevm":
         return (
             "https://zkevm.polygonscan.com"
             if network_name == "mainnet"
-            else "https://testnet-zkevm.polygonscan.com"
+            else "https://cardona-zkevm.polygonscan.com"
         )
     elif ecosystem_name == "base":
         return (
-            "https://basescan.org" if network_name == "mainnet" else "https://goerli.basescan.org"
+            f"https://{network_name}.basescan.org"
+            if network_name != "mainnet"
+            else "https://basescan.org"
         )
     elif ecosystem_name == "polygon":
         return (
             "https://polygonscan.com"
             if network_name == "mainnet"
-            else "https://mumbai.polygonscan.com"
+            else "https://amoy.polygonscan.com"
         )
     elif ecosystem_name == "avalanche":
         return (
             "https://snowtrace.io" if network_name == "mainnet" else "https://testnet.snowtrace.io"
         )
     elif ecosystem_name == "bsc":
         return (
@@ -141,21 +143,21 @@
             if network_name == "mainnet"
             else f"https://api-{network_name}-optimistic.etherscan.io/api"
         )
     elif ecosystem_name == "polygon-zkevm":
         return (
             "https://api-zkevm.polygonscan.com/api"
             if network_name == "mainnet"
-            else "https://api-testnet-zkevm.polygonscan.com/api"
+            else "https://api-cardona-zkevm.polygonscan.com/api"
         )
     elif ecosystem_name == "base":
         return (
-            "https://api.basescan.org/api"
-            if network_name == "mainnet"
-            else "https://api-goerli.basescan.org/api"
+            f"https://api-{network_name}.basescan.org/api"
+            if network_name != "mainnet"
+            else "https://api.basescan.org/api"
         )
     elif ecosystem_name == "polygon":
         return (
             "https://api.polygonscan.com/api"
             if network_name == "mainnet"
             else "https://api-testnet.polygonscan.com/api"
         )
```

### Comparing `ape-etherscan-0.7.2/ape_etherscan/config.py` & `ape-etherscan-0.7.3/ape_etherscan/config.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/ape_etherscan/dependency.py` & `ape-etherscan-0.7.3/ape_etherscan/dependency.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/ape_etherscan/exceptions.py` & `ape-etherscan-0.7.3/ape_etherscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/ape_etherscan/explorer.py` & `ape-etherscan-0.7.3/ape_etherscan/explorer.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/ape_etherscan/query.py` & `ape-etherscan-0.7.3/ape_etherscan/query.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/ape_etherscan/types.py` & `ape-etherscan-0.7.3/ape_etherscan/types.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/ape_etherscan/utils.py` & `ape-etherscan-0.7.3/ape_etherscan/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,49 +10,47 @@
     "optimism": "OPTIMISTIC_ETHERSCAN_API_KEY",
     "polygon": "POLYGONSCAN_API_KEY",
     "polygon-zkevm": "POLYGON_ZKEVM_ETHERSCAN_API_KEY",
 }
 NETWORKS = {
     "arbitrum": [
         "mainnet",
-        "goerli",
+        "sepolia",
     ],
     "avalanche": [
         "mainnet",
         "fuji",
     ],
     "base": [
         "mainnet",
-        "goerli",
+        "sepolia",
     ],
     "blast": [
         "mainnet",
         "sepolia",
     ],
     "bsc": [
         "mainnet",
         "testnet",
     ],
     "ethereum": [
         "mainnet",
-        "goerli",
         "sepolia",
     ],
     "fantom": [
         "opera",
         "testnet",
     ],
     "gnosis": ["mainnet"],
     "optimism": [
         "mainnet",
-        "goerli",
         "sepolia",
     ],
     "polygon": [
         "mainnet",
-        "mumbai",
+        "amoy",
     ],
     "polygon-zkevm": [
         "mainnet",
-        "goerli",
+        "cardona",
     ],
 }
```

### Comparing `ape-etherscan-0.7.2/ape_etherscan/verify.py` & `ape-etherscan-0.7.3/ape_etherscan/verify.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,15 +253,38 @@
 
         Raises:
             :class:`~ape_etherscan.exceptions.ContractVerificationError`: - When fails
               to validate the contract.
         """
 
         version = str(self.compiler.version)
-        settings = self.compiler.settings or self._get_new_settings(version)
+
+        # TODO: Fix compiler output in ape-solidity
+        #  and/or add more validation to ethpm_types.Compiler
+        compiler = self.compiler
+        valid = True
+        settings = {}
+        if compiler:
+            settings = self.compiler.settings or {}
+            output_contracts = settings.get("outputSelection", {})
+            for contract_id in self.compiler.contractTypes or []:
+                parts = contract_id.split(":")
+                if len(parts) != 2:
+                    # Bad compiler.
+                    valid = False
+                    continue
+
+                _, cname = parts
+                if cname not in output_contracts:
+                    valid = False
+                    break
+
+        if not valid:
+            settings = self._get_new_settings(version)
+
         optimizer = settings.get("optimizer", {})
         optimized = optimizer.get("enabled", False)
         runs = optimizer.get("runs", DEFAULT_OPTIMIZATION_RUNS)
         source_id = self.contract_type.source_id
         base_folder = self.project_manager.contracts_folder
         standard_input_json = self._get_standard_input_json(source_id, base_folder, **settings)
         evm_version = settings.get("evmVersion")
```

### Comparing `ape-etherscan-0.7.2/ape_etherscan.egg-info/PKG-INFO` & `ape-etherscan-0.7.3/ape_etherscan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.7.2
+Version: 0.7.3
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -40,15 +41,15 @@
 - [Snowtrace](https://snowtrace.io) for Avalanche networks.
 - [Basescan](https://basescan.org) for Base networks.
 - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
 - [Blastscan](https://blastscan.io) for Blast networks.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-etherscan-0.7.2/ape_etherscan.egg-info/SOURCES.txt` & `ape-etherscan-0.7.3/ape_etherscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/ape_etherscan.egg-info/requires.txt` & `ape-etherscan-0.7.3/ape_etherscan.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 ape-infura
 ape-solidity
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7,>=6.2.0
 pytest-mock
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-requests>=2.28.7
 types-setuptools
 types-PyYAML
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
@@ -47,23 +47,23 @@
 
 [doc]
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-requests>=2.28.7
 types-setuptools
 types-PyYAML
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
```

### Comparing `ape-etherscan-0.7.2/pyproject.toml` & `ape-etherscan-0.7.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-etherscan-0.7.2/setup.py` & `ape-etherscan-0.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7",  # Strategy-based fuzzer
         "pytest-mock",  # Test mocker
     ],
     "lint": [
-        "black>=23.12.0,<24",  # auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-requests>=2.28.7",  # Needed due to mypy typeshed
         "types-setuptools",  # Needed due to mypy typeshed
         "types-PyYAML",  # Needed due to mypy typeshed
-        "flake8>=6.1.0,<7",  # Style linter
+        "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "doc": [
         "Sphinx>=6.1.3,<7",  # Documentation generator
@@ -101,9 +101,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-etherscan-0.7.2/tests/conftest.py` & `ape-etherscan-0.7.3/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,19 @@
         "libraryaddress1": library.address,
     }
 
 
 @pytest.fixture(autouse=True)
 def connection(explorer):
     with ape.networks.ethereum.mainnet.use_provider("infura") as provider:
+        # TODO: Figure out why this is still needed sometimes,
+        #   even after https://github.com/ApeWorX/ape/pull/2022
+        if not provider.is_connected:
+            provider.connect()
+
         yield provider
 
 
 @pytest.fixture
 def mock_provider(mocker):
     @contextmanager
     def func(ecosystem_name="ethereum", network_name="mock"):
@@ -271,45 +276,43 @@
         org_url = get_url_f(tld="org")
         com_testnet_url = get_url_f(testnet=True, tld="com")
         org_testnet_url = get_url_f(testnet=True, tld="org")
 
         return {
             "ethereum": {
                 "mainnet": url("etherscan"),
-                "goerli": testnet_url("goerli", "etherscan"),
                 "sepolia": testnet_url("sepolia", "etherscan"),
             },
             "arbitrum": {
                 "mainnet": url("arbiscan"),
-                "goerli": testnet_url("goerli", "arbiscan"),
+                "sepolia": testnet_url("sepolia", "arbiscan"),
             },
             "fantom": {
                 "opera": com_url("ftmscan"),
                 "testnet": com_testnet_url("testnet", "ftmscan"),
             },
             "optimism": {
                 "mainnet": testnet_url("optimistic", "etherscan"),
-                "goerli": testnet_url("goerli-optimistic", "etherscan"),
                 "sepolia": testnet_url("sepolia-optimistic", "etherscan"),
             },
             "polygon": {
                 "mainnet": com_url("polygonscan"),
-                "mumbai": com_testnet_url("testnet", "polygonscan"),
+                "amoy": com_testnet_url("testnet", "polygonscan"),
             },
             "base": {
-                "goerli": org_testnet_url("goerli", "basescan"),
+                "sepolia": org_testnet_url("sepolia", "basescan"),
                 "mainnet": org_url("basescan"),
             },
             "blast": {
                 "sepolia": testnet_url("sepolia", "blastscan"),
                 "mainnet": url("blastscan"),
             },
             "polygon-zkevm": {
                 "mainnet": com_testnet_url("zkevm", "polygonscan"),
-                "goerli": com_testnet_url("testnet-zkevm", "polygonscan"),
+                "cardona": com_testnet_url("cardona-zkevm", "polygonscan"),
             },
             "avalanche": {"mainnet": url("snowtrace"), "fuji": testnet_url("testnet", "snowtrace")},
             "bsc": {
                 "mainnet": com_url("bscscan"),
                 "testnet": com_testnet_url("testnet", "bscscan"),
             },
             "gnosis": {
```

### Comparing `ape-etherscan-0.7.2/tests/mock_responses/get_account_transactions.json` & `ape-etherscan-0.7.3/tests/mock_responses/get_account_transactions.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/tests/mock_responses/get_account_transactions_with_ctor_args.json` & `ape-etherscan-0.7.3/tests/mock_responses/get_account_transactions_with_ctor_args.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/tests/mock_responses/get_contract_response_flattened.json` & `ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_flattened.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/tests/mock_responses/get_contract_response_json.json` & `ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_json.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/tests/mock_responses/get_contract_response_json_source_code.json` & `ape-etherscan-0.7.3/tests/mock_responses/get_contract_response_json_source_code.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/tests/mock_responses/get_proxy_contract_response.json` & `ape-etherscan-0.7.3/tests/mock_responses/get_proxy_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/tests/mock_responses/get_vyper_contract_response.json` & `ape-etherscan-0.7.3/tests/mock_responses/get_vyper_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/tests/test_config.py` & `ape-etherscan-0.7.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/tests/test_dependency.py` & `ape-etherscan-0.7.3/tests/test_dependency.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.2/tests/test_etherscan.py` & `ape-etherscan-0.7.3/tests/test_etherscan.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,39 +19,36 @@
 PUBLISH_GUID = "123"
 
 base_url_test = pytest.mark.parametrize(
     "ecosystem,network,url",
     [
         ("ethereum", "mainnet", "etherscan.io"),
         ("ethereum", "mainnet-fork", "etherscan.io"),
-        ("ethereum", "goerli", "goerli.etherscan.io"),
-        ("ethereum", "goerli-fork", "goerli.etherscan.io"),
         ("ethereum", "sepolia", "sepolia.etherscan.io"),
+        ("ethereum", "sepolia-fork", "sepolia.etherscan.io"),
         ("fantom", "opera", "ftmscan.com"),
         ("fantom", "opera-fork", "ftmscan.com"),
         ("fantom", "testnet", "testnet.ftmscan.com"),
         ("fantom", "testnet-fork", "testnet.ftmscan.com"),
         ("arbitrum", "mainnet", "arbiscan.io"),
         ("arbitrum", "mainnet-fork", "arbiscan.io"),
-        ("arbitrum", "goerli", "goerli.arbiscan.io"),
-        ("arbitrum", "goerli-fork", "goerli.arbiscan.io"),
+        ("arbitrum", "sepolia", "sepolia.arbiscan.io"),
+        ("arbitrum", "sepolia-fork", "sepolia.arbiscan.io"),
         ("optimism", "mainnet", "optimistic.etherscan.io"),
         ("optimism", "mainnet-fork", "optimistic.etherscan.io"),
-        ("optimism", "goerli", "goerli-optimism.etherscan.io"),
-        ("optimism", "goerli-fork", "goerli-optimism.etherscan.io"),
         ("optimism", "sepolia", "sepolia-optimism.etherscan.io"),
         ("optimism", "sepolia-fork", "sepolia-optimism.etherscan.io"),
         ("polygon", "mainnet", "polygonscan.com"),
         ("polygon", "mainnet-fork", "polygonscan.com"),
-        ("polygon", "mumbai", "mumbai.polygonscan.com"),
-        ("polygon", "mumbai-fork", "mumbai.polygonscan.com"),
+        ("polygon", "amoy", "amoy.polygonscan.com"),
+        ("polygon", "amoy-fork", "amoy.polygonscan.com"),
         ("polygon-zkevm", "mainnet", "zkevm.polygonscan.com"),
-        ("polygon-zkevm", "goerli", "testnet-zkevm.polygonscan.com"),
+        ("polygon-zkevm", "cardona", "cardona-zkevm.polygonscan.com"),
         ("base", "mainnet", "basescan.org"),
-        ("base", "goerli", "goerli.basescan.org"),
+        ("base", "sepolia", "sepolia.basescan.org"),
         ("blast", "mainnet", "blastscan.io"),
         ("blast", "sepolia", "sepolia.blastscan.io"),
         ("avalanche", "mainnet", "snowtrace.io"),
         ("avalanche", "fuji", "testnet.snowtrace.io"),
         ("bsc", "mainnet", "bscscan.com"),
         ("bsc", "mainnet-fork", "bscscan.com"),
         ("bsc", "testnet", "testnet.bscscan.com"),
@@ -172,29 +169,31 @@
     expected = EXPECTED_CONTRACT_NAME_MAP[response.file_name]
     assert actual == expected
 
 
 @pytest.mark.parametrize(
     "file_name", ("get_proxy_contract_response", ("get_vyper_contract_response"))
 )
-def test_get_contract_type_additional_types(mock_backend, file_name, explorer):
+def test_get_contract_type_additional_types(mock_backend, file_name, explorer, connection):
     # This test parametrizes getting edge-case contract types.
     # NOTE: Purposely not merged with test above to avoid adding a new dimension
     #  to the parametrization.
+    _ = connection  # Needed for symbol lookup
+    mock_backend.set_network("ethereum", "mainnet")
     response = mock_backend.setup_mock_get_contract_type_response(file_name)
     actual = explorer.get_contract_type(response.expected_address).name
     expected = EXPECTED_CONTRACT_NAME_MAP[response.file_name]
     assert actual == expected
 
 
-def test_get_contract_type_with_rate_limiting(mock_backend, explorer):
+def test_get_contract_type_with_rate_limiting(mock_backend, explorer, connection):
     """
     This test ensures the rate limiting logic in the Etherscan client works.
     """
-
+    _ = connection  # Needed for calling symbol() on Vyper_contract
     file_name = "get_vyper_contract_response"
     setter_upper = mock_backend.setup_mock_get_contract_type_response_with_throttling
     throttler, response = setter_upper(file_name)
 
     # We still eventually get the response.
     actual = explorer.get_contract_type(response.expected_address).name
     expected = EXPECTED_CONTRACT_NAME_MAP[response.file_name]
```


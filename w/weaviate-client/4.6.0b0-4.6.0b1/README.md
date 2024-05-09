# Comparing `tmp/weaviate_client-4.6.0b0.tar.gz` & `tmp/weaviate_client-4.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaviate_client-4.6.0b0.tar", last modified: Tue May  7 02:24:12 2024, max compression
+gzip compressed data, was "weaviate_client-4.6.0b1.tar", last modified: Tue May  7 23:24:40 2024, max compression
```

## Comparing `weaviate_client-4.6.0b0.tar` & `weaviate_client-4.6.0b1.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.791950 weaviate_client-4.6.0b0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.791950 weaviate_client-4.6.0b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.795950 weaviate_client-4.6.0b0/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/compose.sh
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-async.yml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-azure.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-cluster.yml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-generative.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-okta-cc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-okta-users.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-proxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-rerank.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose-wcs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.795950 weaviate_client-4.6.0b0/ci/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/proxy/envoy.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      922 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/start_weaviate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/ci/stop_weaviate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.799950 weaviate_client-4.6.0b0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    56116 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.backup.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.classification.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.client.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.cluster.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.aggregations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.classes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.grpc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.collections.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.connect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.contextionary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.data.references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.data.replication.rst
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.gql.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.proto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.proto.v1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.schema.properties.rst
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/docs/weaviate.util.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.803950 weaviate_client-4.6.0b0/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/1234.3gp
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/hobbits.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_batch_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    78466 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31180 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    33149 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_multi_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_collection_rerank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_gql_raw_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/test_tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration/weaviate-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.803950 weaviate_client-4.6.0b0/integration_embedded/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_embedded/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.807950 weaviate_client-4.6.0b0/integration_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/people_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_backup_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_grcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/integration_v3/test_timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.807950 weaviate_client-4.6.0b0/mock_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_automatic_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_batching_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_resend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/mock_tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/test_import_and_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/test_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/profiling/test_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/publishing.md
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/run-mypy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/batch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/batch/test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/classification/test_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/cluster/test_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.811950 weaviate_client-4.6.0b0/test/collection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_byteops.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    36501 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/collection/test_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/connection/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/contextionary/test_text2vec_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/data/references/test_crud_references.py
--rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/data/test_crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/gql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/gql/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.815950 weaviate_client-4.6.0b0/test/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/properties/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/schema_company.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/tenants.json
--rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/schema/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_server_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/test/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/backup/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/batch/crud_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/batch/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classes/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/classification/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22119 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.819950 weaviate_client-4.6.0b0/weaviate/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/cluster/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.823950 weaviate_client-4.6.0b0/weaviate/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.823950 weaviate_client-4.6.0b0/weaviate/collections/aggregations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/aggregations/over_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.827950 weaviate_client-4.6.0b0/weaviate/collections/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27772 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/batch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/grpc_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/grpc_batch_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/batch/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.827950 weaviate_client-4.6.0b0/weaviate/collections/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    69063 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    38971 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_vector_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    39194 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/config_vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19528 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/classes/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.827950 weaviate_client-4.6.0b0/weaviate/collections/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28802 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/grpc/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/grpc/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/grpc/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/byteops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.831950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/collections/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.835950 weaviate_client-4.6.0b0/weaviate/connect/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/connect/v4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/contextionary/crud_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/data/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/references/crud_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/data/replication/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/data/replication/replication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/error_msgs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/gql/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42084 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/multi_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/gql/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/outputs/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.839950 weaviate_client-4.6.0b0/weaviate/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.843950 weaviate_client-4.6.0b0/weaviate/proto/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/properties_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/properties_pb2_grpc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/regen.sh
--rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/tenants_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/tenants_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/tenants_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.843950 weaviate_client-4.6.0b0/weaviate/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/schema/crud_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/weaviate/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/schema/properties/crud_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-05-07 02:23:50.000000 weaviate_client-4.6.0b0/weaviate/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:24:12.847950 weaviate_client-4.6.0b0/weaviate_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 02:24:12.000000 weaviate_client-4.6.0b0/weaviate_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.756159 weaviate_client-4.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.692159 weaviate_client-4.6.0b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.692159 weaviate_client-4.6.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-07 23:24:40.756159 weaviate_client-4.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.696159 weaviate_client-4.6.0b1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/compose.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose-async.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose-azure.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose-cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose-generative.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose-okta-cc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose-okta-users.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose-proxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose-rerank.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose-wcs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.696159 weaviate_client-4.6.0b1/ci/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/proxy/envoy.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      922 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/start_weaviate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/ci/stop_weaviate.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.700159 weaviate_client-4.6.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    56116 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.backup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.classification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.collections.aggregations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.collections.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.collections.classes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.collections.grpc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.collections.queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.collections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.connect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.contextionary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.data.references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.data.replication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.gql.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.proto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.proto.v1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.schema.properties.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/docs/weaviate.util.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.708159 weaviate_client-4.6.0b1/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/1234.3gp
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/hobbits.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19306 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_batch_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78632 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31180 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34333 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_multi_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25027 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_collection_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_gql_raw_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/test_tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration/weaviate-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.708159 weaviate_client-4.6.0b1/integration_embedded/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_embedded/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.708159 weaviate_client-4.6.0b1/integration_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/people_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_backup_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_grcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/integration_v3/test_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.712159 weaviate_client-4.6.0b1/mock_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/test_automatic_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/test_batching_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/test_resend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/mock_tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.712159 weaviate_client-4.6.0b1/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/profiling/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/profiling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/profiling/test_import_and_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/profiling/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/profiling/test_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/profiling/test_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/publishing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/run-mypy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-07 23:24:40.756159 weaviate_client-4.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.712159 weaviate_client-4.6.0b1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.712159 weaviate_client-4.6.0b1/test/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/batch/test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.716159 weaviate_client-4.6.0b1/test/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/classification/test_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.716159 weaviate_client-4.6.0b1/test/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/cluster/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.716159 weaviate_client-4.6.0b1/test/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/test_byteops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37924 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/collection/test_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.716159 weaviate_client-4.6.0b1/test/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/connection/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.716159 weaviate_client-4.6.0b1/test/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/contextionary/test_text2vec_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.716159 weaviate_client-4.6.0b1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.716159 weaviate_client-4.6.0b1/test/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/data/references/test_crud_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/data/test_crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.720159 weaviate_client-4.6.0b1/test/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/gql/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/gql/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/gql/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/gql/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.720159 weaviate_client-4.6.0b1/test/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.720159 weaviate_client-4.6.0b1/test/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/schema/properties/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/schema/schema_company.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/schema/tenants.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/schema/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/test_server_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/test/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.720159 weaviate_client-4.6.0b1/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.724159 weaviate_client-4.6.0b1/weaviate/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/backup/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.724159 weaviate_client-4.6.0b1/weaviate/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/batch/crud_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/batch/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.724159 weaviate_client-4.6.0b1/weaviate/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classes/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.724159 weaviate_client-4.6.0b1/weaviate/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/classification/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22119 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.724159 weaviate_client-4.6.0b1/weaviate/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/cluster/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.728159 weaviate_client-4.6.0b1/weaviate/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.728159 weaviate_client-4.6.0b1/weaviate/collections/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/aggregations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/aggregations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/aggregations/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/aggregations/near_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/aggregations/near_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/aggregations/near_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/aggregations/near_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/aggregations/over_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.732159 weaviate_client-4.6.0b1/weaviate/collections/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27772 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/batch/batch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/batch/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/batch/grpc_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/batch/grpc_batch_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/batch/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.732159 weaviate_client-4.6.0b1/weaviate/collections/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70969 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/config_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41098 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/config_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/config_vector_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40780 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/config_vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19528 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/classes/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.736159 weaviate_client-4.6.0b1/weaviate/collections/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28802 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/grpc/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/grpc/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/grpc/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.736159 weaviate_client-4.6.0b1/weaviate/collections/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.736159 weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/byteops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.736159 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_object_by_id/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_object_by_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_object_by_id/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_object_by_id/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.736159 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.736159 weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.740159 weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.740159 weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.740159 weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.740159 weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.744159 weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/collections/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.744159 weaviate_client-4.6.0b1/weaviate/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/connect/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/connect/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15187 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/connect/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/connect/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24958 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/connect/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26680 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/connect/v4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.744159 weaviate_client-4.6.0b1/weaviate/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/contextionary/crud_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.744159 weaviate_client-4.6.0b1/weaviate/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/data/crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.744159 weaviate_client-4.6.0b1/weaviate/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/data/references/crud_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.744159 weaviate_client-4.6.0b1/weaviate/data/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/data/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/data/replication/replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/error_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.748159 weaviate_client-4.6.0b1/weaviate/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42084 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/gql/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/gql/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/gql/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/gql/multi_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/gql/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.748159 weaviate_client-4.6.0b1/weaviate/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/outputs/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/outputs/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/outputs/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/outputs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/outputs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/outputs/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/outputs/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/outputs/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.748159 weaviate_client-4.6.0b1/weaviate/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.752159 weaviate_client-4.6.0b1/weaviate/proto/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/batch_delete_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/batch_delete_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/batch_delete_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/batch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/properties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/properties_pb2_grpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/regen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/search_get_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/search_get_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/search_get_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/tenants_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/tenants_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/tenants_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/weaviate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/weaviate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/proto/v1/weaviate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.752159 weaviate_client-4.6.0b1/weaviate/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/schema/crud_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.752159 weaviate_client-4.6.0b1/weaviate/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/schema/properties/crud_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11662 2024-05-07 23:24:18.000000 weaviate_client-4.6.0b1/weaviate/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:24:40.756159 weaviate_client-4.6.0b1/weaviate_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-07 23:24:40.000000 weaviate_client-4.6.0b1/weaviate_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-07 23:24:40.000000 weaviate_client-4.6.0b1/weaviate_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:24:40.000000 weaviate_client-4.6.0b1/weaviate_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:24:40.000000 weaviate_client-4.6.0b1/weaviate_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 23:24:40.000000 weaviate_client-4.6.0b1/weaviate_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 23:24:40.000000 weaviate_client-4.6.0b1/weaviate_client.egg-info/top_level.txt
```

### Comparing `weaviate_client-4.6.0b0/.flake8` & `weaviate_client-4.6.0b1/.flake8`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/.github/workflows/main.yaml` & `weaviate_client-4.6.0b1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/.pre-commit-config.yaml` & `weaviate_client-4.6.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/.pylintrc` & `weaviate_client-4.6.0b1/.pylintrc`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/CONTRIBUTING.md` & `weaviate_client-4.6.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/LICENSE` & `weaviate_client-4.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/PKG-INFO` & `weaviate_client-4.6.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.6.0b0
+Version: 4.6.0b1
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate_client-4.6.0b0/README.rst` & `weaviate_client-4.6.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose-async.yml` & `weaviate_client-4.6.0b1/ci/docker-compose-async.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose-azure.yml` & `weaviate_client-4.6.0b1/ci/docker-compose-azure.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose-cluster.yml` & `weaviate_client-4.6.0b1/ci/docker-compose-cluster.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose-generative.yml` & `weaviate_client-4.6.0b1/ci/docker-compose-generative.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose-okta-cc.yml` & `weaviate_client-4.6.0b1/ci/docker-compose-okta-cc.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose-okta-users.yml` & `weaviate_client-4.6.0b1/ci/docker-compose-okta-users.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose-proxy.yml` & `weaviate_client-4.6.0b1/ci/docker-compose-proxy.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose-rerank.yml` & `weaviate_client-4.6.0b1/ci/docker-compose-rerank.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose-wcs.yml` & `weaviate_client-4.6.0b1/ci/docker-compose-wcs.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/docker-compose.yml` & `weaviate_client-4.6.0b1/ci/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/proxy/envoy.yaml` & `weaviate_client-4.6.0b1/ci/proxy/envoy.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/ci/start_weaviate.sh` & `weaviate_client-4.6.0b1/ci/start_weaviate.sh`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/Makefile` & `weaviate_client-4.6.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/README.rst` & `weaviate_client-4.6.0b1/docs/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/changelog.rst` & `weaviate_client-4.6.0b1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/conf.py` & `weaviate_client-4.6.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/index.rst` & `weaviate_client-4.6.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/make.bat` & `weaviate_client-4.6.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.classification.rst` & `weaviate_client-4.6.0b1/docs/weaviate.classification.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.collections.aggregations.rst` & `weaviate_client-4.6.0b1/docs/weaviate.collections.aggregations.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.collections.batch.rst` & `weaviate_client-4.6.0b1/docs/weaviate.collections.batch.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.collections.classes.rst` & `weaviate_client-4.6.0b1/docs/weaviate.collections.classes.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.collections.grpc.rst` & `weaviate_client-4.6.0b1/docs/weaviate.collections.grpc.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.collections.queries.rst` & `weaviate_client-4.6.0b1/docs/weaviate.collections.queries.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.collections.rst` & `weaviate_client-4.6.0b1/docs/weaviate.collections.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.connect.rst` & `weaviate_client-4.6.0b1/docs/weaviate.connect.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.gql.rst` & `weaviate_client-4.6.0b1/docs/weaviate.gql.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.proto.v1.rst` & `weaviate_client-4.6.0b1/docs/weaviate.proto.v1.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/docs/weaviate.rst` & `weaviate_client-4.6.0b1/docs/weaviate.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/1234.3gp` & `weaviate_client-4.6.0b1/integration/1234.3gp`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/conftest.py` & `weaviate_client-4.6.0b1/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/constants.py` & `weaviate_client-4.6.0b1/integration/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/hobbits.mp4` & `weaviate_client-4.6.0b1/integration/hobbits.mp4`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_auth.py` & `weaviate_client-4.6.0b1/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_batch_v4.py` & `weaviate_client-4.6.0b1/integration/test_batch_v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -532,7 +532,16 @@
     assert errs2[0].object_.properties is not None
     assert errs2[0].object_.properties["name"] == 2
 
     # err still contains original errors
     assert len(errs) == 1
     assert errs[0].object_.properties is not None
     assert errs[0].object_.properties["name"] == 1
+
+
+def test_non_existant_collection(client_factory: ClientFactory) -> None:
+    client, _ = client_factory()
+    with client.batch.dynamic() as batch:
+        batch.add_object(properties={"name": 2}, collection="DoesNotExist")
+
+    # above should not throw - depending on the autoschema config this might create an error or
+    # not, so we do not check for errors here
```

### Comparing `weaviate_client-4.6.0b0/integration/test_client.py` & `weaviate_client-4.6.0b1/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection.py` & `weaviate_client-4.6.0b1/integration/test_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1964,38 +1964,38 @@
     uuid_banana = collection.data.insert({"text": "banana"})
     obj = collection.query.fetch_object_by_id(uuid_banana, include_vector=True)
 
     if collection._connection._weaviate_version.is_lower_than(1, 25, 0):
         with pytest.raises(WeaviateUnsupportedFeatureError):
             collection.query.hybrid(
                 query=None,
-                vector=wvc.query.HybridNear.vector(vector=obj.vector["default"]),
+                vector=wvc.query.HybridVector.near_vector(vector=obj.vector["default"]),
             ).objects
         return
 
     collection.data.insert({"text": "dog"})
     collection.data.insert({"text": "different concept"})
 
     hybrid_objs: List[Object[Any, Any]] = collection.query.hybrid(
         query=None,
-        vector=wvc.query.HybridNear.vector(vector=obj.vector["default"]),
+        vector=wvc.query.HybridVector.near_vector(vector=obj.vector["default"]),
     ).objects
 
     assert hybrid_objs[0].uuid == uuid_banana
     assert len(hybrid_objs) == 3
 
     # make a near vector search to get the distance
     near_vec = collection.query.near_vector(
         near_vector=obj.vector["default"], return_metadata=["distance"]
     ).objects
     assert near_vec[0].metadata.distance is not None
 
     hybrid_objs2 = collection.query.hybrid(
         query=None,
-        vector=wvc.query.HybridNear.vector(
+        vector=wvc.query.HybridVector.near_vector(
             vector=obj.vector["default"], distance=near_vec[0].metadata.distance + 0.001
         ),
         return_metadata=MetadataQuery.full(),
     ).objects
 
     assert hybrid_objs2[0].uuid == uuid_banana
     assert len(hybrid_objs2) == 1
@@ -2030,35 +2030,37 @@
 
     obj = collection.query.fetch_object_by_id(uuid_banana, include_vector=True)
 
     if collection._connection._weaviate_version.is_lower_than(1, 25, 0):
         with pytest.raises(WeaviateUnsupportedFeatureError):
             hybrid_objs: List[Object[Any, Any]] = collection.query.hybrid(
                 query=None,
-                vector=wvc.query.HybridNear.vector(vector=obj.vector["text"], target_vector="text"),
+                vector=wvc.query.HybridVector.near_vector(
+                    vector=obj.vector["text"], target_vector="text"
+                ),
             ).objects
         return
 
     hybrid_objs = collection.query.hybrid(
         query=None,
-        vector=wvc.query.HybridNear.vector(vector=obj.vector["text"], target_vector="text"),
+        vector=wvc.query.HybridVector.near_vector(vector=obj.vector["text"], target_vector="text"),
     ).objects
 
     assert hybrid_objs[0].uuid == uuid_banana
     assert len(hybrid_objs) == 3
 
     # make a near vector search to get the distance
     near_vec = collection.query.near_vector(
         near_vector=obj.vector["text"], return_metadata=["distance"], target_vector="text"
     ).objects
     assert near_vec[0].metadata.distance is not None
 
     hybrid_objs2 = collection.query.hybrid(
         query=None,
-        vector=wvc.query.HybridNear.vector(
+        vector=wvc.query.HybridVector.near_vector(
             vector=obj.vector["text"],
             distance=near_vec[0].metadata.distance + 0.001,
             target_vector="text",
         ),
         return_metadata=MetadataQuery.full(),
     ).objects
 
@@ -2076,34 +2078,34 @@
         ),
     )
 
     if collection._connection._weaviate_version.is_lower_than(1, 25, 0):
         with pytest.raises(WeaviateUnsupportedFeatureError):
             collection.query.hybrid(
                 query=None,
-                vector=wvc.query.HybridNear.text(text="banana pudding"),
+                vector=wvc.query.HybridVector.near_text(query="banana pudding"),
             ).objects
         return
 
     uuid_banana_pudding = collection.data.insert({"text": "banana pudding"})
     collection.data.insert({"text": "banana smoothie"})
     collection.data.insert({"text": "different concept"})
 
     hybrid_objs: List[Object[Any, Any]] = collection.query.hybrid(
         query=None,
-        vector=wvc.query.HybridNear.text(text="banana pudding"),
+        vector=wvc.query.HybridVector.near_text(query="banana pudding"),
     ).objects
 
     assert hybrid_objs[0].uuid == uuid_banana_pudding
     assert len(hybrid_objs) == 3
 
     hybrid_objs2 = collection.query.hybrid(
         query=None,
-        vector=wvc.query.HybridNear.text(
-            text="banana",
+        vector=wvc.query.HybridVector.near_text(
+            query="banana",
             move_to=wvc.query.Move(concepts="pudding", force=0.1),
             move_away=wvc.query.Move(concepts="smoothie", force=0.1),
         ),
         return_metadata=MetadataQuery.full(),
     ).objects
 
     assert hybrid_objs2[0].uuid == uuid_banana_pudding
@@ -2135,30 +2137,32 @@
     collection.data.insert({"text": "banana smoothie"})
     collection.data.insert({"text": "different concept"})
 
     if collection._connection._weaviate_version.is_lower_than(1, 25, 0):
         with pytest.raises(WeaviateUnsupportedFeatureError):
             hybrid_objs: List[Object[Any, Any]] = collection.query.hybrid(
                 query=None,
-                vector=wvc.query.HybridNear.text(text="banana pudding", target_vector="text"),
+                vector=wvc.query.HybridVector.near_text(
+                    query="banana pudding", target_vector="text"
+                ),
             ).objects
         return
 
     hybrid_objs = collection.query.hybrid(
         query=None,
-        vector=wvc.query.HybridNear.text(text="banana pudding", target_vector="text"),
+        vector=wvc.query.HybridVector.near_text(query="banana pudding", target_vector="text"),
     ).objects
 
     assert hybrid_objs[0].uuid == uuid_banana_pudding
     assert len(hybrid_objs) == 3
 
     hybrid_objs2 = collection.query.hybrid(
         query=None,
-        vector=wvc.query.HybridNear.text(
-            text="banana",
+        vector=wvc.query.HybridVector.near_text(
+            query="banana",
             move_to=wvc.query.Move(concepts="pudding", force=0.1),
             move_away=wvc.query.Move(concepts="smoothie", force=0.1),
             target_vector="text",
         ),
         return_metadata=MetadataQuery.full(),
     ).objects
```

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_aggregate.py` & `weaviate_client-4.6.0b1/integration/test_collection_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_batch.py` & `weaviate_client-4.6.0b1/integration/test_collection_batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 from dataclasses import dataclass
 from typing import Generator, Optional, Union, Any, Protocol
 
 import pytest
 
-from integration.conftest import CollectionFactory
+from integration.conftest import CollectionFactory, CollectionFactoryGet
 from weaviate.collections import Collection
 from weaviate.collections.classes.config import (
     Configure,
     DataType,
     Property,
     ReferenceProperty,
 )
@@ -221,7 +221,16 @@
 
     assert len(col.batch.failed_objects) == 0
     assert len(col.batch.failed_references) == 0
 
     obj = col.query.fetch_object_by_id(uuids[-1], return_references=QueryReference(link_on="test"))
     assert "test" in obj.references
     assert obj.references["test"].objects[0].uuid == uuids[-1]
+
+
+def test_non_existant_collection(collection_factory_get: CollectionFactoryGet) -> None:
+    collection = collection_factory_get("DoesNotExist")
+    with collection.batch.dynamic() as batch:
+        batch.add_object(properties={"name": 2})
+
+    # above should not throw - depending on the autoschema config this might create an error or
+    # not, so we do not check for errors here
```

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_batch_delete.py` & `weaviate_client-4.6.0b1/integration/test_collection_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_config.py` & `weaviate_client-4.6.0b1/integration/test_collection_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -754,22 +754,45 @@
     if collection_dummy._connection._weaviate_version.is_lower_than(1, 25, 0):
         pytest.skip("Dynamic index is not supported in Weaviate versions lower than 1.25.0")
 
     collection = collection_factory(
         vector_index_config=Configure.VectorIndex.dynamic(
             distance_metric=VectorDistances.COSINE,
             threshold=1000,
-            hnsw=Configure.VectorIndex.hnsw(cleanup_interval_seconds=123, flat_search_cutoff=1234),
+            hnsw=Configure.VectorIndex.hnsw(
+                cleanup_interval_seconds=123, flat_search_cutoff=1234, vector_cache_max_objects=789
+            ),
             flat=Configure.VectorIndex.flat(vector_cache_max_objects=7643),
         ),
         ports=(8090, 50061),
     )
 
     config = collection.config.get()
     assert isinstance(config.vector_index_config, _VectorIndexConfigDynamic)
     assert config.vector_index_config.distance_metric == VectorDistances.COSINE
     assert config.vector_index_config.threshold == 1000
     assert isinstance(config.vector_index_config.hnsw, _VectorIndexConfigHNSW)
     assert config.vector_index_config.hnsw.cleanup_interval_seconds == 123
     assert config.vector_index_config.hnsw.flat_search_cutoff == 1234
+    assert config.vector_index_config.hnsw.vector_cache_max_objects == 789
     assert isinstance(config.vector_index_config.flat, _VectorIndexConfigFlat)
     assert config.vector_index_config.flat.vector_cache_max_objects == 7643
+
+    collection.config.update(
+        vectorizer_config=Reconfigure.VectorIndex.dynamic(
+            threshold=2000,
+            hnsw=Reconfigure.VectorIndex.hnsw(
+                flat_search_cutoff=4567, vector_cache_max_objects=678
+            ),
+            flat=Reconfigure.VectorIndex.flat(vector_cache_max_objects=9876),
+        ),
+    )
+    config = collection.config.get()
+    assert isinstance(config.vector_index_config, _VectorIndexConfigDynamic)
+    assert config.vector_index_config.distance_metric == VectorDistances.COSINE
+    assert config.vector_index_config.threshold == 2000
+    assert isinstance(config.vector_index_config.hnsw, _VectorIndexConfigHNSW)
+    assert config.vector_index_config.hnsw.cleanup_interval_seconds == 123
+    assert config.vector_index_config.hnsw.flat_search_cutoff == 4567
+    assert config.vector_index_config.hnsw.vector_cache_max_objects == 678
+    assert isinstance(config.vector_index_config.flat, _VectorIndexConfigFlat)
+    assert config.vector_index_config.flat.vector_cache_max_objects == 9876
```

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_filter.py` & `weaviate_client-4.6.0b1/integration/test_collection_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_geo.py` & `weaviate_client-4.6.0b1/integration/test_collection_geo.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_get.py` & `weaviate_client-4.6.0b1/integration/test_collection_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_model.py` & `weaviate_client-4.6.0b1/integration/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_multi_node.py` & `weaviate_client-4.6.0b1/integration/test_collection_multi_node.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_nested.py` & `weaviate_client-4.6.0b1/integration/test_collection_nested.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_openai.py` & `weaviate_client-4.6.0b1/integration/test_collection_openai.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_references.py` & `weaviate_client-4.6.0b1/integration/test_collection_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_collection_rerank.py` & `weaviate_client-4.6.0b1/integration/test_collection_rerank.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_gql_raw_v4.py` & `weaviate_client-4.6.0b1/integration/test_gql_raw_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_iterator.py` & `weaviate_client-4.6.0b1/integration/test_iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_named_vectors.py` & `weaviate_client-4.6.0b1/integration/test_named_vectors.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/test_tenants.py` & `weaviate_client-4.6.0b1/integration/test_tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration/weaviate-logo.png` & `weaviate_client-4.6.0b1/integration/weaviate-logo.png`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_embedded/test_client.py` & `weaviate_client-4.6.0b1/integration_embedded/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/people_schema.json` & `weaviate_client-4.6.0b1/integration_v3/people_schema.json`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_authentication.py` & `weaviate_client-4.6.0b1/integration_v3/test_authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_backup.py` & `weaviate_client-4.6.0b1/integration_v3/test_backup.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_backup_v4.py` & `weaviate_client-4.6.0b1/integration_v3/test_backup_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_batch.py` & `weaviate_client-4.6.0b1/integration_v3/test_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_classification.py` & `weaviate_client-4.6.0b1/integration_v3/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_cluster.py` & `weaviate_client-4.6.0b1/integration_v3/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_crud.py` & `weaviate_client-4.6.0b1/integration_v3/test_crud.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_graphql.py` & `weaviate_client-4.6.0b1/integration_v3/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_grcp.py` & `weaviate_client-4.6.0b1/integration_v3/test_grcp.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_schema.py` & `weaviate_client-4.6.0b1/integration_v3/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_stress.py` & `weaviate_client-4.6.0b1/integration_v3/test_stress.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/integration_v3/test_timeout.py` & `weaviate_client-4.6.0b1/integration_v3/test_timeout.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/conftest.py` & `weaviate_client-4.6.0b1/mock_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/test_auth.py` & `weaviate_client-4.6.0b1/mock_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/test_automatic_retries.py` & `weaviate_client-4.6.0b1/mock_tests/test_automatic_retries.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/test_batching_manual.py` & `weaviate_client-4.6.0b1/mock_tests/test_batching_manual.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/test_collection.py` & `weaviate_client-4.6.0b1/mock_tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/test_connection.py` & `weaviate_client-4.6.0b1/mock_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/test_exception.py` & `weaviate_client-4.6.0b1/mock_tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/test_graphql.py` & `weaviate_client-4.6.0b1/mock_tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/test_resend.py` & `weaviate_client-4.6.0b1/mock_tests/test_resend.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/mock_tests/test_schema.py` & `weaviate_client-4.6.0b1/mock_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/profiling/conftest.py` & `weaviate_client-4.6.0b1/profiling/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/profiling/constants.py` & `weaviate_client-4.6.0b1/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/profiling/test_import_and_query.py` & `weaviate_client-4.6.0b1/profiling/test_import_and_query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/profiling/test_profiling.py` & `weaviate_client-4.6.0b1/profiling/test_profiling.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/profiling/test_refs.py` & `weaviate_client-4.6.0b1/profiling/test_refs.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/profiling/test_sphere.py` & `weaviate_client-4.6.0b1/profiling/test_sphere.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/publishing.md` & `weaviate_client-4.6.0b1/publishing.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/pyproject.toml` & `weaviate_client-4.6.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/requirements-devel.txt` & `weaviate_client-4.6.0b1/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/setup.cfg` & `weaviate_client-4.6.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/README.md` & `weaviate_client-4.6.0b1/test/README.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/batch/test_requests.py` & `weaviate_client-4.6.0b1/test/batch/test_requests.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/classification/test_classification.py` & `weaviate_client-4.6.0b1/test/classification/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/cluster/test_cluster.py` & `weaviate_client-4.6.0b1/test/cluster/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/collection/test_aggregates.py` & `weaviate_client-4.6.0b1/test/collection/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/collection/test_byteops.py` & `weaviate_client-4.6.0b1/test/collection/test_byteops.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/collection/test_classes.py` & `weaviate_client-4.6.0b1/test/collection/test_classes.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/collection/test_client.py` & `weaviate_client-4.6.0b1/test/collection/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/collection/test_collection_model.py` & `weaviate_client-4.6.0b1/test/collection/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/collection/test_config.py` & `weaviate_client-4.6.0b1/test/collection/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,28 @@
                 "vectorizeClassName": False,
                 "model": "thenlper/gte-large",
                 "baseURL": "https://text.octoai.com",
             }
         },
     ),
     (
+        Configure.Vectorizer.text2vec_ollama(
+            vectorize_collection_name=False,
+            model="cool-model",
+            api_endpoint="https://123.0.0.4",
+        ),
+        {
+            "text2vec-ollama": {
+                "vectorizeClassName": False,
+                "model": "cool-model",
+                "apiEndpoint": "https://123.0.0.4",
+            }
+        },
+    ),
+    (
         Configure.Vectorizer.text2vec_openai(),
         {
             "text2vec-openai": {
                 "vectorizeClassName": True,
             }
         },
     ),
@@ -605,14 +619,26 @@
                 "maxTokens": 123,
                 "temperature": 0.5,
                 "baseURL": "https://text.octoai.run",
             }
         },
     ),
     (
+        Configure.Generative.ollama(
+            model="cool-model",
+            api_endpoint="https://123.456.789.0",
+        ),
+        {
+            "generative-ollama": {
+                "model": "cool-model",
+                "apiEndpoint": "https://123.456.789.0",
+            }
+        },
+    ),
+    (
         Configure.Generative.openai(
             model="gpt-4",
             frequency_penalty=0.5,
             max_tokens=100,
             presence_penalty=0.5,
             temperature=0.5,
             top_p=0.5,
@@ -685,14 +711,15 @@
     ),
     (
         Configure.Generative.aws(model="cohere.command-light-text-v14", region="us-east-1"),
         {
             "generative-aws": {
                 "model": "cohere.command-light-text-v14",
                 "region": "us-east-1",
+                "service": "bedrock",
             }
         },
     ),
     (
         Configure.Generative.azure_openai(resource_name="name", deployment_id="id"),
         {
             "generative-openai": {
@@ -1080,14 +1107,37 @@
                     }
                 },
                 "vectorIndexType": "hnsw",
             }
         },
     ),
     (
+        [
+            Configure.NamedVectors.text2vec_ollama(
+                name="test",
+                source_properties=["prop"],
+                api_endpoint="https://123.0.0.4",
+                model="cool-model",
+            )
+        ],
+        {
+            "test": {
+                "vectorizer": {
+                    "text2vec-ollama": {
+                        "properties": ["prop"],
+                        "vectorizeClassName": True,
+                        "apiEndpoint": "https://123.0.0.4",
+                        "model": "cool-model",
+                    }
+                },
+                "vectorIndexType": "hnsw",
+            }
+        },
+    ),
+    (
         [
             Configure.NamedVectors.text2vec_openai(
                 name="test", source_properties=["prop"], base_url="https://api.openai.com/"
             )
         ],
         {
             "test": {
```

### Comparing `weaviate_client-4.6.0b0/test/collection/test_filter.py` & `weaviate_client-4.6.0b1/test/collection/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/collection/test_queries.py` & `weaviate_client-4.6.0b1/test/collection/test_queries.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/connection/test_connection.py` & `weaviate_client-4.6.0b1/test/connection/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/contextionary/test_text2vec_contextionary.py` & `weaviate_client-4.6.0b1/test/contextionary/test_text2vec_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/data/references/test_crud_references.py` & `weaviate_client-4.6.0b1/test/data/references/test_crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/data/test_crud_data.py` & `weaviate_client-4.6.0b1/test/data/test_crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/gql/test_aggregate.py` & `weaviate_client-4.6.0b1/test/gql/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/gql/test_filter.py` & `weaviate_client-4.6.0b1/test/gql/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/gql/test_get.py` & `weaviate_client-4.6.0b1/test/gql/test_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/gql/test_query.py` & `weaviate_client-4.6.0b1/test/gql/test_query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/schema/properties/test_properties.py` & `weaviate_client-4.6.0b1/test/schema/properties/test_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/schema/schema_company.json` & `weaviate_client-4.6.0b1/test/schema/schema_company.json`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/schema/test_schema.py` & `weaviate_client-4.6.0b1/test/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/test_auth.py` & `weaviate_client-4.6.0b1/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/test_client.py` & `weaviate_client-4.6.0b1/test/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/test_embedded.py` & `weaviate_client-4.6.0b1/test/test_embedded.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/test_exceptions.py` & `weaviate_client-4.6.0b1/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/test_server_version.py` & `weaviate_client-4.6.0b1/test/test_server_version.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/test_util.py` & `weaviate_client-4.6.0b1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/test/util.py` & `weaviate_client-4.6.0b1/test/util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/__init__.py` & `weaviate_client-4.6.0b1/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/auth.py` & `weaviate_client-4.6.0b1/weaviate/auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/backup/backup.py` & `weaviate_client-4.6.0b1/weaviate/backup/backup.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/batch/crud_batch.py` & `weaviate_client-4.6.0b1/weaviate/batch/crud_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/batch/requests.py` & `weaviate_client-4.6.0b1/weaviate/batch/requests.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/classes/config.py` & `weaviate_client-4.6.0b1/weaviate/classes/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/classes/query.py` & `weaviate_client-4.6.0b1/weaviate/classes/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from weaviate.collections.classes.filters import Filter
 from weaviate.collections.classes.aggregate import Metrics
 from weaviate.collections.classes.grpc import (
     HybridFusion,
     GroupBy,
-    HybridNear,
+    HybridVector,
     MetadataQuery,
     Move,
     NearMediaType,
     QueryNested,
     QueryReference,
     Rerank,
     Sort,
@@ -16,15 +16,15 @@
 
 
 __all__ = [
     "Filter",
     "GeoCoordinate",
     "GroupBy",
     "HybridFusion",
-    "HybridNear",
+    "HybridVector",
     "MetadataQuery",
     "Metrics",
     "Move",
     "NearMediaType",
     "QueryNested",
     "QueryReference",
     "Rerank",
```

### Comparing `weaviate_client-4.6.0b0/weaviate/classification/classification.py` & `weaviate_client-4.6.0b1/weaviate/classification/classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/classification/config_builder.py` & `weaviate_client-4.6.0b1/weaviate/classification/config_builder.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/client.py` & `weaviate_client-4.6.0b1/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/cluster/cluster.py` & `weaviate_client-4.6.0b1/weaviate/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/cluster/types.py` & `weaviate_client-4.6.0b1/weaviate/cluster/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/aggregations/base.py` & `weaviate_client-4.6.0b1/weaviate/collections/aggregations/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/aggregations/hybrid.py` & `weaviate_client-4.6.0b1/weaviate/collections/aggregations/hybrid.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_image.py` & `weaviate_client-4.6.0b1/weaviate/collections/aggregations/near_image.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_object.py` & `weaviate_client-4.6.0b1/weaviate/collections/aggregations/near_object.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_text.py` & `weaviate_client-4.6.0b1/weaviate/collections/aggregations/near_text.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/aggregations/near_vector.py` & `weaviate_client-4.6.0b1/weaviate/collections/aggregations/near_vector.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/aggregations/over_all.py` & `weaviate_client-4.6.0b1/weaviate/collections/aggregations/over_all.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/backups.py` & `weaviate_client-4.6.0b1/weaviate/collections/backups.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/base.py` & `weaviate_client-4.6.0b1/weaviate/collections/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/batch/base.py` & `weaviate_client-4.6.0b1/weaviate/collections/batch/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/batch/batch_wrapper.py` & `weaviate_client-4.6.0b1/weaviate/collections/batch/batch_wrapper.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/batch/client.py` & `weaviate_client-4.6.0b1/weaviate/collections/batch/client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/batch/collection.py` & `weaviate_client-4.6.0b1/weaviate/collections/batch/collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     _RateLimitedBatching,
 )
 from weaviate.collections.batch.batch_wrapper import _BatchWrapper, _ContextManagerWrapper
 from weaviate.collections.classes.config import ConsistencyLevel, Vectorizers
 from weaviate.collections.classes.internal import ReferenceInputs, ReferenceInput
 from weaviate.collections.classes.types import Properties
 from weaviate.connect import ConnectionV4
+from weaviate.exceptions import UnexpectedStatusCodeError
 from weaviate.types import UUID, VECTORS
 
 if TYPE_CHECKING:
     from weaviate.collections.config import _ConfigCollection
 
 
 class _BatchCollection(Generic[Properties], _BatchBase):
@@ -123,24 +124,30 @@
         self.__name = name
         self.__tenant = tenant
         self.__config = config
         self._vectorizer_batching: Optional[bool] = None
 
     def __create_batch_and_reset(self) -> _ContextManagerWrapper[_BatchCollection[Properties]]:
         if self._vectorizer_batching is None:
-            config = self.__config.get(simple=True)
-            if config.vector_config is not None:
-                vectorizer_batching = False
-                for vec_config in config.vector_config.values():
-                    if vec_config.vectorizer.vectorizer is not Vectorizers.NONE:
-                        vectorizer_batching = True
-                        break
-                self._vectorizer_batching = vectorizer_batching
-            else:
-                self._vectorizer_batching = config.vectorizer is not Vectorizers.NONE
+            try:
+                config = self.__config.get(simple=True)
+                if config.vector_config is not None:
+                    vectorizer_batching = False
+                    for vec_config in config.vector_config.values():
+                        if vec_config.vectorizer.vectorizer is not Vectorizers.NONE:
+                            vectorizer_batching = True
+                            break
+                    self._vectorizer_batching = vectorizer_batching
+                else:
+                    self._vectorizer_batching = config.vectorizer is not Vectorizers.NONE
+            except UnexpectedStatusCodeError as e:
+                # collection does not have to exist if autoschema is enabled. Individual objects will be validated and might fail
+                if e.status_code != 404:
+                    raise e
+                self._vectorizer_batching = False
 
         self._batch_data = _BatchDataWrapper()  # clear old data
         return _ContextManagerWrapper(
             _BatchCollection[Properties](
                 connection=self._connection,
                 consistency_level=self._consistency_level,
                 results=self._batch_data,
```

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/batch/grpc_batch_delete.py` & `weaviate_client-4.6.0b1/weaviate/collections/batch/grpc_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/batch/grpc_batch_objects.py` & `weaviate_client-4.6.0b1/weaviate/collections/batch/grpc_batch_objects.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/batch/rest.py` & `weaviate_client-4.6.0b1/weaviate/collections/batch/rest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/aggregate.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/batch.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/cluster.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/config.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     _ConfigUpdateModel,
     _QuantizerConfigUpdate,
 )
 
 from weaviate.collections.classes.config_vector_index import (
     _QuantizerConfigCreate,
     _VectorIndexConfigCreate,
+    _VectorIndexConfigDynamicUpdate,
     _VectorIndexConfigHNSWCreate,
     _VectorIndexConfigFlatCreate,
     _VectorIndexConfigHNSWUpdate,
     _VectorIndexConfigFlatUpdate,
     _VectorIndexConfigDynamicCreate,
     _VectorIndexConfigSkipCreate,
     _VectorIndexConfigUpdate,
@@ -57,14 +58,19 @@
 from weaviate.warnings import _Warnings
 
 # BC for direct imports
 Vectorizers: TypeAlias = VectorizersAlias
 VectorIndexType: TypeAlias = VectorIndexTypeAlias
 VectorDistances: TypeAlias = VectorDistancesAlias
 
+AWSService: TypeAlias = Literal[
+    "bedrock",
+    "sagemaker",
+]
+
 
 class ConsistencyLevel(str, Enum):
     """The consistency levels when writing to Weaviate with replication enabled.
 
     Attributes:
         ALL: Wait for confirmation of write success from all, `N`, replicas.
         ONE: Wait for confirmation of write success from only one replica.
@@ -162,14 +168,15 @@
     """
 
     AWS = "generative-aws"
     ANYSCALE = "generative-anyscale"
     COHERE = "generative-cohere"
     MISTRAL = "generative-mistral"
     OCTOAI = "generative-octoai"
+    OLLAMA = "generative-ollama"
     OPENAI = "generative-openai"
     PALM = "generative-palm"
 
 
 class Rerankers(str, Enum):
     """The available reranker modules in Weaviate.
 
@@ -386,14 +393,22 @@
         default=GenerativeSearches.MISTRAL, frozen=True, exclude=True
     )
     temperature: Optional[float]
     model: Optional[str]
     maxTokens: Optional[int]
 
 
+class _GenerativeOllama(_GenerativeConfigCreate):
+    generative: GenerativeSearches = Field(
+        default=GenerativeSearches.OLLAMA, frozen=True, exclude=True
+    )
+    model: Optional[str]
+    apiEndpoint: Optional[str]
+
+
 class _GenerativeOpenAIConfigBase(_GenerativeConfigCreate):
     generative: GenerativeSearches = Field(
         default=GenerativeSearches.OPENAI, frozen=True, exclude=True
     )
     baseURL: Optional[AnyHttpUrl]
     frequencyPenaltyProperty: Optional[float]
     presencePenaltyProperty: Optional[float]
@@ -449,16 +464,18 @@
     topP: Optional[float]
 
 
 class _GenerativeAWSConfig(_GenerativeConfigCreate):
     generative: GenerativeSearches = Field(
         default=GenerativeSearches.AWS, frozen=True, exclude=True
     )
-    model: str
     region: str
+    service: str
+    model: Optional[str]
+    endpoint: Optional[str]
 
 
 class _RerankerConfigCreate(_ConfigCreateModel):
     reranker: Rerankers
 
 
 RerankerCohereModel = Literal["rerank-english-v2.0", "rerank-multilingual-v2.0"]
@@ -512,14 +529,22 @@
         temperature: Optional[float] = None,
     ) -> _GenerativeConfigCreate:
         return _GenerativeOctoai(
             baseURL=base_url, maxTokens=max_tokens, model=model, temperature=temperature
         )
 
     @staticmethod
+    def ollama(
+        *,
+        api_endpoint: Optional[str] = None,
+        model: Optional[str] = None,
+    ) -> _GenerativeConfigCreate:
+        return _GenerativeOllama(model=model, apiEndpoint=api_endpoint)
+
+    @staticmethod
     def openai(
         model: Optional[str] = None,
         frequency_penalty: Optional[float] = None,
         max_tokens: Optional[int] = None,
         presence_penalty: Optional[float] = None,
         temperature: Optional[float] = None,
         top_p: Optional[float] = None,
@@ -681,31 +706,39 @@
             temperature=temperature,
             topK=top_k,
             topP=top_p,
         )
 
     @staticmethod
     def aws(
-        model: str,
-        region: str,
+        model: Optional[str] = None,
+        region: str = "",  # cant have a non-default value after a default value, but we cant change the order for BC
+        endpoint: Optional[str] = None,
+        service: Union[AWSService, str] = "bedrock",
     ) -> _GenerativeConfigCreate:
         """Create a `_GenerativeAWSConfig` object for use when performing AI generation using the `generative-aws` module.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/reader-generator-modules/generative-aws)
         for detailed usage.
 
         Arguments:
             `model`
-                The model to use, REQUIRED.
+                The model to use, REQUIRED for service "bedrock".
             `region`
                 The AWS region to run the model from, REQUIRED.
+            `endpoint`
+                The model to use, REQUIRED for service "sagemaker".
+            `service`
+                The AWS service to use, options are "bedrock" and "sagemaker".
         """
         return _GenerativeAWSConfig(
             model=model,
             region=region,
+            service=service,
+            endpoint=endpoint,
         )
 
 
 class _Reranker:
     """Use this factory class to create the correct object for the `reranker_config` argument in the `collections.create()` method.
 
     Each staticmethod provides options specific to the named reranker in the function's name. Under-the-hood data validation steps
@@ -1580,15 +1613,14 @@
     def none() -> _VectorIndexConfigSkipCreate:
         """Create a `_VectorIndexConfigSkipCreate` object to be used when configuring Weaviate to not index your vectors.
 
         Use this method when defining the `vector_index_config` argument in `collections.create()`.
         """
         return _VectorIndexConfigSkipCreate(
             distance=None,
-            vectorCacheMaxObjects=None,
             quantizer=None,
         )
 
     @staticmethod
     def hnsw(
         cleanup_interval_seconds: Optional[int] = None,
         distance_metric: Optional[VectorDistances] = None,
@@ -1644,30 +1676,28 @@
 
     @staticmethod
     def dynamic(
         distance_metric: Optional[VectorDistances] = None,
         threshold: Optional[int] = None,
         hnsw: Optional[_VectorIndexConfigHNSWCreate] = None,
         flat: Optional[_VectorIndexConfigFlatCreate] = None,
-        vector_cache_max_objects: Optional[int] = None,
         quantizer: Optional[_BQConfigCreate] = None,
     ) -> _VectorIndexConfigDynamicCreate:
         """Create a `_VectorIndexConfigDynamicCreate` object to be used when defining the DYNAMIC vector index configuration of Weaviate.
 
         Use this method when defining the `vector_index_config` argument in `collections.create()`.
 
         Arguments:
             See [the docs](https://weaviate.io/developers/weaviate/configuration/indexes#how-to-configure-hnsw) for a more detailed view!
         """  # noqa: D417 (missing argument descriptions in the docstring)
         return _VectorIndexConfigDynamicCreate(
             distance=distance_metric,
             threshold=threshold,
             hnsw=hnsw,
             flat=flat,
-            vectorCacheMaxObjects=vector_cache_max_objects,
             quantizer=quantizer,
         )
 
 
 class Configure:
     """Use this factory class to generate the correct object for use when using the `collections.create()` method. E.g., `.multi_tenancy()` will return a `MultiTenancyConfigCreate` object to be used in the `multi_tenancy_config` argument.
 
@@ -1837,15 +1867,15 @@
         ef: Optional[int] = None,
         flat_search_cutoff: Optional[int] = None,
         vector_cache_max_objects: Optional[int] = None,
         quantizer: Optional[Union[_PQConfigUpdate, _BQConfigUpdate]] = None,
     ) -> _VectorIndexConfigHNSWUpdate:
         """Create an `_VectorIndexConfigHNSWUpdate` object to update the configuration of the HNSW vector index.
 
-        Use this method when defining the `vector_index_config` argument in `collection.update()`.
+        Use this method when defining the `vectorizer_config` argument in `collection.update()`.
 
         Arguments:
             See [the docs](https://weaviate.io/developers/weaviate/configuration/indexes#configure-the-inverted-index) for a more detailed view!
         """  # noqa: D417 (missing argument descriptions in the docstring)
         return _VectorIndexConfigHNSWUpdate(
             dynamicEfMin=dynamic_ef_min,
             dynamicEfMax=dynamic_ef_max,
@@ -1859,24 +1889,46 @@
     @staticmethod
     def flat(
         vector_cache_max_objects: Optional[int] = None,
         quantizer: Optional[_BQConfigUpdate] = None,
     ) -> _VectorIndexConfigFlatUpdate:
         """Create an `_VectorIndexConfigFlatUpdate` object to update the configuration of the FLAT vector index.
 
-        Use this method when defining the `vector_index_config` argument in `collection.update()`.
+        Use this method when defining the `vectorizer_config` argument in `collection.update()`.
 
         Arguments:
             See [the docs](https://weaviate.io/developers/weaviate/configuration/indexes#configure-the-inverted-index) for a more detailed view!
         """  # noqa: D417 (missing argument descriptions in the docstring)
         return _VectorIndexConfigFlatUpdate(
             vectorCacheMaxObjects=vector_cache_max_objects,
             quantizer=quantizer,
         )
 
+    @staticmethod
+    def dynamic(
+        *,
+        threshold: Optional[int] = None,
+        hnsw: Optional[_VectorIndexConfigHNSWUpdate] = None,
+        flat: Optional[_VectorIndexConfigFlatUpdate] = None,
+        quantizer: Optional[_BQConfigUpdate] = None,
+    ) -> _VectorIndexConfigDynamicUpdate:
+        """Create an `_VectorIndexConfigDynamicUpdate` object to update the configuration of the Dynamic vector index.
+
+        Use this method when defining the `vectorizer_config` argument in `collection.update()`.
+
+        Arguments:
+            See [the docs](https://weaviate.io/developers/weaviate/configuration/indexes#configure-the-inverted-index) for a more detailed view!
+        """  # noqa: D417 (missing argument descriptions in the docstring)
+        return _VectorIndexConfigDynamicUpdate(
+            threshold=threshold,
+            hnsw=hnsw,
+            flat=flat,
+            quantizer=quantizer,
+        )
+
 
 class Reconfigure:
     """Use this factory class to generate the correct `xxxConfig` object for use when using the `collection.update()` method.
 
     Each staticmethod provides options specific to the named configuration type in the function's name. Under-the-hood data validation steps
     will ensure that any mis-specifications are caught before the request is sent to Weaviate. Only those configurations that are mutable are
     available in this class. If you wish to update the configuration of an immutable aspect of your collection then you will have to delete
```

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/config_base.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/config_base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/config_methods.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/config_methods.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/config_named_vectors.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/config_named_vectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     _Text2VecAzureOpenAIConfigCreate,
     _Text2VecCohereConfigCreate,
     _Text2VecContextionaryConfigCreate,
     _Text2VecGPT4AllConfigCreate,
     _Text2VecHuggingFaceConfigCreate,
     _Text2VecJinaConfigCreate,
     _Text2VecOctoConfig,
+    _Text2VecOllamaConfig,
     _Text2VecOpenAIConfigCreate,
     _Text2VecPalmConfigCreate,
     _Text2VecTransformersConfigCreate,
     _Text2VecVoyageConfigCreate,
     _VectorizerConfigCreate,
     AWSModel,
     AWSService,
@@ -192,18 +193,18 @@
     @staticmethod
     def text2vec_octoai(
         name: str,
         *,
         source_properties: Optional[List[str]] = None,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
-        model: Optional[Union[OpenAIModel, str]] = None,
+        model: Optional[str] = None,
         base_url: Optional[str] = None,
     ) -> _NamedVectorConfigCreate:
-        """Create a named vector using the `text2vec_octoai` model.
+        """Create a named vector using the `text2vec-octoai` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-octoai)
         for detailed usage.
 
         Arguments:
             `name`
                 The name of the named vector.
@@ -229,14 +230,57 @@
                 model=model,
                 vectorizeClassName=vectorize_collection_name,
             ),
             vector_index_config=vector_index_config,
         )
 
     @staticmethod
+    def text2vec_ollama(
+        name: str,
+        *,
+        source_properties: Optional[List[str]] = None,
+        vector_index_config: Optional[_VectorIndexConfigCreate] = None,
+        vectorize_collection_name: bool = True,
+        model: Optional[str] = None,
+        api_endpoint: Optional[str] = None,
+    ) -> _NamedVectorConfigCreate:
+        """Create a named vector using the `text2vec-ollama` model.
+
+        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-ollama)
+        for detailed usage.
+
+        Arguments:
+            `name`
+                The name of the named vector.
+            `source_properties`
+                Which properties should be included when vectorizing. By default all text properties are included.
+            `vector_index_config`
+                The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+            `model`
+                The model to use. Defaults to `None`, which uses the server-defined default.
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+            `api_endpoint`
+                The base URL to use where API requests should go. Defaults to `None`, which uses the server-defined default.
+
+        """
+        return _NamedVectorConfigCreate(
+            name=name,
+            source_properties=source_properties,
+            vectorizer=_Text2VecOllamaConfig(
+                apiEndpoint=api_endpoint,
+                model=model,
+                vectorizeClassName=vectorize_collection_name,
+            ),
+            vector_index_config=vector_index_config,
+        )
+
+    @staticmethod
     def text2vec_openai(
         name: str,
         *,
         source_properties: Optional[List[str]] = None,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
         model: Optional[Union[OpenAIModel, str]] = None,
@@ -678,14 +722,15 @@
         project_id: str,
         *,
         source_properties: Optional[List[str]] = None,
         vector_index_config: Optional[_VectorIndexConfigCreate] = None,
         vectorize_collection_name: bool = True,
         api_endpoint: Optional[str] = None,
         model_id: Optional[str] = None,
+        title_property: Optional[str] = None,
     ) -> _NamedVectorConfigCreate:
         """Create a named vector using the `text2vec_palm` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-palm)
         for detailed usage.
 
         Arguments:
@@ -701,26 +746,29 @@
                 The configuration for Weaviate's vector index. Use wvc.config.Configure.VectorIndex to create a vector index configuration. None by default
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
             `api_endpoint`
                 The API endpoint to use without a leading scheme such as `http://`. Defaults to `None`, which uses the server-defined default
             `model_id`
                 The model ID to use. Defaults to `None`, which uses the server-defined default.
+            `title_property`
+                The Weaviate property name for the `gecko-002` or `gecko-003` model to use as the title.
 
         Raises:
             `pydantic.ValidationError` if `api_endpoint` is not a valid URL.
         """
         return _NamedVectorConfigCreate(
             name=name,
             source_properties=source_properties,
             vectorizer=_Text2VecPalmConfigCreate(
                 projectId=project_id,
                 apiEndpoint=api_endpoint,
                 modelId=model_id,
                 vectorizeClassName=vectorize_collection_name,
+                titleProperty=title_property,
             ),
             vector_index_config=vector_index_config,
         )
 
     @staticmethod
     def text2vec_transformers(
         name: str,
```

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/config_vector_index.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/config_vector_index.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     HNSW = "hnsw"
     FLAT = "flat"
     DYNAMIC = "dynamic"
 
 
 class _VectorIndexConfigCreate(_ConfigCreateModel):
     distance: Optional[VectorDistances]
-    vectorCacheMaxObjects: Optional[int]
     quantizer: Optional[_QuantizerConfigCreate] = Field(exclude=True)
 
     @staticmethod
     @abstractmethod
     def vector_index_type() -> VectorIndexType:
         ...
 
@@ -43,15 +42,14 @@
         if self.distance is not None:
             ret_dict["distance"] = str(self.distance.value)
 
         return ret_dict
 
 
 class _VectorIndexConfigUpdate(_ConfigUpdateModel):
-    vectorCacheMaxObjects: Optional[int]
     quantizer: Optional[_QuantizerConfigUpdate] = Field(exclude=True)
 
     @staticmethod
     @abstractmethod
     def vector_index_type() -> VectorIndexType:
         ...
 
@@ -69,21 +67,24 @@
     dynamicEfMin: Optional[int]
     dynamicEfMax: Optional[int]
     dynamicEfFactor: Optional[int]
     efConstruction: Optional[int]
     ef: Optional[int]
     flatSearchCutoff: Optional[int]
     maxConnections: Optional[int]
+    vectorCacheMaxObjects: Optional[int]
 
     @staticmethod
     def vector_index_type() -> VectorIndexType:
         return VectorIndexType.HNSW
 
 
 class _VectorIndexConfigFlatCreate(_VectorIndexConfigCreate):
+    vectorCacheMaxObjects: Optional[int]
+
     @staticmethod
     def vector_index_type() -> VectorIndexType:
         return VectorIndexType.FLAT
 
 
 class _VectorIndexConfigHNSWUpdate(_VectorIndexConfigUpdate):
     dynamicEfMin: Optional[int]
@@ -95,14 +96,16 @@
 
     @staticmethod
     def vector_index_type() -> VectorIndexType:
         return VectorIndexType.HNSW
 
 
 class _VectorIndexConfigFlatUpdate(_VectorIndexConfigUpdate):
+    vectorCacheMaxObjects: Optional[int]
+
     @staticmethod
     def vector_index_type() -> VectorIndexType:
         return VectorIndexType.FLAT
 
 
 class _VectorIndexConfigDynamicCreate(_VectorIndexConfigCreate):
     threshold: Optional[int]
@@ -111,10 +114,14 @@
 
     @staticmethod
     def vector_index_type() -> VectorIndexType:
         return VectorIndexType.DYNAMIC
 
 
 class _VectorIndexConfigDynamicUpdate(_VectorIndexConfigUpdate):
+    threshold: Optional[int]
+    hnsw: Optional[_VectorIndexConfigHNSWUpdate]
+    flat: Optional[_VectorIndexConfigFlatUpdate]
+
     @staticmethod
     def vector_index_type() -> VectorIndexType:
         return VectorIndexType.DYNAMIC
```

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/config_vectorizers.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/config_vectorizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     NONE = "none"
     TEXT2VEC_AWS = "text2vec-aws"
     TEXT2VEC_COHERE = "text2vec-cohere"
     TEXT2VEC_CONTEXTIONARY = "text2vec-contextionary"
     TEXT2VEC_GPT4ALL = "text2vec-gpt4all"
     TEXT2VEC_HUGGINGFACE = "text2vec-huggingface"
     TEXT2VEC_OCTOAI = "text2vec-octoai"
+    TEXT2VEC_OLLAMA = "text2vec-ollama"
     TEXT2VEC_OPENAI = "text2vec-openai"
     TEXT2VEC_PALM = "text2vec-palm"
     TEXT2VEC_TRANSFORMERS = "text2vec-transformers"
     TEXT2VEC_JINAAI = "text2vec-jinaai"
     TEXT2VEC_VOYAGEAI = "text2vec-voyageai"
     IMG2VEC_NEURAL = "img2vec-neural"
     MULTI2VEC_CLIP = "multi2vec-clip"
@@ -252,14 +253,15 @@
 
 class _Text2VecPalmConfig(_ConfigCreateModel):
     vectorizer: Vectorizers = Field(default=Vectorizers.TEXT2VEC_PALM, frozen=True, exclude=True)
     projectId: str
     apiEndpoint: Optional[str]
     modelId: Optional[str]
     vectorizeClassName: bool
+    titleProperty: Optional[str]
 
 
 class _Text2VecPalmConfigCreate(_Text2VecPalmConfig, _VectorizerConfigCreate):
     pass
 
 
 class _Text2VecTransformersConfig(_ConfigCreateModel):
@@ -313,14 +315,21 @@
 class _Text2VecOctoConfig(_VectorizerConfigCreate):
     vectorizer: Vectorizers = Field(default=Vectorizers.TEXT2VEC_OCTOAI, frozen=True, exclude=True)
     model: Optional[str]
     baseURL: Optional[str]
     vectorizeClassName: bool
 
 
+class _Text2VecOllamaConfig(_VectorizerConfigCreate):
+    vectorizer: Vectorizers = Field(default=Vectorizers.TEXT2VEC_OLLAMA, frozen=True, exclude=True)
+    model: Optional[str]
+    apiEndpoint: Optional[str]
+    vectorizeClassName: bool
+
+
 class _Img2VecNeuralConfig(_ConfigCreateModel):
     vectorizer: Vectorizers = Field(default=Vectorizers.IMG2VEC_NEURAL, frozen=True, exclude=True)
     imageFields: List[str]
 
 
 class _Img2VecNeuralConfigCreate(_Img2VecNeuralConfig, _VectorizerConfigCreate):
     pass
@@ -721,18 +730,18 @@
             vectorizeClassName=vectorize_collection_name,
         )
 
     @staticmethod
     def text2vec_octoai(
         *,
         base_url: Optional[str] = None,
-        model: Optional[Union[OpenAIModel, str]] = None,
+        model: Optional[str] = None,
         vectorize_collection_name: bool = True,
     ) -> _VectorizerConfigCreate:
-        """Create a `_Text2VecOctoConfig` object for use when vectorizing using the `text2vec-openai` model.
+        """Create a `_Text2VecOctoConfig` object for use when vectorizing using the `text2vec-octoai` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-octoai)
         for detailed usage.
 
         Arguments:
             `base_url`
                 The base URL to use where API requests should go. Defaults to `None`, which uses the server-defined default.
@@ -744,14 +753,40 @@
         return _Text2VecOctoConfig(
             baseURL=base_url,
             model=model,
             vectorizeClassName=vectorize_collection_name,
         )
 
     @staticmethod
+    def text2vec_ollama(
+        *,
+        api_endpoint: Optional[str] = None,
+        model: Optional[str] = None,
+        vectorize_collection_name: bool = True,
+    ) -> _VectorizerConfigCreate:
+        """Create a `_Text2VecOllamaConfig` object for use when vectorizing using the `text2vec-ollama` model.
+
+        See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-ollama)
+        for detailed usage.
+
+        Arguments:
+            `api_endpoint`
+                The base URL to use where API requests should go. Defaults to `None`, which uses the server-defined default.
+            `modelId`
+                The model to use. Defaults to `None`, which uses the server-defined default.
+            `vectorize_collection_name`
+                Whether to vectorize the collection name. Defaults to `True`.
+        """
+        return _Text2VecOllamaConfig(
+            apiEndpoint=api_endpoint,
+            model=model,
+            vectorizeClassName=vectorize_collection_name,
+        )
+
+    @staticmethod
     def text2vec_openai(
         model: Optional[Union[OpenAIModel, str]] = None,
         model_version: Optional[str] = None,
         type_: Optional[OpenAIType] = None,
         vectorize_collection_name: bool = True,
         base_url: Optional[AnyHttpUrl] = None,
         dimensions: Optional[int] = None,
@@ -788,39 +823,43 @@
         )
 
     @staticmethod
     def text2vec_palm(
         project_id: str,
         api_endpoint: Optional[str] = None,
         model_id: Optional[str] = None,
+        title_property: Optional[str] = None,
         vectorize_collection_name: bool = True,
     ) -> _VectorizerConfigCreate:
         """Create a `_Text2VecPalmConfigCreate` object for use when vectorizing using the `text2vec-palm` model.
 
         See the [documentation](https://weaviate.io/developers/weaviate/modules/retriever-vectorizer-modules/text2vec-palm)
         for detailed usage.
 
         Arguments:
             `project_id`
                 The project ID to use, REQUIRED.
             `api_endpoint`
                 The API endpoint to use without a leading scheme such as `http://`. Defaults to `None`, which uses the server-defined default
             `model_id`
                 The model ID to use. Defaults to `None`, which uses the server-defined default.
+            `title_property`
+                The Weaviate property name for the `gecko-002` or `gecko-003` model to use as the title.
             `vectorize_collection_name`
                 Whether to vectorize the collection name. Defaults to `True`.
 
         Raises:
             `pydantic.ValidationError` if `api_endpoint` is not a valid URL.
         """
         return _Text2VecPalmConfigCreate(
             projectId=project_id,
             apiEndpoint=api_endpoint,
             modelId=model_id,
             vectorizeClassName=vectorize_collection_name,
+            titleProperty=title_property,
         )
 
     @staticmethod
     def multi2vec_palm(
         *,
         location: str,
         project_id: str,
```

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/data.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/filters.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/grpc.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,31 +243,31 @@
 class _HybridNearVector(_HybridNearBase):
     vector: List[float]
 
 
 HybridVectorType = Union[List[float], _HybridNearText, _HybridNearVector]
 
 
-class HybridNear:
+class HybridVector:
     """Use this factory class to define the appropriate classes needed when defining near text and near vector sub-searches in hybrid queries."""
 
     @staticmethod
-    def text(
-        text: Union[str, List[str]],
+    def near_text(
+        query: Union[str, List[str]],
         *,
         certainty: Optional[float] = None,
         distance: Optional[float] = None,
         move_to: Optional[Move] = None,
         move_away: Optional[Move] = None,
         target_vector: Optional[str] = None
     ) -> _HybridNearText:
         """Define a near text search to be used within a hybrid query.
 
         Arguments:
-            `text`
+            `query`
                 The text to search for as a string or a list of strings.
             `certainty`
                 The minimum similarity score to return. If not specified, the default certainty specified by the server is used.
             `distance`
                 The maximum distance to search. If not specified, the default distance specified by the server is used.
             `move_to`
                 Define the concepts that should be moved towards in the vector space during the search.
@@ -276,24 +276,24 @@
             `target_vector`
                 The name of the vector space to search in for named vector configurations. Required if multiple spaces are configured.
 
         Returns:
             A `_HybridNearText` object to be used in the `vector` parameter of the `query.hybrid` and `generate.hybrid` search methods.
         """
         return _HybridNearText(
-            text=text,
+            text=query,
             distance=distance,
             certainty=certainty,
             move_to=move_to,
             move_away=move_away,
             target_vector=target_vector,
         )
 
     @staticmethod
-    def vector(
+    def near_vector(
         vector: List[float],
         *,
         certainty: Optional[float] = None,
         distance: Optional[float] = None,
         target_vector: Optional[str] = None
     ) -> _HybridNearVector:
         """Define a near vector search to be used within a hybrid query.
```

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/internal.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/internal.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/orm.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/tenants.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/classes/types.py` & `weaviate_client-4.6.0b1/weaviate/collections/classes/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/cluster.py` & `weaviate_client-4.6.0b1/weaviate/collections/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/collection.py` & `weaviate_client-4.6.0b1/weaviate/collections/collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/collections.py` & `weaviate_client-4.6.0b1/weaviate/collections/collections.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/config.py` & `weaviate_client-4.6.0b1/weaviate/collections/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/data.py` & `weaviate_client-4.6.0b1/weaviate/collections/data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/filters.py` & `weaviate_client-4.6.0b1/weaviate/collections/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/grpc/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/grpc/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/grpc/shared.py` & `weaviate_client-4.6.0b1/weaviate/collections/grpc/shared.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/grpc/tenants.py` & `weaviate_client-4.6.0b1/weaviate/collections/grpc/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/iterator.py` & `weaviate_client-4.6.0b1/weaviate/collections/iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/orm.py` & `weaviate_client-4.6.0b1/weaviate/collections/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/base.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/generate.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/generate.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/bm25/query.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/bm25/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/byteops.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/byteops.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_object_by_id/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_object_by_id/query.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_object_by_id/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/generate.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/generate.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/fetch_objects/query.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/fetch_objects/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/generate.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/generate.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/hybrid/query.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/hybrid/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/generate.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/generate.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_image/query.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_image/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/generate.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/generate.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_media/query.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_media/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/generate.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/generate.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_object/query.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_object/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/generate.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/generate.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_text/query.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_text/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/generate.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/generate.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/queries/near_vector/query.pyi` & `weaviate_client-4.6.0b1/weaviate/collections/queries/near_vector/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/query.py` & `weaviate_client-4.6.0b1/weaviate/collections/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/collections/tenants.py` & `weaviate_client-4.6.0b1/weaviate/collections/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/config.py` & `weaviate_client-4.6.0b1/weaviate/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/connect/authentication.py` & `weaviate_client-4.6.0b1/weaviate/connect/authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/connect/base.py` & `weaviate_client-4.6.0b1/weaviate/connect/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/connect/helpers.py` & `weaviate_client-4.6.0b1/weaviate/connect/helpers.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/connect/integrations.py` & `weaviate_client-4.6.0b1/weaviate/connect/integrations.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/connect/v3.py` & `weaviate_client-4.6.0b1/weaviate/connect/v3.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/connect/v4.py` & `weaviate_client-4.6.0b1/weaviate/connect/v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/contextionary/crud_contextionary.py` & `weaviate_client-4.6.0b1/weaviate/contextionary/crud_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/data/crud_data.py` & `weaviate_client-4.6.0b1/weaviate/data/crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/data/references/crud_references.py` & `weaviate_client-4.6.0b1/weaviate/data/references/crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/embedded.py` & `weaviate_client-4.6.0b1/weaviate/embedded.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/error_msgs.py` & `weaviate_client-4.6.0b1/weaviate/error_msgs.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/exceptions.py` & `weaviate_client-4.6.0b1/weaviate/exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/gql/aggregate.py` & `weaviate_client-4.6.0b1/weaviate/gql/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/gql/filter.py` & `weaviate_client-4.6.0b1/weaviate/gql/filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/gql/get.py` & `weaviate_client-4.6.0b1/weaviate/gql/get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/gql/multi_get.py` & `weaviate_client-4.6.0b1/weaviate/gql/multi_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/gql/query.py` & `weaviate_client-4.6.0b1/weaviate/gql/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/integrations.py` & `weaviate_client-4.6.0b1/weaviate/integrations.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/outputs/aggregate.py` & `weaviate_client-4.6.0b1/weaviate/outputs/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/outputs/config.py` & `weaviate_client-4.6.0b1/weaviate/outputs/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/outputs/query.py` & `weaviate_client-4.6.0b1/weaviate/outputs/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2.py` & `weaviate_client-4.6.0b1/weaviate/proto/v1/base_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/base_pb2.pyi` & `weaviate_client-4.6.0b1/weaviate/proto/v1/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2.py` & `weaviate_client-4.6.0b1/weaviate/proto/v1/batch_delete_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/batch_delete_pb2.pyi` & `weaviate_client-4.6.0b1/weaviate/proto/v1/batch_delete_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2.py` & `weaviate_client-4.6.0b1/weaviate/proto/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/batch_pb2.pyi` & `weaviate_client-4.6.0b1/weaviate/proto/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/properties_pb2.py` & `weaviate_client-4.6.0b1/weaviate/proto/v1/properties_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/properties_pb2.pyi` & `weaviate_client-4.6.0b1/weaviate/proto/v1/properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2.py` & `weaviate_client-4.6.0b1/weaviate/proto/v1/search_get_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/search_get_pb2.pyi` & `weaviate_client-4.6.0b1/weaviate/proto/v1/search_get_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/tenants_pb2.py` & `weaviate_client-4.6.0b1/weaviate/proto/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/tenants_pb2.pyi` & `weaviate_client-4.6.0b1/weaviate/proto/v1/tenants_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2.py` & `weaviate_client-4.6.0b1/weaviate/proto/v1/weaviate_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/proto/v1/weaviate_pb2_grpc.py` & `weaviate_client-4.6.0b1/weaviate/proto/v1/weaviate_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/schema/crud_schema.py` & `weaviate_client-4.6.0b1/weaviate/schema/crud_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/schema/properties/crud_properties.py` & `weaviate_client-4.6.0b1/weaviate/schema/properties/crud_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/types.py` & `weaviate_client-4.6.0b1/weaviate/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/util.py` & `weaviate_client-4.6.0b1/weaviate/util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/validator.py` & `weaviate_client-4.6.0b1/weaviate/validator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate/warnings.py` & `weaviate_client-4.6.0b1/weaviate/warnings.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.0b0/weaviate_client.egg-info/PKG-INFO` & `weaviate_client-4.6.0b1/weaviate_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.6.0b0
+Version: 4.6.0b1
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate_client-4.6.0b0/weaviate_client.egg-info/SOURCES.txt` & `weaviate_client-4.6.0b1/weaviate_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/dagster-cloud-cli-1.7.4.tar.gz` & `tmp/dagster-cloud-cli-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-cli-1.7.4.tar", last modified: Thu May  2 20:44:08 2024, max compression
+gzip compressed data, was "dagster-cloud-cli-1.7.5.tar", last modified: Thu May  9 17:58:34 2024, max compression
```

## Comparing `dagster-cloud-cli-1.7.4.tar` & `dagster-cloud-cli-1.7.5.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.818659 dagster-cloud-cli-1.7.4/
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-02 20:44:08.818659 dagster-cloud-cli-1.7.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.802659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)      160 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     5173 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    30031 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4121 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8651 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     2952 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1657 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)    17056 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1926 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     4001 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2691 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      669 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18361 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    12434 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18301 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/alert_types.py
--rw-r--r--   0 root         (0) root         (0)     4801 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    13677 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.810659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.814659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.814659 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9423 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    14436 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     6220 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     2106 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     7106 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2463 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    20701 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.806659 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3028 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       97 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-02 20:44:08.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:08.818659 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4130 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16177 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_deps.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8872 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:44:08.818659 dagster-cloud-cli-1.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1139 2024-05-02 20:32:04.000000 dagster-cloud-cli-1.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.728206 dagster-cloud-cli-1.7.5/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-09 17:58:34.728206 dagster-cloud-cli-1.7.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.688206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.688206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.688206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.692206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    30031 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      550 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8651 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)    17101 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     4001 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.704206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18458 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.704206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    12788 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.712206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/agent_queue.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/alert_types.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    13801 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.712206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.716206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.720206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9423 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    14436 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     8034 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    20800 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.688206 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      112 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.728206 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4130 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16177 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_deps.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8872 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 17:58:34.728206 dagster-cloud-cli-1.7.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1288 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/setup.py
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/__init__.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/checks.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/report.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/ci/state.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/state.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/config.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from typing import Optional
 
 import yaml
 from typer import Argument, Typer
 from typing_extensions import Annotated
 
 from ... import gql, ui
 from ...config_utils import dagster_cloud_options
@@ -23,31 +24,33 @@
 
 
 @settings_app.command(name="set-from-file")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def set_from_filecommand(
     api_token: str,
     url: str,
+    deployment: Optional[str],
     file_path: Path = Argument(..., readable=True, metavar="SETTINGS_FILE_PATH"),
 ):
     """Set the Dagster Cloud deployment settings from a YAML file."""
     with open(file_path, "r", encoding="utf8") as f:
         settings = {"settings": yaml.safe_load(f) or {}}
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         gql.set_deployment_settings(client, settings)
 
 
 @settings_app.command(name="get")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def get_command(
     api_token: str,
     url: str,
+    deployment: Optional[str],
 ):
     """Get the Dagster Cloud deployment settings."""
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         settings = gql.get_deployment_settings(client)
     ui.print_yaml(settings)
 
 
 @app.command(name="upload-artifact")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def upload_artifact_command(
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from typing import Optional
 
 import yaml
 from typer import Option, Typer
 
 from .... import gql, ui
 from ....config_utils import dagster_cloud_options
 from .config_schema import INSIGHTS_ALERT_POLICIES_SCHEMA, process_alert_policies_config
@@ -13,37 +14,39 @@
 
 
 @app.command(name="list")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def list_command(
     api_token: str,
     url: str,
+    deployment: Optional[str],
 ):
     """List your alert policies, output in YAML format."""
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         alert_policies_response = gql.get_alert_policies(client)
 
     ui.print_yaml(alert_policies_response)
 
 
 @app.command(name="sync")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def sync_command(
     api_token: str,
     url: str,
+    deployment: Optional[str],
     alert_policies_file: Path = Option(
         DEFAULT_ALERT_POLICIES_YAML_FILENAME,
         "--alert-policies",
         "-a",
         exists=True,
         help="Path to alert policies file.",
     ),
 ):
     """Sync your YAML configured alert policies to Dagster Cloud."""
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         with open(str(alert_policies_file), "r", encoding="utf8") as f:
             config = yaml.load(f.read(), Loader=yaml.SafeLoader)
 
         try:
             process_alert_policies_config(config, INSIGHTS_ALERT_POLICIES_SCHEMA)
 
             alert_policies = gql.reconcile_alert_policies(client, config)
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,15 @@
                             default_value=SINGLETON_REPOSITORY_NAME,
                         ),
                     }
                 ),
             }
         )
     ),
+    "credit_limit_target": Field(config={}),
 }
 
 ALERT_EVENT_TYPES = [
     EnumValue("JOB_FAILURE", description="Alert on job failure."),
     EnumValue("JOB_SUCCESS", description="Alert on job success."),
     EnumValue("TICK_FAILURE", description="Alert on schedule/sensor failure."),
     EnumValue("AGENT_UNAVAILABLE", description="Alert on agent downtime."),
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/job/__init__.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/job/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 
 @app.command(name="launch")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def launch(
     api_token: str,
     url: str,
+    deployment: Optional[str],
     location: str = typer.Option(..., "-l", "--location", help="Location name in the deployment."),
     job: str = typer.Option(..., "-j", "--job", help="Job name to run."),
     repository: str = typer.Option(
         None,
         "-r",
         "--repository",
         help=(
@@ -41,15 +42,15 @@
     ),
 ):
     """Launch a run for a job."""
     loaded_tags: Dict[str, Any] = json.loads(tags) if tags else {}
     loaded_config: Dict[str, Any] = json.loads(config) if config else {}
 
     repository = repository or SINGLETON_REPOSITORY_NAME
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         ui.print(
             gql.launch_run(
                 client,
                 location,
                 repository,
                 job,
                 loaded_tags,
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/metrics.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/__init__.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/run/__init__.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/run/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+from typing import Optional
+
 import typer
 from typer import Typer
 
 from ... import gql, ui
 from ...config_utils import dagster_cloud_options
 
 app = Typer(help="Commands for working with Dagster Cloud runs.")
 
 
 @app.command(name="status")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def status(
     api_token: str,
     url: str,
+    deployment: Optional[str],
     run_id: str = typer.Argument(None),
 ):
     """Check the status of a run."""
     # this should be replaced by using the `dagster` CLI against a dagster-cloud `dagster.yaml`
     if not run_id:
         raise ui.error("No run_id provided")
 
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         ui.print(gql.run_status(client, run_id))
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import json
 import os
 import subprocess
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 from dagster import _seven as seven
 from typer import Argument, Option, Typer
 
 from dagster_cloud_cli import docker_utils, gql, pex_utils, ui
 from dagster_cloud_cli.commands import metrics
 from dagster_cloud_cli.commands.workspace import wait_for_load
@@ -213,15 +213,15 @@
 
     _check_source_directory(source_directory)
     docker_utils.verify_docker()
 
     env_vars = kwargs.get("env", [])
     base_image = kwargs.get("base_image")
 
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         ecr_info = gql.get_ecr_info(client)
         registry = ecr_info["registry_url"]
 
         image_tag = kwargs.get("image") or docker_utils.default_image_tag(
             deployment, location_name, kwargs.get("commit_hash")
         )
         retval = docker_utils.build_image(
@@ -412,14 +412,15 @@
 @metrics.instrument(
     CliEventType.DEPLOY,
     tags=[CliEventTags.subcommand.dagster_cloud_serverless, CliEventTags.server_strategy.pex],
 )
 def deploy_python_executable_command(
     api_token: str,
     url: str,
+    deployment: Optional[str],
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     build_method: pex_builder.deps.BuildMethod,
     source_directory: Path = Argument(".", help="Source directory."),
     **kwargs,
 ):
     """Add a code location from a local directory, deployed as a Python executable."""
@@ -501,15 +502,15 @@
             api_token=api_token,
             location=location,
             build_method=build_method,
             kwargs=kwargs,
         )
         location_documents.append(get_location_document(location.name, location_kwargs))
 
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         for location_document in location_documents:
             gql.add_or_update_code_location(client, location_document)
 
         wait_for_load(
             client,
             [location.name for location in locations],
             location_load_timeout=location_load_timeout,
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,21 +67,22 @@
 
 @app.command(name="add-location", short_help="Add or update a code location image.")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 @add_options(DEPLOYMENT_CLI_OPTIONS)
 def add_command(
     api_token: str,
     url: str,
+    deployment: Optional[str],
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     location: str = Argument(None, help="Code location name."),
     **kwargs,
 ):
     """Add or update the image for a code location in the deployment."""
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         location_document = get_location_document(location, kwargs)
         _add_or_update_location(
             client,
             location_document,
             location_load_timeout=location_load_timeout,
             agent_heartbeat_timeout=agent_heartbeat_timeout,
             url=url,
@@ -99,21 +100,22 @@
 
 @app.command(name="update-location", short_help="Update a code location image.")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 @add_options(DEPLOYMENT_CLI_OPTIONS)
 def update_command(
     api_token: str,
     url: str,
+    deployment: Optional[str],
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     location: str = Argument(None, help="Code location name."),
     **kwargs,
 ):
     """Update the image for a code location in a deployment."""
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         location_document = get_location_document(location, kwargs)
         _add_or_update_location(
             client,
             location_document,
             location_load_timeout=location_load_timeout,
             agent_heartbeat_timeout=agent_heartbeat_timeout,
             url=url,
@@ -143,15 +145,15 @@
     locations,
     location_load_timeout=DEFAULT_LOCATION_LOAD_TIMEOUT,
     agent_heartbeat_timeout=DEFAULT_LOCATION_LOAD_TIMEOUT,
     url: Optional[str] = None,
 ):
     start_time = time.time()
     if url:
-        ui.print(f"View the status of your locations at {url}/workspace.\n")
+        ui.print(f"View the status of your locations at {url}/locations.\n")
     ui.print(f"Waiting for agent to sync changes to {list_locations(locations)}...")
 
     if not location_load_timeout and not agent_heartbeat_timeout:
         return
 
     has_agent_heartbeat = False
     iterations = 0
@@ -224,35 +226,37 @@
 @app.command(
     name="delete-location",
 )
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def delete_command(
     api_token: str,
     url: str,
+    deployment: Optional[str],
     location: str = Argument(..., help="Code location name."),
 ):
     """Delete a code location from the deployment."""
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         try:
             gql.delete_code_location(client, location)
             ui.print(f"Deleted location {location}.")
         except Exception as e:
             raise ui.error(str(e))
 
 
 @app.command(
     name="list",
 )
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def list_command(
     url: str,
+    deployment: Optional[str],
     api_token: str,
 ):
     """List code locations in the deployment."""
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         execute_list_command(client)
 
 
 def execute_list_command(client):
     list_res = gql.fetch_workspace_entries(client)
 
     ui.print("Listing locations...")
@@ -274,41 +278,43 @@
 
 
 @app.command(name="pull")
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def pull_command(
     url: str,
     api_token: str,
+    deployment: Optional[str],
 ):
     """Retrieve code location definitions as a workspace.yaml file."""
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         document = gql.fetch_locations_as_document(client)
         ui.print_yaml(document or {})
 
 
 @app.command(
     name="sync",
     short_help="Sync deployment code locations with a workspace.yaml file.",
 )
 @dagster_cloud_options(allow_empty=True, requires_url=True)
 def sync_command(
     url: str,
     api_token: str,
+    deployment: Optional[str],
     location_load_timeout: int,
     agent_heartbeat_timeout: int,
     workspace: Path = Option(
         DEFAULT_WORKSPACE_YAML_FILENAME,
         "--workspace",
         "-w",
         exists=True,
         help="Path to workspace file.",
     ),
 ):
     """Sync the workspace with the contents of a workspace.yaml file."""
-    with gql.graphql_client_from_url(url, api_token) as client:
+    with gql.graphql_client_from_url(url, api_token, deployment_name=deployment) as client:
         execute_sync_command(
             client,
             workspace,
             location_load_timeout=location_load_timeout,
             agent_heartbeat_timeout=agent_heartbeat_timeout,
             url=url,
         )
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/config_utils.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/alert_types.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/alert_types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/artifacts.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/docker_runner.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/errors.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/graphql_client.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/graphql_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -390,17 +390,24 @@
         retry_date = mktime_tz(retry_date)
         seconds = retry_date - time.time()
 
     return max(seconds, 0)
 
 
 @contextmanager
-def create_cloud_webserver_client(url: str, api_token: str, retries=3):
+def create_cloud_webserver_client(
+    url: str,
+    api_token: str,
+    retries=3,
+    deployment_name: Optional[str] = None,
+):
     with create_graphql_requests_session(adapter_kwargs={}) as session:
         yield DagsterCloudGraphQLClient(
             session=session,
             url=f"{url}/graphql",
             headers=get_dagster_cloud_api_headers(
-                api_token, scope=DagsterCloudInstanceScope.DEPLOYMENT
+                api_token,
+                scope=DagsterCloudInstanceScope.DEPLOYMENT,
+                deployment_name=deployment_name,
             ),
             max_retries=retries,
         )
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/headers/impl.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/git_context.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/gitlab_context.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/source.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pex_builder/util.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/core/workspace.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/workspace.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 from typing import Any, Dict, List, NamedTuple, Optional
 
 import dagster._check as check
+import yaml
 from dagster._core.instance.ref import InstanceRef
 from dagster._serdes import serialize_value, whitelist_for_serdes
 from dagster._utils.merger import merge_dicts
-from dagster_cloud.agent import AgentQueue
+
+from .agent_queue import AgentQueue
 
 
 @whitelist_for_serdes
 class GitMetadata(
     NamedTuple(
         "_GitMetadata",
         [("commit_hash", Optional[str]), ("url", Optional[str])],
@@ -53,14 +55,32 @@
             return None
         if serverless_service_name in ["serverless-agents", "serverless-agents-public-demo"]:
             return f"657821118200.dkr.ecr.us-west-2.amazonaws.com/dagster-cloud-serverless-base-py{self.python_version}:{agent_image_tag}"
         else:
             return f"878483074102.dkr.ecr.us-west-2.amazonaws.com/dagster-cloud-serverless-base-py{self.python_version}:{agent_image_tag}"
 
 
+def get_instance_ref_for_user_code(instance_ref: InstanceRef) -> InstanceRef:
+    # Remove fields from InstanceRef that may not be compatible with earlier
+    # versions of dagster and aren't actually needed by user code
+
+    custom_instance_class_data = instance_ref.custom_instance_class_data
+    if custom_instance_class_data:
+        config_dict = custom_instance_class_data.config_dict
+        new_config_dict = {
+            key: val for key, val in config_dict.items() if key not in {"agent_queues"}
+        }
+
+        custom_instance_class_data = custom_instance_class_data._replace(
+            config_yaml=yaml.dump(new_config_dict)
+        )
+
+    return instance_ref._replace(custom_instance_class_data=custom_instance_class_data)
+
+
 # History of CodeDeploymentMetadata
 # 1. Removal of `enable_metrics` field
 @whitelist_for_serdes
 class CodeDeploymentMetadata(
     NamedTuple(
         "_CodeDeploymentMetadata",
         [
@@ -155,15 +175,23 @@
         return merge_dicts(
             {
                 "DAGSTER_LOCATION_NAME": location_name,
                 "DAGSTER_INJECT_ENV_VARS_FROM_INSTANCE": "1",
                 "DAGSTER_CLI_API_GRPC_LAZY_LOAD_USER_CODE": "1",
                 "DAGSTER_CLI_API_GRPC_HOST": "0.0.0.0",
             },
-            ({"DAGSTER_INSTANCE_REF": serialize_value(instance_ref)} if instance_ref else {}),
+            (
+                {
+                    "DAGSTER_INSTANCE_REF": serialize_value(
+                        get_instance_ref_for_user_code(instance_ref)
+                    )
+                }
+                if instance_ref
+                else {}
+            ),
             ({"DAGSTER_CLI_API_GRPC_PORT": str(port)} if port else {}),
             ({"DAGSTER_CLI_API_GRPC_SOCKET": str(socket)} if socket else {}),
             ({"DAGSTER_CURRENT_IMAGE": self.image} if self.image else {}),
             ({"DAGSTER_CLI_API_GRPC_PYTHON_FILE": self.python_file} if self.python_file else {}),
             ({"DAGSTER_CLI_API_GRPC_MODULE_NAME": self.module_name} if self.module_name else {}),
             ({"DAGSTER_CLI_API_GRPC_PACKAGE_NAME": self.package_name} if self.package_name else {}),
             (
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/docker_utils.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/entrypoint.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/gql.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/gql.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,22 @@
 )
 
 from .core.graphql_client import DagsterCloudGraphQLClient, create_cloud_webserver_client
 
 
 @contextmanager
 def graphql_client_from_url(
-    url: str, token: str, retries: int = 3
+    url: str,
+    token: str,
+    retries: int = 3,
+    deployment_name: Optional[str] = None,
 ) -> Generator[DagsterCloudGraphQLClient, None, None]:
-    with create_cloud_webserver_client(url.rstrip("/"), token, retries) as client:
+    with create_cloud_webserver_client(
+        url.rstrip("/"), token, retries, deployment_name=deployment_name
+    ) as client:
         yield client
 
 
 def url_from_config(organization: str, deployment: Optional[str] = None) -> str:
     """Gets the Cloud webserver base url for a given organization and API token.
     Uses the default deployment if none is specified.
     """
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/pex_utils.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/types.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/ui.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli/utils.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 dagster_cloud_cli/commands/organization/saml/commands.py
 dagster_cloud_cli/commands/run/__init__.py
 dagster_cloud_cli/commands/serverless/Dockerfile
 dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
 dagster_cloud_cli/commands/serverless/__init__.py
 dagster_cloud_cli/commands/workspace/__init__.py
 dagster_cloud_cli/core/__init__.py
+dagster_cloud_cli/core/agent_queue.py
 dagster_cloud_cli/core/alert_types.py
 dagster_cloud_cli/core/artifacts.py
 dagster_cloud_cli/core/docker_runner.py
 dagster_cloud_cli/core/errors.py
 dagster_cloud_cli/core/graphql_client.py
 dagster_cloud_cli/core/pydantic_yaml.py
 dagster_cloud_cli/core/workspace.py
```

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_check.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_deps.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_gql.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/dagster_cloud_cli_tests/test_metrics.py` & `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.4/setup.py` & `dagster-cloud-cli-1.7.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,26 @@
     version: Dict[str, str] = {}
     with open(Path(__file__).parent / "dagster_cloud_cli/version.py", encoding="utf8") as fp:
         exec(fp.read(), version)
 
     return version["__version__"]
 
 
+ver = get_version()
+# dont pin dev installs to avoid pip dep resolver issues
+pin = "" if ver == "1!0+dev" else f"=={ver}"
+
 setup(
     name="dagster-cloud-cli",
     version=get_version(),
     author_email="hello@elementl.com",
     packages=find_packages(exclude=["dagster_cloud.cli_tests*"]),
     include_package_data=True,
     install_requires=[
+        "dagster==1.7.5",
         "packaging>=20.9",
         "questionary",
         "requests",
         "typer[all]>=0.4.1",
         "PyYAML>=5.1",
         "github3.py",
     ],
```


# Comparing `tmp/cdk_opinionated_constructs-3.7.2.tar.gz` & `tmp/cdk_opinionated_constructs-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_opinionated_constructs-3.7.2.tar", last modified: Thu Apr 25 11:25:03 2024, max compression
+gzip compressed data, was "cdk_opinionated_constructs-3.7.3.tar", last modified: Thu May  9 05:24:50 2024, max compression
```

## Comparing `cdk_opinionated_constructs-3.7.2.tar` & `cdk_opinionated_constructs-3.7.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.138684 cdk_opinionated_constructs-3.7.2/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk_opinionated_constructs-3.7.2/LICENSE
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-04-25 11:25:03.138620 cdk_opinionated_constructs-3.7.2/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    27598 2024-02-26 09:49:43.000000 cdk_opinionated_constructs-3.7.2/README.md
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.121819 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     5852 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/alb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2817 2024-01-24 11:50:26.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/ecr.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    10448 2024-01-24 12:01:51.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/lmb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     6821 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/nlb.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4710 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/rds_instance.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2933 2024-02-26 09:49:43.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/s3.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.122148 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/schemas/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/schemas/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3702 2024-03-06 09:09:15.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/schemas/configuration_vars.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1272 2024-02-26 09:49:43.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/sns.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.123618 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     9047 2024-04-25 11:23:56.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2261 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/code_quality_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     6602 2024-02-06 00:49:23.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/governance_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2101 2024-03-21 08:42:47.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1852 2024-03-21 08:42:47.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/integration_tests_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     7239 2024-04-08 20:49:10.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/notifications_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1872 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3644 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2077 2024-03-21 08:42:47.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/services_tests_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.124791 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1103 2024-03-04 14:20:14.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/code_quality_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      958 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      934 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/integration_tests_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1045 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/notifications_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1494 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/plugins_stage.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      915 2024-03-04 14:20:14.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/services_tests_stage.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.124958 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/utils/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2880 2024-02-05 22:11:31.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/utils/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)    15910 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/wafv2.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.138385 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs.egg-info/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-04-25 11:25:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs.egg-info/PKG-INFO
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2380 2024-04-25 11:25:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2024-04-25 11:25:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      125 2024-04-25 11:25:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs.egg-info/requires.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2024-04-25 11:25:03.000000 cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs.egg-info/top_level.txt
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2024-04-25 11:25:03.139119 cdk_opinionated_constructs-3.7.2/setup.cfg
--rw-r--r--   0 tomaszszuster   (501) staff       (20)      806 2024-04-25 11:23:56.000000 cdk_opinionated_constructs-3.7.2/setup.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.125246 cdk_opinionated_constructs-3.7.2/test/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk_opinionated_constructs-3.7.2/test/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1758 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/app.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.136323 cdk_opinionated_constructs-3.7.2/test/infrastucture/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/infrastucture/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2036 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/infrastucture/test_alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1173 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/infrastucture/test_ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1851 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/infrastucture/test_lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1516 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/infrastucture/test_s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1148 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/infrastucture/test_sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3739 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/infrastucture/test_wafv2_stack.py
-drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-04-25 11:25:03.137671 cdk_opinionated_constructs-3.7.2/test/stacks/
--rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk_opinionated_constructs-3.7.2/test/stacks/__init__.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3435 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/stacks/alb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1384 2024-01-24 11:27:38.000000 cdk_opinionated_constructs-3.7.2/test/stacks/ecr_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     4412 2024-01-24 11:50:26.000000 cdk_opinionated_constructs-3.7.2/test/stacks/lmb_docker_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3591 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/stacks/lmb_monitoring_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2719 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/stacks/lmb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2152 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/stacks/nlb_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3293 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/stacks/rds_mysql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     3308 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/stacks/rds_postgresql_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1619 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/stacks/s3_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     1067 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/stacks/sns_stack.py
--rw-r--r--   0 tomaszszuster   (501) staff       (20)     2567 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.2/test/stacks/wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.103721 cdk_opinionated_constructs-3.7.3/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1071 2022-11-05 20:03:58.000000 cdk_opinionated_constructs-3.7.3/LICENSE
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-05-09 05:24:50.103658 cdk_opinionated_constructs-3.7.3/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    27598 2024-02-26 09:49:43.000000 cdk_opinionated_constructs-3.7.3/README.md
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.098440 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     5852 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/alb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2817 2024-01-24 11:50:26.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/ecr.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    10448 2024-01-24 12:01:51.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/lmb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     6821 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/nlb.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4710 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/rds_instance.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2933 2024-02-26 09:49:43.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/s3.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.098686 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/schemas/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/schemas/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3702 2024-03-06 09:09:15.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/schemas/configuration_vars.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1272 2024-02-26 09:49:43.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/sns.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.099722 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     9546 2024-05-09 05:24:13.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2261 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/code_quality_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     6602 2024-02-06 00:49:23.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/governance_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2101 2024-03-21 08:42:47.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1852 2024-03-21 08:42:47.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/integration_tests_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     7239 2024-04-08 20:49:10.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/notifications_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1872 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3644 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2077 2024-03-21 08:42:47.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/services_tests_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.100505 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1103 2024-03-04 14:20:14.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/code_quality_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      958 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      934 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/integration_tests_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1045 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/notifications_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1494 2024-02-05 18:17:09.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/plugins_stage.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      915 2024-03-04 14:20:14.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/services_tests_stage.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.100617 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/utils/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2880 2024-02-05 22:11:31.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/utils/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)    15910 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/wafv2.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.103450 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs.egg-info/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      555 2024-05-09 05:24:50.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2380 2024-05-09 05:24:50.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        1 2024-05-09 05:24:50.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      125 2024-05-09 05:24:50.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs.egg-info/requires.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)       32 2024-05-09 05:24:50.000000 cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs.egg-info/top_level.txt
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3649 2024-05-09 05:24:50.104153 cdk_opinionated_constructs-3.7.3/setup.cfg
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)      806 2024-05-09 05:24:33.000000 cdk_opinionated_constructs-3.7.3/setup.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.100816 cdk_opinionated_constructs-3.7.3/test/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk_opinionated_constructs-3.7.3/test/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1758 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/app.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.101569 cdk_opinionated_constructs-3.7.3/test/infrastucture/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/infrastucture/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2036 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/infrastucture/test_alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1173 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/infrastucture/test_ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1851 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/infrastucture/test_lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1516 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/infrastucture/test_s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1148 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/infrastucture/test_sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3739 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/infrastucture/test_wafv2_stack.py
+drwxr-xr-x   0 tomaszszuster   (501) staff       (20)        0 2024-05-09 05:24:50.102785 cdk_opinionated_constructs-3.7.3/test/stacks/
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)        0 2022-11-20 13:08:21.000000 cdk_opinionated_constructs-3.7.3/test/stacks/__init__.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3435 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/stacks/alb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1384 2024-01-24 11:27:38.000000 cdk_opinionated_constructs-3.7.3/test/stacks/ecr_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     4412 2024-01-24 11:50:26.000000 cdk_opinionated_constructs-3.7.3/test/stacks/lmb_docker_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3591 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/stacks/lmb_monitoring_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2719 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/stacks/lmb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2152 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/stacks/nlb_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3293 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/stacks/rds_mysql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     3308 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/stacks/rds_postgresql_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1619 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/stacks/s3_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     1067 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/stacks/sns_stack.py
+-rw-r--r--   0 tomaszszuster   (501) staff       (20)     2567 2024-01-17 10:21:03.000000 cdk_opinionated_constructs-3.7.3/test/stacks/wafv2_stack.py
```

### Comparing `cdk_opinionated_constructs-3.7.2/LICENSE` & `cdk_opinionated_constructs-3.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/PKG-INFO` & `cdk_opinionated_constructs-3.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-opinionated-constructs
-Version: 3.7.2
+Version: 3.7.3
 Summary: AWS CDK constructs come without added security configurations.
 License: MIT
 Requires-Python: >=3.11
 License-File: LICENSE
 Requires-Dist: aws-cdk-lib>=2.98.0
 Requires-Dist: constructs>=10.2.69
 Requires-Dist: cdk-monitoring-constructs>=6.0.0
```

### Comparing `cdk_opinionated_constructs-3.7.2/README.md` & `cdk_opinionated_constructs-3.7.3/README.md`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/alb.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/alb.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/ecr.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/ecr.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/lmb.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/lmb.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/nlb.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/nlb.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/rds_instance.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/rds_instance.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/s3.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/s3.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/schemas/configuration_vars.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/schemas/configuration_vars.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/sns.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/sns.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/__init__.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -131,24 +131,32 @@
     # The CodePipeline notifications available rules:
     # https://docs.aws.amazon.com/dtconsole/latest/userguide/concepts.html#events-ref-repositories
     NotificationRule(
         self,
         "codepipeline_notifications",
         detail_type=DetailType.FULL,
         events=[
-            "codepipeline-pipeline-pipeline-execution-failed",
+            "codepipeline-pipeline-action-execution-canceled",
+            "codepipeline-pipeline-action-execution-failed",
+            "codepipeline-pipeline-action-execution-started",
+            "codepipeline-pipeline-action-execution-succeeded",
+            "codepipeline-pipeline-manual-approval-failed",
+            "codepipeline-pipeline-manual-approval-needed",
+            "codepipeline-pipeline-manual-approval-succeeded",
             "codepipeline-pipeline-pipeline-execution-canceled",
-            "codepipeline-pipeline-pipeline-execution-started",
+            "codepipeline-pipeline-pipeline-execution-failed",
             "codepipeline-pipeline-pipeline-execution-resumed",
+            "codepipeline-pipeline-pipeline-execution-started",
             "codepipeline-pipeline-pipeline-execution-succeeded",
             "codepipeline-pipeline-pipeline-execution-superseded",
-            "codepipeline-pipeline-action-execution-failed",
+            "codepipeline-pipeline-stage-execution-canceled",
             "codepipeline-pipeline-stage-execution-failed",
-            "codepipeline-pipeline-manual-approval-failed",
-            "codepipeline-pipeline-manual-approval-needed",
+            "codepipeline-pipeline-stage-execution-resumed",
+            "codepipeline-pipeline-stage-execution-started",
+            "codepipeline-pipeline-stage-execution-succeeded",
         ],
         source=self.codepipeline.pipeline,
         targets=[sns_topic],
     )
 
 
 def pipeline_email_notifications(sns_topic: sns.Topic) -> None:
```

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/code_quality_stack.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/code_quality_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/governance_stack.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/governance_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/infrastructure_tests_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/integration_tests_stack.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/integration_tests_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/notifications_stack.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/notifications_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/pipeline_plugins_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/pipeline_trigger_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stacks/services_tests_stack.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stacks/services_tests_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/code_quality_stage.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/code_quality_stage.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/infrastructure_tests_stage.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/integration_tests_stage.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/integration_tests_stage.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/notifications_stage.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/notifications_stage.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/plugins_stage.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/plugins_stage.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/stages/services_tests_stage.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/stages/services_tests_stage.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/utils/__init__.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs/wafv2.py` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs/wafv2.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs.egg-info/PKG-INFO` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-opinionated-constructs
-Version: 3.7.2
+Version: 3.7.3
 Summary: AWS CDK constructs come without added security configurations.
 License: MIT
 Requires-Python: >=3.11
 License-File: LICENSE
 Requires-Dist: aws-cdk-lib>=2.98.0
 Requires-Dist: constructs>=10.2.69
 Requires-Dist: cdk-monitoring-constructs>=6.0.0
```

### Comparing `cdk_opinionated_constructs-3.7.2/cdk_opinionated_constructs.egg-info/SOURCES.txt` & `cdk_opinionated_constructs-3.7.3/cdk_opinionated_constructs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/setup.cfg` & `cdk_opinionated_constructs-3.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/setup.py` & `cdk_opinionated_constructs-3.7.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 https://packaging.python.org/en/latest/distributing.html
 """
 
 from setuptools import find_packages, setup
 
 setup(
     name="cdk-opinionated-constructs",
-    version="3.7.2",
+    version="3.7.3",
     description="AWS CDK constructs come without added security configurations.",
     long_description="The idea behind this project is to create secured constructs from the start. \n"
     "Supported constructs: ALB, ECR, LMB, NLB, S3, SNS, WAF, RDS",
     license="MIT",
     package_dir={"": "."},
     packages=find_packages(where="."),
     install_requires=[
```

### Comparing `cdk_opinionated_constructs-3.7.2/test/app.py` & `cdk_opinionated_constructs-3.7.3/test/app.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/infrastucture/test_alb_stack.py` & `cdk_opinionated_constructs-3.7.3/test/infrastucture/test_alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/infrastucture/test_ecr_stack.py` & `cdk_opinionated_constructs-3.7.3/test/infrastucture/test_ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/infrastucture/test_lmb_stack.py` & `cdk_opinionated_constructs-3.7.3/test/infrastucture/test_lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/infrastucture/test_s3_stack.py` & `cdk_opinionated_constructs-3.7.3/test/infrastucture/test_s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/infrastucture/test_sns_stack.py` & `cdk_opinionated_constructs-3.7.3/test/infrastucture/test_sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/infrastucture/test_wafv2_stack.py` & `cdk_opinionated_constructs-3.7.3/test/infrastucture/test_wafv2_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/alb_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/ecr_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/ecr_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/lmb_docker_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/lmb_docker_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/lmb_monitoring_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/lmb_monitoring_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/lmb_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/lmb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/nlb_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/nlb_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/rds_mysql_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/rds_mysql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/rds_postgresql_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/rds_postgresql_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/s3_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/s3_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/sns_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/sns_stack.py`

 * *Files identical despite different names*

### Comparing `cdk_opinionated_constructs-3.7.2/test/stacks/wafv2_stack.py` & `cdk_opinionated_constructs-3.7.3/test/stacks/wafv2_stack.py`

 * *Files identical despite different names*


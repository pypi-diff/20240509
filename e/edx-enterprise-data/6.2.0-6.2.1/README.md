# Comparing `tmp/edx-enterprise-data-6.2.0.tar.gz` & `tmp/edx_enterprise_data-6.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-data-6.2.0.tar", last modified: Thu Mar  7 11:04:08 2024, max compression
+gzip compressed data, was "edx_enterprise_data-6.2.1.tar", last modified: Thu May  9 13:58:04 2024, max compression
```

## Comparing `edx-enterprise-data-6.2.0.tar` & `edx_enterprise_data-6.2.1.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.361820 edx-enterprise-data-6.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-07 11:04:08.361820 edx-enterprise-data-6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.357820 edx-enterprise-data-6.2.0/edx_enterprise_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-03-07 11:04:08.000000 edx-enterprise-data-6.2.0/edx_enterprise_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-03-07 11:04:08.000000 edx-enterprise-data-6.2.0/edx_enterprise_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 11:04:08.000000 edx-enterprise-data-6.2.0/edx_enterprise_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 11:04:08.000000 edx-enterprise-data-6.2.0/edx_enterprise_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-07 11:04:08.000000 edx-enterprise-data-6.2.0/edx_enterprise_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-07 11:04:08.000000 edx-enterprise-data-6.2.0/edx_enterprise_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.337819 edx-enterprise-data-6.2.0/enterprise_data/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.337819 edx-enterprise-data-6.2.0/enterprise_data/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.337819 edx-enterprise-data-6.2.0/enterprise_data/api/v0/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/v0/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/v0/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/v0/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.337819 edx-enterprise-data-6.2.0/enterprise_data/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/v1/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    22434 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.337819 edx-enterprise-data-6.2.0/enterprise_data/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/fixtures/enterprise_enrollment.json
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/fixtures/enterprise_user.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.337819 edx-enterprise-data-6.2.0/enterprise_data/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.341819 edx-enterprise-data-6.2.0/enterprise_data/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_dummy_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_offer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.341819 edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_enterprise_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.345820 edx-enterprise-data-6.2.0/enterprise_data/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0002_auto_20180430_1358.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0003_auto_20180501_0603.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0004_auto_20180501_0928.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0004_auto_20180508_1652.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0005_auto_20180524_2204.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0006_auto_20180612_0336.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0007_auto_20180612_0534.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0008_auto_20180614_0108.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0009_auto_20180628_1152.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0010_enterpriseenrollment_created.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0011_enterpriseuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0012_auto_20180831_1930.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0013_auto_20180831_1931.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0014_enterpriseuser_created.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0015_auto_20180907_1757.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0016_auto_20180924_2138.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0021_auto_20190329_1241.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0024_auto_20210602_1811.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0025_auto_20210703_1854.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0026_auto_20210916_0414.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0029_enterpriseoffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0030_auto_20230609_1353.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0031_auto_20230615_0705.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0032_auto_20230704_0818.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0033_enterpriseadminlearnerprogress_enterpriseadminsummarizeinsights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0034_auto_20230907_0834.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0035_auto_20230907_1154.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0036_enterprisesubsidybudget_subsidy_access_policy_display_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0037_alter_enterpriseenrollment_consent_granted.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0038_enterpriseoffer_export_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/0039_auto_20240212_1403.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/paginators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/renderers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.349820 edx-enterprise-data-6.2.0/enterprise_data/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.349820 edx-enterprise-data-6.2.0/enterprise_data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.349820 edx-enterprise-data-6.2.0/enterprise_data/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.349820 edx-enterprise-data-6.2.0/enterprise_data/tests/api/v0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/api/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/api/v0/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.349820 edx-enterprise-data-6.2.0/enterprise_data/tests/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/api/v1/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/api/v1/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    69667 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.349820 edx-enterprise-data-6.2.0/enterprise_data_roles/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.353819 edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.353819 edx-enterprise-data-6.2.0/enterprise_data_roles/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_data_roles/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.353819 edx-enterprise-data-6.2.0/enterprise_reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.353819 edx-enterprise-data-6.2.0/enterprise_reporting/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/clients/enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/clients/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/clients/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/clients/vertica.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/external_resource_link_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.353819 edx-enterprise-data-6.2.0/enterprise_reporting/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/fixtures/enterprise_customer_reporting.json
--rw-r--r--   0 runner    (1001) docker     (127)    13807 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/send_enterprise_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.357820 edx-enterprise-data-6.2.0/enterprise_reporting/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_enterprise_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_external_link_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_send_enterprise_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_vertica_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/enterprise_reporting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 11:04:08.357820 edx-enterprise-data-6.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)     5818 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/common_constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9042 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/pip.txt
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/pip_tools.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/quality.txt
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/reporting.in
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/test-master.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/test-reporting.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 11:04:08.361820 edx-enterprise-data-6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-03-07 11:04:05.000000 edx-enterprise-data-6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.336246 edx_enterprise_data-6.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-09 13:58:04.336246 edx_enterprise_data-6.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.336246 edx_enterprise_data-6.2.1/edx_enterprise_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-09 13:58:04.000000 edx_enterprise_data-6.2.1/edx_enterprise_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-05-09 13:58:04.000000 edx_enterprise_data-6.2.1/edx_enterprise_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:58:04.000000 edx_enterprise_data-6.2.1/edx_enterprise_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:58:04.000000 edx_enterprise_data-6.2.1/edx_enterprise_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-09 13:58:04.000000 edx_enterprise_data-6.2.1/edx_enterprise_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 13:58:04.000000 edx_enterprise_data-6.2.1/edx_enterprise_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.316246 edx_enterprise_data-6.2.1/enterprise_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.316246 edx_enterprise_data-6.2.1/enterprise_data/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.316246 edx_enterprise_data-6.2.1/enterprise_data/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/v0/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/v0/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/v0/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.316246 edx_enterprise_data-6.2.1/enterprise_data/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/v1/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22434 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.316246 edx_enterprise_data-6.2.1/enterprise_data/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/fixtures/enterprise_enrollment.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/fixtures/enterprise_user.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.316246 edx_enterprise_data-6.2.1/enterprise_data/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.316246 edx_enterprise_data-6.2.1/enterprise_data/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_dummy_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_offer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.316246 edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_enterprise_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.324246 edx_enterprise_data-6.2.1/enterprise_data/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0002_auto_20180430_1358.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0003_auto_20180501_0603.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0004_auto_20180501_0928.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0004_auto_20180508_1652.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0005_auto_20180524_2204.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0006_auto_20180612_0336.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0007_auto_20180612_0534.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0008_auto_20180614_0108.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0009_auto_20180628_1152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0010_enterpriseenrollment_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0011_enterpriseuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0012_auto_20180831_1930.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0013_auto_20180831_1931.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0014_enterpriseuser_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0015_auto_20180907_1757.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0016_auto_20180924_2138.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0017_enterpriseenrollment_unenrollment_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0020_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0021_auto_20190329_1241.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0024_auto_20210602_1811.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0025_auto_20210703_1854.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0026_auto_20210916_0414.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0027_enterpriselearnerenrollment_total_learning_time_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0028_enterpriselearnerenrollment_offer_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0029_enterpriseoffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0030_auto_20230609_1353.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0031_auto_20230615_0705.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0032_auto_20230704_0818.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0033_enterpriseadminlearnerprogress_enterpriseadminsummarizeinsights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0034_auto_20230907_0834.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0035_auto_20230907_1154.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0036_enterprisesubsidybudget_subsidy_access_policy_display_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0037_alter_enterpriseenrollment_consent_granted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0038_enterpriseoffer_export_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/0039_auto_20240212_1403.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18765 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.324246 edx_enterprise_data-6.2.1/enterprise_data/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.324246 edx_enterprise_data-6.2.1/enterprise_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.324246 edx_enterprise_data-6.2.1/enterprise_data/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.328246 edx_enterprise_data-6.2.1/enterprise_data/tests/api/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/api/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/api/v0/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.328246 edx_enterprise_data-6.2.1/enterprise_data/tests/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/api/v1/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/api/v1/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14586 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69667 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.328246 edx_enterprise_data-6.2.1/enterprise_data_roles/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.328246 edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0004_enterprisedataroleassignment_enterprise_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.328246 edx_enterprise_data-6.2.1/enterprise_data_roles/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_data_roles/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.332246 edx_enterprise_data-6.2.1/enterprise_reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.332246 edx_enterprise_data-6.2.1/enterprise_reporting/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/clients/enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/clients/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/clients/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/clients/vertica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8066 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/external_resource_link_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.332246 edx_enterprise_data-6.2.1/enterprise_reporting/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/fixtures/enterprise_customer_reporting.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13807 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/send_enterprise_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.332246 edx_enterprise_data-6.2.1/enterprise_reporting/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_enterprise_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_external_link_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_send_enterprise_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_vertica_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13860 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/enterprise_reporting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:58:04.336246 edx_enterprise_data-6.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/common_constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9594 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/pip.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/pip_tools.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/quality.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/reporting.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/test-master.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/test-reporting.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:58:04.336246 edx_enterprise_data-6.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-09 13:58:01.000000 edx_enterprise_data-6.2.1/setup.py
```

### Comparing `edx-enterprise-data-6.2.0/CHANGELOG.rst` & `edx_enterprise_data-6.2.1/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
 =========================
+[6.2.1] - 2024-05-09
+---------------------
+  * Bump version
+
 [6.2.0] - 2024-03-06
 ---------------------
   * Dropped support for ``Django<4.2``
   * Added support for ``Python 3.12``
 
 [6.1.1] - 2024-02-22
 ---------------------
```

### Comparing `edx-enterprise-data-6.2.0/LICENSE` & `edx_enterprise_data-6.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/MANIFEST.in` & `edx_enterprise_data-6.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/PKG-INFO` & `edx_enterprise_data-6.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 6.2.0
+Version: 6.2.1
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
```

### Comparing `edx-enterprise-data-6.2.0/README.md` & `edx_enterprise_data-6.2.1/README.md`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/edx_enterprise_data.egg-info/PKG-INFO` & `edx_enterprise_data-6.2.1/edx_enterprise_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-data
-Version: 6.2.0
+Version: 6.2.1
 Summary: Enterprise Reporting
 Home-page: https://github.com/openedx/edx-enterprise-data
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
```

### Comparing `edx-enterprise-data-6.2.0/edx_enterprise_data.egg-info/SOURCES.txt` & `edx_enterprise_data-6.2.1/edx_enterprise_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/api/v0/serializers.py` & `edx_enterprise_data-6.2.1/enterprise_data/api/v0/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/api/v0/urls.py` & `edx_enterprise_data-6.2.1/enterprise_data/api/v0/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/api/v0/views.py` & `edx_enterprise_data-6.2.1/enterprise_data/api/v0/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/api/v1/serializers.py` & `edx_enterprise_data-6.2.1/enterprise_data/api/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/api/v1/urls.py` & `edx_enterprise_data-6.2.1/enterprise_data/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/api/v1/views.py` & `edx_enterprise_data-6.2.1/enterprise_data/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/clients.py` & `edx_enterprise_data-6.2.1/enterprise_data/clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/filters.py` & `edx_enterprise_data-6.2.1/enterprise_data/filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/fixtures/enterprise_enrollment.json` & `edx_enterprise_data-6.2.1/enterprise_data/fixtures/enterprise_enrollment.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/fixtures/enterprise_user.json` & `edx_enterprise_data-6.2.1/enterprise_data/fixtures/enterprise_user.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_dummy_data.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_dummy_data.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_dummy_data_lpr_v1.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_enrollment.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_offer.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_offer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/create_enterprise_user.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_dummy_data_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_enterprise_enrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_enterprise_learner_enrollment_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_enterprise_learner_lpr_v1.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/management/commands/tests/test_create_enterprise_user.py` & `edx_enterprise_data-6.2.1/enterprise_data/management/commands/tests/test_create_enterprise_user.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0001_initial.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0002_auto_20180430_1358.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0002_auto_20180430_1358.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0006_auto_20180612_0336.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0006_auto_20180612_0336.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0007_auto_20180612_0534.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0007_auto_20180612_0534.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0008_auto_20180614_0108.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0008_auto_20180614_0108.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0009_auto_20180628_1152.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0009_auto_20180628_1152.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0011_enterpriseuser.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0011_enterpriseuser.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0012_auto_20180831_1930.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0012_auto_20180831_1930.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0018_enterprisedatafeaturerole_enterprisedataroleassignment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0019_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0020_add_role_based_access_control_switch.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0020_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0021_auto_20190329_1241.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0021_auto_20190329_1241.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0022_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0023_enterpriselearner_enterpriselearnerenrollment.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0024_auto_20210602_1811.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0024_auto_20210602_1811.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0026_auto_20210916_0414.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0026_auto_20210916_0414.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0029_enterpriseoffer.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0029_enterpriseoffer.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0030_auto_20230609_1353.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0030_auto_20230609_1353.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0031_auto_20230615_0705.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0031_auto_20230615_0705.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0032_auto_20230704_0818.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0032_auto_20230704_0818.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0033_enterpriseadminlearnerprogress_enterpriseadminsummarizeinsights.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0033_enterpriseadminlearnerprogress_enterpriseadminsummarizeinsights.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0034_auto_20230907_0834.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0034_auto_20230907_0834.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0035_auto_20230907_1154.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0035_auto_20230907_1154.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/migrations/0039_auto_20240212_1403.py` & `edx_enterprise_data-6.2.1/enterprise_data/migrations/0039_auto_20240212_1403.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/models.py` & `edx_enterprise_data-6.2.1/enterprise_data/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/renderers.py` & `edx_enterprise_data-6.2.1/enterprise_data/renderers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/settings/test.py` & `edx_enterprise_data-6.2.1/enterprise_data/settings/test.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/signals.py` & `edx_enterprise_data-6.2.1/enterprise_data/signals.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/api/v0/test_serializers.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/api/v0/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/api/v1/test_serializers.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/api/v1/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/api/v1/test_views.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/api/v1/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/factories.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/mixins.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/test_clients.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/test_filters.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/test_models.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/test_utils.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/tests/test_views.py` & `edx_enterprise_data-6.2.1/enterprise_data/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data/utils.py` & `edx_enterprise_data-6.2.1/enterprise_data/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/admin.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/admin.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0001_initial.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0002_add_enterprise_data_feature_roles.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0003_add_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0005_turn_on_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0006_remove_role_based_access_control_switch.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/migrations/0007_enterprisedataroleassignment_applies_to_all_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/models.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/rules.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/rules.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/tests/factories.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_data_roles/tests/test_models.py` & `edx_enterprise_data-6.2.1/enterprise_data_roles/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/clients/__init__.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/clients/enterprise.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/clients/enterprise.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/clients/s3.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/clients/s3.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/clients/snowflake.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/clients/snowflake.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/clients/vertica.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/clients/vertica.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/delivery_method.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/external_resource_link_report.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/external_resource_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/fixtures/enterprise_customer_reporting.json` & `edx_enterprise_data-6.2.1/enterprise_reporting/fixtures/enterprise_customer_reporting.json`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/reporter.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/send_enterprise_reports.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_clients.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_delivery_method.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_delivery_method.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_enterprise_client.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_enterprise_client.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_external_link_report.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_external_link_report.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_reporter.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_send_enterprise_reports.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_send_enterprise_reports.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/tests/test_utils.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/tests/utils.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/enterprise_reporting/utils.py` & `edx_enterprise_data-6.2.1/enterprise_reporting/utils.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/requirements/base.txt` & `edx_enterprise_data-6.2.1/requirements/base.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
 amqp==5.2.0
     # via kombu
-asgiref==3.7.2
+asgiref==3.8.1
     # via django
 asn1crypto==1.5.1
     # via snowflake-connector-python
-awscli==1.32.56
+awscli==1.32.99
     # via -r requirements/reporting.in
 backports-zoneinfo[tzdata]==0.2.1 ; python_version < "3.9"
     # via
     #   -c requirements/constraints.txt
     #   celery
     #   django
+    #   djangorestframework
     #   kombu
-bcrypt==4.1.2
+bcrypt==4.1.3
     # via paramiko
 billiard==4.2.0
     # via celery
-boto3==1.34.56
+boto3==1.34.99
     # via -r requirements/reporting.in
-botocore==1.34.56
+botocore==1.34.99
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==5.3.6
     # via -r requirements/reporting.in
 certifi==2024.2.2
@@ -48,32 +49,32 @@
 click==8.1.7
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   edx-django-utils
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
-colorama==0.4.4
+colorama==0.4.6
     # via awscli
-cryptography==42.0.5
+cryptography==42.0.7
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields-v2
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
-django==4.2.11
+django==4.2.12
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields-v2
     #   django-filter
     #   django-model-utils
@@ -85,127 +86,128 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields-v2==0.9
     # via -r requirements/base.in
-django-filter==23.5
+django-filter==24.2
     # via -r requirements/base.in
-django-model-utils==4.4.0
+django-model-utils==4.5.1
     # via
     #   -r requirements/base.in
     #   edx-rbac
 django-waffle==4.1.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.14.0
+djangorestframework==3.15.1
     # via
     #   djangorestframework-csv
     #   drf-jwt
     #   edx-drf-extensions
 djangorestframework-csv==3.0.2
     # via -r requirements/base.in
+dnspython==2.6.1
+    # via pymongo
 docutils==0.16
     # via awscli
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.10.1
+edx-django-utils==5.13.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==10.2.0
+edx-drf-extensions==10.3.0
     # via
     #   -r requirements/base.in
     #   edx-rbac
-edx-opaque-keys==2.5.1
+edx-opaque-keys==2.9.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
-edx-rbac==1.8.0
+edx-rbac==1.9.0
     # via -r requirements/base.in
-edx-rest-api-client==5.6.1
+edx-rest-api-client==5.7.0
     # via -r requirements/base.in
 factory-boy==3.3.0
     # via -r requirements/base.in
-faker==24.0.0
+faker==25.0.1
     # via factory-boy
-filelock==3.13.1
+filelock==3.14.0
     # via snowflake-connector-python
-idna==3.6
+idna==3.7
     # via
     #   requests
     #   snowflake-connector-python
 interchange==2021.0.4
     # via py2neo
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-kombu==5.3.5
+kombu==5.3.7
     # via celery
 monotonic==1.6
     # via py2neo
-newrelic==9.7.0
+newrelic==9.9.0
     # via edx-django-utils
-packaging==23.2
+packaging==24.0
     # via
     #   py2neo
     #   snowflake-connector-python
 pansi==2020.7.3
     # via py2neo
 paramiko==3.4.0
     # via -r requirements/reporting.in
 pbr==6.0.0
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
-platformdirs==3.11.0
+platformdirs==4.2.1
     # via snowflake-connector-python
 prompt-toolkit==3.0.43
     # via click-repl
 psutil==5.9.8
     # via edx-django-utils
 py2neo @ https://github.com/overhangio/py2neo/releases/download/2021.2.3/py2neo-2021.2.3.tar.gz
     # via -r requirements/reporting.in
-pyasn1==0.5.1
+pyasn1==0.6.0
     # via
     #   pgpy
     #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.17.2
+pygments==2.18.0
     # via py2neo
 pyjwt[crypto]==2.8.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.13.0
+pymongo==4.4.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==24.0.0
+pyopenssl==24.1.0
     # via snowflake-connector-python
 python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   celery
     #   faker
     #   vertica-python
 pytz==2024.1
     # via
-    #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==6.0.1
     # via awscli
 requests==2.31.0
     # via
     #   -r requirements/base.in
@@ -213,15 +215,15 @@
     #   edx-rest-api-client
     #   slumber
     #   snowflake-connector-python
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via
     #   awscli
     #   boto3
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
@@ -229,31 +231,30 @@
     #   interchange
     #   pansi
     #   py2neo
     #   python-dateutil
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
-snowflake-connector-python==3.7.1
+snowflake-connector-python==3.10.0
     # via -r requirements/reporting.in
 sortedcontainers==2.4.0
     # via snowflake-connector-python
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via django
 stevedore==5.2.0
     # via
     #   edx-django-utils
     #   edx-opaque-keys
 tomlkit==0.12.4
     # via snowflake-connector-python
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   asgiref
     #   edx-opaque-keys
-    #   faker
     #   kombu
     #   snowflake-connector-python
 tzdata==2024.1
     # via
     #   backports-zoneinfo
     #   celery
 unicodecsv==0.14.1
@@ -269,7 +270,10 @@
 vine==5.1.0
     # via
     #   amqp
     #   celery
     #   kombu
 wcwidth==0.2.13
     # via prompt-toolkit
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `edx-enterprise-data-6.2.0/requirements/ci.txt` & `edx_enterprise_data-6.2.1/requirements/ci.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,35 +6,35 @@
 #
 cachetools==5.3.3
     # via tox
 chardet==5.2.0
     # via tox
 colorama==0.4.6
     # via tox
-coverage==7.4.3
+coverage==7.5.1
     # via -r requirements/ci.in
 distlib==0.3.8
     # via virtualenv
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   tox
     #   virtualenv
-packaging==23.2
+packaging==24.0
     # via
     #   pyproject-api
     #   tox
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via
     #   tox
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via tox
 pyproject-api==1.6.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.14.0
+tox==4.15.0
     # via -r requirements/ci.in
-virtualenv==20.25.1
+virtualenv==20.26.1
     # via tox
```

### Comparing `edx-enterprise-data-6.2.0/requirements/common_constraints.txt` & `edx_enterprise_data-6.2.1/requirements/common_constraints.txt`

 * *Files 24% similar despite different names*

```diff
@@ -18,7 +18,16 @@
 
 # elasticsearch>=7.14.0 includes breaking changes in it which caused issues in discovery upgrade process.
 # elastic search changelog: https://www.elastic.co/guide/en/enterprise-search/master/release-notes-7.14.0.html
 elasticsearch<7.14.0
 
 # django-simple-history>3.0.0 adds indexing and causes a lot of migrations to be affected
 django-simple-history==3.0.0
+
+# opentelemetry requires version 6.x at the moment:
+# https://github.com/open-telemetry/opentelemetry-python/issues/3570
+# Normally this could be added as a constraint in edx-django-utils, where we're
+# adding the opentelemetry dependency. However, when we compile pip-tools.txt,
+# that uses version 7.x, and then there's no undoing that when compiling base.txt.
+# So we need to pin it globally, for now.
+# Ticket for unpinning: https://github.com/openedx/edx-lint/issues/407
+importlib-metadata<7
```

### Comparing `edx-enterprise-data-6.2.0/requirements/constraints.txt` & `edx_enterprise_data-6.2.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/requirements/dev.txt` & `edx_enterprise_data-6.2.1/requirements/dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,57 +2,64 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
 amqp==5.2.0
     # via kombu
-asgiref==3.7.2
+asgiref==3.8.1
     # via django
 asn1crypto==1.5.1
     # via snowflake-connector-python
 astroid==3.1.0
     # via
     #   pylint
     #   pylint-celery
-awscli==1.32.56
+awscli==1.32.99
     # via -r requirements/reporting.in
+backports-tarfile==1.1.1
+    # via jaraco-context
 backports-zoneinfo[tzdata]==0.2.1 ; python_version < "3.9"
     # via
     #   -c requirements/constraints.txt
     #   celery
     #   django
+    #   djangorestframework
     #   kombu
-bcrypt==4.1.2
+bcrypt==4.1.3
     # via paramiko
 billiard==4.2.0
     # via celery
-boto3==1.34.56
+boto3==1.34.99
     # via -r requirements/reporting.in
-botocore==1.34.56
+botocore==1.34.99
     # via
     #   awscli
     #   boto3
     #   s3transfer
-build==1.1.1
+build==1.2.1
     # via pip-tools
+cachetools==5.3.3
+    # via tox
 celery==5.3.6
     # via -r requirements/reporting.in
 certifi==2024.2.2
     # via
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.16.0
     # via
     #   cryptography
     #   pynacl
     #   snowflake-connector-python
 chardet==5.2.0
-    # via diff-cover
+    # via
+    #   diff-cover
+    #   tox
 charset-normalizer==3.3.2
     # via
     #   requests
     #   snowflake-connector-python
 click==8.1.7
     # via
     #   celery
@@ -60,42 +67,45 @@
     #   click-log
     #   click-plugins
     #   click-repl
     #   code-annotations
     #   edx-django-utils
     #   edx-lint
     #   pip-tools
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-log==0.4.0
     # via edx-lint
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
-code-annotations==1.6.0
+code-annotations==1.8.0
     # via edx-lint
-colorama==0.4.4
-    # via awscli
-cryptography==42.0.5
+colorama==0.4.6
+    # via
+    #   awscli
+    #   tox
+cryptography==42.0.7
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields-v2
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
+    #   secretstorage
     #   snowflake-connector-python
-diff-cover==8.0.3
+diff-cover==9.0.0
     # via -r requirements/dev-enterprise_data.in
 dill==0.3.8
     # via pylint
 distlib==0.3.8
     # via virtualenv
-django==4.2.11
+django==4.2.12
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields-v2
     #   django-filter
     #   django-model-utils
@@ -108,168 +118,185 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields-v2==0.9
     # via -r requirements/base.in
-django-filter==23.5
+django-filter==24.2
     # via -r requirements/base.in
-django-model-utils==4.4.0
+django-model-utils==4.5.1
     # via
     #   -r requirements/base.in
     #   edx-rbac
 django-waffle==4.1.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.14.0
+djangorestframework==3.15.1
     # via
     #   djangorestframework-csv
     #   drf-jwt
     #   edx-drf-extensions
 djangorestframework-csv==3.0.2
     # via -r requirements/base.in
+dnspython==2.6.1
+    # via pymongo
 docutils==0.16
     # via
     #   awscli
     #   readme-renderer
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.10.1
+edx-django-utils==5.13.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==10.2.0
+edx-drf-extensions==10.3.0
     # via
     #   -r requirements/base.in
     #   edx-rbac
-edx-i18n-tools==1.3.0
+edx-i18n-tools==1.6.0
     # via -r requirements/dev-enterprise_data.in
 edx-lint==5.3.6
     # via
     #   -r requirements/dev-enterprise_data.in
     #   -r requirements/quality.in
-edx-opaque-keys==2.5.1
+edx-opaque-keys==2.9.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
-edx-rbac==1.8.0
+edx-rbac==1.9.0
     # via -r requirements/base.in
-edx-rest-api-client==5.6.1
+edx-rest-api-client==5.7.0
     # via -r requirements/base.in
 factory-boy==3.3.0
     # via -r requirements/base.in
-faker==24.0.0
+faker==25.0.1
     # via factory-boy
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   snowflake-connector-python
     #   tox
     #   virtualenv
-idna==3.6
+idna==3.7
     # via
     #   requests
     #   snowflake-connector-python
-importlib-metadata==7.0.1
+importlib-metadata==6.11.0
     # via
+    #   -c requirements/common_constraints.txt
     #   build
     #   keyring
     #   twine
-importlib-resources==6.1.2
+importlib-resources==6.4.0
     # via keyring
 interchange==2021.0.4
     # via py2neo
 isort==5.13.2
     # via
     #   -r requirements/quality.in
     #   pylint
-jaraco-classes==3.3.1
+jaraco-classes==3.4.0
     # via keyring
-jinja2==3.1.3
+jaraco-context==5.3.0
+    # via keyring
+jaraco-functools==4.0.1
+    # via keyring
+jeepney==0.8.0
+    # via
+    #   keyring
+    #   secretstorage
+jinja2==3.1.4
     # via
     #   code-annotations
     #   diff-cover
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-keyring==24.3.1
+keyring==25.2.0
     # via twine
-kombu==5.3.5
+kombu==5.3.7
     # via celery
-lxml==5.1.0
-    # via edx-i18n-tools
+lxml[html-clean,html_clean]==5.2.1
+    # via
+    #   edx-i18n-tools
+    #   lxml-html-clean
+lxml-html-clean==0.1.1
+    # via lxml
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
 mccabe==0.7.0
     # via pylint
 mdurl==0.1.2
     # via markdown-it-py
 monotonic==1.6
     # via py2neo
 more-itertools==10.2.0
-    # via jaraco-classes
-newrelic==9.7.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+newrelic==9.9.0
     # via edx-django-utils
-nh3==0.2.15
+nh3==0.2.17
     # via readme-renderer
-packaging==23.2
+packaging==24.0
     # via
     #   build
     #   py2neo
+    #   pyproject-api
     #   snowflake-connector-python
     #   tox
 pansi==2020.7.3
     # via py2neo
 paramiko==3.4.0
     # via -r requirements/reporting.in
-path==16.10.0
+path==16.14.0
     # via edx-i18n-tools
 pbr==6.0.0
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
 pip-tools==7.4.1
     # via -r requirements/dev-enterprise_data.in
 pkginfo==1.10.0
     # via twine
-platformdirs==3.11.0
+platformdirs==4.2.1
     # via
     #   pylint
     #   snowflake-connector-python
+    #   tox
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via
     #   diff-cover
     #   tox
 polib==1.2.0
     # via edx-i18n-tools
 prompt-toolkit==3.0.43
     # via click-repl
 psutil==5.9.8
     # via edx-django-utils
-py==1.11.0
-    # via tox
 py2neo @ https://github.com/overhangio/py2neo/releases/download/2021.2.3/py2neo-2021.2.3.tar.gz
     # via -r requirements/reporting.in
-pyasn1==0.5.1
+pyasn1==0.6.0
     # via
     #   pgpy
     #   rsa
 pycodestyle==2.11.1
     # via -r requirements/quality.in
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pydocstyle==6.3.0
     # via -r requirements/quality.in
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   diff-cover
     #   py2neo
     #   readme-renderer
     #   rich
 pyjwt[crypto]==2.8.0
     # via
@@ -289,37 +316,38 @@
     # via edx-lint
 pylint-plugin-utils==0.8.2
     # via
     #   pylint-celery
     #   pylint-django
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.13.0
+pymongo==4.4.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==24.0.0
+pyopenssl==24.1.0
     # via snowflake-connector-python
-pyproject-hooks==1.0.0
+pyproject-api==1.6.1
+    # via tox
+pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
 python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   celery
     #   faker
     #   vertica-python
 python-slugify==8.0.4
     # via code-annotations
 pytz==2024.1
     # via
-    #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==6.0.1
     # via
     #   awscli
     #   code-annotations
     #   edx-i18n-tools
@@ -340,70 +368,70 @@
     # via twine
 rich==13.7.1
     # via twine
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via
     #   awscli
     #   boto3
+secretstorage==3.3.3
+    # via keyring
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
     #   edx-lint
     #   edx-rbac
     #   interchange
     #   pansi
     #   py2neo
     #   python-dateutil
-    #   tox
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
 snowballstemmer==2.2.0
     # via pydocstyle
-snowflake-connector-python==3.7.1
+snowflake-connector-python==3.10.0
     # via -r requirements/reporting.in
 sortedcontainers==2.4.0
     # via snowflake-connector-python
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via django
 stevedore==5.2.0
     # via
     #   code-annotations
     #   edx-django-utils
     #   edx-opaque-keys
-testfixtures==8.1.0
+testfixtures==8.2.0
     # via -r requirements/quality.in
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
     # via
     #   build
     #   pip-tools
     #   pylint
-    #   pyproject-hooks
+    #   pyproject-api
     #   tox
 tomlkit==0.12.4
     # via
     #   pylint
     #   snowflake-connector-python
-tox==3.28.0
+tox==4.15.0
     # via -r requirements/dev-enterprise_data.in
 twine==5.0.0
     # via -r requirements/dev-enterprise_data.in
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   asgiref
     #   astroid
     #   edx-opaque-keys
-    #   faker
     #   kombu
     #   pylint
     #   rich
     #   snowflake-connector-python
 tzdata==2024.1
     # via
     #   backports-zoneinfo
@@ -420,23 +448,23 @@
 vertica-python==1.3.8
     # via -r requirements/reporting.in
 vine==5.1.0
     # via
     #   amqp
     #   celery
     #   kombu
-virtualenv==20.25.1
+virtualenv==20.26.1
     # via tox
 wcwidth==0.2.13
     # via prompt-toolkit
-wheel==0.42.0
+wheel==0.43.0
     # via
     #   -r requirements/dev-enterprise_data.in
     #   pip-tools
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `edx-enterprise-data-6.2.0/requirements/pip_tools.txt` & `edx_enterprise_data-6.2.1/requirements/pip_tools.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
-build==1.1.1
+build==1.2.1
     # via pip-tools
 click==8.1.7
     # via pip-tools
-importlib-metadata==7.0.1
-    # via build
-packaging==23.2
+importlib-metadata==6.11.0
+    # via
+    #   -c requirements/common_constraints.txt
+    #   build
+packaging==24.0
     # via build
 pip-tools==7.4.1
     # via -r requirements/pip_tools.in
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
 tomli==2.0.1
     # via
     #   build
     #   pip-tools
-    #   pyproject-hooks
-wheel==0.42.0
+wheel==0.43.0
     # via pip-tools
-zipp==3.17.0
+zipp==3.18.1
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `edx-enterprise-data-6.2.0/requirements/quality.txt` & `edx_enterprise_data-6.2.1/requirements/quality.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,57 +2,64 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
 amqp==5.2.0
     # via kombu
-asgiref==3.7.2
+asgiref==3.8.1
     # via django
 asn1crypto==1.5.1
     # via snowflake-connector-python
 astroid==3.1.0
     # via
     #   pylint
     #   pylint-celery
-awscli==1.32.56
+awscli==1.32.99
     # via -r requirements/reporting.in
+backports-tarfile==1.1.1
+    # via jaraco-context
 backports-zoneinfo[tzdata]==0.2.1 ; python_version < "3.9"
     # via
     #   -c requirements/constraints.txt
     #   celery
     #   django
+    #   djangorestframework
     #   kombu
-bcrypt==4.1.2
+bcrypt==4.1.3
     # via paramiko
 billiard==4.2.0
     # via celery
-boto3==1.34.56
+boto3==1.34.99
     # via -r requirements/reporting.in
-botocore==1.34.56
+botocore==1.34.99
     # via
     #   awscli
     #   boto3
     #   s3transfer
-build==1.1.1
+build==1.2.1
     # via pip-tools
+cachetools==5.3.3
+    # via tox
 celery==5.3.6
     # via -r requirements/reporting.in
 certifi==2024.2.2
     # via
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.16.0
     # via
     #   cryptography
     #   pynacl
     #   snowflake-connector-python
 chardet==5.2.0
-    # via diff-cover
+    # via
+    #   diff-cover
+    #   tox
 charset-normalizer==3.3.2
     # via
     #   requests
     #   snowflake-connector-python
 click==8.1.7
     # via
     #   celery
@@ -60,46 +67,49 @@
     #   click-log
     #   click-plugins
     #   click-repl
     #   code-annotations
     #   edx-django-utils
     #   edx-lint
     #   pip-tools
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-log==0.4.0
     # via edx-lint
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
-code-annotations==1.6.0
+code-annotations==1.8.0
     # via edx-lint
-colorama==0.4.4
-    # via awscli
-coverage[toml]==7.4.3
+colorama==0.4.6
+    # via
+    #   awscli
+    #   tox
+coverage[toml]==7.5.1
     # via pytest-cov
-cryptography==42.0.5
+cryptography==42.0.7
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields-v2
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
+    #   secretstorage
     #   snowflake-connector-python
 ddt==1.7.2
     # via -r requirements/test.in
-diff-cover==8.0.3
+diff-cover==9.0.0
     # via -r requirements/dev-enterprise_data.in
 dill==0.3.8
     # via pylint
 distlib==0.3.8
     # via virtualenv
-django==4.2.11
+django==4.2.12
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields-v2
     #   django-filter
     #   django-model-utils
@@ -112,183 +122,200 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields-v2==0.9
     # via -r requirements/base.in
-django-filter==23.5
+django-filter==24.2
     # via -r requirements/base.in
-django-model-utils==4.4.0
+django-model-utils==4.5.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
     #   edx-rbac
 django-waffle==4.1.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.14.0
+djangorestframework==3.15.1
     # via
     #   djangorestframework-csv
     #   drf-jwt
     #   edx-drf-extensions
 djangorestframework-csv==3.0.2
     # via -r requirements/base.in
+dnspython==2.6.1
+    # via pymongo
 docutils==0.16
     # via
     #   awscli
     #   readme-renderer
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.10.1
+edx-django-utils==5.13.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==10.2.0
+edx-drf-extensions==10.3.0
     # via
     #   -r requirements/base.in
     #   edx-rbac
-edx-i18n-tools==1.3.0
+edx-i18n-tools==1.6.0
     # via -r requirements/dev-enterprise_data.in
 edx-lint==5.3.6
     # via
     #   -r requirements/dev-enterprise_data.in
     #   -r requirements/quality.in
-edx-opaque-keys==2.5.1
+edx-opaque-keys==2.9.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
-edx-rbac==1.8.0
+edx-rbac==1.9.0
     # via -r requirements/base.in
-edx-rest-api-client==5.6.1
+edx-rest-api-client==5.7.0
     # via -r requirements/base.in
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 factory-boy==3.3.0
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
-faker==24.0.0
+faker==25.0.1
     # via factory-boy
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   snowflake-connector-python
     #   tox
     #   virtualenv
-flaky==3.7.0
+flaky==3.8.1
     # via -r requirements/test.in
-freezegun==1.4.0
+freezegun==1.5.0
     # via -r requirements/test.in
-idna==3.6
+idna==3.7
     # via
     #   requests
     #   snowflake-connector-python
-importlib-metadata==7.0.1
+importlib-metadata==6.11.0
     # via
+    #   -c requirements/common_constraints.txt
     #   build
     #   keyring
     #   twine
-importlib-resources==6.1.2
+importlib-resources==6.4.0
     # via keyring
 iniconfig==2.0.0
     # via pytest
 interchange==2021.0.4
     # via py2neo
 isort==5.13.2
     # via
     #   -r requirements/quality.in
     #   pylint
-jaraco-classes==3.3.1
+jaraco-classes==3.4.0
     # via keyring
-jinja2==3.1.3
+jaraco-context==5.3.0
+    # via keyring
+jaraco-functools==4.0.1
+    # via keyring
+jeepney==0.8.0
+    # via
+    #   keyring
+    #   secretstorage
+jinja2==3.1.4
     # via
     #   code-annotations
     #   diff-cover
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-keyring==24.3.1
+keyring==25.2.0
     # via twine
-kombu==5.3.5
+kombu==5.3.7
     # via celery
-lxml==5.1.0
-    # via edx-i18n-tools
+lxml[html-clean,html_clean]==5.2.1
+    # via
+    #   edx-i18n-tools
+    #   lxml-html-clean
+lxml-html-clean==0.1.1
+    # via lxml
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
 mccabe==0.7.0
     # via pylint
 mdurl==0.1.2
     # via markdown-it-py
 mock==5.1.0
     # via -r requirements/test.in
 monotonic==1.6
     # via py2neo
 more-itertools==10.2.0
-    # via jaraco-classes
-newrelic==9.7.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+newrelic==9.9.0
     # via edx-django-utils
-nh3==0.2.15
+nh3==0.2.17
     # via readme-renderer
-packaging==23.2
+packaging==24.0
     # via
     #   build
     #   py2neo
+    #   pyproject-api
     #   pytest
     #   snowflake-connector-python
     #   tox
 pansi==2020.7.3
     # via py2neo
 paramiko==3.4.0
     # via -r requirements/reporting.in
-path==16.10.0
+path==16.14.0
     # via edx-i18n-tools
 pbr==6.0.0
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
 pip-tools==7.4.1
     # via -r requirements/dev-enterprise_data.in
 pkginfo==1.10.0
     # via twine
-platformdirs==3.11.0
+platformdirs==4.2.1
     # via
     #   pylint
     #   snowflake-connector-python
+    #   tox
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via
     #   diff-cover
     #   pytest
     #   tox
 polib==1.2.0
     # via edx-i18n-tools
 prompt-toolkit==3.0.43
     # via click-repl
 psutil==5.9.8
     # via edx-django-utils
-py==1.11.0
-    # via tox
 py2neo @ https://github.com/overhangio/py2neo/releases/download/2021.2.3/py2neo-2021.2.3.tar.gz
     # via -r requirements/reporting.in
-pyasn1==0.5.1
+pyasn1==0.6.0
     # via
     #   pgpy
     #   rsa
 pycodestyle==2.11.1
     # via -r requirements/quality.in
-pycparser==2.21
+pycparser==2.22
     # via cffi
 pydocstyle==6.3.0
     # via -r requirements/quality.in
-pygments==2.17.2
+pygments==2.18.0
     # via
     #   diff-cover
     #   py2neo
     #   readme-renderer
     #   rich
 pyjwt[crypto]==2.8.0
     # via
@@ -308,46 +335,47 @@
     # via edx-lint
 pylint-plugin-utils==0.8.2
     # via
     #   pylint-celery
     #   pylint-django
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.13.0
+pymongo==4.4.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==24.0.0
+pyopenssl==24.1.0
     # via snowflake-connector-python
-pyproject-hooks==1.0.0
+pyproject-api==1.6.1
+    # via tox
+pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
-pytest==8.0.2
+pytest==8.2.0
     # via
     #   pytest-cov
     #   pytest-django
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via -r requirements/test.in
 pytest-django==4.8.0
     # via -r requirements/test.in
 python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   celery
     #   faker
     #   freezegun
     #   vertica-python
 python-slugify==8.0.4
     # via code-annotations
 pytz==2024.1
     # via
-    #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==6.0.1
     # via
     #   awscli
     #   code-annotations
     #   edx-i18n-tools
@@ -372,74 +400,74 @@
     # via twine
 rich==13.7.1
     # via twine
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via
     #   awscli
     #   boto3
+secretstorage==3.3.3
+    # via keyring
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
     #   edx-lint
     #   edx-rbac
     #   interchange
     #   pansi
     #   py2neo
     #   python-dateutil
-    #   tox
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
 snowballstemmer==2.2.0
     # via pydocstyle
-snowflake-connector-python==3.7.1
+snowflake-connector-python==3.10.0
     # via -r requirements/reporting.in
 sortedcontainers==2.4.0
     # via snowflake-connector-python
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via django
 stevedore==5.2.0
     # via
     #   code-annotations
     #   edx-django-utils
     #   edx-opaque-keys
-testfixtures==8.1.0
+testfixtures==8.2.0
     # via
     #   -r requirements/quality.in
     #   -r requirements/test.in
 text-unidecode==1.3
     # via python-slugify
 tomli==2.0.1
     # via
     #   build
     #   coverage
     #   pip-tools
     #   pylint
-    #   pyproject-hooks
+    #   pyproject-api
     #   pytest
     #   tox
 tomlkit==0.12.4
     # via
     #   pylint
     #   snowflake-connector-python
-tox==3.28.0
+tox==4.15.0
     # via -r requirements/dev-enterprise_data.in
 twine==5.0.0
     # via -r requirements/dev-enterprise_data.in
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   asgiref
     #   astroid
     #   edx-opaque-keys
-    #   faker
     #   kombu
     #   pylint
     #   rich
     #   snowflake-connector-python
 tzdata==2024.1
     # via
     #   backports-zoneinfo
@@ -457,23 +485,23 @@
 vertica-python==1.3.8
     # via -r requirements/reporting.in
 vine==5.1.0
     # via
     #   amqp
     #   celery
     #   kombu
-virtualenv==20.25.1
+virtualenv==20.26.1
     # via tox
 wcwidth==0.2.13
     # via prompt-toolkit
-wheel==0.42.0
+wheel==0.43.0
     # via
     #   -r requirements/dev-enterprise_data.in
     #   pip-tools
-zipp==3.17.0
+zipp==3.18.1
     # via
     #   importlib-metadata
     #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `edx-enterprise-data-6.2.0/requirements/reporting.in` & `edx_enterprise_data-6.2.1/requirements/reporting.in`

 * *Files identical despite different names*

### Comparing `edx-enterprise-data-6.2.0/requirements/test-master.txt` & `edx_enterprise_data-6.2.1/requirements/test-master.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
 amqp==5.2.0
     # via kombu
-asgiref==3.7.2
+asgiref==3.8.1
     # via django
 asn1crypto==1.5.1
     # via snowflake-connector-python
-awscli==1.32.56
+awscli==1.32.99
     # via -r requirements/reporting.in
 backports-zoneinfo[tzdata]==0.2.1 ; python_version < "3.9"
     # via
     #   -c requirements/constraints.txt
     #   celery
     #   django
+    #   djangorestframework
     #   kombu
-bcrypt==4.1.2
+bcrypt==4.1.3
     # via paramiko
 billiard==4.2.0
     # via celery
-boto3==1.34.56
+boto3==1.34.99
     # via -r requirements/reporting.in
-botocore==1.34.56
+botocore==1.34.99
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==5.3.6
     # via -r requirements/reporting.in
 certifi==2024.2.2
@@ -48,25 +49,25 @@
 click==8.1.7
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   edx-django-utils
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
-colorama==0.4.4
+colorama==0.4.6
     # via awscli
-coverage[toml]==7.4.3
+coverage[toml]==7.5.1
     # via pytest-cov
-cryptography==42.0.5
+cryptography==42.0.7
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields-v2
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
@@ -89,154 +90,155 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields-v2==0.9
     # via -r requirements/base.in
-django-filter==23.5
+django-filter==24.2
     # via -r requirements/base.in
-django-model-utils==4.4.0
+django-model-utils==4.5.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
     #   edx-rbac
 django-waffle==4.1.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.14.0
+djangorestframework==3.15.1
     # via
     #   -r requirements/test-master.in
     #   djangorestframework-csv
     #   drf-jwt
     #   edx-drf-extensions
 djangorestframework-csv==3.0.2
     # via -r requirements/base.in
+dnspython==2.6.1
+    # via pymongo
 docutils==0.16
     # via awscli
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.10.1
+edx-django-utils==5.13.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==10.2.0
+edx-drf-extensions==10.3.0
     # via
     #   -r requirements/base.in
     #   -r requirements/test-master.in
     #   edx-rbac
-edx-opaque-keys==2.5.1
+edx-opaque-keys==2.9.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
-edx-rbac==1.8.0
+edx-rbac==1.9.0
     # via -r requirements/base.in
-edx-rest-api-client==5.6.1
+edx-rest-api-client==5.7.0
     # via -r requirements/base.in
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 factory-boy==3.3.0
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
-faker==24.0.0
+faker==25.0.1
     # via factory-boy
-filelock==3.13.1
+filelock==3.14.0
     # via snowflake-connector-python
-flaky==3.7.0
+flaky==3.8.1
     # via -r requirements/test.in
-freezegun==1.4.0
+freezegun==1.5.0
     # via -r requirements/test.in
-idna==3.6
+idna==3.7
     # via
     #   requests
     #   snowflake-connector-python
 iniconfig==2.0.0
     # via pytest
 interchange==2021.0.4
     # via py2neo
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-kombu==5.3.5
+kombu==5.3.7
     # via celery
 mock==5.1.0
     # via -r requirements/test.in
 monotonic==1.6
     # via py2neo
-newrelic==9.7.0
+newrelic==9.9.0
     # via edx-django-utils
-packaging==23.2
+packaging==24.0
     # via
     #   py2neo
     #   pytest
     #   snowflake-connector-python
 pansi==2020.7.3
     # via py2neo
 paramiko==3.4.0
     # via -r requirements/reporting.in
 pbr==6.0.0
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
-platformdirs==3.11.0
+platformdirs==4.2.1
     # via snowflake-connector-python
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via click-repl
 psutil==5.9.8
     # via edx-django-utils
 py2neo @ https://github.com/overhangio/py2neo/releases/download/2021.2.3/py2neo-2021.2.3.tar.gz
     # via -r requirements/reporting.in
-pyasn1==0.5.1
+pyasn1==0.6.0
     # via
     #   pgpy
     #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.17.2
+pygments==2.18.0
     # via py2neo
 pyjwt[crypto]==2.8.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.13.0
+pymongo==4.4.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==24.0.0
+pyopenssl==24.1.0
     # via snowflake-connector-python
-pytest==8.0.2
+pytest==8.2.0
     # via
     #   pytest-cov
     #   pytest-django
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via -r requirements/test.in
 pytest-django==4.8.0
     # via -r requirements/test.in
 python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   celery
     #   faker
     #   freezegun
     #   vertica-python
 pytz==2024.1
     # via
-    #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==6.0.1
     # via
     #   awscli
     #   responses
 requests==2.31.0
@@ -249,15 +251,15 @@
     #   snowflake-connector-python
 responses==0.25.0
     # via -r requirements/test.in
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via
     #   awscli
     #   boto3
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
@@ -265,37 +267,36 @@
     #   interchange
     #   pansi
     #   py2neo
     #   python-dateutil
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
-snowflake-connector-python==3.7.1
+snowflake-connector-python==3.10.0
     # via -r requirements/reporting.in
 sortedcontainers==2.4.0
     # via snowflake-connector-python
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via django
 stevedore==5.2.0
     # via
     #   edx-django-utils
     #   edx-opaque-keys
-testfixtures==8.1.0
+testfixtures==8.2.0
     # via -r requirements/test.in
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 tomlkit==0.12.4
     # via snowflake-connector-python
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   asgiref
     #   edx-opaque-keys
-    #   faker
     #   kombu
     #   snowflake-connector-python
 tzdata==2024.1
     # via
     #   backports-zoneinfo
     #   celery
 unicodecsv==0.14.1
@@ -312,7 +313,10 @@
 vine==5.1.0
     # via
     #   amqp
     #   celery
     #   kombu
 wcwidth==0.2.13
     # via prompt-toolkit
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `edx-enterprise-data-6.2.0/requirements/test-reporting.txt` & `edx_enterprise_data-6.2.1/requirements/test-reporting.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,146 +4,154 @@
 #
 #    make upgrade
 #
 amqp==5.2.0
     # via kombu
 asn1crypto==1.5.1
     # via snowflake-connector-python
-awscli==1.32.56
+awscli==1.32.99
     # via -r requirements/reporting.in
 backports-zoneinfo[tzdata]==0.2.1 ; python_version < "3.9"
     # via
     #   -c requirements/constraints.txt
     #   celery
     #   kombu
-bcrypt==4.1.2
+bcrypt==4.1.3
     # via paramiko
 billiard==4.2.0
     # via celery
-boto3==1.34.56
+boto3==1.34.99
     # via -r requirements/reporting.in
-botocore==1.34.56
+botocore==1.34.99
     # via
     #   awscli
     #   boto3
     #   s3transfer
+cachetools==5.3.3
+    # via tox
 celery==5.3.6
     # via -r requirements/reporting.in
 certifi==2024.2.2
     # via
     #   py2neo
     #   requests
     #   snowflake-connector-python
 cffi==1.16.0
     # via
     #   cryptography
     #   pynacl
     #   snowflake-connector-python
+chardet==5.2.0
+    # via tox
 charset-normalizer==3.3.2
     # via
     #   requests
     #   snowflake-connector-python
 click==8.1.7
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
-colorama==0.4.4
-    # via awscli
-coverage[toml]==7.4.3
+colorama==0.4.6
+    # via
+    #   awscli
+    #   tox
+coverage[toml]==7.5.1
     # via pytest-cov
-cryptography==42.0.5
+cryptography==42.0.7
     # via
     #   -r requirements/reporting.in
     #   paramiko
     #   pgpy
     #   pyopenssl
     #   snowflake-connector-python
 ddt==1.1.2
     # via -r requirements/test-reporting.in
 distlib==0.3.8
     # via virtualenv
 docutils==0.16
     # via awscli
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
-filelock==3.13.1
+filelock==3.14.0
     # via
     #   snowflake-connector-python
     #   tox
     #   virtualenv
-idna==3.6
+idna==3.7
     # via
     #   requests
     #   snowflake-connector-python
 iniconfig==2.0.0
     # via pytest
 interchange==2021.0.4
     # via py2neo
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-kombu==5.3.5
+kombu==5.3.7
     # via celery
 mock==2.0.0
     # via -r requirements/test-reporting.in
 monotonic==1.6
     # via py2neo
-packaging==23.2
+packaging==24.0
     # via
     #   py2neo
+    #   pyproject-api
     #   pytest
     #   snowflake-connector-python
     #   tox
 pansi==2020.7.3
     # via py2neo
 paramiko==3.4.0
     # via -r requirements/reporting.in
 pbr==6.0.0
     # via mock
 pgpy==0.6.0
     # via -r requirements/reporting.in
-platformdirs==3.11.0
+platformdirs==4.2.1
     # via
     #   snowflake-connector-python
+    #   tox
     #   virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via
     #   pytest
     #   tox
 prompt-toolkit==3.0.43
     # via click-repl
-py==1.11.0
-    # via tox
 py2neo @ https://github.com/overhangio/py2neo/releases/download/2021.2.3/py2neo-2021.2.3.tar.gz
     # via -r requirements/reporting.in
-pyasn1==0.5.1
+pyasn1==0.6.0
     # via
     #   pgpy
     #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.17.2
+pygments==2.18.0
     # via py2neo
 pyjwt==2.8.0
     # via snowflake-connector-python
 pyminizip==0.2.6
     # via -r requirements/reporting.in
 pynacl==1.5.0
     # via paramiko
-pyopenssl==24.0.0
+pyopenssl==24.1.0
     # via snowflake-connector-python
+pyproject-api==1.6.1
+    # via tox
 pytest==8.0.2
     # via
     #   -r requirements/test-reporting.in
     #   pytest-cov
 pytest-cov==4.1.0
     # via -r requirements/test-reporting.in
 python-dateutil==2.9.0.post0
@@ -163,41 +171,41 @@
     # via
     #   responses
     #   snowflake-connector-python
 responses==0.25.0
     # via -r requirements/test-reporting.in
 rsa==4.7.2
     # via awscli
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via
     #   awscli
     #   boto3
 six==1.16.0
     # via
     #   interchange
     #   mock
     #   pansi
     #   py2neo
     #   python-dateutil
-    #   tox
     #   vertica-python
-snowflake-connector-python==3.7.1
+snowflake-connector-python==3.10.0
     # via -r requirements/reporting.in
 sortedcontainers==2.4.0
     # via snowflake-connector-python
 tomli==2.0.1
     # via
     #   coverage
+    #   pyproject-api
     #   pytest
     #   tox
 tomlkit==0.12.4
     # via snowflake-connector-python
-tox==3.28.0
+tox==4.15.0
     # via -r requirements/test-reporting.in
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   kombu
     #   snowflake-connector-python
 tzdata==2024.1
     # via
     #   backports-zoneinfo
     #   celery
@@ -213,11 +221,11 @@
 vertica-python==1.3.8
     # via -r requirements/reporting.in
 vine==5.1.0
     # via
     #   amqp
     #   celery
     #   kombu
-virtualenv==20.25.1
+virtualenv==20.26.1
     # via tox
 wcwidth==0.2.13
     # via prompt-toolkit
```

### Comparing `edx-enterprise-data-6.2.0/requirements/test.txt` & `edx_enterprise_data-6.2.1/requirements/test.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
 amqp==5.2.0
     # via kombu
-asgiref==3.7.2
+asgiref==3.8.1
     # via django
 asn1crypto==1.5.1
     # via snowflake-connector-python
-awscli==1.32.56
+awscli==1.32.99
     # via -r requirements/reporting.in
 backports-zoneinfo[tzdata]==0.2.1 ; python_version < "3.9"
     # via
     #   -c requirements/constraints.txt
     #   celery
     #   django
+    #   djangorestframework
     #   kombu
-bcrypt==4.1.2
+bcrypt==4.1.3
     # via paramiko
 billiard==4.2.0
     # via celery
-boto3==1.34.56
+boto3==1.34.99
     # via -r requirements/reporting.in
-botocore==1.34.56
+botocore==1.34.99
     # via
     #   awscli
     #   boto3
     #   s3transfer
 celery==5.3.6
     # via -r requirements/reporting.in
 certifi==2024.2.2
@@ -48,36 +49,36 @@
 click==8.1.7
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   edx-django-utils
-click-didyoumean==0.3.0
+click-didyoumean==0.3.1
     # via celery
 click-plugins==1.1.1
     # via celery
 click-repl==0.3.0
     # via celery
-colorama==0.4.4
+colorama==0.4.6
     # via awscli
-coverage[toml]==7.4.3
+coverage[toml]==7.5.1
     # via pytest-cov
-cryptography==42.0.5
+cryptography==42.0.7
     # via
     #   -r requirements/reporting.in
     #   django-fernet-fields-v2
     #   paramiko
     #   pgpy
     #   pyjwt
     #   pyopenssl
     #   snowflake-connector-python
 ddt==1.7.2
     # via -r requirements/test.in
-django==4.2.11
+django==4.2.12
     # via
     #   -c requirements/common_constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-fernet-fields-v2
     #   django-filter
     #   django-model-utils
@@ -89,152 +90,153 @@
     #   edx-rbac
 django-crum==0.7.9
     # via
     #   edx-django-utils
     #   edx-rbac
 django-fernet-fields-v2==0.9
     # via -r requirements/base.in
-django-filter==23.5
+django-filter==24.2
     # via -r requirements/base.in
-django-model-utils==4.4.0
+django-model-utils==4.5.1
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
     #   edx-rbac
 django-waffle==4.1.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-djangorestframework==3.14.0
+djangorestframework==3.15.1
     # via
     #   djangorestframework-csv
     #   drf-jwt
     #   edx-drf-extensions
 djangorestframework-csv==3.0.2
     # via -r requirements/base.in
+dnspython==2.6.1
+    # via pymongo
 docutils==0.16
     # via awscli
 drf-jwt==1.19.2
     # via edx-drf-extensions
-edx-django-utils==5.10.1
+edx-django-utils==5.13.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
     #   edx-rest-api-client
-edx-drf-extensions==10.2.0
+edx-drf-extensions==10.3.0
     # via
     #   -r requirements/base.in
     #   edx-rbac
-edx-opaque-keys==2.5.1
+edx-opaque-keys==2.9.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
-edx-rbac==1.8.0
+edx-rbac==1.9.0
     # via -r requirements/base.in
-edx-rest-api-client==5.6.1
+edx-rest-api-client==5.7.0
     # via -r requirements/base.in
-exceptiongroup==1.2.0
+exceptiongroup==1.2.1
     # via pytest
 factory-boy==3.3.0
     # via
     #   -r requirements/base.in
     #   -r requirements/test.in
-faker==24.0.0
+faker==25.0.1
     # via factory-boy
-filelock==3.13.1
+filelock==3.14.0
     # via snowflake-connector-python
-flaky==3.7.0
+flaky==3.8.1
     # via -r requirements/test.in
-freezegun==1.4.0
+freezegun==1.5.0
     # via -r requirements/test.in
-idna==3.6
+idna==3.7
     # via
     #   requests
     #   snowflake-connector-python
 iniconfig==2.0.0
     # via pytest
 interchange==2021.0.4
     # via py2neo
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-kombu==5.3.5
+kombu==5.3.7
     # via celery
 mock==5.1.0
     # via -r requirements/test.in
 monotonic==1.6
     # via py2neo
-newrelic==9.7.0
+newrelic==9.9.0
     # via edx-django-utils
-packaging==23.2
+packaging==24.0
     # via
     #   py2neo
     #   pytest
     #   snowflake-connector-python
 pansi==2020.7.3
     # via py2neo
 paramiko==3.4.0
     # via -r requirements/reporting.in
 pbr==6.0.0
     # via stevedore
 pgpy==0.6.0
     # via -r requirements/reporting.in
-platformdirs==3.11.0
+platformdirs==4.2.1
     # via snowflake-connector-python
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 prompt-toolkit==3.0.43
     # via click-repl
 psutil==5.9.8
     # via edx-django-utils
 py2neo @ https://github.com/overhangio/py2neo/releases/download/2021.2.3/py2neo-2021.2.3.tar.gz
     # via -r requirements/reporting.in
-pyasn1==0.5.1
+pyasn1==0.6.0
     # via
     #   pgpy
     #   rsa
-pycparser==2.21
+pycparser==2.22
     # via cffi
-pygments==2.17.2
+pygments==2.18.0
     # via py2neo
 pyjwt[crypto]==2.8.0
     # via
     #   drf-jwt
     #   edx-drf-extensions
     #   edx-rest-api-client
     #   snowflake-connector-python
 pyminizip==0.2.6
     # via -r requirements/reporting.in
-pymongo==3.13.0
+pymongo==4.4.0
     # via edx-opaque-keys
 pynacl==1.5.0
     # via
     #   edx-django-utils
     #   paramiko
-pyopenssl==24.0.0
+pyopenssl==24.1.0
     # via snowflake-connector-python
-pytest==8.0.2
+pytest==8.2.0
     # via
     #   pytest-cov
     #   pytest-django
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via -r requirements/test.in
 pytest-django==4.8.0
     # via -r requirements/test.in
 python-dateutil==2.9.0.post0
     # via
     #   botocore
     #   celery
     #   faker
     #   freezegun
     #   vertica-python
 pytz==2024.1
     # via
-    #   djangorestframework
     #   interchange
     #   snowflake-connector-python
 pyyaml==6.0.1
     # via
     #   awscli
     #   responses
 requests==2.31.0
@@ -247,15 +249,15 @@
     #   snowflake-connector-python
 responses==0.25.0
     # via -r requirements/test.in
 rsa==4.7.2
     # via awscli
 rules==3.3
     # via -r requirements/base.in
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via
     #   awscli
     #   boto3
 semantic-version==2.10.0
     # via edx-drf-extensions
 six==1.16.0
     # via
@@ -263,37 +265,36 @@
     #   interchange
     #   pansi
     #   py2neo
     #   python-dateutil
     #   vertica-python
 slumber==0.7.1
     # via edx-rest-api-client
-snowflake-connector-python==3.7.1
+snowflake-connector-python==3.10.0
     # via -r requirements/reporting.in
 sortedcontainers==2.4.0
     # via snowflake-connector-python
-sqlparse==0.4.4
+sqlparse==0.5.0
     # via django
 stevedore==5.2.0
     # via
     #   edx-django-utils
     #   edx-opaque-keys
-testfixtures==8.1.0
+testfixtures==8.2.0
     # via -r requirements/test.in
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 tomlkit==0.12.4
     # via snowflake-connector-python
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   asgiref
     #   edx-opaque-keys
-    #   faker
     #   kombu
     #   snowflake-connector-python
 tzdata==2024.1
     # via
     #   backports-zoneinfo
     #   celery
 unicodecsv==0.14.1
@@ -310,7 +311,10 @@
 vine==5.1.0
     # via
     #   amqp
     #   celery
     #   kombu
 wcwidth==0.2.13
     # via prompt-toolkit
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `edx-enterprise-data-6.2.0/setup.py` & `edx_enterprise_data-6.2.1/setup.py`

 * *Files identical despite different names*


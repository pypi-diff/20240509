# Comparing `tmp/alibabacloud_dingtalk-2.0.99.tar.gz` & `tmp/alibabacloud_dingtalk-2.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.99.tar", last modified: Fri Apr 26 02:41:59 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.10.tar", last modified: Thu May  9 06:18:47 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.99.tar` & `alibabacloud_dingtalk-2.1.10.tar`

### file list

```diff
@@ -1,429 +1,429 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/
--rw-r--r--   0 root         (0) root         (0)   126471 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2565 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2650 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15045 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21346 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23757 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38246 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    50325 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22974 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   168107 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12468 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19568 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45004 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26721 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95304 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   142688 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204138 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   393347 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60886 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5222 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4059 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250270 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   651992 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71584 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101499 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9792 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161860 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   394680 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41039 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78198 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   236838 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119949 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   152748 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   221957 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   122524 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   334068 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   418722 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41482 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33392 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44364 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30172 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19630 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8944 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14272 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5652 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10226 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   257462 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   615355 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45878 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499475 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148230 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54091 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64765 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    80337 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259804 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   315211 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   213190 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379351 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19496 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   190495 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   557050 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   850115 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113146 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120009 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18589 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   378556 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   527163 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161906 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   305557 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17280 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28173 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35856 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52698 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4825 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4965 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   134962 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18223 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68862 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119612 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136761 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   208587 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   303006 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   368637 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24693 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33051 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89450 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   671658 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   913856 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152590 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105975 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   131540 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5150 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4229 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22736 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   170469 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52481 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    59878 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62148 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34360 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42471 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7167 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89094 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   162124 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120360 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57967 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68049 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   265120 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   409387 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43482 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169147 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   103368 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93324 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   146182 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44633 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   386598 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   538012 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94517 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346388 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58076 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94327 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28049 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70520 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152094 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15723 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21167 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17009 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77172 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133813 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   107789 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33103 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40753 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20146 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   128063 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8155 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41320 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42730 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198336 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413640 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   494302 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   751756 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14206 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-26 02:41:59.000000 alibabacloud_dingtalk-2.0.99/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-04-26 02:41:58.000000 alibabacloud_dingtalk-2.0.99/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/
+-rw-r--r--   0 root         (0) root         (0)   128007 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15045 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21346 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23757 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38246 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    50325 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22974 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   168107 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12468 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    19568 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45004 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26721 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95304 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   142688 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   209034 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   406412 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60886 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250724 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   652799 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75580 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   109045 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161860 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   394680 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41039 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78198 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   236838 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119949 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   152748 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   221957 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   122524 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334068 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   418722 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41482 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33392 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44364 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30172 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19630 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8944 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14272 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   257462 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   615355 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7215 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45878 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499475 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148230 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54091 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64765 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    80337 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259804 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   315211 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   213190 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379351 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19496 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   190495 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   557050 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   850115 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113146 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120009 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18589 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   378556 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   527163 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161906 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   305557 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17280 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28173 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35856 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52698 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   134962 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18223 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68862 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119612 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136761 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   208587 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   303006 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   368637 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24693 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33051 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89450 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   671658 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   913856 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152590 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105975 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   131540 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22736 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   170469 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52481 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    59878 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62148 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34360 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42471 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7167 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89094 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   162124 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120360 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57967 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68049 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   265120 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   409387 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43482 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169147 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   103368 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93324 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   146182 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44633 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   386598 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   538012 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94517 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346388 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58076 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94327 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28049 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70520 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152094 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15723 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21167 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17009 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77172 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133813 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   107789 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33103 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40753 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20146 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   128063 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8155 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41320 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42730 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198336 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413640 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494302 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   751756 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14206 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-09 06:18:47.000000 alibabacloud_dingtalk-2.1.10/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-05-09 06:18:46.000000 alibabacloud_dingtalk-2.1.10/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.99/ChangeLog.md` & `alibabacloud_dingtalk-2.1.10/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-26 Version: 2.0.99
+- Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-04-23 Version: 2.0.98
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-22 Version: 2.0.97
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-18 Version: 2.0.96
```

### Comparing `alibabacloud_dingtalk-2.0.99/LICENSE` & `alibabacloud_dingtalk-2.1.10/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/PKG-INFO` & `alibabacloud_dingtalk-2.1.10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.0.99
+Version: 2.1.10
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.99/README-CN.md` & `alibabacloud_dingtalk-2.1.10/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/README.md` & `alibabacloud_dingtalk-2.1.10/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/amdp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/amdp_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/amdp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4139,14 +4139,128 @@
         self,
         request: dingtalkattendance__1__0_models.SaveCustomWaterMarkTemplateRequest,
     ) -> dingtalkattendance__1__0_models.SaveCustomWaterMarkTemplateResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkattendance__1__0_models.SaveCustomWaterMarkTemplateHeaders()
         return await self.save_custom_water_mark_template_with_options_async(request, headers, runtime)
 
+    def shift_add_with_options(
+        self,
+        request: dingtalkattendance__1__0_models.ShiftAddRequest,
+        headers: dingtalkattendance__1__0_models.ShiftAddHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.ShiftAddResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.op_user_id):
+            query['opUserId'] = request.op_user_id
+        body = {}
+        if not UtilClient.is_unset(request.name):
+            body['name'] = request.name
+        if not UtilClient.is_unset(request.owner):
+            body['owner'] = request.owner
+        if not UtilClient.is_unset(request.sections):
+            body['sections'] = request.sections
+        if not UtilClient.is_unset(request.service_id):
+            body['serviceId'] = request.service_id
+        if not UtilClient.is_unset(request.setting):
+            body['setting'] = request.setting
+        if not UtilClient.is_unset(request.shift_id):
+            body['shiftId'] = request.shift_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ShiftAdd',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/shifts',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.ShiftAddResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def shift_add_with_options_async(
+        self,
+        request: dingtalkattendance__1__0_models.ShiftAddRequest,
+        headers: dingtalkattendance__1__0_models.ShiftAddHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkattendance__1__0_models.ShiftAddResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.op_user_id):
+            query['opUserId'] = request.op_user_id
+        body = {}
+        if not UtilClient.is_unset(request.name):
+            body['name'] = request.name
+        if not UtilClient.is_unset(request.owner):
+            body['owner'] = request.owner
+        if not UtilClient.is_unset(request.sections):
+            body['sections'] = request.sections
+        if not UtilClient.is_unset(request.service_id):
+            body['serviceId'] = request.service_id
+        if not UtilClient.is_unset(request.setting):
+            body['setting'] = request.setting
+        if not UtilClient.is_unset(request.shift_id):
+            body['shiftId'] = request.shift_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ShiftAdd',
+            version='attendance_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/attendance/shifts',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkattendance__1__0_models.ShiftAddResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def shift_add(
+        self,
+        request: dingtalkattendance__1__0_models.ShiftAddRequest,
+    ) -> dingtalkattendance__1__0_models.ShiftAddResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.ShiftAddHeaders()
+        return self.shift_add_with_options(request, headers, runtime)
+
+    async def shift_add_async(
+        self,
+        request: dingtalkattendance__1__0_models.ShiftAddRequest,
+    ) -> dingtalkattendance__1__0_models.ShiftAddResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkattendance__1__0_models.ShiftAddHeaders()
+        return await self.shift_add_with_options_async(request, headers, runtime)
+
     def sync_schedule_info_with_options(
         self,
         request: dingtalkattendance__1__0_models.SyncScheduleInfoRequest,
         headers: dingtalkattendance__1__0_models.SyncScheduleInfoHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkattendance__1__0_models.SyncScheduleInfoResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11326,14 +11326,432 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SaveCustomWaterMarkTemplateResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ShiftAddHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class ShiftAddRequestSectionsTimes(TeaModel):
+    def __init__(
+        self,
+        across: int = None,
+        begin_min: int = None,
+        check_time: int = None,
+        check_type: str = None,
+        end_min: int = None,
+        flex_minutes: List[int] = None,
+        free_check: bool = None,
+    ):
+        self.across = across
+        self.begin_min = begin_min
+        self.check_time = check_time
+        self.check_type = check_type
+        self.end_min = end_min
+        self.flex_minutes = flex_minutes
+        self.free_check = free_check
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.across is not None:
+            result['across'] = self.across
+        if self.begin_min is not None:
+            result['beginMin'] = self.begin_min
+        if self.check_time is not None:
+            result['checkTime'] = self.check_time
+        if self.check_type is not None:
+            result['checkType'] = self.check_type
+        if self.end_min is not None:
+            result['endMin'] = self.end_min
+        if self.flex_minutes is not None:
+            result['flexMinutes'] = self.flex_minutes
+        if self.free_check is not None:
+            result['freeCheck'] = self.free_check
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('across') is not None:
+            self.across = m.get('across')
+        if m.get('beginMin') is not None:
+            self.begin_min = m.get('beginMin')
+        if m.get('checkTime') is not None:
+            self.check_time = m.get('checkTime')
+        if m.get('checkType') is not None:
+            self.check_type = m.get('checkType')
+        if m.get('endMin') is not None:
+            self.end_min = m.get('endMin')
+        if m.get('flexMinutes') is not None:
+            self.flex_minutes = m.get('flexMinutes')
+        if m.get('freeCheck') is not None:
+            self.free_check = m.get('freeCheck')
+        return self
+
+
+class ShiftAddRequestSections(TeaModel):
+    def __init__(
+        self,
+        times: List[ShiftAddRequestSectionsTimes] = None,
+    ):
+        self.times = times
+
+    def validate(self):
+        if self.times:
+            for k in self.times:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['times'] = []
+        if self.times is not None:
+            for k in self.times:
+                result['times'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.times = []
+        if m.get('times') is not None:
+            for k in m.get('times'):
+                temp_model = ShiftAddRequestSectionsTimes()
+                self.times.append(temp_model.from_map(k))
+        return self
+
+
+class ShiftAddRequestSettingTopRestTimeList(TeaModel):
+    def __init__(
+        self,
+        across: int = None,
+        check_time: int = None,
+    ):
+        self.across = across
+        self.check_time = check_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.across is not None:
+            result['across'] = self.across
+        if self.check_time is not None:
+            result['checkTime'] = self.check_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('across') is not None:
+            self.across = m.get('across')
+        if m.get('checkTime') is not None:
+            self.check_time = m.get('checkTime')
+        return self
+
+
+class ShiftAddRequestSetting(TeaModel):
+    def __init__(
+        self,
+        absenteeism_late_minutes: int = None,
+        attend_days: float = None,
+        extras: Dict[str, Any] = None,
+        is_flexible: bool = None,
+        serious_late_minutes: int = None,
+        tags: str = None,
+        top_rest_time_list: List[ShiftAddRequestSettingTopRestTimeList] = None,
+    ):
+        self.absenteeism_late_minutes = absenteeism_late_minutes
+        self.attend_days = attend_days
+        self.extras = extras
+        self.is_flexible = is_flexible
+        self.serious_late_minutes = serious_late_minutes
+        self.tags = tags
+        self.top_rest_time_list = top_rest_time_list
+
+    def validate(self):
+        if self.top_rest_time_list:
+            for k in self.top_rest_time_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.absenteeism_late_minutes is not None:
+            result['absenteeismLateMinutes'] = self.absenteeism_late_minutes
+        if self.attend_days is not None:
+            result['attendDays'] = self.attend_days
+        if self.extras is not None:
+            result['extras'] = self.extras
+        if self.is_flexible is not None:
+            result['isFlexible'] = self.is_flexible
+        if self.serious_late_minutes is not None:
+            result['seriousLateMinutes'] = self.serious_late_minutes
+        if self.tags is not None:
+            result['tags'] = self.tags
+        result['topRestTimeList'] = []
+        if self.top_rest_time_list is not None:
+            for k in self.top_rest_time_list:
+                result['topRestTimeList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('absenteeismLateMinutes') is not None:
+            self.absenteeism_late_minutes = m.get('absenteeismLateMinutes')
+        if m.get('attendDays') is not None:
+            self.attend_days = m.get('attendDays')
+        if m.get('extras') is not None:
+            self.extras = m.get('extras')
+        if m.get('isFlexible') is not None:
+            self.is_flexible = m.get('isFlexible')
+        if m.get('seriousLateMinutes') is not None:
+            self.serious_late_minutes = m.get('seriousLateMinutes')
+        if m.get('tags') is not None:
+            self.tags = m.get('tags')
+        self.top_rest_time_list = []
+        if m.get('topRestTimeList') is not None:
+            for k in m.get('topRestTimeList'):
+                temp_model = ShiftAddRequestSettingTopRestTimeList()
+                self.top_rest_time_list.append(temp_model.from_map(k))
+        return self
+
+
+class ShiftAddRequest(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        owner: str = None,
+        sections: List[ShiftAddRequestSections] = None,
+        service_id: int = None,
+        setting: ShiftAddRequestSetting = None,
+        shift_id: int = None,
+        op_user_id: str = None,
+    ):
+        self.name = name
+        self.owner = owner
+        self.sections = sections
+        self.service_id = service_id
+        self.setting = setting
+        self.shift_id = shift_id
+        self.op_user_id = op_user_id
+
+    def validate(self):
+        if self.sections:
+            for k in self.sections:
+                if k:
+                    k.validate()
+        if self.setting:
+            self.setting.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.owner is not None:
+            result['owner'] = self.owner
+        result['sections'] = []
+        if self.sections is not None:
+            for k in self.sections:
+                result['sections'].append(k.to_map() if k else None)
+        if self.service_id is not None:
+            result['serviceId'] = self.service_id
+        if self.setting is not None:
+            result['setting'] = self.setting.to_map()
+        if self.shift_id is not None:
+            result['shiftId'] = self.shift_id
+        if self.op_user_id is not None:
+            result['opUserId'] = self.op_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('owner') is not None:
+            self.owner = m.get('owner')
+        self.sections = []
+        if m.get('sections') is not None:
+            for k in m.get('sections'):
+                temp_model = ShiftAddRequestSections()
+                self.sections.append(temp_model.from_map(k))
+        if m.get('serviceId') is not None:
+            self.service_id = m.get('serviceId')
+        if m.get('setting') is not None:
+            temp_model = ShiftAddRequestSetting()
+            self.setting = temp_model.from_map(m['setting'])
+        if m.get('shiftId') is not None:
+            self.shift_id = m.get('shiftId')
+        if m.get('opUserId') is not None:
+            self.op_user_id = m.get('opUserId')
+        return self
+
+
+class ShiftAddResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        shift_id: int = None,
+    ):
+        self.name = name
+        self.shift_id = shift_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.shift_id is not None:
+            result['shiftId'] = self.shift_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('shiftId') is not None:
+            self.shift_id = m.get('shiftId')
+        return self
+
+
+class ShiftAddResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: ShiftAddResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = ShiftAddResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class ShiftAddResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ShiftAddResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ShiftAddResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SyncScheduleInfoHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2907,14 +2907,16 @@
         self,
         request: dingtalkbizfinance__1__0_models.QueryPermissionRoleMemberRequest,
         headers: dingtalkbizfinance__1__0_models.QueryPermissionRoleMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__1__0_models.QueryPermissionRoleMemberResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.company_code):
+            body['companyCode'] = request.company_code
         if not UtilClient.is_unset(request.role_code_list):
             body['roleCodeList'] = request.role_code_list
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -2942,14 +2944,16 @@
         self,
         request: dingtalkbizfinance__1__0_models.QueryPermissionRoleMemberRequest,
         headers: dingtalkbizfinance__1__0_models.QueryPermissionRoleMemberHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__1__0_models.QueryPermissionRoleMemberResponse:
         UtilClient.validate_model(request)
         body = {}
+        if not UtilClient.is_unset(request.company_code):
+            body['companyCode'] = request.company_code
         if not UtilClient.is_unset(request.role_code_list):
             body['roleCodeList'] = request.role_code_list
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
@@ -3609,14 +3613,16 @@
         self,
         request: dingtalkbizfinance__1__0_models.QueryRoleMemberByPageRequest,
         headers: dingtalkbizfinance__1__0_models.QueryRoleMemberByPageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__1__0_models.QueryRoleMemberByPageResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.company_code):
+            query['companyCode'] = request.company_code
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         if not UtilClient.is_unset(request.role_code):
             query['roleCode'] = request.role_code
         real_headers = {}
@@ -3648,14 +3654,16 @@
         self,
         request: dingtalkbizfinance__1__0_models.QueryRoleMemberByPageRequest,
         headers: dingtalkbizfinance__1__0_models.QueryRoleMemberByPageHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__1__0_models.QueryRoleMemberByPageResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.company_code):
+            query['companyCode'] = request.company_code
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['nextToken'] = request.next_token
         if not UtilClient.is_unset(request.role_code):
             query['roleCode'] = request.role_code
         real_headers = {}
```

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,19 @@
 
 
 class RoleMemberMapValue(TeaModel):
     def __init__(
         self,
         role_code: str = None,
         member_list: List[RoleMemberMapValueMemberList] = None,
+        company_code: str = None,
     ):
         self.role_code = role_code
         self.member_list = member_list
+        self.company_code = company_code
 
     def validate(self):
         if self.member_list:
             for k in self.member_list:
                 if k:
                     k.validate()
 
@@ -66,25 +68,29 @@
         result = dict()
         if self.role_code is not None:
             result['roleCode'] = self.role_code
         result['memberList'] = []
         if self.member_list is not None:
             for k in self.member_list:
                 result['memberList'].append(k.to_map() if k else None)
+        if self.company_code is not None:
+            result['companyCode'] = self.company_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('roleCode') is not None:
             self.role_code = m.get('roleCode')
         self.member_list = []
         if m.get('memberList') is not None:
             for k in m.get('memberList'):
                 temp_model = RoleMemberMapValueMemberList()
                 self.member_list.append(temp_model.from_map(k))
+        if m.get('companyCode') is not None:
+            self.company_code = m.get('companyCode')
         return self
 
 
 class AppendRolePermissionHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
@@ -7658,33 +7664,39 @@
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class QueryPermissionRoleMemberRequest(TeaModel):
     def __init__(
         self,
+        company_code: str = None,
         role_code_list: List[str] = None,
     ):
+        self.company_code = company_code
         self.role_code_list = role_code_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.company_code is not None:
+            result['companyCode'] = self.company_code
         if self.role_code_list is not None:
             result['roleCodeList'] = self.role_code_list
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('companyCode') is not None:
+            self.company_code = m.get('companyCode')
         if m.get('roleCodeList') is not None:
             self.role_code_list = m.get('roleCodeList')
         return self
 
 
 class QueryPermissionRoleMemberResponseBody(TeaModel):
     def __init__(
@@ -10023,41 +10035,47 @@
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
 class QueryRoleMemberByPageRequest(TeaModel):
     def __init__(
         self,
+        company_code: str = None,
         max_results: str = None,
         next_token: str = None,
         role_code: str = None,
     ):
+        self.company_code = company_code
         self.max_results = max_results
         self.next_token = next_token
         self.role_code = role_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.company_code is not None:
+            result['companyCode'] = self.company_code
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.next_token is not None:
             result['nextToken'] = self.next_token
         if self.role_code is not None:
             result['roleCode'] = self.role_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('companyCode') is not None:
+            self.company_code = m.get('companyCode')
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('nextToken') is not None:
             self.next_token = m.get('nextToken')
         if m.get('roleCode') is not None:
             self.role_code = m.get('roleCode')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1271,14 +1271,104 @@
         self,
         request: dingtalkbizfinance__2__0_models.QuerySupplierByPageRequest,
     ) -> dingtalkbizfinance__2__0_models.QuerySupplierByPageResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkbizfinance__2__0_models.QuerySupplierByPageHeaders()
         return await self.query_supplier_by_page_with_options_async(request, headers, runtime)
 
+    def query_user_role_list_with_options(
+        self,
+        request: dingtalkbizfinance__2__0_models.QueryUserRoleListRequest,
+        headers: dingtalkbizfinance__2__0_models.QueryUserRoleListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkbizfinance__2__0_models.QueryUserRoleListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.company_code):
+            query['companyCode'] = request.company_code
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryUserRoleList',
+            version='bizfinance_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/bizfinance/users/roles',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkbizfinance__2__0_models.QueryUserRoleListResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_user_role_list_with_options_async(
+        self,
+        request: dingtalkbizfinance__2__0_models.QueryUserRoleListRequest,
+        headers: dingtalkbizfinance__2__0_models.QueryUserRoleListHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkbizfinance__2__0_models.QueryUserRoleListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.company_code):
+            query['companyCode'] = request.company_code
+        if not UtilClient.is_unset(request.user_id):
+            query['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryUserRoleList',
+            version='bizfinance_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/bizfinance/users/roles',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkbizfinance__2__0_models.QueryUserRoleListResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_user_role_list(
+        self,
+        request: dingtalkbizfinance__2__0_models.QueryUserRoleListRequest,
+    ) -> dingtalkbizfinance__2__0_models.QueryUserRoleListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkbizfinance__2__0_models.QueryUserRoleListHeaders()
+        return self.query_user_role_list_with_options(request, headers, runtime)
+
+    async def query_user_role_list_async(
+        self,
+        request: dingtalkbizfinance__2__0_models.QueryUserRoleListRequest,
+    ) -> dingtalkbizfinance__2__0_models.QueryUserRoleListResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkbizfinance__2__0_models.QueryUserRoleListHeaders()
+        return await self.query_user_role_list_with_options_async(request, headers, runtime)
+
     def sign_enterprise_account_with_options(
         self,
         request: dingtalkbizfinance__2__0_models.SignEnterpriseAccountRequest,
         headers: dingtalkbizfinance__2__0_models.SignEnterpriseAccountHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkbizfinance__2__0_models.SignEnterpriseAccountResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2761,14 +2761,255 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QuerySupplierByPageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryUserRoleListHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryUserRoleListRequest(TeaModel):
+    def __init__(
+        self,
+        company_code: str = None,
+        user_id: str = None,
+    ):
+        self.company_code = company_code
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.company_code is not None:
+            result['companyCode'] = self.company_code
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('companyCode') is not None:
+            self.company_code = m.get('companyCode')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class QueryUserRoleListResponseBodyFinanceEmpDeptOpenList(TeaModel):
+    def __init__(
+        self,
+        cascade_dept_id: str = None,
+        dept_id: int = None,
+        name: str = None,
+        super_dept_id: int = None,
+    ):
+        self.cascade_dept_id = cascade_dept_id
+        self.dept_id = dept_id
+        self.name = name
+        self.super_dept_id = super_dept_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cascade_dept_id is not None:
+            result['cascadeDeptId'] = self.cascade_dept_id
+        if self.dept_id is not None:
+            result['deptId'] = self.dept_id
+        if self.name is not None:
+            result['name'] = self.name
+        if self.super_dept_id is not None:
+            result['superDeptId'] = self.super_dept_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('cascadeDeptId') is not None:
+            self.cascade_dept_id = m.get('cascadeDeptId')
+        if m.get('deptId') is not None:
+            self.dept_id = m.get('deptId')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('superDeptId') is not None:
+            self.super_dept_id = m.get('superDeptId')
+        return self
+
+
+class QueryUserRoleListResponseBodyRoleVOList(TeaModel):
+    def __init__(
+        self,
+        role_code: str = None,
+        role_name: str = None,
+    ):
+        self.role_code = role_code
+        self.role_name = role_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.role_code is not None:
+            result['roleCode'] = self.role_code
+        if self.role_name is not None:
+            result['roleName'] = self.role_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('roleCode') is not None:
+            self.role_code = m.get('roleCode')
+        if m.get('roleName') is not None:
+            self.role_name = m.get('roleName')
+        return self
+
+
+class QueryUserRoleListResponseBody(TeaModel):
+    def __init__(
+        self,
+        company_code: str = None,
+        finance_emp_dept_open_list: List[QueryUserRoleListResponseBodyFinanceEmpDeptOpenList] = None,
+        role_volist: List[QueryUserRoleListResponseBodyRoleVOList] = None,
+    ):
+        self.company_code = company_code
+        self.finance_emp_dept_open_list = finance_emp_dept_open_list
+        self.role_volist = role_volist
+
+    def validate(self):
+        if self.finance_emp_dept_open_list:
+            for k in self.finance_emp_dept_open_list:
+                if k:
+                    k.validate()
+        if self.role_volist:
+            for k in self.role_volist:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.company_code is not None:
+            result['companyCode'] = self.company_code
+        result['financeEmpDeptOpenList'] = []
+        if self.finance_emp_dept_open_list is not None:
+            for k in self.finance_emp_dept_open_list:
+                result['financeEmpDeptOpenList'].append(k.to_map() if k else None)
+        result['roleVOList'] = []
+        if self.role_volist is not None:
+            for k in self.role_volist:
+                result['roleVOList'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('companyCode') is not None:
+            self.company_code = m.get('companyCode')
+        self.finance_emp_dept_open_list = []
+        if m.get('financeEmpDeptOpenList') is not None:
+            for k in m.get('financeEmpDeptOpenList'):
+                temp_model = QueryUserRoleListResponseBodyFinanceEmpDeptOpenList()
+                self.finance_emp_dept_open_list.append(temp_model.from_map(k))
+        self.role_volist = []
+        if m.get('roleVOList') is not None:
+            for k in m.get('roleVOList'):
+                temp_model = QueryUserRoleListResponseBodyRoleVOList()
+                self.role_volist.append(temp_model.from_map(k))
+        return self
+
+
+class QueryUserRoleListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryUserRoleListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryUserRoleListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SignEnterpriseAccountHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.0.99
+Version: 2.1.10
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.99/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.1.10/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.99/setup.py` & `alibabacloud_dingtalk-2.1.10/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 26/04/2024
+Created on 09/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```


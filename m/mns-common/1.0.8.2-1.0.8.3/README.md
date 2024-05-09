# Comparing `tmp/mns_common-1.0.8.2.tar.gz` & `tmp/mns_common-1.0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.0.8.2.tar", last modified: Wed May  8 07:36:24 2024, max compression
+gzip compressed data, was "mns_common-1.0.8.3.tar", last modified: Thu May  9 14:23:44 2024, max compression
```

## Comparing `mns_common-1.0.8.2.tar` & `mns_common-1.0.8.3.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.472078 mns_common-1.0.8.2/
--rw-rw-rw-   0        0        0       59 2024-05-08 07:36:24.471081 mns_common-1.0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.8.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.430191 mns_common-1.0.8.2/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.8.2/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.432186 mns_common-1.0.8.2/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.8.2/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.436174 mns_common-1.0.8.2/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.8.2/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.8.2/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.8.2/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.439166 mns_common-1.0.8.2/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.8.2/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-04 09:55:55.000000 mns_common-1.0.8.2/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0    14960 2024-05-01 15:03:02.000000 mns_common-1.0.8.2/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.439166 mns_common-1.0.8.2/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.440164 mns_common-1.0.8.2/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.8.2/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.441162 mns_common-1.0.8.2/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.442160 mns_common-1.0.8.2/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.443157 mns_common-1.0.8.2/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.444153 mns_common-1.0.8.2/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.0.8.2/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.446148 mns_common-1.0.8.2/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.8.2/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.8.2/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.8.2/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.447146 mns_common-1.0.8.2/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.8.2/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.449140 mns_common-1.0.8.2/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.8.2/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.8.2/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.8.2/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.8.2/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.450137 mns_common-1.0.8.2/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.8.2/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.451134 mns_common-1.0.8.2/mns_common/component/cache/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.8.2/mns_common/component/cache/__init__.py
--rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.0.8.2/mns_common/component/cache/cache_service.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.452132 mns_common-1.0.8.2/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.8.2/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.8.2/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.8.2/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.8.2/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.453129 mns_common-1.0.8.2/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.8.2/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.455124 mns_common-1.0.8.2/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     2882 2024-05-06 14:46:13.000000 mns_common-1.0.8.2/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.0.8.2/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.456121 mns_common-1.0.8.2/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.8.2/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.8.2/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.457118 mns_common-1.0.8.2/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.8.2/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.8.2/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.457118 mns_common-1.0.8.2/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.459113 mns_common-1.0.8.2/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.8.2/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.8.2/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.8.2/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.460111 mns_common-1.0.8.2/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.8.2/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.8.2/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.461108 mns_common-1.0.8.2/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.8.2/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.8.2/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.8.2/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.462105 mns_common-1.0.8.2/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/component/real_time/real_time_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.463103 mns_common-1.0.8.2/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.8.2/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.0.8.2/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.464100 mns_common-1.0.8.2/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.8.2/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.465097 mns_common-1.0.8.2/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.2/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.8.2/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.467091 mns_common-1.0.8.2/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.8.2/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     1567 2024-05-03 14:48:19.000000 mns_common-1.0.8.2/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.8.2/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.0.8.2/mns_common/constant/self_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.8.2/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.468089 mns_common-1.0.8.2/mns_common/db/
--rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.8.2/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.8.2/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.471081 mns_common-1.0.8.2/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.8.2/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.8.2/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.8.2/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.8.2/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.8.2/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-08 07:36:24.471081 mns_common-1.0.8.2/mns_common.egg-info/
--rw-rw-rw-   0        0        0       59 2024-05-08 07:36:24.000000 mns_common-1.0.8.2/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3663 2024-05-08 07:36:24.000000 mns_common-1.0.8.2/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 07:36:24.000000 mns_common-1.0.8.2/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 07:36:24.000000 mns_common-1.0.8.2/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 07:36:24.472078 mns_common-1.0.8.2/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-08 07:34:38.000000 mns_common-1.0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.391881 mns_common-1.0.8.3/
+-rw-rw-rw-   0        0        0       59 2024-05-09 14:23:44.391881 mns_common-1.0.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.0.8.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.350304 mns_common-1.0.8.3/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.0.8.3/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.353295 mns_common-1.0.8.3/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.8.3/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.356606 mns_common-1.0.8.3/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.0.8.3/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.0.8.3/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.0.8.3/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.359682 mns_common-1.0.8.3/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.8.3/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-04 09:55:55.000000 mns_common-1.0.8.3/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0    14960 2024-05-01 15:03:02.000000 mns_common-1.0.8.3/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.360222 mns_common-1.0.8.3/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.360741 mns_common-1.0.8.3/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.0.8.3/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.361770 mns_common-1.0.8.3/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.362827 mns_common-1.0.8.3/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.363852 mns_common-1.0.8.3/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.364366 mns_common-1.0.8.3/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.0.8.3/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.366414 mns_common-1.0.8.3/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.0.8.3/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.0.8.3/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.0.8.3/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.367440 mns_common-1.0.8.3/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.0.8.3/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.369940 mns_common-1.0.8.3/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.0.8.3/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.0.8.3/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    39935 2024-04-12 00:08:48.000000 mns_common-1.0.8.3/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6784 2024-01-12 12:47:02.000000 mns_common-1.0.8.3/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.369940 mns_common-1.0.8.3/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.0.8.3/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.370937 mns_common-1.0.8.3/mns_common/component/cache/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.8.3/mns_common/component/cache/__init__.py
+-rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.0.8.3/mns_common/component/cache/cache_service.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.372931 mns_common-1.0.8.3/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.0.8.3/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.0.8.3/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.0.8.3/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     4790 2024-01-13 08:29:24.000000 mns_common-1.0.8.3/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.373929 mns_common-1.0.8.3/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     6987 2023-12-17 11:37:16.000000 mns_common-1.0.8.3/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.374926 mns_common-1.0.8.3/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.0.8.3/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.0.8.3/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.375924 mns_common-1.0.8.3/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.0.8.3/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.0.8.3/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.376921 mns_common-1.0.8.3/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.0.8.3/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.0.8.3/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.377918 mns_common-1.0.8.3/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.378933 mns_common-1.0.8.3/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.0.8.3/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.0.8.3/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.0.8.3/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.379913 mns_common-1.0.8.3/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.0.8.3/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4449 2023-12-29 04:25:17.000000 mns_common-1.0.8.3/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.381908 mns_common-1.0.8.3/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.0.8.3/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.0.8.3/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.0.8.3/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.381908 mns_common-1.0.8.3/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/component/real_time/real_time_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.382905 mns_common-1.0.8.3/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.0.8.3/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.0.8.3/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.383902 mns_common-1.0.8.3/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.0.8.3/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.384899 mns_common-1.0.8.3/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.0.8.3/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     7794 2024-01-13 09:14:41.000000 mns_common-1.0.8.3/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.387892 mns_common-1.0.8.3/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.0.8.3/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     1567 2024-05-03 14:48:19.000000 mns_common-1.0.8.3/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.0.8.3/mns_common/constant/kpl_selection_no_choose_constant.py
+-rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.0.8.3/mns_common/constant/self_choose_constant.py
+-rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.0.8.3/mns_common/constant/ths_concept_no_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.387892 mns_common-1.0.8.3/mns_common/db/
+-rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.0.8.3/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.0.8.3/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.390884 mns_common-1.0.8.3/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.0.8.3/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.0.8.3/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.0.8.3/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.0.8.3/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.0.8.3/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:23:44.390884 mns_common-1.0.8.3/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-05-09 14:23:44.000000 mns_common-1.0.8.3/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3663 2024-05-09 14:23:44.000000 mns_common-1.0.8.3/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 14:23:44.000000 mns_common-1.0.8.3/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 14:23:44.000000 mns_common-1.0.8.3/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 14:23:44.391881 mns_common-1.0.8.3/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-09 14:23:42.000000 mns_common-1.0.8.3/setup.py
```

### Comparing `mns_common-1.0.8.2/README.md` & `mns_common-1.0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/akshare/k_line_api.py` & `mns_common-1.0.8.3/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.0.8.3/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.0.8.3/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.0.8.3/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.0.8.3/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.0.8.3/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.0.8.3/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.0.8.3/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.0.8.3/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.0.8.3/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.0.8.3/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.0.8.3/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/kpl/constant/kpl_constant.py` & `mns_common-1.0.8.3/mns_common/api/kpl/constant/kpl_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.0.8.3/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.0.8.3/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.0.8.3/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.0.8.3/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.0.8.3/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/msg/push_msg_api.py` & `mns_common-1.0.8.3/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.0.8.3/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.0.8.3/mns_common/api/ths/ths_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.0.8.3/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/cache/cache_service.py` & `mns_common-1.0.8.3/mns_common/component/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/classify/classify_constant.py` & `mns_common-1.0.8.3/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.0.8.3/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/common_service_fun_api.py` & `mns_common-1.0.8.3/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/company/company_common_service_api.py` & `mns_common-1.0.8.3/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.0.8.3/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,22 @@
 @lru_cache(maxsize=None)
 def get_kpl_all_concept():
     query = {}
     kpl_best_choose_index = mongodb_util.find_query_data(db_name_constant.KPL_BEST_CHOOSE_INDEX, query)
     return kpl_best_choose_index
 
 
+# 获取开盘啦有效概念列表
+@lru_cache(maxsize=None)
+def get_valid_kpl_all_concept():
+    all_kpl_concept_df = get_kpl_all_concept()
+
+    return all_kpl_concept_df.loc[all_kpl_concept_df['valid']]
+
+
 # 最近股票新添加ths概念 刚好这个模板在热炒中
 def kpl_recent_add_new_concept(str_day, before_num, str_now_date):
     last_trade_day = trade_date_common_service_api.get_before_trade_date(str_day, before_num)
     if str_now_date is not None:
         # 上一个交易结束时间
         last_trade_end_time = last_trade_day + ' 15:00:00'
 
@@ -73,12 +81,15 @@
     ]]
 
 
 # 清除开盘啦概念缓存
 def clear_kpl_concept_cache():
     get_kpl_all_concept.cache_clear()
     get_symbol_all_kpl_concept.cache_clear()
+    get_valid_kpl_all_concept.cache_clear()
 
 
 if __name__ == '__main__':
+    df = get_valid_kpl_all_concept()
+    df = get_valid_kpl_all_concept()
+    clear_kpl_concept_cache()
     df = get_kpl_all_concept()
-    print(1)
```

### Comparing `mns_common-1.0.8.2/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.0.8.3/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/data/data_init_api.py` & `mns_common-1.0.8.3/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.0.8.3/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.0.8.3/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.0.8.3/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.0.8.3/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.0.8.3/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/trade/trade_service_api.py` & `mns_common-1.0.8.3/mns_common/component/trade/trade_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.0.8.3/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.0.8.3/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/constant/db_name_constant.py` & `mns_common-1.0.8.3/mns_common/constant/db_name_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/constant/kpl_selection_no_choose_constant.py` & `mns_common-1.0.8.3/mns_common/constant/kpl_selection_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/constant/ths_concept_no_choose_constant.py` & `mns_common-1.0.8.3/mns_common/constant/ths_concept_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/db/MongodbUtil.py` & `mns_common-1.0.8.3/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/utils/data_frame_util.py` & `mns_common-1.0.8.3/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common/utils/date_handle_util.py` & `mns_common-1.0.8.3/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.0.8.2/mns_common.egg-info/SOURCES.txt` & `mns_common-1.0.8.3/mns_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*


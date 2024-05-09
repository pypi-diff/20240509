# Comparing `tmp/mns-scheduler-1.0.4.3.tar.gz` & `tmp/mns-scheduler-1.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.4.3.tar", last modified: Wed May  8 10:49:44 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.4.5.tar", last modified: Thu May  9 14:49:30 2024, max compression
```

## Comparing `mns-scheduler-1.0.4.3.tar` & `mns-scheduler-1.0.4.5.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.146649 mns-scheduler-1.0.4.3/
--rw-rw-rw-   0        0        0       62 2024-05-08 10:49:44.146649 mns-scheduler-1.0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.116729 mns-scheduler-1.0.4.3/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.118724 mns-scheduler-1.0.4.3/mns_scheduler/backup/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/backup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.119721 mns-scheduler-1.0.4.3/mns_scheduler/backup/app/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/backup/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/backup/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.120718 mns-scheduler-1.0.4.3/mns_scheduler/backup/em/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/backup/em/__init__.py
--rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/backup/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/backup/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.121716 mns-scheduler-1.0.4.3/mns_scheduler/backup/wen_cai/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/backup/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.122713 mns-scheduler-1.0.4.3/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.123710 mns-scheduler-1.0.4.3/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.124708 mns-scheduler-1.0.4.3/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.124708 mns-scheduler-1.0.4.3/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     5870 2024-05-08 10:22:01.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/clean/ths_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.125705 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.126702 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.128697 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/sync_new_index/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/sync_new_index/__init__.py
--rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.129694 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/update_concept_info/
--rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/update_concept_info/__init__.py
--rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.130692 mns-scheduler-1.0.4.3/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-04-30 07:00:04.000000 mns-scheduler-1.0.4.3/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.131689 mns-scheduler-1.0.4.3/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.131689 mns-scheduler-1.0.4.3/mns_scheduler/finance/
--rw-rw-rw-   0        0        0      163 2024-05-05 14:54:50.000000 mns-scheduler-1.0.4.3/mns_scheduler/finance/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.132687 mns-scheduler-1.0.4.3/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.133684 mns-scheduler-1.0.4.3/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.134681 mns-scheduler-1.0.4.3/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.134681 mns-scheduler-1.0.4.3/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.135678 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.136676 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     4748 2024-05-08 05:55:00.000000 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
--rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.137673 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.137673 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.139668 mns-scheduler-1.0.4.3/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.3/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.140665 mns-scheduler-1.0.4.3/mns_scheduler/trade/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/trade/__init__.py
--rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.3/mns_scheduler/trade/auto_ipo_buy_api.py
--rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.3/mns_scheduler/trade/auto_sell_service_api.py
--rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.3/mns_scheduler/trade/sync_position_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.141662 mns-scheduler-1.0.4.3/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.144654 mns-scheduler-1.0.4.3/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.145652 mns-scheduler-1.0.4.3/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    15511 2024-05-08 10:06:57.000000 mns-scheduler-1.0.4.3/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.3/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:49:44.145652 mns-scheduler-1.0.4.3/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-05-08 10:49:44.000000 mns-scheduler-1.0.4.3/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3281 2024-05-08 10:49:44.000000 mns-scheduler-1.0.4.3/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 10:49:44.000000 mns-scheduler-1.0.4.3/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-08 10:49:44.000000 mns-scheduler-1.0.4.3/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 10:49:44.146649 mns-scheduler-1.0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-05-08 10:49:24.000000 mns-scheduler-1.0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.769423 mns-scheduler-1.0.4.5/
+-rw-rw-rw-   0        0        0       62 2024-05-09 14:49:30.768427 mns-scheduler-1.0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.730136 mns-scheduler-1.0.4.5/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.732131 mns-scheduler-1.0.4.5/mns_scheduler/backup/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.733128 mns-scheduler-1.0.4.5/mns_scheduler/backup/app/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.735123 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/__init__.py
+-rw-rw-rw-   0        0        0     4992 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2334 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.736120 mns-scheduler-1.0.4.5/mns_scheduler/backup/wen_cai/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.737657 mns-scheduler-1.0.4.5/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.739161 mns-scheduler-1.0.4.5/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20332 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.740158 mns-scheduler-1.0.4.5/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.741155 mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     4512 2024-05-09 14:49:14.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/kpl_concept_clean_api.py
+-rw-rw-rw-   0        0        0     5907 2024-05-09 07:47:40.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/ths_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.742153 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.743151 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0     6724 2024-04-30 12:29:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     4460 2024-04-30 09:34:23.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.745145 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.746960 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/
+-rw-rw-rw-   0        0        0      163 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/__init__.py
+-rw-rw-rw-   0        0        0     1928 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8764 2024-04-27 03:55:36.000000 mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.748950 mns-scheduler-1.0.4.5/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-04-30 07:00:04.000000 mns-scheduler-1.0.4.5/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.748950 mns-scheduler-1.0.4.5/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.749947 mns-scheduler-1.0.4.5/mns_scheduler/finance/
+-rw-rw-rw-   0        0        0      163 2024-05-05 14:54:50.000000 mns-scheduler-1.0.4.5/mns_scheduler/finance/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.749947 mns-scheduler-1.0.4.5/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.751941 mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7988 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.752938 mns-scheduler-1.0.4.5/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.753935 mns-scheduler-1.0.4.5/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.753935 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.755930 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     4748 2024-05-09 13:26:15.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py
+-rw-rw-rw-   0        0        0     8016 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.756927 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.757924 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0    10461 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.759921 mns-scheduler-1.0.4.5/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     9165 2024-05-06 01:29:24.000000 mns-scheduler-1.0.4.5/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.761915 mns-scheduler-1.0.4.5/mns_scheduler/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/trade/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-04-28 03:16:51.000000 mns-scheduler-1.0.4.5/mns_scheduler/trade/auto_ipo_buy_api.py
+-rw-rw-rw-   0        0        0     4423 2024-04-28 08:59:05.000000 mns-scheduler-1.0.4.5/mns_scheduler/trade/auto_sell_service_api.py
+-rw-rw-rw-   0        0        0     2739 2024-04-28 08:08:30.000000 mns-scheduler-1.0.4.5/mns_scheduler/trade/sync_position_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.762912 mns-scheduler-1.0.4.5/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.765434 mns-scheduler-1.0.4.5/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.767428 mns-scheduler-1.0.4.5/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    15670 2024-05-09 08:01:31.000000 mns-scheduler-1.0.4.5/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-04-22 00:53:06.000000 mns-scheduler-1.0.4.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:49:30.768427 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-05-09 14:49:30.000000 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3334 2024-05-09 14:49:30.000000 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 14:49:30.000000 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-09 14:49:30.000000 mns-scheduler-1.0.4.5/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 14:49:30.769423 mns-scheduler-1.0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-05-09 14:49:28.000000 mns-scheduler-1.0.4.5/setup.py
```

### Comparing `mns-scheduler-1.0.4.3/README.md` & `mns-scheduler-1.0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/backup/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.4.5/mns_scheduler/backup/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/backup/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/backup/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/backup/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.4.5/mns_scheduler/backup/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.4.5/mns_scheduler/backup/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.4.5/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.4.5/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/concept/clean/ths_concept_clean_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/concept/clean/ths_concept_clean_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from loguru import logger
 import mns_common.component.company.company_common_service_api as company_common_service_api
 import mns_common.constant.db_name_constant as db_name_constant
 
 mongodb_util = MongodbUtil('27017')
 
 
-# 统计概念数量
-def update_concept_num():
+# 统计概念股票数量和行业分组信息
+def update_ths_concept_info():
     ths_concept_list = mongodb_util.find_all_data(db_name_constant.THS_CONCEPT_LIST)
     for ths_concept_one in ths_concept_list.itertuples():
         try:
             query = {'concept_code': ths_concept_one.symbol}
             ths_stock_concept_detail_df = (mongodb_util
                                            .find_query_data(db_name_constant.THS_STOCK_CONCEPT_DETAIL, query))
             concept_count = ths_stock_concept_detail_df.shape[0]
@@ -104,10 +104,10 @@
             query_concept = {"symbol": concept_code}
             new_values = {'$set': {"url": url, "str_now_time": str_now_time}}
             mongodb_util.update_one_query(query_concept, new_values, 'ths_concept_list')
 
 
 if __name__ == '__main__':
     logger.info("开始")
-    update_concept_num()
+    update_ths_concept_info()
     logger.info("结束")
     update_null_name()
```

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/sync_new_index/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/sync_one_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/concept/ths/update_concept_info/sync_one_symbol_all_concepts_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.4.5/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.4.5/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.4.5/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.4.5/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.4.5/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py` & `mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/sync_best_choose_his_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.4.5/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.4.5/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/trade/auto_sell_service_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/trade/auto_sell_service_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/trade/sync_position_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/trade/sync_position_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.4.5/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.4.5/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.4.5/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.4.5/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.4.5/mns_scheduler/zz_task/data_sync_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import mns_scheduler.concept.ths.sync_new_index.sync_ths_concept_by_ak_api as sync_ths_concept_by_ak_api
 import mns_scheduler.kpl.selection.total.sync_kpl_best_total_sync_api as sync_kpl_best_total_sync_api
 import mns_scheduler.company_info.company_info_sync_api as company_info_sync_api
 import mns_scheduler.trade.auto_ipo_buy_api as auto_ipo_buy_api
 import mns_scheduler.kpl.selection.index.sync_best_choose_his_index as sync_best_choose_his_index
 import mns_scheduler.concept.ths.common.ths_concept_update_common_api as ths_concept_update_common_api
 import mns_scheduler.trade.sync_position_api as sync_position_api
+import mns_scheduler.concept.clean.kpl_concept_clean_api as kpl_concept_clean_api
 
 
 # 同步交易日期任务完成
 def sync_trade_date():
     trade_date_common_service_api.sync_trade_date()
     logger.info('同步交易日期任务完成')
 
@@ -207,20 +208,22 @@
 def sync_stock_gdfx_free_top_10_one_day():
     logger.info('同步所有股票前十大流通股本')
     now_date = datetime.now()
     str_day = now_date.strftime('%Y-%m-%d')
     east_money_stock_gdfx_free_top_10_api.sync_stock_gdfx_free_top_10_one_day(str_day)
 
 
-# 更新同花顺概念信息
-def ths_concept_info_clean():
+# 更新概念信息
+def concept_info_clean():
     #  更新空概念名称
     ths_concept_choose_api.update_null_name()
     #  更新概念包含个数
-    ths_concept_choose_api.update_concept_num()
+    ths_concept_choose_api.update_ths_concept_info()
+    # 开盘啦概念信息更新
+    kpl_concept_clean_api.update_kpl_concept_info()
 
 
 # 同步概念下所有股票组成 by 概念指数
 def update_one_concept_all_symbol_detail():
     logger.info('同步概念下所有股票组成')
     sync_one_concept_all_symbols_api.update_concept_all_symbol_detail()
     update_ths_concept_choose_null_reason()
@@ -343,15 +346,15 @@
 # 开盘前同步当天交易需要的k线数据
 blockingScheduler.add_job(sync_today_trade_k_line_info, 'cron', hour='08', minute='30')
 
 # 同步十大流通股东信息
 blockingScheduler.add_job(sync_stock_gdfx_free_top_10_one_day, 'cron', hour='08,22', minute='23')
 
 # 更新同花顺概念信息
-blockingScheduler.add_job(ths_concept_info_clean, 'cron', hour='9,12,20', minute='24')
+blockingScheduler.add_job(concept_info_clean, 'cron', hour='9,12,20', minute='24')
 
 # 更新概念指数下所有股票组成 by 概念代码
 blockingScheduler.add_job(update_one_concept_all_symbol_detail, 'cron', hour='08,18,12', minute='30')
 
 # 同步单只股票下所有概念 by 股票代码
 blockingScheduler.add_job(update_one_symbol_all_concepts, 'cron', hour='09,18,12', minute='15')
```

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.4.5/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.4.3/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.4.5/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 mns_scheduler/big_deal/__init__.py
 mns_scheduler/big_deal/ths_big_deal_sync.py
 mns_scheduler/company_info/__init__.py
 mns_scheduler/company_info/company_constant_data.py
 mns_scheduler/company_info/company_info_sync_api.py
 mns_scheduler/concept/__init__.py
 mns_scheduler/concept/clean/__init__.py
+mns_scheduler/concept/clean/kpl_concept_clean_api.py
 mns_scheduler/concept/clean/ths_concept_clean_api.py
 mns_scheduler/concept/ths/__init__.py
 mns_scheduler/concept/ths/common/__init__.py
 mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
 mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
 mns_scheduler/concept/ths/sync_new_index/__init__.py
 mns_scheduler/concept/ths/sync_new_index/sync_ths_concept_by_ak_api.py
```


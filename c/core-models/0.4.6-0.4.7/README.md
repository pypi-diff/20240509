# Comparing `tmp/core_models-0.4.6.tar.gz` & `tmp/core_models-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_models-0.4.6.tar", last modified: Wed Apr 10 15:17:39 2024, max compression
+gzip compressed data, was "core_models-0.4.7.tar", last modified: Wed May  8 13:22:48 2024, max compression
```

## Comparing `core_models-0.4.6.tar` & `core_models-0.4.7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.693117 core_models-0.4.6/
--rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.4.6/LICENSE
--rw-r--r--   0 macbookpro   (501) staff       (20)      910 2024-04-10 15:17:39.692808 core_models-0.4.6/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     6515 2023-11-22 12:00:20.000000 core_models-0.4.6/README.md
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.647922 core_models-0.4.6/core_models/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.4.6/core_models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.4.6/core_models/api_response.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.652341 core_models-0.4.6/core_models/app/
--rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.4.6/core_models/app/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)    14836 2024-01-26 07:17:12.000000 core_models-0.4.6/core_models/app/admin.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.4.6/core_models/app/apps.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.4.6/core_models/app/context_processors.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.652907 core_models-0.4.6/core_models/app/integrations/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-11-10 05:22:31.000000 core_models-0.4.6/core_models/app/integrations/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      428 2023-12-10 23:11:18.000000 core_models-0.4.6/core_models/app/integrations/base_integration.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.657791 core_models-0.4.6/core_models/app/integrations/verto/
--rw-r--r--   0 macbookpro   (501) staff       (20)      210 2023-11-10 05:44:58.000000 core_models-0.4.6/core_models/app/integrations/verto/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     3026 2023-12-11 14:41:49.000000 core_models-0.4.6/core_models/app/integrations/verto/add_beneficiary.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     3254 2023-12-10 23:32:44.000000 core_models-0.4.6/core_models/app/integrations/verto/create_fx_trade.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1704 2023-12-04 10:36:51.000000 core_models-0.4.6/core_models/app/integrations/verto/create_payment.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1776 2023-11-24 10:06:37.000000 core_models-0.4.6/core_models/app/integrations/verto/get_currencies.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1670 2023-12-01 08:30:23.000000 core_models-0.4.6/core_models/app/integrations/verto/get_fx_rate.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1608 2023-12-03 23:53:29.000000 core_models-0.4.6/core_models/app/integrations/verto/get_purposes.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2862 2023-12-04 09:16:51.000000 core_models-0.4.6/core_models/app/integrations/verto/get_wallets.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1036 2023-11-10 08:43:43.000000 core_models-0.4.6/core_models/app/integrations/verto/login.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.658445 core_models-0.4.6/core_models/app/managers/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.4.6/core_models/app/managers/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     6753 2024-01-26 07:37:49.000000 core_models-0.4.6/core_models/app/managers/notification_manager.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.671986 core_models-0.4.6/core_models/app/migrations/
--rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.4.6/core_models/app/migrations/0001_initial.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.4.6/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.4.6/core_models/app/migrations/0003_alter_user_onboarding_stage.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.4.6/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.4.6/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.4.6/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.4.6/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.4.6/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.4.6/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.4.6/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1269 2023-05-30 07:27:17.000000 core_models-0.4.6/core_models/app/migrations/0011_remove_invoice_draft_company_annual_turnover_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1806 2023-06-12 17:47:58.000000 core_models-0.4.6/core_models/app/migrations/0012_rename_amount_invoiceitem_total_invoice_discount_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     7281 2023-06-13 17:40:40.000000 core_models-0.4.6/core_models/app/migrations/0013_country_region_subregion_city_alter_company_city_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      362 2023-06-13 17:42:30.000000 core_models-0.4.6/core_models/app/migrations/0014_remove_company_city.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      483 2023-06-13 17:51:57.000000 core_models-0.4.6/core_models/app/migrations/0015_company_city.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     3370 2023-07-04 13:26:12.000000 core_models-0.4.6/core_models/app/migrations/0016_sector_remove_company_industry_configuration_rpa_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      857 2023-07-04 22:55:41.000000 core_models-0.4.6/core_models/app/migrations/0017_alter_configuration_rpa.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      454 2023-07-05 15:16:17.000000 core_models-0.4.6/core_models/app/migrations/0018_invoice_rpa.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      391 2023-07-06 05:37:36.000000 core_models-0.4.6/core_models/app/migrations/0019_invoice_financed_on.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1965 2023-07-21 12:18:10.000000 core_models-0.4.6/core_models/app/migrations/0020_profileapplication.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      467 2023-07-26 23:45:53.000000 core_models-0.4.6/core_models/app/migrations/0021_profileapplication_company_registration_number.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      725 2023-07-26 23:47:54.000000 core_models-0.4.6/core_models/app/migrations/0022_otp.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      724 2023-08-11 08:23:32.000000 core_models-0.4.6/core_models/app/migrations/0023_alter_company_unique_together_country_oecd_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8112 2023-08-17 13:04:17.000000 core_models-0.4.6/core_models/app/migrations/0024_remove_profileapplication_export_countries_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1395 2023-08-17 17:10:24.000000 core_models-0.4.6/core_models/app/migrations/0025_remove_companyincorporation_team_chart_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      606 2023-08-17 17:12:22.000000 core_models-0.4.6/core_models/app/migrations/0026_companyincorporation_team_chart.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1124 2023-08-18 00:35:31.000000 core_models-0.4.6/core_models/app/migrations/0027_contractinformation_bank_statement_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1275 2023-09-04 17:16:28.000000 core_models-0.4.6/core_models/app/migrations/0028_profileapplication_company_incorporation_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1980 2023-09-10 15:26:07.000000 core_models-0.4.6/core_models/app/migrations/0029_remove_commercialinformation_credit_notes_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      609 2023-10-29 09:46:16.000000 core_models-0.4.6/core_models/app/migrations/0030_invoice_bill_of_lading_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2813 2023-11-10 08:01:25.000000 core_models-0.4.6/core_models/app/migrations/0031_bankaccount_account_type_bankaccount_currency_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      433 2023-11-13 09:50:20.000000 core_models-0.4.6/core_models/app/migrations/0032_invoice_decline_reason.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     5891 2023-11-22 12:08:55.000000 core_models-0.4.6/core_models/app/migrations/0033_invoicetransaction_payment_wallet_wallettransaction_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8243 2023-11-23 10:27:01.000000 core_models-0.4.6/core_models/app/migrations/0034_bankaccount_company_bankaccount_company_name_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1106 2023-11-23 14:23:47.000000 core_models-0.4.6/core_models/app/migrations/0035_remove_contractinformation_past_invoices_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      446 2023-11-29 13:26:38.000000 core_models-0.4.6/core_models/app/migrations/0036_contractinformation_completed.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-12-03 23:48:45.000000 core_models-0.4.6/core_models/app/migrations/0037_bankaccount_status.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1693 2023-12-07 12:53:37.000000 core_models-0.4.6/core_models/app/migrations/0038_contract_percent_discount_alter_bankaccount_status_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1328 2023-12-07 13:01:46.000000 core_models-0.4.6/core_models/app/migrations/0039_baserate.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2074 2023-12-11 09:57:37.000000 core_models-0.4.6/core_models/app/migrations/0040_remove_contract_percent_discount_baserate_date_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      520 2023-12-22 15:09:48.000000 core_models-0.4.6/core_models/app/migrations/0041_company_logo.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1815 2024-01-10 08:36:44.000000 core_models-0.4.6/core_models/app/migrations/0042_contract_buyer_company_contract_seller_company_and_more.py
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.4.6/core_models/app/migrations/__init__.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.691116 core_models-0.4.6/core_models/app/models/
--rw-r--r--   0 macbookpro   (501) staff       (20)      828 2024-01-10 08:47:42.000000 core_models-0.4.6/core_models/app/models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1437 2024-03-07 16:28:18.000000 core_models-0.4.6/core_models/app/models/bank_account.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1889 2024-02-28 09:58:03.000000 core_models-0.4.6/core_models/app/models/base.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      382 2023-12-11 06:52:11.000000 core_models-0.4.6/core_models/app/models/base_rate.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8327 2024-02-23 09:26:48.000000 core_models-0.4.6/core_models/app/models/company.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      686 2024-01-10 08:35:27.000000 core_models-0.4.6/core_models/app/models/company_configuration.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1254 2023-12-01 07:33:10.000000 core_models-0.4.6/core_models/app/models/configuration.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     7441 2024-04-10 11:36:14.000000 core_models-0.4.6/core_models/app/models/contract.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      670 2023-08-11 08:18:07.000000 core_models-0.4.6/core_models/app/models/country.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.4.6/core_models/app/models/currency.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     9862 2024-04-10 11:27:22.000000 core_models-0.4.6/core_models/app/models/invoice.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1472 2024-04-01 15:16:47.000000 core_models-0.4.6/core_models/app/models/notification.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1231 2023-07-27 06:25:34.000000 core_models-0.4.6/core_models/app/models/otp.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1700 2023-11-23 14:04:30.000000 core_models-0.4.6/core_models/app/models/payment.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4203 2024-04-10 11:23:01.000000 core_models-0.4.6/core_models/app/models/profile_application.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      272 2023-07-04 13:25:19.000000 core_models-0.4.6/core_models/app/models/sector.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2293 2024-02-23 09:26:48.000000 core_models-0.4.6/core_models/app/models/user.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      528 2023-11-08 09:07:59.000000 core_models-0.4.6/core_models/app/models/verto_config.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     2775 2024-01-17 09:04:48.000000 core_models-0.4.6/core_models/app/models/wallet.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1515 2023-12-04 09:27:57.000000 core_models-0.4.6/core_models/app/models/withdrawal.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.642928 core_models-0.4.6/core_models/app/templates/
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.691897 core_models-0.4.6/core_models/app/templates/core_models/
--rwxr-xr-x   0 macbookpro   (501) staff       (20)    15605 2023-09-12 16:32:38.000000 core_models-0.4.6/core_models/app/templates/core_models/mail-base.html
--rw-r--r--   0 macbookpro   (501) staff       (20)      750 2023-09-08 07:59:04.000000 core_models-0.4.6/core_models/app/templates/core_models/mail-base.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)     3182 2023-06-12 14:08:46.000000 core_models-0.4.6/core_models/base_views.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     6516 2024-03-28 12:35:04.000000 core_models-0.4.6/core_models/constants.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.4.6/core_models/settings.example.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     8224 2024-02-28 09:49:58.000000 core_models-0.4.6/core_models/settings.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     3469 2024-02-28 09:49:58.000000 core_models-0.4.6/core_models/utils.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-04-10 15:17:39.692435 core_models-0.4.6/core_models.egg-info/
--rw-r--r--   0 macbookpro   (501) staff       (20)      910 2024-04-10 15:17:39.000000 core_models-0.4.6/core_models.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     5135 2024-04-10 15:17:39.000000 core_models-0.4.6/core_models.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2024-04-10 15:17:39.000000 core_models-0.4.6/core_models.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)      233 2024-04-10 15:17:39.000000 core_models-0.4.6/core_models.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       12 2024-04-10 15:17:39.000000 core_models-0.4.6/core_models.egg-info/top_level.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.4.6/pyproject.toml
--rw-r--r--   0 macbookpro   (501) staff       (20)       38 2024-04-10 15:17:39.693229 core_models-0.4.6/setup.cfg
--rw-r--r--   0 macbookpro   (501) staff       (20)     1268 2024-04-10 15:17:21.000000 core_models-0.4.6/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.771940 core_models-0.4.7/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 core_models-0.4.7/LICENSE
+-rw-r--r--   0 macbookpro   (501) staff       (20)      910 2024-05-08 13:22:48.771526 core_models-0.4.7/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6515 2023-11-22 12:00:20.000000 core_models-0.4.7/README.md
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.723578 core_models-0.4.7/core_models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-18 09:44:55.000000 core_models-0.4.7/core_models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      851 2023-05-07 10:35:43.000000 core_models-0.4.7/core_models/api_response.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.744457 core_models-0.4.7/core_models/app/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      109 2023-04-26 13:38:04.000000 core_models-0.4.7/core_models/app/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)    14836 2024-01-26 07:17:12.000000 core_models-0.4.7/core_models/app/admin.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      114 2023-04-19 22:18:54.000000 core_models-0.4.7/core_models/app/apps.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      163 2023-04-29 15:41:05.000000 core_models-0.4.7/core_models/app/context_processors.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.745115 core_models-0.4.7/core_models/app/integrations/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-11-10 05:22:31.000000 core_models-0.4.7/core_models/app/integrations/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      428 2023-12-10 23:11:18.000000 core_models-0.4.7/core_models/app/integrations/base_integration.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.747834 core_models-0.4.7/core_models/app/integrations/verto/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      210 2023-11-10 05:44:58.000000 core_models-0.4.7/core_models/app/integrations/verto/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3026 2023-12-11 14:41:49.000000 core_models-0.4.7/core_models/app/integrations/verto/add_beneficiary.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3254 2023-12-10 23:32:44.000000 core_models-0.4.7/core_models/app/integrations/verto/create_fx_trade.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1704 2023-12-04 10:36:51.000000 core_models-0.4.7/core_models/app/integrations/verto/create_payment.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1776 2023-11-24 10:06:37.000000 core_models-0.4.7/core_models/app/integrations/verto/get_currencies.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1670 2023-12-01 08:30:23.000000 core_models-0.4.7/core_models/app/integrations/verto/get_fx_rate.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1608 2023-12-03 23:53:29.000000 core_models-0.4.7/core_models/app/integrations/verto/get_purposes.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2862 2023-12-04 09:16:51.000000 core_models-0.4.7/core_models/app/integrations/verto/get_wallets.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1036 2023-11-10 08:43:43.000000 core_models-0.4.7/core_models/app/integrations/verto/login.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.748384 core_models-0.4.7/core_models/app/managers/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-26 12:17:14.000000 core_models-0.4.7/core_models/app/managers/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6753 2024-01-26 07:37:49.000000 core_models-0.4.7/core_models/app/managers/notification_manager.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.761326 core_models-0.4.7/core_models/app/migrations/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8126 2023-04-19 22:19:11.000000 core_models-0.4.7/core_models/app/migrations/0001_initial.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      569 2023-04-19 22:36:45.000000 core_models-0.4.7/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-04-19 23:19:29.000000 core_models-0.4.7/core_models/app/migrations/0003_alter_user_onboarding_stage.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      586 2023-04-22 08:50:49.000000 core_models-0.4.7/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2143 2023-04-26 06:58:10.000000 core_models-0.4.7/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4814 2023-04-26 19:53:31.000000 core_models-0.4.7/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2747 2023-04-27 05:17:16.000000 core_models-0.4.7/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8196 2023-04-28 12:13:35.000000 core_models-0.4.7/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      682 2023-04-28 12:38:08.000000 core_models-0.4.7/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6021 2023-05-12 21:02:21.000000 core_models-0.4.7/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1269 2023-05-30 07:27:17.000000 core_models-0.4.7/core_models/app/migrations/0011_remove_invoice_draft_company_annual_turnover_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1806 2023-06-12 17:47:58.000000 core_models-0.4.7/core_models/app/migrations/0012_rename_amount_invoiceitem_total_invoice_discount_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     7281 2023-06-13 17:40:40.000000 core_models-0.4.7/core_models/app/migrations/0013_country_region_subregion_city_alter_company_city_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      362 2023-06-13 17:42:30.000000 core_models-0.4.7/core_models/app/migrations/0014_remove_company_city.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      483 2023-06-13 17:51:57.000000 core_models-0.4.7/core_models/app/migrations/0015_company_city.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3370 2023-07-04 13:26:12.000000 core_models-0.4.7/core_models/app/migrations/0016_sector_remove_company_industry_configuration_rpa_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      857 2023-07-04 22:55:41.000000 core_models-0.4.7/core_models/app/migrations/0017_alter_configuration_rpa.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      454 2023-07-05 15:16:17.000000 core_models-0.4.7/core_models/app/migrations/0018_invoice_rpa.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      391 2023-07-06 05:37:36.000000 core_models-0.4.7/core_models/app/migrations/0019_invoice_financed_on.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1965 2023-07-21 12:18:10.000000 core_models-0.4.7/core_models/app/migrations/0020_profileapplication.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      467 2023-07-26 23:45:53.000000 core_models-0.4.7/core_models/app/migrations/0021_profileapplication_company_registration_number.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      725 2023-07-26 23:47:54.000000 core_models-0.4.7/core_models/app/migrations/0022_otp.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      724 2023-08-11 08:23:32.000000 core_models-0.4.7/core_models/app/migrations/0023_alter_company_unique_together_country_oecd_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8112 2023-08-17 13:04:17.000000 core_models-0.4.7/core_models/app/migrations/0024_remove_profileapplication_export_countries_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1395 2023-08-17 17:10:24.000000 core_models-0.4.7/core_models/app/migrations/0025_remove_companyincorporation_team_chart_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      606 2023-08-17 17:12:22.000000 core_models-0.4.7/core_models/app/migrations/0026_companyincorporation_team_chart.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1124 2023-08-18 00:35:31.000000 core_models-0.4.7/core_models/app/migrations/0027_contractinformation_bank_statement_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1275 2023-09-04 17:16:28.000000 core_models-0.4.7/core_models/app/migrations/0028_profileapplication_company_incorporation_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1980 2023-09-10 15:26:07.000000 core_models-0.4.7/core_models/app/migrations/0029_remove_commercialinformation_credit_notes_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      609 2023-10-29 09:46:16.000000 core_models-0.4.7/core_models/app/migrations/0030_invoice_bill_of_lading_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2813 2023-11-10 08:01:25.000000 core_models-0.4.7/core_models/app/migrations/0031_bankaccount_account_type_bankaccount_currency_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      433 2023-11-13 09:50:20.000000 core_models-0.4.7/core_models/app/migrations/0032_invoice_decline_reason.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     5891 2023-11-22 12:08:55.000000 core_models-0.4.7/core_models/app/migrations/0033_invoicetransaction_payment_wallet_wallettransaction_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8243 2023-11-23 10:27:01.000000 core_models-0.4.7/core_models/app/migrations/0034_bankaccount_company_bankaccount_company_name_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1106 2023-11-23 14:23:47.000000 core_models-0.4.7/core_models/app/migrations/0035_remove_contractinformation_past_invoices_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      446 2023-11-29 13:26:38.000000 core_models-0.4.7/core_models/app/migrations/0036_contractinformation_completed.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      408 2023-12-03 23:48:45.000000 core_models-0.4.7/core_models/app/migrations/0037_bankaccount_status.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1693 2023-12-07 12:53:37.000000 core_models-0.4.7/core_models/app/migrations/0038_contract_percent_discount_alter_bankaccount_status_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1328 2023-12-07 13:01:46.000000 core_models-0.4.7/core_models/app/migrations/0039_baserate.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2074 2023-12-11 09:57:37.000000 core_models-0.4.7/core_models/app/migrations/0040_remove_contract_percent_discount_baserate_date_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      520 2023-12-22 15:09:48.000000 core_models-0.4.7/core_models/app/migrations/0041_company_logo.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1815 2024-01-10 08:36:44.000000 core_models-0.4.7/core_models/app/migrations/0042_contract_buyer_company_contract_seller_company_and_more.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-04-19 22:18:28.000000 core_models-0.4.7/core_models/app/migrations/__init__.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.769603 core_models-0.4.7/core_models/app/models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      828 2024-01-10 08:47:42.000000 core_models-0.4.7/core_models/app/models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1437 2024-03-07 16:28:18.000000 core_models-0.4.7/core_models/app/models/bank_account.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1755 2024-05-08 12:47:53.000000 core_models-0.4.7/core_models/app/models/base.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      382 2023-12-11 06:52:11.000000 core_models-0.4.7/core_models/app/models/base_rate.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8327 2024-02-23 09:26:48.000000 core_models-0.4.7/core_models/app/models/company.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      686 2024-01-10 08:35:27.000000 core_models-0.4.7/core_models/app/models/company_configuration.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1254 2023-12-01 07:33:10.000000 core_models-0.4.7/core_models/app/models/configuration.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     7512 2024-05-08 09:35:19.000000 core_models-0.4.7/core_models/app/models/contract.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      670 2023-08-11 08:18:07.000000 core_models-0.4.7/core_models/app/models/country.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      591 2023-05-12 19:41:41.000000 core_models-0.4.7/core_models/app/models/currency.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     9862 2024-04-10 11:27:22.000000 core_models-0.4.7/core_models/app/models/invoice.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1472 2024-04-01 15:16:47.000000 core_models-0.4.7/core_models/app/models/notification.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1231 2023-07-27 06:25:34.000000 core_models-0.4.7/core_models/app/models/otp.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1700 2023-11-23 14:04:30.000000 core_models-0.4.7/core_models/app/models/payment.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4203 2024-04-10 11:23:01.000000 core_models-0.4.7/core_models/app/models/profile_application.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      272 2023-07-04 13:25:19.000000 core_models-0.4.7/core_models/app/models/sector.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2293 2024-02-23 09:26:48.000000 core_models-0.4.7/core_models/app/models/user.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      528 2023-11-08 09:07:59.000000 core_models-0.4.7/core_models/app/models/verto_config.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     2775 2024-01-17 09:04:48.000000 core_models-0.4.7/core_models/app/models/wallet.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1515 2023-12-04 09:27:57.000000 core_models-0.4.7/core_models/app/models/withdrawal.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.705963 core_models-0.4.7/core_models/app/templates/
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.770444 core_models-0.4.7/core_models/app/templates/core_models/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    15502 2024-04-17 08:47:42.000000 core_models-0.4.7/core_models/app/templates/core_models/mail-base.html
+-rw-r--r--   0 macbookpro   (501) staff       (20)      637 2024-04-17 08:47:42.000000 core_models-0.4.7/core_models/app/templates/core_models/mail-base.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3182 2023-06-12 14:08:46.000000 core_models-0.4.7/core_models/base_views.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6516 2024-03-28 12:35:04.000000 core_models-0.4.7/core_models/constants.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     4433 2023-04-18 15:27:44.000000 core_models-0.4.7/core_models/settings.example.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8224 2024-02-28 09:49:58.000000 core_models-0.4.7/core_models/settings.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3469 2024-02-28 09:49:58.000000 core_models-0.4.7/core_models/utils.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2024-05-08 13:22:48.770882 core_models-0.4.7/core_models.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      910 2024-05-08 13:22:48.000000 core_models-0.4.7/core_models.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     5135 2024-05-08 13:22:48.000000 core_models-0.4.7/core_models.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2024-05-08 13:22:48.000000 core_models-0.4.7/core_models.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      233 2024-05-08 13:22:48.000000 core_models-0.4.7/core_models.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       12 2024-05-08 13:22:48.000000 core_models-0.4.7/core_models.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 core_models-0.4.7/pyproject.toml
+-rw-r--r--   0 macbookpro   (501) staff       (20)       38 2024-05-08 13:22:48.772026 core_models-0.4.7/setup.cfg
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1268 2024-05-08 09:35:19.000000 core_models-0.4.7/setup.py
```

### Comparing `core_models-0.4.6/LICENSE` & `core_models-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/PKG-INFO` & `core_models-0.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core_models
-Version: 0.4.6
+Version: 0.4.7
 Summary: Liquify core package
 Author: Folayemi Bello
 Author-email: <bello.folayemi.az@gmail.com>
 Keywords: python,liquify
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `core_models-0.4.6/README.md` & `core_models-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/api_response.py` & `core_models-0.4.7/core_models/api_response.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/admin.py` & `core_models-0.4.7/core_models/app/admin.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/integrations/verto/add_beneficiary.py` & `core_models-0.4.7/core_models/app/integrations/verto/add_beneficiary.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/integrations/verto/create_fx_trade.py` & `core_models-0.4.7/core_models/app/integrations/verto/create_fx_trade.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/integrations/verto/create_payment.py` & `core_models-0.4.7/core_models/app/integrations/verto/create_payment.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/integrations/verto/get_currencies.py` & `core_models-0.4.7/core_models/app/integrations/verto/get_currencies.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/integrations/verto/get_fx_rate.py` & `core_models-0.4.7/core_models/app/integrations/verto/get_fx_rate.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/integrations/verto/get_purposes.py` & `core_models-0.4.7/core_models/app/integrations/verto/get_purposes.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/integrations/verto/get_wallets.py` & `core_models-0.4.7/core_models/app/integrations/verto/get_wallets.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/integrations/verto/login.py` & `core_models-0.4.7/core_models/app/integrations/verto/login.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/managers/notification_manager.py` & `core_models-0.4.7/core_models/app/managers/notification_manager.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0001_initial.py` & `core_models-0.4.7/core_models/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py` & `core_models-0.4.7/core_models/app/migrations/0002_alter_user_name_alter_user_phone_number.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py` & `core_models-0.4.7/core_models/app/migrations/0004_user_reset_token_user_reset_token_expiry.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0005_remove_bankaccount_user_remove_user_name_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py` & `core_models-0.4.7/core_models/app/migrations/0006_currency_invoice_alter_company_options_invoiceitem.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0007_remove_invoice_paid_invoice_status_invoice_subtotal_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0008_alter_contract_options_contract_status_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py` & `core_models-0.4.7/core_models/app/migrations/0009_alter_currency_options_alter_companydocument_company.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0010_rename_discount_invoice_interest_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0011_remove_invoice_draft_company_annual_turnover_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0011_remove_invoice_draft_company_annual_turnover_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0012_rename_amount_invoiceitem_total_invoice_discount_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0012_rename_amount_invoiceitem_total_invoice_discount_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0013_country_region_subregion_city_alter_company_city_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0013_country_region_subregion_city_alter_company_city_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0016_sector_remove_company_industry_configuration_rpa_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0016_sector_remove_company_industry_configuration_rpa_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0017_alter_configuration_rpa.py` & `core_models-0.4.7/core_models/app/migrations/0017_alter_configuration_rpa.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0020_profileapplication.py` & `core_models-0.4.7/core_models/app/migrations/0020_profileapplication.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0022_otp.py` & `core_models-0.4.7/core_models/app/migrations/0022_otp.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0023_alter_company_unique_together_country_oecd_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0023_alter_company_unique_together_country_oecd_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0024_remove_profileapplication_export_countries_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0024_remove_profileapplication_export_countries_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0025_remove_companyincorporation_team_chart_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0025_remove_companyincorporation_team_chart_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0026_companyincorporation_team_chart.py` & `core_models-0.4.7/core_models/app/migrations/0026_companyincorporation_team_chart.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0027_contractinformation_bank_statement_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0027_contractinformation_bank_statement_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0028_profileapplication_company_incorporation_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0028_profileapplication_company_incorporation_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0029_remove_commercialinformation_credit_notes_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0029_remove_commercialinformation_credit_notes_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0030_invoice_bill_of_lading_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0030_invoice_bill_of_lading_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0031_bankaccount_account_type_bankaccount_currency_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0031_bankaccount_account_type_bankaccount_currency_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0033_invoicetransaction_payment_wallet_wallettransaction_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0033_invoicetransaction_payment_wallet_wallettransaction_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0034_bankaccount_company_bankaccount_company_name_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0034_bankaccount_company_bankaccount_company_name_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0035_remove_contractinformation_past_invoices_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0035_remove_contractinformation_past_invoices_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0038_contract_percent_discount_alter_bankaccount_status_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0038_contract_percent_discount_alter_bankaccount_status_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0039_baserate.py` & `core_models-0.4.7/core_models/app/migrations/0039_baserate.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0040_remove_contract_percent_discount_baserate_date_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0040_remove_contract_percent_discount_baserate_date_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0041_company_logo.py` & `core_models-0.4.7/core_models/app/migrations/0041_company_logo.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/migrations/0042_contract_buyer_company_contract_seller_company_and_more.py` & `core_models-0.4.7/core_models/app/migrations/0042_contract_buyer_company_contract_seller_company_and_more.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/__init__.py` & `core_models-0.4.7/core_models/app/models/__init__.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/bank_account.py` & `core_models-0.4.7/core_models/app/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/base.py` & `core_models-0.4.7/core_models/app/models/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,20 +29,17 @@
         self.deletedBy = None
         self.deleted = False
         return super(BaseModelAbstract, self).undelete(force_policy, **kwargs)
 
     def __str__(self):
         return self.__unicode__()
 
-    @property
-    def is_fully_filled(self):
+    def is_fully_filled(self, exempt):
         ''' Checks if all the fields have been filled '''
         all_fields_names = [f.name for f in self._meta.get_fields()]
-        exempt = ['deleted', 'deleted_by_id', 'deleted_at', 'created_at',
-                  'updated_at', 'is_test', 'company']
         fields_names = set(all_fields_names).difference(set(exempt))
         print(['fields_names', fields_names])
 
         for field_name in fields_names:
             if hasattr(self, field_name):
                 value = getattr(self, field_name)
                 if value is None or value == '':
```

### Comparing `core_models-0.4.6/core_models/app/models/company.py` & `core_models-0.4.7/core_models/app/models/company.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/company_configuration.py` & `core_models-0.4.7/core_models/app/models/company_configuration.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/configuration.py` & `core_models-0.4.7/core_models/app/models/configuration.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/contract.py` & `core_models-0.4.7/core_models/app/models/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
                               choices=constants.CONTRACT_STATUSES,
                               default=constants.PENDING_CONTRACT_STATUS)
     buyer_accepted_on = models.DateTimeField(null=True, blank=True)
     buyer_accepted_via = models.CharField(
         max_length=1, choices=constants.CONTRACT_ACCEPTANCE_CHANNELS,
         null=True, blank=True
     )
+    require_buyer_invoice_approval = models.BooleanField(default=True)
     tracker = FieldTracker(fields=['status'])
 
     def get_absolute_url(self):
         return reverse(
             "sellers:contract-detail",
             kwargs={'pk': self.pk}
         )
```

### Comparing `core_models-0.4.6/core_models/app/models/country.py` & `core_models-0.4.7/core_models/app/models/country.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/currency.py` & `core_models-0.4.7/core_models/app/models/currency.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/invoice.py` & `core_models-0.4.7/core_models/app/models/invoice.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/notification.py` & `core_models-0.4.7/core_models/app/models/notification.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/otp.py` & `core_models-0.4.7/core_models/app/models/otp.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/payment.py` & `core_models-0.4.7/core_models/app/models/payment.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/profile_application.py` & `core_models-0.4.7/core_models/app/models/profile_application.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/user.py` & `core_models-0.4.7/core_models/app/models/user.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/verto_config.py` & `core_models-0.4.7/core_models/app/models/verto_config.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/wallet.py` & `core_models-0.4.7/core_models/app/models/wallet.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/models/withdrawal.py` & `core_models-0.4.7/core_models/app/models/withdrawal.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/app/templates/core_models/mail-base.html` & `core_models-0.4.7/core_models/app/templates/core_models/mail-base.html`

 * *Files 0% similar despite different names*

```diff
@@ -470,16 +470,16 @@
                             <table class="email-body_inner" align="center" width="570" cellpadding="0" cellspacing="0" role="presentation">
                                 <!-- Body content -->
                                 <tr>
                                     <td class="content-cell">
                                         <div class="f-fallback">
                                             {% block content %}{% endblock %}
                                             <p>If you have any questions, feel free to <a href="mailto:inquiries@liquify.digital">email
-                                                our customer success team</a>. (We're lightning quick at replying.) We also
-                                                offer <a href="#">live chat</a> during business hours.</p>
+                                                our customer success team</a>.
+                                            </p>
                                             <p>Thanks,
                                                 <br>
                                                 {{ EMAIL_SIGNATURE }}
                                             </p>
                                             <p><strong>P.S.</strong> Need immediate help getting started? Check out our <a
                                                     href="https://liquify.digital/help">help documentation</a>.</p>
                                             {% if action_url %}
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
 {% block preheader %}{% endblock %}
 _L_i_q_u_i_f_y
 {% block content %}{% endblock %}
-If you have any questions, feel free to _e_m_a_i_l_ _o_u_r_ _c_u_s_t_o_m_e_r_ _s_u_c_c_e_s_s_ _t_e_a_m. (We're
-lightning quick at replying.) We also offer _l_i_v_e_ _c_h_a_t during business hours.
+If you have any questions, feel free to _e_m_a_i_l_ _o_u_r_ _c_u_s_t_o_m_e_r_ _s_u_c_c_e_s_s_ _t_e_a_m.
 Thanks,
 {{ EMAIL_SIGNATURE }}
 PP..SS.. Need immediate help getting started? Check out our _h_e_l_p_ _d_o_c_u_m_e_n_t_a_t_i_o_n.
 {% if action_url %}
 If you’re having trouble with the button above, copy and paste the URL below
 into your web browser.
 {{ action_url }}
 {% endif %}
-           Liquify Digital LTD © {% now 'Y' %} All rights reserved.
-                                71-91 Aldwych,
-                               London WC2B 4HN
-                                United Kingdom
-             This is an auto-generated mail, please do not reply!
+         Liquify Digital LTD © {% now 'Y' %} All rights reserved.
+                              71-91 Aldwych,
+                             London WC2B 4HN
+                              United Kingdom
+           This is an auto-generated mail, please do not reply!
```

### Comparing `core_models-0.4.6/core_models/app/templates/core_models/mail-base.txt` & `core_models-0.4.7/core_models/app/templates/core_models/mail-base.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% block preheader %}{% endblock %}
 
 Liquify ( https://liquify.digital )
 
 {% block content %}{% endblock %}
 
-If you have any questions, feel free to email our customer success team ( inquiries@liquify.digital ). (We're lightning quick at replying.) We also offer live chat ( https://liquify.digital} ) during business hours.
+If you have any questions, feel free to email our customer success team ( inquiries@liquify.digital ).
 
 Thanks,
 Nadya and the Liquify team
 
 P.S. Need immediate help getting started? Check out our help documentation ( https://liquify.digital/help ).
 {% if action_url %}
```

### Comparing `core_models-0.4.6/core_models/base_views.py` & `core_models-0.4.7/core_models/base_views.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/constants.py` & `core_models-0.4.7/core_models/constants.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/settings.example.py` & `core_models-0.4.7/core_models/settings.example.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/settings.py` & `core_models-0.4.7/core_models/settings.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models/utils.py` & `core_models-0.4.7/core_models/utils.py`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/core_models.egg-info/PKG-INFO` & `core_models-0.4.7/core_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core_models
-Version: 0.4.6
+Version: 0.4.7
 Summary: Liquify core package
 Author: Folayemi Bello
 Author-email: <bello.folayemi.az@gmail.com>
 Keywords: python,liquify
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `core_models-0.4.6/core_models.egg-info/SOURCES.txt` & `core_models-0.4.7/core_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core_models-0.4.6/setup.py` & `core_models-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.4.6'
+VERSION = '0.4.7'
 DESCRIPTION = 'Liquify core package'
 LONG_DESCRIPTION = 'Package that holds all models and core ' \
                    'functions/classes of Liquify project'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
```
